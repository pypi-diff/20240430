# Comparing `tmp/assertai_alpha_deployer-4.6.tar.gz` & `tmp/assertai_alpha_deployer-4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assertai_alpha_deployer-4.6.tar", last modified: Tue Apr 30 20:54:39 2024, max compression
+gzip compressed data, was "assertai_alpha_deployer-4.7.tar", last modified: Tue Apr 30 20:57:36 2024, max compression
```

## Comparing `assertai_alpha_deployer-4.6.tar` & `assertai_alpha_deployer-4.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 devl      (1000) devl      (1000)        0 2024-04-30 20:54:39.670926 assertai_alpha_deployer-4.6/
--rw-rw-r--   0 devl      (1000) devl      (1000)       85 2024-04-30 20:51:30.000000 assertai_alpha_deployer-4.6/MANIFEST.in
--rw-r--r--   0 devl      (1000) devl      (1000)      729 2024-04-30 20:54:39.670926 assertai_alpha_deployer-4.6/PKG-INFO
-drwxrwxr-x   0 devl      (1000) devl      (1000)        0 2024-04-30 20:54:39.670926 assertai_alpha_deployer-4.6/assertai_alpha_deployer.egg-info/
--rw-r--r--   0 devl      (1000) devl      (1000)      729 2024-04-30 20:54:39.000000 assertai_alpha_deployer-4.6/assertai_alpha_deployer.egg-info/PKG-INFO
--rw-rw-r--   0 devl      (1000) devl      (1000)      304 2024-04-30 20:54:39.000000 assertai_alpha_deployer-4.6/assertai_alpha_deployer.egg-info/SOURCES.txt
--rw-rw-r--   0 devl      (1000) devl      (1000)        1 2024-04-30 20:54:39.000000 assertai_alpha_deployer-4.6/assertai_alpha_deployer.egg-info/dependency_links.txt
--rw-rw-r--   0 devl      (1000) devl      (1000)       82 2024-04-30 20:54:39.000000 assertai_alpha_deployer-4.6/assertai_alpha_deployer.egg-info/entry_points.txt
--rw-rw-r--   0 devl      (1000) devl      (1000)        7 2024-04-30 20:54:39.000000 assertai_alpha_deployer-4.6/assertai_alpha_deployer.egg-info/requires.txt
--rw-rw-r--   0 devl      (1000) devl      (1000)       24 2024-04-30 20:54:39.000000 assertai_alpha_deployer-4.6/assertai_alpha_deployer.egg-info/top_level.txt
--rw-rw-r--   0 devl      (1000) devl      (1000)       38 2024-04-30 20:54:39.670926 assertai_alpha_deployer-4.6/setup.cfg
--rw-rw-r--   0 devl      (1000) devl      (1000)     1117 2024-04-30 20:54:20.000000 assertai_alpha_deployer-4.6/setup.py
+drwxrwxr-x   0 devl      (1000) devl      (1000)        0 2024-04-30 20:57:36.273035 assertai_alpha_deployer-4.7/
+-rw-rw-r--   0 devl      (1000) devl      (1000)       85 2024-04-30 20:51:30.000000 assertai_alpha_deployer-4.7/MANIFEST.in
+-rw-r--r--   0 devl      (1000) devl      (1000)      729 2024-04-30 20:57:36.273035 assertai_alpha_deployer-4.7/PKG-INFO
+drwxrwxr-x   0 devl      (1000) devl      (1000)        0 2024-04-30 20:57:36.273035 assertai_alpha_deployer-4.7/assertai_alpha_deployer.egg-info/
+-rw-r--r--   0 devl      (1000) devl      (1000)      729 2024-04-30 20:57:36.000000 assertai_alpha_deployer-4.7/assertai_alpha_deployer.egg-info/PKG-INFO
+-rw-rw-r--   0 devl      (1000) devl      (1000)      304 2024-04-30 20:57:36.000000 assertai_alpha_deployer-4.7/assertai_alpha_deployer.egg-info/SOURCES.txt
+-rw-rw-r--   0 devl      (1000) devl      (1000)        1 2024-04-30 20:57:36.000000 assertai_alpha_deployer-4.7/assertai_alpha_deployer.egg-info/dependency_links.txt
+-rw-rw-r--   0 devl      (1000) devl      (1000)       82 2024-04-30 20:57:36.000000 assertai_alpha_deployer-4.7/assertai_alpha_deployer.egg-info/entry_points.txt
+-rw-rw-r--   0 devl      (1000) devl      (1000)        7 2024-04-30 20:57:36.000000 assertai_alpha_deployer-4.7/assertai_alpha_deployer.egg-info/requires.txt
+-rw-rw-r--   0 devl      (1000) devl      (1000)       24 2024-04-30 20:57:36.000000 assertai_alpha_deployer-4.7/assertai_alpha_deployer.egg-info/top_level.txt
+-rw-rw-r--   0 devl      (1000) devl      (1000)       38 2024-04-30 20:57:36.273035 assertai_alpha_deployer-4.7/setup.cfg
+-rw-rw-r--   0 devl      (1000) devl      (1000)     1502 2024-04-30 20:57:20.000000 assertai_alpha_deployer-4.7/setup.py
```

### Comparing `assertai_alpha_deployer-4.6/PKG-INFO` & `assertai_alpha_deployer-4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assertai_alpha_deployer
-Version: 4.6
+Version: 4.7
 Summary: A package to deploy python codes on bare-metal
 Home-page: https://www.linkedin.com/in/rajeshroy402
 Author: Rajesh Roy
 Author-email: rajeshroy402@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `assertai_alpha_deployer-4.6/assertai_alpha_deployer.egg-info/PKG-INFO` & `assertai_alpha_deployer-4.7/assertai_alpha_deployer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assertai_alpha_deployer
-Version: 4.6
+Version: 4.7
 Summary: A package to deploy python codes on bare-metal
 Home-page: https://www.linkedin.com/in/rajeshroy402
 Author: Rajesh Roy
 Author-email: rajeshroy402@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `assertai_alpha_deployer-4.6/setup.py` & `assertai_alpha_deployer-4.7/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 from setuptools import setup, find_packages
+from setuptools.command.install import install
+import os
+
+class PostInstallCommand(install):
+    def run(self):
+        install.run(self)
+        # Remove the script_manager.py file after installation
+        script_manager_path = os.path.join(self.install_lib, 'assertai_alpha_deployer', 'script_manager.py')
+        if os.path.exists(script_manager_path):
+            os.remove(script_manager_path)
 
 setup(
     name='assertai_alpha_deployer',
-    version='4.6',
+    version='4.7',
     packages=find_packages(),
-    package_data={
-        'assertai_alpha_deployer': ['*', '!*.py'],
-    },
     install_requires=[
         'psutil',
     ],
     entry_points={
         'console_scripts': [
             'assertai-alpha-deployer=assertai_alpha_deployer.__main__:main',
         ],
@@ -27,8 +34,11 @@
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
+    cmdclass={
+        'install': PostInstallCommand,
+    },
 )
```

