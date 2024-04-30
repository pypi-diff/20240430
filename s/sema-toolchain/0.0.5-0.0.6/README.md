# Comparing `tmp/sema_toolchain-0.0.5.tar.gz` & `tmp/sema_toolchain-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sema_toolchain-0.0.5.tar", last modified: Sun Apr 28 11:49:10 2024, max compression
+gzip compressed data, was "sema_toolchain-0.0.6.tar", last modified: Tue Apr 30 11:32:52 2024, max compression
```

## Comparing `sema_toolchain-0.0.5.tar` & `sema_toolchain-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 manon     (1000) manon     (1000)        0 2024-04-28 11:49:10.300684 sema_toolchain-0.0.5/
--rw-rw-r--   0 manon     (1000) manon     (1000)     1332 2024-04-16 10:03:35.000000 sema_toolchain-0.0.5/LICENSE
--rw-r--r--   0 manon     (1000) manon     (1000)    17811 2024-04-28 11:49:10.300684 sema_toolchain-0.0.5/PKG-INFO
--rw-rw-r--   0 manon     (1000) manon     (1000)    14573 2024-04-28 10:41:44.000000 sema_toolchain-0.0.5/README.md
--rw-rw-r--   0 manon     (1000) manon     (1000)     1542 2024-04-28 11:49:03.000000 sema_toolchain-0.0.5/pyproject.toml
-drwxrwxr-x   0 manon     (1000) manon     (1000)        0 2024-04-28 11:49:10.300684 sema_toolchain-0.0.5/sema_toolchain.egg-info/
--rw-r--r--   0 manon     (1000) manon     (1000)    17811 2024-04-28 11:49:10.000000 sema_toolchain-0.0.5/sema_toolchain.egg-info/PKG-INFO
--rw-rw-r--   0 manon     (1000) manon     (1000)      221 2024-04-28 11:49:10.000000 sema_toolchain-0.0.5/sema_toolchain.egg-info/SOURCES.txt
--rw-rw-r--   0 manon     (1000) manon     (1000)        1 2024-04-28 11:49:10.000000 sema_toolchain-0.0.5/sema_toolchain.egg-info/dependency_links.txt
--rw-rw-r--   0 manon     (1000) manon     (1000)      520 2024-04-28 11:49:10.000000 sema_toolchain-0.0.5/sema_toolchain.egg-info/requires.txt
--rw-rw-r--   0 manon     (1000) manon     (1000)       39 2024-04-28 11:49:10.000000 sema_toolchain-0.0.5/sema_toolchain.egg-info/top_level.txt
--rw-rw-r--   0 manon     (1000) manon     (1000)       38 2024-04-28 11:49:10.300684 sema_toolchain-0.0.5/setup.cfg
+drwxrwxr-x   0 manon     (1000) manon     (1000)        0 2024-04-30 11:32:52.022475 sema_toolchain-0.0.6/
+-rw-rw-r--   0 manon     (1000) manon     (1000)     1332 2024-04-16 10:03:35.000000 sema_toolchain-0.0.6/LICENSE
+-rw-r--r--   0 manon     (1000) manon     (1000)    18056 2024-04-30 11:32:52.022475 sema_toolchain-0.0.6/PKG-INFO
+-rw-rw-r--   0 manon     (1000) manon     (1000)    14818 2024-04-30 11:31:59.000000 sema_toolchain-0.0.6/README.md
+-rw-rw-r--   0 manon     (1000) manon     (1000)     1542 2024-04-30 11:32:46.000000 sema_toolchain-0.0.6/pyproject.toml
+drwxrwxr-x   0 manon     (1000) manon     (1000)        0 2024-04-30 11:32:52.022475 sema_toolchain-0.0.6/sema_toolchain.egg-info/
+-rw-r--r--   0 manon     (1000) manon     (1000)    18056 2024-04-30 11:32:52.000000 sema_toolchain-0.0.6/sema_toolchain.egg-info/PKG-INFO
+-rw-rw-r--   0 manon     (1000) manon     (1000)      221 2024-04-30 11:32:52.000000 sema_toolchain-0.0.6/sema_toolchain.egg-info/SOURCES.txt
+-rw-rw-r--   0 manon     (1000) manon     (1000)        1 2024-04-30 11:32:52.000000 sema_toolchain-0.0.6/sema_toolchain.egg-info/dependency_links.txt
+-rw-rw-r--   0 manon     (1000) manon     (1000)      520 2024-04-30 11:32:52.000000 sema_toolchain-0.0.6/sema_toolchain.egg-info/requires.txt
+-rw-rw-r--   0 manon     (1000) manon     (1000)       39 2024-04-30 11:32:52.000000 sema_toolchain-0.0.6/sema_toolchain.egg-info/top_level.txt
+-rw-rw-r--   0 manon     (1000) manon     (1000)       38 2024-04-30 11:32:52.022475 sema_toolchain-0.0.6/setup.cfg
```

### Comparing `sema_toolchain-0.0.5/LICENSE` & `sema_toolchain-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sema_toolchain-0.0.5/PKG-INFO` & `sema_toolchain-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sema_toolchain
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python symbolic execution package
 Author-email: Manon-Oreins <manon.oreins@gmail.com>
 License: BSD 2-Clause License
         
         Copyright (c) 2022, UCL-Cybersecurity team
         All rights reserved.
         
