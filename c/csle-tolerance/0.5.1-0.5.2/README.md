# Comparing `tmp/csle_tolerance-0.5.1.tar.gz` & `tmp/csle_tolerance-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_tolerance-0.5.1.tar", last modified: Tue Mar  5 17:31:00 2024, max compression
+gzip compressed data, was "csle_tolerance-0.5.2.tar", last modified: Tue Apr 30 10:50:43 2024, max compression
```

## Comparing `csle_tolerance-0.5.1.tar` & `csle_tolerance-0.5.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:31:00.261382 csle_tolerance-0.5.1/
--rw-r--r--   0 kim        (501) staff       (20)      741 2024-03-05 17:31:00.261443 csle_tolerance-0.5.1/PKG-INFO
--rw-r--r--   0 kim        (501) staff       (20)      674 2023-09-06 08:43:30.000000 csle_tolerance-0.5.1/pyproject.toml
--rw-r--r--   0 kim        (501) staff       (20)     1929 2024-03-05 17:31:00.261685 csle_tolerance-0.5.1/setup.cfg
--rw-r--r--   0 kim        (501) staff       (20)       69 2023-08-15 10:44:03.000000 csle_tolerance-0.5.1/setup.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:31:00.256778 csle_tolerance-0.5.1/src/
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:31:00.257595 csle_tolerance-0.5.1/src/csle_tolerance/
--rw-r--r--   0 kim        (501) staff       (20)       39 2023-09-15 16:43:44.000000 csle_tolerance-0.5.1/src/csle_tolerance/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)       22 2024-03-05 17:30:08.000000 csle_tolerance-0.5.1/src/csle_tolerance/__version__.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:31:00.258624 csle_tolerance-0.5.1/src/csle_tolerance/constants/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_tolerance-0.5.1/src/csle_tolerance/constants/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)      315 2023-10-09 07:12:58.000000 csle_tolerance-0.5.1/src/csle_tolerance/constants/constants.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:31:00.259360 csle_tolerance-0.5.1/src/csle_tolerance/dao/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-09-12 15:45:28.000000 csle_tolerance-0.5.1/src/csle_tolerance/dao/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     5699 2023-10-09 07:12:58.000000 csle_tolerance-0.5.1/src/csle_tolerance/dao/intrusion_recovery_pomdp_config.py
--rw-r--r--   0 kim        (501) staff       (20)     5231 2023-09-15 15:32:19.000000 csle_tolerance-0.5.1/src/csle_tolerance/dao/intrusion_response_cmdp_config.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:31:00.260076 csle_tolerance-0.5.1/src/csle_tolerance/envs/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-09-12 15:44:05.000000 csle_tolerance-0.5.1/src/csle_tolerance/envs/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    11235 2024-02-13 12:24:16.000000 csle_tolerance-0.5.1/src/csle_tolerance/envs/intrusion_recovery_pomdp_env.py
--rw-r--r--   0 kim        (501) staff       (20)     8025 2024-02-13 12:24:16.000000 csle_tolerance-0.5.1/src/csle_tolerance/envs/intrusion_response_cmdp_env.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:31:00.261052 csle_tolerance-0.5.1/src/csle_tolerance/util/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-09-08 12:46:59.000000 csle_tolerance-0.5.1/src/csle_tolerance/util/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     2587 2023-09-15 16:48:21.000000 csle_tolerance-0.5.1/src/csle_tolerance/util/general_util.py
--rw-r--r--   0 kim        (501) staff       (20)    13315 2023-09-15 16:33:36.000000 csle_tolerance-0.5.1/src/csle_tolerance/util/intrusion_recovery_pomdp_util.py
--rw-r--r--   0 kim        (501) staff       (20)     5895 2023-09-15 16:34:23.000000 csle_tolerance-0.5.1/src/csle_tolerance/util/intrusion_response_cmdp_util.py
--rw-r--r--   0 kim        (501) staff       (20)     2058 2023-10-09 07:12:58.000000 csle_tolerance-0.5.1/src/csle_tolerance/util/pomdp_solve_parser.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:31:00.258430 csle_tolerance-0.5.1/src/csle_tolerance.egg-info/
--rw-r--r--   0 kim        (501) staff       (20)      741 2024-03-05 17:31:00.000000 csle_tolerance-0.5.1/src/csle_tolerance.egg-info/PKG-INFO
--rw-r--r--   0 kim        (501) staff       (20)     1007 2024-03-05 17:31:00.000000 csle_tolerance-0.5.1/src/csle_tolerance.egg-info/SOURCES.txt
--rw-r--r--   0 kim        (501) staff       (20)        1 2024-03-05 17:31:00.000000 csle_tolerance-0.5.1/src/csle_tolerance.egg-info/dependency_links.txt
--rw-r--r--   0 kim        (501) staff       (20)        1 2023-09-14 11:59:31.000000 csle_tolerance-0.5.1/src/csle_tolerance.egg-info/not-zip-safe
--rw-r--r--   0 kim        (501) staff       (20)      571 2024-03-05 17:31:00.000000 csle_tolerance-0.5.1/src/csle_tolerance.egg-info/requires.txt
--rw-r--r--   0 kim        (501) staff       (20)       15 2024-03-05 17:31:00.000000 csle_tolerance-0.5.1/src/csle_tolerance.egg-info/top_level.txt
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:31:00.261178 csle_tolerance-0.5.1/tests/
--rw-r--r--   0 kim        (501) staff       (20)      405 2023-09-15 12:17:06.000000 csle_tolerance-0.5.1/tests/test_intrusion_recovery_pomdp_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:43.162974 csle_tolerance-0.5.2/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      741 2024-04-30 10:50:43.162974 csle_tolerance-0.5.2/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      674 2024-01-29 11:24:00.000000 csle_tolerance-0.5.2/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1929 2024-04-30 10:50:43.162974 csle_tolerance-0.5.2/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2024-01-29 11:24:00.000000 csle_tolerance-0.5.2/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:43.154974 csle_tolerance-0.5.2/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:43.154974 csle_tolerance-0.5.2/src/csle_tolerance/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       39 2024-01-29 11:24:00.000000 csle_tolerance-0.5.2/src/csle_tolerance/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-04-30 10:49:10.000000 csle_tolerance-0.5.2/src/csle_tolerance/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:43.158974 csle_tolerance-0.5.2/src/csle_tolerance/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_tolerance-0.5.2/src/csle_tolerance/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      315 2024-01-29 11:24:00.000000 csle_tolerance-0.5.2/src/csle_tolerance/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:43.158974 csle_tolerance-0.5.2/src/csle_tolerance/dao/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_tolerance-0.5.2/src/csle_tolerance/dao/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5699 2024-01-29 11:24:00.000000 csle_tolerance-0.5.2/src/csle_tolerance/dao/intrusion_recovery_pomdp_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5231 2024-01-29 11:24:00.000000 csle_tolerance-0.5.2/src/csle_tolerance/dao/intrusion_response_cmdp_config.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:43.158974 csle_tolerance-0.5.2/src/csle_tolerance/envs/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_tolerance-0.5.2/src/csle_tolerance/envs/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11235 2024-01-29 12:14:49.000000 csle_tolerance-0.5.2/src/csle_tolerance/envs/intrusion_recovery_pomdp_env.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8025 2024-01-29 12:14:49.000000 csle_tolerance-0.5.2/src/csle_tolerance/envs/intrusion_response_cmdp_env.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:43.158974 csle_tolerance-0.5.2/src/csle_tolerance/util/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_tolerance-0.5.2/src/csle_tolerance/util/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2587 2024-01-29 11:24:00.000000 csle_tolerance-0.5.2/src/csle_tolerance/util/general_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    13315 2024-01-29 11:24:00.000000 csle_tolerance-0.5.2/src/csle_tolerance/util/intrusion_recovery_pomdp_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5895 2024-01-29 11:24:00.000000 csle_tolerance-0.5.2/src/csle_tolerance/util/intrusion_response_cmdp_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2058 2024-01-29 11:24:00.000000 csle_tolerance-0.5.2/src/csle_tolerance/util/pomdp_solve_parser.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:43.158974 csle_tolerance-0.5.2/src/csle_tolerance.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      741 2024-04-30 10:50:43.000000 csle_tolerance-0.5.2/src/csle_tolerance.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1007 2024-04-30 10:50:43.000000 csle_tolerance-0.5.2/src/csle_tolerance.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-04-30 10:50:43.000000 csle_tolerance-0.5.2/src/csle_tolerance.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-09-16 07:31:36.000000 csle_tolerance-0.5.2/src/csle_tolerance.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      571 2024-04-30 10:50:43.000000 csle_tolerance-0.5.2/src/csle_tolerance.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       15 2024-04-30 10:50:43.000000 csle_tolerance-0.5.2/src/csle_tolerance.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:43.158974 csle_tolerance-0.5.2/tests/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      405 2024-01-29 11:24:00.000000 csle_tolerance-0.5.2/tests/test_intrusion_recovery_pomdp_util.py
```

### Comparing `csle_tolerance-0.5.1/PKG-INFO` & `csle_tolerance-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_tolerance
-Version: 0.5.1
+Version: 0.5.2
 Summary: An intrusion-tolerant system: Tolerance: (T)w(o)-(l)ev(e)l (r)ecovery (a)nd respo(n)se (c)ontrol with f(e)edback.
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes Intrusion-tolerance
 Platform: unix
 Platform: linux
