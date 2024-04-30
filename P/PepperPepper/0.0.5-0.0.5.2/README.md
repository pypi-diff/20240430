# Comparing `tmp/pepperpepper-0.0.5.tar.gz` & `tmp/pepperpepper-0.0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepperpepper-0.0.5.tar", last modified: Tue Apr 30 02:14:10 2024, max compression
+gzip compressed data, was "pepperpepper-0.0.5.2.tar", last modified: Tue Apr 30 02:17:24 2024, max compression
```

## Comparing `pepperpepper-0.0.5.tar` & `pepperpepper-0.0.5.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 02:14:10.972591 pepperpepper-0.0.5/
--rw-rw-rw-   0        0        0      431 2024-04-30 02:14:10.972091 pepperpepper-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-30 02:14:10.936182 pepperpepper-0.0.5/PepperPepper/
--rw-rw-rw-   0        0        0     5179 2024-04-29 03:25:30.000000 pepperpepper-0.0.5/PepperPepper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:14:10.948825 pepperpepper-0.0.5/PepperPepper/callbacks/
--rw-rw-rw-   0        0        0      985 2024-04-30 01:42:49.000000 pepperpepper-0.0.5/PepperPepper/callbacks/__init__.py
--rw-rw-rw-   0        0        0      785 2024-04-30 01:42:05.000000 pepperpepper-0.0.5/PepperPepper/callbacks/custom_callback.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.5/PepperPepper/callbacks/learning_rate_scheduler.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:14:10.951325 pepperpepper-0.0.5/PepperPepper/core/
--rw-rw-rw-   0        0        0      930 2024-04-30 02:10:06.000000 pepperpepper-0.0.5/PepperPepper/core/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.5/PepperPepper/core/base_model.py
--rw-rw-rw-   0        0        0     4487 2024-04-30 02:03:25.000000 pepperpepper-0.0.5/PepperPepper/core/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:14:10.955336 pepperpepper-0.0.5/PepperPepper/datasets/
--rw-rw-rw-   0        0        0     1008 2024-04-29 04:09:47.000000 pepperpepper-0.0.5/PepperPepper/datasets/__init__.py
--rw-rw-rw-   0        0        0        4 2024-04-29 18:10:09.000000 pepperpepper-0.0.5/PepperPepper/datasets/custom_dataset.py
--rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.5/PepperPepper/datasets/image_datasets.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.5/PepperPepper/datasets/text_datasets.py
--rw-rw-rw-   0        0        0      106 2024-04-30 02:10:15.000000 pepperpepper-0.0.5/PepperPepper/environment.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:14:10.958399 pepperpepper-0.0.5/PepperPepper/examples/
--rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.5/PepperPepper/examples/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.5/PepperPepper/examples/custom_task.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.5/PepperPepper/examples/image_classification.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.5/PepperPepper/examples/text_generation.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:14:10.961386 pepperpepper-0.0.5/PepperPepper/layers/
--rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.5/PepperPepper/layers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.5/PepperPepper/layers/attention.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.5/PepperPepper/layers/custom_layer.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:14:10.962885 pepperpepper-0.0.5/PepperPepper/losses/
--rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.5/PepperPepper/losses/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.5/PepperPepper/losses/custom_loss.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:14:10.967110 pepperpepper-0.0.5/PepperPepper/models/
--rw-rw-rw-   0        0        0      752 2024-04-26 06:22:17.000000 pepperpepper-0.0.5/PepperPepper/models/__init__.py
--rw-rw-rw-   0        0        0     2461 2024-04-26 07:23:39.000000 pepperpepper-0.0.5/PepperPepper/models/cnn.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.5/PepperPepper/models/custom_model.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.5/PepperPepper/models/rnn.py
--rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.5/PepperPepper/models/transformer.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:14:10.968635 pepperpepper-0.0.5/PepperPepper/optimizers/
--rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.5/PepperPepper/optimizers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.5/PepperPepper/optimizers/custom_optimizer.py
--rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.5/PepperPepper/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:14:10.971114 pepperpepper-0.0.5/PepperPepper.egg-info/
--rw-rw-rw-   0        0        0      431 2024-04-30 02:14:10.000000 pepperpepper-0.0.5/PepperPepper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1225 2024-04-30 02:14:10.000000 pepperpepper-0.0.5/PepperPepper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 02:14:10.000000 pepperpepper-0.0.5/PepperPepper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2024-04-30 02:14:10.000000 pepperpepper-0.0.5/PepperPepper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-30 02:14:10.000000 pepperpepper-0.0.5/PepperPepper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.5/PepperPepper.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-04-30 02:14:10.972591 pepperpepper-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      567 2024-04-30 02:11:13.000000 pepperpepper-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:17:24.588329 pepperpepper-0.0.5.2/
+-rw-rw-rw-   0        0        0      433 2024-04-30 02:17:24.587394 pepperpepper-0.0.5.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-30 02:17:24.547763 pepperpepper-0.0.5.2/PepperPepper/
+-rw-rw-rw-   0        0        0     5179 2024-04-29 03:25:30.000000 pepperpepper-0.0.5.2/PepperPepper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:17:24.567183 pepperpepper-0.0.5.2/PepperPepper/callbacks/
+-rw-rw-rw-   0        0        0      985 2024-04-30 01:42:49.000000 pepperpepper-0.0.5.2/PepperPepper/callbacks/__init__.py
+-rw-rw-rw-   0        0        0      785 2024-04-30 01:42:05.000000 pepperpepper-0.0.5.2/PepperPepper/callbacks/custom_callback.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.5.2/PepperPepper/callbacks/learning_rate_scheduler.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:17:24.569681 pepperpepper-0.0.5.2/PepperPepper/core/
+-rw-rw-rw-   0        0        0      930 2024-04-30 02:10:06.000000 pepperpepper-0.0.5.2/PepperPepper/core/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.5.2/PepperPepper/core/base_model.py
+-rw-rw-rw-   0        0        0     4487 2024-04-30 02:03:25.000000 pepperpepper-0.0.5.2/PepperPepper/core/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:17:24.572695 pepperpepper-0.0.5.2/PepperPepper/datasets/
+-rw-rw-rw-   0        0        0     1008 2024-04-29 04:09:47.000000 pepperpepper-0.0.5.2/PepperPepper/datasets/__init__.py
+-rw-rw-rw-   0        0        0        4 2024-04-29 18:10:09.000000 pepperpepper-0.0.5.2/PepperPepper/datasets/custom_dataset.py
+-rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.5.2/PepperPepper/datasets/image_datasets.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.5.2/PepperPepper/datasets/text_datasets.py
+-rw-rw-rw-   0        0        0      106 2024-04-30 02:10:15.000000 pepperpepper-0.0.5.2/PepperPepper/environment.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:17:24.575960 pepperpepper-0.0.5.2/PepperPepper/examples/
+-rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.5.2/PepperPepper/examples/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.5.2/PepperPepper/examples/custom_task.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.5.2/PepperPepper/examples/image_classification.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.5.2/PepperPepper/examples/text_generation.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:17:24.577976 pepperpepper-0.0.5.2/PepperPepper/layers/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.5.2/PepperPepper/layers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.5.2/PepperPepper/layers/attention.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.5.2/PepperPepper/layers/custom_layer.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:17:24.579458 pepperpepper-0.0.5.2/PepperPepper/losses/
+-rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.5.2/PepperPepper/losses/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.5.2/PepperPepper/losses/custom_loss.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:17:24.584273 pepperpepper-0.0.5.2/PepperPepper/models/
+-rw-rw-rw-   0        0        0      752 2024-04-26 06:22:17.000000 pepperpepper-0.0.5.2/PepperPepper/models/__init__.py
+-rw-rw-rw-   0        0        0     2461 2024-04-26 07:23:39.000000 pepperpepper-0.0.5.2/PepperPepper/models/cnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.5.2/PepperPepper/models/custom_model.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.5.2/PepperPepper/models/rnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.5.2/PepperPepper/models/transformer.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:17:24.585803 pepperpepper-0.0.5.2/PepperPepper/optimizers/
+-rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.5.2/PepperPepper/optimizers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.5.2/PepperPepper/optimizers/custom_optimizer.py
+-rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.5.2/PepperPepper/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:17:24.586856 pepperpepper-0.0.5.2/PepperPepper.egg-info/
+-rw-rw-rw-   0        0        0      433 2024-04-30 02:17:24.000000 pepperpepper-0.0.5.2/PepperPepper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1225 2024-04-30 02:17:24.000000 pepperpepper-0.0.5.2/PepperPepper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 02:17:24.000000 pepperpepper-0.0.5.2/PepperPepper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2024-04-30 02:17:24.000000 pepperpepper-0.0.5.2/PepperPepper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-30 02:17:24.000000 pepperpepper-0.0.5.2/PepperPepper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.5.2/PepperPepper.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-04-30 02:17:24.588329 pepperpepper-0.0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      569 2024-04-30 02:17:10.000000 pepperpepper-0.0.5.2/setup.py
```

### Comparing `pepperpepper-0.0.5/PepperPepper/__init__.py` & `pepperpepper-0.0.5.2/PepperPepper/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5/PepperPepper/callbacks/__init__.py` & `pepperpepper-0.0.5.2/PepperPepper/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5/PepperPepper/callbacks/custom_callback.py` & `pepperpepper-0.0.5.2/PepperPepper/callbacks/custom_callback.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5/PepperPepper/core/__init__.py` & `pepperpepper-0.0.5.2/PepperPepper/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5/PepperPepper/core/utils.py` & `pepperpepper-0.0.5.2/PepperPepper/core/utils.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5/PepperPepper/datasets/__init__.py` & `pepperpepper-0.0.5.2/PepperPepper/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5/PepperPepper/datasets/image_datasets.py` & `pepperpepper-0.0.5.2/PepperPepper/datasets/image_datasets.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5/PepperPepper/examples/__init__.py` & `pepperpepper-0.0.5.2/PepperPepper/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5/PepperPepper/layers/__init__.py` & `pepperpepper-0.0.5.2/PepperPepper/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5/PepperPepper/losses/__init__.py` & `pepperpepper-0.0.5.2/PepperPepper/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5/PepperPepper/models/__init__.py` & `pepperpepper-0.0.5.2/PepperPepper/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5/PepperPepper/models/cnn.py` & `pepperpepper-0.0.5.2/PepperPepper/models/cnn.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5/PepperPepper/optimizers/__init__.py` & `pepperpepper-0.0.5.2/PepperPepper/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5/PepperPepper.egg-info/SOURCES.txt` & `pepperpepper-0.0.5.2/PepperPepper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5/setup.py` & `pepperpepper-0.0.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     'torchvision'
 ]
 
 
 
 setuptools.setup(
     name="PepperPepper",
-    version="0.0.5",
+    version="0.0.5.2",
     python_requires='>=3.11',
     author="Aohua Li",
     author_email="pepper2024jlu@163.com",
     description="It is a DeepLearning package to foster developed by Aohua Li",
     url="",
     packages=setuptools.find_packages(),
     zip_safe=True,
```

