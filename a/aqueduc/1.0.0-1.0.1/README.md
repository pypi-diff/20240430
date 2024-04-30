# Comparing `tmp/aqueduc-1.0.0.tar.gz` & `tmp/aqueduc-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqueduc-1.0.0.tar", last modified: Mon Apr 29 14:54:40 2024, max compression
+gzip compressed data, was "aqueduc-1.0.1.tar", last modified: Tue Apr 30 10:47:22 2024, max compression
```

## Comparing `aqueduc-1.0.0.tar` & `aqueduc-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mozenn    (1000) mozenn    (1000)        0 2024-04-29 14:54:40.415704 aqueduc-1.0.0/
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)     1071 2024-04-29 14:32:26.000000 aqueduc-1.0.0/LICENSE
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)     2931 2024-04-29 14:54:40.415704 aqueduc-1.0.0/PKG-INFO
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)     1585 2024-04-29 14:32:26.000000 aqueduc-1.0.0/README.md
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)      416 2024-04-29 14:32:26.000000 aqueduc-1.0.0/pyproject.toml
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)       38 2024-04-29 14:54:40.415704 aqueduc-1.0.0/setup.cfg
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)       37 2024-04-29 14:32:26.000000 aqueduc-1.0.0/setup.py
-drwxr-xr-x   0 mozenn    (1000) mozenn    (1000)        0 2024-04-29 14:54:40.415704 aqueduc-1.0.0/src/
-drwxr-xr-x   0 mozenn    (1000) mozenn    (1000)        0 2024-04-29 14:54:40.415704 aqueduc-1.0.0/src/aqueduc.egg-info/
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)     2931 2024-04-29 14:54:40.000000 aqueduc-1.0.0/src/aqueduc.egg-info/PKG-INFO
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)      246 2024-04-29 14:54:40.000000 aqueduc-1.0.0/src/aqueduc.egg-info/SOURCES.txt
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)        1 2024-04-29 14:54:40.000000 aqueduc-1.0.0/src/aqueduc.egg-info/dependency_links.txt
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)       49 2024-04-29 14:54:40.000000 aqueduc-1.0.0/src/aqueduc.egg-info/entry_points.txt
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)       13 2024-04-29 14:54:40.000000 aqueduc-1.0.0/src/aqueduc.egg-info/top_level.txt
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)     4583 2024-04-29 14:32:26.000000 aqueduc-1.0.0/src/aqueduc.py
--rw-r--r--   0 mozenn    (1000) mozenn    (1000)     2793 2024-04-29 14:32:26.000000 aqueduc-1.0.0/src/test.py
+drwxr-xr-x   0 mozenn    (1000) mozenn    (1000)        0 2024-04-30 10:47:22.532933 aqueduc-1.0.1/
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)     1051 2024-04-30 10:37:44.000000 aqueduc-1.0.1/LICENSE
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)     2871 2024-04-30 10:47:22.532933 aqueduc-1.0.1/PKG-INFO
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)     1585 2024-04-29 14:32:26.000000 aqueduc-1.0.1/README.md
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)      362 2024-04-30 10:38:45.000000 aqueduc-1.0.1/pyproject.toml
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)       38 2024-04-30 10:47:22.532933 aqueduc-1.0.1/setup.cfg
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)       37 2024-04-29 14:32:26.000000 aqueduc-1.0.1/setup.py
+drwxr-xr-x   0 mozenn    (1000) mozenn    (1000)        0 2024-04-30 10:47:22.532933 aqueduc-1.0.1/src/
+drwxr-xr-x   0 mozenn    (1000) mozenn    (1000)        0 2024-04-30 10:47:22.532933 aqueduc-1.0.1/src/aqueduc.egg-info/
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)     2871 2024-04-30 10:47:22.000000 aqueduc-1.0.1/src/aqueduc.egg-info/PKG-INFO
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)      246 2024-04-30 10:47:22.000000 aqueduc-1.0.1/src/aqueduc.egg-info/SOURCES.txt
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)        1 2024-04-30 10:47:22.000000 aqueduc-1.0.1/src/aqueduc.egg-info/dependency_links.txt
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)       50 2024-04-30 10:47:22.000000 aqueduc-1.0.1/src/aqueduc.egg-info/entry_points.txt
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)       13 2024-04-30 10:47:22.000000 aqueduc-1.0.1/src/aqueduc.egg-info/top_level.txt
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)     4583 2024-04-29 14:32:26.000000 aqueduc-1.0.1/src/aqueduc.py
+-rw-r--r--   0 mozenn    (1000) mozenn    (1000)     2793 2024-04-29 15:04:50.000000 aqueduc-1.0.1/src/test.py
```

### Comparing `aqueduc-1.0.0/LICENSE` & `aqueduc-1.0.1/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-Copyright 2020 Gauthier Cassany
+Copyright 2024
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, 
-including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction,
+including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, 
-INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. 
-IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, 
-TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED,
+INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
+TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `aqueduc-1.0.0/PKG-INFO` & `aqueduc-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: aqueduc
-Version: 1.0.0
-Summary: Read the latest Real Python tutorials
+Version: 1.0.1
 Author: Mozenn
-License: Copyright 2020 Gauthier Cassany
+License: Copyright 2024
         
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, 
-        including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction,
+        including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
         and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, 
-        INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. 
-        IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, 
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED,
+        INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+        IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
         TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+        
 Project-URL: Homepage, https://github.com/Mozenn/aqueduc
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Aqueduc
 
 Aqueduc is a small script used to move or copy files and folders using preconfigured parameters.\
```

### Comparing `aqueduc-1.0.0/README.md` & `aqueduc-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `aqueduc-1.0.0/src/aqueduc.egg-info/PKG-INFO` & `aqueduc-1.0.1/src/aqueduc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: aqueduc
-Version: 1.0.0
-Summary: Read the latest Real Python tutorials
+Version: 1.0.1
 Author: Mozenn
-License: Copyright 2020 Gauthier Cassany
+License: Copyright 2024
         
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, 
-        including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
+        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction,
+        including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
         and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, 
-        INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. 
-        IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, 
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED,
+        INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+        IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
         TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+        
 Project-URL: Homepage, https://github.com/Mozenn/aqueduc
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Aqueduc
 
 Aqueduc is a small script used to move or copy files and folders using preconfigured parameters.\
```

### Comparing `aqueduc-1.0.0/src/aqueduc.py` & `aqueduc-1.0.1/src/aqueduc.py`

 * *Files identical despite different names*

### Comparing `aqueduc-1.0.0/src/test.py` & `aqueduc-1.0.1/src/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         self.create_test_file(file_path)
         self.assertEqual(aqueduc.file_toolarge(file_path, {"size_limit": 1000}), False, "Should not be too large")
         os.remove(file_path)
 
     def test_file_not_modified_since_date(self):
         file_path = "test.txt"
         self.create_test_file(file_path)
-        self.assertEqual(aqueduc.file_not_modified_since_date(file_path, {"last_date_allowed": "27 04 2024 10"}), True, "Should not have been modified since date")
+        self.assertEqual(aqueduc.file_not_modified_since_date(file_path, {"last_date_allowed": "27 04 2124 10"}), True, "Should not have been modified since date")
         os.remove(file_path)
 
     def test_file_modified_since_date(self):
         file_path = "test.txt"
         self.create_test_file(file_path)
         self.assertEqual(aqueduc.file_not_modified_since_date(file_path, {"last_date_allowed": "25 04 2024 10"}), False, "Should have been modified since date")
         os.remove(file_path)
```

