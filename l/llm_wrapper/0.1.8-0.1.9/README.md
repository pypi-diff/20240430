# Comparing `tmp/llm_wrapper-0.1.8.tar.gz` & `tmp/llm_wrapper-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_wrapper-0.1.8.tar", max compression
+gzip compressed data, was "llm_wrapper-0.1.9.tar", max compression
```

## Comparing `llm_wrapper-0.1.8.tar` & `llm_wrapper-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1070 2024-01-17 13:40:57.828232 llm_wrapper-0.1.8/LICENSE
--rw-r--r--   0        0        0     4181 2024-01-17 18:25:30.903899 llm_wrapper-0.1.8/README.md
--rw-r--r--   0        0        0       49 2024-04-30 08:12:51.123438 llm_wrapper-0.1.8/llm_wrapper/__init__.py
--rw-r--r--   0        0        0    14551 2024-02-20 14:16:34.131826 llm_wrapper-0.1.8/llm_wrapper/main.py
--rw-r--r--   0        0        0      625 2024-04-30 08:12:36.843864 llm_wrapper-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     4775 1970-01-01 00:00:00.000000 llm_wrapper-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-01-17 13:40:57.828232 llm_wrapper-0.1.9/LICENSE
+-rw-r--r--   0        0        0     4181 2024-01-17 18:25:30.903899 llm_wrapper-0.1.9/README.md
+-rw-r--r--   0        0        0       49 2024-04-30 10:01:57.511360 llm_wrapper-0.1.9/llm_wrapper/__init__.py
+-rw-r--r--   0        0        0    14642 2024-04-30 10:01:36.273362 llm_wrapper-0.1.9/llm_wrapper/main.py
+-rw-r--r--   0        0        0      625 2024-04-30 10:02:02.607680 llm_wrapper-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4775 1970-01-01 00:00:00.000000 llm_wrapper-0.1.9/PKG-INFO
```

### Comparing `llm_wrapper-0.1.8/LICENSE` & `llm_wrapper-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_wrapper-0.1.8/README.md` & `llm_wrapper-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `llm_wrapper-0.1.8/llm_wrapper/main.py` & `llm_wrapper-0.1.9/llm_wrapper/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #             "## CONTEXT\n{doc_string}\n\n" \
 #             "## FORMAT\n{format_instructions}\n\n" \
 #             "## OBJECTIVE\nRespond with the appropiate JSON instance only.\n\n" \
 #             "## RESPONSE\n"
             
 template_minimal = "user request:{query}\n\naction:\n{doc_string}\n\nformatting:\n{format_instructions}\n\nnote:\nrespond exactly as instructed without comments\n\nresponse:\n"
             
-# template_verbose = """You are a developer working on a new API. You are tasked with mimicing the output of a function that returns a JSON instance.
+# template_verbose = """You are a developer working on a new API. You are tasked with mimicking the output of a function that returns a JSON instance.
 # {doc_string}\n\n
 # Respond to the user with a JSON instance that meets their criteria. Do not respond with anything else but the json instance.
 # {format_instructions}
     
 # REQUEST:    
 # {query}
     
@@ -334,14 +334,15 @@
             elif self.return_type == str:
                 return str(response)
             elif self.return_type == bool:
                 return bool(response.lower() == "true")
             elif self.return_type == list:
                 return list(json.loads(response))
             elif self.return_type == dict:
+                response = response.replace("\n", "").replace("\t", "").replace("\r", "")
                 return dict(json.loads(response))
             elif self.return_type == set:
                 # Convert set syntax to list syntax
                 llm_output_as_list = response.replace('{', '[').replace('}', ']')
                 # Parse the string into a list
                 parsed_list = json.loads(llm_output_as_list)
                 # Convert the list to a set
```

### Comparing `llm_wrapper-0.1.8/pyproject.toml` & `llm_wrapper-0.1.9/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llm_wrapper"
-version = "0.1.8"
+version = "0.1.9"
 description = "Run llm functions with just inline documentation and no code"
 authors = ["Meir Michanie <meirm@riunx.com>"]
 readme = "README.md"
 keywords = ["openai", "langchain", "pydantic"]
 homepage = "https://github.com/meirm/llm_functions"
 
 [build-system]
```

### Comparing `llm_wrapper-0.1.8/PKG-INFO` & `llm_wrapper-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm_wrapper
-Version: 0.1.8
+Version: 0.1.9
 Summary: Run llm functions with just inline documentation and no code
 Home-page: https://github.com/meirm/llm_functions
 Keywords: openai,langchain,pydantic
 Author: Meir Michanie
 Author-email: meirm@riunx.com
 Requires-Python: >=3.11
 Classifier: Programming Language :: Python :: 3
```

