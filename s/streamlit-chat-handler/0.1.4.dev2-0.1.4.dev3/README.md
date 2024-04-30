# Comparing `tmp/streamlit_chat_handler-0.1.4.dev2.tar.gz` & `tmp/streamlit_chat_handler-0.1.4.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_chat_handler-0.1.4.dev2.tar", last modified: Mon Apr 29 01:36:40 2024, max compression
+gzip compressed data, was "streamlit_chat_handler-0.1.4.dev3.tar", last modified: Mon Apr 29 01:38:28 2024, max compression
```

## Comparing `streamlit_chat_handler-0.1.4.dev2.tar` & `streamlit_chat_handler-0.1.4.dev3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-29 01:36:40.650458 streamlit_chat_handler-0.1.4.dev2/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1083 2024-04-23 04:06:28.000000 streamlit_chat_handler-0.1.4.dev2/LICENSE
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3737 2024-04-29 01:36:40.650458 streamlit_chat_handler-0.1.4.dev2/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2780 2024-04-23 04:03:07.000000 streamlit_chat_handler-0.1.4.dev2/README.md
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-29 01:36:40.650458 streamlit_chat_handler-0.1.4.dev2/examples/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      728 2024-04-28 03:20:11.000000 streamlit_chat_handler-0.1.4.dev2/examples/template.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1291 2024-04-28 03:20:11.000000 streamlit_chat_handler-0.1.4.dev2/examples/template_expander.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1313 2024-04-29 01:36:22.000000 streamlit_chat_handler-0.1.4.dev2/pyproject.toml
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      363 2024-04-25 04:44:43.000000 streamlit_chat_handler-0.1.4.dev2/requirements.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2024-04-29 01:36:40.650458 streamlit_chat_handler-0.1.4.dev2/setup.cfg
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-29 01:36:40.650458 streamlit_chat_handler-0.1.4.dev2/streamlit_chat_handler/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      110 2024-04-23 00:45:47.000000 streamlit_chat_handler-0.1.4.dev2/streamlit_chat_handler/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    10838 2024-04-29 01:35:47.000000 streamlit_chat_handler-0.1.4.dev2/streamlit_chat_handler/_handler.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2281 2024-04-29 01:23:44.000000 streamlit_chat_handler-0.1.4.dev2/streamlit_chat_handler/types.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-29 01:36:40.650458 streamlit_chat_handler-0.1.4.dev2/streamlit_chat_handler.egg-info/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3737 2024-04-29 01:36:40.000000 streamlit_chat_handler-0.1.4.dev2/streamlit_chat_handler.egg-info/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      431 2024-04-29 01:36:40.000000 streamlit_chat_handler-0.1.4.dev2/streamlit_chat_handler.egg-info/SOURCES.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2024-04-29 01:36:40.000000 streamlit_chat_handler-0.1.4.dev2/streamlit_chat_handler.egg-info/dependency_links.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      279 2024-04-29 01:36:40.000000 streamlit_chat_handler-0.1.4.dev2/streamlit_chat_handler.egg-info/requires.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       42 2024-04-29 01:36:40.000000 streamlit_chat_handler-0.1.4.dev2/streamlit_chat_handler.egg-info/top_level.txt
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-29 01:38:28.737918 streamlit_chat_handler-0.1.4.dev3/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1083 2024-04-23 04:06:28.000000 streamlit_chat_handler-0.1.4.dev3/LICENSE
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3737 2024-04-29 01:38:28.737918 streamlit_chat_handler-0.1.4.dev3/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2780 2024-04-23 04:03:07.000000 streamlit_chat_handler-0.1.4.dev3/README.md
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-29 01:38:28.733918 streamlit_chat_handler-0.1.4.dev3/examples/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      728 2024-04-28 03:20:11.000000 streamlit_chat_handler-0.1.4.dev3/examples/template.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1291 2024-04-28 03:20:11.000000 streamlit_chat_handler-0.1.4.dev3/examples/template_expander.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1313 2024-04-29 01:38:03.000000 streamlit_chat_handler-0.1.4.dev3/pyproject.toml
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      363 2024-04-25 04:44:43.000000 streamlit_chat_handler-0.1.4.dev3/requirements.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2024-04-29 01:38:28.737918 streamlit_chat_handler-0.1.4.dev3/setup.cfg
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-29 01:38:28.733918 streamlit_chat_handler-0.1.4.dev3/streamlit_chat_handler/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      110 2024-04-23 00:45:47.000000 streamlit_chat_handler-0.1.4.dev3/streamlit_chat_handler/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    10840 2024-04-29 01:37:51.000000 streamlit_chat_handler-0.1.4.dev3/streamlit_chat_handler/_handler.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2281 2024-04-29 01:23:44.000000 streamlit_chat_handler-0.1.4.dev3/streamlit_chat_handler/types.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-29 01:38:28.733918 streamlit_chat_handler-0.1.4.dev3/streamlit_chat_handler.egg-info/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3737 2024-04-29 01:38:28.000000 streamlit_chat_handler-0.1.4.dev3/streamlit_chat_handler.egg-info/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      431 2024-04-29 01:38:28.000000 streamlit_chat_handler-0.1.4.dev3/streamlit_chat_handler.egg-info/SOURCES.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2024-04-29 01:38:28.000000 streamlit_chat_handler-0.1.4.dev3/streamlit_chat_handler.egg-info/dependency_links.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      279 2024-04-29 01:38:28.000000 streamlit_chat_handler-0.1.4.dev3/streamlit_chat_handler.egg-info/requires.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       42 2024-04-29 01:38:28.000000 streamlit_chat_handler-0.1.4.dev3/streamlit_chat_handler.egg-info/top_level.txt
```

### Comparing `streamlit_chat_handler-0.1.4.dev2/LICENSE` & `streamlit_chat_handler-0.1.4.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.1.4.dev2/PKG-INFO` & `streamlit_chat_handler-0.1.4.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_chat_handler
-Version: 0.1.4.dev2
+Version: 0.1.4.dev3
 Summary: ...
 Author-email: Eduardo Messias de Morais <emdemor415@gmail.com>
 Keywords: sample,setuptools,development
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit==1.33.0
```

### Comparing `streamlit_chat_handler-0.1.4.dev2/README.md` & `streamlit_chat_handler-0.1.4.dev3/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.1.4.dev2/examples/template.py` & `streamlit_chat_handler-0.1.4.dev3/examples/template.py`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.1.4.dev2/examples/template_expander.py` & `streamlit_chat_handler-0.1.4.dev3/examples/template_expander.py`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.1.4.dev2/pyproject.toml` & `streamlit_chat_handler-0.1.4.dev3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE.txt"}
 keywords = ["sample", "setuptools", "development"]
 authors = [
   {name = "Eduardo Messias de Morais", email = "emdemor415@gmail.com" },
 ]
