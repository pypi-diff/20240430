# Comparing `tmp/pepperpepper-0.0.5.6.tar.gz` & `tmp/pepperpepper-0.0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepperpepper-0.0.5.6.tar", last modified: Tue Apr 30 03:56:36 2024, max compression
+gzip compressed data, was "pepperpepper-0.0.5.7.tar", last modified: Tue Apr 30 06:27:11 2024, max compression
```

## Comparing `pepperpepper-0.0.5.6.tar` & `pepperpepper-0.0.5.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 03:56:36.250071 pepperpepper-0.0.5.6/
--rw-rw-rw-   0        0        0      433 2024-04-30 03:56:36.249063 pepperpepper-0.0.5.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-30 03:56:36.199840 pepperpepper-0.0.5.6/PepperPepper/
--rw-rw-rw-   0        0        0     5179 2024-04-29 03:25:30.000000 pepperpepper-0.0.5.6/PepperPepper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 03:56:36.220720 pepperpepper-0.0.5.6/PepperPepper/callbacks/
--rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.5.6/PepperPepper/callbacks/__init__.py
--rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.5.6/PepperPepper/callbacks/custom_callback.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.5.6/PepperPepper/callbacks/learning_rate_scheduler.py
-drwxrwxrwx   0        0        0        0 2024-04-30 03:56:36.223296 pepperpepper-0.0.5.6/PepperPepper/core/
--rw-rw-rw-   0        0        0     1028 2024-04-30 03:56:08.000000 pepperpepper-0.0.5.6/PepperPepper/core/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.5.6/PepperPepper/core/base_model.py
--rw-rw-rw-   0        0        0     7029 2024-04-30 03:54:40.000000 pepperpepper-0.0.5.6/PepperPepper/core/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-30 03:56:36.230037 pepperpepper-0.0.5.6/PepperPepper/datasets/
--rw-rw-rw-   0        0        0     1008 2024-04-29 04:09:47.000000 pepperpepper-0.0.5.6/PepperPepper/datasets/__init__.py
--rw-rw-rw-   0        0        0        4 2024-04-29 18:10:09.000000 pepperpepper-0.0.5.6/PepperPepper/datasets/custom_dataset.py
--rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.5.6/PepperPepper/datasets/image_datasets.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.5.6/PepperPepper/datasets/text_datasets.py
--rw-rw-rw-   0        0        0      106 2024-04-30 02:10:15.000000 pepperpepper-0.0.5.6/PepperPepper/environment.py
-drwxrwxrwx   0        0        0        0 2024-04-30 03:56:36.233573 pepperpepper-0.0.5.6/PepperPepper/examples/
--rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.5.6/PepperPepper/examples/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.5.6/PepperPepper/examples/custom_task.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.5.6/PepperPepper/examples/image_classification.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.5.6/PepperPepper/examples/text_generation.py
-drwxrwxrwx   0        0        0        0 2024-04-30 03:56:36.236073 pepperpepper-0.0.5.6/PepperPepper/layers/
--rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.5.6/PepperPepper/layers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.5.6/PepperPepper/layers/attention.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.5.6/PepperPepper/layers/custom_layer.py
-drwxrwxrwx   0        0        0        0 2024-04-30 03:56:36.238681 pepperpepper-0.0.5.6/PepperPepper/losses/
--rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.5.6/PepperPepper/losses/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.5.6/PepperPepper/losses/custom_loss.py
-drwxrwxrwx   0        0        0        0 2024-04-30 03:56:36.244191 pepperpepper-0.0.5.6/PepperPepper/models/
--rw-rw-rw-   0        0        0      752 2024-04-26 06:22:17.000000 pepperpepper-0.0.5.6/PepperPepper/models/__init__.py
--rw-rw-rw-   0        0        0     2525 2024-04-30 02:40:06.000000 pepperpepper-0.0.5.6/PepperPepper/models/cnn.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.5.6/PepperPepper/models/custom_model.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.5.6/PepperPepper/models/rnn.py
--rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.5.6/PepperPepper/models/transformer.py
-drwxrwxrwx   0        0        0        0 2024-04-30 03:56:36.247494 pepperpepper-0.0.5.6/PepperPepper/optimizers/
--rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.5.6/PepperPepper/optimizers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.5.6/PepperPepper/optimizers/custom_optimizer.py
--rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.5.6/PepperPepper/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-30 03:56:36.248547 pepperpepper-0.0.5.6/PepperPepper.egg-info/
--rw-rw-rw-   0        0        0      433 2024-04-30 03:56:36.000000 pepperpepper-0.0.5.6/PepperPepper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1225 2024-04-30 03:56:36.000000 pepperpepper-0.0.5.6/PepperPepper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 03:56:36.000000 pepperpepper-0.0.5.6/PepperPepper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2024-04-30 03:56:36.000000 pepperpepper-0.0.5.6/PepperPepper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-30 03:56:36.000000 pepperpepper-0.0.5.6/PepperPepper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.5.6/PepperPepper.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-04-30 03:56:36.250071 pepperpepper-0.0.5.6/setup.cfg
--rw-rw-rw-   0        0        0      569 2024-04-30 03:56:16.000000 pepperpepper-0.0.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 06:27:11.816551 pepperpepper-0.0.5.7/
+-rw-rw-rw-   0        0        0      433 2024-04-30 06:27:11.815550 pepperpepper-0.0.5.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-30 06:27:11.755863 pepperpepper-0.0.5.7/PepperPepper/
+-rw-rw-rw-   0        0        0     5179 2024-04-29 03:25:30.000000 pepperpepper-0.0.5.7/PepperPepper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 06:27:11.786009 pepperpepper-0.0.5.7/PepperPepper/callbacks/
+-rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.5.7/PepperPepper/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.5.7/PepperPepper/callbacks/custom_callback.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.5.7/PepperPepper/callbacks/learning_rate_scheduler.py
+drwxrwxrwx   0        0        0        0 2024-04-30 06:27:11.789008 pepperpepper-0.0.5.7/PepperPepper/core/
+-rw-rw-rw-   0        0        0     1028 2024-04-30 03:56:08.000000 pepperpepper-0.0.5.7/PepperPepper/core/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.5.7/PepperPepper/core/base_model.py
+-rw-rw-rw-   0        0        0     7029 2024-04-30 03:54:40.000000 pepperpepper-0.0.5.7/PepperPepper/core/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-30 06:27:11.795350 pepperpepper-0.0.5.7/PepperPepper/datasets/
+-rw-rw-rw-   0        0        0     1008 2024-04-29 04:09:47.000000 pepperpepper-0.0.5.7/PepperPepper/datasets/__init__.py
+-rw-rw-rw-   0        0        0        4 2024-04-29 18:10:09.000000 pepperpepper-0.0.5.7/PepperPepper/datasets/custom_dataset.py
+-rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.5.7/PepperPepper/datasets/image_datasets.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.5.7/PepperPepper/datasets/text_datasets.py
+-rw-rw-rw-   0        0        0      106 2024-04-30 02:10:15.000000 pepperpepper-0.0.5.7/PepperPepper/environment.py
+drwxrwxrwx   0        0        0        0 2024-04-30 06:27:11.800357 pepperpepper-0.0.5.7/PepperPepper/examples/
+-rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.5.7/PepperPepper/examples/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.5.7/PepperPepper/examples/custom_task.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.5.7/PepperPepper/examples/image_classification.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.5.7/PepperPepper/examples/text_generation.py
+drwxrwxrwx   0        0        0        0 2024-04-30 06:27:11.803993 pepperpepper-0.0.5.7/PepperPepper/layers/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.5.7/PepperPepper/layers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.5.7/PepperPepper/layers/attention.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.5.7/PepperPepper/layers/custom_layer.py
+drwxrwxrwx   0        0        0        0 2024-04-30 06:27:11.806493 pepperpepper-0.0.5.7/PepperPepper/losses/
+-rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.5.7/PepperPepper/losses/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.5.7/PepperPepper/losses/custom_loss.py
+drwxrwxrwx   0        0        0        0 2024-04-30 06:27:11.811550 pepperpepper-0.0.5.7/PepperPepper/models/
+-rw-rw-rw-   0        0        0      793 2024-04-30 06:26:44.000000 pepperpepper-0.0.5.7/PepperPepper/models/__init__.py
+-rw-rw-rw-   0        0        0     6490 2024-04-30 06:26:10.000000 pepperpepper-0.0.5.7/PepperPepper/models/cnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.5.7/PepperPepper/models/custom_model.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.5.7/PepperPepper/models/rnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.5.7/PepperPepper/models/transformer.py
+drwxrwxrwx   0        0        0        0 2024-04-30 06:27:11.814051 pepperpepper-0.0.5.7/PepperPepper/optimizers/
+-rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.5.7/PepperPepper/optimizers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.5.7/PepperPepper/optimizers/custom_optimizer.py
+-rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.5.7/PepperPepper/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-30 06:27:11.815051 pepperpepper-0.0.5.7/PepperPepper.egg-info/
+-rw-rw-rw-   0        0        0      433 2024-04-30 06:27:11.000000 pepperpepper-0.0.5.7/PepperPepper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1225 2024-04-30 06:27:11.000000 pepperpepper-0.0.5.7/PepperPepper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 06:27:11.000000 pepperpepper-0.0.5.7/PepperPepper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2024-04-30 06:27:11.000000 pepperpepper-0.0.5.7/PepperPepper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-30 06:27:11.000000 pepperpepper-0.0.5.7/PepperPepper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.5.7/PepperPepper.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-04-30 06:27:11.816551 pepperpepper-0.0.5.7/setup.cfg
+-rw-rw-rw-   0        0        0      569 2024-04-30 06:27:01.000000 pepperpepper-0.0.5.7/setup.py
```

### Comparing `pepperpepper-0.0.5.6/PepperPepper/__init__.py` & `pepperpepper-0.0.5.7/PepperPepper/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.6/PepperPepper/callbacks/__init__.py` & `pepperpepper-0.0.5.7/PepperPepper/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.6/PepperPepper/callbacks/custom_callback.py` & `pepperpepper-0.0.5.7/PepperPepper/callbacks/custom_callback.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.6/PepperPepper/core/__init__.py` & `pepperpepper-0.0.5.7/PepperPepper/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.6/PepperPepper/core/utils.py` & `pepperpepper-0.0.5.7/PepperPepper/core/utils.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.6/PepperPepper/datasets/__init__.py` & `pepperpepper-0.0.5.7/PepperPepper/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.6/PepperPepper/datasets/image_datasets.py` & `pepperpepper-0.0.5.7/PepperPepper/datasets/image_datasets.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.6/PepperPepper/examples/__init__.py` & `pepperpepper-0.0.5.7/PepperPepper/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.6/PepperPepper/layers/__init__.py` & `pepperpepper-0.0.5.7/PepperPepper/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.6/PepperPepper/losses/__init__.py` & `pepperpepper-0.0.5.7/PepperPepper/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.6/PepperPepper/models/__init__.py` & `pepperpepper-0.0.5.7/PepperPepper/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 # rnn.py：循环神经网络（RNN）相关模型的实现。
 # transformer.py：Transformer模型及其变体的实现。
 # custom_model.py：用户自定义模型的示例或模板。
 
 # models/__init__.py
 # 如果需要，您可以直接导入这些模块中的特定类或函数
 from .cnn import LeNet5
+from .cnn import AlexNet
 #from .rnn import RNNModel
 #from .transformer import TransformerModel
 #from .custom_model import CustomModel
 
 
 # __all__ 变量定义了当使用 from models import * 时导入哪些对象
 # 注意：通常不推荐使用 from package import *
 __all__ = [
-   'LeNet5'
+   'LeNet5',
+   'AlexNet'
 ]
```

### Comparing `pepperpepper-0.0.5.6/PepperPepper/optimizers/__init__.py` & `pepperpepper-0.0.5.7/PepperPepper/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.6/PepperPepper.egg-info/SOURCES.txt` & `pepperpepper-0.0.5.7/PepperPepper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.6/setup.py` & `pepperpepper-0.0.5.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     'torchvision'
 ]
 
 
 
 setuptools.setup(
     name="PepperPepper",
-    version="0.0.5.6",
+    version="0.0.5.7",
     python_requires='>=3.11',
     author="Aohua Li",
     author_email="pepper2024jlu@163.com",
     description="It is a DeepLearning package to foster developed by Aohua Li",
     url="",
     packages=setuptools.find_packages(),
     zip_safe=True,
```

