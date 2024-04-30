# Comparing `tmp/kodexa-7.0.8801100838.tar.gz` & `tmp/kodexa-7.0.8895840398.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa-7.0.8801100838.tar", max compression
+gzip compressed data, was "kodexa-7.0.8895840398.tar", max compression
```

## Comparing `kodexa-7.0.8801100838.tar` & `kodexa-7.0.8895840398.tar`

### file list

```diff
@@ -1,41 +1,43 @@
--rw-r--r--   0        0        0    11357 2024-04-23 13:16:15.353844 kodexa-7.0.8801100838/LICENSE
--rw-r--r--   0        0        0     2178 2024-04-23 13:16:15.353844 kodexa-7.0.8801100838/README.md
--rw-r--r--   0        0        0      957 2024-04-23 13:16:15.357843 kodexa-7.0.8801100838/kodexa/__init__.py
--rw-r--r--   0        0        0      171 2024-04-23 13:16:15.357843 kodexa-7.0.8801100838/kodexa/assistant/__init__.py
--rw-r--r--   0        0        0    14663 2024-04-23 13:16:15.357843 kodexa-7.0.8801100838/kodexa/assistant/assistant.py
--rw-r--r--   0        0        0      328 2024-04-23 13:16:15.357843 kodexa-7.0.8801100838/kodexa/connectors/__init__.py
--rw-r--r--   0        0        0    10413 2024-04-23 13:16:15.357843 kodexa-7.0.8801100838/kodexa/connectors/connectors.py
--rw-r--r--   0        0        0      796 2024-04-23 13:16:15.357843 kodexa-7.0.8801100838/kodexa/model/__init__.py
--rw-r--r--   0        0        0      521 2024-04-23 13:16:15.357843 kodexa-7.0.8801100838/kodexa/model/base.py
--rw-r--r--   0        0        0   115528 2024-04-23 13:16:15.357843 kodexa-7.0.8801100838/kodexa/model/model.py
--rw-r--r--   0        0        0   175434 2024-04-23 13:16:15.361843 kodexa-7.0.8801100838/kodexa/model/objects.py
--rw-r--r--   0        0        0    62032 2024-04-23 13:16:15.361843 kodexa-7.0.8801100838/kodexa/model/persistence.py
--rw-r--r--   0        0        0      236 2024-04-23 13:16:15.361843 kodexa-7.0.8801100838/kodexa/pipeline/__init__.py
--rw-r--r--   0        0        0    25221 2024-04-23 13:16:15.361843 kodexa-7.0.8801100838/kodexa/pipeline/pipeline.py
--rw-r--r--   0        0        0      216 2024-04-23 13:16:15.361843 kodexa-7.0.8801100838/kodexa/platform/__init__.py
--rw-r--r--   0        0        0   213407 2024-04-23 13:16:15.361843 kodexa-7.0.8801100838/kodexa/platform/client.py
--rw-r--r--   0        0        0     1055 2024-04-23 13:16:15.361843 kodexa-7.0.8801100838/kodexa/platform/interaction.py
--rw-r--r--   0        0        0    34024 2024-04-23 13:16:15.361843 kodexa-7.0.8801100838/kodexa/platform/kodexa.py
--rw-r--r--   0        0        0      100 2024-04-23 13:16:15.361843 kodexa-7.0.8801100838/kodexa/selectors/__init__.py
--rw-r--r--   0        0        0    13269 2024-04-23 13:16:15.361843 kodexa-7.0.8801100838/kodexa/selectors/ast.py
--rw-r--r--   0        0        0     3691 2024-04-23 13:16:15.361843 kodexa-7.0.8801100838/kodexa/selectors/core.py
--rw-r--r--   0        0        0     3447 2024-04-23 13:16:15.361843 kodexa-7.0.8801100838/kodexa/selectors/lexrules.py
--rw-r--r--   0        0        0     3155 2024-04-23 13:16:15.361843 kodexa-7.0.8801100838/kodexa/selectors/lextab.py
--rw-r--r--   0        0        0       61 2024-04-23 13:16:15.361843 kodexa-7.0.8801100838/kodexa/selectors/lextab.pyi
--rw-r--r--   0        0        0     7068 2024-04-23 13:16:15.361843 kodexa-7.0.8801100838/kodexa/selectors/parserules.py
--rw-r--r--   0        0        0       61 2024-04-23 13:16:15.361843 kodexa-7.0.8801100838/kodexa/selectors/parserules.pyi
--rw-r--r--   0        0        0    71452 2024-04-23 13:16:15.361843 kodexa-7.0.8801100838/kodexa/selectors/parsetab.py
--rw-r--r--   0        0        0       61 2024-04-23 13:16:15.361843 kodexa-7.0.8801100838/kodexa/selectors/parsetab.pyi
--rw-r--r--   0        0        0        0 2024-04-23 13:16:15.361843 kodexa-7.0.8801100838/kodexa/spatial/__init__.py
--rw-r--r--   0        0        0    30564 2024-04-23 13:16:15.361843 kodexa-7.0.8801100838/kodexa/spatial/azure_models.py
--rw-r--r--   0        0        0     5975 2024-04-23 13:16:15.361843 kodexa-7.0.8801100838/kodexa/spatial/bbox_common.py
--rw-r--r--   0        0        0    44214 2024-04-23 13:16:15.361843 kodexa-7.0.8801100838/kodexa/spatial/table_form_common.py
--rw-r--r--   0        0        0      179 2024-04-23 13:16:15.361843 kodexa-7.0.8801100838/kodexa/steps/__init__.py
--rw-r--r--   0        0        0    10428 2024-04-23 13:16:15.361843 kodexa-7.0.8801100838/kodexa/steps/common.py
--rw-r--r--   0        0        0      323 2024-04-23 13:16:15.361843 kodexa-7.0.8801100838/kodexa/testing/__init__.py
--rw-r--r--   0        0        0     1052 2024-04-23 13:16:15.361843 kodexa-7.0.8801100838/kodexa/testing/test_components.py
--rw-r--r--   0        0        0    14021 2024-04-23 13:16:15.361843 kodexa-7.0.8801100838/kodexa/testing/test_utils.py
--rw-r--r--   0        0        0       52 2024-04-23 13:16:15.361843 kodexa-7.0.8801100838/kodexa/training/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 13:16:15.361843 kodexa-7.0.8801100838/kodexa/training/train_utils.py
--rw-r--r--   0        0        0     1389 2024-04-23 13:16:34.449842 kodexa-7.0.8801100838/pyproject.toml
--rw-r--r--   0        0        0     3493 1970-01-01 00:00:00.000000 kodexa-7.0.8801100838/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-30 13:41:16.794320 kodexa-7.0.8895840398/LICENSE
+-rw-r--r--   0        0        0     2178 2024-04-30 13:41:16.794320 kodexa-7.0.8895840398/README.md
+-rw-r--r--   0        0        0      957 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/__init__.py
+-rw-r--r--   0        0        0      171 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/assistant/__init__.py
+-rw-r--r--   0        0        0    14663 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/assistant/assistant.py
+-rw-r--r--   0        0        0      328 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/connectors/__init__.py
+-rw-r--r--   0        0        0    10413 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/connectors/connectors.py
+-rw-r--r--   0        0        0      796 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/model/__init__.py
+-rw-r--r--   0        0        0      521 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/model/base.py
+-rw-r--r--   0        0        0     3592 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/model/entities/product.py
+-rw-r--r--   0        0        0     3873 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/model/entities/product_subscription.py
+-rw-r--r--   0        0        0   115561 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/model/model.py
+-rw-r--r--   0        0        0   175470 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/model/objects.py
+-rw-r--r--   0        0        0    62032 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/model/persistence.py
+-rw-r--r--   0        0        0      236 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/pipeline/__init__.py
+-rw-r--r--   0        0        0    25221 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/pipeline/pipeline.py
+-rw-r--r--   0        0        0      216 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/platform/__init__.py
+-rw-r--r--   0        0        0   214979 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/platform/client.py
+-rw-r--r--   0        0        0     1055 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/platform/interaction.py
+-rw-r--r--   0        0        0    34024 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/platform/kodexa.py
+-rw-r--r--   0        0        0      100 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/selectors/__init__.py
+-rw-r--r--   0        0        0    13269 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/selectors/ast.py
+-rw-r--r--   0        0        0     3691 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/selectors/core.py
+-rw-r--r--   0        0        0     3447 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/selectors/lexrules.py
+-rw-r--r--   0        0        0     3155 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/selectors/lextab.py
+-rw-r--r--   0        0        0       61 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/selectors/lextab.pyi
+-rw-r--r--   0        0        0     7068 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/selectors/parserules.py
+-rw-r--r--   0        0        0       61 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/selectors/parserules.pyi
+-rw-r--r--   0        0        0    71452 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/selectors/parsetab.py
+-rw-r--r--   0        0        0       61 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/selectors/parsetab.pyi
+-rw-r--r--   0        0        0        0 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/spatial/__init__.py
+-rw-r--r--   0        0        0    30564 2024-04-30 13:41:16.806320 kodexa-7.0.8895840398/kodexa/spatial/azure_models.py
+-rw-r--r--   0        0        0     5975 2024-04-30 13:41:16.806320 kodexa-7.0.8895840398/kodexa/spatial/bbox_common.py
+-rw-r--r--   0        0        0    44214 2024-04-30 13:41:16.806320 kodexa-7.0.8895840398/kodexa/spatial/table_form_common.py
+-rw-r--r--   0        0        0      179 2024-04-30 13:41:16.806320 kodexa-7.0.8895840398/kodexa/steps/__init__.py
+-rw-r--r--   0        0        0    10428 2024-04-30 13:41:16.806320 kodexa-7.0.8895840398/kodexa/steps/common.py
+-rw-r--r--   0        0        0      323 2024-04-30 13:41:16.806320 kodexa-7.0.8895840398/kodexa/testing/__init__.py
+-rw-r--r--   0        0        0     1052 2024-04-30 13:41:16.806320 kodexa-7.0.8895840398/kodexa/testing/test_components.py
+-rw-r--r--   0        0        0    14021 2024-04-30 13:41:16.806320 kodexa-7.0.8895840398/kodexa/testing/test_utils.py
+-rw-r--r--   0        0        0       52 2024-04-30 13:41:16.806320 kodexa-7.0.8895840398/kodexa/training/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 13:41:16.806320 kodexa-7.0.8895840398/kodexa/training/train_utils.py
+-rw-r--r--   0        0        0     1389 2024-04-30 13:41:34.238227 kodexa-7.0.8895840398/pyproject.toml
+-rw-r--r--   0        0        0     3493 1970-01-01 00:00:00.000000 kodexa-7.0.8895840398/PKG-INFO
```

### Comparing `kodexa-7.0.8801100838/LICENSE` & `kodexa-7.0.8895840398/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8801100838/README.md` & `kodexa-7.0.8895840398/README.md`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8801100838/kodexa/__init__.py` & `kodexa-7.0.8895840398/kodexa/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8801100838/kodexa/assistant/assistant.py` & `kodexa-7.0.8895840398/kodexa/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8801100838/kodexa/connectors/connectors.py` & `kodexa-7.0.8895840398/kodexa/connectors/connectors.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8801100838/kodexa/model/__init__.py` & `kodexa-7.0.8895840398/kodexa/model/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8801100838/kodexa/model/base.py` & `kodexa-7.0.8895840398/kodexa/model/base.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8801100838/kodexa/model/model.py` & `kodexa-7.0.8895840398/kodexa/model/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -2627,26 +2627,26 @@
           the document
 
         """
         self.labels.remove(label)
         return self
 
     @classmethod
-    def from_text(cls, text, separator=None):
+    def from_text(cls, text, separator=None, inmemory=False):
         """Creates a new Document from the text provided.
 
         Args:
           text: str  Text to be used as content on the Document's ContentNode(s)
           separator: str   If provided, this string will be used to split the text and the resulting text will be placed on children of the root ContentNode. (Default value = None)
 
         Returns:
           the document
 
         """
-        new_document = Document()
+        new_document = Document(inmemory=inmemory)
         new_document.source.original_filename = f"text-{uuid.uuid4()}"
         new_document.content_node = new_document.create_node(node_type="text", index=0)
         if text:
             if separator:
                 for s in text.split(separator):
                     new_document.content_node.add_child(
                         new_document.create_node(node_type="text", content=s)
```

