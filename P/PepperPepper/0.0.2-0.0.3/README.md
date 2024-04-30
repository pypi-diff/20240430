# Comparing `tmp/pepperpepper-0.0.2.tar.gz` & `tmp/pepperpepper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepperpepper-0.0.2.tar", last modified: Fri Apr 26 06:24:31 2024, max compression
+gzip compressed data, was "pepperpepper-0.0.3.tar", last modified: Mon Apr 29 04:12:29 2024, max compression
```

## Comparing `pepperpepper-0.0.2.tar` & `pepperpepper-0.0.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 06:24:31.361490 pepperpepper-0.0.2/
--rw-rw-rw-   0        0        0      403 2024-04-26 06:24:31.361490 pepperpepper-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-26 06:24:31.302583 pepperpepper-0.0.2/PepperPepper/
--rw-rw-rw-   0        0        0     5165 2024-04-26 05:53:03.000000 pepperpepper-0.0.2/PepperPepper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 06:24:31.341390 pepperpepper-0.0.2/PepperPepper/callbacks/
--rw-rw-rw-   0        0        0     1085 2024-04-26 05:49:40.000000 pepperpepper-0.0.2/PepperPepper/callbacks/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:29.000000 pepperpepper-0.0.2/PepperPepper/callbacks/custom_callback.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.2/PepperPepper/callbacks/learning_rate_scheduler.py
-drwxrwxrwx   0        0        0        0 2024-04-26 06:24:31.341390 pepperpepper-0.0.2/PepperPepper/core/
--rw-rw-rw-   0        0        0      971 2024-04-26 05:47:32.000000 pepperpepper-0.0.2/PepperPepper/core/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.2/PepperPepper/core/base_model.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:22.000000 pepperpepper-0.0.2/PepperPepper/core/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-26 06:24:31.341390 pepperpepper-0.0.2/PepperPepper/datasets/
--rw-rw-rw-   0        0        0     1062 2024-04-26 05:48:57.000000 pepperpepper-0.0.2/PepperPepper/datasets/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:39.000000 pepperpepper-0.0.2/PepperPepper/datasets/custom_dataset.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:23.000000 pepperpepper-0.0.2/PepperPepper/datasets/image_datasets.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.2/PepperPepper/datasets/text_datasets.py
--rw-rw-rw-   0        0        0       88 2024-04-26 06:06:02.000000 pepperpepper-0.0.2/PepperPepper/environment.py
-drwxrwxrwx   0        0        0        0 2024-04-26 06:24:31.351663 pepperpepper-0.0.2/PepperPepper/examples/
--rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.2/PepperPepper/examples/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.2/PepperPepper/examples/custom_task.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.2/PepperPepper/examples/image_classification.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.2/PepperPepper/examples/text_generation.py
-drwxrwxrwx   0        0        0        0 2024-04-26 06:24:31.351663 pepperpepper-0.0.2/PepperPepper/layers/
--rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.2/PepperPepper/layers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.2/PepperPepper/layers/attention.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.2/PepperPepper/layers/custom_layer.py
-drwxrwxrwx   0        0        0        0 2024-04-26 06:24:31.351663 pepperpepper-0.0.2/PepperPepper/losses/
--rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.2/PepperPepper/losses/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.2/PepperPepper/losses/custom_loss.py
-drwxrwxrwx   0        0        0        0 2024-04-26 06:24:31.351663 pepperpepper-0.0.2/PepperPepper/models/
--rw-rw-rw-   0        0        0      752 2024-04-26 06:22:17.000000 pepperpepper-0.0.2/PepperPepper/models/__init__.py
--rw-rw-rw-   0        0        0     1997 2024-04-26 06:21:36.000000 pepperpepper-0.0.2/PepperPepper/models/cnn.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.2/PepperPepper/models/custom_model.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.2/PepperPepper/models/rnn.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:55.000000 pepperpepper-0.0.2/PepperPepper/models/transformer.py
-drwxrwxrwx   0        0        0        0 2024-04-26 06:24:31.351663 pepperpepper-0.0.2/PepperPepper/optimizers/
--rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.2/PepperPepper/optimizers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.2/PepperPepper/optimizers/custom_optimizer.py
--rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.2/PepperPepper/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-26 06:24:31.361490 pepperpepper-0.0.2/PepperPepper.egg-info/
--rw-rw-rw-   0        0        0      403 2024-04-26 06:24:31.000000 pepperpepper-0.0.2/PepperPepper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1225 2024-04-26 06:24:31.000000 pepperpepper-0.0.2/PepperPepper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 06:24:31.000000 pepperpepper-0.0.2/PepperPepper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2024-04-26 06:24:31.000000 pepperpepper-0.0.2/PepperPepper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-26 06:24:31.000000 pepperpepper-0.0.2/PepperPepper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.2/PepperPepper.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-04-26 06:24:31.361490 pepperpepper-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      547 2024-04-26 06:23:28.000000 pepperpepper-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 04:12:29.169279 pepperpepper-0.0.3/
+-rw-rw-rw-   0        0        0      431 2024-04-29 04:12:29.169279 pepperpepper-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-29 04:12:29.073303 pepperpepper-0.0.3/PepperPepper/
+-rw-rw-rw-   0        0        0     5179 2024-04-29 03:25:30.000000 pepperpepper-0.0.3/PepperPepper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 04:12:29.121448 pepperpepper-0.0.3/PepperPepper/callbacks/
+-rw-rw-rw-   0        0        0     1085 2024-04-26 05:49:40.000000 pepperpepper-0.0.3/PepperPepper/callbacks/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:29.000000 pepperpepper-0.0.3/PepperPepper/callbacks/custom_callback.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.3/PepperPepper/callbacks/learning_rate_scheduler.py
+drwxrwxrwx   0        0        0        0 2024-04-29 04:12:29.128675 pepperpepper-0.0.3/PepperPepper/core/
+-rw-rw-rw-   0        0        0      971 2024-04-26 05:47:32.000000 pepperpepper-0.0.3/PepperPepper/core/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.3/PepperPepper/core/base_model.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:22.000000 pepperpepper-0.0.3/PepperPepper/core/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 04:12:29.131966 pepperpepper-0.0.3/PepperPepper/datasets/
+-rw-rw-rw-   0        0        0     1008 2024-04-29 04:09:47.000000 pepperpepper-0.0.3/PepperPepper/datasets/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:39.000000 pepperpepper-0.0.3/PepperPepper/datasets/custom_dataset.py
+-rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.3/PepperPepper/datasets/image_datasets.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.3/PepperPepper/datasets/text_datasets.py
+-rw-rw-rw-   0        0        0      106 2024-04-29 03:32:47.000000 pepperpepper-0.0.3/PepperPepper/environment.py
+drwxrwxrwx   0        0        0        0 2024-04-29 04:12:29.137205 pepperpepper-0.0.3/PepperPepper/examples/
+-rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.3/PepperPepper/examples/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.3/PepperPepper/examples/custom_task.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.3/PepperPepper/examples/image_classification.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.3/PepperPepper/examples/text_generation.py
+drwxrwxrwx   0        0        0        0 2024-04-29 04:12:29.145192 pepperpepper-0.0.3/PepperPepper/layers/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.3/PepperPepper/layers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.3/PepperPepper/layers/attention.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.3/PepperPepper/layers/custom_layer.py
+drwxrwxrwx   0        0        0        0 2024-04-29 04:12:29.145192 pepperpepper-0.0.3/PepperPepper/losses/
+-rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.3/PepperPepper/losses/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.3/PepperPepper/losses/custom_loss.py
+drwxrwxrwx   0        0        0        0 2024-04-29 04:12:29.162847 pepperpepper-0.0.3/PepperPepper/models/
+-rw-rw-rw-   0        0        0      752 2024-04-26 06:22:17.000000 pepperpepper-0.0.3/PepperPepper/models/__init__.py
+-rw-rw-rw-   0        0        0     2461 2024-04-26 07:23:39.000000 pepperpepper-0.0.3/PepperPepper/models/cnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.3/PepperPepper/models/custom_model.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.3/PepperPepper/models/rnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:55.000000 pepperpepper-0.0.3/PepperPepper/models/transformer.py
+drwxrwxrwx   0        0        0        0 2024-04-29 04:12:29.168355 pepperpepper-0.0.3/PepperPepper/optimizers/
+-rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.3/PepperPepper/optimizers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.3/PepperPepper/optimizers/custom_optimizer.py
+-rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.3/PepperPepper/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-29 04:12:29.169279 pepperpepper-0.0.3/PepperPepper.egg-info/
+-rw-rw-rw-   0        0        0      431 2024-04-29 04:12:28.000000 pepperpepper-0.0.3/PepperPepper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1225 2024-04-29 04:12:28.000000 pepperpepper-0.0.3/PepperPepper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 04:12:28.000000 pepperpepper-0.0.3/PepperPepper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2024-04-29 04:12:28.000000 pepperpepper-0.0.3/PepperPepper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-29 04:12:28.000000 pepperpepper-0.0.3/PepperPepper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.3/PepperPepper.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-04-29 04:12:29.169279 pepperpepper-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      567 2024-04-29 04:11:38.000000 pepperpepper-0.0.3/setup.py
```

### Comparing `pepperpepper-0.0.2/PepperPepper/__init__.py` & `pepperpepper-0.0.3/PepperPepper/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,45 +43,52 @@
 模块:
 
 core 模块
 功能：包含包的核心功能和基础类。
 子模块/文件：
 base_model.py：定义基础模型类，提供模型初始化、保存、加载等基础功能。
 utils.py：包含一些通用的工具函数，如数据处理、模型评估等。
