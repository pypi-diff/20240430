# Comparing `tmp/epages_provisioning-1.0.2.tar.gz` & `tmp/epages_provisioning-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/epages_provisioning/epages_provisioning/dist/tmp1sc8qts3/epages_provisioning-1.0.2.tar", last modified: Mon Jan  4 15:10:37 2021, max compression
+gzip compressed data, was "epages_provisioning-1.1.1.tar", last modified: Tue Apr 30 08:23:37 2024, max compression
```

## Comparing `epages_provisioning-1.0.2.tar` & `epages_provisioning-1.1.1.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-04 15:10:37.000000 epages_provisioning-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (116)      158 2021-01-04 15:10:32.000000 epages_provisioning-1.0.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (116)     3707 2021-01-04 15:10:32.000000 epages_provisioning-1.0.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1232 2021-01-04 15:10:32.000000 epages_provisioning-1.0.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1071 2021-01-04 15:10:32.000000 epages_provisioning-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      262 2021-01-04 15:10:32.000000 epages_provisioning-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     4062 2021-01-04 15:10:37.000000 epages_provisioning-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1337 2021-01-04 15:10:32.000000 epages_provisioning-1.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-04 15:10:37.000000 epages_provisioning-1.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (116)     6814 2021-01-04 15:10:32.000000 epages_provisioning-1.0.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)       28 2021-01-04 15:10:32.000000 epages_provisioning-1.0.2/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (116)     8539 2021-01-04 15:10:32.000000 epages_provisioning-1.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)       33 2021-01-04 15:10:32.000000 epages_provisioning-1.0.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (116)       28 2021-01-04 15:10:32.000000 epages_provisioning-1.0.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (116)      314 2021-01-04 15:10:32.000000 epages_provisioning-1.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1199 2021-01-04 15:10:32.000000 epages_provisioning-1.0.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (116)     6485 2021-01-04 15:10:32.000000 epages_provisioning-1.0.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (116)       27 2021-01-04 15:10:32.000000 epages_provisioning-1.0.2/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (116)     4076 2021-01-04 15:10:32.000000 epages_provisioning-1.0.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-04 15:10:37.000000 epages_provisioning-1.0.2/epages_provisioning/
--rw-r--r--   0 runner    (1001) docker     (116)      216 2021-01-04 15:10:32.000000 epages_provisioning-1.0.2/epages_provisioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    17838 2021-01-04 15:10:32.000000 epages_provisioning-1.0.2/epages_provisioning/provisioning.py
--rw-r--r--   0 runner    (1001) docker     (116)     7996 2021-01-04 15:10:32.000000 epages_provisioning-1.0.2/epages_provisioning/shop.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-04 15:10:37.000000 epages_provisioning-1.0.2/epages_provisioning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4062 2021-01-04 15:10:37.000000 epages_provisioning-1.0.2/epages_provisioning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      678 2021-01-04 15:10:37.000000 epages_provisioning-1.0.2/epages_provisioning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-04 15:10:37.000000 epages_provisioning-1.0.2/epages_provisioning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-04 15:10:37.000000 epages_provisioning-1.0.2/epages_provisioning.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       12 2021-01-04 15:10:37.000000 epages_provisioning-1.0.2/epages_provisioning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       20 2021-01-04 15:10:37.000000 epages_provisioning-1.0.2/epages_provisioning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      402 2021-01-04 15:10:37.000000 epages_provisioning-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1442 2021-01-04 15:10:32.000000 epages_provisioning-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-04 15:10:37.000000 epages_provisioning-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (116)      114 2021-01-04 15:10:32.000000 epages_provisioning-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10384 2021-01-04 15:10:32.000000 epages_provisioning-1.0.2/tests/test_epages_provisioning.py
--rw-r--r--   0 runner    (1001) docker     (116)     4025 2021-01-04 15:10:32.000000 epages_provisioning-1.0.2/tests/test_shop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:23:37.976605 epages_provisioning-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-30 08:23:33.000000 epages_provisioning-1.1.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-04-30 08:23:33.000000 epages_provisioning-1.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-30 08:23:33.000000 epages_provisioning-1.1.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-30 08:23:33.000000 epages_provisioning-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-30 08:23:33.000000 epages_provisioning-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-04-30 08:23:37.976605 epages_provisioning-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-30 08:23:33.000000 epages_provisioning-1.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:23:37.972605 epages_provisioning-1.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-30 08:23:33.000000 epages_provisioning-1.1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 08:23:33.000000 epages_provisioning-1.1.1/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8539 2024-04-30 08:23:33.000000 epages_provisioning-1.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-30 08:23:33.000000 epages_provisioning-1.1.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 08:23:33.000000 epages_provisioning-1.1.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-30 08:23:33.000000 epages_provisioning-1.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-30 08:23:33.000000 epages_provisioning-1.1.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-04-30 08:23:33.000000 epages_provisioning-1.1.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-30 08:23:33.000000 epages_provisioning-1.1.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-04-30 08:23:33.000000 epages_provisioning-1.1.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:23:37.972605 epages_provisioning-1.1.1/epages_provisioning/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-30 08:23:33.000000 epages_provisioning-1.1.1/epages_provisioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13875 2024-04-30 08:23:33.000000 epages_provisioning-1.1.1/epages_provisioning/provisioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7996 2024-04-30 08:23:33.000000 epages_provisioning-1.1.1/epages_provisioning/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-04-30 08:23:33.000000 epages_provisioning-1.1.1/epages_provisioning/zeep_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:23:37.972605 epages_provisioning-1.1.1/epages_provisioning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-04-30 08:23:37.000000 epages_provisioning-1.1.1/epages_provisioning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-30 08:23:37.000000 epages_provisioning-1.1.1/epages_provisioning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 08:23:37.000000 epages_provisioning-1.1.1/epages_provisioning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 08:23:37.000000 epages_provisioning-1.1.1/epages_provisioning.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 08:23:37.000000 epages_provisioning-1.1.1/epages_provisioning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-30 08:23:37.000000 epages_provisioning-1.1.1/epages_provisioning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-30 08:23:37.976605 epages_provisioning-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-30 08:23:33.000000 epages_provisioning-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:23:37.972605 epages_provisioning-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-30 08:23:33.000000 epages_provisioning-1.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10635 2024-04-30 08:23:33.000000 epages_provisioning-1.1.1/tests/test_epages_provisioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-30 08:23:33.000000 epages_provisioning-1.1.1/tests/test_shop.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `epages_provisioning-1.0.2/CONTRIBUTING.rst` & `epages_provisioning-1.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `epages_provisioning-1.0.2/HISTORY.rst` & `epages_provisioning-1.1.1/HISTORY.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 =======
 History
 =======
 
