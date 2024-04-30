# Comparing `tmp/streamlit_chat_handler-0.1.4.dev3.tar.gz` & `tmp/streamlit_chat_handler-0.1.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_chat_handler-0.1.4.dev3.tar", last modified: Mon Apr 29 01:38:28 2024, max compression
+gzip compressed data, was "streamlit_chat_handler-0.1.5.dev1.tar", last modified: Tue Apr 30 01:57:56 2024, max compression
```

## Comparing `streamlit_chat_handler-0.1.4.dev3.tar` & `streamlit_chat_handler-0.1.5.dev1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-29 01:38:28.737918 streamlit_chat_handler-0.1.4.dev3/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1083 2024-04-23 04:06:28.000000 streamlit_chat_handler-0.1.4.dev3/LICENSE
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3737 2024-04-29 01:38:28.737918 streamlit_chat_handler-0.1.4.dev3/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2780 2024-04-23 04:03:07.000000 streamlit_chat_handler-0.1.4.dev3/README.md
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-29 01:38:28.733918 streamlit_chat_handler-0.1.4.dev3/examples/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      728 2024-04-28 03:20:11.000000 streamlit_chat_handler-0.1.4.dev3/examples/template.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1291 2024-04-28 03:20:11.000000 streamlit_chat_handler-0.1.4.dev3/examples/template_expander.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1313 2024-04-29 01:38:03.000000 streamlit_chat_handler-0.1.4.dev3/pyproject.toml
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      363 2024-04-25 04:44:43.000000 streamlit_chat_handler-0.1.4.dev3/requirements.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2024-04-29 01:38:28.737918 streamlit_chat_handler-0.1.4.dev3/setup.cfg
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-29 01:38:28.733918 streamlit_chat_handler-0.1.4.dev3/streamlit_chat_handler/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      110 2024-04-23 00:45:47.000000 streamlit_chat_handler-0.1.4.dev3/streamlit_chat_handler/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    10840 2024-04-29 01:37:51.000000 streamlit_chat_handler-0.1.4.dev3/streamlit_chat_handler/_handler.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2281 2024-04-29 01:23:44.000000 streamlit_chat_handler-0.1.4.dev3/streamlit_chat_handler/types.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-29 01:38:28.733918 streamlit_chat_handler-0.1.4.dev3/streamlit_chat_handler.egg-info/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3737 2024-04-29 01:38:28.000000 streamlit_chat_handler-0.1.4.dev3/streamlit_chat_handler.egg-info/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      431 2024-04-29 01:38:28.000000 streamlit_chat_handler-0.1.4.dev3/streamlit_chat_handler.egg-info/SOURCES.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2024-04-29 01:38:28.000000 streamlit_chat_handler-0.1.4.dev3/streamlit_chat_handler.egg-info/dependency_links.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      279 2024-04-29 01:38:28.000000 streamlit_chat_handler-0.1.4.dev3/streamlit_chat_handler.egg-info/requires.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       42 2024-04-29 01:38:28.000000 streamlit_chat_handler-0.1.4.dev3/streamlit_chat_handler.egg-info/top_level.txt
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-30 01:57:56.429913 streamlit_chat_handler-0.1.5.dev1/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1083 2024-04-23 04:06:28.000000 streamlit_chat_handler-0.1.5.dev1/LICENSE
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3737 2024-04-30 01:57:56.429913 streamlit_chat_handler-0.1.5.dev1/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2780 2024-04-23 04:03:07.000000 streamlit_chat_handler-0.1.5.dev1/README.md
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-30 01:57:56.425913 streamlit_chat_handler-0.1.5.dev1/examples/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      728 2024-04-28 03:20:11.000000 streamlit_chat_handler-0.1.5.dev1/examples/template.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1291 2024-04-28 03:20:11.000000 streamlit_chat_handler-0.1.5.dev1/examples/template_expander.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1313 2024-04-30 01:56:42.000000 streamlit_chat_handler-0.1.5.dev1/pyproject.toml
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      363 2024-04-25 04:44:43.000000 streamlit_chat_handler-0.1.5.dev1/requirements.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2024-04-30 01:57:56.429913 streamlit_chat_handler-0.1.5.dev1/setup.cfg
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-30 01:57:56.425913 streamlit_chat_handler-0.1.5.dev1/streamlit_chat_handler/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      110 2024-04-23 00:45:47.000000 streamlit_chat_handler-0.1.5.dev1/streamlit_chat_handler/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    11551 2024-04-30 01:56:01.000000 streamlit_chat_handler-0.1.5.dev1/streamlit_chat_handler/_handler.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2310 2024-04-30 01:32:41.000000 streamlit_chat_handler-0.1.5.dev1/streamlit_chat_handler/types.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-30 01:57:56.425913 streamlit_chat_handler-0.1.5.dev1/streamlit_chat_handler.egg-info/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3737 2024-04-30 01:57:56.000000 streamlit_chat_handler-0.1.5.dev1/streamlit_chat_handler.egg-info/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      431 2024-04-30 01:57:56.000000 streamlit_chat_handler-0.1.5.dev1/streamlit_chat_handler.egg-info/SOURCES.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2024-04-30 01:57:56.000000 streamlit_chat_handler-0.1.5.dev1/streamlit_chat_handler.egg-info/dependency_links.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      279 2024-04-30 01:57:56.000000 streamlit_chat_handler-0.1.5.dev1/streamlit_chat_handler.egg-info/requires.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       42 2024-04-30 01:57:56.000000 streamlit_chat_handler-0.1.5.dev1/streamlit_chat_handler.egg-info/top_level.txt
```

### Comparing `streamlit_chat_handler-0.1.4.dev3/LICENSE` & `streamlit_chat_handler-0.1.5.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.1.4.dev3/PKG-INFO` & `streamlit_chat_handler-0.1.5.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_chat_handler
-Version: 0.1.4.dev3
+Version: 0.1.5.dev1
 Summary: ...
 Author-email: Eduardo Messias de Morais <emdemor415@gmail.com>
 Keywords: sample,setuptools,development
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit==1.33.0
```

### Comparing `streamlit_chat_handler-0.1.4.dev3/README.md` & `streamlit_chat_handler-0.1.5.dev1/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.1.4.dev3/examples/template.py` & `streamlit_chat_handler-0.1.5.dev1/examples/template.py`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.1.4.dev3/examples/template_expander.py` & `streamlit_chat_handler-0.1.5.dev1/examples/template_expander.py`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.1.4.dev3/pyproject.toml` & `streamlit_chat_handler-0.1.5.dev1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE.txt"}
 keywords = ["sample", "setuptools", "development"]
 authors = [
   {name = "Eduardo Messias de Morais", email = "emdemor415@gmail.com" },
 ]
