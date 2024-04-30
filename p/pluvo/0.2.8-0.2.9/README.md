# Comparing `tmp/pluvo-0.2.8.tar.gz` & `tmp/pluvo-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pluvo-0.2.8.tar", last modified: Thu May 17 11:55:32 2018, max compression
+gzip compressed data, was "dist/pluvo-0.2.9.tar", last modified: Wed May 23 13:25:13 2018, max compression
```

## Comparing `pluvo-0.2.8.tar` & `pluvo-0.2.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 Sander     (501) staff       (20)        0 2018-05-17 11:55:32.000000 pluvo-0.2.8/
--rw-r--r--   0 Sander     (501) staff       (20)      566 2018-05-17 11:55:32.000000 pluvo-0.2.8/PKG-INFO
--rw-r--r--   0 Sander     (501) staff       (20)     1071 2018-05-17 10:16:30.000000 pluvo-0.2.8/LICENSE
--rw-r--r--   0 Sander     (501) staff       (20)      129 2018-05-17 10:16:30.000000 pluvo-0.2.8/requirements.txt
-drwxr-xr-x   0 Sander     (501) staff       (20)        0 2018-05-17 11:55:32.000000 pluvo-0.2.8/tests/
--rw-r--r--   0 Sander     (501) staff       (20)        0 2018-05-17 10:16:30.000000 pluvo-0.2.8/tests/__init__.py
--rw-r--r--   0 Sander     (501) staff       (20)    18145 2018-05-17 11:37:08.000000 pluvo-0.2.8/tests/test_pluvo.py
--rw-r--r--   0 Sander     (501) staff       (20)       80 2018-05-17 10:16:30.000000 pluvo-0.2.8/MANIFEST.in
-drwxr-xr-x   0 Sander     (501) staff       (20)        0 2018-05-17 11:55:32.000000 pluvo-0.2.8/pluvo.egg-info/
--rw-r--r--   0 Sander     (501) staff       (20)      566 2018-05-17 11:55:32.000000 pluvo-0.2.8/pluvo.egg-info/PKG-INFO
--rw-r--r--   0 Sander     (501) staff       (20)      288 2018-05-17 11:55:32.000000 pluvo-0.2.8/pluvo.egg-info/SOURCES.txt
--rw-r--r--   0 Sander     (501) staff       (20)        9 2018-05-17 11:55:32.000000 pluvo-0.2.8/pluvo.egg-info/requires.txt
--rw-r--r--   0 Sander     (501) staff       (20)        6 2018-05-17 11:55:32.000000 pluvo-0.2.8/pluvo.egg-info/top_level.txt
--rw-r--r--   0 Sander     (501) staff       (20)        1 2018-05-17 11:55:32.000000 pluvo-0.2.8/pluvo.egg-info/dependency_links.txt
--rw-r--r--   0 Sander     (501) staff       (20)     2431 2018-05-17 10:16:30.000000 pluvo-0.2.8/README.md
--rw-r--r--   0 Sander     (501) staff       (20)      831 2018-05-17 11:37:29.000000 pluvo-0.2.8/setup.py
-drwxr-xr-x   0 Sander     (501) staff       (20)        0 2018-05-17 11:55:32.000000 pluvo-0.2.8/pluvo/
--rw-r--r--   0 Sander     (501) staff       (20)      140 2018-05-17 10:16:30.000000 pluvo-0.2.8/pluvo/__init__.py
--rw-r--r--   0 Sander     (501) staff       (20)    11971 2018-05-17 11:36:19.000000 pluvo-0.2.8/pluvo/pluvo.py
--rw-r--r--   0 Sander     (501) staff       (20)      129 2018-05-17 11:55:32.000000 pluvo-0.2.8/setup.cfg
--rwxr-xr-x   0 Sander     (501) staff       (20)       74 2018-05-17 10:16:30.000000 pluvo-0.2.8/test.sh
+drwxr-xr-x   0 Sander     (501) staff       (20)        0 2018-05-23 13:25:13.000000 pluvo-0.2.9/
+-rw-r--r--   0 Sander     (501) staff       (20)      566 2018-05-23 13:25:13.000000 pluvo-0.2.9/PKG-INFO
+-rw-r--r--   0 Sander     (501) staff       (20)     1071 2018-05-17 10:16:30.000000 pluvo-0.2.9/LICENSE
+-rw-r--r--   0 Sander     (501) staff       (20)      129 2018-05-17 10:16:30.000000 pluvo-0.2.9/requirements.txt
+drwxr-xr-x   0 Sander     (501) staff       (20)        0 2018-05-23 13:25:13.000000 pluvo-0.2.9/tests/
+-rw-r--r--   0 Sander     (501) staff       (20)        0 2018-05-17 10:16:30.000000 pluvo-0.2.9/tests/__init__.py
+-rw-r--r--   0 Sander     (501) staff       (20)    18517 2018-05-23 13:18:14.000000 pluvo-0.2.9/tests/test_pluvo.py
+-rw-r--r--   0 Sander     (501) staff       (20)       80 2018-05-17 10:16:30.000000 pluvo-0.2.9/MANIFEST.in
+drwxr-xr-x   0 Sander     (501) staff       (20)        0 2018-05-23 13:25:13.000000 pluvo-0.2.9/pluvo.egg-info/
+-rw-r--r--   0 Sander     (501) staff       (20)      566 2018-05-23 13:25:13.000000 pluvo-0.2.9/pluvo.egg-info/PKG-INFO
+-rw-r--r--   0 Sander     (501) staff       (20)      288 2018-05-23 13:25:13.000000 pluvo-0.2.9/pluvo.egg-info/SOURCES.txt
+-rw-r--r--   0 Sander     (501) staff       (20)        9 2018-05-23 13:25:13.000000 pluvo-0.2.9/pluvo.egg-info/requires.txt
+-rw-r--r--   0 Sander     (501) staff       (20)        6 2018-05-23 13:25:13.000000 pluvo-0.2.9/pluvo.egg-info/top_level.txt
+-rw-r--r--   0 Sander     (501) staff       (20)        1 2018-05-23 13:25:13.000000 pluvo-0.2.9/pluvo.egg-info/dependency_links.txt
+-rw-r--r--   0 Sander     (501) staff       (20)     2431 2018-05-17 10:16:30.000000 pluvo-0.2.9/README.md
+-rw-r--r--   0 Sander     (501) staff       (20)      831 2018-05-23 13:18:41.000000 pluvo-0.2.9/setup.py
+drwxr-xr-x   0 Sander     (501) staff       (20)        0 2018-05-23 13:25:13.000000 pluvo-0.2.9/pluvo/
+-rw-r--r--   0 Sander     (501) staff       (20)      140 2018-05-17 10:16:30.000000 pluvo-0.2.9/pluvo/__init__.py
+-rw-r--r--   0 Sander     (501) staff       (20)    12061 2018-05-23 13:18:14.000000 pluvo-0.2.9/pluvo/pluvo.py
+-rw-r--r--   0 Sander     (501) staff       (20)      108 2018-05-23 13:25:13.000000 pluvo-0.2.9/setup.cfg
+-rwxr-xr-x   0 Sander     (501) staff       (20)       74 2018-05-17 10:16:30.000000 pluvo-0.2.9/test.sh
```

### Comparing `pluvo-0.2.8/PKG-INFO` & `pluvo-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pluvo
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python library to access the Pluvo REST API.
 Home-page: https://github.com/wendbv/pluvo-python
 Author: Wend BV
 Author-email: info@wend.nl
 License: MIT
 Description: UNKNOWN
 Keywords: REST,API,Pluvo
