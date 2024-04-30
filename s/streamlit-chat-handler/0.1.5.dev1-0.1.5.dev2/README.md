# Comparing `tmp/streamlit_chat_handler-0.1.5.dev1.tar.gz` & `tmp/streamlit_chat_handler-0.1.5.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_chat_handler-0.1.5.dev1.tar", last modified: Tue Apr 30 01:57:56 2024, max compression
+gzip compressed data, was "streamlit_chat_handler-0.1.5.dev2.tar", last modified: Tue Apr 30 03:31:26 2024, max compression
```

## Comparing `streamlit_chat_handler-0.1.5.dev1.tar` & `streamlit_chat_handler-0.1.5.dev2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-30 01:57:56.429913 streamlit_chat_handler-0.1.5.dev1/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1083 2024-04-23 04:06:28.000000 streamlit_chat_handler-0.1.5.dev1/LICENSE
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3737 2024-04-30 01:57:56.429913 streamlit_chat_handler-0.1.5.dev1/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2780 2024-04-23 04:03:07.000000 streamlit_chat_handler-0.1.5.dev1/README.md
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-30 01:57:56.425913 streamlit_chat_handler-0.1.5.dev1/examples/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      728 2024-04-28 03:20:11.000000 streamlit_chat_handler-0.1.5.dev1/examples/template.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1291 2024-04-28 03:20:11.000000 streamlit_chat_handler-0.1.5.dev1/examples/template_expander.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1313 2024-04-30 01:56:42.000000 streamlit_chat_handler-0.1.5.dev1/pyproject.toml
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      363 2024-04-25 04:44:43.000000 streamlit_chat_handler-0.1.5.dev1/requirements.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2024-04-30 01:57:56.429913 streamlit_chat_handler-0.1.5.dev1/setup.cfg
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-30 01:57:56.425913 streamlit_chat_handler-0.1.5.dev1/streamlit_chat_handler/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      110 2024-04-23 00:45:47.000000 streamlit_chat_handler-0.1.5.dev1/streamlit_chat_handler/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    11551 2024-04-30 01:56:01.000000 streamlit_chat_handler-0.1.5.dev1/streamlit_chat_handler/_handler.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2310 2024-04-30 01:32:41.000000 streamlit_chat_handler-0.1.5.dev1/streamlit_chat_handler/types.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-30 01:57:56.425913 streamlit_chat_handler-0.1.5.dev1/streamlit_chat_handler.egg-info/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3737 2024-04-30 01:57:56.000000 streamlit_chat_handler-0.1.5.dev1/streamlit_chat_handler.egg-info/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      431 2024-04-30 01:57:56.000000 streamlit_chat_handler-0.1.5.dev1/streamlit_chat_handler.egg-info/SOURCES.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2024-04-30 01:57:56.000000 streamlit_chat_handler-0.1.5.dev1/streamlit_chat_handler.egg-info/dependency_links.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      279 2024-04-30 01:57:56.000000 streamlit_chat_handler-0.1.5.dev1/streamlit_chat_handler.egg-info/requires.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       42 2024-04-30 01:57:56.000000 streamlit_chat_handler-0.1.5.dev1/streamlit_chat_handler.egg-info/top_level.txt
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-30 03:31:26.792349 streamlit_chat_handler-0.1.5.dev2/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1083 2024-04-23 04:06:28.000000 streamlit_chat_handler-0.1.5.dev2/LICENSE
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3737 2024-04-30 03:31:26.792349 streamlit_chat_handler-0.1.5.dev2/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2780 2024-04-23 04:03:07.000000 streamlit_chat_handler-0.1.5.dev2/README.md
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-30 03:31:26.788349 streamlit_chat_handler-0.1.5.dev2/examples/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      728 2024-04-28 03:20:11.000000 streamlit_chat_handler-0.1.5.dev2/examples/template.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1291 2024-04-28 03:20:11.000000 streamlit_chat_handler-0.1.5.dev2/examples/template_expander.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1313 2024-04-30 03:31:19.000000 streamlit_chat_handler-0.1.5.dev2/pyproject.toml
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      363 2024-04-25 04:44:43.000000 streamlit_chat_handler-0.1.5.dev2/requirements.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2024-04-30 03:31:26.792349 streamlit_chat_handler-0.1.5.dev2/setup.cfg
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-30 03:31:26.788349 streamlit_chat_handler-0.1.5.dev2/streamlit_chat_handler/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      110 2024-04-23 00:45:47.000000 streamlit_chat_handler-0.1.5.dev2/streamlit_chat_handler/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    12371 2024-04-30 03:30:32.000000 streamlit_chat_handler-0.1.5.dev2/streamlit_chat_handler/_handler.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2629 2024-04-30 03:26:43.000000 streamlit_chat_handler-0.1.5.dev2/streamlit_chat_handler/types.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-30 03:31:26.788349 streamlit_chat_handler-0.1.5.dev2/streamlit_chat_handler.egg-info/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3737 2024-04-30 03:31:26.000000 streamlit_chat_handler-0.1.5.dev2/streamlit_chat_handler.egg-info/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      431 2024-04-30 03:31:26.000000 streamlit_chat_handler-0.1.5.dev2/streamlit_chat_handler.egg-info/SOURCES.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2024-04-30 03:31:26.000000 streamlit_chat_handler-0.1.5.dev2/streamlit_chat_handler.egg-info/dependency_links.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      279 2024-04-30 03:31:26.000000 streamlit_chat_handler-0.1.5.dev2/streamlit_chat_handler.egg-info/requires.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       42 2024-04-30 03:31:26.000000 streamlit_chat_handler-0.1.5.dev2/streamlit_chat_handler.egg-info/top_level.txt
```

### Comparing `streamlit_chat_handler-0.1.5.dev1/LICENSE` & `streamlit_chat_handler-0.1.5.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.1.5.dev1/PKG-INFO` & `streamlit_chat_handler-0.1.5.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_chat_handler
-Version: 0.1.5.dev1
+Version: 0.1.5.dev2
 Summary: ...
 Author-email: Eduardo Messias de Morais <emdemor415@gmail.com>
 Keywords: sample,setuptools,development
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit==1.33.0
```

### Comparing `streamlit_chat_handler-0.1.5.dev1/README.md` & `streamlit_chat_handler-0.1.5.dev2/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.1.5.dev1/examples/template.py` & `streamlit_chat_handler-0.1.5.dev2/examples/template.py`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.1.5.dev1/examples/template_expander.py` & `streamlit_chat_handler-0.1.5.dev2/examples/template_expander.py`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.1.5.dev1/pyproject.toml` & `streamlit_chat_handler-0.1.5.dev2/pyproject.toml`

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
-version = "0.1.5dev01"
+version = "0.1.5dev02"
 dynamic = ["dependencies"]
 
 [project.optional-dependencies]
 lint = [
     "black==23.7.0",
     "flake8==6.1.0",
     "Flake8-pyproject==1.2.3",
```

