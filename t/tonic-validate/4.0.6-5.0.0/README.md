# Comparing `tmp/tonic_validate-4.0.6.tar.gz` & `tmp/tonic_validate-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonic_validate-4.0.6.tar", max compression
+gzip compressed data, was "tonic_validate-5.0.0.tar", max compression
```

## Comparing `tonic_validate-4.0.6.tar` & `tonic_validate-5.0.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
--rw-r--r--   0        0        0     1063 2024-04-10 16:24:52.697491 tonic_validate-4.0.6/LICENSE
--rw-r--r--   0        0        0    24571 2024-04-10 16:24:52.697491 tonic_validate-4.0.6/README.md
--rw-r--r--   0        0        0      771 2024-04-10 16:24:52.757490 tonic_validate-4.0.6/pyproject.toml
--rw-r--r--   0        0        0      459 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/__init__.py
--rw-r--r--   0        0        0      387 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/classes/__init__.py
--rw-r--r--   0        0        0     2106 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/classes/benchmark.py
--rw-r--r--   0        0        0      247 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/classes/exceptions.py
--rw-r--r--   0        0        0     1023 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/classes/llm_response.py
--rw-r--r--   0        0        0     2630 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/classes/run.py
--rw-r--r--   0        0        0      314 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/classes/user_info.py
--rw-r--r--   0        0        0      805 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/config.py
--rw-r--r--   0        0        0     1483 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/__init__.py
--rw-r--r--   0        0        0     1584 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/answer_consistency_binary_metric.py
--rw-r--r--   0        0        0     1971 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/answer_consistency_metric.py
--rw-r--r--   0        0        0     2784 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/answer_contains_pii_metric.py
--rw-r--r--   0        0        0     1257 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/answer_match_metric.py
--rw-r--r--   0        0        0     1728 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/answer_similarity_metric.py
--rw-r--r--   0        0        0     1844 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/augmentation_accuracy_metric.py
--rw-r--r--   0        0        0     2354 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/augmentation_precision_metric.py
--rw-r--r--   0        0        0     1452 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/binary_metric.py
--rw-r--r--   0        0        0     1747 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/contains_text_metric.py
--rw-r--r--   0        0        0     2808 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/context_contains_pii_metric.py
--rw-r--r--   0        0        0     1786 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/context_length_metric.py
--rw-r--r--   0        0        0     1155 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/duplication_metric.py
--rw-r--r--   0        0        0     1076 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/hate_speech_content_metric.py
--rw-r--r--   0        0        0     1173 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/latency_metric.py
--rw-r--r--   0        0        0      725 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/metric.py
--rw-r--r--   0        0        0     1239 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/regex_metric.py
--rw-r--r--   0        0        0     1448 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/response_length_metric.py
--rw-r--r--   0        0        0     1795 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/retrieval_precision_metric.py
--rw-r--r--   0        0        0     4746 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/services/openai_service.py
--rw-r--r--   0        0        0    18492 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/tests/test_scorer.py
--rw-r--r--   0        0        0        0 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/utils/__init__.py
--rw-r--r--   0        0        0     2880 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/utils/http_client.py
--rw-r--r--   0        0        0    19067 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/utils/llm_calls.py
--rw-r--r--   0        0        0     2198 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/utils/metrics_util.py
--rw-r--r--   0        0        0      530 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/utils/openai_cache.py
--rw-r--r--   0        0        0     4961 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/utils/telemetry.py
--rw-r--r--   0        0        0     4431 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/validate_api.py
--rw-r--r--   0        0        0    13230 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/validate_scorer.py
--rw-r--r--   0        0        0    25330 1970-01-01 00:00:00.000000 tonic_validate-4.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-30 02:42:36.442480 tonic_validate-5.0.0/LICENSE
+-rw-r--r--   0        0        0    26128 2024-04-30 02:42:36.446480 tonic_validate-5.0.0/README.md
+-rw-r--r--   0        0        0      854 2024-04-30 02:42:36.506479 tonic_validate-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0      459 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/__init__.py
+-rw-r--r--   0        0        0      387 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/classes/__init__.py
+-rw-r--r--   0        0        0     2106 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/classes/benchmark.py
+-rw-r--r--   0        0        0      247 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/classes/exceptions.py
+-rw-r--r--   0        0        0     1023 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/classes/llm_response.py
+-rw-r--r--   0        0        0     2630 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/classes/run.py
+-rw-r--r--   0        0        0      314 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/classes/user_info.py
+-rw-r--r--   0        0        0      805 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/config.py
+-rw-r--r--   0        0        0     1483 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/__init__.py
+-rw-r--r--   0        0        0     1693 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/answer_consistency_binary_metric.py
+-rw-r--r--   0        0        0     2077 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/answer_consistency_metric.py
+-rw-r--r--   0        0        0     2878 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/answer_contains_pii_metric.py
+-rw-r--r--   0        0        0     1369 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/answer_match_metric.py
+-rw-r--r--   0        0        0     1837 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/answer_similarity_metric.py
+-rw-r--r--   0        0        0     1952 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/augmentation_accuracy_metric.py
+-rw-r--r--   0        0        0     2442 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/augmentation_precision_metric.py
+-rw-r--r--   0        0        0     1556 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/binary_metric.py
+-rw-r--r--   0        0        0     1834 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/contains_text_metric.py
+-rw-r--r--   0        0        0     2902 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/context_contains_pii_metric.py
+-rw-r--r--   0        0        0     1880 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/context_length_metric.py
+-rw-r--r--   0        0        0     1264 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/duplication_metric.py
+-rw-r--r--   0        0        0     1185 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/hate_speech_content_metric.py
+-rw-r--r--   0        0        0     1285 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/latency_metric.py
+-rw-r--r--   0        0        0      819 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/metric.py
+-rw-r--r--   0        0        0     1351 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/regex_metric.py
+-rw-r--r--   0        0        0     1542 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/response_length_metric.py
+-rw-r--r--   0        0        0     1903 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/retrieval_precision_metric.py
+-rw-r--r--   0        0        0     5882 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/services/litellm_service.py
+-rw-r--r--   0        0        0     4737 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/services/openai_service.py
+-rw-r--r--   0        0        0    18492 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/tests/test_scorer.py
+-rw-r--r--   0        0        0        0 2024-04-30 02:42:36.514479 tonic_validate-5.0.0/tonic_validate/utils/__init__.py
+-rw-r--r--   0        0        0     2880 2024-04-30 02:42:36.514479 tonic_validate-5.0.0/tonic_validate/utils/http_client.py
+-rw-r--r--   0        0        0      527 2024-04-30 02:42:36.514479 tonic_validate-5.0.0/tonic_validate/utils/llm_cache.py
+-rw-r--r--   0        0        0    19347 2024-04-30 02:42:36.514479 tonic_validate-5.0.0/tonic_validate/utils/llm_calls.py
+-rw-r--r--   0        0        0     2198 2024-04-30 02:42:36.514479 tonic_validate-5.0.0/tonic_validate/utils/metrics_util.py
+-rw-r--r--   0        0        0     4961 2024-04-30 02:42:36.514479 tonic_validate-5.0.0/tonic_validate/utils/telemetry.py
+-rw-r--r--   0        0        0     4431 2024-04-30 02:42:36.514479 tonic_validate-5.0.0/tonic_validate/validate_api.py
+-rw-r--r--   0        0        0    13685 2024-04-30 02:42:36.514479 tonic_validate-5.0.0/tonic_validate/validate_scorer.py
+-rw-r--r--   0        0        0    27006 1970-01-01 00:00:00.000000 tonic_validate-5.0.0/PKG-INFO
```

### Comparing `tonic_validate-4.0.6/LICENSE` & `tonic_validate-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.6/README.md` & `tonic_validate-5.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 <h3 align="center">Tonic Validate</h3>
 
   <p align="center">
     A high performance LLM/RAG evaluation framework
     <br />
     <a href="https://docs.tonic.ai/validate"><strong>Explore the docs »</strong></a>
     <br />
+    <a href="https://www.tonic.ai/textual"><strong>Prepare your unstructured data for RAG »</strong></a>
+    <br />
     <br />
     <a href="https://github.com/TonicAI/tonic_validate/issues">Report Bug</a>
     ·
     <a href="https://github.com/TonicAI/tonic_validate/issues">Request Feature</a>
     ·
     <a href="#quick-start">Quick Start</a>
   </p>
