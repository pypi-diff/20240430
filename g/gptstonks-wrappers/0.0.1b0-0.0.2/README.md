# Comparing `tmp/gptstonks_wrappers-0.0.1b0.tar.gz` & `tmp/gptstonks_wrappers-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptstonks_wrappers-0.0.1b0.tar", last modified: Mon Apr 15 17:13:21 2024, max compression
+gzip compressed data, was "gptstonks_wrappers-0.0.2.tar", last modified: Tue Apr 30 18:03:19 2024, max compression
```

## Comparing `gptstonks_wrappers-0.0.1b0.tar` & `gptstonks_wrappers-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,15 @@
--rw-r--r--   0        0        0     2812 2024-04-15 16:48:42.259960 gptstonks_wrappers-0.0.1b0/README.md
--rw-r--r--   0        0        0     1954 2024-04-15 17:13:21.547405 gptstonks_wrappers-0.0.1b0/pyproject.toml
--rw-r--r--   0        0        0       28 2024-04-15 17:02:37.148728 gptstonks_wrappers-0.0.1b0/tests/env.sh
--rw-r--r--   0        0        0     5700 2024-04-15 16:40:42.021406 gptstonks_wrappers-0.0.1b0/tests/kernels/test_auto_llama_index.py
--rw-r--r--   0        0        0     3553 2024-04-15 16:40:42.024739 gptstonks_wrappers-0.0.1b0/tests/kernels/test_auto_multistep_query_engine.py
--rw-r--r--   0        0        0      566 2024-04-15 16:40:42.028072 gptstonks_wrappers-0.0.1b0/tests/llms/test_chat_model_llm_iface.py
--rw-r--r--   0        0        0      311 2024-04-13 11:16:30.507370 gptstonks_wrappers-0.0.1b0/tests/llms/test_guidance_wrapper.py
--rw-r--r--   0        0        0     4641 1970-01-01 00:00:00.000000 gptstonks_wrappers-0.0.1b0/PKG-INFO
+-rw-r--r--   0        0        0     2617 2024-04-30 18:03:06.426544 gptstonks_wrappers-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 18:03:06.426544 gptstonks_wrappers-0.0.2/gptstonks/wrappers/__init__.py
+-rw-r--r--   0        0        0      306 2024-04-30 18:03:06.426544 gptstonks_wrappers-0.0.2/gptstonks/wrappers/kernels/__init__.py
+-rw-r--r--   0        0        0     7214 2024-04-30 18:03:06.426544 gptstonks_wrappers-0.0.2/gptstonks/wrappers/kernels/auto_multistep_query_engine.py
+-rw-r--r--   0        0        0    36466 2024-04-30 18:03:06.426544 gptstonks_wrappers-0.0.2/gptstonks/wrappers/kernels/auto_rag.py
+-rw-r--r--   0        0        0       56 2024-04-30 18:03:06.426544 gptstonks_wrappers-0.0.2/gptstonks/wrappers/llms/__init__.py
+-rw-r--r--   0        0        0     1375 2024-04-30 18:03:06.426544 gptstonks_wrappers-0.0.2/gptstonks/wrappers/llms/chat_model_llm_iface.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:03:06.426544 gptstonks_wrappers-0.0.2/gptstonks/wrappers/retrievers/__init__.py
+-rw-r--r--   0        0        0     1287 2024-04-30 18:03:06.426544 gptstonks_wrappers-0.0.2/gptstonks/wrappers/retrievers/hybrid_or_retriever.py
+-rw-r--r--   0        0        0     1537 2024-04-30 18:03:19.070627 gptstonks_wrappers-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       41 2024-04-30 18:03:06.426544 gptstonks_wrappers-0.0.2/tests/env.sh
+-rw-r--r--   0        0        0     3495 2024-04-30 18:03:06.426544 gptstonks_wrappers-0.0.2/tests/kernels/test_auto_multistep_query_engine.py
+-rw-r--r--   0        0        0    12040 2024-04-30 18:03:06.426544 gptstonks_wrappers-0.0.2/tests/kernels/test_auto_rag.py
+-rw-r--r--   0        0        0      567 2024-04-30 18:03:06.430544 gptstonks_wrappers-0.0.2/tests/llms/test_chat_model_llm_iface.py
+-rw-r--r--   0        0        0     4082 1970-01-01 00:00:00.000000 gptstonks_wrappers-0.0.2/PKG-INFO
```

### Comparing `gptstonks_wrappers-0.0.1b0/README.md` & `gptstonks_wrappers-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -18,22 +18,16 @@
 <p align="center">
   <!-- Hugging Face Badge -->
   <a href="https://huggingface.co/"><img src="https://img.shields.io/badge/Hugging%20Face-F58025?style=for-the-badge&logo=huggingface&logoColor=white" alt="Hugging Face Badge"></a>
   <!-- LangChain Badge -->
   <a href="https://langchain.com/">
     <img src="https://img.shields.io/badge/LangChain-005A9C?style=for-the-badge&logo=langchain&logoColor=white" alt="LangChain Badge">
   </a>
