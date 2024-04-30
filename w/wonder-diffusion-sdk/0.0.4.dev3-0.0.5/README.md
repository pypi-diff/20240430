# Comparing `tmp/wonder-diffusion-sdk-0.0.4.dev3.tar.gz` & `tmp/wonder-diffusion-sdk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wonder-diffusion-sdk-0.0.4.dev3.tar", last modified: Fri Apr 26 10:29:17 2024, max compression
+gzip compressed data, was "wonder-diffusion-sdk-0.0.5.tar", last modified: Tue Apr 30 13:07:42 2024, max compression
```

## Comparing `wonder-diffusion-sdk-0.0.4.dev3.tar` & `wonder-diffusion-sdk-0.0.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-26 10:29:17.591820 wonder-diffusion-sdk-0.0.4.dev3/
--rw-r--r--   0 basri      (501) staff       (20)     1080 2024-01-31 06:15:26.000000 wonder-diffusion-sdk-0.0.4.dev3/LICENCE
--rw-r--r--   0 basri      (501) staff       (20)      190 2024-04-26 10:29:17.591645 wonder-diffusion-sdk-0.0.4.dev3/PKG-INFO
--rw-r--r--   0 basri      (501) staff       (20)       38 2024-04-26 10:29:17.591877 wonder-diffusion-sdk-0.0.4.dev3/setup.cfg
--rw-r--r--   0 basri      (501) staff       (20)      319 2024-04-26 10:28:37.000000 wonder-diffusion-sdk-0.0.4.dev3/setup.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-26 10:29:17.580117 wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/
--rw-r--r--   0 basri      (501) staff       (20)    11121 2024-04-26 10:28:01.000000 wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/__init__.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-26 10:29:17.582787 wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/components/
--rw-r--r--   0 basri      (501) staff       (20)      199 2024-03-22 14:04:45.000000 wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/components/__init__.py
--rw-r--r--   0 basri      (501) staff       (20)      402 2024-03-22 14:04:23.000000 wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/components/deepcache.py
--rw-r--r--   0 basri      (501) staff       (20)      117 2024-02-28 08:41:39.000000 wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/components/dotdict.py
--rw-r--r--   0 basri      (501) staff       (20)      914 2024-04-17 08:38:18.000000 wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/components/lightning.py
--rw-r--r--   0 basri      (501) staff       (20)     1137 2024-03-11 09:11:53.000000 wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/components/logger.py
--rw-r--r--   0 basri      (501) staff       (20)     3207 2024-02-27 13:23:11.000000 wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/components/safety_checker.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-26 10:29:17.588125 wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/config/
--rw-r--r--   0 basri      (501) staff       (20)      237 2024-04-26 06:33:19.000000 wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/config/__init__.py
--rw-r--r--   0 basri      (501) staff       (20)      610 2024-04-26 06:43:03.000000 wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/config/controlnet_config.py
--rw-r--r--   0 basri      (501) staff       (20)       70 2024-03-20 09:12:50.000000 wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/config/globals.py
--rw-r--r--   0 basri      (501) staff       (20)     1182 2024-04-24 10:00:12.000000 wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/config/lora_config.py
--rw-r--r--   0 basri      (501) staff       (20)     1503 2024-03-22 14:14:11.000000 wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/config/model_config.py
--rw-r--r--   0 basri      (501) staff       (20)      197 2024-03-22 14:06:09.000000 wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/config/sdk_config.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-26 10:29:17.591247 wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/types/
--rw-r--r--   0 basri      (501) staff       (20)      257 2024-04-26 06:37:35.000000 wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/types/__init__.py
--rw-r--r--   0 basri      (501) staff       (20)       98 2024-04-26 10:27:36.000000 wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/types/controlnet_type.py
--rw-r--r--   0 basri      (501) staff       (20)      731 2024-04-26 10:27:42.000000 wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/types/controlnets.py
--rw-r--r--   0 basri      (501) staff       (20)      551 2024-04-26 06:33:19.000000 wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/types/pipeline_type.py
--rw-r--r--   0 basri      (501) staff       (20)     3002 2024-04-26 06:33:19.000000 wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/types/pipelines.py
--rw-r--r--   0 basri      (501) staff       (20)      815 2024-03-12 10:17:49.000000 wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/types/scheduler_type.py
--rw-r--r--   0 basri      (501) staff       (20)     3174 2024-03-22 13:38:15.000000 wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/types/schedulers.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-26 10:29:17.580947 wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk.egg-info/
--rw-r--r--   0 basri      (501) staff       (20)      190 2024-04-26 10:29:17.000000 wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk.egg-info/PKG-INFO
--rw-r--r--   0 basri      (501) staff       (20)     1091 2024-04-26 10:29:17.000000 wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 basri      (501) staff       (20)        1 2024-04-26 10:29:17.000000 wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 basri      (501) staff       (20)       18 2024-04-26 10:29:17.000000 wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk.egg-info/requires.txt
--rw-r--r--   0 basri      (501) staff       (20)       21 2024-04-26 10:29:17.000000 wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-30 13:07:42.788403 wonder-diffusion-sdk-0.0.5/
+-rw-r--r--   0 basri      (501) staff       (20)     1080 2024-01-31 06:15:26.000000 wonder-diffusion-sdk-0.0.5/LICENCE
+-rw-r--r--   0 basri      (501) staff       (20)      185 2024-04-30 13:07:42.788175 wonder-diffusion-sdk-0.0.5/PKG-INFO
+-rw-r--r--   0 basri      (501) staff       (20)       38 2024-04-30 13:07:42.788493 wonder-diffusion-sdk-0.0.5/setup.cfg
+-rw-r--r--   0 basri      (501) staff       (20)      314 2024-04-30 13:07:10.000000 wonder-diffusion-sdk-0.0.5/setup.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-30 13:07:42.781571 wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/
+-rw-r--r--   0 basri      (501) staff       (20)    11121 2024-04-30 13:01:39.000000 wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/__init__.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-30 13:07:42.784060 wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/components/
+-rw-r--r--   0 basri      (501) staff       (20)      199 2024-03-22 14:04:45.000000 wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/components/__init__.py
+-rw-r--r--   0 basri      (501) staff       (20)      402 2024-03-22 14:04:23.000000 wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/components/deepcache.py
+-rw-r--r--   0 basri      (501) staff       (20)      117 2024-02-28 08:41:39.000000 wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/components/dotdict.py
+-rw-r--r--   0 basri      (501) staff       (20)      914 2024-04-17 08:38:18.000000 wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/components/lightning.py
+-rw-r--r--   0 basri      (501) staff       (20)     1137 2024-03-11 09:11:53.000000 wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/components/logger.py
+-rw-r--r--   0 basri      (501) staff       (20)     3207 2024-02-27 13:23:11.000000 wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/components/safety_checker.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-30 13:07:42.785978 wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/config/
+-rw-r--r--   0 basri      (501) staff       (20)      237 2024-04-30 13:01:39.000000 wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/config/__init__.py
+-rw-r--r--   0 basri      (501) staff       (20)      610 2024-04-30 13:01:39.000000 wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/config/controlnet_config.py
+-rw-r--r--   0 basri      (501) staff       (20)       70 2024-03-20 09:12:50.000000 wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/config/globals.py
+-rw-r--r--   0 basri      (501) staff       (20)     1182 2024-04-29 12:32:04.000000 wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/config/lora_config.py
+-rw-r--r--   0 basri      (501) staff       (20)     1503 2024-03-22 14:14:11.000000 wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/config/model_config.py
+-rw-r--r--   0 basri      (501) staff       (20)      197 2024-03-22 14:06:09.000000 wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/config/sdk_config.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-30 13:07:42.787665 wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/types/
+-rw-r--r--   0 basri      (501) staff       (20)      257 2024-04-30 13:01:39.000000 wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/types/__init__.py
+-rw-r--r--   0 basri      (501) staff       (20)       98 2024-04-30 13:01:39.000000 wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/types/controlnet_type.py
+-rw-r--r--   0 basri      (501) staff       (20)      753 2024-04-30 13:07:10.000000 wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/types/controlnets.py
+-rw-r--r--   0 basri      (501) staff       (20)      551 2024-04-30 13:01:39.000000 wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/types/pipeline_type.py
+-rw-r--r--   0 basri      (501) staff       (20)     3002 2024-04-30 13:01:39.000000 wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/types/pipelines.py
+-rw-r--r--   0 basri      (501) staff       (20)      815 2024-03-12 10:17:49.000000 wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/types/scheduler_type.py
+-rw-r--r--   0 basri      (501) staff       (20)     3174 2024-03-22 13:38:15.000000 wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/types/schedulers.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-30 13:07:42.782398 wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk.egg-info/
+-rw-r--r--   0 basri      (501) staff       (20)      185 2024-04-30 13:07:42.000000 wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 basri      (501) staff       (20)     1091 2024-04-30 13:07:42.000000 wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 basri      (501) staff       (20)        1 2024-04-30 13:07:42.000000 wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 basri      (501) staff       (20)       18 2024-04-30 13:07:42.000000 wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk.egg-info/requires.txt
+-rw-r--r--   0 basri      (501) staff       (20)       21 2024-04-30 13:07:42.000000 wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk.egg-info/top_level.txt
```

### Comparing `wonder-diffusion-sdk-0.0.4.dev3/LICENCE` & `wonder-diffusion-sdk-0.0.5/LICENCE`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/__init__.py` & `wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/components/lightning.py` & `wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/components/lightning.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/components/logger.py` & `wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/components/logger.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/components/safety_checker.py` & `wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/components/safety_checker.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/config/controlnet_config.py` & `wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/config/controlnet_config.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/config/lora_config.py` & `wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/config/lora_config.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/config/model_config.py` & `wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/config/model_config.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/types/controlnets.py` & `wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/types/controlnets.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,12 +5,12 @@
 CONTROLNET_MAP = {
     WonderControlNetType.DEPTH: lambda pretrained_model_name_or_path, **kwargs: initialize_depth_controlnet(pretrained_model_name_or_path, **kwargs),
     WonderControlNetType.CANNY: lambda pretrained_model_name_or_path, **kwargs: initialize_canny_controlnet(pretrained_model_name_or_path, **kwargs),
 }
 
 
 def initialize_depth_controlnet(pretrained_model_name_or_path, **kwargs):
-    return ControlNetModel.from_pretrained(pretrained_model_name_or_path, **kwargs)
+    return ControlNetModel.from_pretrained(pretrained_model_name_or_path, **kwargs).to('cuda')
 
 
 def initialize_canny_controlnet(pretrained_model_name_or_path, **kwargs):
-    return ControlNetModel.from_pretrained(pretrained_model_name_or_path, **kwargs)
+    return ControlNetModel.from_pretrained(pretrained_model_name_or_path, **kwargs).to('cuda')
```

### Comparing `wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/types/pipeline_type.py` & `wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/types/pipeline_type.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/types/pipelines.py` & `wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/types/pipelines.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/types/scheduler_type.py` & `wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/types/scheduler_type.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk/types/schedulers.py` & `wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk/types/schedulers.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.4.dev3/wonder_diffusion_sdk.egg-info/SOURCES.txt` & `wonder-diffusion-sdk-0.0.5/wonder_diffusion_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