```

### Comparing `pluvo-0.2.8/LICENSE` & `pluvo-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pluvo-0.2.8/tests/test_pluvo.py` & `pluvo-0.2.9/tests/test_pluvo.py`

 * *Files 1% similar despite different names*

```diff
@@ -576,15 +576,26 @@
 def test_pluvo_get_course_report(mocker):
     p = pluvo.Pluvo(token='token')
     mocker.patch.object(p, '_request')
 
     retval = p.get_course_report(1, 2)
     assert retval == p._request.return_value
     p._request.assert_called_once_with(
-        'GET', 'report/course/1/user/2/')
+        'GET', 'report/course/1/user/2/', params={})
+
+
+def test_pluvo_get_course_report_filename(mocker):
+    p = pluvo.Pluvo(token='token')
+    mocker.patch.object(p, '_request')
+
+    filename = 'test.pdf'
+    retval = p.get_course_report(1, 2, filename)
+    assert retval == p._request.return_value
+    p._request.assert_called_once_with(
+        'GET', 'report/course/1/user/2/', params={'filename': filename})
 
 
 def test_pluvo_get_version(mocker):
     p = pluvo.Pluvo(token='token')
     mocker.patch.object(p, '_request')
 
     retval = p.get_version()
```

### Comparing `pluvo-0.2.8/pluvo.egg-info/PKG-INFO` & `pluvo-0.2.9/pluvo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pluvo
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python library to access the Pluvo REST API.
 Home-page: https://github.com/wendbv/pluvo-python
 Author: Wend BV
 Author-email: info@wend.nl
 License: MIT
 Description: UNKNOWN
 Keywords: REST,API,Pluvo
```

### Comparing `pluvo-0.2.8/README.md` & `pluvo-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pluvo-0.2.8/setup.py` & `pluvo-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 
 setup(
     name='pluvo',
     packages=['pluvo'],
     package_data={},
-    version='0.2.8',
+    version='0.2.9',
     description='Python library to access the Pluvo REST API.',
     author='Wend BV',
     author_email='info@wend.nl',
     license='MIT',
     url='https://github.com/wendbv/pluvo-python',
     keywords=['REST', 'API', 'Pluvo'],
     classifiers=[
```

### Comparing `pluvo-0.2.8/pluvo/pluvo.py` & `pluvo-0.2.9/pluvo/pluvo.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,14 +299,15 @@
             'order_by': order_by,
             'offset': offset,
             'limit': limit
         }
         return self._get_multiple(
             'progress/reports/', params=params, method='GET')
 
-    def get_course_report(self, course_id, student_id):
+    def get_course_report(self, course_id, student_id, filename=None):
+        params = {'filename': filename} if filename else {}
         url = 'report/course/{}/user/{}/'.format(course_id, student_id)
-        return self._request('GET', url)
+        return self._request('GET', url, params=params)
 
     def get_version(self):
         """Get the Pluvo API version."""
         return self._request('GET', 'version/')
```

