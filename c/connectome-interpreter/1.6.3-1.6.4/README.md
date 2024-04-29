# Comparing `tmp/connectome_interpreter-1.6.3.tar.gz` & `tmp/connectome_interpreter-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectome_interpreter-1.6.3.tar", last modified: Mon Apr 29 17:26:03 2024, max compression
+gzip compressed data, was "connectome_interpreter-1.6.4.tar", last modified: Mon Apr 29 17:47:32 2024, max compression
```

## Comparing `connectome_interpreter-1.6.3.tar` & `connectome_interpreter-1.6.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 17:26:03.766310 connectome_interpreter-1.6.3/
--rw-rw-rw-   0        0        0     1086 2024-02-16 09:04:27.000000 connectome_interpreter-1.6.3/LICENSE
--rw-rw-rw-   0        0        0     1095 2024-04-29 17:26:03.764225 connectome_interpreter-1.6.3/PKG-INFO
--rw-rw-rw-   0        0        0     1201 2024-04-14 17:28:06.000000 connectome_interpreter-1.6.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 17:26:03.673426 connectome_interpreter-1.6.3/connectome_interpreter/
--rw-rw-rw-   0        0        0      136 2024-03-07 21:35:51.000000 connectome_interpreter-1.6.3/connectome_interpreter/__init__.py
--rw-rw-rw-   0        0        0    33835 2024-04-29 17:22:56.000000 connectome_interpreter-1.6.3/connectome_interpreter/activation_maximisation.py
--rw-rw-rw-   0        0        0    21563 2024-04-28 18:29:19.000000 connectome_interpreter-1.6.3/connectome_interpreter/compress_paths.py
--rw-rw-rw-   0        0        0    16135 2024-04-28 19:46:57.000000 connectome_interpreter-1.6.3/connectome_interpreter/path_finding.py
--rw-rw-rw-   0        0        0    31484 2024-04-20 23:13:30.000000 connectome_interpreter-1.6.3/connectome_interpreter/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-29 17:26:03.726660 connectome_interpreter-1.6.3/connectome_interpreter.egg-info/
--rw-rw-rw-   0        0        0     1095 2024-04-29 17:26:03.000000 connectome_interpreter-1.6.3/connectome_interpreter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      519 2024-04-29 17:26:03.000000 connectome_interpreter-1.6.3/connectome_interpreter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 17:26:03.000000 connectome_interpreter-1.6.3/connectome_interpreter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      132 2024-04-29 17:26:03.000000 connectome_interpreter-1.6.3/connectome_interpreter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-04-29 17:26:03.000000 connectome_interpreter-1.6.3/connectome_interpreter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 17:26:03.767307 connectome_interpreter-1.6.3/setup.cfg
--rw-rw-rw-   0        0        0     2218 2024-04-29 17:23:50.000000 connectome_interpreter-1.6.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 17:26:03.762095 connectome_interpreter-1.6.3/tests/
--rw-rw-rw-   0        0        0        0 2024-02-16 09:04:27.000000 connectome_interpreter-1.6.3/tests/__init__.py
--rw-rw-rw-   0        0        0     2996 2024-04-20 17:48:24.000000 connectome_interpreter-1.6.3/tests/test_compress_paths.py
--rw-rw-rw-   0        0        0     2534 2024-04-20 14:38:13.000000 connectome_interpreter-1.6.3/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 17:47:32.264776 connectome_interpreter-1.6.4/
+-rw-rw-rw-   0        0        0     1086 2024-02-16 09:04:27.000000 connectome_interpreter-1.6.4/LICENSE
+-rw-rw-rw-   0        0        0     1066 2024-04-29 17:47:32.263466 connectome_interpreter-1.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1201 2024-04-14 17:28:06.000000 connectome_interpreter-1.6.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 17:47:32.233524 connectome_interpreter-1.6.4/connectome_interpreter/
+-rw-rw-rw-   0        0        0      136 2024-03-07 21:35:51.000000 connectome_interpreter-1.6.4/connectome_interpreter/__init__.py
+-rw-rw-rw-   0        0        0    33835 2024-04-29 17:22:56.000000 connectome_interpreter-1.6.4/connectome_interpreter/activation_maximisation.py
+-rw-rw-rw-   0        0        0    21563 2024-04-28 18:29:19.000000 connectome_interpreter-1.6.4/connectome_interpreter/compress_paths.py
+-rw-rw-rw-   0        0        0    16135 2024-04-28 19:46:57.000000 connectome_interpreter-1.6.4/connectome_interpreter/path_finding.py
+-rw-rw-rw-   0        0        0    31484 2024-04-20 23:13:30.000000 connectome_interpreter-1.6.4/connectome_interpreter/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 17:47:32.258484 connectome_interpreter-1.6.4/connectome_interpreter.egg-info/
+-rw-rw-rw-   0        0        0     1066 2024-04-29 17:47:32.000000 connectome_interpreter-1.6.4/connectome_interpreter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      519 2024-04-29 17:47:32.000000 connectome_interpreter-1.6.4/connectome_interpreter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 17:47:32.000000 connectome_interpreter-1.6.4/connectome_interpreter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2024-04-29 17:47:32.000000 connectome_interpreter-1.6.4/connectome_interpreter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-04-29 17:47:32.000000 connectome_interpreter-1.6.4/connectome_interpreter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 17:47:32.264776 connectome_interpreter-1.6.4/setup.cfg
+-rw-rw-rw-   0        0        0     2068 2024-04-29 17:46:53.000000 connectome_interpreter-1.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 17:47:32.261473 connectome_interpreter-1.6.4/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-16 09:04:27.000000 connectome_interpreter-1.6.4/tests/__init__.py
+-rw-rw-rw-   0        0        0     2996 2024-04-20 17:48:24.000000 connectome_interpreter-1.6.4/tests/test_compress_paths.py
+-rw-rw-rw-   0        0        0     2534 2024-04-20 14:38:13.000000 connectome_interpreter-1.6.4/tests/test_utils.py
```

### Comparing `connectome_interpreter-1.6.3/LICENSE` & `connectome_interpreter-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.3/PKG-INFO` & `connectome_interpreter-1.6.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: connectome_interpreter
-Version: 1.6.3
+Version: 1.6.4
 Summary: A tool for connectomics data interpretation
 Author: Yijie Yin
 Author-email: yy432@cam.ac.uk
 Project-URL: Source, https: // github.com/YijieYin/connectome_interpreter
 Project-URL: Documentation, https://connectome-interpreter.readthedocs.io/en/latest/
 Project-URL: Larva connectome example, https://colab.research.google.com/drive/1VIMNFBp7dCgN5XOQ9vvzPaqb80BGPZx4?usp=sharing
 Project-URL: Adult connectome example (FAFB), https://colab.research.google.com/drive/1ECUagwN-r2rnKyfcYgtR1oG8Lox8m8BW?usp=sharing
 Keywords: connectomics,neural network,mechanistic interpretability
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scipy
-Requires-Dist: torch==2.2.0
 Requires-Dist: tqdm
 Requires-Dist: plotly
 Requires-Dist: matplotlib
 Requires-Dist: networkx
 Requires-Dist: seaborn
 Requires-Dist: ipywidgets
 Requires-Dist: IPython
