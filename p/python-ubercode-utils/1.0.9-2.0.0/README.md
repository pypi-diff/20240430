# Comparing `tmp/python-ubercode-utils-1.0.9.tar.gz` & `tmp/python-ubercode-utils-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-ubercode-utils-1.0.9.tar", last modified: Thu Jan 18 22:26:26 2024, max compression
+gzip compressed data, was "dist/python-ubercode-utils-2.0.0.tar", last modified: Tue Apr 30 14:57:23 2024, max compression
```

## Comparing `python-ubercode-utils-1.0.9.tar` & `python-ubercode-utils-2.0.0.tar`

### file list

```diff
@@ -1,34 +1,32 @@
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2024-01-18 22:26:26.541945 python-ubercode-utils-1.0.9/
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1069 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.9/LICENSE
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       43 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.9/MANIFEST.in
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1330 2024-01-18 22:26:26.541945 python-ubercode-utils-1.0.9/PKG-INFO
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      683 2023-03-06 19:32:30.000000 python-ubercode-utils-1.0.9/README.md
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2024-01-18 22:26:26.537945 python-ubercode-utils-1.0.9/python_ubercode_utils.egg-info/
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1330 2024-01-18 22:26:26.000000 python-ubercode-utils-1.0.9/python_ubercode_utils.egg-info/PKG-INFO
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      676 2024-01-18 22:26:26.000000 python-ubercode-utils-1.0.9/python_ubercode_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        1 2024-01-18 22:26:26.000000 python-ubercode-utils-1.0.9/python_ubercode_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        1 2024-01-18 22:26:08.000000 python-ubercode-utils-1.0.9/python_ubercode_utils.egg-info/not-zip-safe
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        9 2024-01-18 22:26:26.000000 python-ubercode-utils-1.0.9/python_ubercode_utils.egg-info/top_level.txt
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       38 2024-01-18 22:26:26.541945 python-ubercode-utils-1.0.9/setup.cfg
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      886 2024-01-18 22:25:24.000000 python-ubercode-utils-1.0.9/setup.py
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2024-01-18 22:26:26.541945 python-ubercode-utils-1.0.9/test/
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)    10782 2023-10-26 21:59:32.000000 python-ubercode-utils-1.0.9/test/test_convert.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     2712 2023-03-09 19:13:29.000000 python-ubercode-utils-1.0.9/test/test_cursor.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1234 2023-04-13 22:45:39.000000 python-ubercode-utils-1.0.9/test/test_dataframe.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     5657 2023-04-13 22:45:39.000000 python-ubercode-utils-1.0.9/test/test_environment.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     3000 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.9/test/test_json.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     2855 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.9/test/test_logging.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     7167 2024-01-18 22:23:25.000000 python-ubercode-utils-1.0.9/test/test_urls.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     2144 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.9/test/test_xml.py
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2024-01-18 22:26:26.541945 python-ubercode-utils-1.0.9/ubercode/
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        0 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.9/ubercode/__init__.py
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2024-01-18 22:26:26.541945 python-ubercode-utils-1.0.9/ubercode/utils/
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        0 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.9/ubercode/utils/__init__.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)    10011 2023-10-26 21:59:32.000000 python-ubercode-utils-1.0.9/ubercode/utils/convert.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1118 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.9/ubercode/utils/cursor.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      870 2023-04-03 13:13:43.000000 python-ubercode-utils-1.0.9/ubercode/utils/dataframe.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)    10854 2023-04-13 22:45:39.000000 python-ubercode-utils-1.0.9/ubercode/utils/environment.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1630 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.9/ubercode/utils/json.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     9199 2023-03-06 22:18:08.000000 python-ubercode-utils-1.0.9/ubercode/utils/logging.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     9332 2024-01-18 22:23:25.000000 python-ubercode-utils-1.0.9/ubercode/utils/urls.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     2876 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.9/ubercode/utils/xml.py
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2024-04-30 14:57:23.017424 python-ubercode-utils-2.0.0/
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1069 2023-03-06 19:22:56.000000 python-ubercode-utils-2.0.0/LICENSE
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       43 2023-03-06 19:22:56.000000 python-ubercode-utils-2.0.0/MANIFEST.in
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1330 2024-04-30 14:57:23.013424 python-ubercode-utils-2.0.0/PKG-INFO
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      683 2023-03-06 19:32:30.000000 python-ubercode-utils-2.0.0/README.md
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2024-04-30 14:57:23.013424 python-ubercode-utils-2.0.0/python_ubercode_utils.egg-info/
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1330 2024-04-30 14:57:22.000000 python-ubercode-utils-2.0.0/python_ubercode_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      637 2024-04-30 14:57:22.000000 python-ubercode-utils-2.0.0/python_ubercode_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        1 2024-04-30 14:57:22.000000 python-ubercode-utils-2.0.0/python_ubercode_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        1 2024-04-30 14:56:56.000000 python-ubercode-utils-2.0.0/python_ubercode_utils.egg-info/not-zip-safe
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        9 2024-04-30 14:57:22.000000 python-ubercode-utils-2.0.0/python_ubercode_utils.egg-info/top_level.txt
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       38 2024-04-30 14:57:23.017424 python-ubercode-utils-2.0.0/setup.cfg
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      886 2024-04-30 14:55:57.000000 python-ubercode-utils-2.0.0/setup.py
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2024-04-30 14:57:23.013424 python-ubercode-utils-2.0.0/test/
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)    10782 2023-10-26 21:59:32.000000 python-ubercode-utils-2.0.0/test/test_convert.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     2712 2023-03-09 19:13:29.000000 python-ubercode-utils-2.0.0/test/test_cursor.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     4975 2024-04-30 14:55:57.000000 python-ubercode-utils-2.0.0/test/test_data.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1234 2023-04-13 22:45:39.000000 python-ubercode-utils-2.0.0/test/test_dataframe.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     5657 2023-04-13 22:45:39.000000 python-ubercode-utils-2.0.0/test/test_environment.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     2855 2023-03-06 19:22:56.000000 python-ubercode-utils-2.0.0/test/test_logging.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     7807 2024-01-22 17:03:36.000000 python-ubercode-utils-2.0.0/test/test_urls.py
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2024-04-30 14:57:23.013424 python-ubercode-utils-2.0.0/ubercode/
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        0 2023-03-06 19:22:56.000000 python-ubercode-utils-2.0.0/ubercode/__init__.py
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2024-04-30 14:57:23.013424 python-ubercode-utils-2.0.0/ubercode/utils/
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        0 2023-03-06 19:22:56.000000 python-ubercode-utils-2.0.0/ubercode/utils/__init__.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)    11371 2024-04-30 14:55:57.000000 python-ubercode-utils-2.0.0/ubercode/utils/convert.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1118 2023-03-06 19:22:56.000000 python-ubercode-utils-2.0.0/ubercode/utils/cursor.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     4348 2024-04-30 14:55:57.000000 python-ubercode-utils-2.0.0/ubercode/utils/data.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      870 2023-04-03 13:13:43.000000 python-ubercode-utils-2.0.0/ubercode/utils/dataframe.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)    10854 2023-04-13 22:45:39.000000 python-ubercode-utils-2.0.0/ubercode/utils/environment.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     9199 2023-03-06 22:18:08.000000 python-ubercode-utils-2.0.0/ubercode/utils/logging.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     9652 2024-01-22 16:47:46.000000 python-ubercode-utils-2.0.0/ubercode/utils/urls.py
```

### Comparing `python-ubercode-utils-1.0.9/LICENSE` & `python-ubercode-utils-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.9/PKG-INFO` & `python-ubercode-utils-2.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ubercode-utils
-Version: 1.0.9
+Version: 2.0.0
 Summary: Core python utilities for all apps
 Home-page: https://github.com/sstacha/python-ubercode-utils
 Author: Steve Stacha
 Author-email: sstacha@gmail.com
 License: MIT
 Description: # python-ubercode-utils
         Extracting common python utilities re-used between all projects.  The intent is to have minimal dependencies