### Comparing `kodexa-7.0.8801100838/kodexa/model/objects.py` & `kodexa-7.0.8895840398/kodexa/model/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -671,17 +671,16 @@
 
     """
     operational = "OPERATIONAL"
     training = "TRAINING"
 
 
 class ProjectStoreFile(BaseModel):
-
     url: Optional[str] = None
-    metadata: Optional[Dict[str,str]] = None
+    metadata: Optional[Dict[str, str]] = None
 
 
 class ProjectStore(BaseModel):
     """
 
     """
     model_config = ConfigDict(
@@ -1768,14 +1767,15 @@
     max_replicas: Optional[int] = Field(None, alias="maxReplicas")
     min_replicas: Optional[int] = Field(None, alias="minReplicas")
     reserved_concurrency: Optional[int] = Field(None, alias="reservedConcurrency")
     memory_assigned: Optional[str] = Field(None, alias="memoryAssigned")
     cpu: Optional[str] = None
     pod_match_labels: Optional[List[MatchLabel]] = Field(None, alias="podMatchLabels")
     child_process: Optional[bool] = Field(None, alias="childProcess")
+    layers: Optional[List[str]] = None
 
 
 class SourceType(Enum):
     """
 
     """
     data_object = "DATA_OBJECT"
@@ -2486,29 +2486,27 @@
     show_in_training: Optional[bool] = Field(None, alias="showInTraining")
     priority_hint: Optional[int] = Field(None, alias="priorityHint")
     chat_enabled: Optional[bool] = Field(None, alias="chatEnabled")
     assistant_role: Optional[str] = Field(None, alias="assistantRole")
 
 
 class TaxonConditionalFormat(BaseModel):
-
     model_config = ConfigDict(
         populate_by_name=True,
         use_enum_values=True,
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
 
     type: Optional[str] = None
     condition: Optional[str] = None
     properties: Optional[Dict[str, Any]] = Field(default_factory=dict)
 
 
 class TaxonCardinality(Enum):
-
     once_per_document = "ONCE_PER_DOCUMENT"
     multiple_per_document = "MULTIPLE_PER_DOCUMENT"
     once_per_segment = "ONCE_PER_SEGMENT"
     multiple_per_segment = "MULTIPLE_PER_SEGMENT"
 
 
 class Taxon(BaseModel):
@@ -2805,15 +2803,14 @@
     status: Optional[str] = Field(None, description="The status of the project")
     color: Optional[str] = None
     organization: Organization
     icon: Optional[str] = None
 
 
 class ProjectOptions(BaseModel):
-
     model_config = ConfigDict(
         populate_by_name=True,
         use_enum_values=True,
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
 
@@ -3836,15 +3833,14 @@
         None,
         alias="minLabelConfidence",
         description="The minimum confidence of each label in the document",
     )
 
 
 class DocumentEmbedding(BaseModel):
-
     model_config = ConfigDict(
         populate_by_name=True,
         use_enum_values=True,
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
     embedding: Optional[List[float]] = None
@@ -4070,14 +4066,15 @@
     definition: Optional[AssistantDefinition] = None
     show_in_training: Optional[bool] = Field(None, alias="showInTraining")
     color: Optional[str] = Field(None, description="The color to use for the assistant")
     priority_hint: Optional[int] = Field(None, alias="priorityHint")
     chat_enabled: Optional[bool] = Field(None, alias="chatEnabled")
     assistant_role: Optional[str] = Field(None, alias="assistantRole")
 
+
 class AssistantExecution(BaseModel):
     """
 
     """
     model_config = ConfigDict(
         populate_by_name=True,
         use_enum_values=True,
@@ -4335,14 +4332,15 @@
     # users selected text, text and line_uuid
     user_selection: Optional[List[UserSelection]] = Field(None, alias="userSelection")
 
     compiled_guidance: Optional[Dict[str, Any]] = Field(None, alias="compiledGuidance")
 
     guidance_options: Optional[List[Option]] = Field(None, alias="guidanceOptions")
 
+
 class GuidanceSet(ExtensionPackProvided):
     """
 
     """
     guidance: List[Guidance] = Field(None, description="The guidance in the set")
 
 
@@ -5258,15 +5256,14 @@
     """
 
     """
     metadata: Optional[PipelineImplementationMetadata] = None
 
 
 class ProjectTemplate(ExtensionPackProvided):
-
     stores: Optional[List[ProjectStore]] = Field(
         None, description="The stores that will be created with the project template"
     )
     assistants: Optional[List[ProjectAssistant]] = Field(
         None,
         description="The assistants that will be created with the project template",
     )
```

### Comparing `kodexa-7.0.8801100838/kodexa/model/persistence.py` & `kodexa-7.0.8895840398/kodexa/model/persistence.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8801100838/kodexa/pipeline/pipeline.py` & `kodexa-7.0.8895840398/kodexa/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8801100838/kodexa/platform/client.py` & `kodexa-7.0.8895840398/kodexa/platform/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1594,14 +1594,50 @@
         Get the taxonomies endpoint of the organization.
 
         Returns:
             TaxonomiesEndpoint: The taxonomies endpoint of the organization.
         """
         return TaxonomiesEndpoint().set_client(self.client).set_organization(self)
 
