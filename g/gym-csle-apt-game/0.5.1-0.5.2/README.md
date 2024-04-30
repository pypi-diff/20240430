# Comparing `tmp/gym_csle_apt_game-0.5.1.tar.gz` & `tmp/gym_csle_apt_game-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym_csle_apt_game-0.5.1.tar", last modified: Tue Mar  5 17:31:05 2024, max compression
+gzip compressed data, was "gym_csle_apt_game-0.5.2.tar", last modified: Tue Apr 30 10:50:51 2024, max compression
```

## Comparing `gym_csle_apt_game-0.5.1.tar` & `gym_csle_apt_game-0.5.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:31:05.658272 gym_csle_apt_game-0.5.1/
--rw-r--r--   0 kim        (501) staff       (20)      704 2024-03-05 17:31:05.658378 gym_csle_apt_game-0.5.1/PKG-INFO
--rw-r--r--   0 kim        (501) staff       (20)      698 2024-02-13 12:24:16.000000 gym_csle_apt_game-0.5.1/pyproject.toml
--rw-r--r--   0 kim        (501) staff       (20)     1883 2024-03-05 17:31:05.659570 gym_csle_apt_game-0.5.1/setup.cfg
--rw-r--r--   0 kim        (501) staff       (20)       69 2024-02-13 12:24:16.000000 gym_csle_apt_game-0.5.1/setup.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:31:05.644201 gym_csle_apt_game-0.5.1/src/
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:31:05.647166 gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/
--rw-r--r--   0 kim        (501) staff       (20)      597 2024-02-13 12:24:16.000000 gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)       22 2024-03-05 17:30:08.000000 gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/__version__.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:31:05.652263 gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/constants/
--rw-r--r--   0 kim        (501) staff       (20)        0 2024-02-13 12:24:16.000000 gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/constants/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)      633 2024-02-13 12:24:16.000000 gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/constants/constants.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:31:05.654637 gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/dao/
--rw-r--r--   0 kim        (501) staff       (20)        0 2024-02-13 12:24:16.000000 gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/dao/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     3329 2024-02-13 12:24:16.000000 gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/dao/apt_game_attacker_mdp_config.py
--rw-r--r--   0 kim        (501) staff       (20)     5139 2024-02-13 12:24:16.000000 gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/dao/apt_game_config.py
--rw-r--r--   0 kim        (501) staff       (20)     3624 2024-02-13 12:24:16.000000 gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/dao/apt_game_defender_pomdp_config.py
--rw-r--r--   0 kim        (501) staff       (20)     2523 2024-02-13 12:24:16.000000 gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/dao/apt_game_state.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:31:05.656148 gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/envs/
--rw-r--r--   0 kim        (501) staff       (20)       74 2024-02-13 12:24:16.000000 gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/envs/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     9887 2024-02-13 12:24:16.000000 gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/envs/apt_game_env.py
--rw-r--r--   0 kim        (501) staff       (20)     9451 2024-02-13 12:24:16.000000 gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/envs/apt_game_mdp_attacker_env.py
--rw-r--r--   0 kim        (501) staff       (20)     6047 2024-02-13 12:24:16.000000 gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/envs/apt_game_pomdp_defender_env.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:31:05.657143 gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/util/
--rw-r--r--   0 kim        (501) staff       (20)        0 2024-02-13 12:24:16.000000 gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/util/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    14401 2024-02-13 12:24:16.000000 gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/util/apt_game_util.py
--rw-r--r--   0 kim        (501) staff       (20)    12988 2024-02-13 12:24:16.000000 gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/util/rollout_util.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:31:05.650516 gym_csle_apt_game-0.5.1/src/gym_csle_apt_game.egg-info/
--rw-r--r--   0 kim        (501) staff       (20)      704 2024-03-05 17:31:05.000000 gym_csle_apt_game-0.5.1/src/gym_csle_apt_game.egg-info/PKG-INFO
--rw-r--r--   0 kim        (501) staff       (20)     1083 2024-03-05 17:31:05.000000 gym_csle_apt_game-0.5.1/src/gym_csle_apt_game.egg-info/SOURCES.txt
--rw-r--r--   0 kim        (501) staff       (20)        1 2024-03-05 17:31:05.000000 gym_csle_apt_game-0.5.1/src/gym_csle_apt_game.egg-info/dependency_links.txt
--rw-r--r--   0 kim        (501) staff       (20)        1 2024-01-11 14:15:04.000000 gym_csle_apt_game-0.5.1/src/gym_csle_apt_game.egg-info/not-zip-safe
--rw-r--r--   0 kim        (501) staff       (20)      557 2024-03-05 17:31:05.000000 gym_csle_apt_game-0.5.1/src/gym_csle_apt_game.egg-info/requires.txt
--rw-r--r--   0 kim        (501) staff       (20)       18 2024-03-05 17:31:05.000000 gym_csle_apt_game-0.5.1/src/gym_csle_apt_game.egg-info/top_level.txt
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:31:05.657919 gym_csle_apt_game-0.5.1/tests/
--rw-r--r--   0 kim        (501) staff       (20)     4230 2024-02-13 12:24:16.000000 gym_csle_apt_game-0.5.1/tests/test_apt_game_dao.py
--rw-r--r--   0 kim        (501) staff       (20)      305 2024-02-13 12:24:16.000000 gym_csle_apt_game-0.5.1/tests/test_apt_game_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:51.779017 gym_csle_apt_game-0.5.2/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      704 2024-04-30 10:50:51.779017 gym_csle_apt_game-0.5.2/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      698 2024-01-29 11:24:00.000000 gym_csle_apt_game-0.5.2/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1883 2024-04-30 10:50:51.779017 gym_csle_apt_game-0.5.2/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2024-01-29 11:24:00.000000 gym_csle_apt_game-0.5.2/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:51.771017 gym_csle_apt_game-0.5.2/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:51.775017 gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      597 2024-01-29 11:24:00.000000 gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-04-30 10:49:10.000000 gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:51.775017 gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      633 2024-01-29 11:24:00.000000 gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:51.775017 gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/dao/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/dao/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3329 2024-01-29 11:24:00.000000 gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/dao/apt_game_attacker_mdp_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5139 2024-01-29 11:24:00.000000 gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/dao/apt_game_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3624 2024-01-29 11:24:00.000000 gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/dao/apt_game_defender_pomdp_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2523 2024-01-29 11:24:00.000000 gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/dao/apt_game_state.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:51.775017 gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/envs/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       74 2024-01-29 11:24:00.000000 gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/envs/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     9887 2024-01-29 12:14:49.000000 gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/envs/apt_game_env.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     9451 2024-01-29 12:14:49.000000 gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/envs/apt_game_mdp_attacker_env.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6047 2024-01-29 12:14:49.000000 gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/envs/apt_game_pomdp_defender_env.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:51.775017 gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/util/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/util/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    14401 2024-04-30 09:37:30.000000 gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/util/apt_game_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    12988 2024-01-29 11:24:00.000000 gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/util/rollout_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:51.775017 gym_csle_apt_game-0.5.2/src/gym_csle_apt_game.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      704 2024-04-30 10:50:51.000000 gym_csle_apt_game-0.5.2/src/gym_csle_apt_game.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1083 2024-04-30 10:50:51.000000 gym_csle_apt_game-0.5.2/src/gym_csle_apt_game.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-04-30 10:50:51.000000 gym_csle_apt_game-0.5.2/src/gym_csle_apt_game.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-12-02 14:34:38.000000 gym_csle_apt_game-0.5.2/src/gym_csle_apt_game.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      557 2024-04-30 10:50:51.000000 gym_csle_apt_game-0.5.2/src/gym_csle_apt_game.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       18 2024-04-30 10:50:51.000000 gym_csle_apt_game-0.5.2/src/gym_csle_apt_game.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:51.779017 gym_csle_apt_game-0.5.2/tests/
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4230 2024-04-30 09:37:30.000000 gym_csle_apt_game-0.5.2/tests/test_apt_game_dao.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      305 2024-01-29 11:24:00.000000 gym_csle_apt_game-0.5.2/tests/test_apt_game_util.py
```

### Comparing `gym_csle_apt_game-0.5.1/PKG-INFO` & `gym_csle_apt_game-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym_csle_apt_game
-Version: 0.5.1
+Version: 0.5.2
 Summary: OpenAI gym reinforcement learning environment of a Dynkin (Optimal stopping) APT game in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `gym_csle_apt_game-0.5.1/pyproject.toml` & `gym_csle_apt_game-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gym_csle_apt_game-0.5.1/setup.cfg` & `gym_csle_apt_game-0.5.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
 	gymnasium>=0.27.1
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

### Comparing `gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/__init__.py` & `gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/__init__.py`

 * *Files identical despite different names*

### Comparing `gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/constants/constants.py` & `gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/constants/constants.py`

 * *Files identical despite different names*

### Comparing `gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/dao/apt_game_attacker_mdp_config.py` & `gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/dao/apt_game_attacker_mdp_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/dao/apt_game_config.py` & `gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/dao/apt_game_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/dao/apt_game_defender_pomdp_config.py` & `gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/dao/apt_game_defender_pomdp_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/dao/apt_game_state.py` & `gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/dao/apt_game_state.py`

 * *Files identical despite different names*

### Comparing `gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/envs/apt_game_env.py` & `gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/envs/apt_game_env.py`

 * *Files identical despite different names*

### Comparing `gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/envs/apt_game_mdp_attacker_env.py` & `gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/envs/apt_game_mdp_attacker_env.py`

 * *Files identical despite different names*

### Comparing `gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/envs/apt_game_pomdp_defender_env.py` & `gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/envs/apt_game_pomdp_defender_env.py`

 * *Files identical despite different names*

### Comparing `gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/util/apt_game_util.py` & `gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/util/apt_game_util.py`

 * *Files identical despite different names*

### Comparing `gym_csle_apt_game-0.5.1/src/gym_csle_apt_game/util/rollout_util.py` & `gym_csle_apt_game-0.5.2/src/gym_csle_apt_game/util/rollout_util.py`

 * *Files identical despite different names*

### Comparing `gym_csle_apt_game-0.5.1/src/gym_csle_apt_game.egg-info/PKG-INFO` & `gym_csle_apt_game-0.5.2/src/gym_csle_apt_game.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-csle-apt-game
-Version: 0.5.1
+Version: 0.5.2
 Summary: OpenAI gym reinforcement learning environment of a Dynkin (Optimal stopping) APT game in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `gym_csle_apt_game-0.5.1/src/gym_csle_apt_game.egg-info/SOURCES.txt` & `gym_csle_apt_game-0.5.2/src/gym_csle_apt_game.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gym_csle_apt_game-0.5.1/src/gym_csle_apt_game.egg-info/requires.txt` & `gym_csle_apt_game-0.5.2/src/gym_csle_apt_game.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 gymnasium>=0.27.1
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

### Comparing `gym_csle_apt_game-0.5.1/tests/test_apt_game_dao.py` & `gym_csle_apt_game-0.5.2/tests/test_apt_game_dao.py`

 * *Files identical despite different names*

