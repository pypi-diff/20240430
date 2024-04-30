# Comparing `tmp/blendr_cli-0.1.2.tar.gz` & `tmp/blendr_cli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blendr_cli-0.1.2.tar", last modified: Tue Apr 30 06:44:49 2024, max compression
+gzip compressed data, was "blendr_cli-0.1.3.tar", last modified: Tue Apr 30 15:23:08 2024, max compression
```

## Comparing `blendr_cli-0.1.2.tar` & `blendr_cli-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 06:44:49.185078 blendr_cli-0.1.2/
--rw-r--r--   0 stefanshiloh   (501) staff       (20)     3079 2024-04-30 06:44:49.184860 blendr_cli-0.1.2/PKG-INFO
--rw-r--r--   0 stefanshiloh   (501) staff       (20)     2677 2024-04-29 20:20:22.000000 blendr_cli-0.1.2/README.md
-drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 06:44:49.181828 blendr_cli-0.1.2/blendr/
--rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-20 16:49:51.000000 blendr_cli-0.1.2/blendr/__init__.py
-drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 06:44:49.182221 blendr_cli-0.1.2/blendr/auth/
--rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-21 17:20:43.000000 blendr_cli-0.1.2/blendr/auth/__init__.py
--rw-r--r--   0 stefanshiloh   (501) staff       (20)     2021 2024-04-28 21:02:26.000000 blendr_cli-0.1.2/blendr/auth/authenticate.py
--rw-r--r--   0 stefanshiloh   (501) staff       (20)     1867 2024-04-29 18:25:08.000000 blendr_cli-0.1.2/blendr/cli.py
-drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 06:44:49.182844 blendr_cli-0.1.2/blendr/config/
--rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-21 17:20:41.000000 blendr_cli-0.1.2/blendr/config/__init__.py
--rw-r--r--   0 stefanshiloh   (501) staff       (20)      119 2024-04-29 18:47:00.000000 blendr_cli-0.1.2/blendr/config/settings.py
--rw-r--r--   0 stefanshiloh   (501) staff       (20)     3440 2024-04-29 18:27:36.000000 blendr_cli-0.1.2/blendr/config/setup.py
-drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 06:44:49.183217 blendr_cli-0.1.2/blendr/gpu_manager/
--rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-29 22:27:38.000000 blendr_cli-0.1.2/blendr/gpu_manager/__init__.py
--rw-r--r--   0 stefanshiloh   (501) staff       (20)      190 2024-04-29 20:05:17.000000 blendr_cli-0.1.2/blendr/gpu_manager/detect.py
-drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 06:44:49.183581 blendr_cli-0.1.2/blendr/task_manager/
--rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-29 22:27:33.000000 blendr_cli-0.1.2/blendr/task_manager/__init__.py
--rw-r--r--   0 stefanshiloh   (501) staff       (20)     2245 2024-04-29 20:05:25.000000 blendr_cli-0.1.2/blendr/task_manager/listen.py
-drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 06:44:49.184632 blendr_cli-0.1.2/blendr_cli.egg-info/
--rw-r--r--   0 stefanshiloh   (501) staff       (20)     3079 2024-04-30 06:44:49.000000 blendr_cli-0.1.2/blendr_cli.egg-info/PKG-INFO
--rw-r--r--   0 stefanshiloh   (501) staff       (20)      506 2024-04-30 06:44:49.000000 blendr_cli-0.1.2/blendr_cli.egg-info/SOURCES.txt
--rw-r--r--   0 stefanshiloh   (501) staff       (20)        1 2024-04-30 06:44:49.000000 blendr_cli-0.1.2/blendr_cli.egg-info/dependency_links.txt
--rw-r--r--   0 stefanshiloh   (501) staff       (20)       43 2024-04-30 06:44:49.000000 blendr_cli-0.1.2/blendr_cli.egg-info/entry_points.txt
--rw-r--r--   0 stefanshiloh   (501) staff       (20)       46 2024-04-30 06:44:49.000000 blendr_cli-0.1.2/blendr_cli.egg-info/requires.txt
--rw-r--r--   0 stefanshiloh   (501) staff       (20)        7 2024-04-30 06:44:49.000000 blendr_cli-0.1.2/blendr_cli.egg-info/top_level.txt
--rw-r--r--   0 stefanshiloh   (501) staff       (20)       38 2024-04-30 06:44:49.185125 blendr_cli-0.1.2/setup.cfg
--rw-r--r--   0 stefanshiloh   (501) staff       (20)      797 2024-04-30 06:44:43.000000 blendr_cli-0.1.2/setup.py
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 15:23:08.015129 blendr_cli-0.1.3/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)     3134 2024-04-30 15:23:08.014868 blendr_cli-0.1.3/PKG-INFO
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)     2677 2024-04-29 20:20:22.000000 blendr_cli-0.1.3/README.md
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 15:23:08.010820 blendr_cli-0.1.3/blendr/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-20 16:49:51.000000 blendr_cli-0.1.3/blendr/__init__.py
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 15:23:08.011414 blendr_cli-0.1.3/blendr/auth/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-21 17:20:43.000000 blendr_cli-0.1.3/blendr/auth/__init__.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)     1923 2024-04-30 07:06:02.000000 blendr_cli-0.1.3/blendr/auth/authenticate.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)     1917 2024-04-30 07:02:44.000000 blendr_cli-0.1.3/blendr/cli.py
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 15:23:08.012276 blendr_cli-0.1.3/blendr/config/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-21 17:20:41.000000 blendr_cli-0.1.3/blendr/config/__init__.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)      158 2024-04-30 13:58:05.000000 blendr_cli-0.1.3/blendr/config/settings.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)     6119 2024-04-30 14:25:22.000000 blendr_cli-0.1.3/blendr/config/setup.py
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 15:23:08.012787 blendr_cli-0.1.3/blendr/gpu_manager/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-29 22:27:38.000000 blendr_cli-0.1.3/blendr/gpu_manager/__init__.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)      190 2024-04-29 20:05:17.000000 blendr_cli-0.1.3/blendr/gpu_manager/detect.py
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 15:23:08.013270 blendr_cli-0.1.3/blendr/task_manager/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-29 22:27:33.000000 blendr_cli-0.1.3/blendr/task_manager/__init__.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)     2245 2024-04-29 20:05:25.000000 blendr_cli-0.1.3/blendr/task_manager/listen.py
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 15:23:08.014600 blendr_cli-0.1.3/blendr_cli.egg-info/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)     3134 2024-04-30 15:23:07.000000 blendr_cli-0.1.3/blendr_cli.egg-info/PKG-INFO
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)      506 2024-04-30 15:23:07.000000 blendr_cli-0.1.3/blendr_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        1 2024-04-30 15:23:07.000000 blendr_cli-0.1.3/blendr_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)       43 2024-04-30 15:23:07.000000 blendr_cli-0.1.3/blendr_cli.egg-info/entry_points.txt
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)       71 2024-04-30 15:23:07.000000 blendr_cli-0.1.3/blendr_cli.egg-info/requires.txt
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        7 2024-04-30 15:23:07.000000 blendr_cli-0.1.3/blendr_cli.egg-info/top_level.txt
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)       38 2024-04-30 15:23:08.015175 blendr_cli-0.1.3/setup.cfg
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)      844 2024-04-30 15:22:52.000000 blendr_cli-0.1.3/setup.py
```

### Comparing `blendr_cli-0.1.2/PKG-INFO` & `blendr_cli-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: blendr-cli
-Version: 0.1.2
+Version: 0.1.3
 Summary: Blendr CLI tool for GPU Lending
 Home-page: https://www.blendr.network
 Author: Blendr Network
 Author-email: tech@blendr.network
 License: MIT
 Keywords: blendr cli
 Description-Content-Type: text/markdown
 Requires-Dist: click
 Requires-Dist: requests
 Requires-Dist: colorama
 Requires-Dist: GPUtil
 Requires-Dist: psutil
 Requires-Dist: keyring
