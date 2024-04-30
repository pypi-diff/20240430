# Comparing `tmp/iss-libs-0.0.7.tar.gz` & `tmp/iss_libs-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iss-libs-0.0.7.tar", last modified: Tue Jan 30 05:54:56 2024, max compression
+gzip compressed data, was "iss_libs-0.0.8.tar", last modified: Tue Apr 30 02:57:18 2024, max compression
```

## Comparing `iss-libs-0.0.7.tar` & `iss_libs-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 timecard  (1000) timecard  (1000)        0 2024-01-30 05:54:56.196190 iss-libs-0.0.7/
--rw-rw-r--   0 timecard  (1000) timecard  (1000)     1084 2024-01-30 04:06:17.000000 iss-libs-0.0.7/LICENSE
--rw-rw-r--   0 timecard  (1000) timecard  (1000)     1167 2024-01-30 05:54:56.196190 iss-libs-0.0.7/PKG-INFO
--rw-rw-r--   0 timecard  (1000) timecard  (1000)      605 2024-01-30 04:06:17.000000 iss-libs-0.0.7/README.md
-drwxrwxr-x   0 timecard  (1000) timecard  (1000)        0 2024-01-30 05:54:56.196190 iss-libs-0.0.7/iss_libs.egg-info/
--rw-rw-r--   0 timecard  (1000) timecard  (1000)     1167 2024-01-30 05:54:56.000000 iss-libs-0.0.7/iss_libs.egg-info/PKG-INFO
--rw-rw-r--   0 timecard  (1000) timecard  (1000)      195 2024-01-30 05:54:56.000000 iss-libs-0.0.7/iss_libs.egg-info/SOURCES.txt
--rw-rw-r--   0 timecard  (1000) timecard  (1000)        1 2024-01-30 05:54:56.000000 iss-libs-0.0.7/iss_libs.egg-info/dependency_links.txt
--rw-rw-r--   0 timecard  (1000) timecard  (1000)      268 2024-01-30 05:54:56.000000 iss-libs-0.0.7/iss_libs.egg-info/requires.txt
--rw-rw-r--   0 timecard  (1000) timecard  (1000)        1 2024-01-30 05:54:56.000000 iss-libs-0.0.7/iss_libs.egg-info/top_level.txt
--rw-rw-r--   0 timecard  (1000) timecard  (1000)       79 2024-01-30 05:54:56.196190 iss-libs-0.0.7/setup.cfg
--rw-rw-r--   0 timecard  (1000) timecard  (1000)     2209 2024-01-30 04:12:47.000000 iss-libs-0.0.7/setup.py
+drwxrwxr-x   0 timecard  (1000) timecard  (1000)        0 2024-04-30 02:57:18.768010 iss_libs-0.0.8/
+-rw-rw-r--   0 timecard  (1000) timecard  (1000)     1084 2024-04-30 02:40:01.000000 iss_libs-0.0.8/LICENSE
+-rw-r--r--   0 timecard  (1000) timecard  (1000)     1841 2024-04-30 02:57:18.768010 iss_libs-0.0.8/PKG-INFO
+-rw-rw-r--   0 timecard  (1000) timecard  (1000)      605 2024-04-30 02:40:01.000000 iss_libs-0.0.8/README.md
+drwxrwxr-x   0 timecard  (1000) timecard  (1000)        0 2024-04-30 02:57:18.768010 iss_libs-0.0.8/iss_libs.egg-info/
+-rw-r--r--   0 timecard  (1000) timecard  (1000)     1841 2024-04-30 02:57:18.000000 iss_libs-0.0.8/iss_libs.egg-info/PKG-INFO
+-rw-rw-r--   0 timecard  (1000) timecard  (1000)      195 2024-04-30 02:57:18.000000 iss_libs-0.0.8/iss_libs.egg-info/SOURCES.txt
+-rw-rw-r--   0 timecard  (1000) timecard  (1000)        1 2024-04-30 02:57:18.000000 iss_libs-0.0.8/iss_libs.egg-info/dependency_links.txt
+-rw-rw-r--   0 timecard  (1000) timecard  (1000)      293 2024-04-30 02:57:18.000000 iss_libs-0.0.8/iss_libs.egg-info/requires.txt
+-rw-rw-r--   0 timecard  (1000) timecard  (1000)        1 2024-04-30 02:57:18.000000 iss_libs-0.0.8/iss_libs.egg-info/top_level.txt
+-rw-rw-r--   0 timecard  (1000) timecard  (1000)       79 2024-04-30 02:57:18.769010 iss_libs-0.0.8/setup.cfg
+-rw-rw-r--   0 timecard  (1000) timecard  (1000)     2359 2024-04-30 02:53:36.000000 iss_libs-0.0.8/setup.py
```

### Comparing `iss-libs-0.0.7/LICENSE` & `iss_libs-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `iss-libs-0.0.7/README.md` & `iss_libs-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `iss-libs-0.0.7/setup.py` & `iss_libs-0.0.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='iss-libs',  # How you named your package folder (MyLib)
-    version='0.0.7',  # Start with a small number and increase it with every change you make
+    version='0.0.8',  # Start with a small number and increase it with every change you make
     author='Somsak Binyaranee',  # Type in your name
     author_email='poster.som@gmail.com',  # Type in your E-Mail
     description='',  # Give a short description about your library
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/postersom/iss-libs',  # Provide either the link to your github or to your website
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
@@ -18,20 +18,23 @@
     install_requires=['connexion==2.14.2',
                       'Flask==2.2.5',
                       'Flask-SocketIO',
                       'marshmallow',
                       'marshmallow_sqlalchemy',
                       'matplotlib',
                       'minimalmodbus',
+                      'ntplib',
                       'paramiko',
                       'prettytable',
                       'psutil',
+                      'pyModbusTCP'
                       'pyserial',
                       'python-dotenv',
                       'python-gitlab',
+                      'PyVISA',
                       'redis',
                       'robotframework',
                       'robotframework-sshlibrary',
                       'six',
                       'sqlalchemy',
                       'swagger-ui-bundle==0.0.9',
                       'xmltodict'],
@@ -40,9 +43,10 @@
         # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Intended Audience :: Developers',  # Define that your audience are developers
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',  # Again, pick a license
         'Programming Language :: Python :: 3.9',  # Specify which pyhton versions that you want to support
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
 )
```