+
 models 模块
 功能：包含各种深度学习模型的实现。
 子模块/文件：
 cnn.py：卷积神经网络（CNN）相关模型的实现。
 rnn.py：循环神经网络（RNN）相关模型的实现。
 transformer.py：Transformer模型及其变体的实现。
 custom_model.py：用户自定义模型的示例或模板。
+
 layers 模块
 功能：包含自定义的神经网络层或模块。
 子模块/文件：
 attention.py：实现各种注意力机制层。
 custom_layer.py：用户自定义层的示例或模板。
+
 datasets 模块
 功能：包含数据集的加载、预处理和增强功能。
 子模块/文件：
 image_datasets.py：图像数据集的处理，如CIFAR、ImageNet等。
 text_datasets.py：文本数据集的处理，如IMDB、WikiText等。
 custom_dataset.py：用户自定义数据集的示例或模板。
+
 optimizers 模块
 功能：包含优化器的实现或扩展。
 子模块/文件：
 custom_optimizer.py：用户自定义优化器的示例或模板。
+
 losses 模块
 功能：包含损失函数的实现或扩展。
 子模块/文件：
 custom_loss.py：用户自定义损失函数的示例或模板。
+
 callbacks 模块
 功能：包含训练过程中的回调函数，用于实现如学习率调整、模型保存等功能。
 子模块/文件：
 learning_rate_scheduler.py：学习率调整策略的实现。
 custom_callback.py：用户自定义回调函数的示例或模板。