@@ -121,80 +121,88 @@
 ====
 <a name="arch"></a>
 
 ### Toolchain architecture
 <a name="arch_std"></a>
 
 
-##### Main depencies:
+#### Main depencies:
 
     * Python 3.8 (angr)
 
-    * KVM/QEMU
-
     * Docker, docker buildx, docker compose
 
-##### Interesting links
+    * radare2
+
+#### Using Pypi sema-toolchain package
+
+If you wish to install the toolchain python dependencies on your system, use :
+
+```bash
+pip install sema-toolchain
+```
+
+#### Pypy3 usage
+
+By default, pypy3 can be used to launch experiments inside the SCDG's docker container. If you wish to use it outside the container, make sure to install pypy3 :
+
+```bash
+sudo add-apt-repository ppa:pypy/ppa
+sudo apt update
+sudo apt install pypy3
+```
+
+Then install the dependecies on pypy3 :
+
+```bash
+pypy3 -m pip install -r /sema_scdg/requirements_pypy.txt
+```
+
+#### Interesting links
 
 * https://angr.io/
 
 * https://bazaar.abuse.ch/
 
 * https://docs.docker.com/engine/install/ubuntu/
 
 :page_with_curl: Installation
 ====
 <a name="install"></a>
 
-Tested on Ubuntu 20.
+Tested on Ubuntu 20.04
 
 **Recommanded installation:**
 
 ```bash
 git clone https://github.com/Manon-Oreins/SEMA-ToolChain.git;
 
 # Full installation (ubuntu)
 make build-toolchain;
 ```
 
 If you only need the SCDG part of the toolchain you can use :
 ```bash
 make pull-scdg
 ```
+To pull the docker image directly from dockerHub
 
-Or visit `https://hub.docker.com/repository/docker/manonoreins/sema-scdg/tags` to pull the image
+Or visit `https://hub.docker.com/repository/docker/manonoreins/sema-scdg/tags`
 
 ## Installation details (optional)
 
-#### Pip
-
-To run this SCDG extractor you first need to install pip.
-
-##### Debian (and Debian-based)
-To install pip on debian-based systems:
-```bash
-sudo apt update;
-sudo apt-get install python3-pip xterm;
-```
-
-##### Arch (and Arch-based)
-To install pip on arch-based systems:
-```bash
-sudo pacman -Sy python-pip xterm;
-```
-
-##### For extracting database
+#### For extracting database
 
 ```bash
 cd databases/Binaries; bash extract_deploy_db.sh
 ```
 
 Password for archive is "infected". Warning : it contains real samples of malwares.
 
-##### For code cleaning
+#### For code cleaning
 
 ```bash
 #To zip back the test database
 cd databases/Binaries; bash compress_db.sh
 ```
 
 :page_with_curl: `SEMA - ToolChain`
```

### Comparing `sema_toolchain-0.0.5/README.md` & `sema_toolchain-0.0.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -34,80 +34,88 @@
 ====
 <a name="arch"></a>
 
 ### Toolchain architecture
 <a name="arch_std"></a>
 
 
-##### Main depencies:
+#### Main depencies:
 
     * Python 3.8 (angr)
 
-    * KVM/QEMU
-
     * Docker, docker buildx, docker compose
 
-##### Interesting links
+    * radare2
+
+#### Using Pypi sema-toolchain package
+
+If you wish to install the toolchain python dependencies on your system, use :
+
+```bash
+pip install sema-toolchain
+```
+
+#### Pypy3 usage
+
+By default, pypy3 can be used to launch experiments inside the SCDG's docker container. If you wish to use it outside the container, make sure to install pypy3 :
+
+```bash
+sudo add-apt-repository ppa:pypy/ppa
+sudo apt update
+sudo apt install pypy3
+```
+
+Then install the dependecies on pypy3 :
+
+```bash
+pypy3 -m pip install -r /sema_scdg/requirements_pypy.txt
+```
+
+#### Interesting links
 
 * https://angr.io/
 
 * https://bazaar.abuse.ch/
 
 * https://docs.docker.com/engine/install/ubuntu/
 
 :page_with_curl: Installation
 ====
 <a name="install"></a>
 
-Tested on Ubuntu 20.
+Tested on Ubuntu 20.04
 
 **Recommanded installation:**
 
 ```bash
 git clone https://github.com/Manon-Oreins/SEMA-ToolChain.git;
 
 # Full installation (ubuntu)
 make build-toolchain;
 ```
 
 If you only need the SCDG part of the toolchain you can use :
 ```bash
 make pull-scdg
 ```
