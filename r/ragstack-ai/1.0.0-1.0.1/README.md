# Comparing `tmp/ragstack_ai-1.0.0.tar.gz` & `tmp/ragstack_ai-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragstack_ai-1.0.0.tar", max compression
+gzip compressed data, was "ragstack_ai-1.0.1.tar", max compression
```

## Comparing `ragstack_ai-1.0.0.tar` & `ragstack_ai-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3781 2024-04-24 15:31:59.581683 ragstack_ai-1.0.0/LICENSE.md
--rw-r--r--   0        0        0     2395 2024-04-24 15:31:59.581683 ragstack_ai-1.0.0/PACKAGE_README.md
--rw-r--r--   0        0        0     1790 2024-04-24 15:31:59.613683 ragstack_ai-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      271 2024-04-24 15:31:59.613683 ragstack_ai-1.0.0/ragstack/__init__.py
--rw-r--r--   0        0        0     3207 1970-01-01 00:00:00.000000 ragstack_ai-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3781 2024-04-30 16:38:42.757662 ragstack_ai-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0     2395 2024-04-30 16:38:42.757662 ragstack_ai-1.0.1/PACKAGE_README.md
+-rw-r--r--   0        0        0     1792 2024-04-30 16:38:42.785662 ragstack_ai-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      271 2024-04-30 16:38:42.785662 ragstack_ai-1.0.1/ragstack/__init__.py
+-rw-r--r--   0        0        0     3207 1970-01-01 00:00:00.000000 ragstack_ai-1.0.1/PKG-INFO
```

### Comparing `ragstack_ai-1.0.0/LICENSE.md` & `ragstack_ai-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ragstack_ai-1.0.0/PACKAGE_README.md` & `ragstack_ai-1.0.1/PACKAGE_README.md`

 * *Files identical despite different names*

### Comparing `ragstack_ai-1.0.0/pyproject.toml` & `ragstack_ai-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "ragstack-ai"
-version = "1.0.0"
+version = "1.0.1"
 description = "DataStax RAGStack"
 license = "BUSL-1.1"
 authors = ["DataStax"]
 readme = "PACKAGE_README.md"
 repository = "https://github.com/datastax/ragstack-ai"
 documentation = "https://docs.datastax.com/en/ragstack"
 packages = [{ include = "ragstack" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
-ragstack-ai-langchain = { version = "1.0.0", extras = ["colbert", "google", "nvidia"] }
-ragstack-ai-llamaindex = { version = "1.0.0", extras = ["colbert", "google", "azure", "bedrock"] }
-ragstack-ai-colbert = "1.0.0"
+ragstack-ai-langchain = { version = "1.0.1", extras = ["colbert", "google", "nvidia"] }
+ragstack-ai-llamaindex = { version = "1.0.1", extras = ["colbert", "google", "azure", "bedrock"] }
+ragstack-ai-colbert = "1.0.1"
 
 [tool.poetry.group.test.dependencies]
 ragstack-ai-langchain = { path = "libs/langchain", develop = true, extras = ["colbert", "google", "nvidia"] }
 ragstack-ai-llamaindex = { path = "libs/llamaindex", develop = true, extras = ["colbert", "google", "azure", "bedrock"] }
 ragstack-ai-colbert = { path = "libs/colbert", develop = true }
 
 pytest = "^7.3.0"
@@ -48,14 +48,16 @@
 warn_unused_ignores = true
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
+
 [tool.poetry.group.dev.dependencies]
 yamllint = "^1.34.0"
 
 
+
 [tool.poetry.group.notebooks.dependencies]
 nbmake = "*"
 astrapy = "*"
```

### Comparing `ragstack_ai-1.0.0/PKG-INFO` & `ragstack_ai-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: ragstack-ai
-Version: 1.0.0
+Version: 1.0.1
 Summary: DataStax RAGStack
 Home-page: https://github.com/datastax/ragstack-ai
 License: BUSL-1.1
 Author: DataStax
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: ragstack-ai-colbert (==1.0.0)
-Requires-Dist: ragstack-ai-langchain[colbert,google,nvidia] (==1.0.0)
-Requires-Dist: ragstack-ai-llamaindex[azure,bedrock,colbert,google] (==1.0.0)
+Requires-Dist: ragstack-ai-colbert (==1.0.1)
+Requires-Dist: ragstack-ai-langchain[colbert,google,nvidia] (==1.0.1)
+Requires-Dist: ragstack-ai-llamaindex[azure,bedrock,colbert,google] (==1.0.1)
 Project-URL: Documentation, https://docs.datastax.com/en/ragstack
 Project-URL: Repository, https://github.com/datastax/ragstack-ai
 Description-Content-Type: text/markdown
 
 # RAGStack
 [![Release Notes](https://img.shields.io/github/v/release/datastax/ragstack-ai.svg)](https://github.com/datastax/ragstack-ai/releases)
 [![Downloads](https://static.pepy.tech/badge/ragstack-ai/month)](https://www.pepy.tech/projects/ragstack-ai)
```

