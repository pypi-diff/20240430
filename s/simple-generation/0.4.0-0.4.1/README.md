# Comparing `tmp/simple_generation-0.4.0.tar.gz` & `tmp/simple_generation-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_generation-0.4.0.tar", max compression
+gzip compressed data, was "simple_generation-0.4.1.tar", max compression
```

## Comparing `simple_generation-0.4.0.tar` & `simple_generation-0.4.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      590 2024-04-17 15:47:25.745257 simple_generation-0.4.0/LICENSE
--rw-r--r--   0        0        0    15034 2024-04-29 15:27:22.505854 simple_generation-0.4.0/README.md
--rw-r--r--   0        0        0      879 2024-04-29 15:28:02.993927 simple_generation-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      225 2024-04-17 15:47:26.249259 simple_generation-0.4.0/simple_generation/__init__.py
--rw-r--r--   0        0        0    20455 2024-04-29 15:27:22.529854 simple_generation-0.4.0/simple_generation/simple_generation.py
--rw-r--r--   0        0        0     4459 2024-04-17 15:47:26.253259 simple_generation-0.4.0/simple_generation/utils.py
--rw-r--r--   0        0        0       36 2024-04-29 15:27:22.537854 simple_generation-0.4.0/simple_generation/vlm/__init__.py
--rw-r--r--   0        0        0      211 2024-04-29 15:27:22.541854 simple_generation-0.4.0/simple_generation/vlm/config.py
--rw-r--r--   0        0        0    13403 2024-04-29 15:27:22.541854 simple_generation-0.4.0/simple_generation/vlm/vlm.py
--rw-r--r--   0        0        0    16103 1970-01-01 00:00:00.000000 simple_generation-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      590 2024-04-17 15:47:25.745257 simple_generation-0.4.1/LICENSE
+-rw-r--r--   0        0        0    15122 2024-04-30 11:52:24.409385 simple_generation-0.4.1/README.md
+-rw-r--r--   0        0        0      879 2024-04-30 11:52:45.585429 simple_generation-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      225 2024-04-17 15:47:26.249259 simple_generation-0.4.1/simple_generation/__init__.py
+-rw-r--r--   0        0        0    20455 2024-04-29 15:27:22.529854 simple_generation-0.4.1/simple_generation/simple_generation.py
+-rw-r--r--   0        0        0     4459 2024-04-17 15:47:26.253259 simple_generation-0.4.1/simple_generation/utils.py
+-rw-r--r--   0        0        0       36 2024-04-29 15:27:22.537854 simple_generation-0.4.1/simple_generation/vlm/__init__.py
+-rw-r--r--   0        0        0     1826 2024-04-30 11:48:57.944947 simple_generation-0.4.1/simple_generation/vlm/utils.py
+-rw-r--r--   0        0        0    13249 2024-04-30 11:38:15.575406 simple_generation-0.4.1/simple_generation/vlm/vlm.py
+-rw-r--r--   0        0        0    16191 1970-01-01 00:00:00.000000 simple_generation-0.4.1/PKG-INFO
```

### Comparing `simple_generation-0.4.0/LICENSE` & `simple_generation-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_generation-0.4.0/README.md` & `simple_generation-0.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 Install:
 ```bash
 pip install simple-generation
 ```
 
 If you want to use inference with Vision Language Models (VLMs) run:
 ```bash
-pip install simple-generation[vlm]
+pip install "simple-generation[vlm]"
 ```
 
 ## Features
 
 - generate with any model that can be loaded with `AutoModelForCausalLM` or `AutoModelForSeq2SeqLM`
 - batched inference for speed (`batch_size=256`)
 - auto find the largest batch size fitting in your accelerator (`batch_size="auto"`, `starting_batch_size=512`)
