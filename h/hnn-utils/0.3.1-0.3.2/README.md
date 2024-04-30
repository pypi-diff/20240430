# Comparing `tmp/hnn_utils-0.3.1.tar.gz` & `tmp/hnn_utils-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnn_utils-0.3.1.tar", max compression
+gzip compressed data, was "hnn_utils-0.3.2.tar", max compression
```

## Comparing `hnn_utils-0.3.1.tar` & `hnn_utils-0.3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1068 2024-04-28 17:40:00.813072 hnn_utils-0.3.1/LICENSE
--rw-r--r--   0        0        0      137 2024-04-28 17:40:00.813072 hnn_utils-0.3.1/README.md
--rw-r--r--   0        0        0        0 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/__init__.py
--rw-r--r--   0        0        0       48 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/callbacks/__init__.py
--rw-r--r--   0        0        0     6566 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/callbacks/ema.py
--rw-r--r--   0        0        0      178 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/datasets/__init__.py
--rw-r--r--   0        0        0     2219 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/datasets/guacamol.py
--rw-r--r--   0        0        0     3119 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/datasets/utils.py
--rw-r--r--   0        0        0     1730 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/datasets/vocab/guac.json
--rw-r--r--   0        0        0     1843 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/datasets/vocab/guac_random.json
--rw-r--r--   0        0        0     5297 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/datasets/vocab/zinc20.json
--rw-r--r--   0        0        0     2721 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/datasets/zinc.py
--rw-r--r--   0        0        0     1370 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/nn/ALiBi.py
--rw-r--r--   0        0        0     1677 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/nn/RotaryEmbedding.py
--rw-r--r--   0        0        0    14366 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/nn/Transformer.py
--rw-r--r--   0        0        0      164 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/nn/__init__.py
--rw-r--r--   0        0        0     1247 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/nn/ffn.py
--rw-r--r--   0        0        0     2000 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/nn/functional.py
--rw-r--r--   0        0        0      800 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/hnn_utils/nn/normalization.py
--rw-r--r--   0        0        0      516 2024-04-28 17:40:00.817072 hnn_utils-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 hnn_utils-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/LICENSE
+-rw-r--r--   0        0        0      137 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/__init__.py
+-rw-r--r--   0        0        0       48 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/callbacks/__init__.py
+-rw-r--r--   0        0        0     6566 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/callbacks/ema.py
+-rw-r--r--   0        0        0      178 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/datasets/__init__.py
+-rw-r--r--   0        0        0     2219 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/datasets/guacamol.py
+-rw-r--r--   0        0        0     3119 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/datasets/utils.py
+-rw-r--r--   0        0        0     1730 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/datasets/vocab/guac.json
+-rw-r--r--   0        0        0     1843 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/datasets/vocab/guac_random.json
+-rw-r--r--   0        0        0     5297 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/datasets/vocab/zinc20.json
+-rw-r--r--   0        0        0     3133 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/datasets/zinc.py
+-rw-r--r--   0        0        0     1370 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/nn/ALiBi.py
+-rw-r--r--   0        0        0     1677 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/nn/RotaryEmbedding.py
+-rw-r--r--   0        0        0    14366 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/nn/Transformer.py
+-rw-r--r--   0        0        0      164 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/nn/__init__.py
+-rw-r--r--   0        0        0     1247 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/nn/ffn.py
+-rw-r--r--   0        0        0     2000 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/nn/functional.py
+-rw-r--r--   0        0        0      800 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/nn/normalization.py
+-rw-r--r--   0        0        0      516 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 hnn_utils-0.3.2/PKG-INFO
```

### Comparing `hnn_utils-0.3.1/LICENSE` & `hnn_utils-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.1/hnn_utils/callbacks/ema.py` & `hnn_utils-0.3.2/hnn_utils/callbacks/ema.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.1/hnn_utils/datasets/guacamol.py` & `hnn_utils-0.3.2/hnn_utils/datasets/guacamol.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.1/hnn_utils/datasets/utils.py` & `hnn_utils-0.3.2/hnn_utils/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.1/hnn_utils/datasets/vocab/guac.json` & `hnn_utils-0.3.2/hnn_utils/datasets/vocab/guac.json`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.1/hnn_utils/datasets/vocab/guac_random.json` & `hnn_utils-0.3.2/hnn_utils/datasets/vocab/guac_random.json`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.1/hnn_utils/datasets/vocab/zinc20.json` & `hnn_utils-0.3.2/hnn_utils/datasets/vocab/zinc20.json`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.1/hnn_utils/datasets/zinc.py` & `hnn_utils-0.3.2/hnn_utils/datasets/zinc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+from typing import Optional
 
 import datasets
 import lightning as L
 import pkg_resources
 from datasets.distributed import split_dataset_by_node
 from torch.utils.data import DataLoader
 
@@ -32,61 +33,69 @@
     def prepare_data(self) -> None:
         datasets.load_dataset(DS_PATH, streaming=True, save_infos=True, split="train")
         datasets.load_dataset(DS_PATH, streaming=True, save_infos=True, split="val")
         datasets.load_dataset(DS_PATH, streaming=True, save_infos=True, split="test")
 
     def train_dataloader(self) -> DataLoader:
         ds = datasets.load_dataset(DS_PATH, streaming=True).select_columns("SELFIES")
-        ds = split_dataset(ds, "train", self.trainer)
+        ds = split_and_shuffle(ds, "train", self.trainer)
 
         transform = build_transform(self.vocab, self.randomize)
 
         return DataLoader(
             ds,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
             pin_memory=True,
             collate_fn=transform,
         )
 
     def val_dataloader(self) -> DataLoader:
         ds = datasets.load_dataset(DS_PATH, streaming=True).select_columns("SELFIES")
-        ds = split_dataset(ds, "val", self.trainer)
+        ds = split_and_shuffle(ds, "val", self.trainer)
 
         transform = build_transform(self.vocab, self.randomize)
 
         return DataLoader(
             ds,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
             pin_memory=True,
             collate_fn=transform,
         )
 
     def test_dataloader(self) -> DataLoader:
         ds = datasets.load_dataset(DS_PATH, streaming=True).select_columns("SELFIES")
-        ds = split_dataset(ds, "test", self.trainer)
+        ds = split_and_shuffle(ds, "test", self.trainer)
 
         transform = build_transform(self.vocab, self.randomize)
 
         return DataLoader(
             ds,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
             pin_memory=True,
             collate_fn=transform,
         )
 
 
-def split_dataset(
-    dataset: datasets.Dataset, split: str, trainer: L.Trainer
+def split_and_shuffle(
+    dataset: datasets.IterableDataset, split: str, trainer: Optional[L.Trainer]
 ) -> datasets.Dataset:
-    if trainer is None:
-        return dataset
-
     dataset = dataset[split]
-    return split_dataset_by_node(
-        dataset, rank=trainer.global_rank, world_size=trainer.world_size
-    )
+
+    # Split according to distributed setup
+    if trainer is not None:
+        dataset = split_dataset_by_node(
+            dataset, rank=trainer.global_rank, world_size=trainer.world_size
+        )
+
+    # Shuffling an iterable dataset shuffles the *shards* and
+    # creates a buffer of size `buffer_size` (in elements, not bytes)
+    # which it randomly samples from. Larger buffer_size
+    # means more memory usage but better shuffling.
+    dataset = dataset.shuffle(buffer_size=16384)
+
+    return dataset
```