+1.1.1 (2024-04-30)
+------------------
+* bump version to get a proper release done after fixing publish workflow
+
+1.1.0 (2024-04-30)
+------------------
+
+* Sync all zeep requirements to 4.2.1
+* Fix `test_010_create_mindata` to send `WebServerScriptNamePart` which is required now
+* Allow defining shoptype as env variable for tests
+* up Pipenv python version to 3.8
+* refactor zeep utils to own file
+* use local copy of soap-encodings as the server is not stable
+  * see: https://github.com/mvantellingen/python-zeep/issues/1417
+
 1.0.2 (2021-01-04)
 ------------------
 
 * remove last remrants of travis from docs
 * fix readme in built package
 * retest deploy process
```

### Comparing `epages_provisioning-1.0.2/LICENSE` & `epages_provisioning-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `epages_provisioning-1.0.2/README.rst` & `epages_provisioning-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `epages_provisioning-1.0.2/docs/Makefile` & `epages_provisioning-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `epages_provisioning-1.0.2/docs/conf.py` & `epages_provisioning-1.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `epages_provisioning-1.0.2/docs/installation.rst` & `epages_provisioning-1.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `epages_provisioning-1.0.2/docs/make.bat` & `epages_provisioning-1.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `epages_provisioning-1.0.2/docs/usage.rst` & `epages_provisioning-1.1.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `epages_provisioning-1.0.2/epages_provisioning/shop.py` & `epages_provisioning-1.1.1/epages_provisioning/shop.py`

 * *Files identical despite different names*

### Comparing `epages_provisioning-1.0.2/epages_provisioning.egg-info/SOURCES.txt` & `epages_provisioning-1.1.1/epages_provisioning.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 epages_provisioning/__init__.py
 epages_provisioning/provisioning.py
 epages_provisioning/shop.py
+epages_provisioning/zeep_utils.py
 epages_provisioning.egg-info/PKG-INFO
 epages_provisioning.egg-info/SOURCES.txt
 epages_provisioning.egg-info/dependency_links.txt
 epages_provisioning.egg-info/not-zip-safe
 epages_provisioning.egg-info/requires.txt
 epages_provisioning.egg-info/top_level.txt
 tests/__init__.py
