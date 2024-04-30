# Comparing `tmp/zato_apitest-24.1.30.tar.gz` & `tmp/zato_apitest-24.1.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zato_apitest-24.1.30.tar", last modified: Mon Apr 29 13:16:48 2024, max compression
+gzip compressed data, was "zato_apitest-24.1.31.tar", last modified: Mon Apr 29 14:34:33 2024, max compression
```

## Comparing `zato_apitest-24.1.30.tar` & `zato_apitest-24.1.31.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 13:16:48.980788 zato_apitest-24.1.30/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)    29450 2024-04-28 07:49:48.000000 zato_apitest-24.1.30/LICENSE.txt
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)       24 2019-06-24 21:01:23.000000 zato_apitest-24.1.30/MANIFEST.in
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     2393 2024-04-29 13:16:48.980788 zato_apitest-24.1.30/PKG-INFO
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)       64 2021-01-13 02:20:20.000000 zato_apitest-24.1.30/README.md
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)      375 2024-03-12 11:30:46.000000 zato_apitest-24.1.30/requirements.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)       38 2024-04-29 13:16:48.980788 zato_apitest-24.1.30/setup.cfg
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)     2663 2024-04-29 13:16:24.000000 zato_apitest-24.1.30/setup.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 13:16:48.976788 zato_apitest-24.1.30/src/
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 13:16:48.980788 zato_apitest-24.1.30/src/zato/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)      211 2024-04-28 07:50:38.000000 zato_apitest-24.1.30/src/zato/__init__.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 13:16:48.980788 zato_apitest-24.1.30/src/zato/apitest/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     1800 2024-04-28 07:51:00.000000 zato_apitest-24.1.30/src/zato/apitest/__init__.py
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     4482 2024-04-28 09:17:32.000000 zato_apitest-24.1.30/src/zato/apitest/cli.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 13:16:48.980788 zato_apitest-24.1.30/src/zato/apitest/console/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)      210 2024-04-28 07:50:47.000000 zato_apitest-24.1.30/src/zato/apitest/console/apitest
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     6434 2024-04-29 09:17:00.000000 zato_apitest-24.1.30/src/zato/apitest/init.py
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     3116 2024-04-28 13:16:28.000000 zato_apitest-24.1.30/src/zato/apitest/run.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 13:16:48.980788 zato_apitest-24.1.30/src/zato/apitest/steps/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)      156 2024-04-28 07:50:55.000000 zato_apitest-24.1.30/src/zato/apitest/steps/__init__.py
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)    48533 2024-04-29 13:13:57.000000 zato_apitest-24.1.30/src/zato/apitest/steps/common.py
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)    22517 2024-04-28 07:50:58.000000 zato_apitest-24.1.30/src/zato/apitest/steps/json.py
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)     7325 2024-04-28 07:50:53.000000 zato_apitest-24.1.30/src/zato/apitest/typing_.py
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)    14680 2024-04-29 09:23:45.000000 zato_apitest-24.1.30/src/zato/apitest/util.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 13:16:48.980788 zato_apitest-24.1.30/src/zato_apitest.egg-info/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     2393 2024-04-29 13:16:48.000000 zato_apitest-24.1.30/src/zato_apitest.egg-info/PKG-INFO
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)      654 2024-04-29 13:16:48.000000 zato_apitest-24.1.30/src/zato_apitest.egg-info/SOURCES.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        1 2024-04-29 13:16:48.000000 zato_apitest-24.1.30/src/zato_apitest.egg-info/dependency_links.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        5 2024-04-29 13:16:48.000000 zato_apitest-24.1.30/src/zato_apitest.egg-info/namespace_packages.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        1 2024-04-29 13:16:46.000000 zato_apitest-24.1.30/src/zato_apitest.egg-info/not-zip-safe
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)      356 2024-04-29 13:16:48.000000 zato_apitest-24.1.30/src/zato_apitest.egg-info/requires.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        5 2024-04-29 13:16:48.000000 zato_apitest-24.1.30/src/zato_apitest.egg-info/top_level.txt
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 14:34:33.845161 zato_apitest-24.1.31/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)    29450 2024-04-28 07:49:48.000000 zato_apitest-24.1.31/LICENSE.txt
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)       24 2019-06-24 21:01:23.000000 zato_apitest-24.1.31/MANIFEST.in
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     2341 2024-04-29 14:34:33.845161 zato_apitest-24.1.31/PKG-INFO
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)       64 2021-01-13 02:20:20.000000 zato_apitest-24.1.31/README.md
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)      375 2024-03-12 11:30:46.000000 zato_apitest-24.1.31/requirements.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)       38 2024-04-29 14:34:33.845161 zato_apitest-24.1.31/setup.cfg
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)     2612 2024-04-29 14:34:00.000000 zato_apitest-24.1.31/setup.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 14:34:33.841161 zato_apitest-24.1.31/src/
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 14:34:33.845161 zato_apitest-24.1.31/src/zato/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)      211 2024-04-28 07:50:38.000000 zato_apitest-24.1.31/src/zato/__init__.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 14:34:33.845161 zato_apitest-24.1.31/src/zato/apitest/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     1800 2024-04-28 07:51:00.000000 zato_apitest-24.1.31/src/zato/apitest/__init__.py
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     4482 2024-04-28 09:17:32.000000 zato_apitest-24.1.31/src/zato/apitest/cli.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 14:34:33.845161 zato_apitest-24.1.31/src/zato/apitest/console/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)      210 2024-04-28 07:50:47.000000 zato_apitest-24.1.31/src/zato/apitest/console/apitest
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     6434 2024-04-29 09:17:00.000000 zato_apitest-24.1.31/src/zato/apitest/init.py
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     3116 2024-04-28 13:16:28.000000 zato_apitest-24.1.31/src/zato/apitest/run.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 14:34:33.845161 zato_apitest-24.1.31/src/zato/apitest/steps/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)      156 2024-04-28 07:50:55.000000 zato_apitest-24.1.31/src/zato/apitest/steps/__init__.py
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)    48533 2024-04-29 13:13:57.000000 zato_apitest-24.1.31/src/zato/apitest/steps/common.py
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)    22517 2024-04-28 07:50:58.000000 zato_apitest-24.1.31/src/zato/apitest/steps/json.py
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)     7325 2024-04-28 07:50:53.000000 zato_apitest-24.1.31/src/zato/apitest/typing_.py
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)    14680 2024-04-29 09:23:45.000000 zato_apitest-24.1.31/src/zato/apitest/util.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 14:34:33.845161 zato_apitest-24.1.31/src/zato_apitest.egg-info/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     2341 2024-04-29 14:34:33.000000 zato_apitest-24.1.31/src/zato_apitest.egg-info/PKG-INFO
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)      654 2024-04-29 14:34:33.000000 zato_apitest-24.1.31/src/zato_apitest.egg-info/SOURCES.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        1 2024-04-29 14:34:33.000000 zato_apitest-24.1.31/src/zato_apitest.egg-info/dependency_links.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        5 2024-04-29 14:34:33.000000 zato_apitest-24.1.31/src/zato_apitest.egg-info/namespace_packages.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        1 2024-04-29 14:34:31.000000 zato_apitest-24.1.31/src/zato_apitest.egg-info/not-zip-safe
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)      356 2024-04-29 14:34:33.000000 zato_apitest-24.1.31/src/zato_apitest.egg-info/requires.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        5 2024-04-29 14:34:33.000000 zato_apitest-24.1.31/src/zato_apitest.egg-info/top_level.txt
```

### Comparing `zato_apitest-24.1.30/LICENSE.txt` & `zato_apitest-24.1.31/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.30/PKG-INFO` & `zato_apitest-24.1.31/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: zato-apitest
-Version: 24.1.30
+Version: 24.1.31
 Summary: API Testing for Humans. Write API tests in pure English, without any programming needed.
 Home-page: https://zato.io
 Author: Zato Source s.r.o.
 Author-email: info@zato.io
