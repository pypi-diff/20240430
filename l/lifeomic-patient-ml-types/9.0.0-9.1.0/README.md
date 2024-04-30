# Comparing `tmp/lifeomic_patient_ml_types-9.0.0.tar.gz` & `tmp/lifeomic_patient_ml_types-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeomic_patient_ml_types-9.0.0.tar", max compression
+gzip compressed data, was "lifeomic_patient_ml_types-9.1.0.tar", max compression
```

## Comparing `lifeomic_patient_ml_types-9.0.0.tar` & `lifeomic_patient_ml_types-9.1.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    18241 2023-09-29 13:35:56.963147 lifeomic_patient_ml_types-9.0.0/lifeomic_patient_ml_types/schemas.py
--rw-r--r--   0        0        0      965 2023-09-29 13:37:09.292130 lifeomic_patient_ml_types-9.0.0/pyproject.toml
--rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-9.0.0/setup.py
--rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-9.0.0/PKG-INFO
+-rw-r--r--   0        0        0    16910 2024-04-30 18:15:45.387156 lifeomic_patient_ml_types-9.1.0/lifeomic_patient_ml_types/schemas.py
+-rw-r--r--   0        0        0      970 2024-04-30 18:17:02.335293 lifeomic_patient_ml_types-9.1.0/pyproject.toml
+-rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-9.1.0/setup.py
+-rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-9.1.0/PKG-INFO
```

### Comparing `lifeomic_patient_ml_types-9.0.0/lifeomic_patient_ml_types/schemas.py` & `lifeomic_patient_ml_types-9.1.0/lifeomic_patient_ml_types/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -346,59 +346,22 @@
     type: Literal["cloud"]
 
 
 class DeployApproach(BaseModel):
     __root__: Union[EdgeDeployApproach, CloudDeployApproach]
 
 
-class EvaluationApproach(BaseModel):
-    class Config:
-        extra = Extra.forbid
-
-    type: Literal["customImage"]
-    imageUri: str = Field(
-        ...,
-        regex="^[0-9]+\\.dkr.ecr.[-a-z0-9]+\\.amazonaws\\.com\\/[-_a-zA-Z0-9]+:[-_a-zA-Z0-9]+$",
-    )
-    """
-    An aws ecr image uri of the form <account-id>.dkr.ecr.<region>.amazonaws.com/<repo-name>:<tag>
-    """
-
-
 class ModelConfigBase(BaseModel):
     class Config:
         extra = Extra.allow
 
     name: str
     description: str
     trainingApproach: TrainingApproach
     deployApproach: DeployApproach
-    evaluationApproach: Optional[EvaluationApproach] = None
-
-
-class Split(BaseModel):
-    class Config:
-        extra = Extra.forbid
-
-    n: float
-    """
-    The number of examples in this split.
-    """
-    start: float
-    """
-    Timestamp marking the beginning of the data for this split (inclusive). Expressed as milliseconds since the UTC epoch.
-    """
-    end: float
-    """
-    Timestamp marking the end of the data for this split (exclusive). Expressed as milliseconds since the UTC epoch.
-    """
-    uri: str = Field(..., regex="^s3:\\/\\/.+$")
-    """
-    S3 URI of where a copy of this exact split is saved.
-    """
 
 
 class Metric(BaseModel):
     class Config:
         extra = Extra.forbid
 
     name: str
@@ -408,15 +371,15 @@
     description: Optional[str] = None
     """
     A description of the metric to help people understand what it means and represents.
     """
     value: float
     stage: Literal["training", "evaluation"]
     """
-    The stage of the model run this metric was computed in. If `training`, the metric could have been computed over the train or val set. If `evaluation`, the metric was computed over the test set.
+    @deprecated The stage of the model run this metric was computed in. If `training`, the metric could have been computed over the train or val set. If `evaluation`, the metric was computed over the test set.
     """
     direction: Optional[OptimizationDirection] = None
     """
     The optimization direction for this metric. E.g. `minimize` means a smaller value for this metric is better. This direction is just used as metadata about the metric value, and does not mean this metric will be optimized during hyperparameter tuning.
     """
 
 
@@ -452,27 +415,14 @@
     user: str
 
 
 class ApprovalDecision(BaseModel):
     __root__: Union[SystemApprovalDecision, UserApprovalDecision]
 
 
-class RunSplits(BaseModel):
-    """
-    Information about the different splits of the dataset used to train this model version.
-    """
-
-    class Config:
-        extra = Extra.forbid
-
-    train: Split
-    val: Split
-    test: Split
-
-
 class RunMetrics(BaseModel):
     class Config:
         extra = Extra.forbid
 
     challenger: List[Metric]
     """
     Metrics about how the model version trained in this run (the challenger) performed on this run's test set.
@@ -696,15 +646,14 @@
     """
     Timestamp of when the run ended. Expressed as milliseconds since the UTC epoch.
     """
     isArchived: Optional[bool] = None
     """
     True if this run has been archived. Archived runs' related artifacts are deleted, and they can no longer be deployed.
     """
-    splits: Optional[RunSplits] = None
     hyperparameters: List[Parameter]
     """
     The hyperparameters used to train the model version created by this run.
     """
     championId: Optional[str] = None
     """
     The ID of the model run that was the current champion while this model run was running. All champion metrics on this model run represent that champion's performance on this run's dataset.
@@ -713,8 +662,7 @@
     approvals: List[ApprovalDecision]
     """
     Decisions made by various actors representing whether they think this model version should be used in production and become the new champion.
     """
     problemDefinition: MlProblemDefinition
     trainingApproach: TrainingApproach
     deployApproach: DeployApproach
-    evaluationApproach: Optional[EvaluationApproach] = None
```

### Comparing `lifeomic_patient_ml_types-9.0.0/setup.py` & `lifeomic_patient_ml_types-9.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['lifeomic_patient_ml_types']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'lifeomic-patient-ml-types',
-    'version': '9.0.0',
+    'version': '9.1.0',
     'description': 'Shared types for the patient-ml-service repos.',
     'long_description': 'None',
     'author': 'LifeOmic',
     'author_email': 'development@lifeomic.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

