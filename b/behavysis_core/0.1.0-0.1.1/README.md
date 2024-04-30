# Comparing `tmp/behavysis_core-0.1.0.tar.gz` & `tmp/behavysis_core-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "behavysis_core-0.1.0.tar", max compression
+gzip compressed data, was "behavysis_core-0.1.1.tar", max compression
```

## Comparing `behavysis_core-0.1.0.tar` & `behavysis_core-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0        0 2024-04-18 23:42:28.085726 behavysis_core-0.1.0/ba_core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 23:42:28.097417 behavysis_core-0.1.0/ba_core/data_models/__init__.py
--rw-r--r--   0        0        0      709 2024-04-19 06:23:55.574720 behavysis_core-0.1.0/ba_core/data_models/bouts.py
--rw-r--r--   0        0        0     1994 2024-04-19 06:21:23.265095 behavysis_core-0.1.0/ba_core/data_models/pydantic_base_model.py
--rw-r--r--   0        0        0      440 2024-04-19 06:47:23.730427 behavysis_core-0.1.0/ba_core/data_models/vid_metadata.py
--rw-r--r--   0        0        0        0 2024-04-18 23:42:28.128379 behavysis_core-0.1.0/ba_core/mixins/__init__.py
--rw-r--r--   0        0        0     6050 2024-04-18 23:42:28.138945 behavysis_core-0.1.0/ba_core/mixins/behaviour_mixin.py
--rw-r--r--   0        0        0     2845 2024-04-18 23:42:28.147720 behavysis_core-0.1.0/ba_core/mixins/df_io_mixin.py
--rw-r--r--   0        0        0     1009 2024-04-19 00:59:01.900816 behavysis_core-0.1.0/ba_core/mixins/diagnostics_mixin.py
--rw-r--r--   0        0        0     1104 2024-04-18 23:42:28.166435 behavysis_core-0.1.0/ba_core/mixins/io_mixin.py
--rw-r--r--   0        0        0     2907 2024-04-18 23:42:28.176334 behavysis_core-0.1.0/ba_core/mixins/keypoints_mixin.py
--rw-r--r--   0        0        0     3122 2024-04-22 07:59:51.869727 behavysis_core-0.1.0/ba_core/mixins/process_vid_mixin.py
--rw-r--r--   0        0        0     2121 2024-04-19 05:43:49.705926 behavysis_core-0.1.0/ba_core/mixins/subprocess_mixin.py
--rw-r--r--   0        0        0       21 2024-04-18 23:42:28.225031 behavysis_core-0.1.0/ba_core/utils/__init__.py
--rw-r--r--   0        0        0     2677 2024-04-19 05:25:53.762072 behavysis_core-0.1.0/ba_core/utils/constants.py
--rw-r--r--   0        0        0    35823 2024-04-18 23:42:28.069104 behavysis_core-0.1.0/LICENSE
--rw-r--r--   0        0        0      700 2024-04-23 02:37:59.166405 behavysis_core-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1273 2024-04-23 01:48:33.698411 behavysis_core-0.1.0/README.md
--rw-r--r--   0        0        0     2185 1970-01-01 00:00:00.000000 behavysis_core-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-18 23:42:28.085726 behavysis_core-0.1.1/behavysis_core/__init__.py
+-rw-r--r--   0        0        0     2552 2024-04-30 16:35:30.039878 behavysis_core-0.1.1/behavysis_core/constants.py
+-rw-r--r--   0        0        0        0 2024-04-18 23:42:28.097417 behavysis_core-0.1.1/behavysis_core/data_models/__init__.py
+-rw-r--r--   0        0        0      716 2024-04-23 03:13:01.805016 behavysis_core-0.1.1/behavysis_core/data_models/bouts.py
+-rw-r--r--   0        0        0     4234 2024-04-30 16:37:09.310061 behavysis_core-0.1.1/behavysis_core/data_models/experiment_configs.py
+-rw-r--r--   0        0        0     2663 2024-04-25 14:51:51.201461 behavysis_core-0.1.1/behavysis_core/data_models/pydantic_base_model.py
+-rw-r--r--   0        0        0      445 2024-04-23 03:10:19.898213 behavysis_core-0.1.1/behavysis_core/data_models/vid_metadata.py
+-rw-r--r--   0        0        0        0 2024-04-18 23:42:28.128379 behavysis_core-0.1.1/behavysis_core/mixins/__init__.py
+-rw-r--r--   0        0        0     6058 2024-04-30 16:37:08.023114 behavysis_core-0.1.1/behavysis_core/mixins/behaviour_mixin.py
+-rw-r--r--   0        0        0     2861 2024-04-30 16:37:08.384787 behavysis_core-0.1.1/behavysis_core/mixins/df_io_mixin.py
+-rw-r--r--   0        0        0     1010 2024-04-30 16:37:08.620985 behavysis_core-0.1.1/behavysis_core/mixins/diagnostics_mixin.py
+-rw-r--r--   0        0        0     1104 2024-04-30 18:39:21.019728 behavysis_core-0.1.1/behavysis_core/mixins/io_mixin.py
+-rw-r--r--   0        0        0     3361 2024-04-30 16:37:08.938742 behavysis_core-0.1.1/behavysis_core/mixins/keypoints_mixin.py
+-rw-r--r--   0        0        0      853 2024-04-24 03:16:56.057013 behavysis_core-0.1.1/behavysis_core/mixins/multiproc_mixin.py
+-rw-r--r--   0        0        0     3118 2024-04-24 03:31:18.337065 behavysis_core-0.1.1/behavysis_core/mixins/process_vid_mixin.py
+-rw-r--r--   0        0        0     1737 2024-04-24 05:25:09.486510 behavysis_core-0.1.1/behavysis_core/mixins/subproc_mixin.py
+-rw-r--r--   0        0        0    35823 2024-04-18 23:42:28.069104 behavysis_core-0.1.1/LICENSE
+-rw-r--r--   0        0        0      726 2024-04-30 19:58:10.967564 behavysis_core-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1308 2024-04-23 03:15:52.937659 behavysis_core-0.1.1/README.md
+-rw-r--r--   0        0        0     2259 1970-01-01 00:00:00.000000 behavysis_core-0.1.1/PKG-INFO
```

### Comparing `behavysis_core-0.1.0/ba_core/data_models/bouts.py` & `behavysis_core-0.1.1/behavysis_core/data_models/bouts.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 _summary_
 """
 
 from typing import Dict, List
 
 from pydantic import BaseModel
 
-from ba_core.data_models.pydantic_base_model import PydanticBaseModel
+from behavysis_core.data_models.pydantic_base_model import PydanticBaseModel
 
 
 class Bout(BaseModel):
     """__summary__"""
 
     start: int
     stop: int
```

### Comparing `behavysis_core-0.1.0/ba_core/data_models/pydantic_base_model.py` & `behavysis_core-0.1.1/behavysis_core/data_models/pydantic_base_model.py`

 * *Files 21% similar despite different names*

```diff
@@ -60,7 +60,24 @@
     def validate_attr_closed_set(v, closed_set):
         """Validate that the attribute is in the given closed set."""
         if v not in closed_set:
             raise ValueError(
                 f"Invalid value: {v}.\nOption must be one of: {', '.join(closed_set)}"
             )
         return v
+
+    @staticmethod
+    def get_field_names(type_) -> list[tuple[str, ...]]:
+        """
+        Returns the nested field names of the class as
+        a list of tuples.
+        Each tuple is a nested field name combination.
+        """
+        fields = []
+        # For each field in the class
+        for name, type_ in type_.__annotations__.items():
+            if hasattr(type_, '__annotations__'):  # Is a nested class
+                for subfield in PydanticBaseModel.get_field_names(type_):
+                    fields.append((name,) + subfield)
+            else:  # is a primitive field
+                fields.append((name,))
+        return fields
```

### Comparing `behavysis_core-0.1.0/ba_core/mixins/behaviour_mixin.py` & `behavysis_core-0.1.1/behavysis_core/mixins/behaviour_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 from typing import Union
 
 import numpy as np
 import pandas as pd
 from scipy.stats import mode
 
-from ba_core.data_models.bouts import Bouts
-from ba_core.utils.constants import (
+from behavysis_core.constants import (
     BEHAV_ACTUAL_COL,
     BEHAV_COLUMN_NAMES,
     BEHAV_PRED_COL,
     BEHAV_PROB_COL,
 )
+from behavysis_core.data_models.bouts import Bouts
 
 
 class BehaviourMixin:
     """_summary_"""
 
     @staticmethod
     def vect_2_bouts(vect: Union[np.ndarray, pd.Series]) -> pd.DataFrame:
```

### Comparing `behavysis_core-0.1.0/ba_core/mixins/df_io_mixin.py` & `behavysis_core-0.1.1/behavysis_core/mixins/df_io_mixin.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,40 +2,40 @@
 Utility functions.
 """
 
 from __future__ import annotations
 
 import functools
 import os
