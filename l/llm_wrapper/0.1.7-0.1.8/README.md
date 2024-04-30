# Comparing `tmp/llm_wrapper-0.1.7.tar.gz` & `tmp/llm_wrapper-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_wrapper-0.1.7.tar", max compression
+gzip compressed data, was "llm_wrapper-0.1.8.tar", max compression
```

## Comparing `llm_wrapper-0.1.7.tar` & `llm_wrapper-0.1.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1070 2024-01-17 13:40:57.828232 llm_wrapper-0.1.7/LICENSE
--rw-r--r--   0        0        0     4181 2024-01-17 18:25:30.903899 llm_wrapper-0.1.7/README.md
--rw-r--r--   0        0        0       48 2024-01-31 04:34:07.939197 llm_wrapper-0.1.7/llm_wrapper/__init__.py
--rw-r--r--   0        0        0     9551 2024-01-31 04:32:47.983407 llm_wrapper-0.1.7/llm_wrapper/main.py
--rw-r--r--   0        0        0      621 2024-01-31 04:34:06.177097 llm_wrapper-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     4802 1970-01-01 00:00:00.000000 llm_wrapper-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-01-17 13:40:57.828232 llm_wrapper-0.1.8/LICENSE
+-rw-r--r--   0        0        0     4181 2024-01-17 18:25:30.903899 llm_wrapper-0.1.8/README.md
+-rw-r--r--   0        0        0       49 2024-04-30 08:12:51.123438 llm_wrapper-0.1.8/llm_wrapper/__init__.py
+-rw-r--r--   0        0        0    14551 2024-02-20 14:16:34.131826 llm_wrapper-0.1.8/llm_wrapper/main.py
+-rw-r--r--   0        0        0      625 2024-04-30 08:12:36.843864 llm_wrapper-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     4775 1970-01-01 00:00:00.000000 llm_wrapper-0.1.8/PKG-INFO
```

### Comparing `llm_wrapper-0.1.7/LICENSE` & `llm_wrapper-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_wrapper-0.1.7/README.md` & `llm_wrapper-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `llm_wrapper-0.1.7/PKG-INFO` & `llm_wrapper-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: llm_wrapper
-Version: 0.1.7
+Version: 0.1.8
 Summary: Run llm functions with just inline documentation and no code
 Home-page: https://github.com/meirm/llm_functions
 Keywords: openai,langchain,pydantic
 Author: Meir Michanie
 Author-email: meirm@riunx.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: langchain (>=0.1.0,<0.2.0)
-Requires-Dist: langchain_community (>=0.0.12,<0.0.13)
-Requires-Dist: pydantic (>=2.5.3,<3.0.0)
+Requires-Dist: langchain (>=0.1.0)
+Requires-Dist: langchain_community (>=0.0.12)
+Requires-Dist: pydantic (>=2.5.3)
 Description-Content-Type: text/markdown
 
 # LLM Functions Library Usage Guide
 
 This guide provides a comprehensive overview of how to use the `llm_wrapper` library, which offers a versatile wrapper, `llm_func`, designed for seamless interactions with various language learning models (LLMs). The wrapper simplifies model initialization, query execution, and structured output parsing, supporting a wide range of return types including basic data types (`int`, `float`, `str`, `bool`, `set`, `list`, `dict`) and complex Pydantic `BaseModel` structures.
 
 ## Getting Started
```

