# Comparing `tmp/decoutilities-0.1.8.tar.gz` & `tmp/decoutilities-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoutilities-0.1.8.tar", last modified: Tue Apr 30 07:13:34 2024, max compression
+gzip compressed data, was "decoutilities-0.1.9.tar", last modified: Tue Apr 30 07:42:10 2024, max compression
```

## Comparing `decoutilities-0.1.8.tar` & `decoutilities-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 07:13:34.092320 decoutilities-0.1.8/
--rw-rw-rw-   0        0        0     1089 2024-04-26 12:51:10.000000 decoutilities-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     5658 2024-04-30 07:13:34.079323 decoutilities-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     5187 2024-04-30 06:54:11.000000 decoutilities-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 07:13:33.896319 decoutilities-0.1.8/decoutilities/
--rw-rw-rw-   0        0        0     1104 2024-04-29 13:11:45.000000 decoutilities-0.1.8/decoutilities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 07:13:34.005320 decoutilities-0.1.8/decoutilities/config/
--rw-rw-rw-   0        0        0      104 2024-04-29 13:15:34.000000 decoutilities-0.1.8/decoutilities/config/__init__.py
--rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.1.8/decoutilities/config/config.py
--rw-rw-rw-   0        0        0     2710 2024-04-30 07:10:32.000000 decoutilities-0.1.8/decoutilities/config/configContainer.py
-drwxrwxrwx   0        0        0        0 2024-04-30 07:13:34.057319 decoutilities-0.1.8/decoutilities/inject/
--rw-rw-rw-   0        0        0       44 2024-04-29 13:15:19.000000 decoutilities-0.1.8/decoutilities/inject/__init__.py
--rw-rw-rw-   0        0        0      483 2024-04-29 13:14:09.000000 decoutilities-0.1.8/decoutilities/inject/injector.py
-drwxrwxrwx   0        0        0        0 2024-04-30 07:13:34.071319 decoutilities-0.1.8/decoutilities.egg-info/
--rw-rw-rw-   0        0        0     5658 2024-04-30 07:13:33.000000 decoutilities-0.1.8/decoutilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      370 2024-04-30 07:13:33.000000 decoutilities-0.1.8/decoutilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 07:13:33.000000 decoutilities-0.1.8/decoutilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-30 07:13:33.000000 decoutilities-0.1.8/decoutilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 07:13:34.093319 decoutilities-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      729 2024-04-30 07:12:02.000000 decoutilities-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 07:42:10.048456 decoutilities-0.1.9/
+-rw-rw-rw-   0        0        0     1089 2024-04-26 12:51:10.000000 decoutilities-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     6074 2024-04-30 07:42:10.029456 decoutilities-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5603 2024-04-30 07:38:44.000000 decoutilities-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 07:42:09.862458 decoutilities-0.1.9/decoutilities/
+-rw-rw-rw-   0        0        0     1399 2024-04-30 07:35:18.000000 decoutilities-0.1.9/decoutilities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 07:42:09.964457 decoutilities-0.1.9/decoutilities/config/
+-rw-rw-rw-   0        0        0      104 2024-04-29 13:15:34.000000 decoutilities-0.1.9/decoutilities/config/__init__.py
+-rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.1.9/decoutilities/config/config.py
+-rw-rw-rw-   0        0        0     2710 2024-04-30 07:10:32.000000 decoutilities-0.1.9/decoutilities/config/configContainer.py
+drwxrwxrwx   0        0        0        0 2024-04-30 07:42:09.997460 decoutilities-0.1.9/decoutilities/inject/
+-rw-rw-rw-   0        0        0       44 2024-04-29 13:15:19.000000 decoutilities-0.1.9/decoutilities/inject/__init__.py
+-rw-rw-rw-   0        0        0      483 2024-04-29 13:14:09.000000 decoutilities-0.1.9/decoutilities/inject/injector.py
+drwxrwxrwx   0        0        0        0 2024-04-30 07:42:10.015457 decoutilities-0.1.9/decoutilities.egg-info/
+-rw-rw-rw-   0        0        0     6074 2024-04-30 07:42:09.000000 decoutilities-0.1.9/decoutilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      370 2024-04-30 07:42:09.000000 decoutilities-0.1.9/decoutilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 07:42:09.000000 decoutilities-0.1.9/decoutilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-30 07:42:09.000000 decoutilities-0.1.9/decoutilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 07:42:10.056457 decoutilities-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      729 2024-04-30 07:40:43.000000 decoutilities-0.1.9/setup.py
```

### Comparing `decoutilities-0.1.8/LICENSE` & `decoutilities-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `decoutilities-0.1.8/PKG-INFO` & `decoutilities-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.1.8
+Version: 0.1.9
 Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -91,14 +91,29 @@
 
 # Start the thread
 thread.start()
 
 # Outputs: Running with value 5
 ```
 