-  <!-- FastAPI Badge -->
-  <a href="https://fastapi.tiangolo.com/">
-    <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" alt="FastAPI Badge">
-  </a>
-  <!-- OpenBB Badge -->
-  <a href="https://openbb.co/">
-    <img src="https://img.shields.io/badge/OpenBB-FFA500?style=for-the-badge&logo=openbb&logoColor=white" alt="OpenBB Badge">
-  </a>
+  <!-- LlamaIndex Badge -->
+  <a href="https://www.llamaindex.ai/"><img src="https://img.shields.io/badge/LlamaIndex-ac6aff?style=for-the-badge&logo=llamaindex&logoColor=white" alt="LlamaIndex Badge"></a>
 </p>
 
 # GPTStonks Wrappers
 
 ## Description
 
 GPTStonks Wrappers provides Auto models, similar to the `transformers` library, but for common AI tools instead of models: LangChain, LlamaIndex, etc.
@@ -53,8 +47,8 @@
 
 # install package
 pdm install -dG default
 ```
 
 ## Sample usage with pre-trained models
 
-In the [API project](../../projects/gptstonks_api/), `AutoLlamaIndex` is used to perform [retrieval-augmented generation](https://arxiv.org/abs/2005.11401) (RAG) with [OpenBB](https://openbb.co)'s official documentation and with pre-trained models (e.g., OpenAI, Anthropic, Llama.cpp, etc.). Additionally, `AutoMultiStepQueryEngine` plans and executes Internet searches to solve complex queries.
+In the [API project](../../projects/gptstonks_api/), `AutoRag` is used to perform [retrieval-augmented generation](https://arxiv.org/abs/2005.11401) (RAG) with [OpenBB](https://openbb.co)'s official documentation and with pre-trained models (e.g., OpenAI, Anthropic, Llama.cpp, etc.). Additionally, `AutoMultiStepQueryEngine` plans and executes Internet searches to solve complex queries.
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
                                     [Logo]
 _[_J_o_i_n_ _W_a_i_t_l_i_s_t_ _B_a_d_g_e_]_[_Y_o_u_t_u_b_e_ _C_h_a_n_n_e_l_ _B_a_d_g_e_]_[_X_ _F_o_l_l_o_w_ _U_s_ _B_a_d_g_e_]_[_D_i_s_c_o_r_d_ _B_a_d_g_e_]
                                 _[_D_o_c_k_e_r_ _B_a_d_g_e_]
-      _[_H_u_g_g_i_n_g_ _F_a_c_e_ _B_a_d_g_e_]_[_L_a_n_g_C_h_a_i_n_ _B_a_d_g_e_]_[_F_a_s_t_A_P_I_ _B_a_d_g_e_]_[_O_p_e_n_B_B_ _B_a_d_g_e_]
+            _[_H_u_g_g_i_n_g_ _F_a_c_e_ _B_a_d_g_e_]_[_L_a_n_g_C_h_a_i_n_ _B_a_d_g_e_]_[_L_l_a_m_a_I_n_d_e_x_ _B_a_d_g_e_]
 # GPTStonks Wrappers ## Description GPTStonks Wrappers provides Auto models,
 similar to the `transformers` library, but for common AI tools instead of
 models: LangChain, LlamaIndex, etc. ## Development 1. Install [PDM](https://
 pdm.fming.dev/latest/#installation). 2. Clone the project and install necessary
 packages: ```bash # clone project git clone https://github.com/GPTStonks/
 gptstonks.git cd gptstonks # install pdm pip install pdm # install package pdm
 install -dG default ``` ## Sample usage with pre-trained models In the [API
-project](../../projects/gptstonks_api/), `AutoLlamaIndex` is used to perform
+project](../../projects/gptstonks_api/), `AutoRag` is used to perform
 [retrieval-augmented generation](https://arxiv.org/abs/2005.11401) (RAG) with
 [OpenBB](https://openbb.co)'s official documentation and with pre-trained
 models (e.g., OpenAI, Anthropic, Llama.cpp, etc.). Additionally,
 `AutoMultiStepQueryEngine` plans and executes Internet searches to solve
 complex queries.
```

