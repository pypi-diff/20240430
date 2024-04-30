# Comparing `tmp/cesnet_datazoo-0.1.4.tar.gz` & `tmp/cesnet_datazoo-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cesnet_datazoo-0.1.4.tar", last modified: Mon Apr 29 08:35:20 2024, max compression
+gzip compressed data, was "cesnet_datazoo-0.1.5.tar", last modified: Tue Apr 30 12:14:13 2024, max compression
```

## Comparing `cesnet_datazoo-0.1.4.tar` & `cesnet_datazoo-0.1.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 08:35:20.306340 cesnet_datazoo-0.1.4/
--rw-rw-rw-   0        0        0     1541 2023-09-18 09:03:44.000000 cesnet_datazoo-0.1.4/LICENCE
--rw-rw-rw-   0        0        0    12953 2024-04-29 08:35:20.305333 cesnet_datazoo-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0    11374 2024-04-09 14:38:48.000000 cesnet_datazoo-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 08:35:20.263486 cesnet_datazoo-0.1.4/cesnet_datazoo/
--rw-rw-rw-   0        0        0        0 2023-09-04 15:14:00.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/__init__.py
--rw-rw-rw-   0        0        0    38406 2024-04-26 10:09:35.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/config.py
--rw-rw-rw-   0        0        0     1481 2024-04-26 10:10:11.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/constants.py
-drwxrwxrwx   0        0        0        0 2024-04-29 08:35:20.289841 cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/
--rw-rw-rw-   0        0        0      443 2023-10-09 14:50:14.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/__init__.py
--rw-rw-rw-   0        0        0    46635 2024-04-26 12:29:44.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/cesnet_dataset.py
--rw-rw-rw-   0        0        0     3617 2024-03-13 15:20:57.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/datasets.py
--rw-rw-rw-   0        0        0    29154 2024-03-13 15:20:40.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/datasets_constants.py
--rw-rw-rw-   0        0        0     1854 2024-03-14 10:53:21.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/loaders.py
-drwxrwxrwx   0        0        0        0 2024-04-29 08:35:20.292010 cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/metadata/
--rw-rw-rw-   0        0        0        0 2023-08-21 14:08:44.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/metadata/__init__.py
--rw-rw-rw-   0        0        0     1623 2024-04-26 12:35:59.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/metadata/dataset_metadata.py
--rw-rw-rw-   0        0        0     2175 2024-03-19 11:54:21.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/metadata/metadata.csv
--rw-rw-rw-   0        0        0    15137 2024-04-26 12:36:13.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/statistics.py
-drwxrwxrwx   0        0        0        0 2024-04-29 08:35:20.294530 cesnet_datazoo-0.1.4/cesnet_datazoo/metrics/
--rw-rw-rw-   0        0        0        0 2023-08-17 21:32:34.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/metrics/__init__.py
--rw-rw-rw-   0        0        0     3981 2024-04-26 10:13:11.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/metrics/classification_report.py
--rw-rw-rw-   0        0        0     1374 2024-04-17 16:35:50.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/metrics/provider_metrics.py
-drwxrwxrwx   0        0        0        0 2024-04-29 08:35:20.298903 cesnet_datazoo-0.1.4/cesnet_datazoo/pytables_data/
--rw-rw-rw-   0        0        0        0 2023-09-01 14:24:29.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/pytables_data/__init__.py
--rw-rw-rw-   0        0        0     1411 2023-10-30 20:40:56.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/pytables_data/apps_split.py
--rw-rw-rw-   0        0        0     5083 2024-03-19 14:07:14.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/pytables_data/data_scalers.py
--rw-rw-rw-   0        0        0    13717 2024-04-26 12:13:42.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/pytables_data/indices_setup.py
--rw-rw-rw-   0        0        0    19413 2024-04-26 12:33:06.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/pytables_data/pytables_dataset.py
-drwxrwxrwx   0        0        0        0 2024-04-29 08:35:20.303312 cesnet_datazoo-0.1.4/cesnet_datazoo/utils/
--rw-rw-rw-   0        0        0        0 2023-09-01 13:35:45.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/utils/__init__.py
--rw-rw-rw-   0        0        0     2462 2024-04-04 20:29:42.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/utils/class_info.py
--rw-rw-rw-   0        0        0     1441 2024-02-20 11:51:54.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/utils/download.py
--rw-rw-rw-   0        0        0      642 2023-09-01 13:43:06.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/utils/fileutils.py
--rw-rw-rw-   0        0        0      575 2023-09-26 08:58:11.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/utils/random.py
-drwxrwxrwx   0        0        0        0 2024-04-29 08:35:20.303827 cesnet_datazoo-0.1.4/cesnet_datazoo.egg-info/
--rw-rw-rw-   0        0        0    12953 2024-04-29 08:35:20.000000 cesnet_datazoo-0.1.4/cesnet_datazoo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1194 2024-04-29 08:35:20.000000 cesnet_datazoo-0.1.4/cesnet_datazoo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 08:35:20.000000 cesnet_datazoo-0.1.4/cesnet_datazoo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      238 2024-04-29 08:35:20.000000 cesnet_datazoo-0.1.4/cesnet_datazoo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-29 08:35:20.000000 cesnet_datazoo-0.1.4/cesnet_datazoo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1792 2024-04-26 13:30:41.000000 cesnet_datazoo-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-29 08:35:20.306340 cesnet_datazoo-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 12:14:13.154084 cesnet_datazoo-0.1.5/
+-rw-rw-rw-   0        0        0     1541 2023-09-18 09:03:44.000000 cesnet_datazoo-0.1.5/LICENCE
+-rw-rw-rw-   0        0        0    12953 2024-04-30 12:14:13.153578 cesnet_datazoo-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0    11374 2024-04-09 14:38:48.000000 cesnet_datazoo-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 12:14:13.110340 cesnet_datazoo-0.1.5/cesnet_datazoo/
+-rw-rw-rw-   0        0        0        0 2023-09-04 15:14:00.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/__init__.py
+-rw-rw-rw-   0        0        0    38406 2024-04-26 10:09:35.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/config.py
+-rw-rw-rw-   0        0        0     1481 2024-04-26 10:10:11.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-30 12:14:13.136146 cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/
+-rw-rw-rw-   0        0        0      443 2023-10-09 14:50:14.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/__init__.py
+-rw-rw-rw-   0        0        0    46988 2024-04-30 11:22:06.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/cesnet_dataset.py
+-rw-rw-rw-   0        0        0     3617 2024-03-13 15:20:57.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/datasets.py
+-rw-rw-rw-   0        0        0    29154 2024-03-13 15:20:40.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/datasets_constants.py
+-rw-rw-rw-   0        0        0     1854 2024-03-14 10:53:21.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/loaders.py
+drwxrwxrwx   0        0        0        0 2024-04-30 12:14:13.139212 cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/metadata/
+-rw-rw-rw-   0        0        0        0 2023-08-21 14:08:44.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/metadata/__init__.py
+-rw-rw-rw-   0        0        0     1623 2024-04-26 12:35:59.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/metadata/dataset_metadata.py
+-rw-rw-rw-   0        0        0     2175 2024-03-19 11:54:21.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/metadata/metadata.csv
+-rw-rw-rw-   0        0        0    15137 2024-04-26 12:36:13.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/statistics.py
+drwxrwxrwx   0        0        0        0 2024-04-30 12:14:13.141105 cesnet_datazoo-0.1.5/cesnet_datazoo/metrics/
+-rw-rw-rw-   0        0        0        0 2023-08-17 21:32:34.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/metrics/__init__.py
+-rw-rw-rw-   0        0        0     3981 2024-04-26 10:13:11.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/metrics/classification_report.py
+-rw-rw-rw-   0        0        0     1374 2024-04-17 16:35:50.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/metrics/provider_metrics.py
+drwxrwxrwx   0        0        0        0 2024-04-30 12:14:13.145674 cesnet_datazoo-0.1.5/cesnet_datazoo/pytables_data/
+-rw-rw-rw-   0        0        0        0 2023-09-01 14:24:29.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/pytables_data/__init__.py
+-rw-rw-rw-   0        0        0     1411 2023-10-30 20:40:56.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/pytables_data/apps_split.py
+-rw-rw-rw-   0        0        0     5236 2024-04-30 11:25:34.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/pytables_data/data_scalers.py
+-rw-rw-rw-   0        0        0    13717 2024-04-26 12:13:42.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/pytables_data/indices_setup.py
+-rw-rw-rw-   0        0        0    19431 2024-04-30 11:22:10.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/pytables_data/pytables_dataset.py
+drwxrwxrwx   0        0        0        0 2024-04-30 12:14:13.150684 cesnet_datazoo-0.1.5/cesnet_datazoo/utils/
+-rw-rw-rw-   0        0        0        0 2023-09-01 13:35:45.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/utils/__init__.py
+-rw-rw-rw-   0        0        0     2462 2024-04-04 20:29:42.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/utils/class_info.py
+-rw-rw-rw-   0        0        0     1441 2024-02-20 11:51:54.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/utils/download.py
+-rw-rw-rw-   0        0        0      642 2023-09-01 13:43:06.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/utils/fileutils.py
+-rw-rw-rw-   0        0        0      575 2023-09-26 08:58:11.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/utils/random.py
+drwxrwxrwx   0        0        0        0 2024-04-30 12:14:13.150684 cesnet_datazoo-0.1.5/cesnet_datazoo.egg-info/
+-rw-rw-rw-   0        0        0    12953 2024-04-30 12:14:13.000000 cesnet_datazoo-0.1.5/cesnet_datazoo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1194 2024-04-30 12:14:13.000000 cesnet_datazoo-0.1.5/cesnet_datazoo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 12:14:13.000000 cesnet_datazoo-0.1.5/cesnet_datazoo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      238 2024-04-30 12:14:13.000000 cesnet_datazoo-0.1.5/cesnet_datazoo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-30 12:14:13.000000 cesnet_datazoo-0.1.5/cesnet_datazoo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1792 2024-04-30 12:13:18.000000 cesnet_datazoo-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-30 12:14:13.154084 cesnet_datazoo-0.1.5/setup.cfg
```

### Comparing `cesnet_datazoo-0.1.4/LICENCE` & `cesnet_datazoo-0.1.5/LICENCE`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.4/PKG-INFO` & `cesnet_datazoo-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cesnet-datazoo
-Version: 0.1.4
+Version: 0.1.5
 Summary: A toolkit for large network traffic datasets
 Author-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 Maintainer-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/CESNET/cesnet-datazoo
 Project-URL: Documentation, https://cesnet.github.io/cesnet-datazoo/
 Project-URL: Bug Tracker, https://github.com/CESNET/cesnet-datazoo/issues
```