-from typing import Callable
+from typing import Callable, Union
 
 import numpy as np
 import pandas as pd
 
-from ba_core.utils.constants import DLC_COLUMN_NAMES, DLC_HDF_KEY
+from behavysis_core.constants import DLC_COLUMN_NAMES, DLC_HDF_KEY
 
 
 class DFIOMixin:
     """__summary"""
 
     # @staticmethod
     def read_decorator(
         func: Callable[[str], pd.DataFrame]
     ) -> Callable[[str], pd.DataFrame]:
         """A decorator to catch errors when reading in files."""
 
         @functools.wraps(func)
         def wrapper(fp: str, *args, **kwargs):
-            try:
-                return func(fp, *args, **kwargs)
-            except Exception as e:
-                raise ValueError(
-                    f'The file, "{fp}", does not exist or is in an invalid format.'
-                    + "Please check this file."
-                ) from e
+            # try:
+            return func(fp, *args, **kwargs)
+            # except Exception as e:
+            #     raise ValueError(
+            #         f'The file, "{fp}", does not exist or is in an invalid format.'
+            #         + "Please check this file."
+            #     ) from e
 
         return wrapper
 
     # @staticmethod
     def write_decorator(
         func: Callable[[pd.DataFrame, str], None]
     ) -> Callable[[pd.DataFrame, str], None]:
