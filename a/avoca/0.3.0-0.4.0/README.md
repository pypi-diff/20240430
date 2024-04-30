# Comparing `tmp/avoca-0.3.0.tar.gz` & `tmp/avoca-0.4.0.tar.gz`

## Comparing `avoca-0.3.0.tar` & `avoca-0.4.0.tar`

### file list

```diff
@@ -1,44 +1,46 @@
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 avoca-0.3.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 avoca-0.3.0/.readthedocs.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/__init__.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/export_nas.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/flags.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/io.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/logging.py
--rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/manager.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/requirements.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/bindings/__init__.py
--rw-r--r--   0        0        0    15939 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/bindings/ebas.py
--rw-r--r--   0        0        0     9293 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/bindings/gcwerks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/qa_class/__init__.py
--rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/qa_class/abstract.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/qa_class/concs.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/qa_class/generate_classes_doc.py
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/qa_class/rt.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/qa_class/test.py
--rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/qa_class/zscore.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/testing/__init__.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/testing/df.py
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/utils/__init__.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/utils/torch_models.py
--rw-r--r--   0        0        0   152471 2020-02-02 00:00:00.000000 avoca-0.3.0/data/CH0001G.20240219123300.20240307132229.online_gc.NMHC.air.16d.61mn.CH01L_Agilent_GC-MS-MEDUSA_Medusa-12_JFJ.CH01L_gc_ms.lev0.nas
--rw-r--r--   0        0        0   499755 2020-02-02 00:00:00.000000 avoca-0.3.0/data/voc_jan2jun_2023.csv
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 avoca-0.3.0/data/.avoca/config.yaml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 avoca-0.3.0/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 avoca-0.3.0/docs/make.bat
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 avoca-0.3.0/docs/source/conf.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 avoca-0.3.0/docs/source/index.rst
--rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 avoca-0.3.0/docs/source/quickstart.ipynb
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 avoca-0.3.0/docs/source/bindings/ebas.md
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 avoca-0.3.0/docs/source/bindings/gcwerks.md
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 avoca-0.3.0/docs/source/bindings/index.rst
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 avoca-0.3.0/examples/config.yaml
--rw-r--r--   0        0        0    10451 2020-02-02 00:00:00.000000 avoca-0.3.0/examples/data_qa.ipynb
--rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 avoca-0.3.0/examples/read_nas.ipynb
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 avoca-0.3.0/tests/test_io.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 avoca-0.3.0/.gitignore
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 avoca-0.3.0/LICENCE.txt
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 avoca-0.3.0/README.md
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 avoca-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 avoca-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 avoca-0.4.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 avoca-0.4.0/.readthedocs.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/__init__.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/export_nas.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/flags.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/io.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/logging.py
+-rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/manager.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/requirements.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/bindings/__init__.py
+-rw-r--r--   0        0        0    15939 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/bindings/ebas.py
+-rw-r--r--   0        0        0    10120 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/bindings/gcwerks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/qa_class/__init__.py
+-rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/qa_class/abstract.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/qa_class/concs.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/qa_class/generate_classes_doc.py
+-rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/qa_class/rt.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/qa_class/test.py
+-rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/qa_class/zscore.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/testing/__init__.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/testing/df.py
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/utils/__init__.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 avoca-0.4.0/avoca/utils/torch_models.py
+-rw-r--r--   0        0        0   152471 2020-02-02 00:00:00.000000 avoca-0.4.0/data/CH0001G.20240219123300.20240307132229.online_gc.NMHC.air.16d.61mn.CH01L_Agilent_GC-MS-MEDUSA_Medusa-12_JFJ.CH01L_gc_ms.lev0.nas
+-rw-r--r--   0        0        0   499755 2020-02-02 00:00:00.000000 avoca-0.4.0/data/voc_jan2jun_2023.csv
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 avoca-0.4.0/data/.avoca/config.yaml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 avoca-0.4.0/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 avoca-0.4.0/docs/make.bat
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 avoca-0.4.0/docs/source/conf.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 avoca-0.4.0/docs/source/index.rst
+-rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 avoca-0.4.0/docs/source/quickstart.ipynb
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 avoca-0.4.0/docs/source/bindings/ebas.md
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 avoca-0.4.0/docs/source/bindings/gcwerks.md
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 avoca-0.4.0/docs/source/bindings/index.rst
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 avoca-0.4.0/examples/config.yaml
+-rw-r--r--   0        0        0    10451 2020-02-02 00:00:00.000000 avoca-0.4.0/examples/data_qa.ipynb
+-rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 avoca-0.4.0/examples/read_nas.ipynb
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 avoca-0.4.0/tests/test_io.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 avoca-0.4.0/tests/bindings/gcwerks.dat
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 avoca-0.4.0/tests/bindings/test_gcwerks.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 avoca-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 avoca-0.4.0/LICENCE.txt
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 avoca-0.4.0/README.md
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 avoca-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 avoca-0.4.0/PKG-INFO
```

