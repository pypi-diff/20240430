# Comparing `tmp/decoutilities-0.1.7.tar.gz` & `tmp/decoutilities-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoutilities-0.1.7.tar", last modified: Mon Apr 29 13:27:31 2024, max compression
+gzip compressed data, was "decoutilities-0.1.8.tar", last modified: Tue Apr 30 07:13:34 2024, max compression
```

## Comparing `decoutilities-0.1.7.tar` & `decoutilities-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 13:27:31.191102 decoutilities-0.1.7/
--rw-rw-rw-   0        0        0     1089 2024-04-26 12:51:10.000000 decoutilities-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     4767 2024-04-29 13:27:31.174105 decoutilities-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     4296 2024-04-29 13:26:01.000000 decoutilities-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 13:27:30.941102 decoutilities-0.1.7/decoutilities/
--rw-rw-rw-   0        0        0     1104 2024-04-29 13:11:45.000000 decoutilities-0.1.7/decoutilities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 13:27:31.084103 decoutilities-0.1.7/decoutilities/config/
--rw-rw-rw-   0        0        0      104 2024-04-29 13:15:34.000000 decoutilities-0.1.7/decoutilities/config/__init__.py
--rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.1.7/decoutilities/config/config.py
--rw-rw-rw-   0        0        0     4322 2024-04-26 08:53:27.000000 decoutilities-0.1.7/decoutilities/config/configContainer.py
-drwxrwxrwx   0        0        0        0 2024-04-29 13:27:31.138101 decoutilities-0.1.7/decoutilities/inject/
--rw-rw-rw-   0        0        0       44 2024-04-29 13:15:19.000000 decoutilities-0.1.7/decoutilities/inject/__init__.py
--rw-rw-rw-   0        0        0      483 2024-04-29 13:14:09.000000 decoutilities-0.1.7/decoutilities/inject/injector.py
-drwxrwxrwx   0        0        0        0 2024-04-29 13:27:31.157102 decoutilities-0.1.7/decoutilities.egg-info/
--rw-rw-rw-   0        0        0     4767 2024-04-29 13:27:30.000000 decoutilities-0.1.7/decoutilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      370 2024-04-29 13:27:30.000000 decoutilities-0.1.7/decoutilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 13:27:30.000000 decoutilities-0.1.7/decoutilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-29 13:27:30.000000 decoutilities-0.1.7/decoutilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 13:27:31.194103 decoutilities-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      729 2024-04-29 13:26:18.000000 decoutilities-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 07:13:34.092320 decoutilities-0.1.8/
+-rw-rw-rw-   0        0        0     1089 2024-04-26 12:51:10.000000 decoutilities-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     5658 2024-04-30 07:13:34.079323 decoutilities-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5187 2024-04-30 06:54:11.000000 decoutilities-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 07:13:33.896319 decoutilities-0.1.8/decoutilities/
+-rw-rw-rw-   0        0        0     1104 2024-04-29 13:11:45.000000 decoutilities-0.1.8/decoutilities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 07:13:34.005320 decoutilities-0.1.8/decoutilities/config/
+-rw-rw-rw-   0        0        0      104 2024-04-29 13:15:34.000000 decoutilities-0.1.8/decoutilities/config/__init__.py
+-rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.1.8/decoutilities/config/config.py
+-rw-rw-rw-   0        0        0     2710 2024-04-30 07:10:32.000000 decoutilities-0.1.8/decoutilities/config/configContainer.py
+drwxrwxrwx   0        0        0        0 2024-04-30 07:13:34.057319 decoutilities-0.1.8/decoutilities/inject/
+-rw-rw-rw-   0        0        0       44 2024-04-29 13:15:19.000000 decoutilities-0.1.8/decoutilities/inject/__init__.py
+-rw-rw-rw-   0        0        0      483 2024-04-29 13:14:09.000000 decoutilities-0.1.8/decoutilities/inject/injector.py
+drwxrwxrwx   0        0        0        0 2024-04-30 07:13:34.071319 decoutilities-0.1.8/decoutilities.egg-info/
+-rw-rw-rw-   0        0        0     5658 2024-04-30 07:13:33.000000 decoutilities-0.1.8/decoutilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      370 2024-04-30 07:13:33.000000 decoutilities-0.1.8/decoutilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 07:13:33.000000 decoutilities-0.1.8/decoutilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-30 07:13:33.000000 decoutilities-0.1.8/decoutilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 07:13:34.093319 decoutilities-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      729 2024-04-30 07:12:02.000000 decoutilities-0.1.8/setup.py
```

### Comparing `decoutilities-0.1.7/LICENSE` & `decoutilities-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `decoutilities-0.1.7/PKG-INFO` & `decoutilities-0.1.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: decoutilities
-Version: 0.1.7
-Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
-Author: Hugo Torres
-Author-email: contact@redactado.es
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # decoutilities
 
 A simple python package that allows using decorators for multiple things like easily setting up singleton or config files.
 
 ## Installation
 
 You can install `decoutilities` using pip:
@@ -162,18 +149,36 @@
 # Use the injector to get the function
 greet_func = injector_instance.inject('greet')
 
 # Call the function
 print(greet_func('World'))  # Outputs: Hello, World!
 ```
 