```

### Comparing `connectome_interpreter-1.6.3/README.md` & `connectome_interpreter-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.3/connectome_interpreter/activation_maximisation.py` & `connectome_interpreter-1.6.4/connectome_interpreter/activation_maximisation.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.3/connectome_interpreter/compress_paths.py` & `connectome_interpreter-1.6.4/connectome_interpreter/compress_paths.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.3/connectome_interpreter/path_finding.py` & `connectome_interpreter-1.6.4/connectome_interpreter/path_finding.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.3/connectome_interpreter/utils.py` & `connectome_interpreter-1.6.4/connectome_interpreter/utils.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.3/connectome_interpreter.egg-info/PKG-INFO` & `connectome_interpreter-1.6.4/connectome_interpreter.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: connectome-interpreter
-Version: 1.6.3
+Version: 1.6.4
 Summary: A tool for connectomics data interpretation
 Author: Yijie Yin
 Author-email: yy432@cam.ac.uk
 Project-URL: Source, https: // github.com/YijieYin/connectome_interpreter
 Project-URL: Documentation, https://connectome-interpreter.readthedocs.io/en/latest/
 Project-URL: Larva connectome example, https://colab.research.google.com/drive/1VIMNFBp7dCgN5XOQ9vvzPaqb80BGPZx4?usp=sharing
 Project-URL: Adult connectome example (FAFB), https://colab.research.google.com/drive/1ECUagwN-r2rnKyfcYgtR1oG8Lox8m8BW?usp=sharing
 Keywords: connectomics,neural network,mechanistic interpretability
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scipy
-Requires-Dist: torch==2.2.0
 Requires-Dist: tqdm
 Requires-Dist: plotly
 Requires-Dist: matplotlib
 Requires-Dist: networkx
 Requires-Dist: seaborn
 Requires-Dist: ipywidgets
 Requires-Dist: IPython