+Requires-Dist: speedtest-cli
+Requires-Dist: py-cpuinfo
 
 # Blendr CLI
 
 Blendr CLI is a command-line interface designed to help users lend their GPU resources for computational tasks on the Blendr platform. This tool allows for easy setup, management, and monitoring of GPU resources from your terminal.
 
 ## Features
```

### Comparing `blendr_cli-0.1.2/README.md` & `blendr_cli-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `blendr_cli-0.1.2/blendr/auth/authenticate.py` & `blendr_cli-0.1.3/blendr/auth/authenticate.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,18 +6,15 @@
 import keyring
 
 
 def login():
     """Handles user login with server validation."""
     
       # Request session ID from server
-    print(f'{SERVER_URL}/api/generate/session-id')
     response = requests.post(f'{SERVER_URL}/api/generate/session-id', json={'deviceID': 'macOS'})
-    print(response)
-    print(response.json())
     session_id = response.json().get('sessionId')
 
     # Open browser for user login and confirmation
     print("Opening browser for user login and confirmation...")
     print(f'URL: {CLIENT_URL}/verify?sessionId={session_id}')
     webbrowser.open(f'{CLIENT_URL}/verify?sessionId={session_id}')
```

### Comparing `blendr_cli-0.1.2/blendr/cli.py` & `blendr_cli-0.1.3/blendr/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,32 +11,34 @@
 # Define ASCII Art
 BLENDR_ASCII_ART = r"""
 __________.__                     .___       
 \______   \  |   ____   ____    __| _/______ 
  |    |  _/  | _/ __ \ /    \  / __ |\_  __ \
  |    |   \  |_\  ___/|   |  \/ /_/ | |  | \/
  |______  /____/\___  >___|  /\____ | |__|   
-        \/          \/     \/      \/        ƒ
+        \/          \/     \/      \/      
 """
 
 
 
 @click.group()
 def cli():
     """
 ======================
 BLENDR CLI
 ======================
-The Blender CLI is a command-line interface that connects users with the Blendr platform. It allows users to lend their GPU for computational tasks. By running the CLI, users can log in to the system, perform initial setup, check for available GPUs, and listen for incoming tasks. The CLI provides a convenient way for users to interact with the Blendr platform and contribute their GPU resources.
+The Blender CLI is a command-line interface that connects users with the Blendr platform. It allows users to lend their GPU for computational tasks.
+By running the CLI, users can log in to the system, perform initial setup, check for available GPUs,  nd listen for incoming tasks. 
+The CLI provides a convenient way for users to interact with the Blendr platform and contribute their GPU resources.
     """
     pass
 
 @cli.command()
 def info():
