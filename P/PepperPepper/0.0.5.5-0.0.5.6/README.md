# Comparing `tmp/pepperpepper-0.0.5.5.tar.gz` & `tmp/pepperpepper-0.0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepperpepper-0.0.5.5.tar", last modified: Tue Apr 30 02:50:03 2024, max compression
+gzip compressed data, was "pepperpepper-0.0.5.6.tar", last modified: Tue Apr 30 03:56:36 2024, max compression
```

## Comparing `pepperpepper-0.0.5.5.tar` & `pepperpepper-0.0.5.6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 02:50:03.102537 pepperpepper-0.0.5.5/
--rw-rw-rw-   0        0        0      433 2024-04-30 02:50:03.101543 pepperpepper-0.0.5.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-30 02:50:03.057243 pepperpepper-0.0.5.5/PepperPepper/
--rw-rw-rw-   0        0        0     5179 2024-04-29 03:25:30.000000 pepperpepper-0.0.5.5/PepperPepper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:50:03.077855 pepperpepper-0.0.5.5/PepperPepper/callbacks/
--rw-rw-rw-   0        0        0      985 2024-04-30 01:42:49.000000 pepperpepper-0.0.5.5/PepperPepper/callbacks/__init__.py
--rw-rw-rw-   0        0        0      785 2024-04-30 01:42:05.000000 pepperpepper-0.0.5.5/PepperPepper/callbacks/custom_callback.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.5.5/PepperPepper/callbacks/learning_rate_scheduler.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:50:03.080317 pepperpepper-0.0.5.5/PepperPepper/core/
--rw-rw-rw-   0        0        0      930 2024-04-30 02:10:06.000000 pepperpepper-0.0.5.5/PepperPepper/core/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.5.5/PepperPepper/core/base_model.py
--rw-rw-rw-   0        0        0     5266 2024-04-30 02:49:08.000000 pepperpepper-0.0.5.5/PepperPepper/core/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:50:03.083312 pepperpepper-0.0.5.5/PepperPepper/datasets/
--rw-rw-rw-   0        0        0     1008 2024-04-29 04:09:47.000000 pepperpepper-0.0.5.5/PepperPepper/datasets/__init__.py
--rw-rw-rw-   0        0        0        4 2024-04-29 18:10:09.000000 pepperpepper-0.0.5.5/PepperPepper/datasets/custom_dataset.py
--rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.5.5/PepperPepper/datasets/image_datasets.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.5.5/PepperPepper/datasets/text_datasets.py
--rw-rw-rw-   0        0        0      106 2024-04-30 02:10:15.000000 pepperpepper-0.0.5.5/PepperPepper/environment.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:50:03.087536 pepperpepper-0.0.5.5/PepperPepper/examples/
--rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.5.5/PepperPepper/examples/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.5.5/PepperPepper/examples/custom_task.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.5.5/PepperPepper/examples/image_classification.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.5.5/PepperPepper/examples/text_generation.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:50:03.090535 pepperpepper-0.0.5.5/PepperPepper/layers/
--rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.5.5/PepperPepper/layers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.5.5/PepperPepper/layers/attention.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.5.5/PepperPepper/layers/custom_layer.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:50:03.092986 pepperpepper-0.0.5.5/PepperPepper/losses/
--rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.5.5/PepperPepper/losses/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.5.5/PepperPepper/losses/custom_loss.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:50:03.097537 pepperpepper-0.0.5.5/PepperPepper/models/
--rw-rw-rw-   0        0        0      752 2024-04-26 06:22:17.000000 pepperpepper-0.0.5.5/PepperPepper/models/__init__.py
--rw-rw-rw-   0        0        0     2525 2024-04-30 02:40:06.000000 pepperpepper-0.0.5.5/PepperPepper/models/cnn.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.5.5/PepperPepper/models/custom_model.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.5.5/PepperPepper/models/rnn.py
--rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.5.5/PepperPepper/models/transformer.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:50:03.099567 pepperpepper-0.0.5.5/PepperPepper/optimizers/
--rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.5.5/PepperPepper/optimizers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.5.5/PepperPepper/optimizers/custom_optimizer.py
--rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.5.5/PepperPepper/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:50:03.100555 pepperpepper-0.0.5.5/PepperPepper.egg-info/
--rw-rw-rw-   0        0        0      433 2024-04-30 02:50:02.000000 pepperpepper-0.0.5.5/PepperPepper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1225 2024-04-30 02:50:02.000000 pepperpepper-0.0.5.5/PepperPepper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 02:50:02.000000 pepperpepper-0.0.5.5/PepperPepper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2024-04-30 02:50:02.000000 pepperpepper-0.0.5.5/PepperPepper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-30 02:50:02.000000 pepperpepper-0.0.5.5/PepperPepper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.5.5/PepperPepper.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-04-30 02:50:03.102537 pepperpepper-0.0.5.5/setup.cfg
--rw-rw-rw-   0        0        0      569 2024-04-30 02:49:26.000000 pepperpepper-0.0.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 03:56:36.250071 pepperpepper-0.0.5.6/
+-rw-rw-rw-   0        0        0      433 2024-04-30 03:56:36.249063 pepperpepper-0.0.5.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-30 03:56:36.199840 pepperpepper-0.0.5.6/PepperPepper/
+-rw-rw-rw-   0        0        0     5179 2024-04-29 03:25:30.000000 pepperpepper-0.0.5.6/PepperPepper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 03:56:36.220720 pepperpepper-0.0.5.6/PepperPepper/callbacks/
+-rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.5.6/PepperPepper/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.5.6/PepperPepper/callbacks/custom_callback.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.5.6/PepperPepper/callbacks/learning_rate_scheduler.py
+drwxrwxrwx   0        0        0        0 2024-04-30 03:56:36.223296 pepperpepper-0.0.5.6/PepperPepper/core/
+-rw-rw-rw-   0        0        0     1028 2024-04-30 03:56:08.000000 pepperpepper-0.0.5.6/PepperPepper/core/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.5.6/PepperPepper/core/base_model.py
+-rw-rw-rw-   0        0        0     7029 2024-04-30 03:54:40.000000 pepperpepper-0.0.5.6/PepperPepper/core/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-30 03:56:36.230037 pepperpepper-0.0.5.6/PepperPepper/datasets/
+-rw-rw-rw-   0        0        0     1008 2024-04-29 04:09:47.000000 pepperpepper-0.0.5.6/PepperPepper/datasets/__init__.py
+-rw-rw-rw-   0        0        0        4 2024-04-29 18:10:09.000000 pepperpepper-0.0.5.6/PepperPepper/datasets/custom_dataset.py
+-rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.5.6/PepperPepper/datasets/image_datasets.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.5.6/PepperPepper/datasets/text_datasets.py
+-rw-rw-rw-   0        0        0      106 2024-04-30 02:10:15.000000 pepperpepper-0.0.5.6/PepperPepper/environment.py
+drwxrwxrwx   0        0        0        0 2024-04-30 03:56:36.233573 pepperpepper-0.0.5.6/PepperPepper/examples/
+-rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.5.6/PepperPepper/examples/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.5.6/PepperPepper/examples/custom_task.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.5.6/PepperPepper/examples/image_classification.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.5.6/PepperPepper/examples/text_generation.py
+drwxrwxrwx   0        0        0        0 2024-04-30 03:56:36.236073 pepperpepper-0.0.5.6/PepperPepper/layers/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.5.6/PepperPepper/layers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.5.6/PepperPepper/layers/attention.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.5.6/PepperPepper/layers/custom_layer.py
+drwxrwxrwx   0        0        0        0 2024-04-30 03:56:36.238681 pepperpepper-0.0.5.6/PepperPepper/losses/
+-rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.5.6/PepperPepper/losses/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.5.6/PepperPepper/losses/custom_loss.py
+drwxrwxrwx   0        0        0        0 2024-04-30 03:56:36.244191 pepperpepper-0.0.5.6/PepperPepper/models/
+-rw-rw-rw-   0        0        0      752 2024-04-26 06:22:17.000000 pepperpepper-0.0.5.6/PepperPepper/models/__init__.py
+-rw-rw-rw-   0        0        0     2525 2024-04-30 02:40:06.000000 pepperpepper-0.0.5.6/PepperPepper/models/cnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.5.6/PepperPepper/models/custom_model.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.5.6/PepperPepper/models/rnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.5.6/PepperPepper/models/transformer.py
+drwxrwxrwx   0        0        0        0 2024-04-30 03:56:36.247494 pepperpepper-0.0.5.6/PepperPepper/optimizers/
+-rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.5.6/PepperPepper/optimizers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.5.6/PepperPepper/optimizers/custom_optimizer.py
+-rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.5.6/PepperPepper/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-30 03:56:36.248547 pepperpepper-0.0.5.6/PepperPepper.egg-info/
+-rw-rw-rw-   0        0        0      433 2024-04-30 03:56:36.000000 pepperpepper-0.0.5.6/PepperPepper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1225 2024-04-30 03:56:36.000000 pepperpepper-0.0.5.6/PepperPepper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 03:56:36.000000 pepperpepper-0.0.5.6/PepperPepper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2024-04-30 03:56:36.000000 pepperpepper-0.0.5.6/PepperPepper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-30 03:56:36.000000 pepperpepper-0.0.5.6/PepperPepper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.5.6/PepperPepper.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-04-30 03:56:36.250071 pepperpepper-0.0.5.6/setup.cfg
+-rw-rw-rw-   0        0        0      569 2024-04-30 03:56:16.000000 pepperpepper-0.0.5.6/setup.py
```

### Comparing `pepperpepper-0.0.5.5/PepperPepper/__init__.py` & `pepperpepper-0.0.5.6/PepperPepper/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.5/PepperPepper/callbacks/__init__.py` & `pepperpepper-0.0.5.6/PepperPepper/callbacks/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,16 +22,18 @@
 # 导入 callback 子包中的各个模块
 # from . import logging_callback
 # from . import model_checkpoint_callback
 # from . import early_stopping_callback
 #
 # 如果需要，可以直接导入这些模块中的特定回调类
 from .custom_callback import save_best_model
