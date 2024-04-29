# Comparing `tmp/diffforms-0.0.2.tar.gz` & `tmp/diffforms-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffforms-0.0.2.tar", last modified: Sun Apr 28 22:26:12 2024, max compression
+gzip compressed data, was "diffforms-0.0.21.tar", last modified: Mon Apr 29 08:52:48 2024, max compression
```

## Comparing `diffforms-0.0.2.tar` & `diffforms-0.0.21.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-28 22:26:12.826621 diffforms-0.0.2/
--rwxrwxrwx   0 root         (0) root         (0)      120 2024-04-25 21:40:15.000000 diffforms-0.0.2/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)      537 2024-04-28 22:26:12.826097 diffforms-0.0.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1479 2024-04-25 21:40:15.000000 diffforms-0.0.2/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-28 22:26:12.822614 diffforms-0.0.2/diffforms/
--rwxrwxrwx   0 root         (0) root         (0)       52 2024-04-25 21:40:15.000000 diffforms-0.0.2/diffforms/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    20219 2024-04-28 22:17:06.000000 diffforms-0.0.2/diffforms/core.py
--rwxrwxrwx   0 root         (0) root         (0)       22 2024-04-28 22:25:47.000000 diffforms-0.0.2/diffforms/release.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-28 22:26:12.825654 diffforms-0.0.2/diffforms.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      537 2024-04-28 22:26:12.000000 diffforms-0.0.2/diffforms.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      272 2024-04-28 22:26:12.000000 diffforms-0.0.2/diffforms.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-28 22:26:12.000000 diffforms-0.0.2/diffforms.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       42 2024-04-28 22:26:12.000000 diffforms-0.0.2/diffforms.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       10 2024-04-28 22:26:12.000000 diffforms-0.0.2/diffforms.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       41 2024-04-25 21:40:15.000000 diffforms-0.0.2/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-28 22:26:12.826704 diffforms-0.0.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      718 2024-04-25 21:40:15.000000 diffforms-0.0.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 08:52:48.448162 diffforms-0.0.21/
+-rwxrwxrwx   0 root         (0) root         (0)      120 2024-04-25 21:40:15.000000 diffforms-0.0.21/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)      538 2024-04-29 08:52:48.447636 diffforms-0.0.21/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1479 2024-04-25 21:40:15.000000 diffforms-0.0.21/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 08:52:48.443853 diffforms-0.0.21/diffforms/
+-rwxrwxrwx   0 root         (0) root         (0)       52 2024-04-25 21:40:15.000000 diffforms-0.0.21/diffforms/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    20230 2024-04-29 08:50:21.000000 diffforms-0.0.21/diffforms/core.py
+-rwxrwxrwx   0 root         (0) root         (0)       23 2024-04-29 08:52:40.000000 diffforms-0.0.21/diffforms/release.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 08:52:48.447041 diffforms-0.0.21/diffforms.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      538 2024-04-29 08:52:48.000000 diffforms-0.0.21/diffforms.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      272 2024-04-29 08:52:48.000000 diffforms-0.0.21/diffforms.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-29 08:52:48.000000 diffforms-0.0.21/diffforms.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       42 2024-04-29 08:52:48.000000 diffforms-0.0.21/diffforms.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       10 2024-04-29 08:52:48.000000 diffforms-0.0.21/diffforms.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       41 2024-04-25 21:40:15.000000 diffforms-0.0.21/requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-29 08:52:48.448252 diffforms-0.0.21/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      718 2024-04-25 21:40:15.000000 diffforms-0.0.21/setup.py
```

### Comparing `diffforms-0.0.2/PKG-INFO` & `diffforms-0.0.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffforms
-Version: 0.0.2
+Version: 0.0.21
 Summary: Symbolic differential forms python library
 Home-page: https://github.com/Bone5505/Differential-Forms
 Author: Adam Shaw
 Keywords: differential forms,sympy,polyforms,exterior derivative
 Requires-Dist: wheel>=0.43.0
 Requires-Dist: sympy>=1.12
 Requires-Dist: ipython>=8.19.0
```

### Comparing `diffforms-0.0.2/README.md` & `diffforms-0.0.21/README.md`

 * *Files identical despite different names*

### Comparing `diffforms-0.0.2/diffforms/core.py` & `diffforms-0.0.21/diffforms/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -459,15 +459,15 @@
         return ret
 
 
 def d(form):
     if isinstance(form,(DifferentialForm,DifferentialFormMul)):
         return form.d
     
-    elif isinstance(form,AtomicExpr):
+    elif isinstance(form,(AtomicExpr,Function)):
         ret = DifferentialFormMul()
         new_forms_list = []
         new_factors_list = []
         for f in form.free_symbols:
             dform = form.diff(f)
             if dform != 0:
                 new_forms_list += [[DifferentialForm(f,0).d]]
```

### Comparing `diffforms-0.0.2/diffforms.egg-info/PKG-INFO` & `diffforms-0.0.21/diffforms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffforms
-Version: 0.0.2
+Version: 0.0.21
 Summary: Symbolic differential forms python library
 Home-page: https://github.com/Bone5505/Differential-Forms
 Author: Adam Shaw
 Keywords: differential forms,sympy,polyforms,exterior derivative
 Requires-Dist: wheel>=0.43.0
 Requires-Dist: sympy>=1.12
 Requires-Dist: ipython>=8.19.0
```

### Comparing `diffforms-0.0.2/setup.py` & `diffforms-0.0.21/setup.py`

 * *Files identical despite different names*