-    """Log in to the system using credentials."""
+    """Blendr Info."""
     click.echo(Fore.BLUE + Style.BRIGHT + BLENDR_ASCII_ART + Style.RESET_ALL)
     click.echo(Fore.YELLOW + "Welcome to Blendr!")
     click.echo(Fore.CYAN+"The Blender CLI is a command-line interface that connects users with the Blendr platform.")
     # click.echo(Style.RESET_ALL)
 
 @cli.command()
 def login():
@@ -57,11 +59,12 @@
 def listentask():
     """Listen to incoming tasks"""
     listen.listen()
 
 
 
 def main():
+    click.echo(Fore.BLUE + Style.BRIGHT + BLENDR_ASCII_ART + Style.RESET_ALL)  
     cli()
 
 if __name__ == "__main__":
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `blendr_cli-0.1.2/blendr/task_manager/listen.py` & `blendr_cli-0.1.3/blendr/task_manager/listen.py`

 * *Files identical despite different names*

### Comparing `blendr_cli-0.1.2/blendr_cli.egg-info/PKG-INFO` & `blendr_cli-0.1.3/blendr_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: blendr-cli
-Version: 0.1.2
+Version: 0.1.3
 Summary: Blendr CLI tool for GPU Lending
 Home-page: https://www.blendr.network
 Author: Blendr Network
 Author-email: tech@blendr.network
 License: MIT
 Keywords: blendr cli
 Description-Content-Type: text/markdown
 Requires-Dist: click
 Requires-Dist: requests
 Requires-Dist: colorama
 Requires-Dist: GPUtil
 Requires-Dist: psutil
 Requires-Dist: keyring
+Requires-Dist: speedtest-cli
+Requires-Dist: py-cpuinfo
 
 # Blendr CLI
 
 Blendr CLI is a command-line interface designed to help users lend their GPU resources for computational tasks on the Blendr platform. This tool allows for easy setup, management, and monitoring of GPU resources from your terminal.
 
 ## Features
```

### Comparing `blendr_cli-0.1.2/setup.py` & `blendr_cli-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 import os
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='blendr-cli',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     install_requires=[
         'click',      
         'requests',  
         'colorama',
         'GPUtil',
         'psutil',
-        'keyring'
+        'keyring',
+        'speedtest-cli',
+        'py-cpuinfo'
     ],
     entry_points={
         'console_scripts': [
             'blendr=blendr.cli:main'
         ]
     },
     author='Blendr Network',
```