+
 examples 模块
 功能：包含使用custom_deep_learning包进行深度学习任务的示例代码。
 子模块/文件：
 image_classification.py：使用CNN进行图像分类的示例。
 text_generation.py：使用Transformer进行文本生成的示例。
 custom_task.py：用户自定义任务的示例。
 这样的包结构使得每个模块都有其明确的功能和职责，方便用户根据需要进行查找和使用。同时，用户还可以根据具体需求在已有模块的基础上进行扩展或添加新的模块。
```

### Comparing `pepperpepper-0.0.2/PepperPepper/callbacks/__init__.py` & `pepperpepper-0.0.3/PepperPepper/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.2/PepperPepper/core/__init__.py` & `pepperpepper-0.0.3/PepperPepper/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.2/PepperPepper/datasets/__init__.py` & `pepperpepper-0.0.3/PepperPepper/datasets/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,27 +10,31 @@
 
 
 
 
 
 
 
-# # datasets/__init__.py
-#
-# # 导入 datasets 子包中的各个模块
+# datasets/__init__.py
+
+# 导入 datasets 子包中的各个模块
 # from . import mnist_dataset
 # from . import cifar10_dataset
 # from . import custom_dataset
-#
-# # 如果需要，可以直接导入这些模块中的特定类或函数
-# from .mnist_dataset import load_mnist_data
+
+
+
+
+# 如果需要，可以直接导入这些模块中的特定类或函数
+from .image_datasets import load_data_minist
+from .image_datasets import load_data_fashion_mnist
 # from .cifar10_dataset import load_cifar10_data
 # from .custom_dataset import load_custom_data
 #
