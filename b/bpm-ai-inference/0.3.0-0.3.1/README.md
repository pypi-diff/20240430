# Comparing `tmp/bpm_ai_inference-0.3.0.tar.gz` & `tmp/bpm_ai_inference-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpm_ai_inference-0.3.0.tar", max compression
+gzip compressed data, was "bpm_ai_inference-0.3.1.tar", max compression
```

## Comparing `bpm_ai_inference-0.3.0.tar` & `bpm_ai_inference-0.3.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    35128 2024-04-29 08:28:08.741572 bpm_ai_inference-0.3.0/LICENSE
--rw-r--r--   0        0        0      743 2024-04-29 08:28:08.741572 bpm_ai_inference-0.3.0/README.md
--rw-r--r--   0        0        0        0 2024-04-29 08:28:08.741572 bpm_ai_inference-0.3.0/bpm_ai_inference/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 08:28:08.741572 bpm_ai_inference-0.3.0/bpm_ai_inference/classification/__init__.py
--rw-r--r--   0        0        0     2852 2024-04-29 08:28:08.741572 bpm_ai_inference-0.3.0/bpm_ai_inference/classification/transformers_text_classifier.py
--rw-r--r--   0        0        0     1740 2024-04-29 08:28:08.741572 bpm_ai_inference-0.3.0/bpm_ai_inference/daemon.py
--rw-r--r--   0        0        0        0 2024-04-29 08:28:08.741572 bpm_ai_inference-0.3.0/bpm_ai_inference/image_classification/__init__.py
--rw-r--r--   0        0        0     2547 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/image_classification/transformers_image_classifier.py
--rw-r--r--   0        0        0        0 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/llm/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/llm/llama_cpp/__init__.py
--rw-r--r--   0        0        0      219 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/llm/llama_cpp/_constants.py
--rw-r--r--   0        0        0     8123 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/llm/llama_cpp/llama_chat.py
--rw-r--r--   0        0        0      199 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/llm/llama_cpp/output_schema.prompt
--rw-r--r--   0        0        0      981 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/llm/llama_cpp/tool_use.prompt
--rw-r--r--   0        0        0     1082 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/llm/llama_cpp/util.py
--rw-r--r--   0        0        0        0 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/ocr/__init__.py
--rw-r--r--   0        0        0     3256 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/ocr/tesseract.py
--rw-r--r--   0        0        0        0 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/pos/__init__.py
--rw-r--r--   0        0        0     1833 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/pos/spacy_pos_tagger.py
--rw-r--r--   0        0        0        0 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/question_answering/__init__.py
--rw-r--r--   0        0        0     2154 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/question_answering/pix2struct_vqa.py
--rw-r--r--   0        0        0     2056 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/question_answering/transformers_docvqa.py
--rw-r--r--   0        0        0     1940 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/question_answering/transformers_qa.py
--rw-r--r--   0        0        0        0 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/speech_recognition/__init__.py
--rw-r--r--   0        0        0     1219 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/speech_recognition/faster_whisper.py
--rw-r--r--   0        0        0        0 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/token_classification/__init__.py
--rw-r--r--   0        0        0     1402 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/token_classification/gliner_token_classifier.py
--rw-r--r--   0        0        0     3178 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/token_classification/transformers_token_classifier.py
--rw-r--r--   0        0        0        0 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/translation/__init__.py
--rw-r--r--   0        0        0        2 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/translation/easy_nmt/__init__.py
--rw-r--r--   0        0        0    18731 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/translation/easy_nmt/easy_nmt.py
--rw-r--r--   0        0        0     2423 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/translation/easy_nmt/opus_mt.py
--rw-r--r--   0        0        0     1784 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/translation/easy_nmt/util.py
--rw-r--r--   0        0        0       36 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/util/__init__.py
--rw-r--r--   0        0        0      483 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/util/files.py
--rw-r--r--   0        0        0      122 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/util/hf.py
--rw-r--r--   0        0        0      828 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/util/language.py
--rw-r--r--   0        0        0     7153 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/util/optimum.py
--rw-r--r--   0        0        0     1014 2024-04-29 08:28:08.749572 bpm_ai_inference-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 bpm_ai_inference-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35128 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/LICENSE
+-rw-r--r--   0        0        0      743 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/classification/__init__.py
+-rw-r--r--   0        0        0     2852 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/classification/transformers_text_classifier.py
+-rw-r--r--   0        0        0     1740 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/daemon.py
+-rw-r--r--   0        0        0        0 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/image_classification/__init__.py
+-rw-r--r--   0        0        0     2547 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/image_classification/transformers_image_classifier.py
+-rw-r--r--   0        0        0        0 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/llm/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/llm/llama_cpp/__init__.py
+-rw-r--r--   0        0        0      222 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/llm/llama_cpp/_constants.py
+-rw-r--r--   0        0        0     8197 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/llm/llama_cpp/llama_chat.py
+-rw-r--r--   0        0        0      199 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/llm/llama_cpp/output_schema.prompt
+-rw-r--r--   0        0        0      981 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/llm/llama_cpp/tool_use.prompt
+-rw-r--r--   0        0        0     1725 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/llm/llama_cpp/util.py
+-rw-r--r--   0        0        0        0 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/ocr/__init__.py
+-rw-r--r--   0        0        0     3256 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/ocr/tesseract.py
+-rw-r--r--   0        0        0        0 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/pos/__init__.py
+-rw-r--r--   0        0        0     1833 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/pos/spacy_pos_tagger.py
+-rw-r--r--   0        0        0        0 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/question_answering/__init__.py
+-rw-r--r--   0        0        0     2154 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/question_answering/pix2struct_vqa.py
+-rw-r--r--   0        0        0     2056 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/question_answering/transformers_docvqa.py
+-rw-r--r--   0        0        0     1940 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/question_answering/transformers_qa.py
+-rw-r--r--   0        0        0        0 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/speech_recognition/__init__.py
+-rw-r--r--   0        0        0     1219 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/speech_recognition/faster_whisper.py
+-rw-r--r--   0        0        0        0 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/token_classification/__init__.py
+-rw-r--r--   0        0        0     1402 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/token_classification/gliner_token_classifier.py
+-rw-r--r--   0        0        0     3178 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/token_classification/transformers_token_classifier.py
+-rw-r--r--   0        0        0        0 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/translation/__init__.py
+-rw-r--r--   0        0        0        2 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/translation/easy_nmt/__init__.py
+-rw-r--r--   0        0        0    18731 2024-04-29 14:05:03.509647 bpm_ai_inference-0.3.1/bpm_ai_inference/translation/easy_nmt/easy_nmt.py
+-rw-r--r--   0        0        0     2423 2024-04-29 14:05:03.509647 bpm_ai_inference-0.3.1/bpm_ai_inference/translation/easy_nmt/opus_mt.py
+-rw-r--r--   0        0        0     1784 2024-04-29 14:05:03.509647 bpm_ai_inference-0.3.1/bpm_ai_inference/translation/easy_nmt/util.py
+-rw-r--r--   0        0        0       36 2024-04-29 14:05:03.509647 bpm_ai_inference-0.3.1/bpm_ai_inference/util/__init__.py
+-rw-r--r--   0        0        0      483 2024-04-29 14:05:03.509647 bpm_ai_inference-0.3.1/bpm_ai_inference/util/files.py
+-rw-r--r--   0        0        0      122 2024-04-29 14:05:03.509647 bpm_ai_inference-0.3.1/bpm_ai_inference/util/hf.py
+-rw-r--r--   0        0        0      828 2024-04-29 14:05:03.509647 bpm_ai_inference-0.3.1/bpm_ai_inference/util/language.py
+-rw-r--r--   0        0        0     7153 2024-04-29 14:05:03.509647 bpm_ai_inference-0.3.1/bpm_ai_inference/util/optimum.py
+-rw-r--r--   0        0        0     1014 2024-04-29 14:05:03.509647 bpm_ai_inference-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 bpm_ai_inference-0.3.1/PKG-INFO
```

### Comparing `bpm_ai_inference-0.3.0/LICENSE` & `bpm_ai_inference-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.0/README.md` & `bpm_ai_inference-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.0/bpm_ai_inference/classification/transformers_text_classifier.py` & `bpm_ai_inference-0.3.1/bpm_ai_inference/classification/transformers_text_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.0/bpm_ai_inference/daemon.py` & `bpm_ai_inference-0.3.1/bpm_ai_inference/daemon.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.0/bpm_ai_inference/image_classification/transformers_image_classifier.py` & `bpm_ai_inference-0.3.1/bpm_ai_inference/image_classification/transformers_image_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.0/bpm_ai_inference/llm/llama_cpp/llama_chat.py` & `bpm_ai_inference-0.3.1/bpm_ai_inference/llm/llama_cpp/llama_chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
             model_file = find_file(hf_home() + "hub/models--" + model.replace("/", "--"), filename)
             self.llm = Llama(
                 model_path=model_file,
                 n_ctx=n_ctx,
                 verbose=False
             )
         else:
+            logger.info(f"Loading model file {filename} from {model}...")
             self.llm = Llama.from_pretrained(
                 repo_id=model,
                 filename=filename,
                 n_ctx=n_ctx,
                 verbose=False
             )
```

### Comparing `bpm_ai_inference-0.3.0/bpm_ai_inference/llm/llama_cpp/tool_use.prompt` & `bpm_ai_inference-0.3.1/bpm_ai_inference/llm/llama_cpp/tool_use.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.0/bpm_ai_inference/llm/llama_cpp/util.py` & `bpm_ai_inference-0.3.1/bpm_ai_inference/llm/llama_cpp/util.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import logging
 
+from bpm_ai_core.llm.common.blob import Blob
 from bpm_ai_core.llm.common.message import ChatMessage, AssistantMessage, ToolResultMessage
 
 logger = logging.getLogger(__name__)
 
 
 async def messages_to_llama_dicts(messages: list[ChatMessage]):
     return [await message_to_llama_dict(m) for m in messages]
@@ -14,14 +15,28 @@
     if isinstance(message, AssistantMessage) and message.has_tool_calls():
         tool_call = message.tool_calls[0]
         tool_content = json.dumps(tool_call.payload_dict())
         content = '<tool_call>\n{"name": "' + tool_call.name + '", "arguments": ' + tool_content + '}\n</tool_call>'
     elif isinstance(message, ToolResultMessage):
         tool_response_content = f"{message.content}"
         content = '<tool_response>\n{"name": "' + message.name + '", "content": ' + tool_response_content + '}\n</tool_response>'
