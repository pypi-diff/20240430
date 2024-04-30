# Comparing `tmp/bpm_ai_inference-0.3.1.tar.gz` & `tmp/bpm_ai_inference-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpm_ai_inference-0.3.1.tar", max compression
+gzip compressed data, was "bpm_ai_inference-0.3.2.tar", max compression
```

## Comparing `bpm_ai_inference-0.3.1.tar` & `bpm_ai_inference-0.3.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    35128 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/LICENSE
--rw-r--r--   0        0        0      743 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/README.md
--rw-r--r--   0        0        0        0 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/classification/__init__.py
--rw-r--r--   0        0        0     2852 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/classification/transformers_text_classifier.py
--rw-r--r--   0        0        0     1740 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/daemon.py
--rw-r--r--   0        0        0        0 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/image_classification/__init__.py
--rw-r--r--   0        0        0     2547 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/image_classification/transformers_image_classifier.py
--rw-r--r--   0        0        0        0 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/llm/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/llm/llama_cpp/__init__.py
--rw-r--r--   0        0        0      222 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/llm/llama_cpp/_constants.py
--rw-r--r--   0        0        0     8197 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/llm/llama_cpp/llama_chat.py
--rw-r--r--   0        0        0      199 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/llm/llama_cpp/output_schema.prompt
--rw-r--r--   0        0        0      981 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/llm/llama_cpp/tool_use.prompt
--rw-r--r--   0        0        0     1725 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/llm/llama_cpp/util.py
--rw-r--r--   0        0        0        0 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/ocr/__init__.py
--rw-r--r--   0        0        0     3256 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/ocr/tesseract.py
--rw-r--r--   0        0        0        0 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/pos/__init__.py
--rw-r--r--   0        0        0     1833 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/pos/spacy_pos_tagger.py
--rw-r--r--   0        0        0        0 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/question_answering/__init__.py
--rw-r--r--   0        0        0     2154 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/question_answering/pix2struct_vqa.py
--rw-r--r--   0        0        0     2056 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/question_answering/transformers_docvqa.py
--rw-r--r--   0        0        0     1940 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/question_answering/transformers_qa.py
--rw-r--r--   0        0        0        0 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/speech_recognition/__init__.py
--rw-r--r--   0        0        0     1219 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/speech_recognition/faster_whisper.py
--rw-r--r--   0        0        0        0 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/token_classification/__init__.py
--rw-r--r--   0        0        0     1402 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/token_classification/gliner_token_classifier.py
--rw-r--r--   0        0        0     3178 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/token_classification/transformers_token_classifier.py
--rw-r--r--   0        0        0        0 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/translation/__init__.py
--rw-r--r--   0        0        0        2 2024-04-29 14:05:03.505646 bpm_ai_inference-0.3.1/bpm_ai_inference/translation/easy_nmt/__init__.py
--rw-r--r--   0        0        0    18731 2024-04-29 14:05:03.509647 bpm_ai_inference-0.3.1/bpm_ai_inference/translation/easy_nmt/easy_nmt.py
--rw-r--r--   0        0        0     2423 2024-04-29 14:05:03.509647 bpm_ai_inference-0.3.1/bpm_ai_inference/translation/easy_nmt/opus_mt.py
--rw-r--r--   0        0        0     1784 2024-04-29 14:05:03.509647 bpm_ai_inference-0.3.1/bpm_ai_inference/translation/easy_nmt/util.py
--rw-r--r--   0        0        0       36 2024-04-29 14:05:03.509647 bpm_ai_inference-0.3.1/bpm_ai_inference/util/__init__.py
--rw-r--r--   0        0        0      483 2024-04-29 14:05:03.509647 bpm_ai_inference-0.3.1/bpm_ai_inference/util/files.py
--rw-r--r--   0        0        0      122 2024-04-29 14:05:03.509647 bpm_ai_inference-0.3.1/bpm_ai_inference/util/hf.py
--rw-r--r--   0        0        0      828 2024-04-29 14:05:03.509647 bpm_ai_inference-0.3.1/bpm_ai_inference/util/language.py
--rw-r--r--   0        0        0     7153 2024-04-29 14:05:03.509647 bpm_ai_inference-0.3.1/bpm_ai_inference/util/optimum.py
--rw-r--r--   0        0        0     1014 2024-04-29 14:05:03.509647 bpm_ai_inference-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 bpm_ai_inference-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    35128 2024-04-30 09:08:44.331001 bpm_ai_inference-0.3.2/LICENSE
+-rw-r--r--   0        0        0      743 2024-04-30 09:08:44.331001 bpm_ai_inference-0.3.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 09:08:44.331001 bpm_ai_inference-0.3.2/bpm_ai_inference/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:08:44.331001 bpm_ai_inference-0.3.2/bpm_ai_inference/classification/__init__.py
+-rw-r--r--   0        0        0     2852 2024-04-30 09:08:44.331001 bpm_ai_inference-0.3.2/bpm_ai_inference/classification/transformers_text_classifier.py
+-rw-r--r--   0        0        0     1875 2024-04-30 09:08:44.331001 bpm_ai_inference-0.3.2/bpm_ai_inference/daemon.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:08:44.331001 bpm_ai_inference-0.3.2/bpm_ai_inference/image_classification/__init__.py
+-rw-r--r--   0        0        0     2547 2024-04-30 09:08:44.331001 bpm_ai_inference-0.3.2/bpm_ai_inference/image_classification/transformers_image_classifier.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:08:44.331001 bpm_ai_inference-0.3.2/bpm_ai_inference/llm/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:08:44.331001 bpm_ai_inference-0.3.2/bpm_ai_inference/llm/llama_cpp/__init__.py
+-rw-r--r--   0        0        0      222 2024-04-30 09:08:44.331001 bpm_ai_inference-0.3.2/bpm_ai_inference/llm/llama_cpp/_constants.py
+-rw-r--r--   0        0        0     8197 2024-04-30 09:08:44.331001 bpm_ai_inference-0.3.2/bpm_ai_inference/llm/llama_cpp/llama_chat.py
+-rw-r--r--   0        0        0      199 2024-04-30 09:08:44.331001 bpm_ai_inference-0.3.2/bpm_ai_inference/llm/llama_cpp/output_schema.prompt
+-rw-r--r--   0        0        0      981 2024-04-30 09:08:44.331001 bpm_ai_inference-0.3.2/bpm_ai_inference/llm/llama_cpp/tool_use.prompt
+-rw-r--r--   0        0        0     1725 2024-04-30 09:08:44.331001 bpm_ai_inference-0.3.2/bpm_ai_inference/llm/llama_cpp/util.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:08:44.331001 bpm_ai_inference-0.3.2/bpm_ai_inference/ocr/__init__.py
+-rw-r--r--   0        0        0     3256 2024-04-30 09:08:44.331001 bpm_ai_inference-0.3.2/bpm_ai_inference/ocr/tesseract.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:08:44.331001 bpm_ai_inference-0.3.2/bpm_ai_inference/pos/__init__.py
+-rw-r--r--   0        0        0     1833 2024-04-30 09:08:44.331001 bpm_ai_inference-0.3.2/bpm_ai_inference/pos/spacy_pos_tagger.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:08:44.331001 bpm_ai_inference-0.3.2/bpm_ai_inference/question_answering/__init__.py
+-rw-r--r--   0        0        0     2154 2024-04-30 09:08:44.331001 bpm_ai_inference-0.3.2/bpm_ai_inference/question_answering/pix2struct_vqa.py
+-rw-r--r--   0        0        0     2056 2024-04-30 09:08:44.335001 bpm_ai_inference-0.3.2/bpm_ai_inference/question_answering/transformers_docvqa.py
+-rw-r--r--   0        0        0     1940 2024-04-30 09:08:44.335001 bpm_ai_inference-0.3.2/bpm_ai_inference/question_answering/transformers_qa.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:08:44.335001 bpm_ai_inference-0.3.2/bpm_ai_inference/speech_recognition/__init__.py
+-rw-r--r--   0        0        0     1219 2024-04-30 09:08:44.335001 bpm_ai_inference-0.3.2/bpm_ai_inference/speech_recognition/faster_whisper.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:08:44.335001 bpm_ai_inference-0.3.2/bpm_ai_inference/token_classification/__init__.py
+-rw-r--r--   0        0        0     1402 2024-04-30 09:08:44.335001 bpm_ai_inference-0.3.2/bpm_ai_inference/token_classification/gliner_token_classifier.py
+-rw-r--r--   0        0        0     3178 2024-04-30 09:08:44.335001 bpm_ai_inference-0.3.2/bpm_ai_inference/token_classification/transformers_token_classifier.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:08:44.335001 bpm_ai_inference-0.3.2/bpm_ai_inference/translation/__init__.py
+-rw-r--r--   0        0        0        2 2024-04-30 09:08:44.335001 bpm_ai_inference-0.3.2/bpm_ai_inference/translation/easy_nmt/__init__.py
+-rw-r--r--   0        0        0    18731 2024-04-30 09:08:44.335001 bpm_ai_inference-0.3.2/bpm_ai_inference/translation/easy_nmt/easy_nmt.py
+-rw-r--r--   0        0        0     2423 2024-04-30 09:08:44.335001 bpm_ai_inference-0.3.2/bpm_ai_inference/translation/easy_nmt/opus_mt.py
+-rw-r--r--   0        0        0     1784 2024-04-30 09:08:44.335001 bpm_ai_inference-0.3.2/bpm_ai_inference/translation/easy_nmt/util.py
+-rw-r--r--   0        0        0       36 2024-04-30 09:08:44.335001 bpm_ai_inference-0.3.2/bpm_ai_inference/util/__init__.py
+-rw-r--r--   0        0        0      483 2024-04-30 09:08:44.335001 bpm_ai_inference-0.3.2/bpm_ai_inference/util/files.py
+-rw-r--r--   0        0        0      122 2024-04-30 09:08:44.335001 bpm_ai_inference-0.3.2/bpm_ai_inference/util/hf.py
+-rw-r--r--   0        0        0      828 2024-04-30 09:08:44.335001 bpm_ai_inference-0.3.2/bpm_ai_inference/util/language.py
+-rw-r--r--   0        0        0     7153 2024-04-30 09:08:44.335001 bpm_ai_inference-0.3.2/bpm_ai_inference/util/optimum.py
+-rw-r--r--   0        0        0     1014 2024-04-30 09:08:44.335001 bpm_ai_inference-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 bpm_ai_inference-0.3.2/PKG-INFO
```

### Comparing `bpm_ai_inference-0.3.1/LICENSE` & `bpm_ai_inference-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.1/README.md` & `bpm_ai_inference-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.1/bpm_ai_inference/classification/transformers_text_classifier.py` & `bpm_ai_inference-0.3.2/bpm_ai_inference/classification/transformers_text_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.1/bpm_ai_inference/daemon.py` & `bpm_ai_inference-0.3.2/bpm_ai_inference/daemon.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,15 +31,17 @@
     ChatLlamaCpp
 ]
 
 if __name__ == "__main__":
     logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.INFO)
 
     daemon = create_remote_object_daemon(
-        host=os.environ.get('DAEMON_HOST', '0.0.0.0'),
-        port=int(os.environ.get('DAEMON_PORT', 6666))
+        host=os.getenv('DAEMON_HOST', '0.0.0.0'),
+        port=int(os.getenv('DAEMON_PORT', 6666)),
+        instance_strategy=os.getenv('INSTANCE_STRATEGY', 'memory_limit'),
+        max_memory=int(os.getenv('SOFT_MEMORY_LIMIT', 8_589_934_592))
     )
 
     for c in remote_classes:
         daemon.register_class(c)
 
     daemon.serve()