+### @trycatch
+
+The `@trycatch` decorator wraps a function in a try-catch block, allowing it to handle exceptions without needing to write explicit try-catch blocks in your code.
+
+```python
+from decoutilities import trycatch
+
+@trycatch
+def risky_function():
+    # Some risky operation that might raise an exception
+    return 1 / 0
+
+risky_function()  # Prints: An error occurred: division by zero
+```
+
 ### Config System
 
 `decoutilities` provides a complex config system that allows you to easily manage configuration settings using decorators.
 
 #### configContainer
 
 The `configContainer` class is responsible for loading and saving configuration data from/to JSON or YAML files.
```

### Comparing `decoutilities-0.1.8/README.md` & `decoutilities-0.1.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -78,14 +78,29 @@
 
 # Start the thread
 thread.start()
 
 # Outputs: Running with value 5
 ```
 
+### @trycatch
+
+The `@trycatch` decorator wraps a function in a try-catch block, allowing it to handle exceptions without needing to write explicit try-catch blocks in your code.
+
+```python
+from decoutilities import trycatch
+
+@trycatch
+def risky_function():
+    # Some risky operation that might raise an exception
+    return 1 / 0
+
+risky_function()  # Prints: An error occurred: division by zero
+```
+
 ### Config System
 
 `decoutilities` provides a complex config system that allows you to easily manage configuration settings using decorators.
 
 #### configContainer
 
 The `configContainer` class is responsible for loading and saving configuration data from/to JSON or YAML files.
```

### Comparing `decoutilities-0.1.8/decoutilities/__init__.py` & `decoutilities-0.1.9/decoutilities/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,8 +32,18 @@
 # Make a class threaded and return a thread object. (EXPERIMENTAL)
 
 def threaded(cls):
     import threading
 
     def wrapper(*args, **kwargs):
         return threading.Thread(target=cls, args=args, kwargs=kwargs)
+    return wrapper
+
+# @trycatch
+# Make a piece of code try-catchable without using try-catch blocks.
+def trycatch(func):
+    def wrapper(*args, **kwargs):
+        try:
+            return func(*args, **kwargs)
+        except Exception as e:
+            print(f"An error occurred: {e}")
     return wrapper
```

### Comparing `decoutilities-0.1.8/decoutilities/config/config.py` & `decoutilities-0.1.9/decoutilities/config/config.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.1.8/decoutilities/config/configContainer.py` & `decoutilities-0.1.9/decoutilities/config/configContainer.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.1.8/decoutilities.egg-info/PKG-INFO` & `decoutilities-0.1.9/decoutilities.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.1.8
+Version: 0.1.9
 Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -91,14 +91,29 @@
 
 # Start the thread
 thread.start()
 
 # Outputs: Running with value 5
 ```
 
+### @trycatch
+
+The `@trycatch` decorator wraps a function in a try-catch block, allowing it to handle exceptions without needing to write explicit try-catch blocks in your code.
+
+```python
+from decoutilities import trycatch
+
+@trycatch
+def risky_function():
+    # Some risky operation that might raise an exception
+    return 1 / 0
+
+risky_function()  # Prints: An error occurred: division by zero
+```
+
 ### Config System
 
 `decoutilities` provides a complex config system that allows you to easily manage configuration settings using decorators.
 
 #### configContainer
 
 The `configContainer` class is responsible for loading and saving configuration data from/to JSON or YAML files.
```

### Comparing `decoutilities-0.1.8/setup.py` & `decoutilities-0.1.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
 name='decoutilities',
-version='0.1.8',
+version='0.1.9',
 author='Hugo Torres',
 author_email='contact@redactado.es',
 description='Enhance the readability of your code with decorators and simplify the creation of configuration files.',
 packages=find_packages(include=['decoutilities', 'decoutilities.*']),
 classifiers=[
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: MIT License',
```

