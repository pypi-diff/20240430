# Comparing `tmp/mulsi-0.1.1.tar.gz` & `tmp/mulsi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mulsi-0.1.1.tar", max compression
+gzip compressed data, was "mulsi-0.1.2.tar", max compression
```

## Comparing `mulsi-0.1.1.tar` & `mulsi-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1088 2024-04-12 20:48:26.813043 mulsi-0.1.1/LICENSE
--rw-r--r--   0        0        0       82 2024-04-12 20:48:26.813043 mulsi-0.1.1/README.md
--rw-r--r--   0        0        0     1247 2024-04-12 20:48:26.817044 mulsi-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      265 2024-04-12 20:48:26.817044 mulsi-0.1.1/src/mulsi/__init__.py
--rw-r--r--   0        0        0     3104 2024-04-12 20:48:26.817044 mulsi-0.1.1/src/mulsi/adversarial.py
--rw-r--r--   0        0        0     5486 2024-04-12 20:48:26.817044 mulsi-0.1.1/src/mulsi/hook.py
--rw-r--r--   0        0        0     3154 2024-04-12 20:48:26.817044 mulsi-0.1.1/src/mulsi/probe.py
--rw-r--r--   0        0        0     2097 2024-04-12 20:48:26.817044 mulsi-0.1.1/src/mulsi/processor.py
--rw-r--r--   0        0        0     1058 2024-04-12 20:48:26.817044 mulsi-0.1.1/src/mulsi/reader.py
--rw-r--r--   0        0        0     4043 2024-04-12 20:48:26.817044 mulsi-0.1.1/src/mulsi/representation.py
--rw-r--r--   0        0        0     2206 2024-04-12 20:48:26.817044 mulsi-0.1.1/src/mulsi/wrapper.py
--rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 mulsi-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1088 2024-04-30 18:07:07.839879 mulsi-0.1.2/LICENSE
+-rw-r--r--   0        0        0       82 2024-04-30 18:07:07.839879 mulsi-0.1.2/README.md
+-rw-r--r--   0        0        0     1540 2024-04-30 18:07:07.839879 mulsi-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      297 2024-04-30 18:07:07.843879 mulsi-0.1.2/src/mulsi/__init__.py
+-rw-r--r--   0        0        0     6963 2024-04-30 18:07:07.843879 mulsi-0.1.2/src/mulsi/adversarial.py
+-rw-r--r--   0        0        0     1139 2024-04-30 18:07:07.843879 mulsi-0.1.2/src/mulsi/clf.py
+-rw-r--r--   0        0        0     5530 2024-04-30 18:07:07.843879 mulsi-0.1.2/src/mulsi/hook.py
+-rw-r--r--   0        0        0     2689 2024-04-30 18:07:07.843879 mulsi-0.1.2/src/mulsi/preprocess.py
+-rw-r--r--   0        0        0     3154 2024-04-30 18:07:07.843879 mulsi-0.1.2/src/mulsi/probe.py
+-rw-r--r--   0        0        0     1073 2024-04-30 18:07:07.843879 mulsi-0.1.2/src/mulsi/reader.py
+-rw-r--r--   0        0        0     4043 2024-04-30 18:07:07.843879 mulsi-0.1.2/src/mulsi/representation.py
+-rw-r--r--   0        0        0     1893 2024-04-30 18:07:07.843879 mulsi-0.1.2/src/mulsi/wrapper.py
+-rw-r--r--   0        0        0      997 1970-01-01 00:00:00.000000 mulsi-0.1.2/PKG-INFO
```

### Comparing `mulsi-0.1.1/LICENSE` & `mulsi-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mulsi-0.1.1/pyproject.toml` & `mulsi-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [tool.isort]
 profile = "black"
 line_length = 79
 src_paths = ["src", "tests", "scripts", "docs", "demo"]
 
 [tool.poetry]
 name = "mulsi"
