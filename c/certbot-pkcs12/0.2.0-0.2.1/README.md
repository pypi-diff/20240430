# Comparing `tmp/certbot-pkcs12-0.2.0.tar.gz` & `tmp/certbot_pkcs12-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot-pkcs12-0.2.0.tar", last modified: Mon May  9 18:29:20 2022, max compression
+gzip compressed data, was "certbot_pkcs12-0.2.1.tar", last modified: Tue Apr 30 20:29:58 2024, max compression
```

## Comparing `certbot-pkcs12-0.2.0.tar` & `certbot_pkcs12-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 lpsinger (273296831) staff       (20)        0 2022-05-09 18:29:20.173643 certbot-pkcs12-0.2.0/
--rw-r--r--   0 lpsinger (273296831) staff       (20)      831 2022-05-09 18:29:20.173826 certbot-pkcs12-0.2.0/PKG-INFO
--rw-r--r--   0 lpsinger (273296831) staff       (20)      241 2022-05-05 18:44:25.000000 certbot-pkcs12-0.2.0/README.md
-drwxr-xr-x   0 lpsinger (273296831) staff       (20)        0 2022-05-09 18:29:20.171529 certbot-pkcs12-0.2.0/certbot_pkcs12.egg-info/
--rw-r--r--   0 lpsinger (273296831) staff       (20)      831 2022-05-09 18:29:19.000000 certbot-pkcs12-0.2.0/certbot_pkcs12.egg-info/PKG-INFO
--rw-r--r--   0 lpsinger (273296831) staff       (20)      282 2022-05-09 18:29:20.000000 certbot-pkcs12-0.2.0/certbot_pkcs12.egg-info/SOURCES.txt
--rw-r--r--   0 lpsinger (273296831) staff       (20)        1 2022-05-09 18:29:19.000000 certbot-pkcs12-0.2.0/certbot_pkcs12.egg-info/dependency_links.txt
--rw-r--r--   0 lpsinger (273296831) staff       (20)       52 2022-05-09 18:29:19.000000 certbot-pkcs12-0.2.0/certbot_pkcs12.egg-info/entry_points.txt
--rw-r--r--   0 lpsinger (273296831) staff       (20)       26 2022-05-09 18:29:20.000000 certbot-pkcs12-0.2.0/certbot_pkcs12.egg-info/requires.txt
--rw-r--r--   0 lpsinger (273296831) staff       (20)       15 2022-05-09 18:29:20.000000 certbot-pkcs12-0.2.0/certbot_pkcs12.egg-info/top_level.txt
--rw-r--r--   0 lpsinger (273296831) staff       (20)     2292 2022-05-09 17:39:54.000000 certbot-pkcs12-0.2.0/certbot_pkcs12.py
--rw-r--r--   0 lpsinger (273296831) staff       (20)       81 2022-05-05 17:44:33.000000 certbot-pkcs12-0.2.0/pyproject.toml
--rw-r--r--   0 lpsinger (273296831) staff       (20)      782 2022-05-09 18:29:20.174725 certbot-pkcs12-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:29:58.338918 certbot_pkcs12-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-30 20:29:58.338918 certbot_pkcs12-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-30 20:29:49.000000 certbot_pkcs12-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:29:58.338918 certbot_pkcs12-0.2.1/certbot_pkcs12.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-30 20:29:58.000000 certbot_pkcs12-0.2.1/certbot_pkcs12.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-30 20:29:58.000000 certbot_pkcs12-0.2.1/certbot_pkcs12.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 20:29:58.000000 certbot_pkcs12-0.2.1/certbot_pkcs12.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-30 20:29:58.000000 certbot_pkcs12-0.2.1/certbot_pkcs12.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-30 20:29:58.000000 certbot_pkcs12-0.2.1/certbot_pkcs12.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-30 20:29:58.000000 certbot_pkcs12-0.2.1/certbot_pkcs12.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-30 20:29:49.000000 certbot_pkcs12-0.2.1/certbot_pkcs12.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-30 20:29:49.000000 certbot_pkcs12-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-30 20:29:58.338918 certbot_pkcs12-0.2.1/setup.cfg
```

### Comparing `certbot-pkcs12-0.2.0/PKG-INFO` & `certbot_pkcs12-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: certbot-pkcs12
-Version: 0.2.0
+Version: 0.2.1
 Summary: "PKCS#12 installer plugin for Certbot and Let's Encrypt"
 Home-page: https://github.com/lpsinger/certbot-pkcs12
 Author: Leo Singer
 Author-email: leo.singer@ligo.org
 License: Apache-2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Security :: Cryptography
 Description-Content-Type: text/markdown
+Requires-Dist: certbot>=1.19.0
+Requires-Dist: pyOpenSSL<24.1.0
 
 # Certbot PKCS#12 plugin
 
 This is an installer plugin for [certbot](https://certbot.eff.org). Whenever
 you generate a certificate with Let's Encrypt, it will save the certificate
 in a [PKCS#12](https://en.wikipedia.org/wiki/PKCS_12) archive.
-
```

### Comparing `certbot-pkcs12-0.2.0/certbot_pkcs12.egg-info/PKG-INFO` & `certbot_pkcs12-0.2.1/certbot_pkcs12.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: certbot-pkcs12
-Version: 0.2.0
+Version: 0.2.1
 Summary: "PKCS#12 installer plugin for Certbot and Let's Encrypt"
 Home-page: https://github.com/lpsinger/certbot-pkcs12
 Author: Leo Singer
 Author-email: leo.singer@ligo.org
 License: Apache-2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Security :: Cryptography
 Description-Content-Type: text/markdown
+Requires-Dist: certbot>=1.19.0
+Requires-Dist: pyOpenSSL<24.1.0
 
 # Certbot PKCS#12 plugin
 
 This is an installer plugin for [certbot](https://certbot.eff.org). Whenever
 you generate a certificate with Let's Encrypt, it will save the certificate
 in a [PKCS#12](https://en.wikipedia.org/wiki/PKCS_12) archive.
-
```

### Comparing `certbot-pkcs12-0.2.0/certbot_pkcs12.py` & `certbot_pkcs12-0.2.1/certbot_pkcs12.py`

 * *Files identical despite different names*

### Comparing `certbot-pkcs12-0.2.0/setup.cfg` & `certbot_pkcs12-0.2.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = certbot-pkcs12
 license = Apache-2.0
-version = 0.2.0
+version = 0.2.1
 description = "PKCS#12 installer plugin for Certbot and Let's Encrypt"
 long_description = file:README.md
 long_description_content_type = text/markdown
 author = Leo Singer
 author_email = leo.singer@ligo.org
 url = https://github.com/lpsinger/certbot-pkcs12
 classifiers = 
@@ -15,15 +15,15 @@
 	Intended Audience :: System Administrators
 	Topic :: Internet :: WWW/HTTP
 	Topic :: Security :: Cryptography
 
 [options]
 install_requires = 
 	certbot >= 1.19.0
-	pyOpenSSL
+	pyOpenSSL < 24.1.0
 py_modules = certbot_pkcs12
 python_version = >= 3.8
 
 [options.entry_points]
 certbot.plugins = 
 	pkcs12 = certbot_pkcs12:Installer
```

