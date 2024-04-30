# Comparing `tmp/tsbot-1.1.0.tar.gz` & `tmp/tsbot-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsbot-1.1.0.tar", last modified: Fri Apr 19 00:19:20 2024, max compression
+gzip compressed data, was "tsbot-1.1.1.tar", last modified: Tue Apr 30 15:45:09 2024, max compression
```

## Comparing `tsbot-1.1.0.tar` & `tsbot-1.1.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:19:20.714462 tsbot-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-19 00:19:04.000000 tsbot-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-19 00:19:20.714462 tsbot-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-19 00:19:04.000000 tsbot-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-19 00:19:04.000000 tsbot-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 00:19:20.714462 tsbot-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:19:20.706462 tsbot-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-04-19 00:19:04.000000 tsbot-1.1.0/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-19 00:19:04.000000 tsbot-1.1.0/tests/test_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-19 00:19:04.000000 tsbot-1.1.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-04-19 00:19:04.000000 tsbot-1.1.0/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-04-19 00:19:04.000000 tsbot-1.1.0/tests/test_query_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-19 00:19:04.000000 tsbot-1.1.0/tests/test_ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-19 00:19:04.000000 tsbot-1.1.0/tests/test_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:19:20.706462 tsbot-1.1.0/tsbot/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17921 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:19:20.710462 tsbot-1.1.0/tsbot/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/commands/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/commands/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:19:20.710462 tsbot-1.1.0/tsbot/default_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/default_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/default_plugins/help.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/default_plugins/keepalive.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:19:20.710462 tsbot-1.1.0/tsbot/events/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/events/event.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/events/event_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/events/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:19:20.710462 tsbot-1.1.0/tsbot/query_builder/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/query_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/query_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/query_builder/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:19:20.710462 tsbot-1.1.0/tsbot/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/tasks/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/tasks/task.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:19:20.710462 tsbot-1.1.0/tsbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-19 00:19:20.000000 tsbot-1.1.0/tsbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-19 00:19:20.000000 tsbot-1.1.0/tsbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 00:19:20.000000 tsbot-1.1.0/tsbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-19 00:19:20.000000 tsbot-1.1.0/tsbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 00:19:20.000000 tsbot-1.1.0/tsbot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:45:09.046346 tsbot-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-30 15:45:05.000000 tsbot-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-30 15:45:09.046346 tsbot-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-30 15:45:05.000000 tsbot-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-30 15:45:05.000000 tsbot-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:45:09.046346 tsbot-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:45:09.038346 tsbot-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-04-30 15:45:05.000000 tsbot-1.1.1/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-30 15:45:05.000000 tsbot-1.1.1/tests/test_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-30 15:45:05.000000 tsbot-1.1.1/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-04-30 15:45:05.000000 tsbot-1.1.1/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-04-30 15:45:05.000000 tsbot-1.1.1/tests/test_query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-30 15:45:05.000000 tsbot-1.1.1/tests/test_ratelimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-30 15:45:05.000000 tsbot-1.1.1/tests/test_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:45:09.042346 tsbot-1.1.1/tsbot/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17920 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:45:09.042346 tsbot-1.1.1/tsbot/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/commands/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:45:09.042346 tsbot-1.1.1/tsbot/default_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/default_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/default_plugins/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/default_plugins/keepalive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:45:09.042346 tsbot-1.1.1/tsbot/events/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/events/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/events/event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/events/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:45:09.046346 tsbot-1.1.1/tsbot/query_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/query_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/query_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/query_builder/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/ratelimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:45:09.046346 tsbot-1.1.1/tsbot/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/tasks/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/tasks/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:45:09.046346 tsbot-1.1.1/tsbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-30 15:45:09.000000 tsbot-1.1.1/tsbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-30 15:45:09.000000 tsbot-1.1.1/tsbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:45:09.000000 tsbot-1.1.1/tsbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-30 15:45:09.000000 tsbot-1.1.1/tsbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 15:45:09.000000 tsbot-1.1.1/tsbot.egg-info/top_level.txt
```

### Comparing `tsbot-1.1.0/LICENSE` & `tsbot-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.0/PKG-INFO` & `tsbot-1.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: tsbot
-Version: 1.1.0
+Version: 1.1.1
 Summary: Asynchronous framework to build TeamSpeak 3 Server Query bots
 Author: 0x4aK
 Project-URL: repository, https://github.com/0x4aK/tsbot
 Project-URL: documentation, https://tsbot.readthedocs.io/en/latest/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: asyncssh>=2.9.0