-version = "0.1.1"
+version = "0.1.2"
 description = "Safe inference using representation engineering."
 readme = "README.md"
 license = "MIT"
 authors = [
     "Yoann Poupart <yoann.poupart@ens-lyon.org>",
     "Imene Kerboua <imene.kerboua@esker.com>",
 ]
@@ -31,30 +31,42 @@
 transformers = "^4.37.2"
 tensordict = "^0.3.0"
 typeguard = "^4.1.5"
 einops = "^0.7.0"
 torchvision = "^0.17.0"
 datasets = {version = "^2.18.0", extras = ["scripts"]}
 wandb = {version = "^0.16.5", extras = ["scripts"]}
+python-semantic-release = "^9.6.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "*"
 pytest = "*"
 pytest-cov = "*"
 gdown = "^5.1.0"
+scikit-learn = "^1.4.2"
 
 [tool.poetry.group.demo]
 optional = true
 
 [tool.poetry.group.demo.dependencies]
 gradio = {extras = ["oauth"], version = "^4.24.0"}
 jsonlines = "^4.0.0"
+huggingface-hub = {extras = ["cli"], version = "^0.22.2"}
 
 [tool.poetry.group.scripts]
 optional = true
 
 [tool.poetry.group.scripts.dependencies]
 datasets = "^2.18.0"
 wandb = "^0.16.5"
+loguru = "^0.7.2"
+scikit-learn = "^1.4.2"
+
+[tool.semantic_release]
+commit_message = "{version}"
+tag_format = "v{version}"
+
+[tool.semantic_release.branches.main]
+match = "main"
```

### Comparing `mulsi-0.1.1/src/mulsi/hook.py` & `mulsi-0.1.2/src/mulsi/hook.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,23 +157,23 @@
 
     def forward_factory(self, name: str):
         if self.config.hook_mode is HookMode.INPUT:
 
             def hook(module, input, output):
                 measure_data = self._get_data(name)
                 self.storage[name] = self.config.data_fn(
-                    input, measure_data=measure_data
+                    input, measure_data=measure_data, name=name
                 )
 
         elif self.config.hook_mode is HookMode.OUTPUT:
 
             def hook(module, input, output):
                 measure_data = self._get_data(name)
                 self.storage[name] = self.config.data_fn(
-                    output, measure_data=measure_data
+                    output, measure_data=measure_data, name=name
                 )
 
         else:
             raise ValueError(f"Unknown measure mode: {self.config.hook_mode}")
         return hook
 
     def backward_factory(self, name: str):
@@ -189,24 +189,24 @@
 
     def forward_factory(self, name: str):
         if self.config.hook_mode is HookMode.INPUT:
 
             def hook(module, input, output):
                 modify_data = self._get_data(name)
                 self.storage[name] = self.config.data_fn(
-                    input, modify_data=modify_data
+                    input, modify_data=modify_data, name=name
                 )
                 return input
 
         elif self.config.hook_mode is HookMode.OUTPUT:
 
             def hook(module, input, output):
                 modify_data = self._get_data(name)
                 self.storage[name] = self.config.data_fn(
-                    output, modify_data=modify_data
+                    output, modify_data=modify_data, name=name
                 )
                 return output
 
         else:
             raise ValueError(f"Unknown modify mode: {self.config.hook_mode}")
 
         return hook
```

### Comparing `mulsi-0.1.1/src/mulsi/probe.py` & `mulsi-0.1.2/src/mulsi/probe.py`

 * *Files identical despite different names*

### Comparing `mulsi-0.1.1/src/mulsi/processor.py` & `mulsi-0.1.2/src/mulsi/preprocess.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 from PIL import Image
 from tensordict import TensorDict
 from torchvision.transforms.functional import pil_to_tensor
 from transformers import CLIPImageProcessor, PreTrainedTokenizer, image_utils
 
 
 @dataclass