### Comparing `streamlit_chat_handler-0.1.5.dev1/streamlit_chat_handler/_handler.py` & `streamlit_chat_handler-0.1.5.dev2/streamlit_chat_handler/_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, List, Literal, Tuple
 from collections import OrderedDict
 
 import streamlit as st
 from loguru import logger
 from streamlit.runtime.state.session_state_proxy import SessionStateProxy
 
-from streamlit_chat_handler.types import StreamlitChatElement
+from streamlit_chat_handler.types import StreamlitChatElement, UserFeedback
 
 
 class StreamlitChatHandler:
     """Handles the state and rendering of chat elements within a Streamlit session.
 
     This class manages chat elements in a Streamlit application, allowing for creating,
     storing, and rendering user and assistant messages dynamically. It uses a singleton pattern
@@ -149,15 +149,15 @@
         """Render the last added chat element."""
         last_key, last_element = _get_last_item(self.session_state[self.elements_label])
         self.rendered_elements[last_key] = last_element.render()
 
     def render(self) -> "StreamlitChatHandler":
         """Render all chat elements in the session."""
         self.rendered_elements = self._render_elements(
-            self.session_state[self.elements_label]
+            self.session_state[self.elements_label],
         )
         return self
 
     def _init_session_state(self) -> None:
         """Initialize the session state for storing chat elements if it doesn't already exist."""
         if self.elements_label not in self.session_state:
             self.session_state[self.elements_label] = OrderedDict({})
