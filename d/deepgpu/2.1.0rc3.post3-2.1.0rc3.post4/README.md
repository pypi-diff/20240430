# Comparing `tmp/deepgpu-2.1.0rc3.post3.tar.gz` & `tmp/deepgpu-2.1.0rc3.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepgpu-2.1.0rc3.post3.tar", last modified: Mon Apr 29 13:07:17 2024, max compression
+gzip compressed data, was "deepgpu-2.1.0rc3.post4.tar", last modified: Tue Apr 30 06:55:34 2024, max compression
```

## Comparing `deepgpu-2.1.0rc3.post3.tar` & `deepgpu-2.1.0rc3.post4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 du         (502) staff       (20)        0 2024-04-29 13:07:17.194213 deepgpu-2.1.0rc3.post3/
--rw-r--r--   0 du         (502) staff       (20)       30 2023-10-10 07:39:14.000000 deepgpu-2.1.0rc3.post3/MANIFEST.in
--rw-r--r--   0 du         (502) staff       (20)      621 2024-04-29 13:07:17.193896 deepgpu-2.1.0rc3.post3/PKG-INFO
--rw-r--r--   0 du         (502) staff       (20)      292 2024-04-26 09:23:15.000000 deepgpu-2.1.0rc3.post3/README.md
-drwxr-xr-x   0 du         (502) staff       (20)        0 2024-04-29 13:07:17.190498 deepgpu-2.1.0rc3.post3/deepgpu/
--rw-r--r--   0 du         (502) staff       (20)       17 2023-10-09 07:10:39.000000 deepgpu-2.1.0rc3.post3/deepgpu/__init__.py
-drwxr-xr-x   0 du         (502) staff       (20)        0 2024-04-29 13:07:17.193517 deepgpu-2.1.0rc3.post3/deepgpu.egg-info/
--rw-r--r--   0 du         (502) staff       (20)      621 2024-04-29 13:07:17.000000 deepgpu-2.1.0rc3.post3/deepgpu.egg-info/PKG-INFO
--rw-r--r--   0 du         (502) staff       (20)      196 2024-04-29 13:07:17.000000 deepgpu-2.1.0rc3.post3/deepgpu.egg-info/SOURCES.txt
--rw-r--r--   0 du         (502) staff       (20)        1 2024-04-29 13:07:17.000000 deepgpu-2.1.0rc3.post3/deepgpu.egg-info/dependency_links.txt
--rw-r--r--   0 du         (502) staff       (20)        8 2024-04-29 13:07:17.000000 deepgpu-2.1.0rc3.post3/deepgpu.egg-info/top_level.txt
--rw-r--r--   0 du         (502) staff       (20)       38 2024-04-29 13:07:17.194276 deepgpu-2.1.0rc3.post3/setup.cfg
--rw-r--r--   0 du         (502) staff       (20)     6933 2024-04-29 13:03:45.000000 deepgpu-2.1.0rc3.post3/setup.py
+drwxr-xr-x   0 du         (502) staff       (20)        0 2024-04-30 06:55:34.359612 deepgpu-2.1.0rc3.post4/
+-rw-r--r--   0 du         (502) staff       (20)       30 2023-10-10 07:39:14.000000 deepgpu-2.1.0rc3.post4/MANIFEST.in
+-rw-r--r--   0 du         (502) staff       (20)      621 2024-04-30 06:55:34.359218 deepgpu-2.1.0rc3.post4/PKG-INFO
+-rw-r--r--   0 du         (502) staff       (20)      292 2024-04-26 09:23:15.000000 deepgpu-2.1.0rc3.post4/README.md
+drwxr-xr-x   0 du         (502) staff       (20)        0 2024-04-30 06:55:34.357730 deepgpu-2.1.0rc3.post4/deepgpu/
+-rw-r--r--   0 du         (502) staff       (20)       17 2023-10-09 07:10:39.000000 deepgpu-2.1.0rc3.post4/deepgpu/__init__.py
+drwxr-xr-x   0 du         (502) staff       (20)        0 2024-04-30 06:55:34.358898 deepgpu-2.1.0rc3.post4/deepgpu.egg-info/
+-rw-r--r--   0 du         (502) staff       (20)      621 2024-04-30 06:55:34.000000 deepgpu-2.1.0rc3.post4/deepgpu.egg-info/PKG-INFO
+-rw-r--r--   0 du         (502) staff       (20)      196 2024-04-30 06:55:34.000000 deepgpu-2.1.0rc3.post4/deepgpu.egg-info/SOURCES.txt
+-rw-r--r--   0 du         (502) staff       (20)        1 2024-04-30 06:55:34.000000 deepgpu-2.1.0rc3.post4/deepgpu.egg-info/dependency_links.txt
+-rw-r--r--   0 du         (502) staff       (20)        8 2024-04-30 06:55:34.000000 deepgpu-2.1.0rc3.post4/deepgpu.egg-info/top_level.txt
+-rw-r--r--   0 du         (502) staff       (20)       38 2024-04-30 06:55:34.359667 deepgpu-2.1.0rc3.post4/setup.cfg
+-rw-r--r--   0 du         (502) staff       (20)     6954 2024-04-30 06:54:57.000000 deepgpu-2.1.0rc3.post4/setup.py
```

### Comparing `deepgpu-2.1.0rc3.post3/PKG-INFO` & `deepgpu-2.1.0rc3.post4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepgpu
-Version: 2.1.0rc3.post3
+Version: 2.1.0rc3.post4
 Summary: DEEPGPU is a toolset for AI training acceleration on Alibaba Cloud.
 Home-page: https://www.aliyun.com
 Author: Alibaba Cloud
 License: Copyright (C) Alibaba Group Holding Limited
 Keywords: Distributed,Deep Learning,Communication,NCCL,Pytorch,Tensorflow
 Requires-Python: >=3.8