```

### Comparing `behavysis_core-0.1.0/ba_core/mixins/diagnostics_mixin.py` & `behavysis_core-0.1.1/behavysis_core/mixins/diagnostics_mixin.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from __future__ import annotations
 
 from inspect import currentframe
 from typing import Callable, Optional
 
 import numpy as np
 
-from ba_core.utils.constants import DIAGNOSTICS_SUCCESS_MESSAGES
+from behavysis_core.constants import DIAGNOSTICS_SUCCESS_MESSAGES
 
 
 class DiagnosticsMixin:
     """__summary__"""
 
     @staticmethod
     def success_msg() -> str:
```

### Comparing `behavysis_core-0.1.0/ba_core/mixins/io_mixin.py` & `behavysis_core-0.1.1/behavysis_core/mixins/io_mixin.py`

 * *Files identical despite different names*

### Comparing `behavysis_core-0.1.0/ba_core/mixins/keypoints_mixin.py` & `behavysis_core-0.1.1/behavysis_core/mixins/keypoints_mixin.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 from __future__ import annotations
 
 import numpy as np
 import pandas as pd
 
-from ba_core.utils.constants import PROCESS_COL, SINGLE_COL
+from behavysis_core.constants import PROCESS_COL, SINGLE_COL
 
 
 class KeypointsMixin:
     """__summary__"""
 
     @staticmethod
     def check_bpts_exist(df: pd.DataFrame, bodyparts: list) -> None:
@@ -88,7 +88,21 @@
         df = df.copy()
         # Removing the scorer column because all values are identical
         df.columns = df.columns.droplevel("scorer")
         # Grouping the columns by the individuals level for cleaner presentation
         # TODO: is there a better way to group/sort the columns?
         df = df.reindex(columns=df.columns.unique("individuals"), level="individuals")
         return df