+To pull the docker image directly from dockerHub
 
-Or visit `https://hub.docker.com/repository/docker/manonoreins/sema-scdg/tags` to pull the image
+Or visit `https://hub.docker.com/repository/docker/manonoreins/sema-scdg/tags`
 
 ## Installation details (optional)
 
-#### Pip
-
-To run this SCDG extractor you first need to install pip.
-
-##### Debian (and Debian-based)
-To install pip on debian-based systems:
-```bash
-sudo apt update;
-sudo apt-get install python3-pip xterm;
-```
-
-##### Arch (and Arch-based)
-To install pip on arch-based systems:
-```bash
-sudo pacman -Sy python-pip xterm;
-```
-
-##### For extracting database
+#### For extracting database
 
 ```bash
 cd databases/Binaries; bash extract_deploy_db.sh
 ```
 
 Password for archive is "infected". Warning : it contains real samples of malwares.
 
-##### For code cleaning
+#### For code cleaning
 
 ```bash
 #To zip back the test database
 cd databases/Binaries; bash compress_db.sh
 ```
 
 :page_with_curl: `SEMA - ToolChain`
```

### Comparing `sema_toolchain-0.0.5/pyproject.toml` & `sema_toolchain-0.0.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 py-modules = ["sema_scdg", "sema_web_app", "sema_classifier"]
 
 [project]
 name = "sema_toolchain"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Manon-Oreins", email="manon.oreins@gmail.com" },
 ]
 description = "Python symbolic execution package"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `sema_toolchain-0.0.5/sema_toolchain.egg-info/PKG-INFO` & `sema_toolchain-0.0.6/sema_toolchain.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sema_toolchain
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python symbolic execution package
 Author-email: Manon-Oreins <manon.oreins@gmail.com>
 License: BSD 2-Clause License
         
         Copyright (c) 2022, UCL-Cybersecurity team
         All rights reserved.
         
@@ -121,80 +121,88 @@
 ====
 <a name="arch"></a>
 
 ### Toolchain architecture
 <a name="arch_std"></a>
 
 
-##### Main depencies:
+#### Main depencies:
 
     * Python 3.8 (angr)
 
-    * KVM/QEMU
-
     * Docker, docker buildx, docker compose
 
-##### Interesting links
+    * radare2
+
+#### Using Pypi sema-toolchain package
+
+If you wish to install the toolchain python dependencies on your system, use :
+
+```bash
+pip install sema-toolchain
+```
+
+#### Pypy3 usage
+
+By default, pypy3 can be used to launch experiments inside the SCDG's docker container. If you wish to use it outside the container, make sure to install pypy3 :
+
+```bash
+sudo add-apt-repository ppa:pypy/ppa
+sudo apt update
+sudo apt install pypy3
+```
+
+Then install the dependecies on pypy3 :
+
+```bash
+pypy3 -m pip install -r /sema_scdg/requirements_pypy.txt
+```
+
+#### Interesting links
 
 * https://angr.io/
 
 * https://bazaar.abuse.ch/
 
 * https://docs.docker.com/engine/install/ubuntu/
 
 :page_with_curl: Installation
 ====
 <a name="install"></a>
 
-Tested on Ubuntu 20.
+Tested on Ubuntu 20.04
 
 **Recommanded installation:**
 
 ```bash
 git clone https://github.com/Manon-Oreins/SEMA-ToolChain.git;
 
 # Full installation (ubuntu)
 make build-toolchain;
 ```
 
 If you only need the SCDG part of the toolchain you can use :
 ```bash
 make pull-scdg
 ```
+To pull the docker image directly from dockerHub
 
-Or visit `https://hub.docker.com/repository/docker/manonoreins/sema-scdg/tags` to pull the image
+Or visit `https://hub.docker.com/repository/docker/manonoreins/sema-scdg/tags`
 
 ## Installation details (optional)
 
-#### Pip
-
-To run this SCDG extractor you first need to install pip.
-
-##### Debian (and Debian-based)
-To install pip on debian-based systems:
-```bash
-sudo apt update;
-sudo apt-get install python3-pip xterm;
-```
-
-##### Arch (and Arch-based)
-To install pip on arch-based systems:
-```bash
-sudo pacman -Sy python-pip xterm;
-```
-
-##### For extracting database
+#### For extracting database
 
 ```bash
 cd databases/Binaries; bash extract_deploy_db.sh
 ```
 
 Password for archive is "infected". Warning : it contains real samples of malwares.
 
-##### For code cleaning
+#### For code cleaning
 
 ```bash
 #To zip back the test database
 cd databases/Binaries; bash compress_db.sh
 ```
 
 :page_with_curl: `SEMA - ToolChain`
```

### Comparing `sema_toolchain-0.0.5/sema_toolchain.egg-info/requires.txt` & `sema_toolchain-0.0.6/sema_toolchain.egg-info/requires.txt`

 * *Files identical despite different names*

