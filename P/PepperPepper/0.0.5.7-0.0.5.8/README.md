# Comparing `tmp/pepperpepper-0.0.5.7.tar.gz` & `tmp/pepperpepper-0.0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepperpepper-0.0.5.7.tar", last modified: Tue Apr 30 06:27:11 2024, max compression
+gzip compressed data, was "pepperpepper-0.0.5.8.tar", last modified: Tue Apr 30 16:33:22 2024, max compression
```

## Comparing `pepperpepper-0.0.5.7.tar` & `pepperpepper-0.0.5.8.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 06:27:11.816551 pepperpepper-0.0.5.7/
--rw-rw-rw-   0        0        0      433 2024-04-30 06:27:11.815550 pepperpepper-0.0.5.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-30 06:27:11.755863 pepperpepper-0.0.5.7/PepperPepper/
--rw-rw-rw-   0        0        0     5179 2024-04-29 03:25:30.000000 pepperpepper-0.0.5.7/PepperPepper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 06:27:11.786009 pepperpepper-0.0.5.7/PepperPepper/callbacks/
--rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.5.7/PepperPepper/callbacks/__init__.py
--rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.5.7/PepperPepper/callbacks/custom_callback.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.5.7/PepperPepper/callbacks/learning_rate_scheduler.py
-drwxrwxrwx   0        0        0        0 2024-04-30 06:27:11.789008 pepperpepper-0.0.5.7/PepperPepper/core/
--rw-rw-rw-   0        0        0     1028 2024-04-30 03:56:08.000000 pepperpepper-0.0.5.7/PepperPepper/core/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.5.7/PepperPepper/core/base_model.py
--rw-rw-rw-   0        0        0     7029 2024-04-30 03:54:40.000000 pepperpepper-0.0.5.7/PepperPepper/core/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-30 06:27:11.795350 pepperpepper-0.0.5.7/PepperPepper/datasets/
--rw-rw-rw-   0        0        0     1008 2024-04-29 04:09:47.000000 pepperpepper-0.0.5.7/PepperPepper/datasets/__init__.py
--rw-rw-rw-   0        0        0        4 2024-04-29 18:10:09.000000 pepperpepper-0.0.5.7/PepperPepper/datasets/custom_dataset.py
--rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.5.7/PepperPepper/datasets/image_datasets.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.5.7/PepperPepper/datasets/text_datasets.py
--rw-rw-rw-   0        0        0      106 2024-04-30 02:10:15.000000 pepperpepper-0.0.5.7/PepperPepper/environment.py
-drwxrwxrwx   0        0        0        0 2024-04-30 06:27:11.800357 pepperpepper-0.0.5.7/PepperPepper/examples/
--rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.5.7/PepperPepper/examples/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.5.7/PepperPepper/examples/custom_task.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.5.7/PepperPepper/examples/image_classification.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.5.7/PepperPepper/examples/text_generation.py
-drwxrwxrwx   0        0        0        0 2024-04-30 06:27:11.803993 pepperpepper-0.0.5.7/PepperPepper/layers/
--rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.5.7/PepperPepper/layers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.5.7/PepperPepper/layers/attention.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.5.7/PepperPepper/layers/custom_layer.py
-drwxrwxrwx   0        0        0        0 2024-04-30 06:27:11.806493 pepperpepper-0.0.5.7/PepperPepper/losses/
--rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.5.7/PepperPepper/losses/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.5.7/PepperPepper/losses/custom_loss.py
-drwxrwxrwx   0        0        0        0 2024-04-30 06:27:11.811550 pepperpepper-0.0.5.7/PepperPepper/models/
--rw-rw-rw-   0        0        0      793 2024-04-30 06:26:44.000000 pepperpepper-0.0.5.7/PepperPepper/models/__init__.py
--rw-rw-rw-   0        0        0     6490 2024-04-30 06:26:10.000000 pepperpepper-0.0.5.7/PepperPepper/models/cnn.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.5.7/PepperPepper/models/custom_model.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.5.7/PepperPepper/models/rnn.py
--rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.5.7/PepperPepper/models/transformer.py
-drwxrwxrwx   0        0        0        0 2024-04-30 06:27:11.814051 pepperpepper-0.0.5.7/PepperPepper/optimizers/
--rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.5.7/PepperPepper/optimizers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.5.7/PepperPepper/optimizers/custom_optimizer.py
--rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.5.7/PepperPepper/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-30 06:27:11.815051 pepperpepper-0.0.5.7/PepperPepper.egg-info/
--rw-rw-rw-   0        0        0      433 2024-04-30 06:27:11.000000 pepperpepper-0.0.5.7/PepperPepper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1225 2024-04-30 06:27:11.000000 pepperpepper-0.0.5.7/PepperPepper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 06:27:11.000000 pepperpepper-0.0.5.7/PepperPepper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2024-04-30 06:27:11.000000 pepperpepper-0.0.5.7/PepperPepper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-30 06:27:11.000000 pepperpepper-0.0.5.7/PepperPepper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.5.7/PepperPepper.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-04-30 06:27:11.816551 pepperpepper-0.0.5.7/setup.cfg
--rw-rw-rw-   0        0        0      569 2024-04-30 06:27:01.000000 pepperpepper-0.0.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:33:22.000879 pepperpepper-0.0.5.8/
+-rw-rw-rw-   0        0        0      433 2024-04-30 16:33:22.000879 pepperpepper-0.0.5.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-30 16:33:21.521544 pepperpepper-0.0.5.8/PepperPepper/
+-rw-rw-rw-   0        0        0     5179 2024-04-29 03:25:30.000000 pepperpepper-0.0.5.8/PepperPepper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:33:21.615744 pepperpepper-0.0.5.8/PepperPepper/callbacks/
+-rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.5.8/PepperPepper/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.5.8/PepperPepper/callbacks/custom_callback.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.5.8/PepperPepper/callbacks/learning_rate_scheduler.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:33:21.746932 pepperpepper-0.0.5.8/PepperPepper/core/
+-rw-rw-rw-   0        0        0     1028 2024-04-30 03:56:08.000000 pepperpepper-0.0.5.8/PepperPepper/core/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.5.8/PepperPepper/core/base_model.py
+-rw-rw-rw-   0        0        0     7029 2024-04-30 03:54:40.000000 pepperpepper-0.0.5.8/PepperPepper/core/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:33:21.788357 pepperpepper-0.0.5.8/PepperPepper/datasets/
+-rw-rw-rw-   0        0        0     1008 2024-04-29 04:09:47.000000 pepperpepper-0.0.5.8/PepperPepper/datasets/__init__.py
+-rw-rw-rw-   0        0        0        4 2024-04-29 18:10:09.000000 pepperpepper-0.0.5.8/PepperPepper/datasets/custom_dataset.py
+-rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.5.8/PepperPepper/datasets/image_datasets.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.5.8/PepperPepper/datasets/text_datasets.py
+-rw-rw-rw-   0        0        0      106 2024-04-30 02:10:15.000000 pepperpepper-0.0.5.8/PepperPepper/environment.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:33:21.804141 pepperpepper-0.0.5.8/PepperPepper/examples/
+-rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.5.8/PepperPepper/examples/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.5.8/PepperPepper/examples/custom_task.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.5.8/PepperPepper/examples/image_classification.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.5.8/PepperPepper/examples/text_generation.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:33:21.914503 pepperpepper-0.0.5.8/PepperPepper/layers/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.5.8/PepperPepper/layers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.5.8/PepperPepper/layers/attention.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.5.8/PepperPepper/layers/custom_layer.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:33:21.937923 pepperpepper-0.0.5.8/PepperPepper/losses/
+-rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.5.8/PepperPepper/losses/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.5.8/PepperPepper/losses/custom_loss.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:33:21.985859 pepperpepper-0.0.5.8/PepperPepper/models/
+-rw-rw-rw-   0        0        0      793 2024-04-30 06:26:44.000000 pepperpepper-0.0.5.8/PepperPepper/models/__init__.py
+-rw-rw-rw-   0        0        0    10402 2024-04-30 16:32:02.000000 pepperpepper-0.0.5.8/PepperPepper/models/cnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.5.8/PepperPepper/models/custom_model.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.5.8/PepperPepper/models/rnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.5.8/PepperPepper/models/transformer.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:33:22.000879 pepperpepper-0.0.5.8/PepperPepper/optimizers/
+-rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.5.8/PepperPepper/optimizers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.5.8/PepperPepper/optimizers/custom_optimizer.py
+-rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.5.8/PepperPepper/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:33:22.000879 pepperpepper-0.0.5.8/PepperPepper.egg-info/
+-rw-rw-rw-   0        0        0      433 2024-04-30 16:33:21.000000 pepperpepper-0.0.5.8/PepperPepper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1225 2024-04-30 16:33:21.000000 pepperpepper-0.0.5.8/PepperPepper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 16:33:21.000000 pepperpepper-0.0.5.8/PepperPepper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2024-04-30 16:33:21.000000 pepperpepper-0.0.5.8/PepperPepper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-30 16:33:21.000000 pepperpepper-0.0.5.8/PepperPepper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.5.8/PepperPepper.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-04-30 16:33:22.000879 pepperpepper-0.0.5.8/setup.cfg
+-rw-rw-rw-   0        0        0      569 2024-04-30 16:33:13.000000 pepperpepper-0.0.5.8/setup.py
```

### Comparing `pepperpepper-0.0.5.7/PepperPepper/__init__.py` & `pepperpepper-0.0.5.8/PepperPepper/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.7/PepperPepper/callbacks/__init__.py` & `pepperpepper-0.0.5.8/PepperPepper/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.7/PepperPepper/callbacks/custom_callback.py` & `pepperpepper-0.0.5.8/PepperPepper/callbacks/custom_callback.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.7/PepperPepper/core/__init__.py` & `pepperpepper-0.0.5.8/PepperPepper/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.7/PepperPepper/core/utils.py` & `pepperpepper-0.0.5.8/PepperPepper/core/utils.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.7/PepperPepper/datasets/__init__.py` & `pepperpepper-0.0.5.8/PepperPepper/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.7/PepperPepper/datasets/image_datasets.py` & `pepperpepper-0.0.5.8/PepperPepper/datasets/image_datasets.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.7/PepperPepper/examples/__init__.py` & `pepperpepper-0.0.5.8/PepperPepper/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.7/PepperPepper/layers/__init__.py` & `pepperpepper-0.0.5.8/PepperPepper/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.7/PepperPepper/losses/__init__.py` & `pepperpepper-0.0.5.8/PepperPepper/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.7/PepperPepper/models/__init__.py` & `pepperpepper-0.0.5.8/PepperPepper/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.7/PepperPepper/models/cnn.py` & `pepperpepper-0.0.5.8/PepperPepper/models/cnn.py`

 * *Files 25% similar despite different names*

```diff
@@ -150,9 +150,127 @@
                     torch.nn.init.zeros_(m.bias)
 
 
 
 
 
 