+Requires-Dist: asyncssh==2.14.0
 Provides-Extra: tests
-Requires-Dist: mypy>=0.931; extra == "tests"
-Requires-Dist: pytest>=7.0.0; extra == "tests"
-Requires-Dist: pytest-cov>=3.0.0; extra == "tests"
+Requires-Dist: mypy>=1.9.0; extra == "tests"
+Requires-Dist: pytest==8.1.1; extra == "tests"
+Requires-Dist: pytest-cov==5.0.0; extra == "tests"
 Provides-Extra: docs
-Requires-Dist: sphinx>=7.2.6; extra == "docs"
-Requires-Dist: myst-parser>=0.18.0; extra == "docs"
-Requires-Dist: sphinx-autodoc-typehints>=1.18.2; extra == "docs"
-Requires-Dist: sphinx-autobuild>=2021.3.14; extra == "docs"
+Requires-Dist: sphinx>=7.3.7; extra == "docs"
+Requires-Dist: myst-parser>=2.0.0; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints>=2.1.0; extra == "docs"
+Requires-Dist: sphinx-autobuild>=2024.4.16; extra == "docs"
 Requires-Dist: sphinx_rtd_theme>=2.0.0; extra == "docs"
 
 # TSBot
 
 Asynchronous framework to build **TeamSpeak 3 Server Query** bots
 
 ## ✅ Features
```

### Comparing `tsbot-1.1.0/README.md` & `tsbot-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.0/pyproject.toml` & `tsbot-1.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 [project]
 name = "tsbot"
-version = "1.1.0"
+version = "1.1.1"
 authors = [{ name = "0x4aK" }]
 description = "Asynchronous framework to build TeamSpeak 3 Server Query bots"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: AsyncIO",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
 ]
-dependencies = ["asyncssh >= 2.9.0"]
+dependencies = ["asyncssh == 2.14.0"]
 license = { file = "LICENCE" }
 urls = { repository = "https://github.com/0x4aK/tsbot", documentation = "https://tsbot.readthedocs.io/en/latest/" }
 
 
 [project.optional-dependencies]
-tests = ["mypy >= 0.931", "pytest >= 7.0.0", "pytest-cov >= 3.0.0"]
+tests = ["mypy >= 1.9.0", "pytest == 8.1.1", "pytest-cov == 5.0.0"]
 docs = [
-    "sphinx >= 7.2.6",
-    "myst-parser >= 0.18.0",
-    "sphinx-autodoc-typehints >= 1.18.2",
-    "sphinx-autobuild >= 2021.3.14",
+    "sphinx >= 7.3.7",
+    "myst-parser >= 2.0.0",
+    "sphinx-autodoc-typehints >= 2.1.0",
+    "sphinx-autobuild >= 2024.4.16",
     "sphinx_rtd_theme >= 2.0.0",
 ]
 
 
 [build-system]