+## Experimental Features
+
+All features marked as in `BETA` or being `EXPERIMENTAL` are untested, what means they were only tested below specific condititons and not with all case of uses.
+
+Please report any issues or contribute by making a PR (look for [CONTRIBUTING](CONTRIBUTING) section for details).
+
+### REMEMBER:
+
+This whole project is still in beta, and versions below `0.1.5` might not work. Also syntax changes could be made in a future, so consider creating a `requeriments.txt`file for your project specifying the version you wonder to use.
+
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
 
 ## Contributing
 
 Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the [GitHub repository](https://github.com/Reddishye/decoutilities).
 
+### Pull Requests
+
+In case you wonder to make a pull request, please include in the title any of these:
+- FEATURE: For new features, include a explanation mentioning why it should be inside `decoutilities`.
+- BUGFIX: For general bugfixes.
+- SECURITY: For fixes related with security issues.
+- QoL: For QoL improvements
+
 ## Author
 
-- [Hugo Torres](https://github.com/Reddishye)
+- [Hugo Torres](https://github.com/Reddishye)
```

### Comparing `decoutilities-0.1.7/decoutilities/__init__.py` & `decoutilities-0.1.8/decoutilities/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.1.7/decoutilities/config/config.py` & `decoutilities-0.1.8/decoutilities/config/config.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.1.7/decoutilities.egg-info/PKG-INFO` & `decoutilities-0.1.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.1.7
+Version: 0.1.8
 Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -162,18 +162,36 @@
 # Use the injector to get the function
 greet_func = injector_instance.inject('greet')
 
 # Call the function
 print(greet_func('World'))  # Outputs: Hello, World!
 ```
 
+## Experimental Features
+
+All features marked as in `BETA` or being `EXPERIMENTAL` are untested, what means they were only tested below specific condititons and not with all case of uses.
+
+Please report any issues or contribute by making a PR (look for [CONTRIBUTING](CONTRIBUTING) section for details).
+
+### REMEMBER:
+
+This whole project is still in beta, and versions below `0.1.5` might not work. Also syntax changes could be made in a future, so consider creating a `requeriments.txt`file for your project specifying the version you wonder to use.
+
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
 
 ## Contributing
 
 Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the [GitHub repository](https://github.com/Reddishye/decoutilities).
 
+### Pull Requests
+
+In case you wonder to make a pull request, please include in the title any of these:
+- FEATURE: For new features, include a explanation mentioning why it should be inside `decoutilities`.
+- BUGFIX: For general bugfixes.
+- SECURITY: For fixes related with security issues.
+- QoL: For QoL improvements
+
 ## Author
 
 - [Hugo Torres](https://github.com/Reddishye)
```

### Comparing `decoutilities-0.1.7/setup.py` & `decoutilities-0.1.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
 name='decoutilities',
-version='0.1.7',
+version='0.1.8',
 author='Hugo Torres',
 author_email='contact@redactado.es',
 description='Enhance the readability of your code with decorators and simplify the creation of configuration files.',
 packages=find_packages(include=['decoutilities', 'decoutilities.*']),
 classifiers=[
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: MIT License',
```