```

### Comparing `python-ubercode-utils-1.0.9/README.md` & `python-ubercode-utils-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.9/python_ubercode_utils.egg-info/PKG-INFO` & `python-ubercode-utils-2.0.0/python_ubercode_utils.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ubercode-utils
-Version: 1.0.9
+Version: 2.0.0
 Summary: Core python utilities for all apps
 Home-page: https://github.com/sstacha/python-ubercode-utils
 Author: Steve Stacha
 Author-email: sstacha@gmail.com
 License: MIT
 Description: # python-ubercode-utils
         Extracting common python utilities re-used between all projects.  The intent is to have minimal dependencies
```

### Comparing `python-ubercode-utils-1.0.9/python_ubercode_utils.egg-info/SOURCES.txt` & `python-ubercode-utils-2.0.0/python_ubercode_utils.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,23 +5,21 @@
 python_ubercode_utils.egg-info/PKG-INFO
 python_ubercode_utils.egg-info/SOURCES.txt
 python_ubercode_utils.egg-info/dependency_links.txt
 python_ubercode_utils.egg-info/not-zip-safe
 python_ubercode_utils.egg-info/top_level.txt
 test/test_convert.py
 test/test_cursor.py
+test/test_data.py
 test/test_dataframe.py
 test/test_environment.py
