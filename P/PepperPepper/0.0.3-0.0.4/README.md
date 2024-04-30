# Comparing `tmp/pepperpepper-0.0.3.tar.gz` & `tmp/pepperpepper-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepperpepper-0.0.3.tar", last modified: Mon Apr 29 04:12:29 2024, max compression
+gzip compressed data, was "pepperpepper-0.0.4.tar", last modified: Tue Apr 30 02:03:36 2024, max compression
```

## Comparing `pepperpepper-0.0.3.tar` & `pepperpepper-0.0.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 04:12:29.169279 pepperpepper-0.0.3/
--rw-rw-rw-   0        0        0      431 2024-04-29 04:12:29.169279 pepperpepper-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-29 04:12:29.073303 pepperpepper-0.0.3/PepperPepper/
--rw-rw-rw-   0        0        0     5179 2024-04-29 03:25:30.000000 pepperpepper-0.0.3/PepperPepper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 04:12:29.121448 pepperpepper-0.0.3/PepperPepper/callbacks/
--rw-rw-rw-   0        0        0     1085 2024-04-26 05:49:40.000000 pepperpepper-0.0.3/PepperPepper/callbacks/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:29.000000 pepperpepper-0.0.3/PepperPepper/callbacks/custom_callback.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.3/PepperPepper/callbacks/learning_rate_scheduler.py
-drwxrwxrwx   0        0        0        0 2024-04-29 04:12:29.128675 pepperpepper-0.0.3/PepperPepper/core/
--rw-rw-rw-   0        0        0      971 2024-04-26 05:47:32.000000 pepperpepper-0.0.3/PepperPepper/core/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.3/PepperPepper/core/base_model.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:22.000000 pepperpepper-0.0.3/PepperPepper/core/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-29 04:12:29.131966 pepperpepper-0.0.3/PepperPepper/datasets/
--rw-rw-rw-   0        0        0     1008 2024-04-29 04:09:47.000000 pepperpepper-0.0.3/PepperPepper/datasets/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:39.000000 pepperpepper-0.0.3/PepperPepper/datasets/custom_dataset.py
--rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.3/PepperPepper/datasets/image_datasets.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.3/PepperPepper/datasets/text_datasets.py
--rw-rw-rw-   0        0        0      106 2024-04-29 03:32:47.000000 pepperpepper-0.0.3/PepperPepper/environment.py
-drwxrwxrwx   0        0        0        0 2024-04-29 04:12:29.137205 pepperpepper-0.0.3/PepperPepper/examples/
--rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.3/PepperPepper/examples/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.3/PepperPepper/examples/custom_task.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.3/PepperPepper/examples/image_classification.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.3/PepperPepper/examples/text_generation.py
-drwxrwxrwx   0        0        0        0 2024-04-29 04:12:29.145192 pepperpepper-0.0.3/PepperPepper/layers/
--rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.3/PepperPepper/layers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.3/PepperPepper/layers/attention.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.3/PepperPepper/layers/custom_layer.py
-drwxrwxrwx   0        0        0        0 2024-04-29 04:12:29.145192 pepperpepper-0.0.3/PepperPepper/losses/
--rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.3/PepperPepper/losses/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.3/PepperPepper/losses/custom_loss.py
-drwxrwxrwx   0        0        0        0 2024-04-29 04:12:29.162847 pepperpepper-0.0.3/PepperPepper/models/
--rw-rw-rw-   0        0        0      752 2024-04-26 06:22:17.000000 pepperpepper-0.0.3/PepperPepper/models/__init__.py
--rw-rw-rw-   0        0        0     2461 2024-04-26 07:23:39.000000 pepperpepper-0.0.3/PepperPepper/models/cnn.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.3/PepperPepper/models/custom_model.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.3/PepperPepper/models/rnn.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:55.000000 pepperpepper-0.0.3/PepperPepper/models/transformer.py
-drwxrwxrwx   0        0        0        0 2024-04-29 04:12:29.168355 pepperpepper-0.0.3/PepperPepper/optimizers/
--rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.3/PepperPepper/optimizers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.3/PepperPepper/optimizers/custom_optimizer.py
--rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.3/PepperPepper/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-29 04:12:29.169279 pepperpepper-0.0.3/PepperPepper.egg-info/
--rw-rw-rw-   0        0        0      431 2024-04-29 04:12:28.000000 pepperpepper-0.0.3/PepperPepper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1225 2024-04-29 04:12:28.000000 pepperpepper-0.0.3/PepperPepper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 04:12:28.000000 pepperpepper-0.0.3/PepperPepper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2024-04-29 04:12:28.000000 pepperpepper-0.0.3/PepperPepper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-29 04:12:28.000000 pepperpepper-0.0.3/PepperPepper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.3/PepperPepper.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-04-29 04:12:29.169279 pepperpepper-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      567 2024-04-29 04:11:38.000000 pepperpepper-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:03:36.249245 pepperpepper-0.0.4/
+-rw-rw-rw-   0        0        0      431 2024-04-30 02:03:36.247246 pepperpepper-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-30 02:03:36.107609 pepperpepper-0.0.4/PepperPepper/
+-rw-rw-rw-   0        0        0     5179 2024-04-29 03:25:30.000000 pepperpepper-0.0.4/PepperPepper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:03:36.145685 pepperpepper-0.0.4/PepperPepper/callbacks/
+-rw-rw-rw-   0        0        0      985 2024-04-30 01:42:49.000000 pepperpepper-0.0.4/PepperPepper/callbacks/__init__.py
+-rw-rw-rw-   0        0        0      785 2024-04-30 01:42:05.000000 pepperpepper-0.0.4/PepperPepper/callbacks/custom_callback.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.4/PepperPepper/callbacks/learning_rate_scheduler.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:03:36.148130 pepperpepper-0.0.4/PepperPepper/core/
+-rw-rw-rw-   0        0        0      876 2024-04-29 18:22:11.000000 pepperpepper-0.0.4/PepperPepper/core/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.4/PepperPepper/core/base_model.py
+-rw-rw-rw-   0        0        0     4487 2024-04-30 02:03:25.000000 pepperpepper-0.0.4/PepperPepper/core/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:03:36.176669 pepperpepper-0.0.4/PepperPepper/datasets/
+-rw-rw-rw-   0        0        0     1008 2024-04-29 04:09:47.000000 pepperpepper-0.0.4/PepperPepper/datasets/__init__.py
+-rw-rw-rw-   0        0        0        4 2024-04-29 18:10:09.000000 pepperpepper-0.0.4/PepperPepper/datasets/custom_dataset.py
+-rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.4/PepperPepper/datasets/image_datasets.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.4/PepperPepper/datasets/text_datasets.py
+-rw-rw-rw-   0        0        0      152 2024-04-30 01:59:46.000000 pepperpepper-0.0.4/PepperPepper/environment.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:03:36.195653 pepperpepper-0.0.4/PepperPepper/examples/
+-rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.4/PepperPepper/examples/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.4/PepperPepper/examples/custom_task.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.4/PepperPepper/examples/image_classification.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.4/PepperPepper/examples/text_generation.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:03:36.208483 pepperpepper-0.0.4/PepperPepper/layers/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.4/PepperPepper/layers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.4/PepperPepper/layers/attention.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.4/PepperPepper/layers/custom_layer.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:03:36.216510 pepperpepper-0.0.4/PepperPepper/losses/
+-rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.4/PepperPepper/losses/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.4/PepperPepper/losses/custom_loss.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:03:36.237225 pepperpepper-0.0.4/PepperPepper/models/
+-rw-rw-rw-   0        0        0      752 2024-04-26 06:22:17.000000 pepperpepper-0.0.4/PepperPepper/models/__init__.py
+-rw-rw-rw-   0        0        0     2461 2024-04-26 07:23:39.000000 pepperpepper-0.0.4/PepperPepper/models/cnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.4/PepperPepper/models/custom_model.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.4/PepperPepper/models/rnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.4/PepperPepper/models/transformer.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:03:36.243731 pepperpepper-0.0.4/PepperPepper/optimizers/
+-rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.4/PepperPepper/optimizers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.4/PepperPepper/optimizers/custom_optimizer.py
+-rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.4/PepperPepper/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:03:36.244744 pepperpepper-0.0.4/PepperPepper.egg-info/
+-rw-rw-rw-   0        0        0      431 2024-04-30 02:03:35.000000 pepperpepper-0.0.4/PepperPepper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1225 2024-04-30 02:03:35.000000 pepperpepper-0.0.4/PepperPepper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 02:03:35.000000 pepperpepper-0.0.4/PepperPepper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2024-04-30 02:03:35.000000 pepperpepper-0.0.4/PepperPepper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-30 02:03:35.000000 pepperpepper-0.0.4/PepperPepper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.4/PepperPepper.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-04-30 02:03:36.249245 pepperpepper-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      567 2024-04-30 02:03:13.000000 pepperpepper-0.0.4/setup.py
```

### Comparing `pepperpepper-0.0.3/PepperPepper/__init__.py` & `pepperpepper-0.0.4/PepperPepper/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.3/PepperPepper/callbacks/__init__.py` & `pepperpepper-0.0.4/PepperPepper/callbacks/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,27 +13,25 @@
 
 
 
 
 
 
 
