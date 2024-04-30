# Comparing `tmp/csle_cli-0.5.1.tar.gz` & `tmp/csle_cli-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_cli-0.5.1.tar", last modified: Tue Mar  5 17:30:54 2024, max compression
+gzip compressed data, was "csle_cli-0.5.2.tar", last modified: Tue Apr 30 10:50:31 2024, max compression
```

## Comparing `csle_cli-0.5.1.tar` & `csle_cli-0.5.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:54.718498 csle_cli-0.5.1/
--rw-r--r--   0 kim        (501) staff       (20)      619 2024-03-05 17:30:54.718543 csle_cli-0.5.1/PKG-INFO
--rw-r--r--   0 kim        (501) staff       (20)    23697 2024-02-13 12:24:16.000000 csle_cli-0.5.1/README.md
--rw-r--r--   0 kim        (501) staff       (20)      668 2023-08-15 10:44:03.000000 csle_cli-0.5.1/pyproject.toml
--rw-r--r--   0 kim        (501) staff       (20)     1998 2024-03-05 17:30:54.718780 csle_cli-0.5.1/setup.cfg
--rw-r--r--   0 kim        (501) staff       (20)       69 2023-08-15 10:44:03.000000 csle_cli-0.5.1/setup.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:54.716353 csle_cli-0.5.1/src/
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:54.717394 csle_cli-0.5.1/src/csle_cli/
--rw-r--r--   0 kim        (501) staff       (20)       38 2023-08-15 10:44:03.000000 csle_cli-0.5.1/src/csle_cli/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)       22 2024-03-05 17:30:08.000000 csle_cli-0.5.1/src/csle_cli/__version__.py
--rwxr-xr-x   0 kim        (501) staff       (20)   118280 2024-03-05 13:14:43.000000 csle_cli-0.5.1/src/csle_cli/cli.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:54.718293 csle_cli-0.5.1/src/csle_cli.egg-info/
--rw-r--r--   0 kim        (501) staff       (20)      619 2024-03-05 17:30:54.000000 csle_cli-0.5.1/src/csle_cli.egg-info/PKG-INFO
--rw-r--r--   0 kim        (501) staff       (20)      387 2024-03-05 17:30:54.000000 csle_cli-0.5.1/src/csle_cli.egg-info/SOURCES.txt
--rw-r--r--   0 kim        (501) staff       (20)        1 2024-03-05 17:30:54.000000 csle_cli-0.5.1/src/csle_cli.egg-info/dependency_links.txt
--rw-r--r--   0 kim        (501) staff       (20)       47 2024-03-05 17:30:54.000000 csle_cli-0.5.1/src/csle_cli.egg-info/entry_points.txt
--rw-r--r--   0 kim        (501) staff       (20)        1 2023-08-16 11:40:31.000000 csle_cli-0.5.1/src/csle_cli.egg-info/not-zip-safe
--rw-r--r--   0 kim        (501) staff       (20)      699 2024-03-05 17:30:54.000000 csle_cli-0.5.1/src/csle_cli.egg-info/requires.txt
--rw-r--r--   0 kim        (501) staff       (20)        9 2024-03-05 17:30:54.000000 csle_cli-0.5.1/src/csle_cli.egg-info/top_level.txt
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:54.718387 csle_cli-0.5.1/tests/
--rw-r--r--   0 kim        (501) staff       (20)      352 2023-08-15 10:44:03.000000 csle_cli-0.5.1/tests/test_cli.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:31.894918 csle_cli-0.5.2/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      619 2024-04-30 10:50:31.894918 csle_cli-0.5.2/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)    23697 2024-01-29 12:14:49.000000 csle_cli-0.5.2/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      668 2023-08-08 14:54:06.000000 csle_cli-0.5.2/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1998 2024-04-30 10:50:31.894918 csle_cli-0.5.2/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_cli-0.5.2/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:31.890918 csle_cli-0.5.2/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:31.894918 csle_cli-0.5.2/src/csle_cli/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       38 2023-03-28 14:03:22.000000 csle_cli-0.5.2/src/csle_cli/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-04-30 10:49:10.000000 csle_cli-0.5.2/src/csle_cli/__version__.py
+-rwxrwxr-x   0 kim       (1000) kim       (1000)   118330 2024-04-30 09:37:30.000000 csle_cli-0.5.2/src/csle_cli/cli.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:31.894918 csle_cli-0.5.2/src/csle_cli.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      619 2024-04-30 10:50:31.000000 csle_cli-0.5.2/src/csle_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      387 2024-04-30 10:50:31.000000 csle_cli-0.5.2/src/csle_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-04-30 10:50:31.000000 csle_cli-0.5.2/src/csle_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       47 2024-04-30 10:50:31.000000 csle_cli-0.5.2/src/csle_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:51:27.000000 csle_cli-0.5.2/src/csle_cli.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      699 2024-04-30 10:50:31.000000 csle_cli-0.5.2/src/csle_cli.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        9 2024-04-30 10:50:31.000000 csle_cli-0.5.2/src/csle_cli.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:31.894918 csle_cli-0.5.2/tests/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      352 2023-08-08 14:54:06.000000 csle_cli-0.5.2/tests/test_cli.py
```

### Comparing `csle_cli-0.5.1/PKG-INFO` & `csle_cli-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_cli
-Version: 0.5.1
+Version: 0.5.2
 Summary: CLI tool for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_cli-0.5.1/README.md` & `csle_cli-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `csle_cli-0.5.1/pyproject.toml` & `csle_cli-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_cli-0.5.1/setup.cfg` & `csle_cli-0.5.2/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
 	click>=8.1.3
-	csle-base>=0.5.1
-	csle-common>=0.5.1
-	csle-cluster>=0.5.1
-	csle-collector>=0.5.1
-	csle-attacker>=0.5.1
-	csle-defender>=0.5.1
-	csle-system-identification>=0.5.1
-	gym-csle-stopping-game>=0.5.1
-	gym-csle-apt-game>=0.5.1
-	gym-csle-cyborg>=0.5.1
-	gym-csle-intrusion-response-game>=0.5.1
-	csle-agents>=0.5.1
-	csle-tolerance>=0.5.1
+	csle-base>=0.5.2
+	csle-common>=0.5.2
+	csle-cluster>=0.5.2
+	csle-collector>=0.5.2
+	csle-attacker>=0.5.2
+	csle-defender>=0.5.2
+	csle-system-identification>=0.5.2
+	gym-csle-stopping-game>=0.5.2
+	gym-csle-apt-game>=0.5.2
+	gym-csle-cyborg>=0.5.2
+	gym-csle-intrusion-response-game>=0.5.2
+	csle-agents>=0.5.2
+	csle-tolerance>=0.5.2
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `csle_cli-0.5.1/src/csle_cli/cli.py` & `csle_cli-0.5.2/src/csle_cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 
 To see options, run:
 `csle --help`
 """
 import logging
 from typing import List, Tuple, Union
 import click
+import warnings
+
+warnings.filterwarnings("ignore")
 from csle_common.dao.simulation_config.simulation_env_config import SimulationEnvConfig
 from csle_common.util.cluster_util import ClusterUtil
 from csle_common.util.general_util import GeneralUtil
 from csle_cluster.cluster_manager.cluster_controller import ClusterController
 from csle_cluster.cluster_manager.cluster_manager_pb2 import DockerContainerDTO
 from csle_common.dao.emulation_config.emulation_env_state import EmulationEnvState
 from csle_common.dao.emulation_config.emulation_env_config import EmulationEnvConfig
@@ -2001,15 +2004,15 @@
     for node in config.cluster_config.cluster_nodes:
         node_status = ClusterController.get_node_status(ip=node.ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT)
         if node_status.nodeExporterRunning:
             click.secho("Node exporter status: " + f" {click.style('[running]', fg='green')} "
                                                    f"ip:{node.ip}, port:{constants.COMMANDS.NODE_EXPORTER_PORT}",
                         bold=False)
         else:
-            click.secho("Node exporter status: " + f" {click.style('[stopped],', fg='red')} ip:{node.ip}",
+            click.secho("Node exporter status: " + f" {click.style('[stopped]', fg='red')} ip:{node.ip}",
                         bold=False)
 
 
 def list_prometheus() -> None:
     """
     Lists status of prometheus