+
+    @staticmethod
+    def check_df(df: pd.DataFrame):
+        """
+        Checks whether the dataframe is in the correct format for the keypoints functions.
+        Checks that:
+
+        - There are no null values.
+        """
+        # Checking for null values
+        if df.isnull().values.any():
+            raise ValueError(
+                "The dataframe contains null values. Be sure to run interpolate_points first."
+            )
```

### Comparing `behavysis_core-0.1.0/ba_core/mixins/process_vid_mixin.py` & `behavysis_core-0.1.1/behavysis_core/mixins/process_vid_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 """
 
 from __future__ import annotations
 
 from typing import Union
 
 import cv2
-from ba_core.data_models.vid_metadata import VidMetadata
-from ba_core.mixins.subprocess_mixin import SubprocessMixin
+from behavysis_core.data_models.vid_metadata import VidMetadata
+from behavysis_core.mixins.subproc_mixin import SubprocMixin
 
 
 class ProcessVidMixin:
     """__summary__"""
 
     @staticmethod
     def process_vid(
@@ -62,16 +62,16 @@
             "20",
             "-y",
             # "-loglevel",
             # "quiet",
             out_fp,
         ]
         # Running ffmpeg command
-        # SubprocessMixin.run_subprocess_fstream(cmd)
-        SubprocessMixin.run_subprocess_console(cmd)
+        # SubprocMixin.run_subproc_fstream(cmd)
+        SubprocMixin.run_subproc_console(cmd)
         # Returning outcome
         return outcome
 
     @staticmethod
     def get_vid_metadata(fp: str) -> VidMetadata:
         """
         Finds the video metadata/parameters for either the raw or formatted video.
```

### Comparing `behavysis_core-0.1.0/ba_core/mixins/subprocess_mixin.py` & `behavysis_core-0.1.1/behavysis_core/mixins/subproc_mixin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,50 @@
 """
 Utility functions.
 """
 
 from __future__ import annotations
 
 import os
-from multiprocessing import current_process
 from subprocess import PIPE, Popen
 
-from ba_core.utils.constants import TEMP_DIR
 
-
-class SubprocessMixin:
+class SubprocMixin:
     """__summary__"""
 
     @staticmethod
-    def get_cpid() -> int:
-        """Get child process ID for multiprocessing."""
-        return current_process()._identity[0] if current_process()._identity else 0
-
-    @staticmethod
-    def run_subprocess_fstream(cmd: list[str], fp: str = None) -> None:
+    def run_subproc_fstream(cmd: list[str], fp: str, **kwargs) -> None:
         """Run a subprocess and stream the output to a file."""
-        if not fp:
-            cpid = SubprocessMixin.get_cpid()
-            fp = os.path.join(TEMP_DIR, f"subprocess_output_{cpid}.txt")
         # Making a file to store the output
         os.makedirs(os.path.split(fp)[0], exist_ok=True)
         with open(fp, "w", encoding="utf-8") as f:
             # Starting the subprocess
-            with Popen(cmd, stdout=f, stderr=f) as p:
+            with Popen(cmd, stdout=f, stderr=f, **kwargs) as p:
                 # Wait for the subprocess to finish
                 p.wait()
                 # Error handling
                 if p.returncode:
                     f.seek(0)
                     raise ValueError(f.read().decode())
 
     @staticmethod
-    def run_subprocess_str(cmd: list[str]) -> str:
+    def run_subproc_str(cmd: list[str], **kwargs) -> str:
         """Run a subprocess and return the output as a string."""
         # Running the subprocess
-        with Popen(cmd, stdout=PIPE, stderr=PIPE) as p:
+        with Popen(cmd, stdout=PIPE, stderr=PIPE, **kwargs) as p:
             # Wait for the subprocess to finish
             out, err = p.communicate()
             # Error handling
             if p.returncode:
                 raise ValueError(err.decode("utf-8"))
             return out.decode("utf-8")
 
     @staticmethod
-    def run_subprocess_console(cmd: list[str]) -> None:
+    def run_subproc_console(cmd: list[str], **kwargs) -> None:
         """Run a subprocess and stream the output to a file."""
         # Starting the subprocess
-        with Popen(cmd) as p:
+        with Popen(cmd, **kwargs) as p:
             # Wait for the subprocess to finish
             p.wait()
             # Error handling
             if p.returncode:
                 raise ValueError("ERROR: Subprocess failed to run.")
```

### Comparing `behavysis_core-0.1.0/ba_core/utils/constants.py` & `behavysis_core-0.1.1/behavysis_core/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,16 +42,14 @@
 ####################################################################################################
 
 BEHAV_PROB_COL = "prob"
 BEHAV_PRED_COL = "pred"
 BEHAV_ACTUAL_COL = "actual"
 BEHAV_COLUMN_NAMES = ("behaviours", "outcomes")
 