+from .custom_callback import load_best_model
 # from .logging_callback import LoggingCallback
 # from .model_checkpoint_callback import ModelCheckpointCallback
 # from .early_stopping_callback import EarlyStoppingCallback
 #
 # # __all__ 变量定义了当使用 from callback import * 时导入哪些对象
 # # 注意：通常不推荐使用 from package import *
 __all__ = [
-    'save_best_model'
+    'save_best_model',
+    'load_best_model'
 ]
```

### Comparing `pepperpepper-0.0.5.5/PepperPepper/core/__init__.py` & `pepperpepper-0.0.5.6/PepperPepper/core/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,17 +18,21 @@
 # from . import utils
 # from . import model_builder
 #
 # 如果需要，可以直接导入这些模块中的特定类或函数
 
 from .utils import evaluate_accuracy_gpu
 from .utils import train_custom
+from .utils import try_gpu
+from .utils import try_all_gpus
 # from .data_structures import CustomDataStructure
 # from .utils import some_utility_function
 # from .model_builder import build_model
 #
 # __all__ 变量定义了当使用 from core import * 时导入哪些对象
 # 注意：通常不推荐使用 from package import *
 __all__ = [
     'evaluate_accuracy_gpu',
-    'train_custom'
+    'train_custom',
+    'try_gpu',
+    'try_all_gpus'
 ]
