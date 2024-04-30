# Comparing `tmp/riddlesolver-0.1.5.tar.gz` & `tmp/riddlesolver-0.1.7.tar.gz`

## Comparing `riddlesolver-0.1.5.tar` & `riddlesolver-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,23 @@
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 riddlesolver-0.1.5/.idea/.gitignore
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 riddlesolver-0.1.5/.idea/.name
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 riddlesolver-0.1.5/.idea/misc.xml
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 riddlesolver-0.1.5/.idea/modules.xml
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 riddlesolver-0.1.5/.idea/riddlesolver.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 riddlesolver-0.1.5/.idea/vcs.xml
--rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 riddlesolver-0.1.5/.idea/workspace.xml
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 riddlesolver-0.1.5/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 riddlesolver-0.1.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 riddlesolver-0.1.5/riddlesolver/__init__.py
--rw-r--r--   0        0        0    17150 2020-02-02 00:00:00.000000 riddlesolver-0.1.5/riddlesolver/app.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 riddlesolver-0.1.5/riddlesolver/requirements.txt
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 riddlesolver-0.1.5/riddlesolver/setup.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 riddlesolver-0.1.5/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 riddlesolver-0.1.5/LICENSE
--rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 riddlesolver-0.1.5/README.md
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 riddlesolver-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     6177 2020-02-02 00:00:00.000000 riddlesolver-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 riddlesolver-0.1.7/.idea/.gitignore
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 riddlesolver-0.1.7/.idea/.name
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 riddlesolver-0.1.7/.idea/misc.xml
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 riddlesolver-0.1.7/.idea/modules.xml
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 riddlesolver-0.1.7/.idea/riddlesolver.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 riddlesolver-0.1.7/.idea/vcs.xml
+-rw-r--r--   0        0        0    10720 2020-02-02 00:00:00.000000 riddlesolver-0.1.7/.idea/workspace.xml
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 riddlesolver-0.1.7/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 riddlesolver-0.1.7/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 riddlesolver-0.1.7/riddlesolver/__init__.py
+-rw-r--r--   0        0        0     3871 2020-02-02 00:00:00.000000 riddlesolver-0.1.7/riddlesolver/app.py
+-rw-r--r--   0        0        0     6094 2020-02-02 00:00:00.000000 riddlesolver-0.1.7/riddlesolver/config.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 riddlesolver-0.1.7/riddlesolver/constants.py
+-rw-r--r--   0        0        0     8702 2020-02-02 00:00:00.000000 riddlesolver-0.1.7/riddlesolver/repository.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 riddlesolver-0.1.7/riddlesolver/requirements.txt
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 riddlesolver-0.1.7/riddlesolver/setup.py
+-rw-r--r--   0        0        0     5372 2020-02-02 00:00:00.000000 riddlesolver-0.1.7/riddlesolver/summary.py
+-rw-r--r--   0        0        0    14023 2020-02-02 00:00:00.000000 riddlesolver-0.1.7/riddlesolver/utils.py
+-rw-r--r--   0        0        0     3258 2020-02-02 00:00:00.000000 riddlesolver-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 riddlesolver-0.1.7/LICENSE
+-rw-r--r--   0        0        0     8525 2020-02-02 00:00:00.000000 riddlesolver-0.1.7/README.md
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 riddlesolver-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 riddlesolver-0.1.7/PKG-INFO
```

### Comparing `riddlesolver-0.1.5/riddlesolver/setup.py` & `riddlesolver-0.1.7/riddlesolver/setup.py`

 * *Files identical despite different names*

### Comparing `riddlesolver-0.1.5/.gitignore` & `riddlesolver-0.1.7/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -153,8 +153,11 @@
 cython_debug/
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-#.idea/
+#.idea/
+
+# OSX
+.DS_Store
```

### Comparing `riddlesolver-0.1.5/LICENSE` & `riddlesolver-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `riddlesolver-0.1.5/pyproject.toml` & `riddlesolver-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "riddlesolver"
-version = "0.1.5"
+version = "0.1.7"
 description = "A command-line tool to summarize Git commits using OpenAI ChatGPT"
 authors = [{ name = "Siyuan Wu", email = "cushmily@gmail.com" }]
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -20,15 +20,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 license = "MIT"
 dependencies = [
     "gitpython",
     "openai",
-    "requests"
+    "requests",
 ]
 
 [project.scripts]
 riddlesolver = "riddlesolver.app:main"
 
 [tool.hatch.build.targets.wheel]
 packages = ["riddlesolver"]
```