@@ -34,15 +34,20 @@
 - carbon emission estimates using [codecarbon](https://mlco2.github.io/codecarbon/)
 - sparsity and fused kernels for speed with [optimum](https://huggingface.co/docs/optimum/main/en/index) (`use_bettertransformer=True`)
 - DDP for single-node, multi-gpu setups using [accelerate](https://github.com/huggingface/accelerate). See [Distributed Inference](#distributed-inference)
 - GUI for quick interaction with models using Gradio's [ChatInterface](https://www.gradio.app/guides/creating-a-chatbot-fast#customizing-your-chatbot). See [Chat Interface](#chat-interface)
 
 **Vision-Language Models**
 
-- all of the above for [LLaVA](https://huggingface.co/docs/transformers/main/en/model_doc/llava#overview), [IDEFICS](https://huggingface.co/docs/transformers/main/en/model_doc/idefics#overview), and [BLIP](https://huggingface.co/docs/transformers/main/en/model_doc/blip#overview). For an example look into `./examples/vlm`.
+- all of the above for [LLaVA](https://huggingface.co/docs/transformers/main/en/model_doc/llava#overview),
+[IDEFICS](https://huggingface.co/docs/transformers/main/en/model_doc/idefics#overview), 
+[IDEFICS2](https://huggingface.co/docs/transformers/v4.40.1/en/model_doc/idefics2),
+and [BLIP](https://huggingface.co/docs/transformers/main/en/model_doc/blip#overview).
+
+For an example look into `./examples/vlm`.
 
 **Loading a Model**
 
 ```python
 from simple_generation import SimpleGenerator
 model_name = "meta-llama/Llama-2-7b-chat-hf"
 generator = SimpleGenerator(model_name, load_in_8bit=True)
@@ -170,14 +175,42 @@
     skip_prompt=False,
     num_beams=5,
     max_new_tokens=256,
     starting_batch_size=128,
 )
 ```
 
+### Distributed Inference
+
+Simple Generation supports DDP to run distributed inference in Single-Node, Multi-GPUs setups. Note that a copy of the model will be instantiated in each GPU (instead of smart weights placements across multiple GPUs with `device_map="auto"`), so **each of your GPU will need to have enough space to fit a copy of the model**.
+
+The only change you'll need to take is launching your script with `accelerate`. E.g.,:
+
+```bash
+accelerate launch --num_processes 2 examples/inference.py # uses 2 GPUs
+```
+
+Note: if you do not specify `--num_processes` all local GPUs will be used.
+
+Some timing tests on 2xA5000 with Llama-2-7b-chat and 384 input prompts:
+
+```shell
+# single GPU
+CUDA_VISIBLE_DEVICES=0 python examples/inference.py
+>> 217s
+
+# two GPUs, smart placement
+CUDA_VISIBLE_DEVICES=0,1 python examples/inference.py
+>> 219s
+
+# two GPUs, DDP
+CUDA_VISIBLE_DEVICES=0,1 accelerate launch --num_processes 2 examples/inference.py
+>> 105s
+```
+
 ### Multiple-Request Conversation
 
 The library supports creating a conversation by prompting models with multiple requests. I.e., it is possible to build a multi-turn conversation with fixed user requests. You can use the `conversation_from_user_prompts()` method, that accepts the same arguments of `__call__`.
 
 For example:
 ```python
 from simple_generation import SimpleGenerator
@@ -247,42 +280,14 @@
 6. Pour the batter into the prepared cake pan and smooth the top.
 7. Bake for 30-35 minutes, or until a toothpick inserted into the center of the cake comes out clean.
 8. Remove the cake from the oven and let it cool in the pan for 10 minutes. Then, remove the cake from the pan and let it cool completely on a wire rack.
 
 This is a basic recipe for a cake, and there are many variations and modifications that can be made to suit your preferences and the occasion for which you are making the cake. For example, you can add flavorings such as vanilla extract or chocolate chips, or use a different type of flour or sugar if you have a specific dietary need or preference.</s></s>
 ```
 
-### Distributed Inference
-
-Simple Generation supports DDP to run distributed inference in Single-Node, Multi-GPUs setups. Note that a copy of the model will be instantiated in each GPU (instead of smart weights placements across multiple GPUs with `device_map="auto"`), so **each of your GPU will need to have enough space to fit a copy of the model**.
-
-The only change you'll need to take is launching your script with `accelerate`. E.g.,:
-
-```bash
-accelerate launch --num_processes 2 examples/inference.py # uses 2 GPUs
-```
-
-Note: if you do not specify `--num_processes` all local GPUs will be used.
-
-Some timing tests on 2xA5000 with Llama-2-7b-chat and 384 input prompts:
-
-```shell
-# single GPU
-CUDA_VISIBLE_DEVICES=0 python examples/inference.py
->> 217s
-
-# two GPUs, smart placement
-CUDA_VISIBLE_DEVICES=0,1 python examples/inference.py
->> 219s
-
-# two GPUs, DDP
-CUDA_VISIBLE_DEVICES=0,1 accelerate launch --num_processes 2 examples/inference.py
->> 105s
-```
-
 ## Defaults
 
 If not specified we set some sensible defaults. **Please note that they might not fit your use case.**
 
 **Default Generation Configuration**
 
 - If not specified otherwise, the library will use the generation configs listed below, **overriding the default config loaded from the specified model**.
```

### Comparing `simple_generation-0.4.0/pyproject.toml` & `simple_generation-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simple-generation"
-version = "0.4.0"
+version = "0.4.1"
 description = "A python package to run inference with HuggingFace checkpoints wrapping many convenient features."
 authors = ["Giuseppe Attanasio <giuseppeattanasio6@gmail.com>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `simple_generation-0.4.0/simple_generation/simple_generation.py` & `simple_generation-0.4.1/simple_generation/simple_generation.py`

 * *Files identical despite different names*

### Comparing `simple_generation-0.4.0/simple_generation/utils.py` & `simple_generation-0.4.1/simple_generation/utils.py`

 * *Files identical despite different names*

### Comparing `simple_generation-0.4.0/simple_generation/vlm/vlm.py` & `simple_generation-0.4.1/simple_generation/vlm/vlm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,43 @@
 import PIL.Image
 import torch
 import torch.distributed as dist
+import pdb
 
 import torch.utils
 import torch.utils.data
 from transformers import (
     GenerationConfig,
     AutoProcessor,
-    AutoTokenizer,
-    LlavaNextForConditionalGeneration,
     IdeficsForVisionText2Text,
-    Blip2ForConditionalGeneration,
-    AutoModelForCausalLM,
-    DataCollatorWithPadding,
+    AutoModelForVision2Seq,
+    AutoConfig,
 )
 from accelerate import Accelerator
 from accelerate.logging import get_logger
 from accelerate.utils import find_executable_batch_size
 from codecarbon import track_emissions
 import PIL
 import dataclasses
 from typing import List, Union, Dict
 from tqdm import tqdm
-from enum import Enum
-from .config import IdeficsHelper
+from .utils import VLMCollator, VLMType
 import math
 import numpy as np
 from datasets import Dataset
 from ..utils import DistributedEvalSampler
 
 
 logger = get_logger(__name__)
 
 inference_decorator = (
     torch.inference_mode if torch.__version__ >= "2.0.0" else torch.no_grad
 )
 
 
-class VLMType(Enum):
-    LLAVA = "LLAVA"
-    IDEFICS = "IDEFICS"
-    QWEN = "QWEN"
-    BLIP2 = "BLIP2"
-
-
 @dataclasses.dataclass
 class DefaultGenerationConfig(GenerationConfig):
     """Default generation configuration.
 
     We apply this parameters to any .generate() call, unless they are not overridden.
 
     Attributes:
@@ -92,49 +82,55 @@
         user_request_move_to_device = False
 
         if "device" in model_kwargs:
             logger.info(f"Setting device to {self.device} per user's request.")
             self.device = model_kwargs.pop("device")
             user_request_move_to_device = True
 
-        # Per-Model configuration
-        if "llava" in self.model_name_or_path.lower():
-            model_cls = LlavaNextForConditionalGeneration
-            self.vlm_type = VLMType.LLAVA
-            # self.processor = AutoProcessor.from_pretrained(self.model_name_or_path)
-        elif "idefics" in self.model_name_or_path.lower():
-            model_cls = IdeficsForVisionText2Text
-            self.vlm_type = VLMType.IDEFICS
-            # self.processor = AutoProcessor.from_pretrained(self.model_name_or_path)
-        elif "blip" in self.model_name_or_path.lower():
-            model_cls = Blip2ForConditionalGeneration
-            self.vlm_type = VLMType.BLIP2
-            # self.processor = AutoProcessor.from_pretrained(self.model_name_or_path)
-        elif "qwen" in self.model_name_or_path.lower():
-            raise NotImplementedError()
-            model_cls = AutoModelForCausalLM
-            self.vlm_type = VLMType.QWEN
-            self.processor = AutoTokenizer.from_pretrained(self.model_name_or_path)
-        else:
-            raise NotImplementedError(f"We do not wrap {model_name_or_path} yet!")
-
         self.processor = AutoProcessor.from_pretrained(self.model_name_or_path)
 
         # padding_size="left" is required for autoregressive models, and should not make a difference for every other model as we use attention_masks. See: https://github.com/huggingface/transformers/issues/3021#issuecomment-1454266627 for a discussion on why left padding is needed on batched inference
         # This is also relevant for VLM batched generation: https://huggingface.co/docs/transformers/model_doc/llava_next#usage-tips
-        self.tokenizer.padding_side = "left"
+        if not hasattr(self.tokenizer, "padding_size"):
+            logger.info("Setting tokenizer.padding_size to 'left'")
+            self.tokenizer.padding_side = "left"
+        if not hasattr(self.tokenizer, "pad_token"):
+            logger.info("Setting tokenizer.pad_token to 'pad'")
+            self.tokenizer.pad_token = "<pad>"
 
         try:
             self.generation_config = GenerationConfig.from_pretrained(
                 model_name_or_path
             )
         except Exception as e:
             logger.warning("Could not load generation config. Using default one.")
             self.generation_config = DefaultGenerationConfig()
 
+        self.config = AutoConfig.from_pretrained(model_name_or_path)
+        if self.config.architectures[0] == "LlavaForConditionalGeneration":
+            self.vlm_type = VLMType.LLAVA
+        elif self.config.architectures[0] == "IdeficsForVisionText2Text":
+            self.vlm_type = VLMType.IDEFICS
+        elif self.config.architectures[0] == "Idefics2ForConditionalGeneration":
+            self.vlm_type = VLMType.IDEFICS2
+        elif self.config.architectures[0] == "Blip2ForConditionalGeneration":
+            self.vlm_type = VLMType.BLIP2
+        else:
+            logger.error(
+                f"Model architecture for {model_name_or_path} is not yet supported"
+            )
+            raise ValueError(
+                f"Model architecture for {model_name_or_path} is not yet supported"
+            )
+
+        model_cls = (
+            IdeficsForVisionText2Text
+            if self.vlm_type == VLMType.IDEFICS
+            else AutoModelForVision2Seq
+        )
         self.model = model_cls.from_pretrained(model_name_or_path, **model_kwargs)
 
         if self.is_ddp or user_request_move_to_device:
             self.model.to(self.device)
             logger.debug(f"Moving model to {self.device}")
 
         self.model.eval()
@@ -149,16 +145,14 @@
 
             Model placement:
             - device_map: {model_kwargs.pop('device_map', None)},
             - device: {self.device},
 
             DDP:
             - distributed inference: {self.is_ddp}
-
-            **Note** We do not enforce input formatting. Be sure to format you inputs according to the used model. See here examples for LlaVA: https://huggingface.co/docs/transformers/model_doc/llava_next#usage-tips
             """
         )
 
     def _prepare_generation_args(self, **generation_kwargs):
         current_generation_args = self.generation_config.to_dict()
 
         logger.info("Setting pad_token_id to eos_token_id for open-end generation")
@@ -194,24 +188,21 @@
     @inference_decorator()
     def __call__(
         self,
         texts,
         images,
         batch_size="auto",
         starting_batch_size=256,
-        num_workers=4,
+        num_workers=0,
         skip_prompt=False,
         log_batch_sample=-1,
         show_progress_bar=None,
         macro_batch_size: int = 512,
         **generation_kwargs,
     ):
-        """
-        TBD.
-        """
 
         if not isinstance(texts, list):
             logger.debug("Texts is not a list. Wrapping it in a list.")
             texts = [texts]
         if not isinstance(images, list):
             logger.debug("Images is not a list. Wrapping it in a list.")
             images = [images]
@@ -226,23 +217,34 @@
         logger.debug("Generation args:", current_generation_args)
 
         # Prepare model specific processor and generation args
         processor_args = dict()
         if self.vlm_type == VLMType.IDEFICS:
             processor_args["add_end_of_utterance_token"] = False
 
-            exit_condition = self.processor.tokenizer(
+            exit_condition = self.tokenizer(
                 "<end_of_utterance>", add_special_tokens=False
             ).input_ids
             generation_kwargs["eos_token_id"] = exit_condition
             bad_words_ids = self.processor.tokenizer(
                 ["<image>", "<fake_token_around_image>"], add_special_tokens=False
             ).input_ids
             generation_kwargs["bad_words_ids"] = bad_words_ids
 
+        # if self.vlm_type == VLMType.LLAVA:
+
+        # pad truncate and batch on the fly (see set_transform())
+        processor_args["truncation"] = True
+        processor_args["return_tensors"] = "pt"
+        if batch_size == "auto" or batch_size > 1:
+            logger.info(
+                f"Found batch size {batch_size}: setting tokenizer.padding to 'longest'"
+            )
+            processor_args["padding"] = "longest"
+
         batch_starts = range(0, len(texts), macro_batch_size)
         responses = list()
         for batch_start_id in tqdm(
             batch_starts,
             desc="Macro batch",
             total=math.ceil(len(texts) / macro_batch_size),
             disable=(len(texts) <= macro_batch_size),
@@ -250,24 +252,15 @@
             curr_prompts = texts[batch_start_id : batch_start_id + macro_batch_size]
             curr_images = images[batch_start_id:macro_batch_size]
 
             if isinstance(curr_images[0], str):
                 curr_images = [PIL.Image.open(i) for i in curr_images]
 
             dataset = Dataset.from_dict({"text": curr_prompts, "image": curr_images})
-            dataset = dataset.map(
-                lambda x: self.processor(x["text"], x["image"], **processor_args),
-                batched=True,
-                remove_columns=["text", "image"],
-                desc="Processing macro batch",
-            )
-
-            collator = DataCollatorWithPadding(
-                self.processor.tokenizer, pad_to_multiple_of=8, return_tensors="pt"
-            )
+            collator = VLMCollator(self.vlm_type, self.processor, processor_args)
 
             def base_loop(batch_size):
                 """Base loop for generation."""
 
                 loader = torch.utils.data.DataLoader(
                     dataset,
                     batch_size=batch_size,
@@ -342,10 +335,12 @@
                 logger.info(
                     f"Finding the optimal batch size... Starting with {starting_batch_size}"
                 )
                 macro_batch_responses = find_batch_size_loop()
             else:
                 macro_batch_responses = base_loop(batch_size)
 
+            # macro_batch_responses = base_loop(batch_size=1)
+
             responses.extend(macro_batch_responses)
 
         return responses
```

### Comparing `simple_generation-0.4.0/PKG-INFO` & `simple_generation-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-generation
-Version: 0.4.0
+Version: 0.4.1
 Summary: A python package to run inference with HuggingFace checkpoints wrapping many convenient features.
 License: Apache Software License 2.0
 Author: Giuseppe Attanasio
 Author-email: giuseppeattanasio6@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -44,15 +44,15 @@
 Install:
 ```bash
 pip install simple-generation
 ```
 
 If you want to use inference with Vision Language Models (VLMs) run:
 ```bash
-pip install simple-generation[vlm]
+pip install "simple-generation[vlm]"
 ```
 
 ## Features
 
 - generate with any model that can be loaded with `AutoModelForCausalLM` or `AutoModelForSeq2SeqLM`
 - batched inference for speed (`batch_size=256`)
 - auto find the largest batch size fitting in your accelerator (`batch_size="auto"`, `starting_batch_size=512`)
@@ -62,15 +62,20 @@
 - carbon emission estimates using [codecarbon](https://mlco2.github.io/codecarbon/)
 - sparsity and fused kernels for speed with [optimum](https://huggingface.co/docs/optimum/main/en/index) (`use_bettertransformer=True`)
 - DDP for single-node, multi-gpu setups using [accelerate](https://github.com/huggingface/accelerate). See [Distributed Inference](#distributed-inference)
 - GUI for quick interaction with models using Gradio's [ChatInterface](https://www.gradio.app/guides/creating-a-chatbot-fast#customizing-your-chatbot). See [Chat Interface](#chat-interface)
 
 **Vision-Language Models**
 
-- all of the above for [LLaVA](https://huggingface.co/docs/transformers/main/en/model_doc/llava#overview), [IDEFICS](https://huggingface.co/docs/transformers/main/en/model_doc/idefics#overview), and [BLIP](https://huggingface.co/docs/transformers/main/en/model_doc/blip#overview). For an example look into `./examples/vlm`.
+- all of the above for [LLaVA](https://huggingface.co/docs/transformers/main/en/model_doc/llava#overview),
+[IDEFICS](https://huggingface.co/docs/transformers/main/en/model_doc/idefics#overview), 
+[IDEFICS2](https://huggingface.co/docs/transformers/v4.40.1/en/model_doc/idefics2),
+and [BLIP](https://huggingface.co/docs/transformers/main/en/model_doc/blip#overview).
+
+For an example look into `./examples/vlm`.
 
 **Loading a Model**
 
 ```python
 from simple_generation import SimpleGenerator
 model_name = "meta-llama/Llama-2-7b-chat-hf"
 generator = SimpleGenerator(model_name, load_in_8bit=True)
@@ -198,14 +203,42 @@
     skip_prompt=False,
     num_beams=5,
     max_new_tokens=256,
     starting_batch_size=128,
 )
 ```
 
+### Distributed Inference
+
+Simple Generation supports DDP to run distributed inference in Single-Node, Multi-GPUs setups. Note that a copy of the model will be instantiated in each GPU (instead of smart weights placements across multiple GPUs with `device_map="auto"`), so **each of your GPU will need to have enough space to fit a copy of the model**.
+
+The only change you'll need to take is launching your script with `accelerate`. E.g.,:
+
+```bash
+accelerate launch --num_processes 2 examples/inference.py # uses 2 GPUs
+```
+
+Note: if you do not specify `--num_processes` all local GPUs will be used.
+
+Some timing tests on 2xA5000 with Llama-2-7b-chat and 384 input prompts:
+
+```shell
+# single GPU
+CUDA_VISIBLE_DEVICES=0 python examples/inference.py
+>> 217s
+
+# two GPUs, smart placement
+CUDA_VISIBLE_DEVICES=0,1 python examples/inference.py
+>> 219s
+
+# two GPUs, DDP
+CUDA_VISIBLE_DEVICES=0,1 accelerate launch --num_processes 2 examples/inference.py
+>> 105s
+```
+
 ### Multiple-Request Conversation
 
 The library supports creating a conversation by prompting models with multiple requests. I.e., it is possible to build a multi-turn conversation with fixed user requests. You can use the `conversation_from_user_prompts()` method, that accepts the same arguments of `__call__`.
 
 For example:
 ```python
 from simple_generation import SimpleGenerator
@@ -275,42 +308,14 @@
 6. Pour the batter into the prepared cake pan and smooth the top.
 7. Bake for 30-35 minutes, or until a toothpick inserted into the center of the cake comes out clean.
 8. Remove the cake from the oven and let it cool in the pan for 10 minutes. Then, remove the cake from the pan and let it cool completely on a wire rack.
 
 This is a basic recipe for a cake, and there are many variations and modifications that can be made to suit your preferences and the occasion for which you are making the cake. For example, you can add flavorings such as vanilla extract or chocolate chips, or use a different type of flour or sugar if you have a specific dietary need or preference.</s></s>
 ```
 
-### Distributed Inference
-
-Simple Generation supports DDP to run distributed inference in Single-Node, Multi-GPUs setups. Note that a copy of the model will be instantiated in each GPU (instead of smart weights placements across multiple GPUs with `device_map="auto"`), so **each of your GPU will need to have enough space to fit a copy of the model**.
-
-The only change you'll need to take is launching your script with `accelerate`. E.g.,:
-
-```bash
-accelerate launch --num_processes 2 examples/inference.py # uses 2 GPUs
-```
-
-Note: if you do not specify `--num_processes` all local GPUs will be used.
-
-Some timing tests on 2xA5000 with Llama-2-7b-chat and 384 input prompts:
-
-```shell
-# single GPU
-CUDA_VISIBLE_DEVICES=0 python examples/inference.py
->> 217s
-
-# two GPUs, smart placement
-CUDA_VISIBLE_DEVICES=0,1 python examples/inference.py
->> 219s
-
-# two GPUs, DDP
-CUDA_VISIBLE_DEVICES=0,1 accelerate launch --num_processes 2 examples/inference.py
->> 105s
-```
-
 ## Defaults
 
 If not specified we set some sensible defaults. **Please note that they might not fit your use case.**
 
 **Default Generation Configuration**
 
 - If not specified otherwise, the library will use the generation configs listed below, **overriding the default config loaded from the specified model**.
```