-version = "0.1.4dev03"
+version = "0.1.5dev01"
 dynamic = ["dependencies"]
 
 [project.optional-dependencies]
 lint = [
     "black==23.7.0",
     "flake8==6.1.0",
     "Flake8-pyproject==1.2.3",
```

### Comparing `streamlit_chat_handler-0.1.4.dev3/streamlit_chat_handler/_handler.py` & `streamlit_chat_handler-0.1.5.dev1/streamlit_chat_handler/_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,24 +89,25 @@
             index: Optional; a unique identifier for the chat element. Automatically generated if not provided.
             render: Optional; if True, the message is rendered immediately.
 
         Raises:
             ValueError: If an unsupported type is provided.
         """
 
-        index = self._set_index(index)
+        index = self._set_index(index, chat_element)
 
         if not chat_element:
             chat_element = self._get_chat_element(
-                role,
-                type,
-                content,
-                parent,
-                parent_args,
-                parent_kwargs,
+                role=role,
+                type=type,
+                content=content,
+                parent=parent,
+                index=index,
+                parent_args=parent_args,
+                parent_kwargs=parent_kwargs,
                 *args,
                 **kwargs,
             )
 
         self.session_state[self.elements_label][index] = chat_element
 
         if render:
@@ -114,23 +115,23 @@
         return self
 
     def append_multiple(
         self, elements: list[StreamlitChatElement], render: bool = False
     ) -> None:
         """Append multiple chat elements to the session state."""
 
-        chat_element = OrderedDict({self._set_index(): element for element in elements})
+        chat_element = OrderedDict({self._set_index(chat_element=e): e for e in elements})
 
         for index, element in chat_element.items():
             self.append(
                 role=element.role,
                 type=element.type,
                 content=element.content,
                 index=index,
-                render=False,  # Aqui, os componentes serão renderizados separadamente
+                render=element.index,  # Aqui, os componentes serão renderizados separadamente
                 parent=element.parent,
                 parent_args=element.parent_args,
                 parent_kwargs=element.parent_kwargs,
             )
 
         if render:
             response = self._render_elements(chat_element)
@@ -157,34 +158,49 @@
         return self
 
     def _init_session_state(self) -> None:
         """Initialize the session state for storing chat elements if it doesn't already exist."""
         if self.elements_label not in self.session_state:
             self.session_state[self.elements_label] = OrderedDict({})
 
-    def _set_index(self, index: str | None = None) -> str:
+    def _set_index(self, index: str | None = None, chat_element: StreamlitChatElement | None = None) -> str:
         """Set the index for the chat element.
 
         Args:
             index: The index to set.
 
         Returns:
             The set index.
         """
+
+        index_was_passed = index is not None
+        element_was_passed = chat_element is not None
+        element_has_index = (chat_element.index is not None) if element_was_passed else False
+
+        if element_was_passed:
+            if index_was_passed and element_has_index and (index != chat_element.index):
+                raise ValueError(
+                    "Cannot pass both an index and a StreamlitChatElement with an index."
+                )
+
+        if element_has_index and not index_was_passed:
+            index = chat_element.index
+
         if index is None:
-            index = uuid.uuid4().hex
-            return f"{str(self.step_counter).zfill(6)}{index}"
+            return uuid.uuid4().hex
+    
         return index
 
     def _get_chat_element(
         self,
         role: Literal["user", "assistant"] = None,
         type: str = None,
         content: Any = None,
         parent: str | None = None,
+        index: str | None = None,
         parent_args: Tuple[Any, ...] = (),
         parent_kwargs: dict[str, Any] = {},
         *args,
         **kwargs,
     ):
         args_were_passed = all([_check_argument(arg) for arg in (role, type, content)])
 
@@ -192,14 +208,15 @@
             return StreamlitChatElement(
                 role=role,
                 type=type,
                 content=content,
                 parent=parent,
                 parent_args=parent_args,
                 parent_kwargs=parent_kwargs,
+                index=index,
                 args=args,
                 kwargs=kwargs,
             )
         else:
             raise ValueError("Missing required arguments for StreamlitChatElement.")
 
     def _render_elements(
```

### Comparing `streamlit_chat_handler-0.1.4.dev3/streamlit_chat_handler/types.py` & `streamlit_chat_handler-0.1.5.dev1/streamlit_chat_handler/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     Methods:
         render: Render the chat element using the specified Streamlit widget.
     """
     role: Literal["user", "assistant"]
     type: str
     content: Any
     parent: str | None = None
+    index: str | None = None
     args: List[Any] = Field(default_factory=list)
     kwargs: Dict[str, Any] = Field(default_factory=dict)
     parent_args: List[Any] | None = None
     parent_kwargs: Dict[str, Any] | None = None
 
     def render(self):
         """Render the chat element using the specified Streamlit widget.
```

### Comparing `streamlit_chat_handler-0.1.4.dev3/streamlit_chat_handler.egg-info/PKG-INFO` & `streamlit_chat_handler-0.1.5.dev1/streamlit_chat_handler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_chat_handler
-Version: 0.1.4.dev3
+Version: 0.1.5.dev1
 Summary: ...
 Author-email: Eduardo Messias de Morais <emdemor415@gmail.com>
 Keywords: sample,setuptools,development
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit==1.33.0
```

