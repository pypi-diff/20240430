# Comparing `tmp/ecologits-0.1.2.tar.gz` & `tmp/ecologits-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecologits-0.1.2.tar", max compression
+gzip compressed data, was "ecologits-0.1.3.tar", max compression
```

## Comparing `ecologits-0.1.2.tar` & `ecologits-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    16725 2024-04-18 18:10:36.160210 ecologits-0.1.2/LICENSE
--rw-r--r--   0        0        0     1312 2024-04-18 18:10:36.160210 ecologits-0.1.2/README.md
--rw-r--r--   0        0        0       58 2024-04-18 18:10:36.160210 ecologits-0.1.2/ecologits/__init__.py
--rw-r--r--   0        0        0     5763 2024-04-18 18:10:36.160210 ecologits-0.1.2/ecologits/data/models.csv
--rw-r--r--   0        0        0     1865 2024-04-18 18:10:36.160210 ecologits-0.1.2/ecologits/ecologits.py
--rw-r--r--   0        0        0      140 2024-04-18 18:10:36.160210 ecologits-0.1.2/ecologits/exceptions.py
--rw-r--r--   0        0        0      121 2024-04-18 18:10:36.160210 ecologits-0.1.2/ecologits/impacts/__init__.py
--rw-r--r--   0        0        0     1468 2024-04-18 18:10:36.160210 ecologits-0.1.2/ecologits/impacts/dag.py
--rw-r--r--   0        0        0     7605 2024-04-18 18:10:36.160210 ecologits-0.1.2/ecologits/impacts/llm.py
--rw-r--r--   0        0        0     1458 2024-04-18 18:10:36.160210 ecologits-0.1.2/ecologits/impacts/models.py
--rw-r--r--   0        0        0     2992 2024-04-18 18:10:36.160210 ecologits-0.1.2/ecologits/model_repository.py
--rw-r--r--   0        0        0        0 2024-04-18 18:10:36.160210 ecologits-0.1.2/ecologits/tracers/__init__.py
--rw-r--r--   0        0        0     7848 2024-04-18 18:10:36.160210 ecologits-0.1.2/ecologits/tracers/anthropic_tracer.py
--rw-r--r--   0        0        0     5094 2024-04-18 18:10:36.160210 ecologits-0.1.2/ecologits/tracers/cohere_tracer.py
--rw-r--r--   0        0        0     5554 2024-04-18 18:10:36.160210 ecologits-0.1.2/ecologits/tracers/huggingface_tracer.py
--rw-r--r--   0        0        0     5065 2024-04-18 18:10:36.160210 ecologits-0.1.2/ecologits/tracers/mistralai_tracer.py
--rw-r--r--   0        0        0     5313 2024-04-18 18:10:36.160210 ecologits-0.1.2/ecologits/tracers/openai_tracer.py
--rw-r--r--   0        0        0     1139 2024-04-18 18:10:36.160210 ecologits-0.1.2/ecologits/tracers/utils.py
--rw-r--r--   0        0        0     3401 2024-04-18 18:10:36.160210 ecologits-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3497 1970-01-01 00:00:00.000000 ecologits-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    16725 2024-04-30 16:58:29.732136 ecologits-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2243 2024-04-30 16:58:29.732136 ecologits-0.1.3/README.md
+-rw-r--r--   0        0        0       80 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/__init__.py
+-rw-r--r--   0        0        0    11901 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/data/models.csv
+-rw-r--r--   0        0        0     2798 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/ecologits.py
+-rw-r--r--   0        0        0      140 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/exceptions.py
+-rw-r--r--   0        0        0      121 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/impacts/__init__.py
+-rw-r--r--   0        0        0     1468 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/impacts/dag.py
+-rw-r--r--   0        0        0    14956 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/impacts/llm.py
+-rw-r--r--   0        0        0     4066 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/impacts/models.py
+-rw-r--r--   0        0        0     2992 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/model_repository.py
+-rw-r--r--   0        0        0        0 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/tracers/__init__.py
+-rw-r--r--   0        0        0     7848 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/tracers/anthropic_tracer.py
+-rw-r--r--   0        0        0     5094 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/tracers/cohere_tracer.py
+-rw-r--r--   0        0        0     5554 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/tracers/huggingface_tracer.py
+-rw-r--r--   0        0        0     5065 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/tracers/mistralai_tracer.py
+-rw-r--r--   0        0        0     5313 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/tracers/openai_tracer.py
+-rw-r--r--   0        0        0     1496 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/tracers/utils.py
+-rw-r--r--   0        0        0     3591 2024-04-30 16:58:29.736136 ecologits-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4428 1970-01-01 00:00:00.000000 ecologits-0.1.3/PKG-INFO
```

### Comparing `ecologits-0.1.2/LICENSE` & `ecologits-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.2/ecologits/impacts/dag.py` & `ecologits-0.1.3/ecologits/impacts/dag.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.2/ecologits/model_repository.py` & `ecologits-0.1.3/ecologits/model_repository.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.2/ecologits/tracers/anthropic_tracer.py` & `ecologits-0.1.3/ecologits/tracers/anthropic_tracer.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.2/ecologits/tracers/cohere_tracer.py` & `ecologits-0.1.3/ecologits/tracers/cohere_tracer.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.2/ecologits/tracers/huggingface_tracer.py` & `ecologits-0.1.3/ecologits/tracers/huggingface_tracer.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.2/ecologits/tracers/mistralai_tracer.py` & `ecologits-0.1.3/ecologits/tracers/mistralai_tracer.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.2/ecologits/tracers/openai_tracer.py` & `ecologits-0.1.3/ecologits/tracers/openai_tracer.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.2/pyproject.toml` & `ecologits-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ecologits"
-version = "0.1.2"
+version = "0.1.3"
 description = "EcoLogits tracks and estimates the energy consumption and environmental impacts of using generative AI models through APIs."
 authors = [
     "GenAI Impact",
     "Data For Good"
 ]
 maintainers = [
     "GenAI Impact"
@@ -68,14 +68,18 @@
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.5.3"
 mkdocs-material = "^9.5.12"
+mkdocstrings = {version = "^0.25.0", extras = ["python"]}
+mkdocs-gen-files = "^0.5.0"
+mkdocs-autorefs = "^1.0.1"
+mkdocs-literate-nav = "^0.6.1"
 
 
 [pytest]
 env_files = [".env"]
 
 
 [tool.ruff]
@@ -182,7 +186,10 @@
 
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
 target-version = "py39"
 
 [tool.ruff.mccabe]
 max-complexity = 10
+
+[tool.ruff.pydocstyle]
+convention = "google"
```