### Comparing `cesnet_datazoo-0.1.4/README.md` & `cesnet_datazoo-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.4/cesnet_datazoo/config.py` & `cesnet_datazoo-0.1.5/cesnet_datazoo/config.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.4/cesnet_datazoo/constants.py` & `cesnet_datazoo-0.1.5/cesnet_datazoo/constants.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/cesnet_dataset.py` & `cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/cesnet_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,24 @@
 from functools import partial
 from typing import Callable, Literal, Optional
 
 import numpy as np
 import pandas as pd
 import tables as tb
 import torch
+from numpy.lib.recfunctions import repack_fields
 from sklearn.model_selection import train_test_split
 from sklearn.preprocessing import LabelEncoder
 from torch.utils.data import BatchSampler, DataLoader, RandomSampler, Sampler, SequentialSampler
 from typing_extensions import assert_never
 
 from cesnet_datazoo.config import AppSelection, DataLoaderOrder, DatasetConfig, ValidationApproach
 from cesnet_datazoo.constants import (APP_COLUMN, CATEGORY_COLUMN, DATASET_SIZES, INDICES_APP_FIELD,
-                                      SERVICEMAP_FILE, UNKNOWN_STR_LABEL)
+                                      INDICES_INDEX_FIELD, INDICES_TABLE_FIELD, SERVICEMAP_FILE,
+                                      UNKNOWN_STR_LABEL)
 from cesnet_datazoo.datasets.loaders import collate_fn_simple, create_df_from_dataloader
 from cesnet_datazoo.datasets.metadata.dataset_metadata import DatasetMetadata, load_metadata
 from cesnet_datazoo.datasets.statistics import compute_dataset_statistics
 from cesnet_datazoo.pytables_data.apps_split import is_background_app
 from cesnet_datazoo.pytables_data.data_scalers import fit_scalers
 from cesnet_datazoo.pytables_data.indices_setup import (IndicesTuple, compute_known_app_counts,
                                                         compute_unknown_app_counts,
@@ -615,15 +617,15 @@
         encode_labels_with_unknown_fn = partial(_encode_labels_with_unknown, encoder=encoder, class_info=class_info)
         # Create train, validation, and test datasets
         train_dataset = val_dataset = test_dataset = None
         if dataset_config.need_train_set:
             train_dataset = PyTablesDataset(
                 database_path=dataset_config.database_path,
                 tables_paths=dataset_config._get_train_tables_paths(),
-                indices=dataset_indices.train_indices,
+                indices=repack_fields(dataset_indices.train_indices[[INDICES_TABLE_FIELD, INDICES_INDEX_FIELD]]), # type: ignore
                 tables_app_enum=self._tables_app_enum,
                 tables_cat_enum=self._tables_cat_enum,
                 flowstats_features=dataset_config.flowstats_features,
                 flowstats_features_boolean=dataset_config.flowstats_features_boolean,
                 flowstats_features_phist=dataset_config.flowstats_features_phist,
                 other_fields=self.dataset_config.other_fields,
                 sni_column=self.dataset_config.sni_column,
@@ -634,15 +636,15 @@
                 target_transform=encode_labels_with_unknown_fn,
                 return_tensors=dataset_config.return_tensors,)
         if dataset_config.need_val_set:
             assert val_data_path is not None
             val_dataset = PyTablesDataset(
                 database_path=dataset_config.database_path,
                 tables_paths=dataset_config._get_val_tables_paths(),
-                indices=dataset_indices.val_known_indices,
+                indices=repack_fields(dataset_indices.val_known_indices[[INDICES_TABLE_FIELD, INDICES_INDEX_FIELD]]), # type: ignore
                 tables_app_enum=self._tables_app_enum,
                 tables_cat_enum=self._tables_cat_enum,
                 flowstats_features=dataset_config.flowstats_features,
                 flowstats_features_boolean=dataset_config.flowstats_features_boolean,
                 flowstats_features_phist=dataset_config.flowstats_features_phist,
                 other_fields=self.dataset_config.other_fields,
                 sni_column=self.dataset_config.sni_column,
@@ -655,15 +657,15 @@
                 preload=dataset_config.preload_val,
                 preload_blob=os.path.join(val_data_path, "preload", f"val_dataset-{dataset_config.val_known_size}.npz"),)
         if dataset_config.need_test_set:
             assert test_data_path is not None
             test_dataset = PyTablesDataset(
                 database_path=dataset_config.database_path,
                 tables_paths=dataset_config._get_test_tables_paths(),
-                indices=test_combined_indices,
+                indices=repack_fields(test_combined_indices[[INDICES_TABLE_FIELD, INDICES_INDEX_FIELD]]), # type: ignore
                 tables_app_enum=self._tables_app_enum,
                 tables_cat_enum=self._tables_cat_enum,
                 flowstats_features=dataset_config.flowstats_features,
                 flowstats_features_boolean=dataset_config.flowstats_features_boolean,
                 flowstats_features_phist=dataset_config.flowstats_features_phist,
                 other_fields=self.dataset_config.other_fields,
                 sni_column=self.dataset_config.sni_column,
```

### Comparing `cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/datasets.py` & `cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/datasets_constants.py` & `cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/datasets_constants.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/loaders.py` & `cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/loaders.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/metadata/dataset_metadata.py` & `cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/metadata/dataset_metadata.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/metadata/metadata.csv` & `cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/metadata/metadata.csv`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/statistics.py` & `cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/statistics.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.4/cesnet_datazoo/metrics/classification_report.py` & `cesnet_datazoo-0.1.5/cesnet_datazoo/metrics/classification_report.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.4/cesnet_datazoo/metrics/provider_metrics.py` & `cesnet_datazoo-0.1.5/cesnet_datazoo/metrics/provider_metrics.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.4/cesnet_datazoo/pytables_data/apps_split.py` & `cesnet_datazoo-0.1.5/cesnet_datazoo/pytables_data/apps_split.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.4/cesnet_datazoo/pytables_data/data_scalers.py` & `cesnet_datazoo-0.1.5/cesnet_datazoo/pytables_data/data_scalers.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,26 +42,28 @@
     if clip_and_scale_ppi_transform is not None and clip_and_scale_ppi_transform.needs_fitting:
         assert isinstance(clip_and_scale_ppi_transform, ClipAndScalePPI)
         data_ppi = data[PPI_COLUMN].astype("float32")
         ppi_channels = data_ppi.shape[1]
         data_ppi = data_ppi.transpose(0, 2, 1).reshape(-1, ppi_channels)
         padding_mask = data_ppi[:, DIR_POS] == 0 # Mask of padded packets
         # Fit IPT scaler
-        train_ipt = data_ppi[:, IPT_POS].clip(max=clip_and_scale_ppi_transform.ipt_max, min=clip_and_scale_ppi_transform.ipt_min)
-        train_ipt[padding_mask] = np.nan # NaNs are ignored in sklearn scalers
-        if isinstance(clip_and_scale_ppi_transform.ipt_scaler, MinMaxScaler):
-            # Let zero be the minimum for minmax scaling
-            train_ipt = np.concatenate((train_ipt, [0]))
-        clip_and_scale_ppi_transform.ipt_scaler.fit(train_ipt.reshape(-1, 1))
+        if clip_and_scale_ppi_transform.ipt_scaler:
+            train_ipt = data_ppi[:, IPT_POS].clip(max=clip_and_scale_ppi_transform.ipt_max, min=clip_and_scale_ppi_transform.ipt_min)
+            train_ipt[padding_mask] = np.nan # NaNs are ignored in sklearn scalers
+            if isinstance(clip_and_scale_ppi_transform.ipt_scaler, MinMaxScaler):
+                # Let zero be the minimum for minmax scaling
+                train_ipt = np.concatenate((train_ipt, [0]))
+            clip_and_scale_ppi_transform.ipt_scaler.fit(train_ipt.reshape(-1, 1))
         # Fit packet sizes scaler
-        train_psizes = data_ppi[:, SIZE_POS].clip(max=clip_and_scale_ppi_transform.psizes_max, min=clip_and_scale_ppi_transform.pszies_min)
-        train_psizes[padding_mask] = np.nan
-        if isinstance(clip_and_scale_ppi_transform.psizes_scaler, MinMaxScaler):
-            train_psizes = np.concatenate((train_psizes, [0]))
-        clip_and_scale_ppi_transform.psizes_scaler.fit(train_psizes.reshape(-1, 1))
+        if clip_and_scale_ppi_transform.psizes_scaler:
+            train_psizes = data_ppi[:, SIZE_POS].clip(max=clip_and_scale_ppi_transform.psizes_max, min=clip_and_scale_ppi_transform.pszies_min)
+            train_psizes[padding_mask] = np.nan
+            if isinstance(clip_and_scale_ppi_transform.psizes_scaler, MinMaxScaler):
+                train_psizes = np.concatenate((train_psizes, [0]))
+            clip_and_scale_ppi_transform.psizes_scaler.fit(train_psizes.reshape(-1, 1))
         clip_and_scale_ppi_transform.needs_fitting = False
         json.dump(clip_and_scale_ppi_transform.to_dict(), open(os.path.join(train_data_path, "transforms", "ppi-transform.json"), "w"), indent=4)
 
     # Fit the ClipAndScaleFlowstats transform
     if clip_and_scale_flowstats_transform is not None and clip_and_scale_flowstats_transform.needs_fitting:
         assert isinstance(clip_and_scale_flowstats_transform, ClipAndScaleFlowstats)
         train_flowstats = structured_to_unstructured(data[dataset_config.flowstats_features])
```

### Comparing `cesnet_datazoo-0.1.4/cesnet_datazoo/pytables_data/indices_setup.py` & `cesnet_datazoo-0.1.5/cesnet_datazoo/pytables_data/indices_setup.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.4/cesnet_datazoo/pytables_data/pytables_dataset.py` & `cesnet_datazoo-0.1.5/cesnet_datazoo/pytables_data/pytables_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,19 +154,17 @@
         inverted_tables_app_enum = {v: k for k, v in self.tables_app_enum.items()}
         disabled_apps_ids = [inverted_tables_app_enum[app] for app in disabled_apps] if disabled_apps is not None else []
         base_labels = {}
         base_indices = {}
         for i in range(len(tables)):
             base_labels[i] = tables[i].read(field=APP_COLUMN)
             base_indices[i] = np.nonzero(np.isin(base_labels[i], disabled_apps_ids, invert=True))[0]
-        indices = np.column_stack((
+        indices = np.array(list(zip(
             np.concatenate([[table_id] * len(base_indices[table_id]) for table_id in tables]),
-            np.concatenate(list(base_indices.values())),
-            np.concatenate(list(base_labels.values()))
-        )).astype(np.int32)
+            np.concatenate(list(base_indices.values())))), dtype=[field for field in INDICES_DTYPE if field[0] in [INDICES_INDEX_FIELD, INDICES_TABLE_FIELD]])
         self.indices = indices
         database.close()
 
     def cleanup(self):
         self.database.close()
 
 def worker_init_fn(worker_id):
```

### Comparing `cesnet_datazoo-0.1.4/cesnet_datazoo/utils/class_info.py` & `cesnet_datazoo-0.1.5/cesnet_datazoo/utils/class_info.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.4/cesnet_datazoo/utils/download.py` & `cesnet_datazoo-0.1.5/cesnet_datazoo/utils/download.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.4/cesnet_datazoo/utils/fileutils.py` & `cesnet_datazoo-0.1.5/cesnet_datazoo/utils/fileutils.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.4/cesnet_datazoo/utils/random.py` & `cesnet_datazoo-0.1.5/cesnet_datazoo/utils/random.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.4/cesnet_datazoo.egg-info/PKG-INFO` & `cesnet_datazoo-0.1.5/cesnet_datazoo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cesnet-datazoo
-Version: 0.1.4
+Version: 0.1.5
 Summary: A toolkit for large network traffic datasets
 Author-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 Maintainer-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/CESNET/cesnet-datazoo
 Project-URL: Documentation, https://cesnet.github.io/cesnet-datazoo/
 Project-URL: Bug Tracker, https://github.com/CESNET/cesnet-datazoo/issues
```

### Comparing `cesnet_datazoo-0.1.4/cesnet_datazoo.egg-info/SOURCES.txt` & `cesnet_datazoo-0.1.5/cesnet_datazoo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.4/pyproject.toml` & `cesnet_datazoo-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cesnet-datazoo"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   {name = "Jan Luxemburk", email = "luxemburk@cesnet.cz"},
   {name = "Karel Hynek", email = "hynekkar@cesnet.cz"},
 ]
 maintainers = [
   {name = "Jan Luxemburk", email = "luxemburk@cesnet.cz"},
   {name = "Karel Hynek", email = "hynekkar@cesnet.cz"},
```