@@ -82,16 +84,19 @@
 
 
 <!-- ABOUT THE PROJECT -->
 ## About The Project
 
 Tonic Validate is a framework for the evaluation of LLM outputs, such as Retrieval Augmented Generation (RAG) pipelines. Validate makes it easy to evaluate, track, and monitor your LLM and RAG applications. Validate allows you to evaluate your LLM outputs through the use of our provided metrics which measure everything from answer correctness to LLM hallucination. Additionally, Validate has an optional UI to visualize your evaluation results for easy tracking and monitoring.
 
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
+> **Good RAG systems start with good inputs. Are you blocked on pre-processing messy, complex unstructured data into a standardized format for embedding and ingestion into your vector database?** 
+>
+>Tonic Textual is a privacy-focused ETL for LLMs that standardizes unstructured data for AI development and uses proprietary NER models to create metadata tags that enable improved retreival performance via metadata filtering. If you're spending too much time on data preparation, we can help; reach out to us for a [demo](https://www.tonic.ai/product-demo/textual).
 
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- Quick Start -->
 ## Quick Start
 
 This is an example of how you may give instructions on setting up your project locally.
 To get a local copy up and running follow these simple example steps.
@@ -295,14 +300,29 @@
 If you are using Azure, instead of setting the `OPENAI_API_KEY` environment variable, you instead need to set `AZURE_OPENAI_KEY` and `AZURE_OPENAI_ENDPOINT`. `AZURE_OPENAI_ENDPOINT` is the endpoint url for your Azure OpenAI deployment and `AZURE_OPENAI_KEY` is your API key.
 ```python
 import os
 os.environ["AZURE_OPENAI_KEY"] = "put-your-azure-openai-api-key-here"
 os.environ["AZURE_OPENAI_ENDPOINT"] = "put-your-azure-endpoint-here"
 ```
 
+#### Using Gemini
+If you already have the `GEMINI_API_KEY` set in your system's environment variables then you can skip this step. Otherwise, please set the environment variable before proceeding.
+```python
+import os
+os.environ["GEMINI_API_KEY"] = "put-your-gemini-api-key-here"
+```
+_Note that to use gemini, your Python version must be 3.9 or higher._
+
+#### Using Claude
+If you already have the `ANTHROPIC_API_KEY` set in your system's environment variables then you can skip this step. Otherwise, please set the environment variable before proceeding.
+```python
+import os
+os.environ["ANTHROPIC_API_KEY"] = "put-your-anthropic-api-key-here"
+```
+
 
 #### Setting up the Tonic Validate Scorer
 To use metrics, instantiate an instance of ValidateScorer.
 ```python
 from tonic_validate import ValidateScorer
 scorer = ValidateScorer()
 ```
@@ -315,14 +335,21 @@
 
 scorer = ValidateScorer([
     AnswerConsistencyMetric(),
     AugmentationAccuracyMetric()
 ], model_evaluator="gpt-3.5-turbo")
 ```
 
+You can also pass in other models like Google Gemini or Claude by setting the `model_evaluator` argument to the model name like so
+```python
+scorer = ValidateScorer(model_evaluator="gemini/gemini-1.5-pro-latest")
+```
+```python
+scorer = ValidateScorer(model_evaluator="claude-3")
+```
 If an error occurs while scoring an item's metric, the score for that metric will be set to `None`. If you instead wish to have Tonic Validate throw an exception when there's an error scoring, then set `fail_on_error` to `True` in the constructor
 
 ```python
 scorer = ValidateScorer(fail_on_error=True)
 ```
 
 #### **Important**: Using the scorer on Azure
@@ -457,21 +484,19 @@
 
 
 <!-- FAQ -->
 ## FAQ
 
 #### What models can I use an LLM evaluator?
 
-We currently allow the family of chat completion models from Open AI.
-
-This restriction makes it easy to follow the logic for the definition of the metrics in this package. It also ensures that this package does not depend on langchain, which also makes the logic of the package easier to follow.
+We currently allow the family of chat completion models from Open AI, Google, Anthropic, and more.  We are always looking to add more models to our evaluator.  If you have a model you would like to see added, please file an issue against this repository.
 
 We'd like to add more models as choices for the LLM evaluator without adding to the complexity of the package too much.
 
-The default model used for scoring metrics is GPT 4 Turbo. To change the OpenAI model, pass the OpenAI model name into the `model` argument for `ValidateScorer`
+The default model used for scoring metrics is GPT 4 Turbo. To change the model, pass the model name into the `model` argument for `ValidateScorer`
 
 ```python
 scorer = ValidateScorer([
     AnswerConsistencyMetric(),
     AugmentationAccuracyMetric()
 ], model_evaluator="gpt-3.5-turbo")
 ```
```

### Comparing `tonic_validate-4.0.6/pyproject.toml` & `tonic_validate-5.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [tool.poetry]
 name = "tonic-validate"
