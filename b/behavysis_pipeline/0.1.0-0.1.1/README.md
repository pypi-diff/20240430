# Comparing `tmp/behavysis_pipeline-0.1.0.tar.gz` & `tmp/behavysis_pipeline-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "behavysis_pipeline-0.1.0.tar", max compression
+gzip compressed data, was "behavysis_pipeline-0.1.1.tar", max compression
```

## Comparing `behavysis_pipeline-0.1.0.tar` & `behavysis_pipeline-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0     1233 2024-04-23 03:22:22.709814 behavysis_pipeline-0.1.0/behavysis_pipeline/__init__.py
--rw-r--r--   0        0        0       70 2024-04-22 07:42:28.518460 behavysis_pipeline-0.1.0/behavysis_pipeline/behav_classifier/__init__.py
--rw-r--r--   0        0        0    34527 2024-04-23 03:22:22.710918 behavysis_pipeline-0.1.0/behavysis_pipeline/behav_classifier/behav_classifier.py
--rw-r--r--   0        0        0      820 2024-04-23 03:22:30.848622 behavysis_pipeline-0.1.0/behavysis_pipeline/behav_classifier/behav_classifier_configs.py
--rw-r--r--   0        0        0      161 2024-04-23 03:22:22.706805 behavysis_pipeline-0.1.0/behavysis_pipeline/pipeline/__init__.py
--rw-r--r--   0        0        0    19616 2024-04-23 04:43:56.212268 behavysis_pipeline-0.1.0/behavysis_pipeline/pipeline/experiment.py
--rw-r--r--   0        0        0     5007 2024-04-23 03:17:43.919563 behavysis_pipeline-0.1.0/behavysis_pipeline/pipeline/experiment_configs.py
--rw-r--r--   0        0        0    18833 2024-04-23 03:22:22.710828 behavysis_pipeline-0.1.0/behavysis_pipeline/pipeline/project.py
--rw-r--r--   0        0        0      375 2024-04-18 23:44:38.297020 behavysis_pipeline-0.1.0/behavysis_pipeline/processes/__init__.py
--rw-r--r--   0        0        0    29457 2024-04-23 03:18:00.473989 behavysis_pipeline-0.1.0/behavysis_pipeline/processes/analyse.py
--rw-r--r--   0        0        0     6706 2024-04-23 03:18:00.485257 behavysis_pipeline-0.1.0/behavysis_pipeline/processes/calculate_params.py
--rw-r--r--   0        0        0     4117 2024-04-23 03:18:00.473924 behavysis_pipeline-0.1.0/behavysis_pipeline/processes/classify_behaviours.py
--rw-r--r--   0        0        0    13419 2024-04-23 03:18:00.475469 behavysis_pipeline-0.1.0/behavysis_pipeline/processes/evaluate.py
--rw-r--r--   0        0        0     6977 2024-04-23 03:18:00.485100 behavysis_pipeline-0.1.0/behavysis_pipeline/processes/extract_features.py
--rw-r--r--   0        0        0     3661 2024-04-23 03:18:00.475386 behavysis_pipeline-0.1.0/behavysis_pipeline/processes/format_vid.py
--rw-r--r--   0        0        0    12634 2024-04-23 03:18:00.485190 behavysis_pipeline-0.1.0/behavysis_pipeline/processes/preprocess.py
--rw-r--r--   0        0        0     2071 2024-04-23 03:18:00.496881 behavysis_pipeline-0.1.0/behavysis_pipeline/processes/run_dlc.py
--rw-r--r--   0        0        0     2504 2024-04-23 03:18:00.489806 behavysis_pipeline-0.1.0/behavysis_pipeline/processes/update_configs.py
--rw-r--r--   0        0        0    35821 2024-04-18 23:44:38.135361 behavysis_pipeline-0.1.0/LICENSE
--rw-r--r--   0        0        0      695 2024-04-23 05:11:24.810066 behavysis_pipeline-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1203 2024-04-23 03:18:33.575213 behavysis_pipeline-0.1.0/README.md
--rw-r--r--   0        0        0     1935 1970-01-01 00:00:00.000000 behavysis_pipeline-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1733 2024-04-30 16:37:09.700342 behavysis_pipeline-0.1.1/behavysis_pipeline/__init__.py
+-rw-r--r--   0        0        0       70 2024-04-22 07:42:28.518460 behavysis_pipeline-0.1.1/behavysis_pipeline/behav_classifier/__init__.py
+-rw-r--r--   0        0        0    34516 2024-04-30 17:43:43.957582 behavysis_pipeline-0.1.1/behavysis_pipeline/behav_classifier/behav_classifier.py
+-rw-r--r--   0        0        0      820 2024-04-23 03:22:30.848622 behavysis_pipeline-0.1.1/behavysis_pipeline/behav_classifier/behav_classifier_configs.py
+-rw-r--r--   0        0        0      143 2024-04-30 04:15:54.090529 behavysis_pipeline-0.1.1/behavysis_pipeline/pipeline/__init__.py
+-rw-r--r--   0        0        0    19082 2024-04-30 17:43:28.054972 behavysis_pipeline-0.1.1/behavysis_pipeline/pipeline/experiment.py
+-rw-r--r--   0        0        0    25067 2024-04-30 19:44:43.249976 behavysis_pipeline-0.1.1/behavysis_pipeline/pipeline/project.py
+-rw-r--r--   0        0        0      436 2024-04-30 13:59:20.350573 behavysis_pipeline-0.1.1/behavysis_pipeline/processes/__init__.py
+-rw-r--r--   0        0        0    34401 2024-04-30 16:56:00.235440 behavysis_pipeline-0.1.1/behavysis_pipeline/processes/analyse.py
+-rw-r--r--   0        0        0     7875 2024-04-30 18:01:02.983479 behavysis_pipeline-0.1.1/behavysis_pipeline/processes/calculate_params.py
+-rw-r--r--   0        0        0     4169 2024-04-30 19:41:08.279459 behavysis_pipeline-0.1.1/behavysis_pipeline/processes/classify_behaviours.py
+-rw-r--r--   0        0        0    13118 2024-04-30 16:37:05.575130 behavysis_pipeline-0.1.1/behavysis_pipeline/processes/evaluate.py
+-rw-r--r--   0        0        0     6935 2024-04-30 19:35:35.747582 behavysis_pipeline-0.1.1/behavysis_pipeline/processes/extract_features.py
+-rw-r--r--   0        0        0     3658 2024-04-30 07:31:57.441936 behavysis_pipeline-0.1.1/behavysis_pipeline/processes/format_vid.py
+-rw-r--r--   0        0        0    13798 2024-04-30 17:05:45.566321 behavysis_pipeline-0.1.1/behavysis_pipeline/processes/preprocess.py
+-rw-r--r--   0        0        0     6802 2024-04-30 19:30:58.122100 behavysis_pipeline-0.1.1/behavysis_pipeline/processes/run_dlc.py
+-rw-r--r--   0        0        0     2403 2024-04-30 17:37:53.737501 behavysis_pipeline-0.1.1/behavysis_pipeline/processes/update_configs.py
+-rw-r--r--   0        0        0    35821 2024-04-18 23:44:38.135361 behavysis_pipeline-0.1.1/LICENSE
+-rw-r--r--   0        0        0      693 2024-04-30 19:57:35.243286 behavysis_pipeline-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1203 2024-04-23 03:18:33.575213 behavysis_pipeline-0.1.1/README.md
+-rw-r--r--   0        0        0     1935 1970-01-01 00:00:00.000000 behavysis_pipeline-0.1.1/PKG-INFO
```

### Comparing `behavysis_pipeline-0.1.0/behavysis_pipeline/__init__.py` & `behavysis_pipeline-0.1.1/behavysis_pipeline/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,8 +17,26 @@
 
 warnings.filterwarnings("ignore")
 
 #####################################################################
 #         IMPORTING MODULES (INCL. RELATIVE AND 3RD PARTY)
 #####################################################################
 