```

### Comparing `epages_provisioning-1.0.2/setup.py` & `epages_provisioning-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
 requirements = [
-    'zeep>=4.0.0',
+    'zeep==4.2.1',
 ]
 
 setup_requirements = [
     # TODO: put setup requirements (distutils extensions, etc.) here
 ]
 
 test_requirements = [
     # TODO: put package test requirements here
 ]
 
 setup(
     name='epages_provisioning',
-    version='1.0.2',
+    version='1.1.1',
     description="Python library for calling ePages provisioning services",
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/x-rst',
     author="Tatu Wikman",
     author_email='tatu.wikman@gmail.com',
     url='https://github.com/tswfi/epages_provisioning',
     packages=find_packages(include=['epages_provisioning']),
```

### Comparing `epages_provisioning-1.0.2/tests/test_epages_provisioning.py` & `epages_provisioning-1.1.1/tests/test_epages_provisioning.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,20 @@
     These tests also assume that the ePages service is a default installation
     with default shoptypes etc.
 
     Also if you want to see a full message trace say:
 
         export EP_TRACE=1
 
+    And you can define the shoptype to use with
+
+        export EP_SHOPTYPE=MinDemo
+
+    MinDemo is the default value if not set
+
     and then run your tests
 
     Warning: these will take a while to run.
     """
     @classmethod
     def setUpClass(cls):
         """
@@ -72,25 +78,26 @@
             provider=os.environ['EP_PROVIDER'],
             username=os.environ['EP_USERNAME'],
             password=os.environ['EP_PASSWORD'],
         )
         # used as alias for these tests
         cls._nowstr = datetime.now().strftime('%Y%m%d%H%M%S%f')
         cls._shopalias_min = 'test-{}-min'.format(cls._nowstr)
-        cls._shoptype = 'MinDemo'
+        cls._shoptype = os.environ.get('EP_SHOPTYPE', 'MinDemo')
 
     def test_000_get_all_info(self):
         """ get info of all shops for this provider """
         self.assertTrue(self._sc.get_all_info())
 
     def test_010_create_mindata(self):
         """ create shop with minimal data """
         shop = self._sc.get_createshop_obj()
         shop.Alias = self._shopalias_min
         shop.ShopAlias = self._shopalias_min
+        shop.WebServerScriptNamePart = self._shopalias_min
         shop.ShopType = self._shoptype
         self.assertIsNone(self._sc.create(shop))
 
     def test_020_exists(self):
         """ check that our creation was succesfull by checking
         that the shop exists """
         shopref = self._sc.get_shopref_obj()
@@ -180,15 +187,15 @@
         cls._nowstr = datetime.now().strftime('%Y%m%d%H%M%S%f')
         cls._shopalias_min = 'test-{}-min'.format(cls._nowstr)
         cls._shopalias_min_tmp = 'test-{}-min_tmp'.format(cls._nowstr)
         cls._shopalias_add = 'test-{}-add'.format(cls._nowstr)
 
         # this is probably the smallest shoptype for testing, others might be
         # "EBiz5" or "eCMSFree"
-        cls._shoptype = "MinDemo"
+        cls._shoptype = os.environ.get('EP_SHOPTYPE', 'MinDemo')
 
     def test_000_create_mindata(self):
         """
         test creating new shop with minimal data
         """
         shop = self._sp.get_createshop_obj(
             {
```

### Comparing `epages_provisioning-1.0.2/tests/test_shop.py` & `epages_provisioning-1.1.1/tests/test_shop.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,20 @@
     These tests also assume that the ePages service is a default installation
     with default shoptypes etc.
 
     Also if you want to see a full message trace say:
 
         export EP_TRACE=1
 
+    And you can define the shoptype to use with
+
+        export EP_SHOPTYPE=MinDemo
+
+    MinDemo is the default value if not set
+
     and then run your tests
 
     Warning: these will take a while to run.
     """
     @classmethod
     def setUpClass(cls):
         """
@@ -60,15 +66,15 @@
             provider=os.environ['EP_PROVIDER'],
             username=os.environ['EP_USERNAME'],
             password=os.environ['EP_PASSWORD'],
         )
         # used as alias for these tests
         cls._nowstr = datetime.now().strftime('%Y%m%d%H%M%S%f')
         cls._alias = 'test-{}-min'.format(cls._nowstr)
-        cls._shoptype = 'MinDemo'
+        cls._shoptype = os.environ.get('EP_SHOPTYPE', 'MinDemo')
         print("Using shopalias: {} for testing".format(cls._alias))
 
     def setUp(self):
         """ get a shop to play with """
         self.s = Shop(Alias=self._alias, provisioning=self._sc)
 
     def test_001_start(self):
```

