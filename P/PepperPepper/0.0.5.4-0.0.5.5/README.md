# Comparing `tmp/pepperpepper-0.0.5.4.tar.gz` & `tmp/pepperpepper-0.0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepperpepper-0.0.5.4.tar", last modified: Tue Apr 30 02:40:41 2024, max compression
+gzip compressed data, was "pepperpepper-0.0.5.5.tar", last modified: Tue Apr 30 02:50:03 2024, max compression
```

## Comparing `pepperpepper-0.0.5.4.tar` & `pepperpepper-0.0.5.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 02:40:41.268593 pepperpepper-0.0.5.4/
--rw-rw-rw-   0        0        0      433 2024-04-30 02:40:41.267604 pepperpepper-0.0.5.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-30 02:40:41.213795 pepperpepper-0.0.5.4/PepperPepper/
--rw-rw-rw-   0        0        0     5179 2024-04-29 03:25:30.000000 pepperpepper-0.0.5.4/PepperPepper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:40:41.239870 pepperpepper-0.0.5.4/PepperPepper/callbacks/
--rw-rw-rw-   0        0        0      985 2024-04-30 01:42:49.000000 pepperpepper-0.0.5.4/PepperPepper/callbacks/__init__.py
--rw-rw-rw-   0        0        0      785 2024-04-30 01:42:05.000000 pepperpepper-0.0.5.4/PepperPepper/callbacks/custom_callback.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.5.4/PepperPepper/callbacks/learning_rate_scheduler.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:40:41.243389 pepperpepper-0.0.5.4/PepperPepper/core/
--rw-rw-rw-   0        0        0      930 2024-04-30 02:10:06.000000 pepperpepper-0.0.5.4/PepperPepper/core/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.5.4/PepperPepper/core/base_model.py
--rw-rw-rw-   0        0        0     4471 2024-04-30 02:21:34.000000 pepperpepper-0.0.5.4/PepperPepper/core/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:40:41.248165 pepperpepper-0.0.5.4/PepperPepper/datasets/
--rw-rw-rw-   0        0        0     1008 2024-04-29 04:09:47.000000 pepperpepper-0.0.5.4/PepperPepper/datasets/__init__.py
--rw-rw-rw-   0        0        0        4 2024-04-29 18:10:09.000000 pepperpepper-0.0.5.4/PepperPepper/datasets/custom_dataset.py
--rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.5.4/PepperPepper/datasets/image_datasets.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.5.4/PepperPepper/datasets/text_datasets.py
--rw-rw-rw-   0        0        0      106 2024-04-30 02:10:15.000000 pepperpepper-0.0.5.4/PepperPepper/environment.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:40:41.251135 pepperpepper-0.0.5.4/PepperPepper/examples/
--rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.5.4/PepperPepper/examples/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.5.4/PepperPepper/examples/custom_task.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.5.4/PepperPepper/examples/image_classification.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.5.4/PepperPepper/examples/text_generation.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:40:41.253641 pepperpepper-0.0.5.4/PepperPepper/layers/
--rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.5.4/PepperPepper/layers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.5.4/PepperPepper/layers/attention.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.5.4/PepperPepper/layers/custom_layer.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:40:41.256204 pepperpepper-0.0.5.4/PepperPepper/losses/
--rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.5.4/PepperPepper/losses/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.5.4/PepperPepper/losses/custom_loss.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:40:41.262725 pepperpepper-0.0.5.4/PepperPepper/models/
--rw-rw-rw-   0        0        0      752 2024-04-26 06:22:17.000000 pepperpepper-0.0.5.4/PepperPepper/models/__init__.py
--rw-rw-rw-   0        0        0     2525 2024-04-30 02:40:06.000000 pepperpepper-0.0.5.4/PepperPepper/models/cnn.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.5.4/PepperPepper/models/custom_model.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.5.4/PepperPepper/models/rnn.py
--rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.5.4/PepperPepper/models/transformer.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:40:41.264722 pepperpepper-0.0.5.4/PepperPepper/optimizers/
--rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.5.4/PepperPepper/optimizers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.5.4/PepperPepper/optimizers/custom_optimizer.py
--rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.5.4/PepperPepper/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:40:41.267068 pepperpepper-0.0.5.4/PepperPepper.egg-info/
--rw-rw-rw-   0        0        0      433 2024-04-30 02:40:41.000000 pepperpepper-0.0.5.4/PepperPepper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1225 2024-04-30 02:40:41.000000 pepperpepper-0.0.5.4/PepperPepper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 02:40:41.000000 pepperpepper-0.0.5.4/PepperPepper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2024-04-30 02:40:41.000000 pepperpepper-0.0.5.4/PepperPepper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-30 02:40:41.000000 pepperpepper-0.0.5.4/PepperPepper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.5.4/PepperPepper.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-04-30 02:40:41.268593 pepperpepper-0.0.5.4/setup.cfg
--rw-rw-rw-   0        0        0      569 2024-04-30 02:40:34.000000 pepperpepper-0.0.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:50:03.102537 pepperpepper-0.0.5.5/
+-rw-rw-rw-   0        0        0      433 2024-04-30 02:50:03.101543 pepperpepper-0.0.5.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-30 02:50:03.057243 pepperpepper-0.0.5.5/PepperPepper/
+-rw-rw-rw-   0        0        0     5179 2024-04-29 03:25:30.000000 pepperpepper-0.0.5.5/PepperPepper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:50:03.077855 pepperpepper-0.0.5.5/PepperPepper/callbacks/
+-rw-rw-rw-   0        0        0      985 2024-04-30 01:42:49.000000 pepperpepper-0.0.5.5/PepperPepper/callbacks/__init__.py
+-rw-rw-rw-   0        0        0      785 2024-04-30 01:42:05.000000 pepperpepper-0.0.5.5/PepperPepper/callbacks/custom_callback.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.5.5/PepperPepper/callbacks/learning_rate_scheduler.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:50:03.080317 pepperpepper-0.0.5.5/PepperPepper/core/
+-rw-rw-rw-   0        0        0      930 2024-04-30 02:10:06.000000 pepperpepper-0.0.5.5/PepperPepper/core/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.5.5/PepperPepper/core/base_model.py
+-rw-rw-rw-   0        0        0     5266 2024-04-30 02:49:08.000000 pepperpepper-0.0.5.5/PepperPepper/core/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:50:03.083312 pepperpepper-0.0.5.5/PepperPepper/datasets/
+-rw-rw-rw-   0        0        0     1008 2024-04-29 04:09:47.000000 pepperpepper-0.0.5.5/PepperPepper/datasets/__init__.py
+-rw-rw-rw-   0        0        0        4 2024-04-29 18:10:09.000000 pepperpepper-0.0.5.5/PepperPepper/datasets/custom_dataset.py
+-rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.5.5/PepperPepper/datasets/image_datasets.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.5.5/PepperPepper/datasets/text_datasets.py
+-rw-rw-rw-   0        0        0      106 2024-04-30 02:10:15.000000 pepperpepper-0.0.5.5/PepperPepper/environment.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:50:03.087536 pepperpepper-0.0.5.5/PepperPepper/examples/
+-rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.5.5/PepperPepper/examples/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.5.5/PepperPepper/examples/custom_task.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.5.5/PepperPepper/examples/image_classification.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.5.5/PepperPepper/examples/text_generation.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:50:03.090535 pepperpepper-0.0.5.5/PepperPepper/layers/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.5.5/PepperPepper/layers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.5.5/PepperPepper/layers/attention.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.5.5/PepperPepper/layers/custom_layer.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:50:03.092986 pepperpepper-0.0.5.5/PepperPepper/losses/
+-rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.5.5/PepperPepper/losses/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.5.5/PepperPepper/losses/custom_loss.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:50:03.097537 pepperpepper-0.0.5.5/PepperPepper/models/
+-rw-rw-rw-   0        0        0      752 2024-04-26 06:22:17.000000 pepperpepper-0.0.5.5/PepperPepper/models/__init__.py
+-rw-rw-rw-   0        0        0     2525 2024-04-30 02:40:06.000000 pepperpepper-0.0.5.5/PepperPepper/models/cnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.5.5/PepperPepper/models/custom_model.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.5.5/PepperPepper/models/rnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.5.5/PepperPepper/models/transformer.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:50:03.099567 pepperpepper-0.0.5.5/PepperPepper/optimizers/
+-rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.5.5/PepperPepper/optimizers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.5.5/PepperPepper/optimizers/custom_optimizer.py
+-rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.5.5/PepperPepper/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-30 02:50:03.100555 pepperpepper-0.0.5.5/PepperPepper.egg-info/
+-rw-rw-rw-   0        0        0      433 2024-04-30 02:50:02.000000 pepperpepper-0.0.5.5/PepperPepper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1225 2024-04-30 02:50:02.000000 pepperpepper-0.0.5.5/PepperPepper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 02:50:02.000000 pepperpepper-0.0.5.5/PepperPepper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2024-04-30 02:50:02.000000 pepperpepper-0.0.5.5/PepperPepper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-30 02:50:02.000000 pepperpepper-0.0.5.5/PepperPepper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.5.5/PepperPepper.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-04-30 02:50:03.102537 pepperpepper-0.0.5.5/setup.cfg
+-rw-rw-rw-   0        0        0      569 2024-04-30 02:49:26.000000 pepperpepper-0.0.5.5/setup.py
```

### Comparing `pepperpepper-0.0.5.4/PepperPepper/__init__.py` & `pepperpepper-0.0.5.5/PepperPepper/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.4/PepperPepper/callbacks/__init__.py` & `pepperpepper-0.0.5.5/PepperPepper/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.4/PepperPepper/callbacks/custom_callback.py` & `pepperpepper-0.0.5.5/PepperPepper/callbacks/custom_callback.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.4/PepperPepper/core/__init__.py` & `pepperpepper-0.0.5.5/PepperPepper/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.4/PepperPepper/core/utils.py` & `pepperpepper-0.0.5.5/PepperPepper/core/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -72,29 +72,46 @@
         model_path (str): 最佳模型保存路径  
 
     返回:  
         None  
 """
 
 def train_custom(model, train_loader, valid_loader, epochs, lr, device, model_path):
+    # 用于评估模型准确率的函数，同时返回验证损失和准确率
+    def evaluate_accuracy(model, valid_loader, criterion, device):
+        model.eval()
+        val_loss = 0.0
+        correct = 0
+        total = 0
+        with torch.no_grad():
+            for images, labels in valid_loader:
+                images, labels = images.to(device), labels.to(device)
+                outputs = model(images)
+                loss = criterion(outputs, labels)
+                val_loss += loss.item() * images.size(0)
+                _, predicted = torch.max(outputs, 1)
+                total += labels.size(0)
+                correct += (predicted == labels).sum().item()
+        val_acc = 100 * correct / total
+        return val_loss / total, val_acc
 
-    # 初始化模型参数，使用xavier方法
+        # 初始化模型参数，使用xavier方法
     def init_weights(m):
         if isinstance(m, (torch.nn.Linear, torch.nn.Conv2d)):  # 使用isinstance替代type判断
             torch.nn.init.xavier_uniform_(m.weight)
     model.apply(init_weights)
 
 
     # 将模型移至指定设备
     model.to(device)
     model.train()
 
     # 定义优化器和损失函数
     optimizer = torch.optim.SGD(model.parameters(), lr=lr, momentum=0.9)
-    loss = torch.nn.CrossEntropyLoss()
+    criterion  = torch.nn.CrossEntropyLoss()
 
     best_acc = 0.0
     history = {'loss': [], 'val_loss': [], 'acc': [], 'val_acc': []}
 
     for epoch in range(epochs):
         model.train(True)
         running_loss = 0.0
@@ -102,25 +119,25 @@
         total = 0
 
 
         for images, labels in train_loader:
             images, labels = images.to(device), labels.to(device)
             optimizer.zero_grad()
             outputs = model(images)
-            loss = loss(outputs, labels)
+            loss = criterion(outputs, labels)
             loss.backward()
             optimizer.step()
 
             running_loss += loss.item() * images.size(0)
             _, predicted = torch.max(outputs, 1)
             total += labels.size(0)
             correct += (predicted == labels).sum().item()
 
         train_acc = 100 * correct / total
-        val_loss, val_acc = evaluate_accuracy_gpu(model, valid_loader, loss, device)
+        val_loss, val_acc = evaluate_accuracy(model, valid_loader, criterion, device)
         history['loss'].append(running_loss / total)
         history['val_loss'].append(val_loss)
         history['acc'].append(train_acc)
         history['val_acc'].append(val_acc)
 
         # 打印训练和验证的统计信息
         print(
```

### Comparing `pepperpepper-0.0.5.4/PepperPepper/datasets/__init__.py` & `pepperpepper-0.0.5.5/PepperPepper/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.4/PepperPepper/datasets/image_datasets.py` & `pepperpepper-0.0.5.5/PepperPepper/datasets/image_datasets.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.4/PepperPepper/examples/__init__.py` & `pepperpepper-0.0.5.5/PepperPepper/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.4/PepperPepper/layers/__init__.py` & `pepperpepper-0.0.5.5/PepperPepper/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.4/PepperPepper/losses/__init__.py` & `pepperpepper-0.0.5.5/PepperPepper/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.4/PepperPepper/models/__init__.py` & `pepperpepper-0.0.5.5/PepperPepper/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.4/PepperPepper/models/cnn.py` & `pepperpepper-0.0.5.5/PepperPepper/models/cnn.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.4/PepperPepper/optimizers/__init__.py` & `pepperpepper-0.0.5.5/PepperPepper/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.4/PepperPepper.egg-info/SOURCES.txt` & `pepperpepper-0.0.5.5/PepperPepper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.4/setup.py` & `pepperpepper-0.0.5.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     'torchvision'
 ]
 
 
 
 setuptools.setup(
     name="PepperPepper",
-    version="0.0.5.4",
+    version="0.0.5.5",
     python_requires='>=3.11',
     author="Aohua Li",
     author_email="pepper2024jlu@163.com",
     description="It is a DeepLearning package to foster developed by Aohua Li",
     url="",
     packages=setuptools.find_packages(),
     zip_safe=True,
```