```

### Comparing `bpm_ai_inference-0.3.1/bpm_ai_inference/image_classification/transformers_image_classifier.py` & `bpm_ai_inference-0.3.2/bpm_ai_inference/image_classification/transformers_image_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.1/bpm_ai_inference/llm/llama_cpp/llama_chat.py` & `bpm_ai_inference-0.3.2/bpm_ai_inference/llm/llama_cpp/llama_chat.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.1/bpm_ai_inference/llm/llama_cpp/tool_use.prompt` & `bpm_ai_inference-0.3.2/bpm_ai_inference/llm/llama_cpp/tool_use.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.1/bpm_ai_inference/llm/llama_cpp/util.py` & `bpm_ai_inference-0.3.2/bpm_ai_inference/llm/llama_cpp/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.1/bpm_ai_inference/ocr/tesseract.py` & `bpm_ai_inference-0.3.2/bpm_ai_inference/ocr/tesseract.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.1/bpm_ai_inference/pos/spacy_pos_tagger.py` & `bpm_ai_inference-0.3.2/bpm_ai_inference/pos/spacy_pos_tagger.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.1/bpm_ai_inference/question_answering/pix2struct_vqa.py` & `bpm_ai_inference-0.3.2/bpm_ai_inference/question_answering/pix2struct_vqa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.1/bpm_ai_inference/question_answering/transformers_docvqa.py` & `bpm_ai_inference-0.3.2/bpm_ai_inference/question_answering/transformers_docvqa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.1/bpm_ai_inference/question_answering/transformers_qa.py` & `bpm_ai_inference-0.3.2/bpm_ai_inference/question_answering/transformers_qa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.1/bpm_ai_inference/speech_recognition/faster_whisper.py` & `bpm_ai_inference-0.3.2/bpm_ai_inference/speech_recognition/faster_whisper.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.1/bpm_ai_inference/token_classification/gliner_token_classifier.py` & `bpm_ai_inference-0.3.2/bpm_ai_inference/token_classification/gliner_token_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.1/bpm_ai_inference/token_classification/transformers_token_classifier.py` & `bpm_ai_inference-0.3.2/bpm_ai_inference/token_classification/transformers_token_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.1/bpm_ai_inference/translation/easy_nmt/easy_nmt.py` & `bpm_ai_inference-0.3.2/bpm_ai_inference/translation/easy_nmt/easy_nmt.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.1/bpm_ai_inference/translation/easy_nmt/opus_mt.py` & `bpm_ai_inference-0.3.2/bpm_ai_inference/translation/easy_nmt/opus_mt.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.1/bpm_ai_inference/translation/easy_nmt/util.py` & `bpm_ai_inference-0.3.2/bpm_ai_inference/translation/easy_nmt/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.1/bpm_ai_inference/util/language.py` & `bpm_ai_inference-0.3.2/bpm_ai_inference/util/language.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.1/bpm_ai_inference/util/optimum.py` & `bpm_ai_inference-0.3.2/bpm_ai_inference/util/optimum.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.3.1/pyproject.toml` & `bpm_ai_inference-0.3.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bpm-ai-inference"
-version = "0.3.1"
+version = "0.3.2"
 description = "Inference and server for local AI implementations of bpm-ai-core abstractions."
 authors = ["Bennet Krause <bennet.krause@holisticon.de>"]
 repository = "https://github.com/holunda-io/bpm-ai-inference"
 homepage = "https://www.holisticon.de/"
 license = "GPL-3.0-or-later"
 readme = "README.md"
```

### Comparing `bpm_ai_inference-0.3.1/PKG-INFO` & `bpm_ai_inference-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpm-ai-inference
-Version: 0.3.1
+Version: 0.3.2
 Summary: Inference and server for local AI implementations of bpm-ai-core abstractions.
 Home-page: https://www.holisticon.de/
 License: GPL-3.0-or-later
 Author: Bennet Krause
 Author-email: bennet.krause@holisticon.de
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