-requires = ["setuptools>=42", "wheel"]
+requires = ["setuptools >= 69.5.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [tool.setuptools]
 packages = { find = { include = ["tsbot*"] } }
```

### Comparing `tsbot-1.1.0/tests/test_connection.py` & `tsbot-1.1.1/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.0/tests/test_encoders.py` & `tsbot-1.1.1/tests/test_encoders.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.0/tests/test_parsers.py` & `tsbot-1.1.1/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.0/tests/test_query_builder.py` & `tsbot-1.1.1/tests/test_query_builder.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.0/tests/test_ratelimiter.py` & `tsbot-1.1.1/tests/test_ratelimiter.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.0/tests/test_response.py` & `tsbot-1.1.1/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.0/tsbot/bot.py` & `tsbot-1.1.1/tsbot/bot.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,24 +81,24 @@
         self._query_timeout = query_timeout
 
     def emit(self, event_name: str, ctx: Any | None = None) -> None:
         """
         Creates :class:`TSevent<tsbot.events.TSEvent>` instance and emits it.
 
         :param event_name: Name of the event being emitted.
-        :param ctx: Addittional context for the event.
+        :param ctx: Additional context for the event.
         """
         event = events.TSEvent(event=event_name, ctx=ctx)
         self.emit_event(event)
 
     def emit_event(self, event: events.TSEvent) -> None:
         """
         Emits an event to be handled.
 
-        :param event: Event to be emmitted.
+        :param event: Event to be emitted.
         """
         self._event_handler.add_event(event)
 
     def on(self, event_type: str) -> Callable[[events.TEventHandler], events.TEventHandler]:
         """
         Decorator to register event handlers.
 
@@ -114,15 +114,15 @@
     def register_event_handler(
         self, event_type: str, handler: events.TEventHandler
     ) -> events.TSEventHandler:
         """
         Register an event handler to be ran on an event.
 
         :param event_type: Name of the event.
-        :param handler: async function to handle the event.
+        :param handler: Async function to handle the event.
         :return: The instance of :class:`TSEventHandler<tsbot.events.TSEventHandler>` created.
         """
 
         event_handler = events.TSEventHandler(event_type, handler)
         self._event_handler.register_event_handler(event_handler)
         return event_handler
 
@@ -142,15 +142,15 @@
     def register_once_handler(
         self, event_type: str, handler: events.TEventHandler
     ) -> events.TSEventOnceHandler:
         """
         Register an event handler to be ran once on an event.
 
         :param event_type: Name of the event.
-        :param handler: async function to handle the event.
+        :param handler: Async function to handle the event.
         :return: The instance of :class:`TSEventOnceHandler<tsbot.events.TSEventOnceHandler>` created.
         """
 
         event_handler = events.TSEventOnceHandler(event_type, handler, self._event_handler)
         self._event_handler.register_event_handler(event_handler)
         return event_handler
 
@@ -230,15 +230,15 @@
         """
         self._command_handler.remove_command(command)
 
     def get_command_handler(self, command: str) -> commands.TSCommand | None:
         """
         Get :class:`TSCommand<tsbot.commands.TSCommand>` instance associated with a given `str`
 
-        :param command: command that invokes :class:`TSCommand<tsbot.commands.TSCommand>`
+        :param command: Command that invokes :class:`TSCommand<tsbot.commands.TSCommand>`
         :return: :class:`TSCommand<tsbot.commands.TSCommand>` associated with `command`
         """
         return self._command_handler.commands.get(command)
 
     def register_every_task(
         self,
         seconds: float,
@@ -246,15 +246,15 @@
         *,
         name: str | None = None,
     ) -> tasks.TSTask:
         """
         Register task handler to be ran every given second.
 
         :param seconds: How often the task is executed.
-        :param handler: async function to be called when the task is executed.
+        :param handler: Async function to be called when the task is executed.
         :param name: Name of the task.
         :return: Instance of :class:`TSTask<tsbot.tasks.TSTask>` created.
         """
         task = tasks.TSTask(handler=tasks.every(handler, seconds), name=name)
         self._tasks_handler.register_task(self, task)
         return task
 
@@ -263,15 +263,15 @@
         handler: tasks.TTaskHandler,
         *,
         name: str | None = None,
     ) -> tasks.TSTask:
         """
         Register task handler as a background task.
 
-        :param handler: async function to be called when the task is executed.
+        :param handler: Async function to be called when the task is executed.
         :param name: Name of the task.
         :return: Instance of :class:`TSTask<tsbot.tasks.TSTask>` created.
         """
 
         task = tasks.TSTask(handler=handler, name=name)
         self._tasks_handler.register_task(self, task)
         return task
@@ -299,24 +299,24 @@
     async def send_raw(self, raw_query: str) -> response.TSResponse:
         """
         Sends raw commands to the server.
 
         Its recommended to use built-in query builder and
         :func:`send()<tsbot.TSBot.send()>` method instead.
 
-        :param raw_query: raw query command to be send to the server.
+        :param raw_query: Raw query command to be send to the server.
         :return: Response from the server.
         """
         try:
             return await asyncio.shield(self._send(raw_query))
         except exceptions.TSResponseError as response_error:
             raise utils.pop_traceback(response_error, 2)
 
     async def _send(self, raw_query: str) -> response.TSResponse:
-        """Method responsibe for actually sending the data."""
+        """Method responsible for actually sending the data."""
 
         async with self._sending_lock:
             self._response = asyncio.Future()
 
             if self._ratelimited:
                 await self._ratelimiter.wait()
```

### Comparing `tsbot-1.1.0/tsbot/commands/handler.py` & `tsbot-1.1.1/tsbot/commands/handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,19 +21,25 @@
 
 class CommandHandler:
     def __init__(self, invoker: str = "!") -> None:
         self.invoker = invoker
         self.commands: dict[str, commands.TSCommand] = {}
 
     def register_command(self, command: commands.TSCommand) -> None:
+        if already_registered := tuple(filter(lambda c: c in self.commands, command.commands)):
+            logger.warn(
+                "Command %s are already registered and will be overwritten",
+                ", ".join(map(repr, already_registered)),
+            )
+
         self.commands.update({c: command for c in command.commands})
 
         logger.debug(
             "Registered %s command to execute handler %r",
-            ", ".join(repr(c) for c in command.commands),
+            ", ".join(map(repr, command.commands)),
             command.handler.__name__,
         )
 
     def remove_command(self, command: commands.TSCommand) -> None:
         for c in command.commands:
             del self.commands[c]
```

### Comparing `tsbot-1.1.0/tsbot/connection.py` & `tsbot-1.1.1/tsbot/connection.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import itertools
 import logging
 from typing import AsyncGenerator
 
 import asyncssh
 
 logger = logging.getLogger(__name__)
 
@@ -39,18 +40,17 @@
         if self._connection:
             self._connection.close()
             await self._connection.wait_closed()
 
         logger.info("Connection closed")
 
     async def read_lines(self, number_of_lines: int = 1) -> AsyncGenerator[str, None]:
-        lines_read = 0
+        count = itertools.count()
 
-        while lines_read < number_of_lines and (data := await self._read()) is not None:
-            lines_read += 1
+        while next(count) < number_of_lines and (data := await self._read()) is not None:
             yield data
 
     async def read(self) -> AsyncGenerator[str, None]:
         while (data := await self._read()) is not None:
             yield data
 
         logger.debug("Reading done")
```

### Comparing `tsbot-1.1.0/tsbot/default_plugins/keepalive.py` & `tsbot-1.1.1/tsbot/default_plugins/keepalive.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             self.command_sent_event.clear()
             try:
                 await asyncio.wait_for(
                     asyncio.shield(self.command_sent_event.wait()),
                     timeout=self.KEEP_ALIVE_INTERVAL,
                 )
             except asyncio.TimeoutError:
-                logger.debug("Sengind keep-alive")
+                logger.debug("Sending keep-alive")
                 await bot.send_raw(self.KEEP_ALIVE_COMMAND)
 
             except asyncio.CancelledError:
                 logger.debug("Keep-alive task cancelled")
                 break
 
     @plugin.on("send")
```

### Comparing `tsbot-1.1.0/tsbot/encoders.py` & `tsbot-1.1.1/tsbot/encoders.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.0/tsbot/events/event.py` & `tsbot-1.1.1/tsbot/events/event.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.0/tsbot/events/event_handler.py` & `tsbot-1.1.1/tsbot/events/event_handler.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.0/tsbot/events/handler.py` & `tsbot-1.1.1/tsbot/events/handler.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.0/tsbot/exceptions.py` & `tsbot-1.1.1/tsbot/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
     def __str__(self) -> str:
         return f"Error {self.error_id}: {self.msg}"
 
 
 class TSResponsePermissionError(TSResponseError):
     """
-    Raised when a response has error_id of '2568', idicating that the client
-    doesn't have the propper permissions to execute this query.
+    Raised when a response has error_id of '2568', indicating that the client
+    doesn't have the proper permissions to execute this query.
     """
 
     def __init__(self, msg: str, error_id: int, perm_id: int) -> None:
         super().__init__(msg, error_id)
         self.perm_id = perm_id
 
     def __str__(self) -> str:
```

### Comparing `tsbot-1.1.0/tsbot/parsers.py` & `tsbot-1.1.1/tsbot/parsers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from __future__ import annotations
 
+import itertools
+
 from tsbot import encoders
 
 KWARG_INDICATOR = "-"
+QUOTES = ('"', "'")
 
 
 def parse_data(input_str: str) -> tuple[dict[str, str], ...]:
     if not input_str:
         return tuple()
 
     return tuple(map(parse_line, input_str.split("|")))
@@ -18,26 +21,29 @@
 
     return dict(map(parse_value, input_str.split(" ")))
 
 
 def parse_value(input_str: str) -> tuple[str, str]:
     key, _, value = input_str.partition("=")
 
+    if not value:
+        return key, ""
+
     if "|" in value:
         # Multiple values associated with the key. Making values comma separated
         return key, ",".join(map(encoders.unescape, value.split(f"|{key}=")))
 
-    return key, encoders.unescape(value) if value else ""
+    return key, encoders.unescape(value)
 
 
 def _parse_quoted_arg(unparsed: str) -> tuple[str, str]:
     """
     Parses a quoted argument, returns it and unparsed part.
 
-    If a qoute doesn't have a whitespace behind it, that part is not considered a quote end.
+    If a quote doesn't have a whitespace behind it, that part is not considered a quote end.
     If a valid quote is not found, parse as normal argument.
     """
     quote, unparsed_len = unparsed[0], len(unparsed)
 
     if (quote_end := unparsed.find(quote, 1)) < 0:
         return _parse_arg(unparsed)
 
@@ -46,27 +52,27 @@
             return _parse_arg(unparsed)
 
     return unparsed[1:quote_end], unparsed[quote_end + 1 :].lstrip()
 
 
 def _parse_arg(unparsed: str) -> tuple[str, str]:
     """Parse an argument out of unparsed message, return it and unparsed part."""
-    arg, unparsed = d if len(d := unparsed.split(maxsplit=1)) > 1 else (d[0] if d else "", "")
+    arg, unparsed = (*unparsed.split(maxsplit=1), *itertools.repeat("", times=2))[:2]
 
     return arg, unparsed
 
 
 def _parse_kwarg(unparsed: str) -> tuple[str, str, str]:
     """Parse an key-value argument"""
     key, unparsed = _parse_arg(unparsed[len(KWARG_INDICATOR) :])
 
     if unparsed.startswith(KWARG_INDICATOR):
         return key, "", unparsed
 
-    if unparsed.startswith(('"', "'")):
+    if unparsed.startswith(QUOTES):
         return key, *_parse_quoted_arg(unparsed)
 
     return key, *_parse_arg(unparsed)
 
 
 def parse_args_kwargs(msg: str) -> tuple[tuple[str, ...], dict[str, str]]:
     """Parses a message in to arguments and keyword arguments"""
@@ -77,15 +83,15 @@
     unparsed = msg.strip()
 
     while unparsed:
         if unparsed.startswith(KWARG_INDICATOR):
             key, value, unparsed = _parse_kwarg(unparsed)
             kwargs[key] = value
 
-        elif unparsed.startswith(('"', "'")):
+        elif unparsed.startswith(QUOTES):
             value, unparsed = _parse_quoted_arg(unparsed)
             args.append(value)
 
         else:
             value, unparsed = _parse_arg(unparsed)
             args.append(value)
```

### Comparing `tsbot-1.1.0/tsbot/plugin.py` & `tsbot-1.1.1/tsbot/plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,21 +32,22 @@
     Callable[Concatenate[_T, bot.TSBot, context.TSCtx, _P], Coroutine[None, None, None]],
 ]:
     """Decorator to register plugin commands"""
 
     def command_decorator(
         func: Callable[Concatenate[_T, bot.TSBot, context.TSCtx, _P], Coroutine[None, None, None]]
     ) -> Callable[Concatenate[_T, bot.TSBot, context.TSCtx, _P], Coroutine[None, None, None]]:
-        func.__ts_command__ = {  # type: ignore
+        kwargs = {
             "command": command,
             "help_text": help_text,
             "raw": raw,
             "hidden": hidden,
             "checks": checks or [],
         }
+        setattr(func, "__ts_command__", kwargs)
         return func
 
     return command_decorator
 
 
 def on(
     event_type: str,
@@ -55,15 +56,15 @@
     Callable[[_T, bot.TSBot, Any], Coroutine[None, None, None]],
 ]:
     """Decorator to register plugin events"""
 
     def event_decorator(
         func: Callable[[_T, bot.TSBot, Any], Coroutine[None, None, None]]
     ) -> Callable[[_T, bot.TSBot, Any], Coroutine[None, None, None]]:
-        func.__ts_event__ = {"event_type": event_type}  # type: ignore
+        setattr(func, "__ts_event__", {"event_type": event_type})
         return func
 
     return event_decorator
 
 
 def once(
     event_type: str,
@@ -72,11 +73,11 @@
     Callable[[_T, bot.TSBot, Any], Coroutine[None, None, None]],
 ]:
     """Decorator to register plugin events to be ran only once"""
 
     def once_decorator(
         func: Callable[[_T, bot.TSBot, Any], Coroutine[None, None, None]]
     ) -> Callable[[_T, bot.TSBot, Any], Coroutine[None, None, None]]:
-        func.__ts_once__ = {"event_type": event_type}  # type: ignore
+        setattr(func, "__ts_once__", {"event_type": event_type})
         return func
 
     return once_decorator
```

### Comparing `tsbot-1.1.0/tsbot/query_builder/builder.py` & `tsbot-1.1.1/tsbot/query_builder/builder.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.0/tsbot/query_builder/commands.py` & `tsbot-1.1.1/tsbot/query_builder/commands.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.0/tsbot/ratelimiter.py` & `tsbot-1.1.1/tsbot/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.0/tsbot/response.py` & `tsbot-1.1.1/tsbot/response.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.0/tsbot/tasks/handler.py` & `tsbot-1.1.1/tsbot/tasks/handler.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.0/tsbot/tasks/task.py` & `tsbot-1.1.1/tsbot/tasks/task.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.0/tsbot/utils.py` & `tsbot-1.1.1/tsbot/utils.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.0/tsbot.egg-info/PKG-INFO` & `tsbot-1.1.1/tsbot.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: tsbot
-Version: 1.1.0
+Version: 1.1.1
 Summary: Asynchronous framework to build TeamSpeak 3 Server Query bots
 Author: 0x4aK
 Project-URL: repository, https://github.com/0x4aK/tsbot
 Project-URL: documentation, https://tsbot.readthedocs.io/en/latest/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: asyncssh>=2.9.0
+Requires-Dist: asyncssh==2.14.0
 Provides-Extra: tests
-Requires-Dist: mypy>=0.931; extra == "tests"
-Requires-Dist: pytest>=7.0.0; extra == "tests"
-Requires-Dist: pytest-cov>=3.0.0; extra == "tests"
+Requires-Dist: mypy>=1.9.0; extra == "tests"
+Requires-Dist: pytest==8.1.1; extra == "tests"
+Requires-Dist: pytest-cov==5.0.0; extra == "tests"
 Provides-Extra: docs
-Requires-Dist: sphinx>=7.2.6; extra == "docs"
-Requires-Dist: myst-parser>=0.18.0; extra == "docs"
-Requires-Dist: sphinx-autodoc-typehints>=1.18.2; extra == "docs"
-Requires-Dist: sphinx-autobuild>=2021.3.14; extra == "docs"
+Requires-Dist: sphinx>=7.3.7; extra == "docs"
+Requires-Dist: myst-parser>=2.0.0; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints>=2.1.0; extra == "docs"
+Requires-Dist: sphinx-autobuild>=2024.4.16; extra == "docs"
 Requires-Dist: sphinx_rtd_theme>=2.0.0; extra == "docs"
 
 # TSBot
 
 Asynchronous framework to build **TeamSpeak 3 Server Query** bots
 
 ## ✅ Features
```

### Comparing `tsbot-1.1.0/tsbot.egg-info/SOURCES.txt` & `tsbot-1.1.1/tsbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