```

### Comparing `pepperpepper-0.0.5.5/PepperPepper/core/utils.py` & `pepperpepper-0.0.5.6/PepperPepper/core/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -143,8 +143,61 @@
         print(
             f'Epoch {epoch + 1}/{epochs}, Loss: {running_loss / total:.4f}, Train Acc: {train_acc:.2f}%, Val Loss: {val_loss:.4f}, Val Acc: {val_acc:.2f}%')
 
         # 如果当前验证准确率是最佳的，则保存模型
         if val_acc > best_acc:
             best_acc = val_acc
             save_best_model(model, optimizer, model_path)
-            print(f"Model improved and saved to {model_path}")
+            print(f"Model improved and saved to {model_path}")
+
+
+
+"""
+3.try_gpu(i=0) 
+    如果存在，则返回指定的GPU设备，否则返回CPU设备。  
+  
+    Args:  
+        i (int, optional): GPU设备的索引。默认为0。  
+  
+    Returns:  
+        torch.device: 指定的GPU设备或CPU设备。 
+
+"""
+def try_gpu(i=0):
+    # @save 注解：这个通常用于Jupyter Notebook中，用于保存函数定义到某个地方，但在这里它对代码执行没有影响。
+    """如果存在，则返回gpu(i)，否则返回cpu()"""
+    # 检查是否有足够的GPU设备数量，至少要比指定的索引i大1
+    if torch.cuda.device_count() >= i + 1:
+        # 如果有足够的GPU设备，则返回指定索引i的GPU设备
+        return torch.device(f'cuda:{i}')
+        # 如果没有足够的GPU设备或没有检测到GPU，则返回CPU设备
+    return torch.device('cpu')
+
+
+
+
+
+
+
+
+
+
+"""  
+4.try_all_gpus()
+   返回所有可用的GPU设备列表，如果没有GPU，则返回包含CPU设备的列表。  
+
+   Returns:  
+       list[torch.device]: 所有GPU设备或CPU设备的列表。  
+"""
+
+def try_all_gpus():
+    # @save 注解：同样地，这个注解通常用于Jupyter Notebook中，用于保存函数定义。
+    """返回所有可用的GPU，如果没有GPU，则返回[cpu(),]"""
+    # 初始化一个空列表用于存储所有GPU设备
+    devices = []
+    # 遍历所有检测到的GPU设备
+    for i in range(torch.cuda.device_count()):
+        # 将每个GPU设备添加到列表中
+        devices.append(torch.device(f'cuda:{i}'))
+        # 如果devices列表不为空（即存在GPU设备），则返回该列表
+    # 否则，返回只包含CPU设备的列表
+    return devices if devices else [torch.device('cpu')]
```

### Comparing `pepperpepper-0.0.5.5/PepperPepper/datasets/__init__.py` & `pepperpepper-0.0.5.6/PepperPepper/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.5/PepperPepper/datasets/image_datasets.py` & `pepperpepper-0.0.5.6/PepperPepper/datasets/image_datasets.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.5/PepperPepper/examples/__init__.py` & `pepperpepper-0.0.5.6/PepperPepper/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.5/PepperPepper/layers/__init__.py` & `pepperpepper-0.0.5.6/PepperPepper/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.5/PepperPepper/losses/__init__.py` & `pepperpepper-0.0.5.6/PepperPepper/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.5/PepperPepper/models/__init__.py` & `pepperpepper-0.0.5.6/PepperPepper/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.5/PepperPepper/models/cnn.py` & `pepperpepper-0.0.5.6/PepperPepper/models/cnn.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.5/PepperPepper/optimizers/__init__.py` & `pepperpepper-0.0.5.6/PepperPepper/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.5/PepperPepper.egg-info/SOURCES.txt` & `pepperpepper-0.0.5.6/PepperPepper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.5/setup.py` & `pepperpepper-0.0.5.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     'torchvision'
 ]
 
 
 
 setuptools.setup(
     name="PepperPepper",
-    version="0.0.5.5",
+    version="0.0.5.6",
     python_requires='>=3.11',
     author="Aohua Li",
     author_email="pepper2024jlu@163.com",
     description="It is a DeepLearning package to foster developed by Aohua Li",
     url="",
     packages=setuptools.find_packages(),
     zip_safe=True,
```