-License: Proprietary
+License: SSPL 1.0
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Other Audience
-Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Communications
```

#### html2text {}

```diff
@@ -1,23 +1,22 @@
-Metadata-Version: 2.1 Name: zato-apitest Version: 24.1.30 Summary: API Testing
+Metadata-Version: 2.1 Name: zato-apitest Version: 24.1.31 Summary: API Testing
 for Humans. Write API tests in pure English, without any programming needed.
 Home-page: https://zato.io Author: Zato Source s.r.o. Author-email:
-info@zato.io License: Proprietary Platform: OS Independent Classifier:
-Development Status :: 5 - Production/Stable Classifier: Environment :: Console
-Classifier: Environment :: Web Environment Classifier: Intended Audience ::
-Developers Classifier: Intended Audience :: Information Technology Classifier:
-Intended Audience :: Other Audience Classifier: License :: Other/Proprietary
-License Classifier: Natural Language :: English Classifier: Operating System ::
-OS Independent Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 2 Classifier: Programming Language :: Python
-:: 3 Classifier: Intended Audience :: Developers Classifier: Topic ::
-Communications Classifier: Topic :: Education :: Testing Classifier: Topic ::
-Internet Classifier: Topic :: Internet :: Proxy Servers Classifier: Topic ::
-Internet :: WWW/HTTP Classifier: Topic :: Security Classifier: Topic ::
-Software Development :: Quality Assurance Classifier: Topic :: Software
+info@zato.io License: SSPL 1.0 Platform: OS Independent Classifier: Development
+Status :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
+Environment :: Web Environment Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology Classifier: Intended
+Audience :: Other Audience Classifier: Natural Language :: English Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2 Classifier: Programming
+Language :: Python :: 3 Classifier: Intended Audience :: Developers Classifier:
+Topic :: Communications Classifier: Topic :: Education :: Testing Classifier:
+Topic :: Internet Classifier: Topic :: Internet :: Proxy Servers Classifier:
+Topic :: Internet :: WWW/HTTP Classifier: Topic :: Security Classifier: Topic
+:: Software Development :: Quality Assurance Classifier: Topic :: Software
 Development :: Testing Classifier: Topic :: System :: Networking Classifier:
 Topic :: Utilities Description-Content-Type: text/markdown License-File:
 LICENSE.txt Requires-Dist: argparse>=1.4.0 Requires-Dist: arrow>=1.3.0
 Requires-Dist: base32-crockford>=0.3.0 Requires-Dist: behave>=1.2.6 Requires-
 Dist: bunch>=1.0.1 Requires-Dist: click>=8.1.7 Requires-Dist: configobj>=5.0.8
 Requires-Dist: datadiff>=2.2.0 Requires-Dist: flake8>=7.0.0 Requires-Dist:
 jsonpointer>=2.4 Requires-Dist: lxml>=5.1.0 Requires-Dist: parse>=1.20.1