```

### Comparing `deepgpu-2.1.0rc3.post3/deepgpu.egg-info/PKG-INFO` & `deepgpu-2.1.0rc3.post4/deepgpu.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepgpu
-Version: 2.1.0rc3.post3
+Version: 2.1.0rc3.post4
 Summary: DEEPGPU is a toolset for AI training acceleration on Alibaba Cloud.
 Home-page: https://www.aliyun.com
 Author: Alibaba Cloud
 License: Copyright (C) Alibaba Group Holding Limited
 Keywords: Distributed,Deep Learning,Communication,NCCL,Pytorch,Tensorflow
 Requires-Python: >=3.8
```

### Comparing `deepgpu-2.1.0rc3.post3/setup.py` & `deepgpu-2.1.0rc3.post4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import subprocess
 from setuptools.command.install import install
 import os
 
 NAME="deepgpu"
 DEEPGPU_VERSION = "2.1.0rc3"
 DEEPYTORCH_PKG_VERSION = DEEPGPU_VERSION # same as DEEPGPU version so far
-DEEPGPU_VERSION = "2.1.0rc3.post3"
+DEEPGPU_VERSION = "2.1.0rc3.post4"
 support_os_list = ['ubuntu', 'centos', 'alinux'] # add version later
 support_pytorch_version = ['1.10', '1.11', '1.12', '1.13', '2.0', '2.1']
 support_cuda_version = ['11.1', '11.3', '11.6', '11.7', '11.8', '12.1', '12.3']
 support_python_version = ['38', '39', '310', '311']
 
 _root_path_deepgpu = "https://mirrors.aliyun.com/deepgpu/"
 _root_path_deepytorch = f"{_root_path_deepgpu}/deepytorch/{DEEPYTORCH_PKG_VERSION}/"
@@ -97,16 +97,17 @@
             assert supported == True, \
                 f"{NAME}-{DEEPGPU_VERSION} installed failed for not testing on this os: {os_name} "
         if python_version not in support_python_version:
             supported = False
         if cuda_version not in support_cuda_version:
             supported = False
         if framework_version not in support_pytorch_version:
-            if framework_version[-2:] != 'a0':
-                supported = False
+            supported = False
+        if framework_version[-2:] != 'a0':
+            supported = True
         assert supported == True, \
             f"{NAME}-{DEEPGPU_VERSION} installed failed for not supporting torch with version: " \
             f"{framework_type}-{framework_version}+cu{cuda_version}-cp{python_version}"
         os.system(f'echo "check deepgpu-version successed!" >> {_temp_log} ')
 
     def run(self):
         # get env
```