+# 3.定义一个VGG卷积块
+class VGGBlock(torch.nn.Module):
+    def __init__(self, in_channels, out_channels, num_convs, pool=True):
+        """
+        VGG块，包含多个卷积层和一个可选的最大池化层
+
+        参数:
+            in_channels (int): 输入通道数
+            out_channels (int): 输出通道数（每个卷积层的输出通道数）
+            num_convs (int): 卷积层的数量
+            pool (bool, 可选): 是否在块后添加最大池化层。默认为True
+        """
+        super(VGGBlock, self).__init__()
+
+        # 创建多个卷积层，每个卷积层后面都跟着ReLU激活函数
+        layers = []
+        for _ in range(num_convs):
+            layers.append(torch.nn.Conv2d(in_channels if _ == 0 else out_channels, out_channels, kernel_size=3, padding=1))
+            layers.append(torch.nn.ReLU(inplace=True))
+
+            # 如果有池化层，则添加
+        if pool:
+            layers.append(torch.nn.MaxPool2d(kernel_size=2, stride=2))
+
+            # 将所有层组合成一个Sequential模块
+        self.conv_block = torch.nn.Sequential(*layers)
+
+    def forward(self, x):
+        """
+        前向传播
+
+        参数:
+            x (torch.Tensor): 输入张量
+
+        返回:
+            torch.Tensor: 输出张量
+        """
+        x = self.conv_block(x)
+        return x
+
+
+
+
+
+
+#4.定义VGG16模型
+class VGG16(torch.nn.Module):
+    def __init__(self, num_classes=1000):
+        """
+        VGG16模型
+
+        参数:
+            num_classes (int, 可选): 分类的数量。默认为1000
+        """
+        super(VGG16, self).__init__()
+
+        # 定义特征提取部分
+        self.features = torch.nn.Sequential(
+            VGGBlock(3, 64, 2, pool=True),  # block1: 64 channels, 2 conv layers, maxpool
+            VGGBlock(64, 128, 2, pool=True),  # block2: 128 channels, 2 conv layers, maxpool
+            VGGBlock(128, 256, 3, pool=True),  # block3: 256 channels, 3 conv layers, maxpool
+            VGGBlock(256, 512, 3, pool=True),  # block4: 512 channels, 3 conv layers, maxpool
+            VGGBlock(512, 512, 3, pool=True)  # block5: 512 channels, 3 conv layers, maxpool
+        )
+
+        # 定义分类器部分（全连接层）
+        self.classifier = torch.nn.Sequential(
+            torch.nn.Linear(512 * 7 * 7, 4096),  # fully connected layer, 4096 output neurons
+            torch.nn.ReLU(True),
+            torch.nn.Dropout(),
+            torch.nn.Linear(4096, 4096),
+            torch.nn.ReLU(True),
+            torch.nn.Dropout(),
+            torch.nn.Linear(4096, num_classes)  # fully connected layer, num_classes output neurons for classification
+        )
+
+        # 初始化权重
+        for m in self.modules():
+            if isinstance(m, torch.nn.Conv2d):
+                torch.nn.init.kaiming_normal_(m.weight, mode='fan_out', nonlinearity='relu')
+                if m.bias is not None:
+                    torch.nn.init.constant_(m.bias, 0)
+            elif isinstance(m, torch.nn.Linear):
+                torch.nn.init.normal_(m.weight, 0, 0.01)
+                torch.nn.init.constant_(m.bias, 0)
+
+    def forward(self, x):
+        """
+        前向传播
+
+        参数:
+            x (torch.Tensor): 输入张量
+
+        返回:
+            torch.Tensor: 分类的logits
+        """
+        # 特征提取
+        x = self.features(x)
+
+        # 在将特征图送入全连接层之前，需要将其展平（flatten）
+        # 假设输入图像的大小是224x224，经过5个池化层（每个池化层将尺寸减半）后，
+        # 特征图的大小会变成 7x7
+        x = x.view(x.size(0), -1)  # 展平操作，-1 表示让PyTorch自动计算该维度的大小
+
+        # 送入分类器
+        x = self.classifier(x)
+
+        return x
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
```

### Comparing `pepperpepper-0.0.5.7/PepperPepper/optimizers/__init__.py` & `pepperpepper-0.0.5.8/PepperPepper/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.7/PepperPepper.egg-info/SOURCES.txt` & `pepperpepper-0.0.5.8/PepperPepper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.7/setup.py` & `pepperpepper-0.0.5.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     'torchvision'
 ]
 
 
 
 setuptools.setup(
     name="PepperPepper",
-    version="0.0.5.7",
+    version="0.0.5.8",
     python_requires='>=3.11',
     author="Aohua Li",
     author_email="pepper2024jlu@163.com",
     description="It is a DeepLearning package to foster developed by Aohua Li",
     url="",
     packages=setuptools.find_packages(),
     zip_safe=True,
```