@@ -235,36 +235,53 @@
         if isinstance(chat_element, StreamlitChatElement):
             chat_element = OrderedDict({self._set_index(): chat_element})
 
         chat_element_list = [v for v in chat_element.values()]
         element_groups = _group_elements_by_role(chat_element_list)
 
         response = OrderedDict({})
+        feedback = OrderedDict({})
         count = 0
         for element_list in element_groups:
             role = element_list[0].role
             chat_message = st.chat_message(role)
+            last_index = None
             for element in element_list:
                 try:
                     parent = (
                         getattr(chat_message, element.parent)(
                             *element.parent_args, **element.parent_kwargs
                         )
                         if element.parent
                         else chat_message
                     )
-                    response[list(chat_element)[count]] = getattr(parent, element.type)(
+                    last_index = list(chat_element)[count]
+                    response[last_index] = getattr(parent, element.type)(
                         element.content, *element.args, **element.kwargs
                     )
+
                 except Exception as err:
                     logger.warning(
                         f"Error rendering element {element} in key {list(chat_element)[count]}: {err}"
                     )
                 count += 1
 
+            if last_index and (role == "assistant"):
+                *_, cont = st.columns([5,2])
+                comments_popover = cont.popover("**⯌ Avalie**")
+                comment_text = comments_popover.text_input(label="**Insira seu comentário** *(opcional)*")
+                col1, col2, col3 = comments_popover.columns([6, 1, 1])
+                positive_button = col2.button("**🖒**", type="primary")
+                negative_button = col3.button("**🖓**")
+                feedback[last_index] = UserFeedback(
+                    positive_button=positive_button,
+                    negative_button=negative_button,
+                    comment=comment_text,
+                )
+
         return response
 
 
 def _get_last_item(ordered_dict: OrderedDict) -> Tuple[str, Any]:
     """Retrieve the last key-value pair from an OrderedDict.
 
     This function fetches the last key and its corresponding value from an OrderedDict
```

### Comparing `streamlit_chat_handler-0.1.5.dev1/streamlit_chat_handler/types.py` & `streamlit_chat_handler-0.1.5.dev2/streamlit_chat_handler/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from pydantic import BaseModel, Field
 from typing import Any, Literal, List, Dict
 
 import streamlit as st
+from collections import OrderedDict
 
 
 class StreamlitChatElement(BaseModel):
     """Represents a chat element within a Streamlit application, handling its rendering.
 
     This model defines a chat element's role (user or assistant), type (e.g., 'text', 'image'), 
     and content along with any additional arguments or keyword arguments used in rendering 
@@ -45,7 +46,17 @@
             # Assuming an instance `chat_element` with type 'text':
             chat_element.render()  # This would render the content using `st.text()`.
         """
 
         chat_message = st.chat_message(self.role)
         _parent = getattr(chat_message, self.parent)(*self.parent_args, **self.parent_kwargs) if self.parent else chat_message
         return getattr(_parent, self.type)(self.content, *self.args, **self.kwargs)
+
+
+class UserFeedback(BaseModel):
+    positive_button: str | None = None
+    negative_button: str | None = None
+    comment: str | None = None
+
+class StreamlitRenderResponse(BaseModel):
+    rendered_elements: OrderedDict[str, Any]
+    feedback_metadata: OrderedDict[str, UserFeedback]
```

### Comparing `streamlit_chat_handler-0.1.5.dev1/streamlit_chat_handler.egg-info/PKG-INFO` & `streamlit_chat_handler-0.1.5.dev2/streamlit_chat_handler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_chat_handler
-Version: 0.1.5.dev1
+Version: 0.1.5.dev2
 Summary: ...
 Author-email: Eduardo Messias de Morais <emdemor415@gmail.com>
 Keywords: sample,setuptools,development
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit==1.33.0
```

