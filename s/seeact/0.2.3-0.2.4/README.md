# Comparing `tmp/seeact-0.2.3.tar.gz` & `tmp/seeact-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seeact-0.2.3.tar", last modified: Mon Apr 29 00:52:07 2024, max compression
+gzip compressed data, was "seeact-0.2.4.tar", last modified: Mon Apr 29 22:15:43 2024, max compression
```

## Comparing `seeact-0.2.3.tar` & `seeact-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-29 00:52:07.360027 seeact-0.2.3/
--rw-r--r--   0 geminigby   (501) staff       (20)    11495 2024-04-29 00:05:59.000000 seeact-0.2.3/LICENSE
--rw-r--r--   0 geminigby   (501) staff       (20)    13352 2024-04-29 00:52:07.359737 seeact-0.2.3/PKG-INFO
--rw-r--r--   0 geminigby   (501) staff       (20)     1123 2024-04-29 00:52:03.000000 seeact-0.2.3/pyproject.toml
-drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-29 00:52:07.356765 seeact-0.2.3/seeact/
--rw-r--r--   0 geminigby   (501) staff       (20)      607 2024-04-29 00:05:59.000000 seeact-0.2.3/seeact/__init__.py
--rw-r--r--   0 geminigby   (501) staff       (20)    32251 2024-04-29 00:52:03.000000 seeact-0.2.3/seeact/agent.py
-drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-29 00:52:07.358243 seeact-0.2.3/seeact/data_utils/
--rw-r--r--   0 geminigby   (501) staff       (20)      607 2024-04-29 00:05:59.000000 seeact-0.2.3/seeact/data_utils/__init__.py
--rw-r--r--   0 geminigby   (501) staff       (20)     4278 2024-04-29 00:05:59.000000 seeact-0.2.3/seeact/data_utils/format_prompt_utils.py
--rw-r--r--   0 geminigby   (501) staff       (20)     7487 2024-04-29 00:05:59.000000 seeact-0.2.3/seeact/data_utils/prompts.py
-drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-29 00:52:07.359104 seeact-0.2.3/seeact/demo_utils/
--rw-r--r--   0 geminigby   (501) staff       (20)        0 2024-04-29 00:05:59.000000 seeact-0.2.3/seeact/demo_utils/__init__.py
--rw-r--r--   0 geminigby   (501) staff       (20)    13193 2024-04-29 00:45:49.000000 seeact-0.2.3/seeact/demo_utils/browser_helper.py
--rw-r--r--   0 geminigby   (501) staff       (20)     7555 2024-04-29 00:05:59.000000 seeact-0.2.3/seeact/demo_utils/format_prompt.py
--rw-r--r--   0 geminigby   (501) staff       (20)     8411 2024-04-29 00:05:59.000000 seeact-0.2.3/seeact/demo_utils/inference_engine.py
-drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-29 00:52:07.359479 seeact-0.2.3/seeact.egg-info/
--rw-r--r--   0 geminigby   (501) staff       (20)    13352 2024-04-29 00:52:07.000000 seeact-0.2.3/seeact.egg-info/PKG-INFO
--rw-r--r--   0 geminigby   (501) staff       (20)      445 2024-04-29 00:52:07.000000 seeact-0.2.3/seeact.egg-info/SOURCES.txt
--rw-r--r--   0 geminigby   (501) staff       (20)        1 2024-04-29 00:52:07.000000 seeact-0.2.3/seeact.egg-info/dependency_links.txt
--rw-r--r--   0 geminigby   (501) staff       (20)       53 2024-04-29 00:52:07.000000 seeact-0.2.3/seeact.egg-info/requires.txt
--rw-r--r--   0 geminigby   (501) staff       (20)        7 2024-04-29 00:52:07.000000 seeact-0.2.3/seeact.egg-info/top_level.txt
--rw-r--r--   0 geminigby   (501) staff       (20)       38 2024-04-29 00:52:07.360098 seeact-0.2.3/setup.cfg
+drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-29 22:15:43.513302 seeact-0.2.4/
+-rw-r--r--   0 geminigby   (501) staff       (20)    11495 2024-04-29 00:05:59.000000 seeact-0.2.4/LICENSE
+-rw-r--r--   0 geminigby   (501) staff       (20)    13352 2024-04-29 22:15:43.512911 seeact-0.2.4/PKG-INFO
+-rw-r--r--   0 geminigby   (501) staff       (20)     1123 2024-04-29 22:15:29.000000 seeact-0.2.4/pyproject.toml
+drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-29 22:15:43.507993 seeact-0.2.4/seeact/
+-rw-r--r--   0 geminigby   (501) staff       (20)      607 2024-04-29 00:05:59.000000 seeact-0.2.4/seeact/__init__.py
+-rw-r--r--   0 geminigby   (501) staff       (20)    32298 2024-04-29 22:15:29.000000 seeact-0.2.4/seeact/agent.py
+drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-29 22:15:43.510120 seeact-0.2.4/seeact/data_utils/
+-rw-r--r--   0 geminigby   (501) staff       (20)      607 2024-04-29 00:05:59.000000 seeact-0.2.4/seeact/data_utils/__init__.py
+-rw-r--r--   0 geminigby   (501) staff       (20)     4278 2024-04-29 00:05:59.000000 seeact-0.2.4/seeact/data_utils/format_prompt_utils.py
+-rw-r--r--   0 geminigby   (501) staff       (20)     7487 2024-04-29 00:05:59.000000 seeact-0.2.4/seeact/data_utils/prompts.py
+drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-29 22:15:43.511403 seeact-0.2.4/seeact/demo_utils/
+-rw-r--r--   0 geminigby   (501) staff       (20)        0 2024-04-29 00:05:59.000000 seeact-0.2.4/seeact/demo_utils/__init__.py
+-rw-r--r--   0 geminigby   (501) staff       (20)    13193 2024-04-29 00:45:49.000000 seeact-0.2.4/seeact/demo_utils/browser_helper.py
+-rw-r--r--   0 geminigby   (501) staff       (20)     7555 2024-04-29 00:05:59.000000 seeact-0.2.4/seeact/demo_utils/format_prompt.py
+-rw-r--r--   0 geminigby   (501) staff       (20)     8411 2024-04-29 00:05:59.000000 seeact-0.2.4/seeact/demo_utils/inference_engine.py
+drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-29 22:15:43.512020 seeact-0.2.4/seeact.egg-info/
+-rw-r--r--   0 geminigby   (501) staff       (20)    13352 2024-04-29 22:15:43.000000 seeact-0.2.4/seeact.egg-info/PKG-INFO
+-rw-r--r--   0 geminigby   (501) staff       (20)      445 2024-04-29 22:15:43.000000 seeact-0.2.4/seeact.egg-info/SOURCES.txt
+-rw-r--r--   0 geminigby   (501) staff       (20)        1 2024-04-29 22:15:43.000000 seeact-0.2.4/seeact.egg-info/dependency_links.txt
+-rw-r--r--   0 geminigby   (501) staff       (20)       53 2024-04-29 22:15:43.000000 seeact-0.2.4/seeact.egg-info/requires.txt
+-rw-r--r--   0 geminigby   (501) staff       (20)        7 2024-04-29 22:15:43.000000 seeact-0.2.4/seeact.egg-info/top_level.txt
+-rw-r--r--   0 geminigby   (501) staff       (20)       38 2024-04-29 22:15:43.513453 seeact-0.2.4/setup.cfg
```

### Comparing `seeact-0.2.3/LICENSE` & `seeact-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `seeact-0.2.3/PKG-INFO` & `seeact-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeact
-Version: 0.2.3
+Version: 0.2.4
 Summary: SeeAct is a system for generalist web agents that autonomously carry out tasks on any given website, with a focus on large multimodal models (LMMs) such as GPT-4V(ision). It consists of two main components: (1) A robust codebase that supports running web agents on live websites, and (2) an innovative framework that utilizes LMMs as generalist web agents.
 Author-email: Boyu Gou <gou.43@buckeyemail.osu.edu>, Boyuan Zheng <zheng.2372@osu.edu>, Zheng Du <du.913@buckeyemail.osu.edu>
 License: AI PUBS OPEN RAIL-S LICENSE
         Version 0.1, March 2, 2023
         
         http://licenses.ai/
```

