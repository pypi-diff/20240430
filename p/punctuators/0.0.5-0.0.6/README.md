# Comparing `tmp/punctuators-0.0.5-py3-none-any.whl.zip` & `tmp/punctuators-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 10176 bytes, number of entries: 13
+Zip file size: 10209 bytes, number of entries: 13
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-28 00:39 punctuators/__init__.py
 -rw-r--r--  2.0 unx      208 b- defN 23-Mar-04 22:49 punctuators/collectors/__init__.py
 -rw-r--r--  2.0 unx     4408 b- defN 23-Mar-12 00:51 punctuators/collectors/pcs_collector.py
 -rw-r--r--  2.0 unx     1682 b- defN 23-Mar-04 23:07 punctuators/collectors/sbd_collector.py
 -rw-r--r--  2.0 unx      140 b- defN 23-Feb-28 23:53 punctuators/data/__init__.py
 -rw-r--r--  2.0 unx     4598 b- defN 23-Mar-01 23:45 punctuators/data/infer_dataset.py
 -rw-r--r--  2.0 unx      177 b- defN 23-Mar-04 22:53 punctuators/models/__init__.py
--rw-r--r--  2.0 unx     6899 b- defN 23-May-29 21:39 punctuators/models/punc_cap_seg_model.py
+-rw-r--r--  2.0 unx     6982 b- defN 24-Apr-29 22:16 punctuators/models/punc_cap_seg_model.py
 -rw-r--r--  2.0 unx     5630 b- defN 23-Mar-04 23:04 punctuators/models/sbd_model.py
--rw-r--r--  2.0 unx      322 b- defN 23-Jun-02 21:07 punctuators-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-02 21:07 punctuators-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jun-02 21:07 punctuators-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1117 b- defN 23-Jun-02 21:07 punctuators-0.0.5.dist-info/RECORD
-13 files, 25285 bytes uncompressed, 8284 bytes compressed:  67.2%
+-rw-r--r--  2.0 unx      322 b- defN 24-Apr-29 22:19 punctuators-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-29 22:19 punctuators-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-Apr-29 22:19 punctuators-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1117 b- defN 24-Apr-29 22:19 punctuators-0.0.6.dist-info/RECORD
+13 files, 25368 bytes uncompressed, 8317 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: punctuators/models/punc_cap_seg_model.py
 Comment: 
 
 Filename: punctuators/models/sbd_model.py
 Comment: 
 
-Filename: punctuators-0.0.5.dist-info/METADATA
+Filename: punctuators-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: punctuators-0.0.5.dist-info/WHEEL
+Filename: punctuators-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: punctuators-0.0.5.dist-info/top_level.txt
+Filename: punctuators-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: punctuators-0.0.5.dist-info/RECORD
+Filename: punctuators-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## punctuators/models/punc_cap_seg_model.py

```diff
@@ -1,10 +1,10 @@
 import os
 from dataclasses import dataclass
-from typing import List, Optional, Dict, Union, Tuple
+from typing import Dict, List, Optional, Tuple, Union
 
 import onnxruntime as ort
 import torch
 from huggingface_hub import hf_hub_download
 from omegaconf import OmegaConf
 from sentencepiece import SentencePieceProcessor
 from torch.utils.data import DataLoader
@@ -46,15 +46,17 @@
         else:
             if cfg.directory is None:
                 raise ValueError(f"Need HF repo ID or local directory name; got {cfg}")
             self._spe_path = os.path.join(cfg.directory, cfg.spe_filename)
             onnx_path = os.path.join(cfg.directory, cfg.model_filename)
             config_path = os.path.join(cfg.directory, cfg.config_filename)
         self._tokenizer: SentencePieceProcessor = SentencePieceProcessor(self._spe_path)  # noqa
-        self._ort_session: ort.InferenceSession = ort.InferenceSession(onnx_path)
+        self._ort_session: ort.InferenceSession = ort.InferenceSession(
+            onnx_path, providers=["CUDAExecutionProvider", "CPUExecutionProvider"]
+        )
         self._config = OmegaConf.load(config_path)
         self._max_len = self._config.max_length
         self._pre_labels: List[str] = self._config.pre_labels
         self._post_labels: List[str] = self._config.post_labels
         self._languages: List[str] = self._config.languages
         self._null_token = self._config.get("null_token", "<NULL>")
```

