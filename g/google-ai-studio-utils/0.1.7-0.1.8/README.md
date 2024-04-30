# Comparing `tmp/google_ai_studio_utils-0.1.7.tar.gz` & `tmp/google_ai_studio_utils-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_ai_studio_utils-0.1.7.tar", max compression
+gzip compressed data, was "google_ai_studio_utils-0.1.8.tar", max compression
```

## Comparing `google_ai_studio_utils-0.1.7.tar` & `google_ai_studio_utils-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0       24 2024-04-15 15:56:31.370705 google_ai_studio_utils-0.1.7/README.md
--rw-r--r--   0        0        0      188 2024-04-17 01:59:04.520871 google_ai_studio_utils-0.1.7/google_ai_studio_utils/config.py
--rwxr-xr-x   0        0        0     2916 2024-04-15 17:01:31.595230 google_ai_studio_utils-0.1.7/google_ai_studio_utils/google_ai_studio_conversation_csv_to_html.py
--rw-r--r--   0        0        0     5305 2024-04-15 17:02:05.628767 google_ai_studio_utils-0.1.7/google_ai_studio_utils/templates/google-ai-studio-conversation.html
--rw-r--r--   0        0        0     2740 2024-04-22 21:32:53.381446 google_ai_studio_utils-0.1.7/google_ai_studio_utils/utils.py
--rw-r--r--   0        0        0      827 2024-04-22 21:33:06.144183 google_ai_studio_utils-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 google_ai_studio_utils-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       24 2024-04-15 15:56:31.370705 google_ai_studio_utils-0.1.8/README.md
+-rw-r--r--   0        0        0      188 2024-04-17 01:59:04.520871 google_ai_studio_utils-0.1.8/google_ai_studio_utils/config.py
+-rwxr-xr-x   0        0        0     2916 2024-04-15 17:01:31.595230 google_ai_studio_utils-0.1.8/google_ai_studio_utils/google_ai_studio_conversation_csv_to_html.py
+-rwxr-xr-x   0        0        0     3145 2024-04-30 15:01:04.901844 google_ai_studio_utils-0.1.8/google_ai_studio_utils/google_ai_studio_conversation_python_to_html.py
+-rw-r--r--   0        0        0     5305 2024-04-15 17:02:05.628767 google_ai_studio_utils-0.1.8/google_ai_studio_utils/templates/google-ai-studio-conversation.html
+-rw-r--r--   0        0        0     5230 2024-04-30 15:18:47.363938 google_ai_studio_utils-0.1.8/google_ai_studio_utils/utils.py
+-rw-r--r--   0        0        0      915 2024-04-30 15:19:20.828045 google_ai_studio_utils-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 google_ai_studio_utils-0.1.8/PKG-INFO
```

### Comparing `google_ai_studio_utils-0.1.7/google_ai_studio_utils/google_ai_studio_conversation_csv_to_html.py` & `google_ai_studio_utils-0.1.8/google_ai_studio_utils/google_ai_studio_conversation_csv_to_html.py`

 * *Files identical despite different names*

### Comparing `google_ai_studio_utils-0.1.7/google_ai_studio_utils/templates/google-ai-studio-conversation.html` & `google_ai_studio_utils-0.1.8/google_ai_studio_utils/templates/google-ai-studio-conversation.html`

 * *Files identical despite different names*

### Comparing `google_ai_studio_utils-0.1.7/pyproject.toml` & `google_ai_studio_utils-0.1.8/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "google-ai-studio-utils"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/tddschn/google-ai-studio-utils"
 repository = "https://github.com/tddschn/google-ai-studio-utils"
 classifiers = ["Topic :: Utilities"]
 keywords = ["chatgpt"]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/tddschn/google-ai-studio-utils/issues"
 [tool.poetry.scripts]
-gai2html = "google_ai_studio_utils.google_ai_studio_conversation_csv_to_html:main"
+# gai2html = "google_ai_studio_utils.google_ai_studio_conversation_csv_to_html:main"
+gai2html = "google_ai_studio_utils.google_ai_studio_conversation_python_to_html:main"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <4.0"
 pyperclip = "^1.8.2"
 markdown = "^3.6"
```

### Comparing `google_ai_studio_utils-0.1.7/PKG-INFO` & `google_ai_studio_utils-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-ai-studio-utils
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Home-page: https://github.com/tddschn/google-ai-studio-utils
 License: MIT
 Keywords: chatgpt
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
```

