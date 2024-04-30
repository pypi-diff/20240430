# Comparing `tmp/mlx_llm-1.0.3.tar.gz` & `tmp/mlx_llm-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlx_llm-1.0.3.tar", max compression
+gzip compressed data, was "mlx_llm-1.0.4.tar", max compression
```

## Comparing `mlx_llm-1.0.3.tar` & `mlx_llm-1.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     7020 2023-12-17 18:14:37.703503 mlx_llm-1.0.3/LICENSE
--rw-r--r--   0        0        0     4056 2024-04-26 13:24:58.253104 mlx_llm-1.0.3/README.md
--rw-r--r--   0        0        0     2346 2024-04-26 15:11:41.976962 mlx_llm-1.0.3/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-26 14:51:50.795408 mlx_llm-1.0.3/src/mlx_llm/__init__.py
--rw-r--r--   0        0        0       37 2024-04-26 13:24:58.257004 mlx_llm-1.0.3/src/mlx_llm/chat/__init__.py
--rw-r--r--   0        0        0     4271 2024-04-26 15:05:25.028107 mlx_llm-1.0.3/src/mlx_llm/chat/chat.py
--rw-r--r--   0        0        0      449 2024-04-26 13:24:58.258114 mlx_llm-1.0.3/src/mlx_llm/chat/utils.py
--rw-r--r--   0        0        0      132 2024-04-26 13:24:58.258969 mlx_llm-1.0.3/src/mlx_llm/model/__init__.py
--rw-r--r--   0        0        0      406 2024-04-26 13:24:58.259541 mlx_llm-1.0.3/src/mlx_llm/model/_config.py
--rw-r--r--   0        0        0     4566 2024-04-26 15:06:37.297364 mlx_llm-1.0.3/src/mlx_llm/model/_factory.py
--rw-r--r--   0        0        0    12747 2024-04-26 15:11:45.007197 mlx_llm-1.0.3/src/mlx_llm/model/_registry.py
--rw-r--r--   0        0        0     5552 2024-04-26 14:45:13.721964 mlx_llm-1.0.3/src/mlx_llm/model/_utils.py
--rw-r--r--   0        0        0     5935 2024-04-26 14:32:00.243551 mlx_llm-1.0.3/src/mlx_llm/model/converter.py
--rw-r--r--   0        0        0    12123 2024-04-26 15:10:36.466384 mlx_llm-1.0.3/src/mlx_llm/model/transformer.py
--rw-r--r--   0        0        0     1122 2024-04-26 13:48:34.485319 mlx_llm-1.0.3/src/mlx_llm/prompt/__init__.py
--rw-r--r--   0        0        0      287 2024-04-26 13:24:58.264679 mlx_llm-1.0.3/src/mlx_llm/prompt/_base.py
--rw-r--r--   0        0        0     1691 2024-04-26 14:32:00.238359 mlx_llm-1.0.3/src/mlx_llm/prompt/gemma.py
--rw-r--r--   0        0        0     4333 2024-04-26 13:24:58.265041 mlx_llm-1.0.3/src/mlx_llm/prompt/llama.py
--rw-r--r--   0        0        0     1689 2024-04-26 13:24:58.265937 mlx_llm-1.0.3/src/mlx_llm/prompt/mistral.py
--rw-r--r--   0        0        0      559 2024-04-26 13:24:58.266273 mlx_llm-1.0.3/src/mlx_llm/prompt/phi.py
--rw-r--r--   0        0        0        1 2024-04-26 13:24:58.267232 mlx_llm-1.0.3/src/mlx_llm/utils/__init__.py
--rw-r--r--   0        0        0     1235 2024-04-26 13:24:58.267997 mlx_llm-1.0.3/src/mlx_llm/utils/hf.py
--rw-r--r--   0        0        0     4810 2024-04-26 13:24:58.268439 mlx_llm-1.0.3/src/mlx_llm/utils/session.py
--rw-r--r--   0        0        0     1261 2024-02-09 16:22:28.193671 mlx_llm-1.0.3/src/mlx_llm/utils/time.py
--rw-r--r--   0        0        0     2129 2024-04-26 13:24:58.269430 mlx_llm-1.0.3/src/mlx_llm/utils/weights.py
--rw-r--r--   0        0        0     4965 1970-01-01 00:00:00.000000 mlx_llm-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     7020 2023-12-17 18:14:37.703503 mlx_llm-1.0.4/LICENSE
+-rw-r--r--   0        0        0     4730 2024-04-30 08:49:35.034833 mlx_llm-1.0.4/README.md
+-rw-r--r--   0        0        0     2346 2024-04-30 08:49:32.693547 mlx_llm-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-30 08:49:32.694137 mlx_llm-1.0.4/src/mlx_llm/__init__.py
+-rw-r--r--   0        0        0       37 2024-04-26 13:24:58.257004 mlx_llm-1.0.4/src/mlx_llm/chat/__init__.py
+-rw-r--r--   0        0        0     4097 2024-04-30 08:49:32.694862 mlx_llm-1.0.4/src/mlx_llm/chat/chat.py
+-rw-r--r--   0        0        0      449 2024-04-26 13:24:58.258114 mlx_llm-1.0.4/src/mlx_llm/chat/utils.py
+-rw-r--r--   0        0        0      132 2024-04-26 13:24:58.258969 mlx_llm-1.0.4/src/mlx_llm/model/__init__.py
+-rw-r--r--   0        0        0      447 2024-04-30 08:49:32.695556 mlx_llm-1.0.4/src/mlx_llm/model/_config.py
+-rw-r--r--   0        0        0     4742 2024-04-30 08:49:32.696295 mlx_llm-1.0.4/src/mlx_llm/model/_factory.py
+-rw-r--r--   0        0        0    19666 2024-04-30 08:49:32.697085 mlx_llm-1.0.4/src/mlx_llm/model/_registry.py
+-rw-r--r--   0        0        0     6428 2024-04-30 08:49:32.697930 mlx_llm-1.0.4/src/mlx_llm/model/_utils.py
+-rw-r--r--   0        0        0     8795 2024-04-30 08:49:32.698588 mlx_llm-1.0.4/src/mlx_llm/model/converter.py
+-rw-r--r--   0        0        0    14301 2024-04-30 08:49:32.699154 mlx_llm-1.0.4/src/mlx_llm/model/transformer.py
+-rw-r--r--   0        0        0     1122 2024-04-30 08:49:32.699584 mlx_llm-1.0.4/src/mlx_llm/prompt/__init__.py
+-rw-r--r--   0        0        0      287 2024-04-26 13:24:58.264679 mlx_llm-1.0.4/src/mlx_llm/prompt/_base.py
+-rw-r--r--   0        0        0     1691 2024-04-30 08:49:32.699930 mlx_llm-1.0.4/src/mlx_llm/prompt/gemma.py
+-rw-r--r--   0        0        0     4333 2024-04-26 13:24:58.265041 mlx_llm-1.0.4/src/mlx_llm/prompt/llama.py
+-rw-r--r--   0        0        0     1689 2024-04-26 13:24:58.265937 mlx_llm-1.0.4/src/mlx_llm/prompt/mistral.py
+-rw-r--r--   0        0        0      559 2024-04-26 13:24:58.266273 mlx_llm-1.0.4/src/mlx_llm/prompt/phi.py
+-rw-r--r--   0        0        0        1 2024-04-26 13:24:58.267232 mlx_llm-1.0.4/src/mlx_llm/utils/__init__.py
+-rw-r--r--   0        0        0     1235 2024-04-26 13:24:58.267997 mlx_llm-1.0.4/src/mlx_llm/utils/hf.py
+-rw-r--r--   0        0        0     4810 2024-04-26 13:24:58.268439 mlx_llm-1.0.4/src/mlx_llm/utils/session.py
+-rw-r--r--   0        0        0     1261 2024-02-09 16:22:28.193671 mlx_llm-1.0.4/src/mlx_llm/utils/time.py
+-rw-r--r--   0        0        0     2258 2024-04-30 08:49:32.700387 mlx_llm-1.0.4/src/mlx_llm/utils/weights.py
+-rw-r--r--   0        0        0     5639 1970-01-01 00:00:00.000000 mlx_llm-1.0.4/PKG-INFO
```

### Comparing `mlx_llm-1.0.3/LICENSE` & `mlx_llm-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.3/README.md` & `mlx_llm-1.0.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -5,55 +5,62 @@
 
 Go to the entire [Youtube Video](https://www.youtube.com/watch?v=vB7tk6W6VIw).
 
 ## **How to install 🔨**
 ```
 pip install mlx-llm
 ```
-<!-- git clone https://github.com/riccardomusmeci/mlx-llm
-cd mlx-llm
-pip install . -->
 
 ## **Models 🧠**
+
+Currently, out-of-the-box supported models are:
+
+| Family        |  Models |
+|---------------------|----------------|
+| LLaMA 2                  |     llama_2_7b_chat_hf, llama_2_7b_hf            |
+| LLaMA 3          |  llama_3_8b, llama_3_8b_instruct              |
+| Phi3 |   phi_3_mini_4k_instruct, phi_3_mini_128k_instruct           |
+| Mistral |  mistral_7b_instruct_v0.2, openhermes_2.5_mistral_7b          |
+| TinyLLaMA |     tiny_llama_1.1B_chat_v1.0       |
+| Gemma |  gemma_1.1_2b_it, gemma_1.1_7b_it                    |
+| OpenELM |  openelm_270M_instruct, openelm_450M_instruct, openelm_1.1B_instruct, openelm_3B_instruct |
+
 To create a model with pre-trained weights from HuggingFace:
 
 ```python
 from mlx_llm.model import create_model
 
 # loading weights from HuggingFace
 model = create_model("llama_3_8b_instruct")
 ```
 
 You can also load a new version of pre-trained weights for a specific model directly from HuggingFace:
-- set `weights` by adding `hf://` before the HuggingFace repository
-- load the proper weights converter function  
+- set `weights` by adding `hf://` before the HuggingFace repository 
 - if necessary, specify custom model configs (rope_theta, rope_traditional, vocab_size, norm_eps)
 
 Here's an example of how to to it:
 ```python
 from mlx_llm.model import create_model
-from mlx_llm.model.converter import llama_to_mlxllm
 
+# an example of loading new weights from HuggingFace
+model = create_model(
+    model_name="openelm_1.1B_instruct", # it's the base model
+    weights="hf://apple/OpenELM-1.1B", # new weights from HuggingFace
+)
+
+# an example of loading new weights from HuggingFace with custom model configs
 model = create_model(
     model_name="llama_3_8b_instruct", # it's the base model
     weights="hf://gradientai/Llama-3-8B-Instruct-262k", # new weights from HuggingFace
-    converter=llama_to_mlxllm, # it's the weights converter function for the base model
     model_config={
         "rope_theta": 207112184.0
     }
 )
 ```
 
-To list all available models:
-```python
-from mlx_llm.model import list_models
-
-print(list_models())
-```
-
 ### **Quantization 📉**
 
 To quantize a model and save its weights just use:
 
 ```python
 from mlx_llm.model import create_model, quantize, get_weights
 from mlx_llm.utils.weights import save_weights
@@ -80,15 +87,14 @@
 text = ["I like to play basketball", "I like to play tennis"]
 tokens = tokenizer(text)
 x = mx.array(tokens["input_ids"])
 embeds, _ = model.embed(x, norm=True)
 ```
 
 ## **Applications 📁**
-
 With `mlx-llm` you can run a variety of applications, such as:
 - Chat with an LLM running on Apple Silicon on a Command Line interface
 - Fine-Tuning a model with LoRA or QLoRA
 - Retrieval Augmented Generation (RAG) for Question Answering
 
 ### **Chat with LLM 📱**
 `mlx-llm` comes with tools to easily run your LLM chat on Apple Silicon.
@@ -115,14 +121,17 @@
     ),
     quantized=False, # if you want it faster use the quantization params (e.g., group_size=64, bits=4)
 )
 
 chat.start()
 ```
 
+> [!WARNING]
+> In current release (v1.0.4) OpenELM chat-mode is not supported since Apple did not release the chat template.
+
 ### **Fine-Tuning with LoRA or QLoRA 🚀**
 ```python
 raise NotImplementedError
 ```
 
 ### **Retrieval Augmented Generation (RAG) 📚**
 ```python