```

### Comparing `connectome_interpreter-1.6.3/connectome_interpreter.egg-info/SOURCES.txt` & `connectome_interpreter-1.6.4/connectome_interpreter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.3/setup.py` & `connectome_interpreter-1.6.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,47 @@
 from setuptools import setup, find_packages
 import pkg_resources
 
 # Function to check if PyTorch is already installed
 
 
-def get_torch_version():
+def is_torch_installed():
     try:
-        return pkg_resources.get_distribution('torch').version
+        pkg_resources.get_distribution('torch')
+        return True
     except pkg_resources.DistributionNotFound:
-        return None
+        return False
 
 
-# Specify a PyTorch version requirement only if it's not installed
-torch_version = get_torch_version()
-if torch_version is None:
-    torch_requirement = 'torch>=1.7.1'
-else:
-    torch_requirement = f'torch=={torch_version}'
+install_requires_list = [
+    # List your package dependencies here
+    'numpy',
+    'pandas',
+    'scipy',
+    'tqdm',
+    'plotly',
+    'matplotlib',
+    'networkx',
+    'seaborn',
+    'ipywidgets',
+    'IPython',
+]
+# Add torch only if it's not already installed
+if not is_torch_installed():
+    install_requires_list.append('torch>=1.7.1')
 
 
 setup(
     name='connectome_interpreter',
     # If you're making a patch or a minor bug fix, increment the patch version, e.g., from 0.1.0 to 0.1.1.
     # If you're adding functionality in a backwards-compatible manner, increment the minor version, e.g., from 0.1.0 to 0.2.0.
     # If you're making incompatible API changes, increment the major version, e.g., from 0.1.0 to 1.0.0.
-    version='1.6.3',
+    version='1.6.4',
     packages=find_packages(),
-    install_requires=[
-        # List your package dependencies here
-        'numpy',
-        'pandas',
-        'scipy',
-        # 'torch>=1.7.1',
-        torch_requirement,
-        'tqdm',
-        'plotly',
-        'matplotlib',
-        'networkx',
-        'seaborn',
-        'ipywidgets',
-        'IPython',
-    ],
+    install_requires=install_requires_list,
     extras_require={
         'get_ngl_link': ['nglscenes'],
         'wandb': ['wandb'],
     },
     # Optional metadata
     author='Yijie Yin',
     author_email='yy432@cam.ac.uk',
```

### Comparing `connectome_interpreter-1.6.3/tests/test_compress_paths.py` & `connectome_interpreter-1.6.4/tests/test_compress_paths.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.3/tests/test_utils.py` & `connectome_interpreter-1.6.4/tests/test_utils.py`

 * *Files identical despite different names*