-version = "4.0.6"
+version = "5.0.0"
 description = "RAG evaluation metrics."
 authors = ["Joe Ferrara <joeferrara@tonic.ai>", "Ethan Philpott <ephilpott@tonic.ai>", "Adam Kamor <adam@tonic.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0.0"
 openai = ">=1.0.0"
 tiktoken = ">=0.5.2,<0.7.0"
 appdirs = "^1.4.4"
 python-dotenv = "^1.0.1"
 tqdm = "^4.66.2"
 pydantic = "^2.6.4"
 typing-extensions = "^4.10.0"
+litellm = "^1.35.8"
+google-generativeai = { version = "^0.5.2", python = ">=3.9" }
 
 [tool.poetry.group.dev.dependencies]
 sphinx = "^7.0.0"
 sphinx-rtd-theme = ">=1.2,<3.0"
 ruff = ">=0.1.15,<0.4.0"
 tonic-textual = "^1.0.5"
 pytest = "^8.1.1"
```

### Comparing `tonic_validate-4.0.6/tonic_validate/classes/benchmark.py` & `tonic_validate-5.0.0/tonic_validate/classes/benchmark.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.6/tonic_validate/classes/llm_response.py` & `tonic_validate-5.0.0/tonic_validate/classes/llm_response.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.6/tonic_validate/classes/run.py` & `tonic_validate-5.0.0/tonic_validate/classes/run.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.6/tonic_validate/config.py` & `tonic_validate-5.0.0/tonic_validate/config.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.6/tonic_validate/metrics/__init__.py` & `tonic_validate-5.0.0/tonic_validate/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.6/tonic_validate/metrics/answer_consistency_binary_metric.py` & `tonic_validate-5.0.0/tonic_validate/metrics/answer_consistency_binary_metric.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import logging
+from typing import Union
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.binary_metric import BinaryMetric
 from tonic_validate.utils.metrics_util import parse_boolean_response
 from tonic_validate.services.openai_service import OpenAIService
+from tonic_validate.services.litellm_service import LiteLLMService
 from tonic_validate.utils.llm_calls import answer_consistent_with_context_call, context_consistency_prompt
 
 logger = logging.getLogger()
 
 
 class AnswerConsistencyBinaryMetric(BinaryMetric):
     name: str = "answer_consistency_binary"
@@ -16,15 +18,15 @@
         """
         Binary metric that checks whether there is information in the LLM answer that does not come from the context.
         Returns either 1 (consistent) or 0 (inconsistent).
         """
         super().__init__(self.name, self.metric_callback)
 
     async def metric_callback(
-        self, llm_response: LLMResponse, openai_service: OpenAIService
+        self, llm_response: LLMResponse, llm_service: Union[LiteLLMService, OpenAIService]
     ) -> bool:
         """Check if answer is consistent with context.
 
         Parameters
         ----------
         llm_response: LLMResponse
             The response from the LLM system.
@@ -33,10 +35,10 @@
 
         Returns
         -------
         bool
             True if answer is consistent with context, False otherwise.
         """
         hallucination_response = await answer_consistent_with_context_call(
-            llm_response.llm_answer, llm_response.llm_context_list, openai_service
+            llm_response.llm_answer, llm_response.llm_context_list, llm_service
         )
         return parse_boolean_response(hallucination_response)
```

### Comparing `tonic_validate-4.0.6/tonic_validate/metrics/answer_consistency_metric.py` & `tonic_validate-5.0.0/tonic_validate/metrics/answer_consistency_metric.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import logging
+from typing import Union
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.metric import Metric
 from tonic_validate.utils.metrics_util import (
     parse_boolean_response,
     parse_bullet_list_response,
 )
 from tonic_validate.services.openai_service import OpenAIService
+from tonic_validate.services.litellm_service import LiteLLMService
 from tonic_validate.utils.llm_calls import (
     main_points_call,
     statement_derived_from_context_call,
     statement_derived_from_context_prompt,
     main_points_prompt,
 )
 
@@ -30,24 +32,24 @@
         """
         Metric that checks whether the LLM answer contains information that does not come from the context.
         Returns a float between 0 and 1, where 1 is completely consistent and 0 is completely inconsistent.
         """
         pass
 
     async def score(
-        self, llm_response: LLMResponse, openai_service: OpenAIService
+        self, llm_response: LLMResponse, llm_service: Union[LiteLLMService, OpenAIService]
     ) -> float:
         main_points_response = await main_points_call(
-            llm_response.llm_answer, openai_service
+            llm_response.llm_answer, llm_service
         )
         main_point_list = parse_bullet_list_response(main_points_response)
         main_point_derived_from_context_list = []
         for main_point in main_point_list:
             statement_derived_from_context_response = (
                 await statement_derived_from_context_call(
-                    main_point, llm_response.llm_context_list, openai_service
+                    main_point, llm_response.llm_context_list, llm_service
                 )
             )
             main_point_derived_from_context_list.append(
                 parse_boolean_response(statement_derived_from_context_response)
             )
         return sum(main_point_derived_from_context_list) / len(main_point_list)
```

### Comparing `tonic_validate-4.0.6/tonic_validate/metrics/answer_contains_pii_metric.py` & `tonic_validate-5.0.0/tonic_validate/metrics/answer_contains_pii_metric.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import requests
-from typing import List, Optional
+from typing import List, Optional, Union
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.binary_metric import BinaryMetric
 from tonic_validate.services.openai_service import OpenAIService
+from tonic_validate.services.litellm_service import LiteLLMService
 
 
 class AnswerContainsPiiMetric(BinaryMetric):
     def __init__(self, pii_types: List[str], textual_api_key: Optional[str] = None):
         """
         Checks to see if PII is contained in the RAG provided answer.  The types of PII looked for are found in the pii_types list.
 
@@ -36,15 +37,15 @@
             self.textual = TonicTextual("https://textual.tonic.ai")
         else:
             self.textual = TonicTextual("https://textual.tonic.ai", textual_api_key)
 
         super().__init__("answer_contains_pii", self.metric_callback)
 
     def metric_callback(
-        self, llm_response: LLMResponse, openai_service: OpenAIService
+        self, llm_response: LLMResponse, llm_service: Union[LiteLLMService, OpenAIService]
     ) -> bool:
         try:
             response = self.textual.redact(llm_response.llm_answer)
             for d in response.de_identify_results:
                 if d.label.lower() in self.pii_types:
                     return True
             return False
```

### Comparing `tonic_validate-4.0.6/tonic_validate/metrics/answer_match_metric.py` & `tonic_validate-5.0.0/tonic_validate/metrics/answer_match_metric.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import logging
 
+from typing import Union
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.binary_metric import BinaryMetric
 from tonic_validate.services.openai_service import OpenAIService
+from tonic_validate.services.litellm_service import LiteLLMService
 
 logger = logging.getLogger()
 
 
 class AnswerMatchMetric(BinaryMetric):
     def __init__(self, name: str, answer: str, case_sensitive: bool = False):
         """
@@ -23,12 +25,12 @@
             If True, the comparison will be case sensitive
         """
         super().__init__(name, self.metric_callback)
         self.answer = answer
         self.case_sensitive = case_sensitive
 
     def metric_callback(
-        self, llm_response: LLMResponse, openai_service: OpenAIService
+        self, llm_response: LLMResponse, llm_service: Union[LiteLLMService, OpenAIService]
     ) -> bool:
         if self.case_sensitive:
             return self.answer == llm_response.llm_answer
         return self.answer.lower() == llm_response.llm_answer.lower()
```

### Comparing `tonic_validate-4.0.6/tonic_validate/metrics/answer_similarity_metric.py` & `tonic_validate-5.0.0/tonic_validate/metrics/answer_similarity_metric.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import logging
+from typing import Union
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.metric import Metric
 from tonic_validate.services.openai_service import OpenAIService
+from tonic_validate.services.litellm_service import LiteLLMService
 from tonic_validate.utils.llm_calls import similarity_score_call, similarity_score_prompt
 
 logger = logging.getLogger()
 
 
 class AnswerSimilarityMetric(Metric):
     name: str = "answer_similarity"
@@ -15,25 +17,25 @@
         """
         Metric that checks how well the reference answer matches the LLM answer.
         Returns a float between 0 and 5, where 5 is the most similar and 0 is the least similar.
         """
         pass
 
     async def score(
-        self, llm_response: LLMResponse, openai_service: OpenAIService
+        self, llm_response: LLMResponse, llm_service: Union[LiteLLMService, OpenAIService]
     ) -> float:
         # Check that the benchmark item has an answer
         if llm_response.benchmark_item.answer is None:
             raise ValueError("The benchmark item does not have an answer")
 
         similarity_score_response = await similarity_score_call(
             llm_response.benchmark_item.question,
             llm_response.benchmark_item.answer,
             llm_response.llm_answer,
-            openai_service,
+            llm_service,
         )
         try:
             similarity_score = float(similarity_score_response)
         except ValueError:
             raise ValueError(
                 f"Failed to parse similarity score {similarity_score_response} as float"
             )
```

### Comparing `tonic_validate-4.0.6/tonic_validate/metrics/augmentation_accuracy_metric.py` & `tonic_validate-5.0.0/tonic_validate/metrics/retrieval_precision_metric.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 import logging
-from typing import List, Tuple
+from typing import List, Tuple, Union
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.metric import Metric
 from tonic_validate.utils.metrics_util import parse_boolean_response
 from tonic_validate.services.openai_service import OpenAIService
-from tonic_validate.utils.llm_calls import answer_contains_context_call, answer_contains_context_prompt
+from tonic_validate.utils.llm_calls import context_relevancy_call, context_relevancy_prompt
+from tonic_validate.services.litellm_service import LiteLLMService
 
 logger = logging.getLogger()
 
 
-class AugmentationAccuracyMetric(Metric):
-    name: str = "augmentation_accuracy"
-    prompt: str = answer_contains_context_prompt()
+class RetrievalPrecisionMetric(Metric):
+    name: str = "retrieval_precision"
+    prompt: str = context_relevancy_prompt()
 
     def __init__(self):
         """
-        Metric that checks whether the LLM answer includes all of the context.
-        Returns a float between 0 and 1. 1 indicates that the answer contains all of the context. 0 indicates that it contains none of the context.
+        Metric that checks whether the retrieved context is relevant to answer the given question.
+        Returns a float between 0 and 1. 1 indicates that all of the context is relevant. 0 indicates that none of the context is relevant.
         """
         pass
 
     async def score(
-        self, llm_response: LLMResponse, openai_service: OpenAIService
+        self, llm_response: LLMResponse, llm_service: Union[LiteLLMService, OpenAIService]
     ) -> float:
-        return (await self.calculate_metric(llm_response, openai_service))[0]
+        return (await self.calculate_metric(llm_response, llm_service))[0]
 
     async def calculate_metric(
-        self, llm_response: LLMResponse, openai_service: OpenAIService
+        self, llm_response: LLMResponse, llm_service: Union[LiteLLMService, OpenAIService]
     ) -> Tuple[float, List[bool]]:
-        contains_context_list: List[bool] = []
         if len(llm_response.llm_context_list) == 0:
             raise ValueError(
-                "No context provided, cannot calculate augmentation accuracy"
+                "No context provided, cannot calculate retrieval precision"
             )
+        context_relevant_list: List[bool] = []
         for context in llm_response.llm_context_list:
-            contains_context_response = await answer_contains_context_call(
-                llm_response.llm_answer, context, openai_service
-            )
-            contains_context_list.append(
-                parse_boolean_response(contains_context_response)
+            relevance_response = await context_relevancy_call(
+                llm_response.benchmark_item.question, context, llm_service
             )
+            context_relevant_list.append(parse_boolean_response(relevance_response))
 
-        score = sum(contains_context_list) / len(contains_context_list)
-        return (score, contains_context_list)
+        score = sum(context_relevant_list) / len(context_relevant_list)
+        return (score, context_relevant_list)
```

### Comparing `tonic_validate-4.0.6/tonic_validate/metrics/augmentation_precision_metric.py` & `tonic_validate-5.0.0/tonic_validate/metrics/augmentation_precision_metric.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import logging
-from typing import List
+from typing import List, Union
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.augmentation_accuracy_metric import (
     AugmentationAccuracyMetric,
 )
 from tonic_validate.metrics.metric import Metric
 from tonic_validate.metrics.retrieval_precision_metric import RetrievalPrecisionMetric
 from tonic_validate.services.openai_service import OpenAIService
+from tonic_validate.services.litellm_service import LiteLLMService
 
 logger = logging.getLogger()
 
 
 class AugmentationPrecisionMetric(Metric):
     name: str = "augmentation_precision"
 
@@ -19,22 +20,22 @@
         Metric that checks whether the LLM answer contains the relevant context.
         Returns a float between 0 and 1. 1 indicates that the answer contains all of the relevant context. 0 indicates that it contains none of the relevant context.
         """
         self.augmentation_accuracy = AugmentationAccuracyMetric()
         self.retrieval_precision = RetrievalPrecisionMetric()
 
     async def score(
-        self, llm_response: LLMResponse, openai_service: OpenAIService
+        self, llm_response: LLMResponse, llm_service: Union[LiteLLMService, OpenAIService]
     ) -> float:
         retrieval_precision_score = await self.retrieval_precision.calculate_metric(
-            llm_response, openai_service
+            llm_response, llm_service
         )
         context_relevant_list = retrieval_precision_score[1]
         augmentation_accuracy_score = await self.augmentation_accuracy.calculate_metric(
-            llm_response, openai_service
+            llm_response, llm_service
         )
         contains_context_list = augmentation_accuracy_score[1]
 
         return self.score_from_context_labels(
             context_relevant_list, contains_context_list
         )
```

### Comparing `tonic_validate-4.0.6/tonic_validate/metrics/binary_metric.py` & `tonic_validate-5.0.0/tonic_validate/metrics/binary_metric.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import logging
 from typing import Awaitable, Callable, Union
 
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.metric import Metric
 from tonic_validate.services.openai_service import OpenAIService
+from tonic_validate.services.litellm_service import LiteLLMService
 import inspect
 
 logger = logging.getLogger()
 
 
 class BinaryMetric(Metric):
     @property
     def name(self) -> str:
         return self._name
 
     def __init__(
         self,
         name: str,
-        callback: Callable[[LLMResponse, OpenAIService], Union[Awaitable[bool], bool]],
+        callback: Callable[[LLMResponse, Union[LiteLLMService, OpenAIService]], Union[Awaitable[bool], bool]],
     ):
         """
         Create a binary metric with a name and a callback. A binary metric returns either True (1) or False (0).
 
         Parameters
         ----------
         name: str
@@ -31,14 +32,14 @@
             The callback can be either an async function or a regular function.
         """
 
         self._name = name
         self.callback = callback
 
     async def score(
-        self, llm_response: LLMResponse, openai_service: OpenAIService
+        self, llm_response: LLMResponse, llm_service: Union[LiteLLMService, OpenAIService]
     ) -> float:
         if inspect.iscoroutinefunction(self.callback):
-            result = await self.callback(llm_response, openai_service)
+            result = await self.callback(llm_response, llm_service)
         else:
-            result = self.callback(llm_response, openai_service)
+            result = self.callback(llm_response, llm_service)
         return 1.0 if result else 0.0
```

### Comparing `tonic_validate-4.0.6/tonic_validate/metrics/contains_text_metric.py` & `tonic_validate-5.0.0/tonic_validate/metrics/contains_text_metric.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 from typing import List, Optional, Union
 
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.binary_metric import BinaryMetric
 from tonic_validate.services.openai_service import OpenAIService
+from tonic_validate.services.litellm_service import LiteLLMService
 
 logger = logging.getLogger()
 
 
 class ContainsTextMetric(BinaryMetric):
     """Checks whether or not response contains the given text."""
 
@@ -31,15 +32,15 @@
             If True, the comparison will be case sensitive
         """
         super().__init__(name, self.metric_callback)
         self.text = text
         self.case_sensitive = case_sensitive
 
     def metric_callback(
-        self, llm_response: LLMResponse, openai_service: OpenAIService
+        self, llm_response: LLMResponse, llm_service: Union[LiteLLMService, OpenAIService]
     ) -> bool:
         if isinstance(self.text, list):
             return all(self.contains_text(llm_response, text) for text in self.text)
         return self.contains_text(llm_response, self.text)
 
     def contains_text(self, llm_response: LLMResponse, text_to_find: str) -> bool:
         if self.case_sensitive:
```

### Comparing `tonic_validate-4.0.6/tonic_validate/metrics/context_contains_pii_metric.py` & `tonic_validate-5.0.0/tonic_validate/metrics/context_contains_pii_metric.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import requests
-from typing import List, Optional
+from typing import List, Optional, Union
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.binary_metric import BinaryMetric
 from tonic_validate.services.openai_service import OpenAIService
+from tonic_validate.services.litellm_service import LiteLLMService
 
 
 class ContextContainsPiiMetric(BinaryMetric):
     def __init__(self, pii_types: List[str], textual_api_key: Optional[str] = None):
         """
         Checks to see if PII is contained in the RAG provided context.  The types of PII looked for are found in the pii_types list.
 
@@ -36,15 +37,15 @@
             self.textual = TonicTextual("https://textual.tonic.ai")
         else:
             self.textual = TonicTextual("https://textual.tonic.ai", textual_api_key)
 
         super().__init__("context_contains_pii", self.metric_callback)
 
     def metric_callback(
-        self, llm_response: LLMResponse, openai_service: OpenAIService
+        self, llm_response: LLMResponse, llm_service: Union[LiteLLMService, OpenAIService]
     ) -> bool:
         try:
             response = self.textual.redact("\n".join(llm_response.llm_context_list))
             for d in response.de_identify_results:
                 if d.label.lower() in self.pii_types:
                     return True
             return False
```

### Comparing `tonic_validate-4.0.6/tonic_validate/metrics/context_length_metric.py` & `tonic_validate-5.0.0/tonic_validate/metrics/context_length_metric.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
-from typing import Optional
+from typing import Optional, Union
 
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.binary_metric import BinaryMetric
 from tonic_validate.services.openai_service import OpenAIService
+from tonic_validate.services.litellm_service import LiteLLMService
 
 logger = logging.getLogger()
 
 
 class ContextLengthMetric(BinaryMetric):
     """Checks that context length is within a certain range."""
 
@@ -31,15 +32,15 @@
             The maximum length of the context
         """
         super().__init__(name, self.metric_callback)
         self.min_length = min_length
         self.max_length = max_length
 
     def metric_callback(
-        self, llm_response: LLMResponse, openai_service: OpenAIService
+        self, llm_response: LLMResponse, llm_service: Union[LiteLLMService, OpenAIService]
     ) -> bool:
         # For all items in the context list, check if the length is within the min and max length
         return all(
             self.check_context_length(context)
             for context in llm_response.llm_context_list
         )
```

### Comparing `tonic_validate-4.0.6/tonic_validate/metrics/duplication_metric.py` & `tonic_validate-5.0.0/tonic_validate/metrics/duplication_metric.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import logging
 
+from typing import Union
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.binary_metric import BinaryMetric
 from tonic_validate.services.openai_service import OpenAIService
+from tonic_validate.services.litellm_service import LiteLLMService
 from tonic_validate.utils.llm_calls import contains_duplicate_information, contains_duplicate_info_prompt
 from tonic_validate.utils.metrics_util import parse_boolean_response
 
 logger = logging.getLogger()
 
 
 class DuplicationMetric(BinaryMetric):
@@ -17,14 +19,14 @@
         """
         Binary metric that checks whether the response contains duplicate information.
         Returns 1 (True) if the response contains duplicate information. Returns 0 (False) if it does not contain duplicate information.
         """
         super().__init__(self.name, self.metric_callback)
 
     async def metric_callback(
-        self, llm_response: LLMResponse, openai_service: OpenAIService
+        self, llm_response: LLMResponse, llm_service: Union[LiteLLMService, OpenAIService]
     ) -> bool:
         return parse_boolean_response(
             await contains_duplicate_information(
-                llm_response.llm_answer, openai_service
+                llm_response.llm_answer, llm_service
             )
         )
```

### Comparing `tonic_validate-4.0.6/tonic_validate/metrics/hate_speech_content_metric.py` & `tonic_validate-5.0.0/tonic_validate/metrics/hate_speech_content_metric.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import logging
 
+from typing import Union
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.binary_metric import BinaryMetric
 from tonic_validate.services.openai_service import OpenAIService
+from tonic_validate.services.litellm_service import LiteLLMService
 from tonic_validate.utils.llm_calls import contains_hate_speech, contains_hate_speech_prompt
 from tonic_validate.utils.metrics_util import parse_boolean_response
 
 logger = logging.getLogger()
 
 
 class HateSpeechContentMetric(BinaryMetric):
@@ -17,12 +19,12 @@
         """
         Binary metric that checks whether the response contains hate speech.
         Returns 1 (True) if the response contains hate speech. Returns 0 (False) if it does not contain hate speech.
         """
         super().__init__(self.name, self.metric_callback)
 
     async def metric_callback(
-        self, llm_response: LLMResponse, openai_service: OpenAIService
+        self, llm_response: LLMResponse, llm_service: Union[LiteLLMService, OpenAIService]
     ) -> bool:
         return parse_boolean_response(
-            await contains_hate_speech(llm_response.llm_answer, openai_service)
+            await contains_hate_speech(llm_response.llm_answer, llm_service)
         )
```

### Comparing `tonic_validate-4.0.6/tonic_validate/metrics/latency_metric.py` & `tonic_validate-5.0.0/tonic_validate/metrics/latency_metric.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import logging
+from typing import Union
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.binary_metric import BinaryMetric
 from tonic_validate.services.openai_service import OpenAIService
+from tonic_validate.services.litellm_service import LiteLLMService
 
 logger = logging.getLogger()
 
 
 class LatencyMetric(BinaryMetric):
     name: str = "latency_metric"
 
@@ -19,15 +21,15 @@
         target_time: float
             The target time for the model to complete the request in seconds.
         """
         self.target_time = target_time
 
     # We do async here for consistency even though this method doesn't use async
     async def score(
-        self, llm_response: LLMResponse, openai_service: OpenAIService
+        self, llm_response: LLMResponse, llm_service: Union[LiteLLMService, OpenAIService]
     ) -> float:
         # Check that llm_response.run_time is not None
         if llm_response.run_time is None:
             raise ValueError("No run time provided in LLMResponse")
         if llm_response.run_time > self.target_time:
             return 0.0
         return 1.0
```

### Comparing `tonic_validate-4.0.6/tonic_validate/metrics/regex_metric.py` & `tonic_validate-5.0.0/tonic_validate/metrics/regex_metric.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import logging
 import re
 
+from typing import Union
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.binary_metric import BinaryMetric
 from tonic_validate.services.openai_service import OpenAIService
+from tonic_validate.services.litellm_service import LiteLLMService
 
 logger = logging.getLogger()
 
 
 class RegexMetric(BinaryMetric):
     def __init__(self, name: str, pattern: str, match_count: int = 1):
         """
@@ -24,12 +26,12 @@
             The number of matches that should be found in the LLM response
         """
         super().__init__(name, self.metric_callback)
         self.pattern = pattern
         self.match_count = match_count
 
     def metric_callback(
-        self, llm_response: LLMResponse, openai_service: OpenAIService
+        self, llm_response: LLMResponse, llm_service: Union[LiteLLMService, OpenAIService]
     ) -> bool:
         return self.match_count == len(
             re.findall(self.pattern, llm_response.llm_answer)
         )
```

### Comparing `tonic_validate-4.0.6/tonic_validate/metrics/response_length_metric.py` & `tonic_validate-5.0.0/tonic_validate/metrics/response_length_metric.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
-from typing import Optional
+from typing import Optional, Union
 
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.binary_metric import BinaryMetric
 from tonic_validate.services.openai_service import OpenAIService
+from tonic_validate.services.litellm_service import LiteLLMService
 
 logger = logging.getLogger()
 
 
 class ResponseLengthMetric(BinaryMetric):
     def __init__(
         self,
@@ -29,14 +30,14 @@
             The maximum length of the LLM response
         """
         super().__init__(name, self.metric_callback)
         self.min_length = min_length
         self.max_length = max_length
 
     def metric_callback(
-        self, llm_response: LLMResponse, openai_service: OpenAIService
+        self, llm_response: LLMResponse, llm_service: Union[LiteLLMService, OpenAIService]
     ) -> bool:
         if self.min_length and len(llm_response.llm_answer) < self.min_length:
             return False
         if self.max_length and len(llm_response.llm_answer) > self.max_length:
             return False
         return True
```

### Comparing `tonic_validate-4.0.6/tonic_validate/services/openai_service.py` & `tonic_validate-5.0.0/tonic_validate/services/openai_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import os
 import random
 from openai import AsyncAzureOpenAI, BadRequestError, AsyncOpenAI, RateLimitError
 from tiktoken import Encoding
 
 from tonic_validate.classes.exceptions import ContextLengthException, LLMException
-from tonic_validate.utils.openai_cache import OpenAICache
+from tonic_validate.utils.llm_cache import LLMCache
 
 logger = logging.getLogger()
 
 
 class OpenAIService:
     def __init__(
         self,
@@ -51,15 +51,15 @@
                 "OPENAI_API_KEY or AZURE_OPENAI_API_KEY must be set in the environment"
             )
         self.model = model
         self.encoder = encoder
         self.max_retries = max_retries
         self.exp_delay_base = exp_delay_base
         self.starting_wait_time = starting_wait_time
-        self.cache = OpenAICache()
+        self.cache = LLMCache()
 
     async def get_response(self, prompt: str) -> str:
         """
         Retrieves a response from the language model
 
         Parameters
         ----------
```

### Comparing `tonic_validate-4.0.6/tonic_validate/tests/test_scorer.py` & `tonic_validate-5.0.0/tonic_validate/tests/test_scorer.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.6/tonic_validate/utils/http_client.py` & `tonic_validate-5.0.0/tonic_validate/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.6/tonic_validate/utils/llm_calls.py` & `tonic_validate-5.0.0/tonic_validate/utils/llm_calls.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 import logging
-from typing import List
+from typing import List, Union
 from tonic_validate.classes.exceptions import ContextLengthException
 from tonic_validate.services.openai_service import OpenAIService
+from tonic_validate.services.litellm_service import LiteLLMService
 
 logger = logging.getLogger()
 
 
 async def similarity_score_call(
-    question: str, reference_answer: str, llm_answer: str, openai_service: OpenAIService
+    question: str, reference_answer: str, llm_answer: str, llm_service: Union[LiteLLMService, OpenAIService]
 ) -> str:
     """Sends prompt for answer similarity score to OpenAI API, and returns response.
 
     Parameters
     ----------
     question: str
         The question that was asked.
     reference_answer: str
         The answer that was expected.
     llm_answer: str
         The answer that was generated by the RAG system.
-    openai_service: OpenAIService
+    llm_service: Union[LiteLLMService, OpenAIService]
         The OpenAI Service which allows for communication with the OpenAI API.
 
     Returns
     -------
     str
         Response from OpenAI API.
     """
     logger.debug(
-        f"Asking {openai_service.model} for similarity score for question: {question}"
+        f"Asking {llm_service.model} for similarity score for question: {question}"
     )
     main_message = similarity_score_prompt()
     main_message += f"\nQUESTION: {question}\n"
     main_message += f"REFERENCE ANSWER: {reference_answer}\n"
     main_message += f"NEW ANSWER: {llm_answer}\n"
 
     try:
-        response_message = await openai_service.get_response(main_message)
+        response_message = await llm_service.get_response(main_message)
     except ContextLengthException as e:
-        question_tokens = openai_service.get_token_count(question)
-        reference_answer_tokens = openai_service.get_token_count(reference_answer)
-        llm_answer_tokens = openai_service.get_token_count(llm_answer)
-        total_tokens = openai_service.get_token_count(main_message)
+        question_tokens = llm_service.get_token_count(question)
+        reference_answer_tokens = llm_service.get_token_count(reference_answer)
+        llm_answer_tokens = llm_service.get_token_count(llm_answer)
+        total_tokens = llm_service.get_token_count(main_message)
         base_prompt_tokens = (
             total_tokens - question_tokens - reference_answer_tokens - llm_answer_tokens
         )
         raise ContextLengthException(
             "Similarity score prompt too long to score item. OpenAI returned the "
             "following error message"
             "\n----------"
@@ -76,47 +77,47 @@
         "similar, how similar in meaning is the new answer to the reference answer? "
         "Respond with just a number and no additional text."
     )
     return main_message
 
 
 async def answer_consistent_with_context_call(
-    answer: str, context_list: List[str], openai_service: OpenAIService
+    answer: str, context_list: List[str], llm_service: Union[LiteLLMService, OpenAIService]
 ) -> str:
     """Sends prompt for answer consistency binary score and returns response.
 
     Parameters
     ----------
     answer: str
         The answer that was generated by the RAG system.
     context_list: List[str]
         Retrieved context used by the RAG system to make answer.
-    openai_service: OpenAIService
+    llm_service: Union[LiteLLMService, OpenAIService]
         The OpenAI Service which allows for communication with the OpenAI API.
 
     Returns
     -------
     str
         Response from OpenAI API.
     """
 
-    logger.debug(f"Asking {openai_service.model} whether answer hallucinates")
+    logger.debug(f"Asking {llm_service.model} whether answer hallucinates")
     main_message = context_consistency_prompt()
     for i, context in enumerate(context_list):
         main_message += f"\n\nCONTEXT {i}:\n{context}\nEND OF CONTEXT {i}"
     main_message += f"\n\nANSWER: {answer}"
 
     try:
-        response_message = await openai_service.get_response(main_message)
+        response_message = await llm_service.get_response(main_message)
     except ContextLengthException as e:
-        answer_tokens = openai_service.get_token_count(answer)
+        answer_tokens = llm_service.get_token_count(answer)
         context_tokens = 0
         for context in context_list:
-            context_tokens += openai_service.get_token_count(context)
-        total_tokens = openai_service.get_token_count(main_message)
+            context_tokens += llm_service.get_token_count(context)
+        total_tokens = llm_service.get_token_count(main_message)
         base_prompt_tokens = total_tokens - context_tokens - answer_tokens
         raise ContextLengthException(
             "Consistency prompt too long to score item. OpenAI returned the following "
             "error message"
             "\n----------"
             f"\n{e}"
             "\n----------"
@@ -146,45 +147,45 @@
         "context then respond with false. Otherwise respond with true. Respond with "
         "either true or false and no additional text."
     )
     return main_message
 
 
 async def context_relevancy_call(
-    question: str, context: str, openai_service: OpenAIService
+    question: str, context: str, llm_service: Union[LiteLLMService, OpenAIService]
 ) -> str:
     """Sends prompt to get context relevance to Open AI API and returns response.
 
     Parameters
     ----------
     question: str
         The question that was asked.
     context: str
         One piece of context retrieved by RAG system.
-    openai_service: OpenAIService
+    llm_service: Union[LiteLLMService, OpenAIService]
         The OpenAI Service which allows for communication with the OpenAI API.
 
     Returns
     -------
     str
         Response from OpenAI API.
     """
     logger.debug(
-        f"Asking {openai_service.model} for context relevance for question {question}"
+        f"Asking {llm_service.model} for context relevance for question {question}"
     )
     main_message = context_relevancy_prompt()
     main_message += f"\nQUESTION: {question}\n"
     main_message += f"CONTEXT: {context}\n"
 
     try:
-        response_message = await openai_service.get_response(main_message)
+        response_message = await llm_service.get_response(main_message)
     except ContextLengthException as e:
-        question_tokens = openai_service.get_token_count(question)
-        context_tokens = openai_service.get_token_count(context)
-        total_tokens = openai_service.get_token_count(main_message)
+        question_tokens = llm_service.get_token_count(question)
+        context_tokens = llm_service.get_token_count(context)
+        total_tokens = llm_service.get_token_count(main_message)
         base_prompt_tokens = total_tokens - question_tokens - context_tokens
         raise ContextLengthException(
             "Relevance prompt too long to score item. OpenAI returned the following "
             "error message"
             "\n----------"
             f"\n{e}"
             "\n----------"
@@ -213,43 +214,43 @@
         "answering the question, respond with false. Respond with either true or false "
         "and no additional text."
     )
     return main_message
 
 
 async def answer_contains_context_call(
-    answer: str, context: str, openai_service: OpenAIService
+    answer: str, context: str, llm_service: Union[LiteLLMService, OpenAIService]
 ) -> str:
     """Sends prompt for whether answer contains context and returns response.
 
     Parameters
     ----------
     answer: str
         The answer that was generated by the RAG system.
     context: str
         One piece of context retrieved by RAG system.
-    openai_service: OpenAIService
+    llm_service: Union[LiteLLMService, OpenAIService]
         The OpenAI Service which allows for communication with the OpenAI API.
 
     Returns
     -------
     str
         Response from OpenAI API.
     """
-    logger.debug(f"Asking {openai_service.model} whether answer contains context")
+    logger.debug(f"Asking {llm_service.model} whether answer contains context")
     main_message = answer_contains_context_prompt()
     main_message += f"\nANSWER: {answer}\n"
     main_message += f"CONTEXT: {context}\n"
 
     try:
-        response_message = await openai_service.get_response(main_message)
+        response_message = await llm_service.get_response(main_message)
     except ContextLengthException as e:
-        answer_tokens = openai_service.get_token_count(answer)
-        context_tokens = openai_service.get_token_count(context)
-        total_tokens = openai_service.get_token_count(main_message)
+        answer_tokens = llm_service.get_token_count(answer)
+        context_tokens = llm_service.get_token_count(context)
+        total_tokens = llm_service.get_token_count(main_message)
         base_prompt_tokens = total_tokens - answer_tokens - context_tokens
         raise ContextLengthException(
             "Contains context prompt too long to score item. OpenAI returned the "
             "following error message"
             "\n----------"
             f"\n{e}"
             "\n----------"
@@ -276,40 +277,40 @@
         "information derived from the context, respond with true. If the answer does "
         "not contain information derived from the context, respond with false. "
         "Respond with either true or false and no additional text."
     )
     return main_message
 
 
-async def main_points_call(answer: str, openai_service: OpenAIService) -> str:
+async def main_points_call(answer: str, llm_service: Union[LiteLLMService, OpenAIService]) -> str:
     """Sends prompt for main points in answer to Open AI API and returns response.
 
     Parameters
     ----------
     answer: str
         The answer that was generated by the RAG system.
-    openai_service: OpenAIService
+    llm_service: Union[LiteLLMService, OpenAIService]
         The OpenAI Service which allows for communication with the OpenAI API.
 
     Returns
     -------
     str
         Response from OpenAI API.
     """
     logger.debug(
-        f"Asking {openai_service.model} for bullet list of main points in answer"
+        f"Asking {llm_service.model} for bullet list of main points in answer"
     )
     main_message = main_points_prompt()
     main_message += f"\nANSWER: {answer}"
 
     try:
-        response_message = await openai_service.get_response(main_message)
+        response_message = await llm_service.get_response(main_message)
     except ContextLengthException as e:
-        answer_tokens = openai_service.get_token_count(answer)
-        total_tokens = openai_service.get_token_count(main_message)
+        answer_tokens = llm_service.get_token_count(answer)
+        total_tokens = llm_service.get_token_count(main_message)
         base_prompt_tokens = total_tokens - answer_tokens
         raise ContextLengthException(
             "Main points prompt too long to score item. OpenAI returned the following "
             "error message"
             "\n----------"
             f"\n{e}"
             "\n----------"
@@ -335,46 +336,46 @@
         "bulleted list and no additional text. Only use a single '*' for each bullet "
         "and do not use a '*' anywhere in your response except for the bullets."
     )
     return main_message
 
 
 async def statement_derived_from_context_call(
-    statement: str, context_list: List[str], openai_service: OpenAIService
+    statement: str, context_list: List[str], llm_service: Union[LiteLLMService, OpenAIService]
 ) -> str:
     """Sends prompt for whether statement is derived from context and returns response.
 
     Parameters
     ----------
     statement: str
         The statement to be checked.
     context_list: List[str]
         List of retrieved context to see if statement is derived from this context.
-    openai_service: OpenAIService
+    llm_service: Union[LiteLLMService, OpenAIService]
         The OpenAI Service which allows for communication with the OpenAI API.
 
     Returns
     -------
     str
         Response from OpenAI API.
     """
     logger.debug(
-        f"Asking {openai_service.model} whether statement is derived from context"
+        f"Asking {llm_service.model} whether statement is derived from context"
     )
 
     main_message = statement_derived_from_context_prompt(statement, context_list)
 
     try:
-        response_message = await openai_service.get_response(main_message)
+        response_message = await llm_service.get_response(main_message)
     except ContextLengthException as e:
-        statement_tokens = openai_service.get_token_count(statement)
+        statement_tokens = llm_service.get_token_count(statement)
         context_tokens = 0
         for context in context_list:
-            context_tokens += openai_service.get_token_count(context)
-        total_tokens = openai_service.get_token_count(main_message)
+            context_tokens += llm_service.get_token_count(context)
+        total_tokens = llm_service.get_token_count(main_message)
         base_prompt_tokens = total_tokens - context_tokens - statement_tokens
         raise ContextLengthException(
             "Derived from context prompt too long to score item. OpenAI returned the "
             "following error message"
             "\n----------"
             f"\n{e}"
             "\n----------"
@@ -417,41 +418,41 @@
         "respond with 'false'. Your response must be either 'true' or 'false' with no "
         "additional text."
     )
     return main_message
 
 
 async def contains_duplicate_information(
-    statement: str, openai_service: OpenAIService
+    statement: str, llm_service: Union[LiteLLMService, OpenAIService]
 ) -> str:
     """Sends prompt for whether statement contains duplicate information and returns response.
 
     Parameters
     ----------
     statement: str
         The statement to be checked.
-    openai_service: OpenAIService
+    llm_service: Union[LiteLLMService, OpenAIService]
         The OpenAI Service which allows for communication with the OpenAI API.
 
     Returns
     -------
     str
         Response from OpenAI API.
     """
     logger.debug(
-        f"Asking {openai_service.model} whether statement contains duplicate information"
+        f"Asking {llm_service.model} whether statement contains duplicate information"
     )
     main_message = contains_duplicate_info_prompt()
     main_message += f"\n\nSTATEMENT:\n{statement}\nEND OF STATEMENT"
 
     try:
-        response_message = await openai_service.get_response(main_message)
+        response_message = await llm_service.get_response(main_message)
     except ContextLengthException as e:
-        statement_tokens = openai_service.get_token_count(statement)
-        total_tokens = openai_service.get_token_count(main_message)
+        statement_tokens = llm_service.get_token_count(statement)
+        total_tokens = llm_service.get_token_count(main_message)
         base_prompt_tokens = total_tokens - statement_tokens
         raise ContextLengthException(
             "Duplicate information prompt too long to score item. OpenAI returned the following error message"
             "\n----------"
             f"\n{e}"
             "\n----------"
             "\nSee details below for breakdown of token counts"
@@ -475,40 +476,40 @@
         "duplicate information. If the statement contains duplicate information, respond "
         "with 'true'. If the statement does not contain duplicate information, respond "
         "with 'false'. Respond with either 'true' or 'false' and no additional text."
     )
     return main_message
 
 
-async def contains_hate_speech(statement: str, openai_service: OpenAIService) -> str:
+async def contains_hate_speech(statement: str, llm_service: Union[LiteLLMService, OpenAIService]) -> str:
     """Sends prompt for whether statement contains hate speech and returns response.
 
     Parameters
     ----------
     statement: str
         The statement to be checked.
-    openai_service: OpenAIService
+    llm_service: Union[LiteLLMService, OpenAIService]
         The OpenAI Service which allows for communication with the OpenAI API.
 
     Returns
     -------
     str
         Response from OpenAI API.
     """
     logger.debug(
-        f"Asking {openai_service.model} whether statement contains hate speech"
+        f"Asking {llm_service.model} whether statement contains hate speech"
     )
     main_message = contains_hate_speech_prompt()
     main_message += f"\n\nSTATEMENT:\n{statement}\nEND OF STATEMENT"
 
     try:
-        response_message = await openai_service.get_response(main_message)
+        response_message = await llm_service.get_response(main_message)
     except ContextLengthException as e:
-        statement_tokens = openai_service.get_token_count(statement)
-        total_tokens = openai_service.get_token_count(main_message)
+        statement_tokens = llm_service.get_token_count(statement)
+        total_tokens = llm_service.get_token_count(main_message)
         base_prompt_tokens = total_tokens - statement_tokens
         raise ContextLengthException(
             "Hate speech prompt too long to score item. OpenAI returned the following error message"
             "\n----------"
             f"\n{e}"
             "\n----------"
             "\nSee details below for breakdown of token counts"
```

### Comparing `tonic_validate-4.0.6/tonic_validate/utils/metrics_util.py` & `tonic_validate-5.0.0/tonic_validate/utils/metrics_util.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.6/tonic_validate/utils/openai_cache.py` & `tonic_validate-5.0.0/tonic_validate/utils/llm_cache.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections import OrderedDict
 
 
-class OpenAICache:
+class LLMCache:
     def __init__(self, maxsize=512):
         self.maxsize = maxsize
         self.cache = OrderedDict()
 
     def get(self, key):
         if key in self.cache:
             self.cache.move_to_end(key)
```

### Comparing `tonic_validate-4.0.6/tonic_validate/utils/telemetry.py` & `tonic_validate-5.0.0/tonic_validate/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.6/tonic_validate/validate_api.py` & `tonic_validate-5.0.0/tonic_validate/validate_api.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.6/tonic_validate/validate_scorer.py` & `tonic_validate-5.0.0/tonic_validate/validate_scorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from tonic_validate.metrics.answer_similarity_metric import AnswerSimilarityMetric
 from tonic_validate.metrics.augmentation_precision_metric import (
     AugmentationPrecisionMetric,
 )
 
 from tonic_validate.metrics.metric import Metric
 from tonic_validate.services.openai_service import OpenAIService
+from tonic_validate.services.litellm_service import LiteLLMService
 import tiktoken
 from tonic_validate.utils.telemetry import Telemetry
 from tqdm.asyncio import tqdm as async_tqdm
 from tqdm import tqdm
 import time
 
 logger = logging.getLogger()
@@ -44,15 +45,15 @@
         model_evaluator: str = "gpt-4-turbo-preview",
         max_parsing_retries: int = 3,
         max_llm_retries: int = 10,
         fail_on_error: bool = False,
         quiet: bool = False,
     ):
         """
-        Create a Tonic Validate scorer.
+        Create a Tonic Validate scorer that can work with either OpenAIService or LiteLLMService.
 
         Parameters
         ----------
         metrics: List[Metric]
             The list of metrics to be used for scoring.
         model_evaluator: str
             The model to be used for scoring.
@@ -66,25 +67,35 @@
             If True, will suppress all logging except errors.
         """
         self.metrics = metrics
         self.model_evaluator = model_evaluator
         self.max_parsing_retries = max_parsing_retries
         self.max_llm_retries = max_llm_retries
         self.fail_on_error = fail_on_error
-        logger.setLevel(logging.ERROR if quiet else logging.INFO)
         self.quiet = quiet
         self.telemetry = Telemetry()
+        logger.setLevel(logging.ERROR if quiet else logging.INFO)
+
         try:
             self.encoder = tiktoken.encoding_for_model(model_evaluator)
         except Exception as _:
             logger.info("Defaulting to cl100k_base for measuring token count")
             self.encoder = tiktoken.get_encoding("cl100k_base")
-        self.openai_service = OpenAIService(
-            self.encoder, self.model_evaluator, max_retries=self.max_llm_retries
-        )
+
+        model_name_lower = self.model_evaluator.lower()
+        if model_name_lower.startswith("gemini/") or model_name_lower.startswith(
+            "claude"
+        ):
+            self.llm_service = LiteLLMService(
+                self.encoder, self.model_evaluator, max_retries=self.max_llm_retries
+            )
+        else:
+            self.llm_service = OpenAIService(
+                self.encoder, self.model_evaluator, max_retries=self.max_llm_retries
+            )
 
     @validate_call(config=ConfigDict(arbitrary_types_allowed=True))
     async def _score_item_rundata(
         self, response: LLMResponse, semaphore: Semaphore
     ) -> RunData:
         """
         Calculates scores for a single LLMResponse object
@@ -103,15 +114,15 @@
             scores: Dict[str, Union[float, None]] = {}
             for metric in self.metrics:
                 tries = 0
                 exceptions = []
                 while tries < self.max_parsing_retries:
                     try:
                         scores[metric.name] = await metric.score(
-                            response, self.openai_service
+                            response, self.llm_service
                         )
                         break
                     except LLMException as e:
                         if self.fail_on_error:
                             raise Exception("Error getting LLM response: " + str(e))
                         scores[metric.name] = None
                         logger.warning(
@@ -164,15 +175,15 @@
         Run
             The Run object containing the scores and other data.
         """
         try:
             start_time = time.time()
         except Exception as _:
             start_time = -1
-        
+
         semaphore = Semaphore(parallelism)
         tasks = [
             self._score_item_rundata(response, semaphore) for response in responses
         ]
 
         run_data: List[RunData] = await async_tqdm.gather(
             *tasks,
```

### Comparing `tonic_validate-4.0.6/PKG-INFO` & `tonic_validate-5.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: tonic-validate
-Version: 4.0.6
+Version: 5.0.0
 Summary: RAG evaluation metrics.
 Author: Joe Ferrara
 Author-email: joeferrara@tonic.ai
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
+Requires-Dist: google-generativeai (>=0.5.2,<0.6.0) ; python_version >= "3.9"
+Requires-Dist: litellm (>=1.35.8,<2.0.0)
 Requires-Dist: openai (>=1.0.0)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: tiktoken (>=0.5.2,<0.7.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: typing-extensions (>=4.10.0,<5.0.0)
 Description-Content-Type: text/markdown
@@ -58,14 +60,16 @@
 <h3 align="center">Tonic Validate</h3>
 
   <p align="center">
     A high performance LLM/RAG evaluation framework
     <br />
     <a href="https://docs.tonic.ai/validate"><strong>Explore the docs »</strong></a>
     <br />
+    <a href="https://www.tonic.ai/textual"><strong>Prepare your unstructured data for RAG »</strong></a>
+    <br />
     <br />
     <a href="https://github.com/TonicAI/tonic_validate/issues">Report Bug</a>
     ·
     <a href="https://github.com/TonicAI/tonic_validate/issues">Request Feature</a>
     ·
     <a href="#quick-start">Quick Start</a>
   </p>
@@ -103,16 +107,19 @@
 
 
 <!-- ABOUT THE PROJECT -->
 ## About The Project
 
 Tonic Validate is a framework for the evaluation of LLM outputs, such as Retrieval Augmented Generation (RAG) pipelines. Validate makes it easy to evaluate, track, and monitor your LLM and RAG applications. Validate allows you to evaluate your LLM outputs through the use of our provided metrics which measure everything from answer correctness to LLM hallucination. Additionally, Validate has an optional UI to visualize your evaluation results for easy tracking and monitoring.
 
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
+> **Good RAG systems start with good inputs. Are you blocked on pre-processing messy, complex unstructured data into a standardized format for embedding and ingestion into your vector database?** 
+>
+>Tonic Textual is a privacy-focused ETL for LLMs that standardizes unstructured data for AI development and uses proprietary NER models to create metadata tags that enable improved retreival performance via metadata filtering. If you're spending too much time on data preparation, we can help; reach out to us for a [demo](https://www.tonic.ai/product-demo/textual).
 
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- Quick Start -->
 ## Quick Start
 
 This is an example of how you may give instructions on setting up your project locally.
 To get a local copy up and running follow these simple example steps.
@@ -316,14 +323,29 @@
 If you are using Azure, instead of setting the `OPENAI_API_KEY` environment variable, you instead need to set `AZURE_OPENAI_KEY` and `AZURE_OPENAI_ENDPOINT`. `AZURE_OPENAI_ENDPOINT` is the endpoint url for your Azure OpenAI deployment and `AZURE_OPENAI_KEY` is your API key.
 ```python
 import os
 os.environ["AZURE_OPENAI_KEY"] = "put-your-azure-openai-api-key-here"
 os.environ["AZURE_OPENAI_ENDPOINT"] = "put-your-azure-endpoint-here"
 ```
 
+#### Using Gemini
+If you already have the `GEMINI_API_KEY` set in your system's environment variables then you can skip this step. Otherwise, please set the environment variable before proceeding.
+```python
+import os
+os.environ["GEMINI_API_KEY"] = "put-your-gemini-api-key-here"
+```
+_Note that to use gemini, your Python version must be 3.9 or higher._
+
+#### Using Claude
+If you already have the `ANTHROPIC_API_KEY` set in your system's environment variables then you can skip this step. Otherwise, please set the environment variable before proceeding.
+```python
+import os
+os.environ["ANTHROPIC_API_KEY"] = "put-your-anthropic-api-key-here"
+```
+
 
 #### Setting up the Tonic Validate Scorer
 To use metrics, instantiate an instance of ValidateScorer.
 ```python
 from tonic_validate import ValidateScorer
 scorer = ValidateScorer()
 ```
@@ -336,14 +358,21 @@
 
 scorer = ValidateScorer([
     AnswerConsistencyMetric(),
     AugmentationAccuracyMetric()
 ], model_evaluator="gpt-3.5-turbo")
 ```
 
+You can also pass in other models like Google Gemini or Claude by setting the `model_evaluator` argument to the model name like so
+```python
+scorer = ValidateScorer(model_evaluator="gemini/gemini-1.5-pro-latest")
+```
+```python
+scorer = ValidateScorer(model_evaluator="claude-3")
+```
 If an error occurs while scoring an item's metric, the score for that metric will be set to `None`. If you instead wish to have Tonic Validate throw an exception when there's an error scoring, then set `fail_on_error` to `True` in the constructor
 
 ```python
 scorer = ValidateScorer(fail_on_error=True)
 ```
 
 #### **Important**: Using the scorer on Azure
@@ -478,21 +507,19 @@
 
 
 <!-- FAQ -->
 ## FAQ
 
 #### What models can I use an LLM evaluator?
 
-We currently allow the family of chat completion models from Open AI.
-
-This restriction makes it easy to follow the logic for the definition of the metrics in this package. It also ensures that this package does not depend on langchain, which also makes the logic of the package easier to follow.
+We currently allow the family of chat completion models from Open AI, Google, Anthropic, and more.  We are always looking to add more models to our evaluator.  If you have a model you would like to see added, please file an issue against this repository.
 
 We'd like to add more models as choices for the LLM evaluator without adding to the complexity of the package too much.
 
-The default model used for scoring metrics is GPT 4 Turbo. To change the OpenAI model, pass the OpenAI model name into the `model` argument for `ValidateScorer`
+The default model used for scoring metrics is GPT 4 Turbo. To change the model, pass the model name into the `model` argument for `ValidateScorer`
 
 ```python
 scorer = ValidateScorer([
     AnswerConsistencyMetric(),
     AugmentationAccuracyMetric()
 ], model_evaluator="gpt-3.5-turbo")
 ```
```