```

### Comparing `csle_cli-0.5.1/src/csle_cli.egg-info/PKG-INFO` & `csle_cli-0.5.2/src/csle_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-cli
-Version: 0.5.1
+Version: 0.5.2
 Summary: CLI tool for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_cli-0.5.1/src/csle_cli.egg-info/requires.txt` & `csle_cli-0.5.2/src/csle_cli.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 click>=8.1.3
-csle-base>=0.5.1
-csle-common>=0.5.1
-csle-cluster>=0.5.1
-csle-collector>=0.5.1
-csle-attacker>=0.5.1
-csle-defender>=0.5.1
-csle-system-identification>=0.5.1
-gym-csle-stopping-game>=0.5.1
-gym-csle-apt-game>=0.5.1
-gym-csle-cyborg>=0.5.1
-gym-csle-intrusion-response-game>=0.5.1
-csle-agents>=0.5.1
-csle-tolerance>=0.5.1
+csle-base>=0.5.2
+csle-common>=0.5.2
+csle-cluster>=0.5.2
+csle-collector>=0.5.2
+csle-attacker>=0.5.2
+csle-defender>=0.5.2
+csle-system-identification>=0.5.2
+gym-csle-stopping-game>=0.5.2
+gym-csle-apt-game>=0.5.2
+gym-csle-cyborg>=0.5.2
+gym-csle-intrusion-response-game>=0.5.2
+csle-agents>=0.5.2
+csle-tolerance>=0.5.2
 
 [testing]
 pytest>=6.0
 pytest-cov>=2.0
 pytest-mock>=3.6.0
 grpcio>=1.57.0
 grpcio-tools>=1.57.0
```