-# # NEED TO CHANGE THIS FOR DIFFERENT NAMES OF CORNERS
-# ARENAPARTS = ("TopRight", "TopLeft", "BottomRight", "BottomLeft")
 
 ####################################################################################################
 # DIAGNOSTICS CONSTANTS
 ####################################################################################################
 
 DIAGNOSTICS_SUCCESS_MESSAGES = (
     "Success! Success! Success!!",
```

### Comparing `behavysis_core-0.1.0/LICENSE` & `behavysis_core-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `behavysis_core-0.1.0/pyproject.toml` & `behavysis_core-0.1.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [tool.poetry]
 name = "behavysis_core"
-version = "0.1.0"
+version = "0.1.1"
 description = "Core functionality supporting the `ba` suite"
 authors = ["BowenLab"]
 license = "LGPL-3.0-or-later"
 readme = "README.md"
-packages = [{ include = "ba_core" }]
+packages = [{ include = "behavysis_core" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pydantic = "^2.7.0"
 numpy = "^1.26.4"
 pandas = "^2.2.2"
+tables = "^3.9.2"
 pyarrow = "^15.0.2"
 scipy = "^1.13.0"
 opencv-python = "^4.9.0.80"
 matplotlib = "^3.8.4"
 natsort = "^8.4.0"
-tqdm = "^4.66.0"
+tqdm = "^4.30.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.4.0"
 pytest = "^8.1.1"
 mkdocs-material = "^9.5.18"
 mkdocstrings-python = "^1.9.2"
```

### Comparing `behavysis_core-0.1.0/README.md` & `behavysis_core-0.1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-# ba_core
+# behavysis_core
 
-[Documentation](https://tlee08.github.io/ba_core/)
+[Documentation](https://tlee08.github.io/behavysis_core/)
 
-Core functionalities shared across the ba suite.
+Core functionalities shared across the Behavysis suite.
 
 ## Installation
 
 ### Dev installation
 
 ```bash
 conda env create -f conda_env.yaml
-conda activate ba_pipeline_env
+conda activate behavysis_pipeline_env
 pip install poetry
 poetry install
 ```
 
 ### User installation
 
 ```bash
 conda env create -f conda_env.yaml
-conda activate ba_pipeline_env
+conda activate behavysis_pipeline_env
 pip install .
 ```
 
 ## References
 
 Mathis, A., Mamidanna, P., Cury, K. M., Abe, T., Murthy, V. N., Mathis, M. W., & Bethge, M. (2018, August 20). DeepLabCut: markerless pose estimation of user-defined body parts with deep learning. Nature Neuroscience. Springer Science and Business Media LLC. http://doi.org/10.1038/s41593-018-0209-y
```

### Comparing `behavysis_core-0.1.0/PKG-INFO` & `behavysis_core-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: behavysis_core
-Version: 0.1.0
+Version: 0.1.1
 Summary: Core functionality supporting the `ba` suite
 License: LGPL-3.0-or-later
 Author: BowenLab
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -15,39 +15,40 @@
 Requires-Dist: natsort (>=8.4.0,<9.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: opencv-python (>=4.9.0.80,<5.0.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: pyarrow (>=15.0.2,<16.0.0)
 Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Requires-Dist: scipy (>=1.13.0,<2.0.0)
-Requires-Dist: tqdm (>=4.66.0,<5.0.0)
+Requires-Dist: tables (>=3.9.2,<4.0.0)
+Requires-Dist: tqdm (>=4.30.0,<5.0.0)
 Description-Content-Type: text/markdown
 
-# ba_core
+# behavysis_core
 
-[Documentation](https://tlee08.github.io/ba_core/)
+[Documentation](https://tlee08.github.io/behavysis_core/)
 
-Core functionalities shared across the ba suite.
+Core functionalities shared across the Behavysis suite.
 
 ## Installation
 
 ### Dev installation
 
 ```bash
 conda env create -f conda_env.yaml
-conda activate ba_pipeline_env
+conda activate behavysis_pipeline_env
 pip install poetry
 poetry install
 ```
 
 ### User installation
 
 ```bash
 conda env create -f conda_env.yaml
-conda activate ba_pipeline_env
+conda activate behavysis_pipeline_env
 pip install .
 ```
 
 ## References
 
 Mathis, A., Mamidanna, P., Cury, K. M., Abe, T., Murthy, V. N., Mathis, M. W., & Bethge, M. (2018, August 20). DeepLabCut: markerless pose estimation of user-defined body parts with deep learning. Nature Neuroscience. Springer Science and Business Media LLC. http://doi.org/10.1038/s41593-018-0209-y
```