### Comparing `avoca-0.3.0/.gitlab-ci.yml` & `avoca-0.4.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `avoca-0.3.0/.readthedocs.yaml` & `avoca-0.4.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `avoca-0.3.0/avoca/flags.py` & `avoca-0.4.0/avoca/flags.py`

 * *Files identical despite different names*

### Comparing `avoca-0.3.0/avoca/manager.py` & `avoca-0.4.0/avoca/manager.py`

 * *Files identical despite different names*

### Comparing `avoca-0.3.0/avoca/requirements.py` & `avoca-0.4.0/avoca/requirements.py`

 * *Files identical despite different names*

### Comparing `avoca-0.3.0/avoca/settings.py` & `avoca-0.4.0/avoca/settings.py`

 * *Files identical despite different names*

### Comparing `avoca-0.3.0/avoca/bindings/ebas.py` & `avoca-0.4.0/avoca/bindings/ebas.py`

 * *Files identical despite different names*

### Comparing `avoca-0.3.0/avoca/bindings/gcwerks.py` & `avoca-0.4.0/avoca/bindings/gcwerks.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 
 """
 
 from __future__ import annotations
 
 import logging
 import subprocess
+import warnings
 from datetime import datetime
 from os import PathLike
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 
@@ -112,23 +113,35 @@
 cols_zero_is_nan = ["rt"]
 
 
 def read_gcwerks(
     file_path: PathLike,
     datetime_format: str = "%y%m%d%H%M",
     runtypes: list[str] = [],
+    keep_ordering_from_file: bool = False,
+    return_flags: bool = True,
 ) -> pd.DataFrame:
-    """Read the input '.dat' file from gcwerks, adding a column: ('-', 'datetime')."""
+    """Read the input '.dat' file from gcwerks, adding a column: ('-', 'datetime').
+
+
+
+    Args:
+        file_path: The path to the file to read.
+        datetime_format: The format of the datetime in the file.
+        runtypes: The run types to keep. If empty, all run types are kept.
+        keep_ordering_from_file: Keep the ordering of the columns from the file.
+        return_flags: Return the flags in the dataframe.
+    """
 
     file_path = Path(file_path)
 
     df = pd.read_csv(
         file_path,
         # Separator
-        sep="\s+",
+        sep=r"\s+",
         # use the line number 1 and 2 as headers # Line 0 is skipped
         header=[1, 2],
         # Ensure the date an time are read as str
         dtype={("-", "date"): str, ("-", "time"): str},
     )
     df[("-", "datetime")] = pd.to_datetime(
         # Merge the str for date and time
@@ -140,16 +153,20 @@
 
     for col in df.columns:
         sub = col[0]
 
         if sub != "-":
             if sub not in substances:
                 substances.append(sub)
-            if (sub, "flag") not in df.columns:
-                df[(sub, "flag")] = pd.Series(data=0, index=df.index, dtype=int)
+            if return_flags and (sub, "flag") not in df.columns:
+                with warnings.catch_warnings():
+                    warnings.simplefilter(
+                        action="ignore", category=pd.errors.PerformanceWarning
+                    )
+                    df[(sub, "flag")] = pd.Series(data=0, index=df.index, dtype=int)
 
         # Make a serie full of 0 = `Valid measurement`
         serie_str: pd.Series = df[col].astype(str)
         # Last character is the flag
         flags: pd.Series = serie_str.str[-1]
         if col[1] in cols_float:
             # Convert the serie to numeric
@@ -163,47 +180,50 @@
             # There is a flag
 
             # Ensure there are no unknown flags
             unknown_flags = flags[~flags.isin(flags_known)].unique()
             if len(unknown_flags):
                 raise ValueError(f"Unknown flags for {col}: {unknown_flags}")
 
-
             for flag_str, flag_obj in flag_values.items():
                 # Add the flag to the serie
                 mask_flag = flags == flag_str
-                df.loc[mask_flag, (sub, "flag")] |= flag_obj.value
+                if return_flags:
+                    df.loc[mask_flag, (sub, "flag")] |= flag_obj.value
 
                 if flag_obj == QA_Flag.INVALIDATED_EXT:
                     df.loc[mask_flag, col] = np.nan
 
-            # where value is nan or inf, the flag is
-            # 999 = `Missing measurement, unspecified reason`
-            mask_nan = serie_str.isin(["nan", "inf"])
-            mask_nan |= df[col].isna()
-            df.loc[mask_nan, (sub, "flag")] |= QA_Flag.MISSING.value
+            if return_flags:
+                # where value is nan or inf, the flag is
+                # 999 = `Missing measurement, unspecified reason`
+                mask_nan = serie_str.isin(["nan", "inf"])
+                mask_nan |= df[col].isna()
+                df.loc[mask_nan, (sub, "flag")] |= QA_Flag.MISSING.value
 
     # Set the calibration flag
     type_col = ("-", "type")
     if type_col in df.columns:
         mask_calib = df[("-", "type")].isin(["std"])
-        for sub in substances:
-            df.loc[mask_calib, (sub, "flag")] |= QA_Flag.CALIBRATION.value
+        if return_flags:
+            for sub in substances:
+                df.loc[mask_calib, (sub, "flag")] |= QA_Flag.CALIBRATION.value
 
         if runtypes:
             df = df[df[("-", "type")].isin(runtypes)]
     else:
         if runtypes:
             logger.warning(
                 "No type column found in the data. Run types cannot be filtered as"
                 " specified."
             )
 
     # Sort the columns by the first level
-    df = df.sort_index(axis=1, level=0)
+    if not keep_ordering_from_file:
+        df = df.sort_index(axis=1, level=0)
     df = df.set_index(("-", "datetime"))
     return df
 
 
 def export(
     workdir: PathLike,
     gcdir: PathLike,
```

### Comparing `avoca-0.3.0/avoca/qa_class/abstract.py` & `avoca-0.4.0/avoca/qa_class/abstract.py`

 * *Files identical despite different names*

### Comparing `avoca-0.3.0/avoca/qa_class/concs.py` & `avoca-0.4.0/avoca/qa_class/concs.py`

 * *Files identical despite different names*

### Comparing `avoca-0.3.0/avoca/qa_class/generate_classes_doc.py` & `avoca-0.4.0/avoca/qa_class/generate_classes_doc.py`

 * *Files identical despite different names*

### Comparing `avoca-0.3.0/avoca/qa_class/rt.py` & `avoca-0.4.0/avoca/qa_class/rt.py`

 * *Files identical despite different names*

### Comparing `avoca-0.3.0/avoca/qa_class/test.py` & `avoca-0.4.0/avoca/qa_class/test.py`

 * *Files identical despite different names*

### Comparing `avoca-0.3.0/avoca/qa_class/zscore.py` & `avoca-0.4.0/avoca/qa_class/zscore.py`

 * *Files identical despite different names*

### Comparing `avoca-0.3.0/avoca/utils/__init__.py` & `avoca-0.4.0/avoca/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `avoca-0.3.0/avoca/utils/torch_models.py` & `avoca-0.4.0/avoca/utils/torch_models.py`

 * *Files identical despite different names*

### Comparing `avoca-0.3.0/data/CH0001G.20240219123300.20240307132229.online_gc.NMHC.air.16d.61mn.CH01L_Agilent_GC-MS-MEDUSA_Medusa-12_JFJ.CH01L_gc_ms.lev0.nas` & `avoca-0.4.0/data/CH0001G.20240219123300.20240307132229.online_gc.NMHC.air.16d.61mn.CH01L_Agilent_GC-MS-MEDUSA_Medusa-12_JFJ.CH01L_gc_ms.lev0.nas`

 * *Files identical despite different names*

### Comparing `avoca-0.3.0/data/voc_jan2jun_2023.csv` & `avoca-0.4.0/data/voc_jan2jun_2023.csv`

 * *Files identical despite different names*

### Comparing `avoca-0.3.0/docs/Makefile` & `avoca-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `avoca-0.3.0/docs/make.bat` & `avoca-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `avoca-0.3.0/docs/source/conf.py` & `avoca-0.4.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `avoca-0.3.0/docs/source/index.rst` & `avoca-0.4.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `avoca-0.3.0/docs/source/quickstart.ipynb` & `avoca-0.4.0/docs/source/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `avoca-0.3.0/docs/source/bindings/ebas.md` & `avoca-0.4.0/docs/source/bindings/ebas.md`

 * *Files identical despite different names*

### Comparing `avoca-0.3.0/examples/data_qa.ipynb` & `avoca-0.4.0/examples/data_qa.ipynb`

 * *Files identical despite different names*

### Comparing `avoca-0.3.0/examples/read_nas.ipynb` & `avoca-0.4.0/examples/read_nas.ipynb`

 * *Files identical despite different names*

### Comparing `avoca-0.3.0/LICENCE.txt` & `avoca-0.4.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `avoca-0.3.0/pyproject.toml` & `avoca-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "avoca"
-version = "0.3.0"
+version = "0.4.0"
 authors = [
   { name="Lionel Constantin", email="lionel.constantin@empa.ch" },
 ]
 description = "@voc@: Quality assessement of measurement data"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `avoca-0.3.0/PKG-INFO` & `avoca-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: avoca
-Version: 0.3.0
+Version: 0.4.0
 Summary: @voc@: Quality assessement of measurement data
 Project-URL: Homepage, https://gitlab.com/empa503/atmospheric-measurements/avoca
 Project-URL: Bug Tracker, https://gitlab.com/empa503/atmospheric-measurements/avoca/-/issues
 Project-URL: Documentation, http://avoca.readthedocs.io/
 Author-email: Lionel Constantin <lionel.constantin@empa.ch>
 License-File: LICENCE.txt
 Classifier: License :: OSI Approved :: MIT License
```