-class DiffClipProcessor:
+class DiffCLIPImageProcessor:
     """Differentiable CLIP processor.
 
     TODO: Temporary solution. Should be inheriting from the processor.
     """
 
     processor: CLIPImageProcessor
 
-    def preprocess(self, image):
+    def preprocess(self, image) -> torch.Tensor:
         if isinstance(image, Image.Image):
             image = pil_to_tensor(image).float().unsqueeze(0)
-        if image.dim() != 4:
-            raise NotImplementedError
+        if image.dim() == 3:
+            image = image.unsqueeze(0)
         if self.processor.resample != 3:
             raise NotImplementedError
         size = tuple(self.processor.crop_size.values())
         im_proc = torch.nn.functional.interpolate(
             image, size=size, antialias=True, mode="bicubic"
         )
 
@@ -39,22 +39,28 @@
 
         im_proc = einops.rearrange(
             (einops.rearrange(im_proc, "b c h w -> b h w c") - mean) / std,
             "b h w c -> b c h w",
         )
         return im_proc
 
-    def __call__(self, images, return_tensors="pt", padding=True):
-        if return_tensors != "pt":
-            raise NotImplementedError
-        images = image_utils.make_list_of_images(images)
-        return TensorDict(
-            {"pixel_values": [self.preprocess(image) for image in images]},
-            batch_size=len(images),
-        )
+    def __call__(self, images, **kwargs):
+        kwargs["return_tensors"] = "pt"
+        if isinstance(images, torch.Tensor):
+            if images.dim() == 3:
+                images = images.unsqueeze(0)
+            return {"pixel_values": self.preprocess(images)}
+        else:
+            images = image_utils.make_list_of_images(images)
+            return {
+                "pixel_values": torch.cat(
+                    [self.preprocess(image) for image in images],
+                    dim=0,
+                )
+            }
 
 
 @dataclass
 class TdTokenizer:
     """Tokenizer for Tensordict.
 
     TODO: Temporary solution. Should be inheriting from the tokenizer.
@@ -65,7 +71,21 @@
     def __call__(self, *args, **kwargs):
         kwargs["return_tensors"] = "pt"
         inputs = self.tokenizer(*args, **kwargs)
         return TensorDict(
             {k: v for k, v in inputs.items()},
             batch_size=inputs["input_ids"].shape[0],
         )
+
+
+@dataclass
+class DiffCLIPProcessor:
+    """Differentiable CLIP processor."""
+
+    image_processor: DiffCLIPImageProcessor
+    text_processor: PreTrainedTokenizer
+
+    def __call__(self, images, text=None, **kwargs):
+        outputs = {}
+        outputs.update(self.image_processor(images, **kwargs))
+        outputs.update(self.text_processor(text, **kwargs))
+        return outputs
```

### Comparing `mulsi-0.1.1/src/mulsi/reader.py` & `mulsi-0.1.2/src/mulsi/reader.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """Module for reading representations from a model.
 """
 
 from typing import Union
 
-from mulsi.wrapper import ClipWrapper, LlmWrapper
+from mulsi.wrapper import CLIPModelWrapper, LlmWrapper
 
 
 class ContrastReader:
     """Class to read a representation using contrast vectors."""
 
     def __init__(self, pros_inputs, cons_inputs):
         self.pros_inputs = pros_inputs
         self.cons_inputs = cons_inputs
 
     def read(
         self,
-        wrapper: Union[LlmWrapper, ClipWrapper],
+        wrapper: Union[LlmWrapper, CLIPModelWrapper],
         inputs,
         reading_vector=None,
         **kwargs
     ):
         """Reads the representation."""
         if reading_vector is None:
             reading_vector = self.compute_reading_vector(wrapper, **kwargs)
         return wrapper.compute_representation(inputs, **kwargs).cosim(
             reading_vector
         )
 
     def compute_reading_vector(
-        self, wrapper: Union[LlmWrapper, ClipWrapper], **kwargs
+        self, wrapper: Union[LlmWrapper, CLIPModelWrapper], **kwargs
     ):
         """Reads the representation."""
         return wrapper.compute_representation(
             self.pros_inputs, **kwargs
         ) - wrapper.compute_representation(self.cons_inputs, **kwargs)
```

### Comparing `mulsi-0.1.1/src/mulsi/representation.py` & `mulsi-0.1.2/src/mulsi/representation.py`

 * *Files identical despite different names*

### Comparing `mulsi-0.1.1/src/mulsi/wrapper.py` & `mulsi-0.1.2/src/mulsi/wrapper.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 """Class for MULSI models.
 """
 
 from dataclasses import dataclass
 
 import torch
-from transformers import AutoModelForCausalLM, AutoTokenizer
+from transformers import (
+    AutoModelForCausalLM,
+    AutoTokenizer,
+    CLIPModel,
+    CLIPProcessor,
+)
 
 from mulsi.hook import CacheHook, HookConfig
 from mulsi.representation import Representation
 
 
 @dataclass
 class LlmWrapper:
@@ -35,32 +40,25 @@
         """Computes the loss."""
         encoded_inputs = self.tokenizer(inputs, return_tensors="pt")
         outputs = self.model(**encoded_inputs, labels=labels, **kwargs)
         return outputs.loss
 
 
 @dataclass
-class ClipWrapper:
+class CLIPModelWrapper:
     """Wrapper for CLIP model."""
 
-    model: AutoModelForCausalLM
-    tokenizer: AutoTokenizer
-    _cache_hook = CacheHook(
-        HookConfig(module_exp=r"^transformer\.h\.\d*\.mlp\.act$")
-    )
+    model: CLIPModel
+    processor: CLIPProcessor
+    _cache_hook = CacheHook(HookConfig(module_exp=r"*layers\.\d+\.mlp\.act$"))
 
     @torch.no_grad()
-    def compute_representation(self, inputs, **kwargs) -> Representation:
+    def compute_representation(
+        self, images, text=None, **kwargs
+    ) -> Representation:
         """Computes the representation."""
         self._cache_hook.register(self.model)
-        encoded_inputs = self.tokenizer(inputs, return_tensors="pt")
+        encoded_inputs = self.processor(
+            images=images, text=text, return_tensors="pt"
+        )
         self.model(**encoded_inputs, **kwargs)
-        representation = Representation(self._cache_hook.storage)
-        representation = representation.mean(dim=(0, 1)).flatten()
-        self._cache_hook.clear()
-        return representation
-
-    def compute_loss(self, inputs, labels, **kwargs):
-        """Computes the loss."""
-        encoded_inputs = self.tokenizer(inputs, return_tensors="pt")
-        outputs = self.model(**encoded_inputs, labels=labels, **kwargs)
-        return outputs.loss
+        return Representation(self._cache_hook.storage)
```

### Comparing `mulsi-0.1.1/PKG-INFO` & `mulsi-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: mulsi
-Version: 0.1.1
+Version: 0.1.2
 Summary: Safe inference using representation engineering.
 License: MIT
 Author: Yoann Poupart
 Author-email: yoann.poupart@ens-lyon.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: datasets[scripts] (>=2.18.0,<3.0.0)
 Requires-Dist: einops (>=0.7.0,<0.8.0)
+Requires-Dist: python-semantic-release (>=9.6.0,<10.0.0)
 Requires-Dist: tensordict (>=0.3.0,<0.4.0)
 Requires-Dist: torch (>=2.1.2,<3.0.0)
 Requires-Dist: torchvision (>=0.17.0,<0.18.0)
 Requires-Dist: transformers (>=4.37.2,<5.0.0)
 Requires-Dist: typeguard (>=4.1.5,<5.0.0)
 Requires-Dist: wandb[scripts] (>=0.16.5,<0.17.0)
 Description-Content-Type: text/markdown
```