```

### Comparing `csle_tolerance-0.5.1/pyproject.toml` & `csle_tolerance-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.5.1/setup.cfg` & `csle_tolerance-0.5.2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
 	gymnasium>=0.27.1
 	numpy>=1.23.5
-	csle-base>=0.5.1
-	csle-common>=0.5.1
-	csle-attacker>=0.5.1
-	csle-defender>=0.5.1
-	csle-collector>=0.5.1
+	csle-base>=0.5.2
+	csle-common>=0.5.2
+	csle-attacker>=0.5.2
+	csle-defender>=0.5.2
+	csle-collector>=0.5.2
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `csle_tolerance-0.5.1/src/csle_tolerance/dao/intrusion_recovery_pomdp_config.py` & `csle_tolerance-0.5.2/src/csle_tolerance/dao/intrusion_recovery_pomdp_config.py`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.5.1/src/csle_tolerance/dao/intrusion_response_cmdp_config.py` & `csle_tolerance-0.5.2/src/csle_tolerance/dao/intrusion_response_cmdp_config.py`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.5.1/src/csle_tolerance/envs/intrusion_recovery_pomdp_env.py` & `csle_tolerance-0.5.2/src/csle_tolerance/envs/intrusion_recovery_pomdp_env.py`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.5.1/src/csle_tolerance/envs/intrusion_response_cmdp_env.py` & `csle_tolerance-0.5.2/src/csle_tolerance/envs/intrusion_response_cmdp_env.py`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.5.1/src/csle_tolerance/util/general_util.py` & `csle_tolerance-0.5.2/src/csle_tolerance/util/general_util.py`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.5.1/src/csle_tolerance/util/intrusion_recovery_pomdp_util.py` & `csle_tolerance-0.5.2/src/csle_tolerance/util/intrusion_recovery_pomdp_util.py`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.5.1/src/csle_tolerance/util/intrusion_response_cmdp_util.py` & `csle_tolerance-0.5.2/src/csle_tolerance/util/intrusion_response_cmdp_util.py`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.5.1/src/csle_tolerance/util/pomdp_solve_parser.py` & `csle_tolerance-0.5.2/src/csle_tolerance/util/pomdp_solve_parser.py`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.5.1/src/csle_tolerance.egg-info/PKG-INFO` & `csle_tolerance-0.5.2/src/csle_tolerance.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-tolerance
-Version: 0.5.1
+Version: 0.5.2
 Summary: An intrusion-tolerant system: Tolerance: (T)w(o)-(l)ev(e)l (r)ecovery (a)nd respo(n)se (c)ontrol with f(e)edback.
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes Intrusion-tolerance
 Platform: unix
 Platform: linux
```

### Comparing `csle_tolerance-0.5.1/src/csle_tolerance.egg-info/SOURCES.txt` & `csle_tolerance-0.5.2/src/csle_tolerance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.5.1/src/csle_tolerance.egg-info/requires.txt` & `csle_tolerance-0.5.2/src/csle_tolerance.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 gymnasium>=0.27.1
 numpy>=1.23.5
-csle-base>=0.5.1
-csle-common>=0.5.1
-csle-attacker>=0.5.1
-csle-defender>=0.5.1
-csle-collector>=0.5.1
+csle-base>=0.5.2
+csle-common>=0.5.2
+csle-attacker>=0.5.2
+csle-defender>=0.5.2
+csle-collector>=0.5.2
 
 [testing]
 pytest>=6.0
 pytest-cov>=2.0
 pytest-mock>=3.6.0
 grpcio>=1.57.0
 grpcio-tools>=1.57.0
```