### Comparing `gptstonks_wrappers-0.0.1b0/tests/kernels/test_auto_multistep_query_engine.py` & `gptstonks_wrappers-0.0.2/tests/kernels/test_auto_multistep_query_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 import os
 from unittest.mock import patch
 
 import pytest
-from gptstonks.wrappers.kernels import AutoMultiStepQueryEngine
-from langchain_community.tools import (
-    DuckDuckGoSearchResults,
-    RequestsGetTool,
-    WikipediaQueryRun,
-)
+from langchain_community.tools import DuckDuckGoSearchResults, WikipediaQueryRun
 from langchain_community.utilities import (
     DuckDuckGoSearchAPIWrapper,
-    TextRequestsWrapper,
     WikipediaAPIWrapper,
 )
 from llama_index.core.query_engine import BaseQueryEngine
 from llama_index.llms.openai import OpenAI
 
+from gptstonks.wrappers.kernels import AutoMultiStepQueryEngine
+
 
 @pytest.mark.asyncio
 @patch.object(BaseQueryEngine, "query")
 @patch.object(BaseQueryEngine, "aquery")
 async def test_factory_react_agent(mocked_aquery, mocked_query):
     os.environ["OPENAI_API_KEY"] = "sk-..."
```

### Comparing `gptstonks_wrappers-0.0.1b0/tests/llms/test_chat_model_llm_iface.py` & `gptstonks_wrappers-0.0.2/tests/llms/test_chat_model_llm_iface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 from collections import namedtuple
 from unittest.mock import patch
 
-from gptstonks.wrappers.llms.chat_model_llm_iface import ChatModelWithLLMIface
 from langchain.chat_models import ChatOpenAI
 
+from gptstonks.wrappers.llms.chat_model_llm_iface import ChatModelWithLLMIface
+
 
 @patch.object(ChatOpenAI, "_generate", return_value=namedtuple("output", "generations")([]))
 def test_chat_model_llm_iface(mocked_generate):
     os.environ["OPENAI_API_KEY"] = "randomkeyfortesting"
     chat = ChatModelWithLLMIface(chat_model=ChatOpenAI(temperature=0))
     chat._generate(["Generate some random story"])
```

### Comparing `gptstonks_wrappers-0.0.1b0/PKG-INFO` & `gptstonks_wrappers-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,35 @@
 Metadata-Version: 2.1
 Name: gptstonks-wrappers
-Version: 0.0.1b0
+Version: 0.0.2
 Summary: Useful wrappers around common AI tools: LangChain, LlamaIndex, etc.
 Author-Email: GPTStonks Team <gptstonks@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Project-URL: Homepage, https://github.com/GPTStonks/gptstonks-core
-Project-URL: Bug tracker, https://github.com/GPTStonks/gptstonks-core/issues
+Project-URL: Homepage, https://github.com/GPTStonks/gptstonks
+Project-URL: Bug tracker, https://github.com/GPTStonks/gptstonks/issues
 Requires-Python: <3.12,>=3.10
 Requires-Dist: rank-bm25>=0.2.2
 Requires-Dist: llama-index>=0.10.13
 Requires-Dist: langchain>=0.0.353
 Requires-Dist: llama-index-llms-openai>=0.1.6
 Requires-Dist: llama-index-retrievers-bm25>=0.1.3
-Requires-Dist: rich<13.0.0,>=12.6.0; extra == "guidance"
-Requires-Dist: transformers>=4.33.0; extra == "guidance"
-Requires-Dist: peft>=0.5.0; extra == "guidance"
-Requires-Dist: accelerate>=0.22.0; extra == "guidance"
-Requires-Dist: bitsandbytes>=0.41.1; extra == "guidance"
-Requires-Dist: sentencepiece>=0.1.99; extra == "guidance"
-Requires-Dist: guidance>=0.0.64; extra == "guidance"
-Requires-Dist: auto-gptq>=0.4.2; extra == "guidance"
-Requires-Dist: optimum>=1.12.0; extra == "guidance"
 Requires-Dist: llama-index-embeddings-huggingface>=0.1.3; extra == "huggingface"
 Requires-Dist: llama-index-llms-huggingface>=0.1.3; extra == "huggingface"
-Requires-Dist: pytest>=8.0.2; extra == "testing"
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
+Requires-Dist: trio>=0.23.2; extra == "testing"
 Requires-Dist: sentence-transformers>=2.2.2; extra == "testing"