-# # __all__ 变量定义了当使用 from datasets import * 时导入哪些对象
-# # 注意：通常不推荐使用 from package import *
-# __all__ = [
-#     'load_mnist_data',
-#     'load_cifar10_data',
-#     'load_custom_data',
-#     # ... 其他希望用户直接访问的关键数据集类或函数 ...
-# ]
+# __all__ 变量定义了当使用 from datasets import * 时导入哪些对象
+# 注意：通常不推荐使用 from package import *
+__all__ = [
+    'load_data_minist',
+    'load_data_fashion_mnist'
+]
+
+
```

### Comparing `pepperpepper-0.0.2/PepperPepper/examples/__init__.py` & `pepperpepper-0.0.3/PepperPepper/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.2/PepperPepper/layers/__init__.py` & `pepperpepper-0.0.3/PepperPepper/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.2/PepperPepper/losses/__init__.py` & `pepperpepper-0.0.3/PepperPepper/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.2/PepperPepper/models/__init__.py` & `pepperpepper-0.0.3/PepperPepper/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.2/PepperPepper/models/cnn.py` & `pepperpepper-0.0.3/PepperPepper/models/cnn.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 """
 1.LeNet
 abstract:
-        LeNet是一个经典的卷积神经网络，由多个卷积层、池化层和全连接层组成。它通过卷积操作提取图像中的局部特征，利用池化层进行特征下采样，并通过全连接层进行分类。LeNet最初用于手写数字识别任务，并展现出了良好的性能。其结构简洁明了，为后续更复杂的神经网络结构提供了基础，对深度学习领域的发展产生了重要影响。
+        LeNet5是一个经典的卷积神经网络，由多个卷积层、池化层和全连接层组成。它通过卷积操作提取图像中的局部特征，利用池化层进行特征下采样，并通过全连接层进行分类。LeNet最初用于手写数字识别任务，并展现出了良好的性能。其结构简洁明了，为后续更复杂的神经网络结构提供了基础，对深度学习领域的发展产生了重要影响。
 
 struct:
         卷积编码器：由两个卷积层组成;
         全连接层密集块：由三个全连接层组成。
 
 input: 
         28*28的单通道（黑白）图像通过LeNet。
@@ -40,7 +40,18 @@
         x = torch.nn.functional.relu(self.fc1(x))
         x = torch.nn.functional.relu(self.fc2(x))
         x = self.fc3(x)
 
         return x
 
 
+    def initialize_weights(self):
+        for m in self.modules():
+            if isinstance(m, torch.nn.Conv2d):
+                torch.nn.init.xavier_uniform_(m.weight)
+                if m.bias is not None:
+                    torch.nn.init.zeros_(m.bias)
+            elif isinstance(m, torch.nn.Linear):
+                torch.nn.init.xavier_uniform_(m.weight)
+                if m.bias is not None:
+                    torch.nn.init.zeros_(m.bias)
+
```

### Comparing `pepperpepper-0.0.2/PepperPepper/optimizers/__init__.py` & `pepperpepper-0.0.3/PepperPepper/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.2/PepperPepper.egg-info/SOURCES.txt` & `pepperpepper-0.0.3/PepperPepper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.2/setup.py` & `pepperpepper-0.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 
 requirements = [
     'jupyter>=1.0.0',
     'numpy>=1.21.5',
     'matplotlib>=3.5.1',
     'requests>=2.25.1',
     'pandas>=1.2.4',
-    'torch'
+    'torch',
+    'torchvision'
 ]
 
 
 
 setuptools.setup(
     name="PepperPepper",
-    version="0.0.2",
+    version="0.0.3",
     python_requires='>=3.11',
     author="Aohua Li",
     author_email="pepper2024jlu@163.com",
     description="It is a DeepLearning package to foster developed by Aohua Li",
     url="",
     packages=setuptools.find_packages(),
     zip_safe=True,
```

