# Comparing `tmp/static_analysis_script-0.1.9.tar.gz` & `tmp/static_analysis_script-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "static_analysis_script-0.1.9.tar", last modified: Mon Apr 29 08:50:18 2024, max compression
+gzip compressed data, was "static_analysis_script-0.2.0.tar", last modified: Tue Apr 30 17:34:41 2024, max compression
```

## Comparing `static_analysis_script-0.1.9.tar` & `static_analysis_script-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 08:50:18.017592 static_analysis_script-0.1.9/
--rw-rw-rw-   0        0        0     2318 2024-04-29 08:50:18.017592 static_analysis_script-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     1579 2024-04-29 08:47:54.000000 static_analysis_script-0.1.9/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 08:50:18.017592 static_analysis_script-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1594 2024-04-29 08:48:32.000000 static_analysis_script-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 08:50:17.991081 static_analysis_script-0.1.9/src/
-drwxrwxrwx   0        0        0        0 2024-04-29 08:50:17.993083 static_analysis_script-0.1.9/src/analysis/
--rw-rw-rw-   0        0        0        0 2024-04-29 08:47:54.000000 static_analysis_script-0.1.9/src/analysis/__init__.py
--rw-rw-rw-   0        0        0    11818 2024-04-29 08:47:13.000000 static_analysis_script-0.1.9/src/analysis/main.py
-drwxrwxrwx   0        0        0        0 2024-04-29 08:50:17.996080 static_analysis_script-0.1.9/src/bin/
--rwxrwxrwx   0        0        0   370056 2024-04-29 08:47:54.000000 static_analysis_script-0.1.9/src/bin/strings.exe
-drwxrwxrwx   0        0        0        0 2024-04-29 08:50:18.016592 static_analysis_script-0.1.9/src/static_analysis_script.egg-info/
--rw-rw-rw-   0        0        0     2318 2024-04-29 08:50:17.000000 static_analysis_script-0.1.9/src/static_analysis_script.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2024-04-29 08:50:17.000000 static_analysis_script-0.1.9/src/static_analysis_script.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 08:50:17.000000 static_analysis_script-0.1.9/src/static_analysis_script.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-29 08:50:17.000000 static_analysis_script-0.1.9/src/static_analysis_script.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       18 2024-04-29 08:50:17.000000 static_analysis_script-0.1.9/src/static_analysis_script.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-29 08:50:17.000000 static_analysis_script-0.1.9/src/static_analysis_script.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 17:34:41.577360 static_analysis_script-0.2.0/
+-rw-rw-rw-   0        0        0     2318 2024-04-30 17:34:41.576360 static_analysis_script-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1579 2024-04-30 17:32:58.000000 static_analysis_script-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-30 17:34:41.577360 static_analysis_script-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1594 2024-04-30 17:28:52.000000 static_analysis_script-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 17:34:41.560354 static_analysis_script-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-30 17:34:41.562354 static_analysis_script-0.2.0/src/analysis/
+-rw-rw-rw-   0        0        0        0 2024-04-30 17:32:58.000000 static_analysis_script-0.2.0/src/analysis/__init__.py
+-rw-rw-rw-   0        0        0    11843 2024-04-30 17:27:30.000000 static_analysis_script-0.2.0/src/analysis/main.py
+drwxrwxrwx   0        0        0        0 2024-04-30 17:34:41.565355 static_analysis_script-0.2.0/src/bin/
+-rwxrwxrwx   0        0        0   370056 2024-04-30 17:32:58.000000 static_analysis_script-0.2.0/src/bin/strings.exe
+drwxrwxrwx   0        0        0        0 2024-04-30 17:34:41.576360 static_analysis_script-0.2.0/src/static_analysis_script.egg-info/
+-rw-rw-rw-   0        0        0     2318 2024-04-30 17:34:41.000000 static_analysis_script-0.2.0/src/static_analysis_script.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2024-04-30 17:34:41.000000 static_analysis_script-0.2.0/src/static_analysis_script.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 17:34:41.000000 static_analysis_script-0.2.0/src/static_analysis_script.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-30 17:34:41.000000 static_analysis_script-0.2.0/src/static_analysis_script.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       18 2024-04-30 17:34:41.000000 static_analysis_script-0.2.0/src/static_analysis_script.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-30 17:34:41.000000 static_analysis_script-0.2.0/src/static_analysis_script.egg-info/top_level.txt
```

### Comparing `static_analysis_script-0.1.9/PKG-INFO` & `static_analysis_script-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-analysis-script
-Version: 0.1.9
+Version: 0.2.0
 Summary: A utility to perform static analysis on files.
 Home-page: https://github.com/perzibel/static-analysis-script
 Author: Perzibel
 Author-email: perzibel@outlook.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Security
```

### Comparing `static_analysis_script-0.1.9/README.md` & `static_analysis_script-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `static_analysis_script-0.1.9/setup.py` & `static_analysis_script-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Used for the long_description. It's nice to have this in the setup file so
 # that the distribution will have a more comprehensive description.
 def read(file_name):
     return open(os.path.join(os.path.dirname(__file__), file_name)).read()
 
 setup(
     name='static-analysis-script',
-    version='0.1.9',
+    version='0.2.0',
     author='Perzibel',
     author_email='perzibel@outlook.com',
     description='A utility to perform static analysis on files.',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',  # This is important for rendering Markdown from README
     url='https://github.com/perzibel/static-analysis-script',
     packages=find_packages(where="src"),
```

### Comparing `static_analysis_script-0.1.9/src/analysis/main.py` & `static_analysis_script-0.2.0/src/analysis/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,16 +260,15 @@
           "Usage: main.py <file_path> <option> \n"
           "Available Options:\n"
           "-u, -U    Show only unique values from the extracted strings. \n"
           "-e, -E    Print out the entropy calculation only. \n"
           "-c, -C    Print certificate information, including supplementary details. \n\n"
           "for more information or requests, please visit the project repository. ")
 
-
-if __name__ == "__main__":
+def main():
     import sys
 
     num_args = len(sys.argv)
     if num_args == 2 or num_args == 3:
         UserInput = sys.argv[1]
         try:
             clean_path = UserInput.replace('"', "")
@@ -307,7 +306,11 @@
                     print("\n Urls:", findings[4])
             else:
                 print("file doesn't exists, please read main.py -h for further explanation")
         except Exception as e:
             print("\n ----- error: ", e, " ---------")
     else:
         print("\n please enter main.py -h to see help")
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `static_analysis_script-0.1.9/src/bin/strings.exe` & `static_analysis_script-0.2.0/src/bin/strings.exe`

 * *Files identical despite different names*

### Comparing `static_analysis_script-0.1.9/src/static_analysis_script.egg-info/PKG-INFO` & `static_analysis_script-0.2.0/src/static_analysis_script.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-analysis-script
-Version: 0.1.9
+Version: 0.2.0
 Summary: A utility to perform static analysis on files.
 Home-page: https://github.com/perzibel/static-analysis-script
 Author: Perzibel
 Author-email: perzibel@outlook.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Security
```