-from behavysis_pipeline.pipeline import BehavysisExperiment, BehavysisProject
+import matplotlib
+import matplotlib.pyplot as plt
+import seaborn as sns
+from behavysis_core.constants import PLOT_DPI, PLOT_STYLE
+
+from behavysis_pipeline.pipeline import Experiment, Project
+
+#####################################################################
+#           INITIALISE MPL PLOTTING PARAMETERS
+#####################################################################
+
+
+# Makes graphs non-interactive (saves memory)
+matplotlib.use("Agg")
+
+sns.set_theme(style=PLOT_STYLE)
+
+plt.rcParams["figure.dpi"] = PLOT_DPI
+plt.rcParams["savefig.dpi"] = PLOT_DPI
```

### Comparing `behavysis_pipeline-0.1.0/behavysis_pipeline/behav_classifier/behav_classifier.py` & `behavysis_pipeline-0.1.1/behavysis_pipeline/behav_classifier/behav_classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,35 +9,37 @@
 from typing import TYPE_CHECKING, Optional
 
 import joblib
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
-from behavysis_core.mixins.df_io_mixin import DFIOMixin
-from behavysis_core.utils.constants import (
+from behavysis_core.constants import (
     BEHAV_ACTUAL_COL,
     BEHAV_COLUMN_NAMES,
     BEHAV_PRED_COL,
     BEHAV_PROB_COL,
 )
+from behavysis_core.mixins.df_io_mixin import DFIOMixin
 from imblearn.under_sampling import RandomUnderSampler
 from matplotlib.figure import Figure
 from sklearn.ensemble import GradientBoostingClassifier
 from sklearn.metrics import (
     accuracy_score,
     classification_report,
     confusion_matrix,
     precision_recall_fscore_support,
 )
 
-from behavysis_pipeline.behav_classifier.behav_classifier_configs import BehavClassifierConfigs
+from behavysis_pipeline.behav_classifier.behav_classifier_configs import (
+    BehavClassifierConfigs,
+)
 
 if TYPE_CHECKING:
-    from behavysis_pipeline.pipeline.project import BehavysisProject
+    from behavysis_pipeline.pipeline.project import Project
 
 
 class BehavClassifier:
     """
     BehavClassifier class peforms behav classifier model preparation, training, saving,
     evaluation, and inference.
     """
@@ -65,22 +67,22 @@
                 configs = BehavClassifierConfigs.read_json(self.configs_fp)
             except FileNotFoundError:
                 configs = BehavClassifierConfigs()
         # Saving configs
         configs.write_json(self.configs_fp)
 
     @classmethod
-    def from_BehavysisProject(cls, proj: BehavysisProject) -> BehavClassifier:
+    def from_Project(cls, proj: Project) -> BehavClassifier:
         """
-        Loading classifier from given BehavysisProject instance.
+        Loading classifier from given Project instance.
 
         Parameters
         ----------
-        proj : BehavysisProject
-            The BehavysisProject instance.
+        proj : Project
+            The Project instance.
 
         Returns
         -------
         BehavClassifier
             The loaded BehavClassifier instance.
         """
         configs_fp: str = os.path.abspath(
@@ -454,17 +456,19 @@
         ].values
         # Saving eval df to file
         eval_fp = os.path.join(self.root_dir, "eval", "eval_df.feather")
         DFIOMixin.write_feather(eval_df, eval_fp)
         # Making pcutoff metrics plot
         fig = self.model_eval_plot_metrics(eval_df)
         fig.savefig(os.path.join(self.root_dir, "eval", "pcutoff_metrics.png"))
+        fig.clf()
         # Making logistic results plot
         fig = self.model_eval_plot_results(eval_df)
         fig.savefig(os.path.join(self.root_dir, "eval", "logistic_results.png"))
+        fig.clf()
 
     #################################################
     #         EVALUATE MODEL PREDICTIONS
     #################################################
 
     def model_eval_report(self, eval_df: pd.DataFrame) -> None:
         """
```

### Comparing `behavysis_pipeline-0.1.0/behavysis_pipeline/behav_classifier/behav_classifier_configs.py` & `behavysis_pipeline-0.1.1/behavysis_pipeline/behav_classifier/behav_classifier_configs.py`

 * *Files identical despite different names*

### Comparing `behavysis_pipeline-0.1.0/behavysis_pipeline/pipeline/experiment.py` & `behavysis_pipeline-0.1.1/behavysis_pipeline/pipeline/experiment.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,34 @@
 
 import os
 import shutil
 from typing import Any, Callable
 
 import numpy as np
 import pandas as pd
+from behavysis_core.constants import (
+    ANALYSIS_DIR,
+    EVALUATE_DIR,
+    FOLDERS,
+    STR_DIV,
+    TEMP_DIR,
+)
 from behavysis_core.mixins.df_io_mixin import DFIOMixin
 from behavysis_core.mixins.diagnostics_mixin import DiagnosticsMixin
-from behavysis_core.utils.constants import (ANALYSIS_DIR, EVALUATE_DIR, FOLDERS,
-                                     STR_DIV, TEMP_DIR)
 
-from behavysis_pipeline.processes import (ClassifyBehaviours, ExtractFeatures, RunDLC,
-                                   UpdateConfigs)
+from behavysis_pipeline.processes import (
+    ClassifyBehaviours,
+    ExtractFeatures,
+    Preprocess,
+    RunDLC,
+    UpdateConfigs,
+)
 
 
-class BehavysisExperiment:
+class Experiment:
     """
     Behavioral Analysis Pipeline class for a single experiment.
 
     Encompasses the entire process including:
     - Raw mp4 file import.
     - mp4 file formatting (px and fps).
     - DLC keypoints inference.
@@ -42,28 +52,28 @@
     ------
     ValueError
         ValueError: `root_dir` does not exist or `name` does not exist in the `root_dir` folder.
     """
 
     def __init__(self, name: str, root_dir: str) -> None:
         """
-        Make a BehavysisExperiment instance.
+        Make a Experiment instance.
         """
         # Assertion: root_dir mus† exist
         if not os.path.isdir(root_dir):
             raise ValueError(
                 f'Cannot find the project folder named "{root_dir}".\n'
                 + "Please specify a folder that exists."
             )
         # Assertion: name must correspond to at least one file in root_dir
-        folder_fp_ls = [
-            os.path.join(root_dir, folder, f"{name}{ext}")
+        file_exists_ls = [
+            os.path.isfile(os.path.join(root_dir, folder, f"{name}{ext}"))
             for folder, ext in FOLDERS.items()
         ]
-        if not np.any([os.path.isfile(i) for i in folder_fp_ls]):
+        if not np.any(file_exists_ls):
             raise ValueError(
                 f'No files named "{name}" exist in "{root_dir}".\n'
                 + f'Please specify a file that exists in "{root_dir}", in one of the'
                 + " following folder WITH the correct file extension name:\n"
                 + "    - "
                 + "\n    - ".join(FOLDERS.keys())
             )
@@ -104,65 +114,48 @@
         # Getting experiment filepath for given folder
         fp = os.path.join(self.root_dir, folder, f"{self.name}{FOLDERS[folder]}")
         # Making a folder if it does not exist
         os.makedirs(os.path.split(fp)[0], exist_ok=True)
         # Returning filepath
         return fp
 
-    def check_fp(self, folder: str) -> bool:
-        """
-        Returns whether the corresponding experiment file exists in the given folder.
-
-        Parameters
-        ----------
-        folder : str
-            The folder to check the experiment document's filepath for.
-
-        Returns
-        -------
-        bool
-            Boolean outcome of whether the corresponding file exists.
-        """
-        fp = self.get_fp(folder)
-        return os.path.isfile(fp)
-
     #####################################################################
     #               EXPERIMENT PROCESSING SCAFFOLD METHODS
     #####################################################################
 
     def _process_scaffold(
         self,
         funcs: tuple[Callable, ...],
         *args: Any,
         **kwargs: Any,
-    ) -> dict:
+    ) -> dict[str, str]:
         """
         All processing runs through here.
         This method ensures that the stdout and diagnostics dict are correctly generated.
 
         Parameters
         ----------
         funcs : tuple[Callable, ...]
             List of functions.
 
         Returns
         -------
-        dict
+        dict[str, str]
             Diagnostics dictionary, with description of each function's outcome.
 
         Notes
         -----
         Each func in `funcs` is called in the form:
         ```
         func(*args, **kwargs)
         ```
         """
+        print(f"Processing experiment: {self.name}")
         # Setting up diagnostics dict
         dd = {"experiment": self.name}
-        print(f"Processing experiment: {self.name}")
         # Running functions and saving outcome to diagnostics dict
         for f in funcs:
             # Running each func and saving outcome
             try:
                 dd[f.__name__] = f(*args, **kwargs)
                 dd[f.__name__] += f"SUCCESS: {DiagnosticsMixin.success_msg()}\n"
             except Exception as e:
@@ -259,18 +252,19 @@
             Diagnostics dictionary, with description of each function's outcome.
 
         Notes
         -----
         Can call any methods from `RunDLC`.
         """
         return self._process_scaffold(
-            (RunDLC.ma_dlc_analyse,),
+            (RunDLC.ma_dlc_analyse_single,),
             in_fp=self.get_fp("2_formatted_vid"),
             out_fp=self.get_fp("3_dlc"),
             configs_fp=self.get_fp("0_configs"),
+            temp_dir=os.path.join(self.root_dir, TEMP_DIR),
             gputouse=gputouse,
             overwrite=overwrite,
         )
 
     def calculate_params(self, funcs: tuple[Callable, ...]) -> dict:
         """
         A pipeline to calculate the parameters of the raw DLC file, which will
@@ -317,24 +311,25 @@
             Diagnostics dictionary, with description of each function's outcome.
 
         Notes
         -----
         Can call any methods from `Preprocess`.
         """
         # Exporting 3_dlc df to 4_preprocessed folder
+        dd = self._process_scaffold(
+            (Preprocess.import_keypoints_df,),
+            in_fp=self.get_fp("3_dlc"),
+            out_fp=self.get_fp("4_preprocessed"),
+            configs_fp=self.get_fp("0_configs"),
+            overwrite=overwrite,
+        )
         # If there is an error, then makes the diagnostics dict
-        # where all function outcomes have the error message
-        try:
-            df = DFIOMixin.read_feather(self.get_fp("3_dlc"))
-            DFIOMixin.write_feather(df, self.get_fp("4_preprocessed"))
-        except Exception as e:
-            dd = {f.__name__: str(e) for f in funcs}
-            dd["experiment"] = self.name
+        res = dd["import_keypoints_df"]
+        if res.startswith("ERROR") or res.startswith("WARNING"):
             return dd
-
         # Feeding through preprocessing functions
         return self._process_scaffold(
             funcs,
             in_fp=self.get_fp("4_preprocessed"),
             out_fp=self.get_fp("4_preprocessed"),
             configs_fp=self.get_fp("0_configs"),
             overwrite=overwrite,
@@ -417,39 +412,36 @@
         DFIOMixin.write_feather(total_df, out_fp)
         return dd
 
     #####################################################################
     #                 SIMBA BEHAVIOUR CLASSIFICATION METHODS
     #####################################################################
 
-    def extract_features(self, remove_temp: bool, overwrite: bool) -> dict:
+    def extract_features(self, overwrite: bool) -> dict:
         """
         Extracts features from the preprocessed dlc file to generate many more features.
         This dataframe of derived features will be input for a ML classifier to detect
         particularly trained behaviours.
 
         Parameters
         ----------
-        remove_temp : bool
-            Whether to remove the temp directory.
         overwrite : bool
             Whether to overwrite the output file (if it exists).
 
         Returns
         -------
         dict
             Diagnostics dictionary, with description of each function's outcome.
         """
         return self._process_scaffold(
             (ExtractFeatures.extract_features,),
             dlc_fp=self.get_fp("4_preprocessed"),
             out_fp=self.get_fp("5_features_extracted"),
             configs_fp=self.get_fp("0_configs"),
             temp_dir=os.path.join(self.root_dir, TEMP_DIR),
-            remove_temp=remove_temp,
             overwrite=overwrite,
         )
 
     def classify_behaviours(self, overwrite: bool) -> dict:
         """
         Given model config files in the BehavClassifier format, generates beahviour predidctions
         on the given extracted features dataframe.
```

### Comparing `behavysis_pipeline-0.1.0/behavysis_pipeline/pipeline/project.py` & `behavysis_pipeline-0.1.1/behavysis_pipeline/pipeline/project.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,24 +6,33 @@
 import os
 import re
 from multiprocessing import Pool
 from typing import Any, Callable
 
 import numpy as np
 import pandas as pd
+import seaborn as sns
+from behavysis_core.constants import (
+    ANALYSIS_DIR,
+    DIAGNOSTICS_DIR,
+    FOLDERS,
+    STR_DIV,
+    TEMP_DIR,
+)
+from behavysis_core.data_models.experiment_configs import ConfigsAuto, ExperimentConfigs
 from behavysis_core.mixins.df_io_mixin import DFIOMixin
 from behavysis_core.mixins.io_mixin import IOMixin
-from behavysis_core.utils.constants import ANALYSIS_DIR, DIAGNOSTICS_DIR, FOLDERS, STR_DIV
+from behavysis_core.mixins.multiproc_mixin import MultiprocMixin
 from natsort import natsort_keygen, natsorted
 
-from behavysis_pipeline.pipeline.experiment import BehavysisExperiment
-from behavysis_pipeline.pipeline.experiment_configs import ExperimentConfigs
+from behavysis_pipeline.pipeline.experiment import Experiment
+from behavysis_pipeline.processes.run_dlc import RunDLC
 
 
-class BehavysisProject:
+class Project:
     """
     A project is used to process and analyse many experiments at the same time.
 
     Expected filesystem hierarchy of project directory is below:
     ```
         - dir
             - 0_configs
@@ -132,180 +141,275 @@
         or absolute.
         experiments: The experiments that have been loaded into the project.
 
     Raises:
         ValueError: The givendir filepath does not exist.
     """
 
+    root_dir: str
+    experiments: dict[str, Experiment]
+    nprocs: int
+
     def __init__(self, root_dir: str) -> None:
         """
-        Make a BehavysisProject instance.
+        Make a Project instance.
         """
         # Assertion: project directory must exist
         if not os.path.isdir(root_dir):
             raise ValueError(
                 f'Error: The folder, "{root_dir}" does not exist.\n'
                 + "Please specify a folder that exists. Ensure you have the correct"
                 + "forward-slashes or back-slashes for the path name."
             )
-        self.root_dir = root_dir
+        self.root_dir = os.path.abspath(root_dir)
         self.experiments = {}
         self.nprocs = 4
 
-        # Making batch processing methods dynamically for BehavysisExperiment methods
-        self.process_scaffold = self.process_scaffold_mp
-        method_names_ls = [i for i in dir(BehavysisExperiment) if not re.search(r"^_", i)]
-        for method_name in method_names_ls:
-            self._batch_process_factory(method_name)
-
-    def _batch_process_factory(self, method_name: str):
-        method = getattr(BehavysisExperiment, method_name)
-
-        @functools.wraps(method)
-        def batch_process(*args, **kwargs):
-            # Starting
-            print(f"Running {method_name}")
-            # Running
-            self.process_scaffold(method, *args, **kwargs)
-            # Finishing
-            print(f"Finished {method_name}!")
-            print(f"{STR_DIV}\n{STR_DIV}\n")
-
-        setattr(self, method_name, batch_process)
-
     #####################################################################
     #               GETTER METHODS
     #####################################################################
 
-    def get_experiment(self, name: str) -> BehavysisExperiment:
+    def get_experiment(self, name: str) -> Experiment:
         """
         Gets the experiment with the given name
 
         Parameters
         ----------
         name : str
             The experiment name.
 
         Returns
         -------
-        BehavysisExperiment
+        Experiment
             The experiment.
 
         Raises
         ------
         ValueError
             Experiment with the given name does not exist.
         """
         if name in self.experiments:
             return self.experiments[name]
         raise ValueError(
             f'Experiment with the name "{name}" does not exist in the project.'
         )
 
-    def get_experiments(self) -> list[BehavysisExperiment]:
+    def get_experiments(self) -> list[Experiment]:
         """
-        Gets the ordered (natsorted) list of Experiment instances in the BehavysisProject.
+        Gets the ordered (natsorted) list of Experiment instances in the Project.
 
         Returns
         -------
-        list[BehavysisExperiment]
-            The list of all BehavysisExperiment instances stored in the BehavysisProject instance.
+        list[Experiment]
+            The list of all Experiment instances stored in the Project instance.
         """
         return [self.experiments[i] for i in natsorted(self.experiments)]
 
     #####################################################################
     #               PROJECT PROCESSING SCAFFOLD METHODS
     #####################################################################
 
     @staticmethod
-    def _process_scaffold_worker(args_tuple: tuple):
+    def _process_scaffold_mp_worker(args_tuple: tuple):
         method, exp, args, kwargs = args_tuple
         return method(exp, *args, **kwargs)
 
-    def process_scaffold_mp(
-        self,
-        method: Callable,
-        *args: Any,
-        **kwargs: Any,
-    ) -> None:
+    def _process_scaffold_mp(
+        self, method: Callable, *args: Any, **kwargs: Any
+    ) -> list[dict]:
         """
-        Processes an experiment with the given `BehavysisExperiment` method and records the diagnostics
-        of the process in a MULTI-PROCESSING way.
+        Processes an experiment with the given `Experiment` method and records
+        the diagnostics of the process in a MULTI-PROCESSING way.
 
         Parameters
         ----------
         method : Callable
-            The `BehavysisExperiment` method to run.
+            The `Experiment` class method to run.
 
         Notes
         -----
-        Can call any `BehavysisExperiment` methods instance.
+        Can call any `Experiment` methods instance.
         Effectively, `method` gets called with:
         ```
-        # exp is a BehavysisExperiment instance
+        # exp is a Experiment instance
         method(exp, *args, **kwargs)
         ```
         """
-        # Initialising diagnostics dataframe
-        df = pd.DataFrame()
-
-        # TODO: maybe have a try-except-finally block to ensure that the diagnostics file is saved
         # Create a Pool of processes
         with Pool(processes=self.nprocs) as p:
             # Apply method to each experiment in self.get_experiments() in parallel
-            results = p.map(
-                BehavysisProject._process_scaffold_worker,
+            return p.map(
+                Project._process_scaffold_mp_worker,
                 [(method, exp, args, kwargs) for exp in self.get_experiments()],
             )
 
-        # Processing all experiments
-        for dd in results:
-            # Converting outcomes dict to dataframe
-            dd = pd.DataFrame(pd.Series(dd)).transpose().set_index("experiment")
-            # Adding outcomes dict to diagnostics dataframe
-            df = pd.concat([df, dd], axis=0).sort_index(key=natsort_keygen())
-            # Updating the diagnostics file at each step
-            self.save_diagnostics(method.__name__, df)
-
-    def process_scaffold_sp(
-        self,
-        method: Callable,
-        *args: Any,
-        **kwargs: Any,
-    ) -> None:
+    def _process_scaffold_sp(
+        self, method: Callable, *args: Any, **kwargs: Any
+    ) -> list[dict]:
         """
-        Processes an experiment with the given `BehavysisExperiment` method and records the diagnostics
-        of the process in a SINGLE-PROCESSING way.
+        Processes an experiment with the given `Experiment` method and records
+        the diagnostics of the process in a SINGLE-PROCESSING way.
 
         Parameters
         ----------
         method : Callable
-            The experiment `BehavysisExperiment` method to run.
+            The experiment `Experiment` class method to run.
 
         Notes
         -----
-        Can call any `BehavysisExperiment` instance method.
+        Can call any `Experiment` instance method.
         Effectively, `method` gets called with:
         ```
-        # exp is a BehavysisExperiment instance
+        # exp is a Experiment instance
         method(exp, *args, **kwargs)
         ```
         """
-        # Initialising diagnostics dataframe
-        df = pd.DataFrame()
+        # Processing all experiments and storing process outcomes as list of dicts
+        return [method(exp, *args, **kwargs) for exp in self.get_experiments()]
+
+    def _process_scaffold(self, method: Callable, *args: Any, **kwargs: Any) -> None:
+        """
+        Runs the given method on all experiments in the project.
+        """
+        # Choosing whether to run the scaffold function in single or multi-processing mode
+        if self.nprocs == 1:
+            scaffold_func = self._process_scaffold_sp
+        else:
+            scaffold_func = self._process_scaffold_mp
+        # Running the scaffold function
+        # Starting
+        print(f"Running {method.__name__}")
+        # Running
+        dd_ls = scaffold_func(method, *args, **kwargs)
         # Processing all experiments
-        for exp in self.get_experiments():
-            # Processing and storing process outcomes as dict
-            dd = method(exp, *args, **kwargs)
-            # Converting outcomes dict to dataframe
-            dd = pd.DataFrame(pd.Series(dd)).transpose().set_index("experiment")
-            # Adding outcomes dict to diagnostics dataframe
-            df = pd.concat([df, dd], axis=0).sort_index(key=natsort_keygen())
-            # Updating the diagnostics file at each step
-            self.save_diagnostics(method.__name__, df)
+        df = (
+            pd.DataFrame(dd_ls).set_index("experiment").sort_index(key=natsort_keygen())
+        )
+        # Updating the diagnostics file at each step
+        self.save_diagnostics(method.__name__, df)
+        # Finishing
+        print(f"Finished {method.__name__}!\n{STR_DIV}\n{STR_DIV}\n")
+
+    #####################################################################
+    #               BATCH PROCESSING METHODS
+    #####################################################################
+
+    @functools.wraps(Experiment.update_configs)
+    def update_configs(self, *args, **kwargs) -> None:
+        """
+        Batch processing for corresponding [Experiment method](experiment.md#behavysis_pipeline.pipeline.Experiment.update_configs)
+        """
+        method = Experiment.update_configs
+        self._process_scaffold(method, *args, **kwargs)
+
+    @functools.wraps(Experiment.format_vid)
+    def format_vid(self, *args, **kwargs) -> None:
+        """
+        Batch processing for corresponding [Experiment method](experiment.md#behavysis_pipeline.pipeline.Experiment.format_vid)
+        """
+        method = Experiment.format_vid
+        self._process_scaffold(method, *args, **kwargs)
+
+    @functools.wraps(Experiment.run_dlc)
+    def run_dlc(self, gputouse: int = None, overwrite: bool = False) -> None:
+        """
+        Batch processing for corresponding [Experiment method](experiment.md#behavysis_pipeline.pipeline.Experiment.run_dlc)
+        """
+        nprocs = len(MultiprocMixin.get_gpu_ids()) if gputouse is None else 1
+        # Getting the experiments to run DLC on
+        exp_ls = self.get_experiments()
+        # If overwrite is false, filtering for only experiments that need to be run
+        if not overwrite:
+            exp_ls = [exp for exp in exp_ls if not os.path.isfile(exp.get_fp("3_dlc"))]
+        # Splitting the experiments into batches
+        exp_batches_ls = np.array_split(exp_ls, nprocs)
+        # Running DLC on each batch of experiments
+        with Pool(processes=nprocs) as p:
+            p.starmap(
+                RunDLC.ma_dlc_analyse_batch,
+                [
+                    (
+                        [exp.get_fp("2_formatted_vid") for exp in exp_batch],
+                        os.path.join(self.root_dir, "3_dlc"),
+                        os.path.join(self.root_dir, "0_configs"),
+                        os.path.join(self.root_dir, TEMP_DIR),
+                        gputouse,
+                        overwrite,
+                    )
+                    for exp_batch in exp_batches_ls
+                ],
+            )
+
+    @functools.wraps(Experiment.calculate_params)
+    def calculate_params(self, *args, **kwargs) -> None:
+        """
+        Batch processing for corresponding [Experiment method](experiment.md#behavysis_pipeline.pipeline.Experiment.calculate_params)
+        """
+        method = Experiment.calculate_params
+        self._process_scaffold(method, *args, **kwargs)
+
+    @functools.wraps(Experiment.preprocess)
+    def preprocess(self, *args, **kwargs) -> None:
+        """
+        Batch processing for corresponding [Experiment method](experiment.md#behavysis_pipeline.pipeline.Experiment.preprocess)
+        """
+        method = Experiment.preprocess
+        self._process_scaffold(method, *args, **kwargs)
+
+    @functools.wraps(Experiment.extract_features)
+    def extract_features(self, *args, **kwargs) -> None:
+        """
+        Batch processing for corresponding [Experiment method](experiment.md#behavysis_pipeline.pipeline.Experiment.extract_features)
+        """
+        method = Experiment.extract_features
+        self._process_scaffold(method, *args, **kwargs)
+
+    @functools.wraps(Experiment.classify_behaviours)
+    def classify_behaviours(self, *args, **kwargs) -> None:
+        """
+        Batch processing for corresponding [Experiment method](experiment.md#behavysis_pipeline.pipeline.Experiment.classify_behaviours)
+        """
+        # TODO: handle reading the model file whilst in multiprocessing. Current fix is single processing.
+        nprocs = self.nprocs
+        self.nprocs = 1
+        method = Experiment.classify_behaviours
+        self._process_scaffold(method, *args, **kwargs)
+        self.nprocs = nprocs
+
+    @functools.wraps(Experiment.export_behaviours)
+    def export_behaviours(self, *args, **kwargs) -> None:
+        """
+        Batch processing for corresponding [Experiment method](experiment.md#behavysis_pipeline.pipeline.Experiment.export_behaviours)
+        """
+        method = Experiment.export_behaviours
+        self._process_scaffold(method, *args, **kwargs)
+
+    @functools.wraps(Experiment.export_feather)
+    def export_feather(self, *args, **kwargs) -> None:
+        """
+        Batch processing for corresponding [Experiment method](experiment.md#behavysis_pipeline.pipeline.Experiment.export_feather)
+        """
+        method = Experiment.export_feather
+        self._process_scaffold(method, *args, **kwargs)
+
+    @functools.wraps(Experiment.evaluate)
+    def evaluate(self, *args, **kwargs) -> None:
+        """
+        Batch processing for corresponding [Experiment method](experiment.md#behavysis_pipeline.pipeline.Experiment.evaluate)
+        """
+        method = Experiment.evaluate
+        self._process_scaffold(method, *args, **kwargs)
+
+    @functools.wraps(Experiment.analyse)
+    def analyse(self, *args, **kwargs) -> None:
+        """
+        Batch processing for corresponding [Experiment method](experiment.md#behavysis_pipeline.pipeline.Experiment.analyse)
+        """
+        method = Experiment.analyse
+        self._process_scaffold(method, *args, **kwargs)
 
     #####################################################################
     #               DIAGNOSTICS DICT METHODS
     #####################################################################
 
     def load_diagnostics(self, name: str) -> pd.DataFrame:
         """
@@ -339,14 +443,54 @@
         fp = os.path.join(self.root_dir, DIAGNOSTICS_DIR, f"{name}.csv")
         # Making a folder if it does not exist
         os.makedirs(os.path.split(fp)[0], exist_ok=True)
         # Writing diagnostics file
         df.to_csv(fp)
 
     #####################################################################
+    #                CONFIGS DIAGONOSTICS METHODS
+    #####################################################################
+
+    def collate_configs_auto(self) -> None:
+        """
+        Collates the auto fields of the configs of all experiments into a DataFrame.
+        """
+        # Getting all the auto field keys
+        auto_field_keys = ConfigsAuto.get_field_names(ConfigsAuto)
+        # Making a DataFrame to store all the auto fields for each experiment
+        df_configs = pd.DataFrame(
+            index=[exp.name for exp in self.get_experiments()],
+            # columns=ConfigsAuto.model_fields.keys(),
+            columns=["_".join(i) for i in auto_field_keys],
+        )
+        # Collating all the auto fields for each experiment
+        for exp in self.get_experiments():
+            configs = ExperimentConfigs.read_json(exp.get_fp("0_configs"))
+            for i in auto_field_keys:
+                val = configs.auto
+                for j in i:
+                    val = getattr(val, j)
+                df_configs.loc[exp.name, "_".join(i)] = val
+        # Saving the collated auto fields DataFrame to diagnostics folder
+        self.save_diagnostics("collated_configs_auto", df_configs)
+
+        # Making and saving histogram plots of all the auto fields
+        g = sns.FacetGrid(
+            data=df_configs.melt(), col="variable", sharex=False, col_wrap=4
+        )
+        g.map(sns.histplot, "value", bins=20)
+        g.set_titles("{col_name}")
+        g.savefig(
+            os.path.join(
+                self.root_dir, DIAGNOSTICS_DIR, "collated_configs_auto_hist.png"
+            )
+        )
+        g.figure.clf()
+
+    #####################################################################
     #               IMPORT EXPERIMENTS METHODS
     #####################################################################
 
     def import_experiment(self, name: str) -> bool:
         """
         Adds an experiment with the given name to the .experiments dict.
         The key of this experiment in the `self.experiments` dict is "dir/name".
@@ -360,73 +504,70 @@
         Returns
         -------
         bool
             Whether the experiment was imported or not.
             True if imported, False if not.
         """
         if not name in self.experiments:
-            self.experiments[name] = BehavysisExperiment(name, self.root_dir)
+            self.experiments[name] = Experiment(name, self.root_dir)
             return True
         return False
 
     def import_experiments(self) -> None:
         """
         Add all experiments in the project folder to the experiments dict.
         The key of each experiment in the .experiments dict is "name".
-        Refer to BehavysisProject.addExperiment() for details about how each experiment is added.
+        Refer to Project.addExperiment() for details about how each experiment is added.
         """
         print(f"Searching project folder: {self.root_dir}\n")
         # Adding all experiments within given project dir
-        imported = []
         failed = []
         for i in FOLDERS:
-            dir_folder = os.path.join(self.root_dir, i)
-            if os.path.isdir(dir_folder):
-                for j in natsorted(os.listdir(dir_folder)):
-                    if j[0] == ".":  # do not add hidden files
-                        continue
-                    name = IOMixin.get_name(j)
-                    try:
-                        if self.import_experiment(name):
-                            imported.append(name)
-                    except ValueError as e:  # do not add invalid files
-                        print(f"failed: {i}    --    {j}")
-                        print(e)
-                        failed.append(name)
+            folder = os.path.join(self.root_dir, i)
+            # If folder does not exist, skip
+            if not os.path.isdir(folder):
+                continue
+            # For each file in the folder
+            for j in natsorted(os.listdir(folder)):
+                if re.search(r"^\.", j):  # do not add hidden files
+                    continue
+                name = IOMixin.get_name(j)
+                try:
+                    self.import_experiment(name)
+                except ValueError as e:  # do not add invalid files
+                    print(f"failed: {i}    --    {j}:\n{e}")
+                    failed.append(name)
         # Printing outcome of imported and failed experiments
         print("Experiments imported successfully:")
-        for i in imported:
-            print(f"    - {i}")
-        print("")
+        print("\n".join([f"    - {i}" for i in self.experiments]), end="\n\n")
         print("Experiments failed to import:")
-        for i in failed:
-            print(f"    - {i}")
-        print("")
+        print("\n".join([f"    - {i}" for i in failed]), end="\n\n")
         # Making diagnostics DataFrame of all the files associated with each experiment that exists
-        dd_df = pd.DataFrame(
-            index=list(self.experiments.keys()), columns=list(FOLDERS.keys())
-        )
-        for exp in self.get_experiments():
-            for folder in FOLDERS:
-                dd_df.loc[exp.name, folder] = exp.check_fp(folder)
-        self.save_diagnostics("importExperiments.csv", dd_df)
+        # TODO: MAKE FASTER
+        cols_ls = list(FOLDERS)
+        rows_ls = list(self.experiments)
+        shape = (len(rows_ls), len(cols_ls))
+        dd_arr = np.apply_along_axis(
+            lambda i: os.path.isfile(self.experiments[i[1]].get_fp(i[0])),
+            axis=0,
+            arr=np.array(np.meshgrid(cols_ls, rows_ls)).reshape((2, np.prod(shape))),
+        ).reshape(shape)
+        # Creating the diagnostics DataFrame
+        dd_df = pd.DataFrame(dd_arr, index=rows_ls, columns=cols_ls)
+        # Saving the diagnostics DataFrame
+        self.save_diagnostics("import_experiments", dd_df)
 
     #####################################################################
     #            COMBINING ANALYSIS DATA ACROSS EXPS METHODS
     #####################################################################
 
-    def combine_analysis_binned(self) -> None:
+    def collate_analysis_binned(self) -> None:
         """
         Combines an analysis of all the experiments together to generate combined h5 files for:
         - Each binned data. The index is (bin) and columns are (expName, indiv, measure).
-
-        Parameters
-        ----------
-        overwrite : bool
-            Whether to overwrite the output file (if it exists).
         """
         # Initialising the process and printing the description
         description = "Combining binned analysis"
         print(f"{description}...")
         # dd_df = pd.DataFrame()
 
         # AGGREGATING BINNED DATA
@@ -456,24 +597,19 @@
                         df = pd.concat(
                             [df], keys=[exp.name], names=["experiment"], axis=1
                         )
                         # Concatenating total_df with df across columns
                         total_df = pd.concat([total_df, df], axis=1)
                     DFIOMixin.write_feather(total_df, out_fp)
 
-    def combine_analysis_summary(self) -> None:
+    def collate_analysis_summary(self) -> None:
         """
         Combines an analysis of all the experiments together to generate combined h5 files for:
         - The summary data. The index is (expName, indiv, measure) and columns are
         (statistics -e.g., mean).
-
-        Parameters
-        ----------
-        overwrite : bool
-            Whether to overwrite the output file (if it exists).
         """
         # Initialising the process and printing the description
         description = "Combining summary analysis"
         print(f"{description}...")
         # dd_df = pd.DataFrame()
 
         # AGGREGATING SUMMARY DATA
```

### Comparing `behavysis_pipeline-0.1.0/behavysis_pipeline/processes/analyse.py` & `behavysis_pipeline-0.1.1/behavysis_pipeline/processes/analyse.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,50 +16,37 @@
     The outcome of the process.
 """
 
 from __future__ import annotations
 
 import os
 
-import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
-from behavysis_core.mixins.behaviour_mixin import BehaviourMixin
-from behavysis_core.mixins.df_io_mixin import DFIOMixin
-from behavysis_core.mixins.io_mixin import IOMixin
-from behavysis_core.mixins.keypoints_mixin import KeypointsMixin
-from behavysis_core.utils.constants import (
+from behavysis_core.constants import (
     ANALYSIS_COLUMN_NAMES,
     ANALYSIS_INDEX_NAMES,
-    BODYCENTRE,
-    PLOT_DPI,
-    PLOT_STYLE,
     SINGLE_COL,
 )
-
-from behavysis_pipeline.pipeline.experiment_configs import ExperimentConfigs
-
-#####################################################################
-#               INITIALISE MPL PLOTTING PARAMETERS
-#####################################################################
-
-
-sns.set_theme(style=PLOT_STYLE)
-
-plt.rcParams["figure.dpi"] = PLOT_DPI
-plt.rcParams["savefig.dpi"] = PLOT_DPI
-
+from behavysis_core.data_models.experiment_configs import ExperimentConfigs
+from behavysis_core.mixins.behaviour_mixin import BehaviourMixin
+from behavysis_core.mixins.df_io_mixin import DFIOMixin
+from behavysis_core.mixins.io_mixin import IOMixin
+from behavysis_core.mixins.keypoints_mixin import KeypointsMixin
+from pydantic import BaseModel
 
 #####################################################################
 #               ANALYSIS API FUNCS
 #####################################################################
 
 
 class Analyse:
+    """__summary__"""
+
     @staticmethod
     def thigmotaxis(
         dlc_fp: str,
         analysis_dir: str,
         configs_fp: str,
     ) -> str:
         """
@@ -75,55 +62,61 @@
         """
         outcome = ""
         name = IOMixin.get_name(dlc_fp)
         out_dir = os.path.join(analysis_dir, Analyse.thigmotaxis.__name__)
         # Getting necessary config parameters
         configs = ExperimentConfigs.read_json(configs_fp)
         fps, _, _, px_per_mm, bins_ls, custom_bins_ls = get_analysis_configs(configs)
-        configs_filt = configs.user.analyse.thigmotaxis
-        thresh_mm = float(configs_filt.thresh_mm)
+        configs_filt = Model_in_roi(**configs.user.analyse.thigmotaxis)
+        bpts = configs_filt.bodyparts
         # Calculating more parameters
-        thresh_px = thresh_mm / px_per_mm
+        thresh_px = configs_filt.thresh_mm / px_per_mm
+
         # Loading in dataframe
         dlc_df = KeypointsMixin.clean_headings(DFIOMixin.read_feather(dlc_fp))
+        # Checking df
+        KeypointsMixin.check_df(dlc_df)
         # Getting indivs and bpts list
         indivs, _ = KeypointsMixin.get_headings(dlc_df)
 
         # Getting average corner coordinates. Assumes arena does not move.
-        tl = dlc_df[(SINGLE_COL, "TopLeft")].mean()
-        tr = dlc_df[(SINGLE_COL, "TopRight")].mean()
-        bl = dlc_df[(SINGLE_COL, "BottomLeft")].mean()
-        br = dlc_df[(SINGLE_COL, "BottomRight")].mean()
+        tl = dlc_df[(SINGLE_COL, configs_filt.roi_top_left)].mean()
+        tr = dlc_df[(SINGLE_COL, configs_filt.roi_top_right)].mean()
+        bl = dlc_df[(SINGLE_COL, configs_filt.roi_bottom_left)].mean()
+        br = dlc_df[(SINGLE_COL, configs_filt.roi_bottom_right)].mean()
         # Making boundary functions
         top = hline_factory(tl, tr)
         bottom = hline_factory(bl, br)
         left = vline_factory(tl, bl)
         right = vline_factory(tr, br)
 
         analysis_df = init_fbf_analysis_df(dlc_df.index, fps)
         dlc_df.index = analysis_df.index
+        idx = pd.IndexSlice
         for indiv in indivs:
-            indiv_x = dlc_df[(indiv, BODYCENTRE, "x")]
-            indiv_y = dlc_df[(indiv, BODYCENTRE, "y")]
+            indiv_x = dlc_df.loc[:, idx[indiv, bpts, "x"]].mean(axis=1)
+            indiv_y = dlc_df.loc[:, idx[indiv, bpts, "y"]].mean(axis=1)
             # Determining if the indiv is outside of the boundaries (with the thresh_px buffer)
             analysis_df[(indiv, "thigmotaxis")] = (
                 (indiv_y <= top(indiv_x) + thresh_px)
                 | (indiv_y >= bottom(indiv_x) - thresh_px)
                 | (indiv_x <= left(indiv_y) + thresh_px)
                 | (indiv_x >= right(indiv_y) - thresh_px)
             ).astype(np.int8)
         # Saving analysis_df
         fbf_fp = os.path.join(out_dir, "fbf", f"{name}.feather")
         DFIOMixin.write_feather(analysis_df, fbf_fp)
 
         # Generating scatterplot
         # Adding bodypoint x and y coords
         for indiv in indivs:
-            analysis_df[(indiv, "x")] = dlc_df[(indiv, BODYCENTRE, "x")]
-            analysis_df[(indiv, "y")] = dlc_df[(indiv, BODYCENTRE, "y")]
+            indiv_x = dlc_df.loc[:, idx[indiv, bpts, "x"]].mean(axis=1)
+            indiv_y = dlc_df.loc[:, idx[indiv, bpts, "y"]].mean(axis=1)
+            analysis_df[(indiv, "x")] = indiv_x
+            analysis_df[(indiv, "y")] = indiv_y
         # making corners_df
         corners_df = pd.DataFrame([tl, tr, bl, br])
         plot_fp = os.path.join(out_dir, "scatter_plot", f"{name}.png")
         make_location_scatterplot(analysis_df, corners_df, plot_fp, "thigmotaxis")
 
         # Summarising and binning analysis_df
         make_summary_binned(
@@ -150,67 +143,156 @@
         """
         outcome = ""
         name = IOMixin.get_name(dlc_fp)
         out_dir = os.path.join(analysis_dir, Analyse.center_crossing.__name__)
         # Getting necessary config parameters
         configs = ExperimentConfigs.read_json(configs_fp)
         fps, _, _, px_per_mm, bins_ls, custom_bins_ls = get_analysis_configs(configs)
-        configs_filt = configs.user.analyse.center_crossing
-        thresh_mm = float(configs_filt.thresh_mm)
+        configs_filt = Model_in_roi(**configs.user.analyse.center_crossing)
+        bpts = configs_filt.bodyparts
         # Calculating more parameters
-        thresh_px = thresh_mm / px_per_mm
+        thresh_px = configs_filt.thresh_mm / px_per_mm
+
         # Loading in dataframe
         dlc_df = KeypointsMixin.clean_headings(DFIOMixin.read_feather(dlc_fp))
+        # Checking df
+        KeypointsMixin.check_df(dlc_df)
         # Getting indivs and bpts list
         indivs, _ = KeypointsMixin.get_headings(dlc_df)
 
-        # Getting average corner coordinates. NOTE: assumes arena does not move.
-        tl = dlc_df[(SINGLE_COL, "TopLeft")].mean()
-        tr = dlc_df[(SINGLE_COL, "TopRight")].mean()
-        bl = dlc_df[(SINGLE_COL, "BottomLeft")].mean()
-        br = dlc_df[(SINGLE_COL, "BottomRight")].mean()
+        # Getting average corner coordinates. Assumes arena does not move.
+        tl = dlc_df[(SINGLE_COL, configs_filt.roi_top_left)].mean()
+        tr = dlc_df[(SINGLE_COL, configs_filt.roi_top_right)].mean()
+        bl = dlc_df[(SINGLE_COL, configs_filt.roi_bottom_left)].mean()
+        br = dlc_df[(SINGLE_COL, configs_filt.roi_bottom_right)].mean()
         # Making boundary functions
         top = hline_factory(tl, tr)
         bottom = hline_factory(bl, br)
         left = vline_factory(tl, bl)
         right = vline_factory(tr, br)
 
         analysis_df = init_fbf_analysis_df(dlc_df.index, fps)
         dlc_df.index = analysis_df.index
+        idx = pd.IndexSlice
         for indiv in indivs:
-            indiv_x = dlc_df[(indiv, BODYCENTRE, "x")]
-            indiv_y = dlc_df[(indiv, BODYCENTRE, "y")]
+            indiv_x = dlc_df.loc[:, idx[indiv, bpts, "x"]].mean(axis=1)
+            indiv_y = dlc_df.loc[:, idx[indiv, bpts, "y"]].mean(axis=1)
             # Determining if the indiv is outside of the boundaries (with the thresh_px buffer)
             analysis_df[(indiv, "in_center")] = (
-                (indiv_y > top(indiv_x) + thresh_px)
-                & (indiv_y < bottom(indiv_x) - thresh_px)
-                & (indiv_x > left(indiv_y) + thresh_px)
-                & (indiv_x < right(indiv_y) - thresh_px)
+                (indiv_y >= top(indiv_x) + thresh_px)
+                & (indiv_y <= bottom(indiv_x) - thresh_px)
+                & (indiv_x >= left(indiv_y) + thresh_px)
+                & (indiv_x <= right(indiv_y) - thresh_px)
             ).astype(np.int8)
         # Saving analysis_df
         fbf_fp = os.path.join(out_dir, "fbf", f"{name}.feather")
         DFIOMixin.write_feather(analysis_df, fbf_fp)
 
         # Generating scatterplot
         # Adding bodypoint x and y coords
         for indiv in indivs:
-            analysis_df[(indiv, "x")] = dlc_df[(indiv, BODYCENTRE, "x")]
-            analysis_df[(indiv, "y")] = dlc_df[(indiv, BODYCENTRE, "y")]
+            indiv_x = dlc_df.loc[:, idx[indiv, bpts, "x"]].mean(axis=1)
+            indiv_y = dlc_df.loc[:, idx[indiv, bpts, "y"]].mean(axis=1)
+            analysis_df[(indiv, "x")] = indiv_x
+            analysis_df[(indiv, "y")] = indiv_y
         # making corners_df
         corners_df = pd.DataFrame([tl, tr, bl, br])
         plot_fp = os.path.join(out_dir, "scatter_plot", f"{name}.png")
         make_location_scatterplot(analysis_df, corners_df, plot_fp, "in_center")
 
         # Summarising and binning analysis_df
         make_summary_binned(
             DFIOMixin.read_feather(fbf_fp), out_dir, name, bins_ls, custom_bins_ls, True
         )
         return outcome
 
     @staticmethod
+    def in_roi(
+        dlc_fp: str,
+        analysis_dir: str,
+        configs_fp: str,
+    ) -> str:
+        """
+        Determines the frames in which the subject is inside the cage (from average
+        of given bodypoints).
+
+        Takes DLC data as input and returns the following analysis output:
+
+        - a feather file with the following columns for each video frame (row).
+        - a feather file with the summary statistics (sum, mean, std, min, median, Q1, median,
+        Q3, max) for DeltaMMperSec, and DeltaMMperSecSmoothed
+        - Each row `is_frozen`, and bout number.
+        """
+        outcome = ""
+        name = IOMixin.get_name(dlc_fp)
+        out_dir = os.path.join(analysis_dir, Analyse.in_roi.__name__)
+        # Calculating the deltas (changes in body position) between each frame for the subject
+        configs = ExperimentConfigs.read_json(configs_fp)
+        fps, _, _, px_per_mm, bins_ls, custom_bins_ls = get_analysis_configs(configs)
+        configs_filt = Model_in_roi(**configs.user.analyse.in_roi)
+        bpts = configs_filt.bodyparts
+        # Calculating more parameters
+        thresh_px = configs_filt.thresh_mm / px_per_mm
+
+        # Loading in dataframe
+        dlc_df = KeypointsMixin.clean_headings(DFIOMixin.read_feather(dlc_fp))
+        # Checking df
+        KeypointsMixin.check_df(dlc_df)
+        # Getting indivs and bpts list
+        indivs, bpts = KeypointsMixin.get_headings(dlc_df)
+        # Checking body-centre bodypart exists
+        KeypointsMixin.check_bpts_exist(dlc_df, bpts)
+
+        # Getting average corner coordinates. Assumes arena does not move.
+        tl = dlc_df[(SINGLE_COL, configs_filt.roi_top_left)].mean()
+        tr = dlc_df[(SINGLE_COL, configs_filt.roi_top_right)].mean()
+        bl = dlc_df[(SINGLE_COL, configs_filt.roi_bottom_left)].mean()
+        br = dlc_df[(SINGLE_COL, configs_filt.roi_bottom_right)].mean()
+        # Making boundary functions
+        top = hline_factory(tl, tr)
+        bottom = hline_factory(bl, br)
+        left = vline_factory(tl, bl)
+        right = vline_factory(tr, br)
+
+        analysis_df = init_fbf_analysis_df(dlc_df.index, fps)
+        dlc_df.index = analysis_df.index
+        idx = pd.IndexSlice
+        for indiv in indivs:
+            indiv_x = dlc_df.loc[:, idx[indiv, bpts, "x"]].mean(axis=1)
+            indiv_y = dlc_df.loc[:, idx[indiv, bpts, "y"]].mean(axis=1)
+            # Determining if the indiv is inside of the box region (with the thresh_px buffer)
+            analysis_df[(indiv, "in_roi")] = (
+                (indiv_y >= top(indiv_x) - thresh_px)
+                & (indiv_y <= bottom(indiv_x) + thresh_px)
+                & (indiv_x >= left(indiv_y) - thresh_px)
+                & (indiv_x <= right(indiv_y) + thresh_px)
+            ).astype(np.int8)
+        # Saving analysis_df
+        fbf_fp = os.path.join(out_dir, "fbf", f"{name}.feather")
+        DFIOMixin.write_feather(analysis_df, fbf_fp)
+
+        # Generating scatterplot
+        # Adding bodypoint x and y coords
+        for indiv in indivs:
+            indiv_x = dlc_df.loc[:, idx[indiv, bpts, "x"]].mean(axis=1)
+            indiv_y = dlc_df.loc[:, idx[indiv, bpts, "y"]].mean(axis=1)
+            analysis_df[(indiv, "x")] = indiv_x
+            analysis_df[(indiv, "y")] = indiv_y
+        # making corners_df
+        corners_df = pd.DataFrame([tl, tr, bl, br])
+        plot_fp = os.path.join(out_dir, "scatter_plot", f"{name}.png")
+        make_location_scatterplot(analysis_df, corners_df, plot_fp, "in_roi")
+
+        # Summarising and binning analysis_df
+        make_summary_binned(
+            DFIOMixin.read_feather(fbf_fp), out_dir, name, bins_ls, custom_bins_ls, True
+        )
+        return outcome
+
+    @staticmethod
     def speed(
         dlc_fp: str,
         analysis_dir: str,
         configs_fp: str,
     ) -> str:
         """
         Determines the speed of the subject in each frame.
@@ -223,37 +305,41 @@
         """
         outcome = ""
         name = IOMixin.get_name(dlc_fp)
         out_dir = os.path.join(analysis_dir, Analyse.speed.__name__)
         # Calculating the deltas (changes in body position) between each frame for the subject
         configs = ExperimentConfigs.read_json(configs_fp)
         fps, _, _, px_per_mm, bins_ls, custom_bins_ls = get_analysis_configs(configs)
-        configs_filt = configs.user.analyse.speed
-        smoothing_sec = configs_filt.smoothing_sec
+        configs_filt = Model_speed(**configs.user.analyse.speed)
+        bpts = configs_filt.bodyparts
         # Calculating more parameters
-        smoothing_frames = int(smoothing_sec * fps)
+        smoothing_frames = int(configs_filt.smoothing_sec * fps)
+
         # Loading in dataframe
         dlc_df = KeypointsMixin.clean_headings(DFIOMixin.read_feather(dlc_fp))
+        # Checking df
+        KeypointsMixin.check_df(dlc_df)
         # Getting indivs and bpts list
         indivs, _ = KeypointsMixin.get_headings(dlc_df)
         # Checking body-centre bodypart exists
-        KeypointsMixin.check_bpts_exist(dlc_df, [BODYCENTRE])
+        KeypointsMixin.check_bpts_exist(dlc_df, bpts)
 
         # Calculating speed of subject for each frame
         analysis_df = init_fbf_analysis_df(dlc_df.index, fps)
         dlc_df.index = analysis_df.index
+        idx = pd.IndexSlice
         for indiv in indivs:
             # Making a rolling window of 3?? maybe 4 frames for average body-centre
             # Otherwise jitter contributes to movement
             jitter_frames = 3
             smoothed_xy_df = dlc_df.rolling(
                 window=jitter_frames, center=True, min_periods=1
             ).agg(np.nanmean)
-            delta_x = smoothed_xy_df[(indiv, BODYCENTRE, "x")].diff()
-            delta_y = smoothed_xy_df[(indiv, BODYCENTRE, "y")].diff()
+            delta_x = smoothed_xy_df.loc[:, idx[indiv, bpts, "x"]].mean(axis=1).diff()
+            delta_y = smoothed_xy_df.loc[:, idx[indiv, bpts, "y"]].mean(axis=1).diff()
             delta = np.sqrt(np.power(delta_x, 2) + np.power(delta_y, 2))
             analysis_df[(indiv, "SpeedMMperSec")] = (delta / px_per_mm) * fps
             analysis_df[(indiv, "SpeedMMperSecSmoothed")] = (
                 analysis_df[(indiv, "SpeedMMperSec")]
                 .rolling(window=smoothing_frames, min_periods=1)
                 .agg(np.nanmean)
             )
@@ -289,34 +375,40 @@
         """
         outcome = ""
         name = IOMixin.get_name(dlc_fp)
         out_dir = os.path.join(analysis_dir, Analyse.social_distance.__name__)
         # Calculating the deltas (changes in body position) between each frame for the subject
         configs = ExperimentConfigs.read_json(configs_fp)
         fps, _, _, px_per_mm, bins_ls, custom_bins_ls = get_analysis_configs(configs)
-        configs_filt = configs.user.analyse.social_distance
-        smoothing_sec = configs_filt.smoothing_sec
+        configs_filt = Model_social_distance(**configs.user.analyse.social_distance)
+        bpts = configs_filt.bodyparts
         # Calculating more parameters
-        smoothing_frames = int(smoothing_sec * fps)
+        smoothing_frames = int(configs_filt.smoothing_sec * fps)
+
         # Loading in dataframe
         dlc_df = KeypointsMixin.clean_headings(DFIOMixin.read_feather(dlc_fp))
-        KeypointsMixin.check_bpts_exist(dlc_df, [BODYCENTRE])
+        # Checking df
+        KeypointsMixin.check_df(dlc_df)
         # Getting indivs and bpts list
         indivs, _ = KeypointsMixin.get_headings(dlc_df)
+        # Checking body-centre bodypart exists
+        KeypointsMixin.check_bpts_exist(dlc_df, bpts)
 
         # Calculating speed of subject for each frame
         analysis_df = init_fbf_analysis_df(dlc_df.index, fps)
         dlc_df.index = analysis_df.index
+        idx = pd.IndexSlice
         # Assumes there are only two individuals
         indiv_a = indivs[0]
         indiv_b = indivs[1]
-        bpt = "Nose"
         # Getting distances between each individual
-        dist_x = dlc_df[(indiv_a, bpt, "x")] - dlc_df[(indiv_b, bpt, "x")]
-        dist_y = dlc_df[(indiv_a, bpt, "y")] - dlc_df[(indiv_b, bpt, "y")]
+        idx_a = idx[indiv_b, bpts, "x"]
+        dist_x = (dlc_df.loc[:, idx_a] - dlc_df.loc[:, idx_a]).mean(axis=1)
+        idx_b = idx[indiv_a, bpts, "y"]
+        dist_y = (dlc_df.loc[:, idx_b] - dlc_df.loc[:, idx_b]).mean(axis=1)
         dist = np.sqrt(np.power(dist_x, 2) + np.power(dist_y, 2))
         # Adding mm distance to saved analysis_df table
         analysis_df[(f"{indiv_a}_{indiv_b}", "DistMM")] = dist / px_per_mm
         analysis_df[(f"{indiv_a}_{indiv_b}", "DistMMSmoothed")] = (
             analysis_df[(f"{indiv_a}_{indiv_b}", "DistMM")]
             .rolling(window=smoothing_frames, min_periods=1)
             .agg(np.nanmean)
@@ -359,24 +451,24 @@
         """
         outcome = ""
         name = IOMixin.get_name(dlc_fp)
         out_dir = os.path.join(analysis_dir, Analyse.freezing.__name__)
         # Calculating the deltas (changes in body position) between each frame for the subject
         configs = ExperimentConfigs.read_json(configs_fp)
         fps, _, _, px_per_mm, bins_ls, custom_bins_ls = get_analysis_configs(configs)
-        configs_filt = configs.user.analyse.freezing
-        window_sec = configs_filt.window_sec
-        thresh_mm = configs_filt.thresh_mm
-        smoothing_sec = configs_filt.smoothing_sec
+        configs_filt = Model_freezing(**configs.user.analyse.freezing)
         # Calculating more parameters
-        thresh_px = thresh_mm / px_per_mm
-        smoothing_frames = int(smoothing_sec * fps)
-        window_frames = int(np.round(fps * window_sec, 0))
+        thresh_px = configs_filt.thresh_mm / px_per_mm
+        smoothing_frames = int(configs_filt.smoothing_sec * fps)
+        window_frames = int(np.round(fps * configs_filt.window_sec, 0))
+
         # Loading in dataframe
         dlc_df = KeypointsMixin.clean_headings(DFIOMixin.read_feather(dlc_fp))
+        # Checking df
+        KeypointsMixin.check_df(dlc_df)
         # Getting indivs and bpts list
         indivs, bpts = KeypointsMixin.get_headings(dlc_df)
 
         # Calculating speed of subject for each frame
         analysis_df = init_fbf_analysis_df(dlc_df.index, fps)
         dlc_df.index = analysis_df.index
         for indiv in indivs:
@@ -453,16 +545,15 @@
         configs.user.analyse.custom_bins_sec,
     )
 
 
 def init_fbf_analysis_df(frame_vect: pd.Series | pd.Index, fps: int) -> pd.DataFrame:
     """
     Returning a frame-by-frame analysis_df with the frame number (according to original video)
-    and timestamps as the MultiIndex index, according to when the "experiment" begins
-    (i.e., the first frame in the frame_vect).
+    and timestamps as the MultiIndex index, relative to the first element of frame_vect.
     Note that that the frame number can thus begin on a non-zero number.
 
     Parameters
     ----------
     frame_vect : pd.Series | pd.Index
         _description_
     fps : int
@@ -533,14 +624,15 @@
     # Setting fig titles and labels
     g.set_titles(col_template="{col_name}")
     g.figure.subplots_adjust(top=0.85)
     g.figure.suptitle("Spatial position", fontsize=12)
     # Saving fig
     os.makedirs(os.path.split(out_fp)[0], exist_ok=True)
     g.savefig(out_fp)
+    g.figure.clf()
 
 
 def _make_summary_quantitative(
     analysis_df: pd.DataFrame,
     out_fp: str,
 ) -> str:
     """
@@ -630,43 +722,39 @@
     DFIOMixin.write_feather(summary_df, out_fp)
     return outcome
 
 
 def _make_binned(
     analysis_df: pd.DataFrame,
     out_fp: str,
-    bins: float | list,
+    bins: list,
 ) -> str:
     """
     Generates the binned data and line graph for the given analysis_df, and given bin_sec.
 
     # TODO - should this be user-changeable?
     # TODO - for behaviour (binary), make a bout frequency stat (binned) and mean bout time (binned)
 
     Parameters
     ----------
     analysis_df : pd.DataFrame
         _description_
     out_fp : str
         _description_
-    bins : float | list
+    bins : list
         _description_
 
     Returns
     -------
     str
         _description_
     """
     # For each column, displays the mean of each binned group.
     outcome = ""
     timestamps = analysis_df.index.get_level_values("timestamp")
-    # If bins is a float, then making even-interval bins list.
-    # Otherwise, using the bins list given
-    if isinstance(bins, float):
-        bins = np.arange(np.min(timestamps), np.max(timestamps) + bins, bins)
     # Ensuring all bins are included (start frame and end frame)
     if np.min(bins) > 0:  # If 0 is not included
         bins = np.append(0, bins)
     if np.max(bins) < np.max(timestamps):  # If end timestamp is not included
         bins = np.append(bins, np.max(timestamps))
     # Making binned data
     bin_sec = pd.cut(timestamps, bins=bins, labels=bins[1:], include_lowest=True)
@@ -725,14 +813,16 @@
     g.figure.subplots_adjust(top=0.85)
     g.figure.suptitle("Binned data", fontsize=12)
     if is_bool:
         g.set(ylim=(0, 1))
     # Saving fig
     os.makedirs(os.path.split(out_fp)[0], exist_ok=True)
     g.savefig(out_fp)
+    g.figure.clf()
+    # Returning outcome
     return outcome
 
 
 def make_summary_binned(
     analysis_df: pd.DataFrame,
     out_dir: str,
     name: str,
@@ -766,20 +856,23 @@
     outcome = ""
     # Summarising analysis_df
     summary_fp = os.path.join(out_dir, "summary", f"{name}.feather")
     if is_bool:
         outcome += _make_summary_behaviour(analysis_df, summary_fp)
     else:
         outcome += _make_summary_quantitative(analysis_df, summary_fp)
+    # Getting timestamps index
+    timestamps = analysis_df.index.get_level_values("timestamp")
     # Binning analysis_df
     for bin_sec in bins_ls:
         binned_fp = os.path.join(out_dir, f"binned_{bin_sec}", f"{name}.feather")
         binned_plot_fp = os.path.join(out_dir, f"binned_{bin_sec}_plot", f"{name}.png")
         # Making binned df
-        outcome += _make_binned(analysis_df, binned_fp, bin_sec)
+        bins = np.arange(np.min(timestamps), np.max(timestamps) + bin_sec, bin_sec)
+        outcome += _make_binned(analysis_df, binned_fp, bins)
         # Making binned plots
         outcome += _make_binned_plot(
             DFIOMixin.read_feather(binned_fp), binned_plot_fp, is_bool
         )
     # Custom binning analysis_df
     binned_fp = os.path.join(out_dir, "binned_custom", f"{name}.feather")
     binned_plot_fp = os.path.join(out_dir, "binned_custom_plot", f"{name}.png")
@@ -804,7 +897,40 @@
 def vline_factory(p1, p2):
     """
     Boundary function factories (y input to x).
     Making boundary line, given corner points. Expects input to be y
     m = (x2-x1)/(y2-y1)   &   x = m(y-y1) + b + x1
     """
     return lambda y: (p2["x"] - p1["x"]) / (p2["y"] - p1["y"]) * (y - p1["y"]) + p1["x"]
+
+
+class Model_speed(BaseModel):
+    """_summary_"""
+
+    smoothing_sec: float
+    bodyparts: list[str]
+
+
+class Model_social_distance(BaseModel):
+    """_summary_"""
+
+    smoothing_sec: float
+    bodyparts: list[str]
+
+
+class Model_freezing(BaseModel):
+    """_summary_"""
+
+    window_sec: float
+    thresh_mm: float
+    smoothing_sec: float
+
+
+class Model_in_roi(BaseModel):
+    """_summary_"""
+
+    thresh_mm: float
+    roi_top_left: str
+    roi_top_right: str
+    roi_bottom_left: str
+    roi_bottom_right: str
+    bodyparts: list[str]
```

### Comparing `behavysis_pipeline-0.1.0/behavysis_pipeline/processes/calculate_params.py` & `behavysis_pipeline-0.1.1/behavysis_pipeline/processes/calculate_params.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 -------
 str
     The outcome of the process.
 """
 
 import numpy as np
 import pandas as pd
+from behavysis_core.constants import SINGLE_COL
+from behavysis_core.data_models.experiment_configs import ExperimentConfigs
 from behavysis_core.mixins.df_io_mixin import DFIOMixin
 from behavysis_core.mixins.keypoints_mixin import KeypointsMixin
-from behavysis_core.utils.constants import SINGLE_COL
-
-from behavysis_pipeline.pipeline.experiment_configs import ExperimentConfigs
+from pydantic import BaseModel
 
 
 class CalculateParams:
     """__summary__"""
 
     @staticmethod
     def start_frame(
@@ -39,38 +39,42 @@
         existing in each frame across the sliding window is greater than the defined pcutoff, then
         the determine this as the start time.
 
         Notes
         -----
         The config file must contain the following parameters:
         ```
-        - (user, auto)
+        - user
             - calculate_params
                 - start_frame
                     - window_sec: float
                     - pcutoff: float
         ```
         """
         outcome = ""
         # Getting necessary config parameters
         configs = ExperimentConfigs.read_json(configs_fp)
-        configs_filt = configs.user.calculate_params.start_frame
+        configs_filt = Model_start_frame(**configs.user.calculate_params.start_frame)
         bpts = configs_filt.bodyparts
         window_sec = configs_filt.window_sec
         pcutoff = configs_filt.pcutoff
         fps = configs.auto.formatted_vid.fps
         # Deriving more parameters
         window_frames = int(np.round(fps * window_sec, 0))  # for rounding
         # Loading dataframe
         dlc_df = DFIOMixin.read_feather(dlc_fp)
+        # Imputing missing values with 0 (only really relevant for "likelihood" columns)
+        dlc_df = dlc_df.fillna(0)
+        # Checking that the two reference points are valid
+        KeypointsMixin.check_bpts_exist(dlc_df, bpts)
         # Calculating likelihood of subject existing.
         idx = pd.IndexSlice
         df_lhoods = pd.DataFrame(index=dlc_df.index)
         df_lhoods["current"] = dlc_df.loc[:, idx[:, :, bpts, "likelihood"]].apply(
-            np.nanmedian, axis=1
+            np.nanmean, axis=1
         )
         # Calculating likelihood of subject existing over time window
         df_lhoods["rolling"] = (
             df_lhoods["current"].rolling(window_frames).agg(np.nanmedian)
         )
         # Determining start time. Start frame is the first frame of the rolling window's range
         try:
@@ -103,15 +107,15 @@
         ```
         TODO
         ```
         """
         outcome = ""
         # Getting necessary config parameters
         configs = ExperimentConfigs.read_json(configs_fp)
-        configs_filt = configs.user.calculate_params.stop_frame
+        configs_filt = Model_stop_frame(**configs.user.calculate_params.stop_frame)
         dur_sec = configs_filt.dur_sec
         start_frame = configs.auto.start_frame
         fps = configs.auto.formatted_vid.fps
         auto_stop_frame = configs.auto.formatted_vid.total_frames
         # Calculating stop_frame
         dur_frames = int(dur_sec * fps)
         stop_frame = start_frame + dur_frames
@@ -141,43 +145,74 @@
         the px to mm
         conversion.
 
         Notes
         -----
         The config file must contain the following parameters:
         ```
-        - (user, auto)
+        - user
             - calculate_params
                 - px_per_mm
                     - point_a: str
                     - point_b: str
                     - dist_mm: float
         ```
         """
         outcome = ""
         # Getting necessary config parameters
         configs = ExperimentConfigs.read_json(configs_fp)
-        configs_filt = configs.user.calculate_params.px_per_mm
+        configs_filt = Model_px_per_mm(**configs.user.calculate_params.px_per_mm)
         pt_a = configs_filt.pt_a
         pt_b = configs_filt.pt_b
+        pcutoff = configs_filt.pcutoff
         dist_mm = configs_filt.dist_mm
         # Loading dataframe
         dlc_df = KeypointsMixin.clean_headings(DFIOMixin.read_feather(dlc_fp))
+        # Imputing missing values with 0 (only really relevant for "likelihood" columns)
+        dlc_df = dlc_df.fillna(0)
         # Checking that the two reference points are valid
         KeypointsMixin.check_bpts_exist(dlc_df, [pt_a, pt_b])
         # Finding the arena height and width in pixels
         pt_a_df = dlc_df[SINGLE_COL, pt_a]
         pt_b_df = dlc_df[SINGLE_COL, pt_b]
-        dist_px = np.mean(
+        # Interpolating points
+        pt_a_df.loc[pt_a_df["likelihood"] < pcutoff] = np.nan
+        pt_a_df = pt_a_df.interpolate(method="linear", axis=0).bfill()
+        pt_b_df.loc[pt_b_df["likelihood"] < pcutoff] = np.nan
+        pt_b_df = pt_b_df.interpolate(method="linear", axis=0).bfill()
+        # Getting distances
+        dist_px = np.nanmean(
             np.sqrt(
                 np.square(pt_a_df["x"] - pt_b_df["x"])
                 + np.square(pt_a_df["y"] - pt_b_df["y"])
             )
         )
         # Finding pixels per mm conversion, using the given arena width and height as calibration
         px_per_mm = dist_px / dist_mm
         # Saving to configs file
         configs = ExperimentConfigs.read_json(configs_fp)
         configs.auto.px_per_mm = px_per_mm
         configs.write_json(configs_fp)
         return outcome
-        return outcome
+
+
+class Model_start_frame(BaseModel):
+    """_summary_"""
+
+    bodyparts: list[str] = []
+    window_sec: float = 0
+    pcutoff: float = 0
+
+
+class Model_stop_frame(BaseModel):
+    """_summary_"""
+
+    dur_sec: float = 0
+
+
+class Model_px_per_mm(BaseModel):
+    """_summary_"""
+
+    pt_a: str = "pt_a"
+    pt_b: str = "pt_b"
+    pcutoff: int = 0
+    dist_mm: float = 0
```

### Comparing `behavysis_pipeline-0.1.0/behavysis_pipeline/processes/classify_behaviours.py` & `behavysis_pipeline-0.1.1/behavysis_pipeline/processes/classify_behaviours.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 Classify Behaviours
 """
 
 import os
 
 import numpy as np
 import pandas as pd
+from behavysis_core.constants import BEHAV_COLUMN_NAMES, BEHAV_PRED_COL
+from behavysis_core.data_models.experiment_configs import ExperimentConfigs
 from behavysis_core.mixins.behaviour_mixin import BehaviourMixin
 from behavysis_core.mixins.df_io_mixin import DFIOMixin
 from behavysis_core.mixins.diagnostics_mixin import DiagnosticsMixin
-from behavysis_core.utils.constants import BEHAV_COLUMN_NAMES, BEHAV_PRED_COL
 
 from behavysis_pipeline.behav_classifier import BehavClassifier
-from behavysis_pipeline.pipeline.experiment_configs import ExperimentConfigs
+
+# TODO: handle reading the model file whilst in multiprocessing
 
 
 class ClassifyBehaviours:
     """__summary__"""
 
     @staticmethod
     def classify_behaviours(
@@ -45,15 +47,15 @@
         str
             Description of the function's outcome.
 
         Notes
         -----
         The config file must contain the following parameters:
         ```
-        - (user, auto)
+        - user
             - classify_behaviours
                 - models: list[str]
         ```
         Where the `models` list is a list of `model_config.json` filepaths.
         """
         outcome = ""
         # If overwrite is False, checking if we should skip processing
```

### Comparing `behavysis_pipeline-0.1.0/behavysis_pipeline/processes/evaluate.py` & `behavysis_pipeline-0.1.1/behavysis_pipeline/processes/evaluate.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,42 +30,30 @@
 from typing import Callable, Sequence
 
 import cv2
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
-from behavysis_core.mixins.df_io_mixin import DFIOMixin
-from behavysis_core.mixins.diagnostics_mixin import DiagnosticsMixin
-from behavysis_core.mixins.io_mixin import IOMixin
-from behavysis_core.mixins.keypoints_mixin import KeypointsMixin
-from behavysis_core.utils.constants import (
+from behavysis_core.constants import (
     BEHAV_ACTUAL_COL,
     BEHAV_COLUMN_NAMES,
     BEHAV_PRED_COL,
     BEHAV_PROB_COL,
     PLOT_DPI,
     PLOT_STYLE,
     PROCESS_COL,
 )
+from behavysis_core.data_models.experiment_configs import ExperimentConfigs
+from behavysis_core.mixins.df_io_mixin import DFIOMixin
+from behavysis_core.mixins.diagnostics_mixin import DiagnosticsMixin
+from behavysis_core.mixins.io_mixin import IOMixin
+from behavysis_core.mixins.keypoints_mixin import KeypointsMixin
 from tqdm import trange
 
-from behavysis_pipeline.pipeline.experiment_configs import ExperimentConfigs
-
-#####################################################################
-#               INITIALISE MPL PLOTTING PARAMETERS
-#####################################################################
-
-
-sns.set_theme(style=PLOT_STYLE)
-
-plt.rcParams["figure.dpi"] = PLOT_DPI
-plt.rcParams["savefig.dpi"] = PLOT_DPI
-
-
 #####################################################################
 #               MAKE KEYPOINTS PLOTS
 #####################################################################
 
 
 class Evaluate:
     @staticmethod
@@ -113,14 +101,15 @@
             y="likelihood",
             hue="bodyparts",
             alpha=0.4,
         )
         g.add_legend()
         # Saving plot
         g.savefig(out_fp)
+        g.figure.clf()
         # Returning outcome string
         return outcome
 
     #####################################################################
     #               MAKE KEYPOINTS VIDEO
     #####################################################################
```

### Comparing `behavysis_pipeline-0.1.0/behavysis_pipeline/processes/extract_features.py` & `behavysis_pipeline-0.1.1/behavysis_pipeline/processes/extract_features.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 _summary_
 """
 
 import os
 import shutil
 
 import pandas as pd
+from behavysis_core.data_models.experiment_configs import ExperimentConfigs
 from behavysis_core.mixins.df_io_mixin import DFIOMixin
 from behavysis_core.mixins.diagnostics_mixin import DiagnosticsMixin
 from behavysis_core.mixins.io_mixin import IOMixin
 from behavysis_core.mixins.keypoints_mixin import KeypointsMixin
-from behavysis_core.mixins.subprocess_mixin import SubprocessMixin
-
-from behavysis_pipeline.pipeline.experiment_configs import ExperimentConfigs
+from behavysis_core.mixins.multiproc_mixin import MultiprocMixin
+from behavysis_core.mixins.subproc_mixin import SubprocMixin
 
 # Order of bodyparts is from
 # - https://github.com/sgoldenlab/simba/blob/master/docs/Multi_animal_pose.md
 # - https://github.com/sgoldenlab/simba/blob/master/docs/Tutorial_DLC.md
 # - https://github.com/sgoldenlab/simba/blob/master/simba/pose_configurations/bp_names/bp_names.csv
 # - https://github.com/sgoldenlab/simba/blob/master/simba/pose_configurations/configuration_names/pose_config_names.csv
 # And can also double check by looking at the order in "project_folder\csv\input_csv" files.
@@ -29,15 +29,14 @@
 class ExtractFeatures:
     @staticmethod
     def extract_features(
         dlc_fp: str,
         out_fp: str,
         configs_fp: str,
         temp_dir: str,
-        remove_temp: bool,
         overwrite: bool,
     ) -> str:
         """
         Extracting features from preprocessed DLC dataframe using SimBA
         processes.
 
         Parameters
@@ -46,59 +45,58 @@
             Preprocessed DLC filepath.
         out_fp : str
             Filepath to save extracted_features dataframe.
         configs_fp : str
             Configs JSON filepath.
         temp_dir : str
             Temporary directory path. Used during intermediate SimBA processes.
-        remove_temp : bool
-            Whether to remove the temp directory.
         overwrite : bool
             Whether to overwrite the out_fp file (if it exists).
 
         Returns
         -------
         str
             The outcome of the process.
         """
         outcome = ""
         # If overwrite is False, checking if we should skip processing
         if not overwrite and os.path.exists(out_fp):
             return DiagnosticsMixin.warning_msg()
         # Getting directory and file paths
         name = IOMixin.get_name(dlc_fp)
+        cpid = MultiprocMixin.get_cpid()
         configs_dir = os.path.split(configs_fp)[0]
-        simba_in_dir = os.path.join(temp_dir, "input")
-        simba_dir = os.path.join(temp_dir, "simba_proj")
+        simba_in_dir = os.path.join(temp_dir, f"input_{cpid}")
+        simba_dir = os.path.join(temp_dir, f"simba_proj_{cpid}")
         features_from_dir = os.path.join(
             simba_dir, "project_folder", "csv", "features_extracted"
         )
         # Preparing dlc dfs for input to SimBA project
         os.makedirs(simba_in_dir, exist_ok=True)
         simba_in_fp = os.path.join(simba_in_dir, f"{name}.csv")
         # TODO: order mousemarked and mouseunmarked correctly as 1 and 2
         # Selecting bodyparts for SimBA (8 bpts, 2 indivs)
         df = DFIOMixin.read_feather(dlc_fp)
         df = select_cols(df, configs_fp)
         # Saving dlc frame to place in the SimBA features extraction df
         index = df.index
         # Saving as csv
         df.to_csv(simba_in_fp)
+        # Removing simba folder (if it exists)
+        if os.path.exists(simba_dir):
+            shutil.rmtree(simba_dir)
         # Running SimBA env and script to run SimBA feature extraction
         outcome += run_extract_features_script(simba_dir, simba_in_dir, configs_dir)
         # Reading SimBA feature extraction csv (to select column and convert to feather)
         simba_out_fp = os.path.join(features_from_dir, f"{name}.csv")
         df = pd.read_csv(simba_out_fp, header=0, index_col=0)
         # Setting index to same as dlc preprocessed df
         df.index = index
         # Saving SimBA extracted features df as feather
         DFIOMixin.write_feather(df, out_fp)
-        # Removing temp dir
-        if remove_temp:
-            shutil.rmtree(temp_dir, ignore_errors=True)
         # Returning outcome
         return outcome
 
 
 #####################################################################
 #               PREPARE FOR SIMBA
 #####################################################################
@@ -162,24 +160,24 @@
         For each DLC dataframe file, there should be a config file with the same name.
     """
     cmd = [
         os.environ["CONDA_EXE"],
         "run",
         "--no-capture-output",
         "-n",
-        "simba_wrapper_env",
+        "simba_subproc_env",
         "python",
         "-m",
-        "simbehavysis_pipeline.extract_features",
+        "simba_subproc",
         simba_dir,
         dlc_dir,
         configs_dir,
     ]
-    # SubprocessMixin.run_subprocess_fstream(cmd)
-    SubprocessMixin.run_subprocess_console(cmd)
+    # SubprocMixin.run_subproc_fstream(cmd)
+    SubprocMixin.run_subproc_console(cmd)
     return "Ran SimBA feature extraction script.\n"
 
 
 def remove_bpts_cols(
     df: pd.DataFrame,
 ) -> pd.DataFrame:
     """
@@ -197,8 +195,7 @@
         Features extracted dataframe with the bodyparts columns dropped.
     """
     indivs_n = 2
     bpts_n = 8
     coords_n = 3
     n = indivs_n * bpts_n * coords_n
     return df.iloc[:, n:]
-    return df.iloc[:, n:]
```

### Comparing `behavysis_pipeline-0.1.0/behavysis_pipeline/processes/format_vid.py` & `behavysis_pipeline-0.1.1/behavysis_pipeline/processes/format_vid.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,19 +16,18 @@
 -------
 str
     Description of the function's outcome.
 """
 
 import os
 
+from behavysis_core.data_models.experiment_configs import ExperimentConfigs
 from behavysis_core.mixins.diagnostics_mixin import DiagnosticsMixin
 from behavysis_core.mixins.process_vid_mixin import ProcessVidMixin
 
-from behavysis_pipeline.pipeline.experiment_configs import ExperimentConfigs
-
 
 class FormatVid:
     """
     Class for formatting videos based on given parameters.
     """
 
     @staticmethod
```

### Comparing `behavysis_pipeline-0.1.0/behavysis_pipeline/processes/preprocess.py` & `behavysis_pipeline-0.1.1/behavysis_pipeline/processes/preprocess.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,182 +16,198 @@
 -------
 str
     Description of the function's outcome.
 
 """
 
 import os
+from typing import Literal
 
 import numpy as np
 import pandas as pd
+from behavysis_core.constants import SINGLE_COL
+from behavysis_core.data_models.experiment_configs import ExperimentConfigs
 from behavysis_core.mixins.df_io_mixin import DFIOMixin
 from behavysis_core.mixins.diagnostics_mixin import DiagnosticsMixin
 from behavysis_core.mixins.keypoints_mixin import KeypointsMixin
-from behavysis_core.utils.constants import BODYCENTRE, SINGLE_COL
-
-from behavysis_pipeline.pipeline.experiment_configs import ExperimentConfigs
+from pydantic import BaseModel
 
 
 class Preprocess:
     """_summary_"""
 
     @staticmethod
+    def import_keypoints_df(
+        in_fp: str, out_fp: str, configs_fp: str, overwrite: bool
+    ) -> str:
+        """ """
+        outcome = ""
+        # If overwrite is False, checking if we should skip processing
+        if not overwrite and os.path.exists(out_fp):
+            return DiagnosticsMixin.warning_msg()
+        # Reading file
+        df = DFIOMixin.read_feather(in_fp)
+        # Writing file
+        DFIOMixin.write_feather(df, out_fp)
+        # Returning outcome
+        outcome += "Imported keypoints dataframe."
+        return outcome
+
+    @staticmethod
     def start_stop_trim(
-        in_fp: str,
-        out_fp: str,
-        configs_fp: str,
-        overwrite: bool,
+        in_fp: str, out_fp: str, configs_fp: str, overwrite: bool
     ) -> str:
         """
         Filters the rows of a DLC formatted dataframe to include only rows within the start
         and end time of the experiment, given a corresponding configs dict.
 
+        Parameters
+        ----------
+        in_fp : str
+            The file path of the input DLC formatted dataframe.
+        out_fp : str
+            The file path of the output trimmed dataframe.
+        configs_fp : str
+            The file path of the configs dict.
+        overwrite : bool
+            If True, overwrite the output file if it already exists. If False, skip processing
+            if the output file already exists.
+
+        Returns
+        -------
+        str
+            An outcome message indicating the result of the trimming process.
+
         Notes
         -----
         The config file must contain the following parameters:
         ```
-        - (user, auto)
+        - user
             - preprocess
                 - start_stop_trim
                     - start_frame: int
                     - stop_frame: int
         ```
         """
         outcome = ""
         # If overwrite is False, checking if we should skip processing
         if not overwrite and os.path.exists(out_fp):
             return DiagnosticsMixin.warning_msg()
+
         # Getting necessary config parameters
         configs = ExperimentConfigs.read_json(configs_fp)
         start_frame = configs.auto.start_frame
         stop_frame = configs.auto.stop_frame
+
         # Reading file
         df = DFIOMixin.read_feather(in_fp)
+
         # Trimming dataframe
         df = df.loc[start_frame:stop_frame, :]
+
         # Writing file
         DFIOMixin.write_feather(df, out_fp)
+
         return outcome
 
     @staticmethod
-    def interpolate_points(
-        in_fp: str,
-        out_fp: str,
-        configs_fp: str,
-        overwrite: bool,
-    ) -> str:
+    def interpolate(in_fp: str, out_fp: str, configs_fp: str, overwrite: bool) -> str:
         """
         "Smooths" out noticeable jitter of points, where the likelihood (and accuracy) of
         a point's coordinates are low (e.g., when the subject's head goes out of view). It
         does this by linearly interpolating the frames of a body part that are below a given
         likelihood pcutoff.
 
         Notes
         -----
         The config file must contain the following parameters:
         ```
-        - (user, auto)
+        - user
             - preprocess
-                - interpolate_points
+                - interpolate
                     - pcutoff: float
         ```
         """
         outcome = ""
         # If overwrite is False, checking if we should skip processing
         if not overwrite and os.path.exists(out_fp):
             return DiagnosticsMixin.warning_msg()
         # Getting necessary config parameters
         configs = ExperimentConfigs.read_json(configs_fp)
-        configs_filt = configs.user.preprocess.interpolate_points
-        pcutoff = configs_filt.pcutoff
+        configs_filt = Model_interpolate(**configs.user.preprocess.interpolate)
         # Reading file
         df = DFIOMixin.read_feather(in_fp)
         # Gettings the unique groups of (individual, bodypart) groups.
         unique_cols = df.columns.droplevel(["coords"]).unique()
         # Setting low-likelihood points to Nan to later interpolate
         for scorer, indiv, bp in unique_cols:
-            try:
-                # Imputing Nan likelihood points with 0
-                df[(scorer, indiv, bp, "likelihood")].fillna(value=0, inplace=True)
-                # Setting x and y coordinates of points that have low likelihood to Nan
-                to_remove = df[(scorer, indiv, bp, "likelihood")] < pcutoff
-                df.loc[to_remove, (scorer, indiv, bp, "x")] = np.nan
-                df.loc[to_remove, (scorer, indiv, bp, "y")] = np.nan
-            except KeyError:
-                pass
+            # Imputing Nan likelihood points with 0
+            df[(scorer, indiv, bp, "likelihood")].fillna(value=0, inplace=True)
+            # Setting x and y coordinates of points that have low likelihood to Nan
+            to_remove = df[(scorer, indiv, bp, "likelihood")] < configs_filt.pcutoff
+            df.loc[to_remove, (scorer, indiv, bp, "x")] = np.nan
+            df.loc[to_remove, (scorer, indiv, bp, "y")] = np.nan
         # linearly interpolating Nan x and y points. Also backfilling points at the start.
         df = df.interpolate(method="linear", axis=0).bfill()
         # Writing file
         DFIOMixin.write_feather(df, out_fp)
         return outcome
 
-    @staticmethod
-    def bodycentre(
-        in_fp: str,
-        out_fp: str,
-        configs_fp: str,
-        overwrite: bool,
-    ) -> str:
-        """
-        Calculates the body centre of the subject in each frame, given the body parts to
-        consider in the configs. The calculation used is the mean of all the body parts to consider.
-        A new column is added called "name", with "x" and "y" sub-columns (does not include a
-        "likelihood" column).
-
-        Notes
-        -----
-        The config file must contain the following parameters:
-        ```
-        - (user, auto)
-            - preprocess
-                - interpolate_points
-                    - pcutoff: float
-        ```
-        """
-        outcome = ""
-        # If overwrite is False, checking if we should skip processing
-        if not overwrite and os.path.exists(out_fp):
-            return DiagnosticsMixin.warning_msg()
-        # Reading file
-        df = DFIOMixin.read_feather(in_fp)
-        # Getting indivs and bpts list
-        indivs, _ = KeypointsMixin.get_headings(df)
-        # Getting necessary config parameters
-        configs = ExperimentConfigs.read_json(configs_fp)
-        configs_filt = configs.user.preprocess.bodycentre
-        bpts = configs_filt.bodyparts
-        # Checking that the bodyparts are all valid
-        KeypointsMixin.check_bpts_exist(df, bpts)
-        # Calculating the body centre in each frame for each individual
-        l0 = df.columns.unique(0)[0]
-        idx = pd.IndexSlice
-        for indiv in indivs:
-            for coord in ["x", "y", "likelihood"]:
-                df[l0, indiv, BODYCENTRE, coord] = df.loc[
-                    :, idx[l0, indiv, bpts, coord]
-                ].apply(np.nanmean, axis=1)
-        # Writing file
-        DFIOMixin.write_feather(df, out_fp)
-        return outcome
+    # @staticmethod
+    # def bodycentre(
+    #     in_fp: str,
+    #     out_fp: str,
+    #     configs_fp: str,
+    #     overwrite: bool,
+    # ) -> str:
+    #     """
+    #     Calculates the body centre of the subject in each frame, given the body parts to
+    #     consider in the configs. The calculation used is the mean of all the body parts to
+    #     consider.
+    #     A new column is added called "name", with "x" and "y" sub-columns (does not include a
+    #     "likelihood" column).
+    #     """
+    #     outcome = ""
+    #     # If overwrite is False, checking if we should skip processing
+    #     if not overwrite and os.path.exists(out_fp):
+    #         return DiagnosticsMixin.warning_msg()
+    #     # Reading file
+    #     df = DFIOMixin.read_feather(in_fp)
+    #     # Getting indivs and bpts list
+    #     indivs, _ = KeypointsMixin.get_headings(df)
+    #     # Getting necessary config parameters
+    #     configs = ExperimentConfigs.read_json(configs_fp)
+    #     configs_filt = configs.user.preprocess.bodycentre
+    #     bpts = configs_filt.bodyparts
+    #     # Checking that the bodyparts are all valid
+    #     KeypointsMixin.check_bpts_exist(df, bpts)
+    #     # Calculating the body centre in each frame for each individual
+    #     l0 = df.columns.unique(0)[0]
+    #     idx = pd.IndexSlice
+    #     for indiv in indivs:
+    #         for coord in ["x", "y", "likelihood"]:
+    #             x = df.loc[:, idx[l0, indiv, bpts, coord]].mean(axis=1)
+    #             df[l0, indiv, BODYCENTRE, coord] = x
+    #     # Writing file
+    #     DFIOMixin.write_feather(df, out_fp)
+    #     return outcome
 
     @staticmethod
-    def refine_identities(
-        in_fp: str, out_fp: str, configs_fp: str, overwrite: bool
-    ) -> str:
+    def refine_ids(in_fp: str, out_fp: str, configs_fp: str, overwrite: bool) -> str:
         """
         Ensures that the identity is correctly tracked for maDLC.
         Assumes interpolatePoints and calcBodyCentre has already been run.
 
         Notes
         -----
         The config file must contain the following parameters:
         ```
-        - (user, auto)
+        - user
             - preprocess
-                - refine_identities
+                - refine_ids
                     - marked: str
                     - unmarked: str
                     - marking: str
                     - window_sec: float
                     - metric: ["current", "rolling", "binned"]
         ```
         """
@@ -199,22 +215,20 @@
         # If overwrite is False, checking if we should skip processing
         if not overwrite and os.path.exists(out_fp):
             return DiagnosticsMixin.warning_msg()
         # Reading file
         df = DFIOMixin.read_feather(in_fp)
         # Getting necessary config parameters
         configs = ExperimentConfigs.read_json(configs_fp)
-        configs_filt = configs.user.preprocess.refine_identities
-        # bpts = (
-        #     configs_filt.bodyparts
-        # )  # TODO: need to implement the body_centre function again
+        configs_filt = Model_refine_ids(**configs.user.preprocess.refine_ids)
         marked = configs_filt.marked
         unmarked = configs_filt.unmarked
         marking = configs_filt.marking
         window_sec = configs_filt.window_sec
+        bpts = configs_filt.bodyparts
         metric = configs_filt.metric
         fps = configs.auto.formatted_vid.fps
         # Calculating more parameters
         window_frames = int(np.round(fps * window_sec, 0))
         # Error checking for invalid/non-existent column names marked, unmarked, and marking
         for column, level in [
             (marked, "individuals"),
@@ -222,29 +236,32 @@
             (marking, "bodyparts"),
         ]:
             if column not in df.columns.unique(level):
                 raise ValueError(
                     f'The marking value in the config file, "{column}",'
                     + " is not a column name in the DLC file."
                 )
+        # Checking that bodyparts are all valid
+        KeypointsMixin.check_bpts_exist(df, bpts)
         # Calculating the distances between the bodycentres and the marking
-        df_aggr = aggregate_df(df, marking, [marked, unmarked])
+        df_aggr = aggregate_df(df, marking, [marked, unmarked], bpts)
         # Getting "to_switch" decision series for each frame
         df_switch = decice_switch(df_aggr, window_frames, marked, unmarked)
         # Updating df with the switched values
         df_switched = switch_identities(df, df_switch[metric], marked, unmarked)
         # Writing to file
         DFIOMixin.write_feather(df_switched, out_fp)
         return outcome
 
 
 def aggregate_df(
     df: pd.DataFrame,
     marking: str,
     indivs: list[str],
+    bpts: list[str],
 ) -> pd.DataFrame:
     """
     _summary_
 
     Parameters
     ----------
     df : pd.DataFrame
@@ -260,18 +277,19 @@
         _description_
     """
     l0 = df.columns.unique(0)[0]
     df_aggr = pd.DataFrame(index=df.index)
     for coord in ["x", "y"]:
         # Getting the coordinates of the colour marking in each frame
         df_aggr[("mark", coord)] = df[l0, SINGLE_COL, marking, coord]
+        idx = pd.IndexSlice
         for indiv in indivs:
             # Getting the coordinates of each individual (average of the given bodyparts list)
-            df_aggr[(indiv, coord)] = df[l0, indiv, BODYCENTRE, coord]
-            df_aggr[(indiv, coord)] = df[l0, indiv, BODYCENTRE, coord]
+            idx_a = idx[l0, indiv, bpts, coord]
+            df_aggr[(indiv, coord)] = df.loc[:, idx_a].mean(axis=1)
     # Getting the distance between each mouse and the colour marking in each frame
     for indiv in indivs:
         df_aggr[(indiv, "dist")] = np.sqrt(
             np.square(df_aggr[(indiv, "x")] - df_aggr[("mark", "x")])
             + np.square(df_aggr[(indiv, "y")] - df_aggr[("mark", "y")])
         )
     # Formatting columns as a MultiIndex
@@ -365,8 +383,24 @@
             row[header, unmarked] = list(row[header, marked].copy())
             row[header, marked] = temp
         return row
 
     df = df.apply(lambda row: _f(row, marked, unmarked), axis=1)
     df = df.drop(columns="isSwitch")
     return df
-    return df
+
+
+class Model_interpolate(BaseModel):
+    """_summary_"""
+
+    pcutoff: float = 0
+
+
+class Model_refine_ids(BaseModel):
+    """_summary_"""
+
+    marked: str = ""
+    unmarked: str = ""
+    marking: str = ""
+    bodyparts: list[str] = []
+    window_sec: float = 0
+    metric: Literal["current", "rolling", "binned"] = "current"
```

### Comparing `behavysis_pipeline-0.1.0/behavysis_pipeline/processes/update_configs.py` & `behavysis_pipeline-0.1.1/behavysis_pipeline/processes/update_configs.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,18 +14,17 @@
 -------
 str
     Description of the function's outcome.
 """
 
 from typing import Literal, Type
 
+from behavysis_core.data_models.experiment_configs import ExperimentConfigs
 from pydantic import ValidationError
 
-from behavysis_pipeline.pipeline.experiment_configs import ExperimentConfigs
-
 
 class UpdateConfigs:
     """_summary_"""
 
     @staticmethod
     def update_configs(
         configs_fp: str,
@@ -42,16 +41,14 @@
         ----------
         configs_fp : str
             The filepath of the existing config file.
         default_configs_fp : str
             The filepath of the default config file to use.
         overwrite : Literal["user", "all"]
             Specifies how to update the config files.
-        model_class : Type[BaseModel]
-            The Pydantic model class used for validation.
 
         Returns
         -------
         str
             Description of the function's outcome.
         """
         outcome = ""
```

### Comparing `behavysis_pipeline-0.1.0/LICENSE` & `behavysis_pipeline-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `behavysis_pipeline-0.1.0/pyproject.toml` & `behavysis_pipeline-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "behavysis_pipeline"
-version = "0.1.0"
+version = "0.1.1"
 description = "A behaviour processing and analysis package"
 authors = ["BowenLab"]
 license = "LGPL-3.0-or-later"
 readme = "README.md"
 packages = [{ include = "behavysis_pipeline" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 seaborn = "^0.13.2"
 scikit-learn = "^1.4.2"
 imbalanced-learn = "^0.12.2"
 behavysis_core = "^0.1.0"
-# behavysis_core = { path = "../behavysis_core", develop = true }
 
 [tool.poetry.group.dev.dependencies]
+behavysis_core = { path = "../behavysis_core", develop = true }
 black = "^24.4.0"
 pytest = "^8.1.1"
 mkdocs-material = "^9.5.18"
 mkdocstrings-python = "^1.9.2"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `behavysis_pipeline-0.1.0/README.md` & `behavysis_pipeline-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `behavysis_pipeline-0.1.0/PKG-INFO` & `behavysis_pipeline-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: behavysis_pipeline
-Version: 0.1.0
+Version: 0.1.1
 Summary: A behaviour processing and analysis package
 License: LGPL-3.0-or-later
 Author: BowenLab
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