```

### Comparing `mlx_llm-1.0.3/pyproject.toml` & `mlx_llm-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlx_llm"
-version = "1.0.3"
+version = "1.0.4"
 description = "Large Language Models (LLMs) applications and tools running on Apple Silicon in real-time with Apple MLX"
 authors = ["Riccardo Musmeci <riccardomusmeci92@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "mlx_llm", from = "src" },
 ]
```

### Comparing `mlx_llm-1.0.3/src/mlx_llm/chat/chat.py` & `mlx_llm-1.0.4/src/mlx_llm/chat/chat.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,30 +15,28 @@
     """Dataclass for chat setup
 
     Raises:
         ValueError: Each element in history must contain a question and an answer.
     """
 
     system: str
-    history: Optional[List[Dict[str, str]]] = None
+    history: List[Dict[str, str]] = ()
 
     def session(self) -> Session:
         """Create session
 
         Raises:
             ValueError: Each element in history must contain a question and an answer.
 
         Returns:
             Session: session
         """
         for el in self.history:  # type: ignore
             if "question" not in el.keys() or "answer" not in el.keys():
                 raise ValueError("Each element in history must contain a question and an answer.")
-        if self.history is None:
-            return Session()
         else:
             return Session(
                 questions=[el["question"] for el in self.history], answers=[el["answer"] for el in self.history]
             )
 
 
 class LLMChat:
@@ -75,19 +73,17 @@
             print(f"[INFO] Quantizing model {model_name} with group_size={group_size} and bits={bits}")
             self.model = quantize(self.model, group_size=group_size, bits=bits)
 
         self.model.eval()
 
     def start(self) -> None:
         """Start chat"""
-        print("\n[INFO] Start chatting! Press 'q' to quit or 'r' to reset conversation.\n")
+        print("[INFO] Start chatting! Press 'q' to quit or 'r' to reset conversation.")
 
-        print("******* CHAT *******")
-        print(f"[SYSTEM] {self.prompt.system}")
-        print(f"[HISTORY]\n{self.session.to_string()}[/HISTORY]")
+        print("\n*************** CHAT ***************")
 
         while True:
             user = input("User: ")
             if user == "q":
                 break
             if user == "r":
                 self.session.reset()
```

### Comparing `mlx_llm-1.0.3/src/mlx_llm/model/_factory.py` & `mlx_llm-1.0.4/src/mlx_llm/model/_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     >>> # Create a LLaMA 3 8B model with pretrained weights from HF.
     >>> model = create_model('llama_2_8b_instruct')
 
     >>> # Create a LLaMA 3 8B model with pretrained weights from HF from another repository.
     >>> model = create_model(
             model_name="llama_3_8b_instruct", # it's the base model
             weights="hf://gradientai/Llama-3-8B-Instruct-262k", # new weights from HuggingFace
-            converter=llama_to_mlxllm, # it's the weights converter function for the base model
             model_config={ "rope_theta": 207112184.0 }
     >>> )
 
     >>> # Create a LLaMA 3 8B model model with custom local weights.
     >>> model = create_model('llama_2_8b_instruct', weights="path/to/model.safetensors")
     ```
 
@@ -80,17 +79,19 @@
     if isinstance(weights, str) and weights.endswith(".safetensors"):
         model = load_weights(model=model, weights=weights, strict=strict, verbose=verbose)
     elif isinstance(weights, str) and weights.startswith("hf://"):
         model_path = download_from_hf(
             repo_id=weights.replace("hf://", ""),
         )
         weights = glob.glob(os.path.join(model_path, "*.safetensors"))  # type: ignore
-        if converter is not None:
-            weights = converter(weights)
-            model = apply_weights(model, weights)  # type: ignore
+        if len(weights) == 0:
+            raise ValueError(f"No safetensors weights found in {model_path}.")
+        converter = config.converter if converter is None else converter
+        weights = converter(weights)
+        model = apply_weights(model, weights)  # type: ignore
 
     elif isinstance(weights, bool) and weights is True:
         model_path = download_from_hf(
             repo_id=config.hf.repo_id, revision=config.hf.revision, filename=config.hf.filename
         )
         if os.path.isfile(model_path):
             weights = model_path
@@ -118,9 +119,13 @@
     if model_name.startswith("hf://"):
         repo_id = model_name.replace("hf://", "")
         tokenizer = AutoTokenizer.from_pretrained(repo_id, legacy=True)
     elif model_name not in MODEL_ENTRYPOINTS:
         raise ValueError(f"Unknown model name: {model_name}.")
     else:
         _, config = MODEL_ENTRYPOINTS[model_name]()
-        tokenizer = AutoTokenizer.from_pretrained(config.hf.repo_id, legacy=True)
+        if config.tokenizer is not None:
+            repo_id = config.tokenizer.repo_id
+        else:
+            repo_id = config.hf.repo_id
+        tokenizer = AutoTokenizer.from_pretrained(repo_id, legacy=True)
     return tokenizer
```

### Comparing `mlx_llm-1.0.3/src/mlx_llm/model/_registry.py` & `mlx_llm-1.0.4/src/mlx_llm/model/_registry.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from functools import partial
 from typing import Callable, Dict, Optional, Tuple
 
 from ._config import HFConfig, ModelConfig, QuantizeConfig
