# Comparing `tmp/convert-us-to-uk-0.1.4.tar.gz` & `tmp/convert-us-to-uk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convert-us-to-uk-0.1.4.tar", last modified: Tue Apr 23 13:00:05 2024, max compression
+gzip compressed data, was "convert-us-to-uk-0.1.5.tar", last modified: Tue Apr 30 10:47:51 2024, max compression
```

## Comparing `convert-us-to-uk-0.1.4.tar` & `convert-us-to-uk-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 13:00:05.530028 convert-us-to-uk-0.1.4/
--rw-rw-rw-   0        0        0       43 2024-04-17 15:15:06.000000 convert-us-to-uk-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1990 2024-04-23 13:00:05.525588 convert-us-to-uk-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1660 2024-04-18 11:43:12.000000 convert-us-to-uk-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 13:00:05.500211 convert-us-to-uk-0.1.4/convert_us_to_uk/
--rw-rw-rw-   0        0        0        0 2024-04-17 12:42:42.000000 convert-us-to-uk-0.1.4/convert_us_to_uk/__init__.py
--rw-rw-rw-   0        0        0     1530 2024-04-18 11:33:40.000000 convert-us-to-uk-0.1.4/convert_us_to_uk/converter.py
--rw-rw-rw-   0        0        0    40125 2024-04-23 12:59:33.000000 convert-us-to-uk-0.1.4/convert_us_to_uk/us_to_uk_trans.csv
-drwxrwxrwx   0        0        0        0 2024-04-23 13:00:05.520366 convert-us-to-uk-0.1.4/convert_us_to_uk.egg-info/
--rw-rw-rw-   0        0        0     1990 2024-04-23 13:00:05.000000 convert-us-to-uk-0.1.4/convert_us_to_uk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2024-04-23 13:00:05.000000 convert-us-to-uk-0.1.4/convert_us_to_uk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 13:00:05.000000 convert-us-to-uk-0.1.4/convert_us_to_uk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-04-23 13:00:05.000000 convert-us-to-uk-0.1.4/convert_us_to_uk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-04-23 13:00:05.000000 convert-us-to-uk-0.1.4/convert_us_to_uk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 13:00:05.530028 convert-us-to-uk-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      696 2024-04-23 12:59:48.000000 convert-us-to-uk-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 13:00:05.524923 convert-us-to-uk-0.1.4/tests/
--rw-rw-rw-   0        0        0      296 2024-04-17 14:23:12.000000 convert-us-to-uk-0.1.4/tests/test_converter.py
+drwxrwxrwx   0        0        0        0 2024-04-30 10:47:51.171639 convert-us-to-uk-0.1.5/
+-rw-rw-rw-   0        0        0       43 2024-04-17 15:15:06.000000 convert-us-to-uk-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1990 2024-04-30 10:47:51.163532 convert-us-to-uk-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1660 2024-04-18 11:43:12.000000 convert-us-to-uk-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 10:47:51.002599 convert-us-to-uk-0.1.5/convert_us_to_uk/
+-rw-rw-rw-   0        0        0        0 2024-04-17 12:42:42.000000 convert-us-to-uk-0.1.5/convert_us_to_uk/__init__.py
+-rw-rw-rw-   0        0        0     1533 2024-04-30 10:34:39.000000 convert-us-to-uk-0.1.5/convert_us_to_uk/converter.py
+-rw-rw-rw-   0        0        0    40125 2024-04-23 12:59:33.000000 convert-us-to-uk-0.1.5/convert_us_to_uk/us_to_uk_trans.csv
+drwxrwxrwx   0        0        0        0 2024-04-30 10:47:51.140412 convert-us-to-uk-0.1.5/convert_us_to_uk.egg-info/
+-rw-rw-rw-   0        0        0     1990 2024-04-30 10:47:50.000000 convert-us-to-uk-0.1.5/convert_us_to_uk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2024-04-30 10:47:50.000000 convert-us-to-uk-0.1.5/convert_us_to_uk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 10:47:50.000000 convert-us-to-uk-0.1.5/convert_us_to_uk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-04-30 10:47:50.000000 convert-us-to-uk-0.1.5/convert_us_to_uk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-04-30 10:47:50.000000 convert-us-to-uk-0.1.5/convert_us_to_uk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 10:47:51.176559 convert-us-to-uk-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      696 2024-04-30 10:37:08.000000 convert-us-to-uk-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 10:47:51.146749 convert-us-to-uk-0.1.5/tests/
+-rw-rw-rw-   0        0        0      296 2024-04-17 14:23:12.000000 convert-us-to-uk-0.1.5/tests/test_converter.py
```

### Comparing `convert-us-to-uk-0.1.4/PKG-INFO` & `convert-us-to-uk-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convert-us-to-uk
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simple utility to convert US spelling to UK spelling.
 Home-page: https://github.com/oliverblane/convert-us-to-uk/tree/main
 Author: Oliver Blane
 Author-email: oliverblane72@gmail.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `convert-us-to-uk-0.1.4/README.md` & `convert-us-to-uk-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `convert-us-to-uk-0.1.4/convert_us_to_uk/converter.py` & `convert-us-to-uk-0.1.5/convert_us_to_uk/converter.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     output = text
     for word in set(words):  # we only need to replace each unique word once, so we use a set
         word_lower = word.lower()  # handle case insensitivity
         if word_lower in spelling_dict:
             # Create a case-matched replacement
             replacement = match_case(word, spelling_dict[word_lower])
             # Replace keeping the same case (assuming all dictionary entries are lowercase)
-            output = re.sub(r'\b' + re.escape(word) + r'\b', replacement, output, flags=re.IGNORECASE)
+            output = re.sub(r'\b' + re.escape(word) + r'\b', replacement, output) # , flags=re.IGNORECASE
 
     return output
 
 
 def match_case(word, replacement):
     """ Adjust the case of the replacement to match the input word """
     if word.isupper():
```

### Comparing `convert-us-to-uk-0.1.4/convert_us_to_uk/us_to_uk_trans.csv` & `convert-us-to-uk-0.1.5/convert_us_to_uk/us_to_uk_trans.csv`

 * *Files identical despite different names*

### Comparing `convert-us-to-uk-0.1.4/convert_us_to_uk.egg-info/PKG-INFO` & `convert-us-to-uk-0.1.5/convert_us_to_uk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convert-us-to-uk
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simple utility to convert US spelling to UK spelling.
 Home-page: https://github.com/oliverblane/convert-us-to-uk/tree/main
 Author: Oliver Blane
 Author-email: oliverblane72@gmail.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `convert-us-to-uk-0.1.4/setup.py` & `convert-us-to-uk-0.1.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='convert-us-to-uk',
-    version='0.1.4',
+    version='0.1.5',
     packages=find_packages(),
     include_package_data=True,
     description='A simple utility to convert US spelling to UK spelling.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Oliver Blane',
     author_email='oliverblane72@gmail.com',
```