### Comparing `hnn_utils-0.3.1/hnn_utils/nn/ALiBi.py` & `hnn_utils-0.3.2/hnn_utils/nn/ALiBi.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.1/hnn_utils/nn/RotaryEmbedding.py` & `hnn_utils-0.3.2/hnn_utils/nn/RotaryEmbedding.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.1/hnn_utils/nn/Transformer.py` & `hnn_utils-0.3.2/hnn_utils/nn/Transformer.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.1/hnn_utils/nn/ffn.py` & `hnn_utils-0.3.2/hnn_utils/nn/ffn.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.1/hnn_utils/nn/functional.py` & `hnn_utils-0.3.2/hnn_utils/nn/functional.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.1/hnn_utils/nn/normalization.py` & `hnn_utils-0.3.2/hnn_utils/nn/normalization.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.1/pyproject.toml` & `hnn_utils-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hnn_utils"
-version = "0.3.1"
+version = "0.3.2"
 description = "Various utilities used throughout my research"
 authors = ["Haydn Jones <haydnjonest@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "hnn_utils" }]
 
 include = ["hnn_utils/datasets/vocab/*.json"]
```

### Comparing `hnn_utils-0.3.1/PKG-INFO` & `hnn_utils-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hnn_utils
-Version: 0.3.1
+Version: 0.3.2
 Summary: Various utilities used throughout my research
 Author: Haydn Jones
 Author-email: haydnjonest@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