-from .converter import llama_to_mlxllm, mistral_to_mlxllm, phi3_to_mlxllm
+from ._utils import make_divisible
+from .converter import llama_to_mlxllm, mistral_to_mlxllm, openelm_to_mlxllm, phi3_to_mlxllm
 from .transformer import Transformer
 
 MODEL_ENTRYPOINTS = {}
 
 
 def register_model(name: Optional[str] = None) -> Callable:
     """Register a model entrypoint.
@@ -363,14 +365,15 @@
         n_heads=8,
         n_kv_heads=1,
         head_dim=256,
         norm_eps=norm_eps,
         rope_theta=rope_theta,
         rope_traditional=rope_traditional,
         gemma=True,
+        embed_as_head=True,
     )
 
     config = ModelConfig(hf=HFConfig(repo_id="google/gemma-1.1-2b-it"), converter=llama_to_mlxllm)
 
     return model, config
 
 
@@ -397,12 +400,310 @@
         n_heads=16,
         n_kv_heads=16,
         head_dim=256,
         norm_eps=norm_eps,
         rope_theta=rope_theta,
         rope_traditional=rope_traditional,
         gemma=True,
+        embed_as_head=True,
     )
 
     config = ModelConfig(hf=HFConfig(repo_id="google/gemma-1.1-7b-it"), converter=llama_to_mlxllm)
 
     return model, config
+
+
+@register_model("openelm_3B_instruct")
+def openelm_3B(
+    vocab_size: int = 32000, norm_eps: float = 1e-5, rope_theta: float = 10000, rope_traditional: bool = False
+) -> Tuple[Transformer, ModelConfig]:
+    dim = 3072
+    head_dim = 128
+    num_gqa_groups = 4
+    divisble_by = 256
+    n_kv_heads = [
+        3,
+        3,
+        3,
+        3,
+        4,
+        4,
+        4,
+        4,
+        4,
+        4,
+        4,
+        4,
+        4,
+        4,
+        4,
+        4,
+        4,
+        4,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5,
+        6,
+        6,
+        6,
+        6,
+        6,
+        6,
+    ]
+    mlp_scales = [
+        0.5,
+        0.6,
+        0.7,
+        0.8,
+        0.9,
+        1.0,
+        1.1,
+        1.2,
+        1.3,
+        1.4,
+        1.5,
+        1.6,
+        1.7,
+        1.8,
+        1.9,
+        2.0,
+        2.1,
+        2.2,
+        2.3,
+        2.4,
+        2.5,
+        2.6,
+        2.7,
+        2.8,
+        2.9,
+        3.0,
+        3.1,
+        3.2,
+        3.3,
+        3.4,
+        3.5,
+        3.6,
+        3.7,
+        3.8,
+        3.9,
+        4.0,
+    ]
+
+    n_heads = [num_gqa_groups * el for el in n_kv_heads]
+    hidden_dim = [make_divisible(v=mlp_scale * dim, divisor=divisble_by) for mlp_scale in mlp_scales]
+
+    model = Transformer(
+        dim=dim,
+        hidden_dim=hidden_dim,
+        vocab_size=vocab_size,
+        n_layers=36,
+        n_heads=n_heads,
+        n_kv_heads=n_kv_heads,
+        head_dim=head_dim,
+        norm_eps=norm_eps,
+        rope_traditional=rope_traditional,
+        rope_theta=rope_theta,
+        rope_scaling=None,
+        norm_qk_proj=True,
+        attention_norm_eps=norm_eps,
+        embed_as_head=True,
+    )
+
+    config = ModelConfig(
+        hf=HFConfig(repo_id="apple/OpenELM-3B-Instruct"),
+        tokenizer=HFConfig(repo_id="meta-llama/Llama-2-7b-hf"),
+        converter=partial(
+            openelm_to_mlxllm,
+            head_dim=head_dim,
+            n_kv_heads=n_kv_heads,
+        ),
+    )
+
+    return model, config
+
+
+@register_model("openelm_1.1B_instruct")
+def openelm_11B(
+    vocab_size: int = 32000, norm_eps: float = 1e-5, rope_theta: float = 10000, rope_traditional: bool = False
+) -> Tuple[Transformer, ModelConfig]:
+    dim = 2048
+    head_dim = 64
+    num_gqa_groups = 4
+    divisble_by = 256
+    n_kv_heads = [4, 4, 4, 5, 5, 5, 5, 5, 5, 5, 6, 6, 6, 6, 6, 6, 6, 6, 7, 7, 7, 7, 7, 7, 8, 8, 8, 8]
+    mlp_scales = [
+        0.5,
+        0.63,
+        0.76,
+        0.89,
+        1.02,
+        1.15,
+        1.28,
+        1.41,
+        1.54,
+        1.67,
+        1.8,
+        1.93,
+        2.06,
+        2.19,
+        2.31,
+        2.44,
+        2.57,
+        2.7,
+        2.83,
+        2.96,
+        3.09,
+        3.22,
+        3.35,
+        3.48,
+        3.61,
+        3.74,
+        3.87,
+        4.0,
+    ]
+    n_heads = [num_gqa_groups * el for el in n_kv_heads]
+    hidden_dim = [make_divisible(v=mlp_scale * dim, divisor=divisble_by) for mlp_scale in mlp_scales]
+
+    model = Transformer(
+        dim=dim,
+        hidden_dim=hidden_dim,
+        vocab_size=vocab_size,
+        n_layers=28,
+        n_heads=n_heads,
+        n_kv_heads=n_kv_heads,
+        head_dim=head_dim,
+        norm_eps=norm_eps,
+        rope_traditional=rope_traditional,
+        rope_theta=rope_theta,
+        rope_scaling=None,
+        norm_qk_proj=True,
+        attention_norm_eps=norm_eps,
+        embed_as_head=True,
+    )
+
+    config = ModelConfig(
+        hf=HFConfig(repo_id="apple/OpenELM-1_1B-Instruct"),
+        tokenizer=HFConfig(repo_id="meta-llama/Llama-2-7b-hf"),
+        converter=partial(
+            openelm_to_mlxllm,
+            head_dim=head_dim,
+            n_kv_heads=n_kv_heads,
+        ),
+    )
+
+    return model, config
+
+
+@register_model("openelm_450M_instruct")
+def openelm_450M(
+    vocab_size: int = 32000, norm_eps: float = 1e-5, rope_theta: float = 10000, rope_traditional: bool = False
+) -> Tuple[Transformer, ModelConfig]:
+    dim = 1536
+    head_dim = 64
+    num_gqa_groups = 4
+    divisble_by = 256
+    n_kv_heads = [3, 3, 3, 4, 4, 4, 4, 4, 4, 4, 5, 5, 5, 5, 5, 5, 6, 6, 6, 6]
+    mlp_scales = [
+        0.5,
+        0.68,
+        0.87,
+        1.05,
+        1.24,
+        1.42,
+        1.61,
+        1.79,
+        1.97,
+        2.16,
+        2.34,
+        2.53,
+        2.71,
+        2.89,
+        3.08,
+        3.26,
+        3.45,
+        3.63,
+        3.82,
+        4.0,
+    ]
+    n_heads = [num_gqa_groups * el for el in n_kv_heads]
+    hidden_dim = [make_divisible(v=mlp_scale * dim, divisor=divisble_by) for mlp_scale in mlp_scales]
+
+    model = Transformer(
+        dim=dim,
+        hidden_dim=hidden_dim,
+        vocab_size=vocab_size,
+        n_layers=20,
+        n_heads=n_heads,
+        n_kv_heads=n_kv_heads,
+        head_dim=head_dim,
+        norm_eps=norm_eps,
+        rope_traditional=rope_traditional,
+        rope_theta=rope_theta,
+        rope_scaling=None,
+        norm_qk_proj=True,
+        attention_norm_eps=norm_eps,
+        embed_as_head=True,
+    )
+
+    config = ModelConfig(
+        hf=HFConfig(repo_id="apple/OpenELM-450M-Instruct"),
+        tokenizer=HFConfig(repo_id="meta-llama/Llama-2-7b-hf"),
+        converter=partial(
+            openelm_to_mlxllm,
+            head_dim=head_dim,
+            n_kv_heads=n_kv_heads,
+        ),
+    )
+
+    return model, config
+
+
+@register_model("openelm_270M_instruct")
+def openelm_270M(
+    vocab_size: int = 32000, norm_eps: float = 1e-5, rope_theta: float = 10000, rope_traditional: bool = False
+) -> Tuple[Transformer, ModelConfig]:
+    dim = 1280
+    head_dim = 64
+    num_gqa_groups = 4
+    divisble_by = 256
+    n_kv_heads = [3, 3, 3, 3, 3, 4, 4, 4, 4, 4, 4, 4, 5, 5, 5, 5]
+    mlp_scales = [0.5, 0.73, 0.97, 1.2, 1.43, 1.67, 1.9, 2.13, 2.37, 2.6, 2.83, 3.07, 3.3, 3.53, 3.77, 4.0]
+    n_heads = [num_gqa_groups * el for el in n_kv_heads]
+    hidden_dim = [make_divisible(v=mlp_scale * dim, divisor=divisble_by) for mlp_scale in mlp_scales]
+
+    model = Transformer(
+        dim=dim,
+        hidden_dim=hidden_dim,
+        vocab_size=vocab_size,
+        n_layers=16,
+        n_heads=n_heads,
+        n_kv_heads=n_kv_heads,
+        head_dim=head_dim,
+        norm_eps=norm_eps,
+        rope_traditional=rope_traditional,
+        rope_theta=rope_theta,
+        rope_scaling=None,
+        norm_qk_proj=True,
+        attention_norm_eps=norm_eps,
+        embed_as_head=True,
+    )
+
+    config = ModelConfig(
+        hf=HFConfig(repo_id="apple/OpenELM-270M-Instruct"),
+        tokenizer=HFConfig(repo_id="meta-llama/Llama-2-7b-hf"),
+        converter=partial(
+            openelm_to_mlxllm,
+            head_dim=head_dim,
+            n_kv_heads=n_kv_heads,
+        ),
+    )
+
+    return model, config
```

### Comparing `mlx_llm-1.0.3/src/mlx_llm/model/_utils.py` & `mlx_llm-1.0.4/src/mlx_llm/model/_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -169,7 +169,33 @@
         answer = tokenizer.decode(token_list)
         print(answer[skip:], end="", flush=True)
         skip = len(answer)
     tock = time.time()
     tokens_per_second = len(tokens) / (tock - tick)
     if stats:
         print(f"\n\n[STATS] Tokens/sec: {tokens_per_second:.3f}")
+
+
+def make_divisible(
+    v: Union[float, int],
+    divisor: Optional[int] = 8,
+    min_value: Optional[Union[float, int]] = None,
+) -> Union[float, int]:
+    """
+    This function is taken from the original tf repo.
+    It ensures that all layers have a channel number that is divisible by the divisor
+    It can be seen at:
+    https://github.com/tensorflow/models/blob/2cfc99eff5e5eb729c6793d2f3d03aa1c9be2b15/research/slim/nets/mobilenet/mobilenet.py#L62
+    Args:
+        v: input value
+        divisor: default to 8
+        min_value: minimum divisor value
+    Returns:
+        new_v: new divisible value
+    """
+    if min_value is None:
+        min_value = divisor
+    new_v = max(min_value, int(v + divisor / 2) // divisor * divisor)
+    # Make sure that round down does not go down by more than 10%.
+    if new_v < 0.9 * v:
+        new_v += divisor
+    return new_v
```

### Comparing `mlx_llm-1.0.3/src/mlx_llm/model/transformer.py` & `mlx_llm-1.0.4/src/mlx_llm/model/transformer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,60 +1,84 @@
 from typing import Dict, List, Optional, Tuple, Union
 
 import mlx.core as mx
 import mlx.nn as nn
 
 
 class RMSNorm(nn.Module):
-    def __init__(self, dims: int, eps: float = 1e-5):
+    """Custom RMSNorm module
+
+    Args:
+        dims (int): model dimension
+        eps (float, optional): epsilon. Defaults to 1e-5.
+    """
+
+    def __init__(self, dims: int, eps: float = 1e-5) -> None:
         super().__init__()
         self.weight = mx.ones((dims,))
         self.eps = eps
 
-    def __call__(self, x):
+    def __call__(self, x: mx.array) -> mx.array:
+        """Forward pass
+
+        Args:
+            x (mx.array): input
+
+        Returns:
+            mx.array: output
+        """
         return mx.fast.rms_norm(x, 1.0 + self.weight, self.eps)
 
 
 class Attention(nn.Module):
     """Attention module
 
     Args:
         dim (int): model dimension
         n_heads (int): number of attention heads
         n_kv_heads (int): number of key-value heads
         head_dim (Optional[int]): head dimension. If None, it is set to dim // n_heads. Defaults to None.
         rope_traditional (bool, optional): whether to use traditional RoPE. Defaults to False.
         rope_theta (float, optional): RoPE theta. Defaults to 1000.
         rope_scaling (Optional[Dict[str, Union[float, str]]], optional): RoPE scaling. Defaults to None.