+    elif isinstance(message.content, list):
+        content = ""
+        for e in message.content:
+            if isinstance(e, str):
+                content += e
+            elif isinstance(e, Blob) and (e.is_text()):
+                text = (await e.as_bytes()).decode("utf-8")
+                filename = (" name='" + e.path + "'") if e.path else ''
+                text = f"\n<file{filename}>\n{text}\n</file>\n"
+                content += text
+            else:
+                raise ValueError(
+                    "Elements in ChatMessage.content must be str or Blob (text)"
+                )
     else:
         content = message.content
 
     return {
         "role": message.role,
         **({"content": content} if content else {}),
         **({"name": message.name} if message.name else {})
```

### Comparing `bpm_ai_inference-0.3.0/bpm_ai_inference/ocr/tesseract.py` & `bpm_ai_inference-0.3.1/bpm_ai_inference/ocr/tesseract.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.0/bpm_ai_inference/pos/spacy_pos_tagger.py` & `bpm_ai_inference-0.3.1/bpm_ai_inference/pos/spacy_pos_tagger.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.0/bpm_ai_inference/question_answering/pix2struct_vqa.py` & `bpm_ai_inference-0.3.1/bpm_ai_inference/question_answering/pix2struct_vqa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.0/bpm_ai_inference/question_answering/transformers_docvqa.py` & `bpm_ai_inference-0.3.1/bpm_ai_inference/question_answering/transformers_docvqa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.0/bpm_ai_inference/question_answering/transformers_qa.py` & `bpm_ai_inference-0.3.1/bpm_ai_inference/question_answering/transformers_qa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.0/bpm_ai_inference/speech_recognition/faster_whisper.py` & `bpm_ai_inference-0.3.1/bpm_ai_inference/speech_recognition/faster_whisper.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.0/bpm_ai_inference/token_classification/gliner_token_classifier.py` & `bpm_ai_inference-0.3.1/bpm_ai_inference/token_classification/gliner_token_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.0/bpm_ai_inference/token_classification/transformers_token_classifier.py` & `bpm_ai_inference-0.3.1/bpm_ai_inference/token_classification/transformers_token_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.0/bpm_ai_inference/translation/easy_nmt/easy_nmt.py` & `bpm_ai_inference-0.3.1/bpm_ai_inference/translation/easy_nmt/easy_nmt.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.0/bpm_ai_inference/translation/easy_nmt/opus_mt.py` & `bpm_ai_inference-0.3.1/bpm_ai_inference/translation/easy_nmt/opus_mt.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.0/bpm_ai_inference/translation/easy_nmt/util.py` & `bpm_ai_inference-0.3.1/bpm_ai_inference/translation/easy_nmt/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.0/bpm_ai_inference/util/language.py` & `bpm_ai_inference-0.3.1/bpm_ai_inference/util/language.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.0/bpm_ai_inference/util/optimum.py` & `bpm_ai_inference-0.3.1/bpm_ai_inference/util/optimum.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.0/pyproject.toml` & `bpm_ai_inference-0.3.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "bpm-ai-inference"
-version = "0.3.0"
+version = "0.3.1"
 description = "Inference and server for local AI implementations of bpm-ai-core abstractions."
 authors = ["Bennet Krause <bennet.krause@holisticon.de>"]
 repository = "https://github.com/holunda-io/bpm-ai-inference"
 homepage = "https://www.holisticon.de/"
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
-bpm-ai-core = "^2.6.0"
+bpm-ai-core = "^2.6.1"
 langfuse = "^2.7.6"
 faster-whisper = "^0.10.0"
 lingua-language-detector = "^2.0.2"
 pytesseract = "^0.3.10"
 transformers = "^4.39.3"
 sacremoses = "^0.1.1"
 sentencepiece = "^0.2.0"
```

### Comparing `bpm_ai_inference-0.3.0/PKG-INFO` & `bpm_ai_inference-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: bpm-ai-inference
-Version: 0.3.0
+Version: 0.3.1
 Summary: Inference and server for local AI implementations of bpm-ai-core abstractions.
 Home-page: https://www.holisticon.de/
 License: GPL-3.0-or-later
 Author: Bennet Krause
 Author-email: bennet.krause@holisticon.de
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: bpm-ai-core (>=2.6.0,<3.0.0)
+Requires-Dist: bpm-ai-core (>=2.6.1,<3.0.0)
 Requires-Dist: faster-whisper (>=0.10.0,<0.11.0)
 Requires-Dist: gliner (>=0.1.6,<0.2.0)
 Requires-Dist: langfuse (>=2.7.6,<3.0.0)
 Requires-Dist: lingua-language-detector (>=2.0.2,<3.0.0)
 Requires-Dist: llama-cpp-python (>=0.2.65,<0.3.0)
 Requires-Dist: nltk (>=3.8.0,<4.0.0)
 Requires-Dist: optimum[onnxruntime] (>=1.18.0,<2.0.0)
```