-# # callbacks/__init__.py
-#
-# # 导入 callback 子包中的各个模块
+# callbacks/__init__.py
+
+# 导入 callback 子包中的各个模块
 # from . import logging_callback
 # from . import model_checkpoint_callback
 # from . import early_stopping_callback
 #
-# # 如果需要，可以直接导入这些模块中的特定回调类
+# 如果需要，可以直接导入这些模块中的特定回调类
+from .custom_callback import save_best_model
 # from .logging_callback import LoggingCallback
 # from .model_checkpoint_callback import ModelCheckpointCallback
 # from .early_stopping_callback import EarlyStoppingCallback
 #
 # # __all__ 变量定义了当使用 from callback import * 时导入哪些对象
 # # 注意：通常不推荐使用 from package import *
-# __all__ = [
-#     'LoggingCallback',
-#     'ModelCheckpointCallback',
-#     'EarlyStoppingCallback',
-#     # ... 其他希望用户直接访问的关键回调类 ...
-# ]
+__all__ = [
+    'save_best_model'
+]
```

### Comparing `pepperpepper-0.0.3/PepperPepper/core/__init__.py` & `pepperpepper-0.0.4/PepperPepper/core/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,27 +7,26 @@
 """
 
 
 
 
 
 
-# # core/__init__.py
-#
-# # 导入 core 子包中的关键模块
+# core/__init__.py
+
+# 导入 core 子包中的关键模块
 # from . import data_structures
 # from . import utils
 # from . import model_builder
 #
-# # 如果需要，可以直接导入这些模块中的特定类或函数
+# 如果需要，可以直接导入这些模块中的特定类或函数
+
+from .utils import evaluate_accuracy_gpu
 # from .data_structures import CustomDataStructure
 # from .utils import some_utility_function
 # from .model_builder import build_model
 #
-# # __all__ 变量定义了当使用 from core import * 时导入哪些对象
-# # 注意：通常不推荐使用 from package import *
-# __all__ = [
-#     'CustomDataStructure',
-#     'some_utility_function',
-#     'build_model',
-#     # ... 其他希望用户直接访问的核心类或函数 ...
-# ]
+# __all__ 变量定义了当使用 from core import * 时导入哪些对象
+# 注意：通常不推荐使用 from package import *
+__all__ = [
+    'evaluate_accuracy_gpu'
+]
```

### Comparing `pepperpepper-0.0.3/PepperPepper/datasets/__init__.py` & `pepperpepper-0.0.4/PepperPepper/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.3/PepperPepper/datasets/image_datasets.py` & `pepperpepper-0.0.4/PepperPepper/datasets/image_datasets.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.3/PepperPepper/examples/__init__.py` & `pepperpepper-0.0.4/PepperPepper/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.3/PepperPepper/layers/__init__.py` & `pepperpepper-0.0.4/PepperPepper/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.3/PepperPepper/losses/__init__.py` & `pepperpepper-0.0.4/PepperPepper/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.3/PepperPepper/models/__init__.py` & `pepperpepper-0.0.4/PepperPepper/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.3/PepperPepper/models/cnn.py` & `pepperpepper-0.0.4/PepperPepper/models/cnn.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.3/PepperPepper/optimizers/__init__.py` & `pepperpepper-0.0.4/PepperPepper/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.3/PepperPepper.egg-info/SOURCES.txt` & `pepperpepper-0.0.4/PepperPepper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.3/setup.py` & `pepperpepper-0.0.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     'torchvision'
 ]
 
 
 
 setuptools.setup(
     name="PepperPepper",
-    version="0.0.3",
+    version="0.0.4",
     python_requires='>=3.11',
     author="Aohua Li",
     author_email="pepper2024jlu@163.com",
     description="It is a DeepLearning package to foster developed by Aohua Li",
     url="",
     packages=setuptools.find_packages(),
     zip_safe=True,
```