### Comparing `seeact-0.2.3/pyproject.toml` & `seeact-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "seeact"
-version = "0.2.3"
+version = "0.2.4"
 description = "SeeAct is a system for generalist web agents that autonomously carry out tasks on any given website, with a focus on large multimodal models (LMMs) such as GPT-4V(ision). It consists of two main components: (1) A robust codebase that supports running web agents on live websites, and (2) an innovative framework that utilizes LMMs as generalist web agents."
 authors = [
     {name = "Boyu Gou", email = "gou.43@buckeyemail.osu.edu"},
     {name = "Boyuan Zheng", email = "zheng.2372@osu.edu"},
     {name = "Zheng Du", email = "du.913@buckeyemail.osu.edu"}
 ]
 license = {file="LICENSE"}
```

### Comparing `seeact-0.2.3/seeact/__init__.py` & `seeact-0.2.4/seeact/__init__.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.3/seeact/agent.py` & `seeact-0.2.4/seeact/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,14 +64,15 @@
                  ):
 
         try:
             if config_path is not None:
                 with open(config_path,
                           'r') as config:
                     print(f"Configuration File Loaded - {config_path}")
+                    config = toml.load(config)
             else:
                 config = {
                     "basic": {
                         "save_file_dir": save_file_dir,
                         "default_task": default_task,
                         "default_website": default_website
                     },
```

### Comparing `seeact-0.2.3/seeact/data_utils/__init__.py` & `seeact-0.2.4/seeact/data_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.3/seeact/data_utils/format_prompt_utils.py` & `seeact-0.2.4/seeact/data_utils/format_prompt_utils.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.3/seeact/data_utils/prompts.py` & `seeact-0.2.4/seeact/data_utils/prompts.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.3/seeact/demo_utils/browser_helper.py` & `seeact-0.2.4/seeact/demo_utils/browser_helper.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.3/seeact/demo_utils/format_prompt.py` & `seeact-0.2.4/seeact/demo_utils/format_prompt.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.3/seeact/demo_utils/inference_engine.py` & `seeact-0.2.4/seeact/demo_utils/inference_engine.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.3/seeact.egg-info/PKG-INFO` & `seeact-0.2.4/seeact.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeact
-Version: 0.2.3
+Version: 0.2.4
 Summary: SeeAct is a system for generalist web agents that autonomously carry out tasks on any given website, with a focus on large multimodal models (LMMs) such as GPT-4V(ision). It consists of two main components: (1) A robust codebase that supports running web agents on live websites, and (2) an innovative framework that utilizes LMMs as generalist web agents.
 Author-email: Boyu Gou <gou.43@buckeyemail.osu.edu>, Boyuan Zheng <zheng.2372@osu.edu>, Zheng Du <du.913@buckeyemail.osu.edu>
 License: AI PUBS OPEN RAIL-S LICENSE
         Version 0.1, March 2, 2023
         
         http://licenses.ai/
```