-test/test_json.py
 test/test_logging.py
 test/test_urls.py
-test/test_xml.py
 ubercode/__init__.py
 ubercode/utils/__init__.py
 ubercode/utils/convert.py
 ubercode/utils/cursor.py
+ubercode/utils/data.py
 ubercode/utils/dataframe.py
 ubercode/utils/environment.py
-ubercode/utils/json.py
 ubercode/utils/logging.py
-ubercode/utils/urls.py
-ubercode/utils/xml.py
+ubercode/utils/urls.py
```

### Comparing `python-ubercode-utils-1.0.9/setup.py` & `python-ubercode-utils-2.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(name='python-ubercode-utils',
-      version='1.0.9',
+      version='2.0.0',
       description='Core python utilities for all apps',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/sstacha/python-ubercode-utils',
       author='Steve Stacha',
       author_email='sstacha@gmail.com',
       license='MIT',
```

### Comparing `python-ubercode-utils-1.0.9/test/test_convert.py` & `python-ubercode-utils-2.0.0/test/test_convert.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.9/test/test_cursor.py` & `python-ubercode-utils-2.0.0/test/test_cursor.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.9/test/test_dataframe.py` & `python-ubercode-utils-2.0.0/test/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.9/test/test_environment.py` & `python-ubercode-utils-2.0.0/test/test_environment.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.9/test/test_logging.py` & `python-ubercode-utils-2.0.0/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.9/test/test_urls.py` & `python-ubercode-utils-2.0.0/test/test_urls.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,14 +36,24 @@
         self.assertEqual(test_uri, str(parsed_url))
         # test domain uri with default_scheme returns fully qualified url
         test_uri = "//ex.org/?id=1&b=2"
         parsed_url = ParsedUrl(test_uri)
         self.assertEqual(test_uri, str(parsed_url))
         parsed_url = ParsedUrl(test_uri, default_scheme='https')
         self.assertEqual("https:" + test_uri, str(parsed_url))
+        # test that mailto and tel links don't get defaulted
+        test_uri = 'mailto:me@mail.com?subject=mysubject&body=mybody'
+        parsed_url = ParsedUrl(test_uri, default_scheme='http', default_netloc='localhost:8000', default_filepath='/booger/')
+        self.assertEqual("mailto", str(parsed_url.scheme))
+        self.assertEqual(test_uri, parsed_url.url)
+        test_uri = 'tel: 222.222.2222'
+        parsed_url = ParsedUrl(test_uri, default_scheme='http', default_netloc='localhost:8000', default_filepath='/booger/')
+        self.assertEqual("tel", str(parsed_url.scheme))
+        self.assertEqual(test_uri, parsed_url.url)
+
 
     # --- basic retrieval
     # -------------------
     # NOTE: not testing the base parsed value from urllib only differences
     def test_retrieval(self):
         # hostname is domain instead; but can be gotten from raw property and are equal
         test_uri = "/?id=1&b=2"
```

### Comparing `python-ubercode-utils-1.0.9/ubercode/utils/convert.py` & `python-ubercode-utils-2.0.0/ubercode/utils/convert.py`

 * *Files 12% similar despite different names*

```diff
@@ -246,7 +246,35 @@
         _mask = value[:_iqtr]
         # append the masked values (length - iqtr * 2)
         _mask += "*" * (len(value) - (_iqtr * 2))
         # append the last quarter of the values up to 6 unmasked
         _mask += value[-_iqtr:]
     return _mask
 
+def obj_to_str(obj, property_filter_list=None):
+    """
+    Mostly used for debugging.  Very useful to print the properties of an object on a line; condensing reasonably
+
+    :param obj: the object to inspect properties for
+    :param property_filter_list: any property names we want to omit
+    :return: a string containing the outputted properties
+    """
+    attbuf = ""
+    for key, value in vars(obj).items():
+        if property_filter_list and key in property_filter_list:
+            continue
+        if not key.startswith('__'):
+            if len(attbuf) > 0:
+                attbuf += ", "
+            # show the first 50 chars and last 25 chars
+            this_content = str(value)
+            this_content = this_content.replace('\n', ' ').replace('\r', '').strip()
+            if this_content:
+                if len(this_content) > 150:
+                    attbuf += str(key) + ": [" + this_content[0:25] + " ... " + this_content[
+                                                                                len(this_content) - 25:len(
+                                                                                    this_content)] + "]"
+                else:
+                    attbuf += str(key) + ": " + this_content or ""
+            else:
+                attbuf += str(key) + ": " + this_content or ""
+    return "[" + attbuf + "]"
```

### Comparing `python-ubercode-utils-1.0.9/ubercode/utils/cursor.py` & `python-ubercode-utils-2.0.0/ubercode/utils/cursor.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.9/ubercode/utils/dataframe.py` & `python-ubercode-utils-2.0.0/ubercode/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.9/ubercode/utils/environment.py` & `python-ubercode-utils-2.0.0/ubercode/utils/environment.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.9/ubercode/utils/logging.py` & `python-ubercode-utils-2.0.0/ubercode/utils/logging.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.9/ubercode/utils/urls.py` & `python-ubercode-utils-2.0.0/ubercode/utils/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,34 +60,34 @@
     def __init__(self, url: str, default_netloc: str = None, default_scheme: str = None,
                  default_filepath: str = None, allow_fragments: bool = True, symlinks=False):
         self.original_url = url
         if self.url_filter(url) is None or len(self.url_filter(url)) == 0:
             raise Exception(
                 f'Attempted to parse [{str(self.url_filter(url))}].  Url parameter must exist and be a relative or absolute url after filtering!')
         self.parsed = urlsplit(self.url_filter(url), default_scheme or "", allow_fragments=allow_fragments)
-        if default_netloc and not self.parsed.netloc:
+        if default_scheme and not self.parsed.scheme and self.netloc:
+            self.scheme = default_scheme
+        if default_netloc and not self.parsed.netloc and self.scheme in ["http", "https", ""]:
             self.netloc = default_netloc
-        if default_filepath and default_filepath not in self.filepath:
+        if default_filepath and default_filepath not in self.filepath and self.scheme in ["http", "https", ""]:
             # we have a parent path we need to append to the existing one
             new_path = str(PurePath(default_filepath, self.path))
             # note: I don't want .. since this is web urls; using normpath to remove them unless symlinks is true
             if not symlinks and '..' in new_path:
                 new_path = os.path.normpath(new_path)
             # PurePath always strips the last path.  If we had a path before appending lets add it back
             if self.path.endswith('/') and not new_path.endswith('/'):
                 new_path += '/'
             # if we only have the default path make sure we have a slash (since we know it is a path)
             #   note: PurePath will strip it off even if we send it
             if new_path.endswith(default_filepath) or new_path.endswith(default_filepath[:-1]) and not new_path.endswith('/'):
                 new_path += '/'
             self.path = new_path
-        if default_scheme and not self.parsed.scheme and self.netloc:
-            self.scheme = default_scheme
         # one last correction; if we have a scheme but no netloc lets omit the scheme so it doesn't give bad results
-        if not self.parsed.netloc and self.parsed.scheme:
+        if not self.parsed.netloc and self.parsed.scheme and self.parsed.scheme in ['http', 'https']:
             self.parsed = self.parsed._replace(scheme='')
 
     @property
     def filepath(self):
         return os.path.dirname(self.parsed.path)
 
     @property
@@ -218,32 +218,36 @@
 
 
 if __name__ == "__main__":
     # test_uri = "http://localhost:8000/test1/?id=1&x=2"
     # parsed_url = ParsedUrl(test_uri)
     # print(f"root domain [{test_uri}]: {parsed_url.get_root_domain()}")
     # print(f"url:{parsed_url.url}")
-    # test_uri = "/?id=1&b=&c=3"
-    # parsed_url = ParsedUrl(test_uri, default_netloc='ex.org')
-    # print(f"root domain [{test_uri}]: {parsed_url.root_domain}")
-    # print(f"url:{parsed_url.url}")
-    # print(f"base: {parsed_url.base}")
-    # print(f"rel: {parsed_url.rel}")
+    test_uri = "/?id=1&b=&c=3"
+    parsed_url = ParsedUrl(test_uri, default_netloc='ex.org')
+    print(f"root domain [{test_uri}]: {parsed_url.root_domain}")
+    print(f"url:{parsed_url.url}")
+    print(f"base: {parsed_url.base}")
+    print(f"rel: {parsed_url.rel}")
     # print(f"url after base: {parsed_url.url}")
     # parsed_url.domain = "ex.org"
     # print(f"root domain [{str(parsed_url)}]: {parsed_url.root_domain}")
     # test_uri = "ex.org/"
     # print(f"root domain [{test_uri}]: {ParsedUrl(test_uri).root_domain}")
     # test_uri = "http://www.ex.org/go/"
     # print(f"root domain [{test_uri}]: {ParsedUrl(test_uri).root_domain}")
     # test_uri = "http://store.ex.org/go/"
     # print(f"root domain [{test_uri}]: {ParsedUrl(test_uri).root_domain}")
     # test_uri = "1.png"
     # print(f"test parent fragment only: {ParsedUrl(test_uri, default_netloc='localhost:8000', default_scheme='http', default_path='/mdb/')}")
     # test_uri = "#testproduct"
     # print(f"test parent fragment only: {ParsedUrl(test_uri, default_netloc='localhost:8000', default_scheme='http', default_path='/mdb/')}")
-    test_uri = "/products/"
-    purl = ParsedUrl(test_uri, default_scheme='http', default_netloc='localhost:8000', default_filepath='/blog')
-    print(purl)
-    test_uri = "../products/"
-    purl = ParsedUrl(test_uri, default_scheme='http', default_netloc='localhost:8000', default_filepath='/')
-    print(purl)
+    # test_uri = "/products/"
+    # purl = ParsedUrl(test_uri, default_scheme='http', default_netloc='localhost:8000', default_filepath='/blog')
+    # print(purl)
+    # test_uri = "../products/"
+    # purl = ParsedUrl(test_uri, default_scheme='http', default_netloc='localhost:8000', default_filepath='/')
+    # print(purl)
+    # # test mailto links
+    test_uri = 'mailto:me@mail.com?subject=mysubject&body=mybody'
+    purl = ParsedUrl(test_uri, default_scheme='http', default_netloc='localhost:8000')
+    print(purl)
```