+        norm_qk_proj (bool, optional): whether to normalize the queries and keys projection (for OpenELM). Defaults to False.
+        attention_norm_eps (float, optional): attention normalization epsilon (for OpenELM). Defaults to 1e-6.
     """
 
     def __init__(
         self,
         dim: int,
         n_heads: int,
         n_kv_heads: int,
         head_dim: Optional[int] = None,
         rope_traditional: bool = False,
         rope_theta: float = 1000,
         rope_scaling: Optional[Dict[str, Union[float, str]]] = None,
-    ):
+        norm_qk_proj: bool = False,
+        attention_norm_eps: float = 1e-6,
+    ) -> None:
         super().__init__()
 
         self.n_heads = n_heads
         self.n_kv_heads = n_kv_heads
+        self.norm_qk_proj = norm_qk_proj
 
         head_dim = dim // n_heads if head_dim is None else head_dim
 
         self.scale = head_dim**-0.5
 
         self.q_proj = nn.Linear(dim, n_heads * head_dim, bias=False)
         self.k_proj = nn.Linear(dim, n_kv_heads * head_dim, bias=False)
         self.v_proj = nn.Linear(dim, n_kv_heads * head_dim, bias=False)
         self.o_proj = nn.Linear(n_heads * head_dim, dim, bias=False)
 
+        if self.norm_qk_proj:
+            self.q_norm = nn.RMSNorm(dims=head_dim, eps=attention_norm_eps)
+            self.k_norm = nn.RMSNorm(dims=head_dim, eps=attention_norm_eps)
+
         rope_scale = 1 / rope_scaling["factor"] if rope_scaling is not None and rope_scaling["type"] == "linear" else 1  # type: ignore
 
         self.rope = nn.RoPE(
             dims=head_dim,
             traditional=rope_traditional,
             base=rope_theta,
             scale=rope_scale,
@@ -81,14 +105,18 @@
         queries, keys, values = self.q_proj(x), self.k_proj(x), self.v_proj(x)
 
         # Prepare the queries, keys and values for the attention computation
         queries = queries.reshape(B, L, self.n_heads, -1).transpose(0, 2, 1, 3)
         keys = keys.reshape(B, L, self.n_kv_heads, -1).transpose(0, 2, 1, 3)
         values = values.reshape(B, L, self.n_kv_heads, -1).transpose(0, 2, 1, 3)
 
+        if self.norm_qk_proj:
+            queries = self.q_norm(queries)
+            keys = self.k_norm(keys)
+
         if kv_cache is not None:
             key_cache, value_cache = kv_cache
             queries = self.rope(queries, offset=key_cache.shape[2])
             keys = self.rope(keys, offset=key_cache.shape[2])
             keys = mx.concatenate([key_cache, keys], axis=2)
             values = mx.concatenate([value_cache, values], axis=2)
         else:
@@ -141,41 +169,47 @@
         n_kv_heads (int): number of key-value heads
         hidden_dim (int): hidden dimension
         norm_eps (float): normalization epsilon
         head_dim (Optional[int], optional): head dimension. Defaults to None.
         rope_traditional (bool, optional): whether to use traditional RoPE. Defaults to False.
         rope_theta (float, optional): RoPE theta. Defaults to 1000.
         rope_scaling (Optional[Dict[str, Union[float, str]]], optional): RoPE scaling. Defaults to None.
+        norm_qk_proj (bool, optional): whether to normalize the queries and keys projection (for OpenELM). Defaults to False.
+        attention_norm_eps (float, optional): attention normalization epsilon (for OpenELM). Defaults to 1e-6.
         gemma (bool, optional): whether using Gemma layers. Defaults to False.
     """
 
     def __init__(
         self,
         dim: int,
         n_heads: int,
         n_kv_heads: int,
         hidden_dim: int,
         norm_eps: float,
         head_dim: Optional[int] = None,
         rope_traditional: bool = False,
         rope_theta: float = 1000,
         rope_scaling: Optional[Dict[str, Union[float, str]]] = None,
+        norm_qk_proj: bool = False,
+        attention_norm_eps: float = 1e-6,
         gemma: bool = False,
     ) -> None:
         super().__init__()
         self.n_heads = n_heads
         self.dim = dim
         self.attention = Attention(
             dim=dim,
             n_heads=n_heads,
             n_kv_heads=n_kv_heads,
             head_dim=head_dim,
             rope_traditional=rope_traditional,
             rope_theta=rope_theta,
             rope_scaling=rope_scaling,
+            norm_qk_proj=norm_qk_proj,
+            attention_norm_eps=attention_norm_eps,
         )
         self.mlp = MLP(dim=dim, hidden_dim=hidden_dim, gemma=gemma)
 
         if not gemma:
             self.attention_norm = nn.RMSNorm(dim, eps=norm_eps)
             self.mlp_norm = nn.RMSNorm(dim, eps=norm_eps)
         else:
@@ -216,63 +250,79 @@
         n_heads (int): number of attention heads
         n_kv_heads (Optional[int]): number of key-value heads. If None, it is set to num_heads. Defaults to None.
         head_dim (Optional[int], optional): head dimension. Defaults to None.
         norm_eps (float): normalization epsilon. Defaults to 1e-5.
         rope_traditional (bool, optional): whether to use traditional RoPE. Defaults to False.
         rope_theta (float, optional): RoPE theta. Defaults to 1000.
         rope_scaling (Optional[Dict[str, Union[float, str]]], optional): RoPE scaling. Defaults to None.
+        norm_qk_proj (bool, optional): whether to normalize the queries and keys projection (for OpenELM). Defaults to False.
+        attention_norm_eps (float, optional): attention normalization epsilon (for OpenELM). Defaults to 1e-6.
         gemma (bool, optional): whether to use Gemma Transformer. Defaults to False.
     """
 
     def __init__(
         self,
         dim: int,
-        hidden_dim: int,
+        hidden_dim: Union[int, List[int]],
         vocab_size: int,
         n_layers: int,
-        n_heads: int,
-        n_kv_heads: Optional[int] = None,
+        n_heads: Union[int, List[int]],
+        n_kv_heads: Optional[Union[int, List[int]]] = None,
         head_dim: Optional[int] = None,
         norm_eps: float = 1e-5,
         rope_traditional: bool = False,
         rope_theta: float = 1000,
         rope_scaling: Optional[Dict[str, Union[float, str]]] = None,
+        norm_qk_proj: bool = False,
+        attention_norm_eps: float = 1e-6,
         gemma: bool = False,
+        embed_as_head: bool = False,
     ):
         super().__init__()
+
+        assert vocab_size > 0
+
         self.dim = dim
         self.hidden_dim = hidden_dim
         self.vocab_size = vocab_size
         self.n_layers = n_layers
         self.gemma = gemma
-        assert self.vocab_size > 0
+        self.embed_as_head = True if self.gemma is True else embed_as_head
+
         if n_kv_heads is None:
             n_kv_heads = n_heads
+
         self.token_embed = nn.Embedding(vocab_size, self.dim)
+
+        if isinstance(hidden_dim, int):
+            hidden_dim = [hidden_dim] * n_layers
+        if isinstance(n_heads, int):
+            n_heads = [n_heads] * n_layers
+        if isinstance(n_kv_heads, int):
+            n_kv_heads = [n_kv_heads] * n_layers
+
         self.layers = [
             TransformerBlock(
                 dim=dim,
-                n_heads=n_heads,
-                n_kv_heads=n_kv_heads,
-                hidden_dim=hidden_dim,
+                n_heads=n_heads[i],
+                n_kv_heads=n_kv_heads[i],
+                hidden_dim=hidden_dim[i],
                 norm_eps=norm_eps,
                 head_dim=head_dim,
                 rope_traditional=rope_traditional,
                 rope_theta=rope_theta,
                 rope_scaling=rope_scaling,
+                norm_qk_proj=norm_qk_proj,
+                attention_norm_eps=attention_norm_eps,
                 gemma=self.gemma,
             )
-            for _ in range(n_layers)
+            for i in range(n_layers)
         ]
-        if not self.gemma:
-            self.norm = nn.RMSNorm(dim, eps=norm_eps)
-            self.head = nn.Linear(dim, vocab_size, bias=False)
-        else:
-            self.norm = RMSNorm(dim, eps=norm_eps)
-            self.head = None  # type: ignore
+        self.norm = nn.RMSNorm(dim, eps=norm_eps) if not self.gemma else RMSNorm(dim, eps=norm_eps)
+        self.head = nn.Linear(dim, vocab_size, bias=False) if not self.embed_as_head else None  # type: ignore
 
     def embed(
         self, x: mx.array, kv_cache: Optional[List[Tuple[mx.array, mx.array]]] = None, norm: bool = False
     ) -> Tuple[mx.array, Optional[List[Tuple[mx.array, mx.array]]]]:
         """Compute embedding for the input tokens.
 
         Args:
@@ -310,15 +360,15 @@
             x (mx.array): input tokens
             kv_cache (Optional[List[mx.array]], optional): key-value cache. Defaults to None.
 
         Returns:
             Tuple[mx.array, List[mx.array]]: output and key-value cache
         """
         x, kv_cache = self.embed(x, kv_cache=kv_cache, norm=True)
-        if self.gemma:
+        if self.embed_as_head:
             out = self.token_embed.as_linear(x)
         else:
             out = self.head(x)
         return out, kv_cache  # type: ignore
 
     def generate(self, x: mx.array, temp: Optional[float] = 0.0):
         """Generate tokens from a given input
```

### Comparing `mlx_llm-1.0.3/src/mlx_llm/prompt/__init__.py` & `mlx_llm-1.0.4/src/mlx_llm/prompt/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ._base import Prompt
-from .llama import LLaMA2Prompt, LLaMA3Prompt, TinyLLaMAPrompt
 from .gemma import GemmaPrompt
+from .llama import LLaMA2Prompt, LLaMA3Prompt, TinyLLaMAPrompt
 from .mistral import MistralPrompt
 from .phi import Phi3Prompt
 
 PROMPT_ENTRYPOINTS = {
     "llama2": LLaMA2Prompt,
     "llama3": LLaMA3Prompt,
     "phi3": Phi3Prompt,
```

### Comparing `mlx_llm-1.0.3/src/mlx_llm/prompt/gemma.py` & `mlx_llm-1.0.4/src/mlx_llm/prompt/gemma.py`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.3/src/mlx_llm/prompt/llama.py` & `mlx_llm-1.0.4/src/mlx_llm/prompt/llama.py`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.3/src/mlx_llm/prompt/mistral.py` & `mlx_llm-1.0.4/src/mlx_llm/prompt/mistral.py`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.3/src/mlx_llm/prompt/phi.py` & `mlx_llm-1.0.4/src/mlx_llm/prompt/phi.py`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.3/src/mlx_llm/utils/hf.py` & `mlx_llm-1.0.4/src/mlx_llm/utils/hf.py`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.3/src/mlx_llm/utils/session.py` & `mlx_llm-1.0.4/src/mlx_llm/utils/session.py`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.3/src/mlx_llm/utils/time.py` & `mlx_llm-1.0.4/src/mlx_llm/utils/time.py`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.3/src/mlx_llm/utils/weights.py` & `mlx_llm-1.0.4/src/mlx_llm/utils/weights.py`

 * *Files 15% similar despite different names*

```diff
@@ -47,27 +47,29 @@
             state_dict = torch.load(ckpt_path, map_location="cpu")
         yield state_dict
 
 
 def weights_to_mlx(
     ckpt_paths: Union[List[str], str],
     show_kv: bool = False,
+    tensor_type: torch.dtype = torch.float16,
 ) -> Dict[str, mx.array]:
     """Convert a checkpoint from PyTorch or safetensors to a MLX weights (Dict[str, mx.array]).
 
     Args:
         ckpt_paths (Union[List[str], str]): path to checkpoint
         show_kv (bool, optional): whether to show key-value pairs. Defaults to False.
+        tensor_type (torch.dtype, optional): tensor type. Defaults to torch.float16.
 
     Returns:
         Dict[str, mx.array]: MLX weights dict (key, mx.array)
     """
     weights = {}
     for state_dict in smart_load(ckpt_paths):
         for k, w in state_dict.items():
             if show_kv:
                 print(k, w.shape)
             if isinstance(w, torch.Tensor):
-                w = w.to(torch.float16).numpy()
+                w = w.to(tensor_type).numpy()
                 w = mx.array(w)
             weights[k] = w
     return weights
```

### Comparing `mlx_llm-1.0.3/PKG-INFO` & `mlx_llm-1.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx_llm
-Version: 1.0.3
+Version: 1.0.4
 Summary: Large Language Models (LLMs) applications and tools running on Apple Silicon in real-time with Apple MLX
 Author: Riccardo Musmeci
 Author-email: riccardomusmeci92@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -31,55 +31,62 @@
 
 Go to the entire [Youtube Video](https://www.youtube.com/watch?v=vB7tk6W6VIw).
 
 ## **How to install 🔨**
 ```
 pip install mlx-llm
 ```
-<!-- git clone https://github.com/riccardomusmeci/mlx-llm
-cd mlx-llm
-pip install . -->
 
 ## **Models 🧠**
+
+Currently, out-of-the-box supported models are:
+
+| Family        |  Models |
+|---------------------|----------------|
+| LLaMA 2                  |     llama_2_7b_chat_hf, llama_2_7b_hf            |
+| LLaMA 3          |  llama_3_8b, llama_3_8b_instruct              |
+| Phi3 |   phi_3_mini_4k_instruct, phi_3_mini_128k_instruct           |
+| Mistral |  mistral_7b_instruct_v0.2, openhermes_2.5_mistral_7b          |
+| TinyLLaMA |     tiny_llama_1.1B_chat_v1.0       |
+| Gemma |  gemma_1.1_2b_it, gemma_1.1_7b_it                    |
+| OpenELM |  openelm_270M_instruct, openelm_450M_instruct, openelm_1.1B_instruct, openelm_3B_instruct |
+
 To create a model with pre-trained weights from HuggingFace:
 
 ```python
 from mlx_llm.model import create_model
 
 # loading weights from HuggingFace
 model = create_model("llama_3_8b_instruct")
 ```
 
 You can also load a new version of pre-trained weights for a specific model directly from HuggingFace:
-- set `weights` by adding `hf://` before the HuggingFace repository
-- load the proper weights converter function  
+- set `weights` by adding `hf://` before the HuggingFace repository 
 - if necessary, specify custom model configs (rope_theta, rope_traditional, vocab_size, norm_eps)
 
 Here's an example of how to to it:
 ```python
 from mlx_llm.model import create_model
-from mlx_llm.model.converter import llama_to_mlxllm
 
+# an example of loading new weights from HuggingFace
+model = create_model(
+    model_name="openelm_1.1B_instruct", # it's the base model
+    weights="hf://apple/OpenELM-1.1B", # new weights from HuggingFace
+)
+
+# an example of loading new weights from HuggingFace with custom model configs
 model = create_model(
     model_name="llama_3_8b_instruct", # it's the base model
     weights="hf://gradientai/Llama-3-8B-Instruct-262k", # new weights from HuggingFace
-    converter=llama_to_mlxllm, # it's the weights converter function for the base model
     model_config={
         "rope_theta": 207112184.0
     }
 )
 ```
 
-To list all available models:
-```python
-from mlx_llm.model import list_models
-
-print(list_models())
-```
-
 ### **Quantization 📉**
 
 To quantize a model and save its weights just use:
 
 ```python
 from mlx_llm.model import create_model, quantize, get_weights
 from mlx_llm.utils.weights import save_weights
@@ -106,15 +113,14 @@
 text = ["I like to play basketball", "I like to play tennis"]
 tokens = tokenizer(text)
 x = mx.array(tokens["input_ids"])
 embeds, _ = model.embed(x, norm=True)
 ```
 
 ## **Applications 📁**
-
 With `mlx-llm` you can run a variety of applications, such as:
 - Chat with an LLM running on Apple Silicon on a Command Line interface
 - Fine-Tuning a model with LoRA or QLoRA
 - Retrieval Augmented Generation (RAG) for Question Answering
 
 ### **Chat with LLM 📱**
 `mlx-llm` comes with tools to easily run your LLM chat on Apple Silicon.
@@ -141,14 +147,17 @@
     ),
     quantized=False, # if you want it faster use the quantization params (e.g., group_size=64, bits=4)
 )
 
 chat.start()
 ```
 
+> [!WARNING]
+> In current release (v1.0.4) OpenELM chat-mode is not supported since Apple did not release the chat template.
+
 ### **Fine-Tuning with LoRA or QLoRA 🚀**
 ```python
 raise NotImplementedError
 ```
 
 ### **Retrieval Augmented Generation (RAG) 📚**
 ```python
```