-Requires-Dist: pytest-cov[toml]>=4.1.0; extra == "testing"
 Requires-Dist: pytest-asyncio>=0.23.5; extra == "testing"
 Requires-Dist: duckduckgo-search>=4.5.0; extra == "testing"
 Requires-Dist: wikipedia>=1.4.0; extra == "testing"
-Provides-Extra: guidance
+Requires-Dist: pinecone-client>=3.2.2; extra == "testing"
+Requires-Dist: llama-index-vector-stores-pinecone>=0.1.6; extra == "testing"
 Provides-Extra: huggingface
 Provides-Extra: testing
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="../../docs/assets/logo-chatbot.png" alt="Logo">
 </p>
@@ -57,22 +50,16 @@
 <p align="center">
   <!-- Hugging Face Badge -->
   <a href="https://huggingface.co/"><img src="https://img.shields.io/badge/Hugging%20Face-F58025?style=for-the-badge&logo=huggingface&logoColor=white" alt="Hugging Face Badge"></a>
   <!-- LangChain Badge -->
   <a href="https://langchain.com/">
     <img src="https://img.shields.io/badge/LangChain-005A9C?style=for-the-badge&logo=langchain&logoColor=white" alt="LangChain Badge">
   </a>
-  <!-- FastAPI Badge -->
-  <a href="https://fastapi.tiangolo.com/">
-    <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" alt="FastAPI Badge">
-  </a>
-  <!-- OpenBB Badge -->
-  <a href="https://openbb.co/">
-    <img src="https://img.shields.io/badge/OpenBB-FFA500?style=for-the-badge&logo=openbb&logoColor=white" alt="OpenBB Badge">
-  </a>
+  <!-- LlamaIndex Badge -->
+  <a href="https://www.llamaindex.ai/"><img src="https://img.shields.io/badge/LlamaIndex-ac6aff?style=for-the-badge&logo=llamaindex&logoColor=white" alt="LlamaIndex Badge"></a>
 </p>
 
 # GPTStonks Wrappers
 
 ## Description
 
 GPTStonks Wrappers provides Auto models, similar to the `transformers` library, but for common AI tools instead of models: LangChain, LlamaIndex, etc.
@@ -92,8 +79,8 @@
 
 # install package
 pdm install -dG default
 ```
 
 ## Sample usage with pre-trained models
 
-In the [API project](../../projects/gptstonks_api/), `AutoLlamaIndex` is used to perform [retrieval-augmented generation](https://arxiv.org/abs/2005.11401) (RAG) with [OpenBB](https://openbb.co)'s official documentation and with pre-trained models (e.g., OpenAI, Anthropic, Llama.cpp, etc.). Additionally, `AutoMultiStepQueryEngine` plans and executes Internet searches to solve complex queries.
+In the [API project](../../projects/gptstonks_api/), `AutoRag` is used to perform [retrieval-augmented generation](https://arxiv.org/abs/2005.11401) (RAG) with [OpenBB](https://openbb.co)'s official documentation and with pre-trained models (e.g., OpenAI, Anthropic, Llama.cpp, etc.). Additionally, `AutoMultiStepQueryEngine` plans and executes Internet searches to solve complex queries.
```

#### html2text {}