-version = "0.1.4dev02"
+version = "0.1.4dev03"
 dynamic = ["dependencies"]
 
 [project.optional-dependencies]
 lint = [
     "black==23.7.0",
     "flake8==6.1.0",
     "Flake8-pyproject==1.2.3",
```

### Comparing `streamlit_chat_handler-0.1.4.dev2/streamlit_chat_handler/_handler.py` & `streamlit_chat_handler-0.1.4.dev3/streamlit_chat_handler/_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     def append_multiple(
         self, elements: list[StreamlitChatElement], render: bool = False
     ) -> None:
         """Append multiple chat elements to the session state."""
 
         chat_element = OrderedDict({self._set_index(): element for element in elements})
 
-        for index, element in chat_element.items:
+        for index, element in chat_element.items():
             self.append(
                 role=element.role,
                 type=element.type,
                 content=element.content,
                 index=index,
                 render=False,  # Aqui, os componentes serão renderizados separadamente
                 parent=element.parent,
```

### Comparing `streamlit_chat_handler-0.1.4.dev2/streamlit_chat_handler/types.py` & `streamlit_chat_handler-0.1.4.dev3/streamlit_chat_handler/types.py`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.1.4.dev2/streamlit_chat_handler.egg-info/PKG-INFO` & `streamlit_chat_handler-0.1.4.dev3/streamlit_chat_handler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_chat_handler
-Version: 0.1.4.dev2
+Version: 0.1.4.dev3
 Summary: ...
 Author-email: Eduardo Messias de Morais <emdemor415@gmail.com>
 Keywords: sample,setuptools,development
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit==1.33.0
```