+    @property
+    def available_templates(self, page=1, page_size=10, query="*"):
+        """
+        Get the available templates for the organization.
+
+        Returns:
+            MarketplaceEndpoint: The marketplace endpoint of the organization.
+        """
+        url = f"/api/organizations/{self.id}/availableTemplates"
+        response = self.client.get(url, params={"page": page, "pageSize": page_size, "query": query})
+        return PageProjectTemplateEndpoint.model_validate(response.json()).set_client(self.client)
+
+    @property
+    def available_models(self, page=1, page_size=10, query="*"):
+        """
+        Get the available models for the organization.
+
+        Returns:
+            MarketplaceEndpoint: The marketplace endpoint of the organization.
+        """
+        url = f"/api/organizations/{self.id}/availableModels"
+        response = self.client.get(url, params={"page": page, "pageSize": page_size, "query": query})
+        return PageStoreEndpoint.model_validate(response.json()).set_client(self.client)
+
+    @property
+    def available_assistants(self, page=1, page_size=10, query="*"):
+        """
+        Get the available assistants for the organization.
+
+        Returns:
+            MarketplaceEndpoint: The marketplace endpoint of the organization.
+        """
+        url = f"/api/organizations/{self.id}/availableAssistants"
+        response = self.client.get(url, params={"page": page, "pageSize": page_size, "query": query})
+        return PageAssistantDefinitionEndpoint.model_validate(response.json()).set_client(self.client)
+
 
 class ComponentsEndpoint(ClientEndpoint):
     """
     Represents a components endpoint.
 
     Attributes:
         organization (OrganizationEndpoint): The organization endpoint that the components endpoint belongs to.
```

### Comparing `kodexa-7.0.8801100838/kodexa/platform/interaction.py` & `kodexa-7.0.8895840398/kodexa/platform/interaction.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8801100838/kodexa/platform/kodexa.py` & `kodexa-7.0.8895840398/kodexa/platform/kodexa.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8801100838/kodexa/selectors/ast.py` & `kodexa-7.0.8895840398/kodexa/selectors/ast.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8801100838/kodexa/selectors/core.py` & `kodexa-7.0.8895840398/kodexa/selectors/core.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8801100838/kodexa/selectors/lexrules.py` & `kodexa-7.0.8895840398/kodexa/selectors/lexrules.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8801100838/kodexa/selectors/lextab.py` & `kodexa-7.0.8895840398/kodexa/selectors/lextab.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8801100838/kodexa/selectors/parserules.py` & `kodexa-7.0.8895840398/kodexa/selectors/parserules.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8801100838/kodexa/selectors/parsetab.py` & `kodexa-7.0.8895840398/kodexa/selectors/parsetab.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8801100838/kodexa/spatial/azure_models.py` & `kodexa-7.0.8895840398/kodexa/spatial/azure_models.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8801100838/kodexa/spatial/bbox_common.py` & `kodexa-7.0.8895840398/kodexa/spatial/bbox_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8801100838/kodexa/spatial/table_form_common.py` & `kodexa-7.0.8895840398/kodexa/spatial/table_form_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8801100838/kodexa/steps/common.py` & `kodexa-7.0.8895840398/kodexa/steps/common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8801100838/kodexa/testing/test_components.py` & `kodexa-7.0.8895840398/kodexa/testing/test_components.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8801100838/kodexa/testing/test_utils.py` & `kodexa-7.0.8895840398/kodexa/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8801100838/pyproject.toml` & `kodexa-7.0.8895840398/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa"
-version = "7.0.08801100838"
+version = "7.0.08895840398"
 description = "Python SDK for the Kodexa Platform"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>"]
 readme = "README.md"
 
 packages = [
     { include = "kodexa" }
 ]
```

### Comparing `kodexa-7.0.8801100838/PKG-INFO` & `kodexa-7.0.8895840398/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa
-Version: 7.0.8801100838
+Version: 7.0.8895840398
 Summary: Python SDK for the Kodexa Platform
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