```diff
@@ -1,43 +1,38 @@
-Metadata-Version: 2.1 Name: gptstonks-wrappers Version: 0.0.1b0 Summary: Useful
+Metadata-Version: 2.1 Name: gptstonks-wrappers Version: 0.0.2 Summary: Useful
 wrappers around common AI tools: LangChain, LlamaIndex, etc. Author-Email:
 GPTStonks Team
 gmail.com> License: MIT Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Project-URL: Homepage, https://github.com/GPTStonks/
-gptstonks-core Project-URL: Bug tracker, https://github.com/GPTStonks/
-gptstonks-core/issues Requires-Python: <3.12,>=3.10 Requires-Dist: rank-
-bm25>=0.2.2 Requires-Dist: llama-index>=0.10.13 Requires-Dist:
-langchain>=0.0.353 Requires-Dist: llama-index-llms-openai>=0.1.6 Requires-Dist:
-llama-index-retrievers-bm25>=0.1.3 Requires-Dist: rich<13.0.0,>=12.6.0; extra
-== "guidance" Requires-Dist: transformers>=4.33.0; extra == "guidance"
-Requires-Dist: peft>=0.5.0; extra == "guidance" Requires-Dist:
-accelerate>=0.22.0; extra == "guidance" Requires-Dist: bitsandbytes>=0.41.1;
-extra == "guidance" Requires-Dist: sentencepiece>=0.1.99; extra == "guidance"
-Requires-Dist: guidance>=0.0.64; extra == "guidance" Requires-Dist: auto-
-gptq>=0.4.2; extra == "guidance" Requires-Dist: optimum>=1.12.0; extra ==
-"guidance" Requires-Dist: llama-index-embeddings-huggingface>=0.1.3; extra ==
+:: OS Independent Project-URL: Homepage, https://github.com/GPTStonks/gptstonks
+Project-URL: Bug tracker, https://github.com/GPTStonks/gptstonks/issues
+Requires-Python: <3.12,>=3.10 Requires-Dist: rank-bm25>=0.2.2 Requires-Dist:
+llama-index>=0.10.13 Requires-Dist: langchain>=0.0.353 Requires-Dist: llama-
+index-llms-openai>=0.1.6 Requires-Dist: llama-index-retrievers-bm25>=0.1.3
+Requires-Dist: llama-index-embeddings-huggingface>=0.1.3; extra ==
 "huggingface" Requires-Dist: llama-index-llms-huggingface>=0.1.3; extra ==
-"huggingface" Requires-Dist: pytest>=8.0.2; extra == "testing" Requires-Dist:
-sentence-transformers>=2.2.2; extra == "testing" Requires-Dist: pytest-cov
-[toml]>=4.1.0; extra == "testing" Requires-Dist: pytest-asyncio>=0.23.5; extra
-== "testing" Requires-Dist: duckduckgo-search>=4.5.0; extra == "testing"
-Requires-Dist: wikipedia>=1.4.0; extra == "testing" Provides-Extra: guidance
-Provides-Extra: huggingface Provides-Extra: testing Description-Content-Type:
-text/markdown
+"huggingface" Requires-Dist: pytest; extra == "testing" Requires-Dist: pytest-
+cov; extra == "testing" Requires-Dist: trio>=0.23.2; extra == "testing"
+Requires-Dist: sentence-transformers>=2.2.2; extra == "testing" Requires-Dist:
+pytest-asyncio>=0.23.5; extra == "testing" Requires-Dist: duckduckgo-
+search>=4.5.0; extra == "testing" Requires-Dist: wikipedia>=1.4.0; extra ==
+"testing" Requires-Dist: pinecone-client>=3.2.2; extra == "testing" Requires-
+Dist: llama-index-vector-stores-pinecone>=0.1.6; extra == "testing" Provides-
+Extra: huggingface Provides-Extra: testing Description-Content-Type: text/
+markdown
                                     [Logo]
 _[_J_o_i_n_ _W_a_i_t_l_i_s_t_ _B_a_d_g_e_]_[_Y_o_u_t_u_b_e_ _C_h_a_n_n_e_l_ _B_a_d_g_e_]_[_X_ _F_o_l_l_o_w_ _U_s_ _B_a_d_g_e_]_[_D_i_s_c_o_r_d_ _B_a_d_g_e_]
                                 _[_D_o_c_k_e_r_ _B_a_d_g_e_]
-      _[_H_u_g_g_i_n_g_ _F_a_c_e_ _B_a_d_g_e_]_[_L_a_n_g_C_h_a_i_n_ _B_a_d_g_e_]_[_F_a_s_t_A_P_I_ _B_a_d_g_e_]_[_O_p_e_n_B_B_ _B_a_d_g_e_]
+            _[_H_u_g_g_i_n_g_ _F_a_c_e_ _B_a_d_g_e_]_[_L_a_n_g_C_h_a_i_n_ _B_a_d_g_e_]_[_L_l_a_m_a_I_n_d_e_x_ _B_a_d_g_e_]
 # GPTStonks Wrappers ## Description GPTStonks Wrappers provides Auto models,
 similar to the `transformers` library, but for common AI tools instead of
 models: LangChain, LlamaIndex, etc. ## Development 1. Install [PDM](https://
 pdm.fming.dev/latest/#installation). 2. Clone the project and install necessary
 packages: ```bash # clone project git clone https://github.com/GPTStonks/
 gptstonks.git cd gptstonks # install pdm pip install pdm # install package pdm
 install -dG default ``` ## Sample usage with pre-trained models In the [API
-project](../../projects/gptstonks_api/), `AutoLlamaIndex` is used to perform
+project](../../projects/gptstonks_api/), `AutoRag` is used to perform
 [retrieval-augmented generation](https://arxiv.org/abs/2005.11401) (RAG) with
 [OpenBB](https://openbb.co)'s official documentation and with pre-trained
 models (e.g., OpenAI, Anthropic, Llama.cpp, etc.). Additionally,
 `AutoMultiStepQueryEngine` plans and executes Internet searches to solve
 complex queries.
```