```

### Comparing `zato_apitest-24.1.30/setup.py` & `zato_apitest-24.1.31/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under SSPL 1.0, see LICENSE.txt for terms and conditions.
 """
 
 # stdlib
 import os
 from setuptools import setup, find_packages
 
-version = '24.1.30'
+version = '24.1.31'
 
 LONG_DESCRIPTION = """
 
 Write API tests for your [API integrations](https://zato.io) in plain English, with no programming needed.
 
 Here is how it looks like:
 
@@ -39,15 +39,15 @@
       author = 'Zato Source s.r.o.',
       author_email = 'info@zato.io',
       url = 'https://zato.io',
       description = 'API Testing for Humans. Write API tests in pure English, without any programming needed.',
       long_description = LONG_DESCRIPTION,
       long_description_content_type='text/markdown',
       platforms = ['OS Independent'],
-      license = 'Proprietary',
+      license = 'SSPL 1.0',
 
       package_dir = {'':'src'},
       packages = find_packages('src'),
 
       namespace_packages = ['zato'],
       install_requires = parse_requirements(
           os.path.join(os.path.dirname(os.path.realpath(__file__)), 'requirements.txt')),
@@ -57,15 +57,14 @@
       classifiers = [
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'Intended Audience :: Information Technology',
         'Intended Audience :: Other Audience',
-        'License :: Other/Proprietary License',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 3',
         'Intended Audience :: Developers',
         'Topic :: Communications',
```

#### html2text {}

```diff
@@ -1,31 +1,31 @@
 # -*- coding: utf-8 -*- """ Copyright (C) 2024, Zato Source s.r.o. https://
 zato.io Licensed under SSPL 1.0, see LICENSE.txt for terms and conditions. """
 # stdlib import os from setuptools import setup, find_packages version =
-'24.1.30' LONG_DESCRIPTION = """ Write API tests for your [API integrations]
+'24.1.31' LONG_DESCRIPTION = """ Write API tests for your [API integrations]
 (https://zato.io) in plain English, with no programming needed. Here is how it
 looks like: _!_[_A_P_I_ _t_e_s_t_i_n_g_ _i_n_ _P_y_t_h_o_n_]_(_h_t_t_p_s_:_/_/_u_p_c_d_n_._i_o_/_k_W_1_5_b_q_q_/_r_a_w_/_r_o_o_t_/_e_n_/_d_o_c_s_/
 _3_._2_/_g_f_x_/_a_p_i_-_t_e_s_t_i_n_g_/_d_e_m_o_._w_e_b_p_) More information about API testing: https://
 zato.io/en/docs/3.2/api-testing/index.html """ def parse_requirements
 (requirements): # type: ignore ignored = ['#', 'setuptools', '-e'] with open
 (requirements) as f: return [line for line in f if line.strip() and not any
 (line.startswith(prefix) for prefix in ignored)] setup( name = 'zato-apitest',
 version = version, scripts = ['src/zato/apitest/console/apitest'], author =
 'Zato Source s.r.o.', author_email = 'info@zato.io', url = 'https://zato.io',
 description = 'API Testing for Humans. Write API tests in pure English, without
 any programming needed.', long_description = LONG_DESCRIPTION,
 long_description_content_type='text/markdown', platforms = ['OS Independent'],
-license = 'Proprietary', package_dir = {'':'src'}, packages = find_packages
+license = 'SSPL 1.0', package_dir = {'':'src'}, packages = find_packages
 ('src'), namespace_packages = ['zato'], install_requires = parse_requirements
 ( os.path.join(os.path.dirname(os.path.realpath(__file__)),
 'requirements.txt')), zip_safe = False, classifiers = [ 'Development Status ::
 5 - Production/Stable', 'Environment :: Console', 'Environment :: Web
 Environment', 'Intended Audience :: Developers', 'Intended Audience ::
-Information Technology', 'Intended Audience :: Other Audience', 'License ::
-Other/Proprietary License', 'Natural Language :: English', 'Operating System ::
-OS Independent', 'Programming Language :: Python', 'Programming Language ::
-Python :: 2', 'Programming Language :: Python :: 3', 'Intended Audience ::
-Developers', 'Topic :: Communications', 'Topic :: Education :: Testing', 'Topic
-:: Internet', 'Topic :: Internet :: Proxy Servers', 'Topic :: Internet :: WWW/
-HTTP', 'Topic :: Security', 'Topic :: Software Development :: Quality
-Assurance', 'Topic :: Software Development :: Testing', 'Topic :: System ::
-Networking', 'Topic :: Utilities', ], )
+Information Technology', 'Intended Audience :: Other Audience', 'Natural
+Language :: English', 'Operating System :: OS Independent', 'Programming
+Language :: Python', 'Programming Language :: Python :: 2', 'Programming
+Language :: Python :: 3', 'Intended Audience :: Developers', 'Topic ::
+Communications', 'Topic :: Education :: Testing', 'Topic :: Internet', 'Topic
+:: Internet :: Proxy Servers', 'Topic :: Internet :: WWW/HTTP', 'Topic ::
+Security', 'Topic :: Software Development :: Quality Assurance', 'Topic ::
+Software Development :: Testing', 'Topic :: System :: Networking', 'Topic ::
+Utilities', ], )
```

### Comparing `zato_apitest-24.1.30/src/zato/apitest/__init__.py` & `zato_apitest-24.1.31/src/zato/apitest/__init__.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.30/src/zato/apitest/cli.py` & `zato_apitest-24.1.31/src/zato/apitest/cli.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.30/src/zato/apitest/init.py` & `zato_apitest-24.1.31/src/zato/apitest/init.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.30/src/zato/apitest/run.py` & `zato_apitest-24.1.31/src/zato/apitest/run.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.30/src/zato/apitest/steps/common.py` & `zato_apitest-24.1.31/src/zato/apitest/steps/common.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.30/src/zato/apitest/steps/json.py` & `zato_apitest-24.1.31/src/zato/apitest/steps/json.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.30/src/zato/apitest/typing_.py` & `zato_apitest-24.1.31/src/zato/apitest/typing_.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.30/src/zato/apitest/util.py` & `zato_apitest-24.1.31/src/zato/apitest/util.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.30/src/zato_apitest.egg-info/PKG-INFO` & `zato_apitest-24.1.31/src/zato_apitest.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: zato-apitest
-Version: 24.1.30
+Version: 24.1.31
 Summary: API Testing for Humans. Write API tests in pure English, without any programming needed.
 Home-page: https://zato.io
 Author: Zato Source s.r.o.
 Author-email: info@zato.io
-License: Proprietary
+License: SSPL 1.0
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Other Audience
-Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Communications
```

#### html2text {}

```diff
@@ -1,23 +1,22 @@
-Metadata-Version: 2.1 Name: zato-apitest Version: 24.1.30 Summary: API Testing
+Metadata-Version: 2.1 Name: zato-apitest Version: 24.1.31 Summary: API Testing
 for Humans. Write API tests in pure English, without any programming needed.
 Home-page: https://zato.io Author: Zato Source s.r.o. Author-email:
-info@zato.io License: Proprietary Platform: OS Independent Classifier:
-Development Status :: 5 - Production/Stable Classifier: Environment :: Console
-Classifier: Environment :: Web Environment Classifier: Intended Audience ::
-Developers Classifier: Intended Audience :: Information Technology Classifier:
-Intended Audience :: Other Audience Classifier: License :: Other/Proprietary
-License Classifier: Natural Language :: English Classifier: Operating System ::
-OS Independent Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 2 Classifier: Programming Language :: Python
-:: 3 Classifier: Intended Audience :: Developers Classifier: Topic ::
-Communications Classifier: Topic :: Education :: Testing Classifier: Topic ::
-Internet Classifier: Topic :: Internet :: Proxy Servers Classifier: Topic ::
-Internet :: WWW/HTTP Classifier: Topic :: Security Classifier: Topic ::
-Software Development :: Quality Assurance Classifier: Topic :: Software
+info@zato.io License: SSPL 1.0 Platform: OS Independent Classifier: Development
+Status :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
+Environment :: Web Environment Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology Classifier: Intended
+Audience :: Other Audience Classifier: Natural Language :: English Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2 Classifier: Programming
+Language :: Python :: 3 Classifier: Intended Audience :: Developers Classifier:
+Topic :: Communications Classifier: Topic :: Education :: Testing Classifier:
+Topic :: Internet Classifier: Topic :: Internet :: Proxy Servers Classifier:
+Topic :: Internet :: WWW/HTTP Classifier: Topic :: Security Classifier: Topic
+:: Software Development :: Quality Assurance Classifier: Topic :: Software
 Development :: Testing Classifier: Topic :: System :: Networking Classifier:
 Topic :: Utilities Description-Content-Type: text/markdown License-File:
 LICENSE.txt Requires-Dist: argparse>=1.4.0 Requires-Dist: arrow>=1.3.0
 Requires-Dist: base32-crockford>=0.3.0 Requires-Dist: behave>=1.2.6 Requires-
 Dist: bunch>=1.0.1 Requires-Dist: click>=8.1.7 Requires-Dist: configobj>=5.0.8
 Requires-Dist: datadiff>=2.2.0 Requires-Dist: flake8>=7.0.0 Requires-Dist:
 jsonpointer>=2.4 Requires-Dist: lxml>=5.1.0 Requires-Dist: parse>=1.20.1
```

### Comparing `zato_apitest-24.1.30/src/zato_apitest.egg-info/SOURCES.txt` & `zato_apitest-24.1.31/src/zato_apitest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

