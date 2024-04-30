# Comparing `tmp/githc-0.1.3.tar.gz` & `tmp/githc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "githc-0.1.3.tar", last modified: Thu Apr 25 00:54:52 2024, max compression
+gzip compressed data, was "githc-0.2.0.tar", last modified: Tue Apr 30 16:48:27 2024, max compression
```

## Comparing `githc-0.1.3.tar` & `githc-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 chris.gravel   (502) staff       (20)        0 2024-04-25 00:54:52.268442 githc-0.1.3/
--rw-r--r--   0 chris.gravel   (502) staff       (20)     1055 2024-04-24 22:19:20.000000 githc-0.1.3/LICENSE.md
--rw-r--r--   0 chris.gravel   (502) staff       (20)        5 2024-04-24 22:19:20.000000 githc-0.1.3/MANIFEST.in
--rw-r--r--   0 chris.gravel   (502) staff       (20)      793 2024-04-25 00:54:52.268321 githc-0.1.3/PKG-INFO
--rw-r--r--   0 chris.gravel   (502) staff       (20)     1047 2024-04-24 22:19:20.000000 githc-0.1.3/README.md
--rwxr-xr-x   0 chris.gravel   (502) staff       (20)     5018 2024-04-25 00:51:40.000000 githc-0.1.3/gh.py
-drwxr-xr-x   0 chris.gravel   (502) staff       (20)        0 2024-04-25 00:54:52.267624 githc-0.1.3/githc.egg-info/
--rw-r--r--   0 chris.gravel   (502) staff       (20)      793 2024-04-25 00:54:52.000000 githc-0.1.3/githc.egg-info/PKG-INFO
--rw-r--r--   0 chris.gravel   (502) staff       (20)      205 2024-04-25 00:54:52.000000 githc-0.1.3/githc.egg-info/SOURCES.txt
--rw-r--r--   0 chris.gravel   (502) staff       (20)        1 2024-04-25 00:54:52.000000 githc-0.1.3/githc.egg-info/dependency_links.txt
--rw-r--r--   0 chris.gravel   (502) staff       (20)       31 2024-04-25 00:54:52.000000 githc-0.1.3/githc.egg-info/entry_points.txt
--rw-r--r--   0 chris.gravel   (502) staff       (20)        1 2024-04-25 00:54:52.000000 githc-0.1.3/githc.egg-info/top_level.txt
--rw-r--r--   0 chris.gravel   (502) staff       (20)       79 2024-04-25 00:54:52.268812 githc-0.1.3/setup.cfg
--rw-r--r--   0 chris.gravel   (502) staff       (20)      949 2024-04-25 00:52:50.000000 githc-0.1.3/setup.py
+drwxr-xr-x   0 chris.gravel   (502) staff       (20)        0 2024-04-30 16:48:27.119111 githc-0.2.0/
+-rw-r--r--   0 chris.gravel   (502) staff       (20)     1055 2024-04-24 22:19:20.000000 githc-0.2.0/LICENSE.md
+-rw-r--r--   0 chris.gravel   (502) staff       (20)        5 2024-04-24 22:19:20.000000 githc-0.2.0/MANIFEST.in
+-rw-r--r--   0 chris.gravel   (502) staff       (20)      793 2024-04-30 16:48:27.118864 githc-0.2.0/PKG-INFO
+-rw-r--r--   0 chris.gravel   (502) staff       (20)     1047 2024-04-24 22:19:20.000000 githc-0.2.0/README.md
+-rwxr-xr-x   0 chris.gravel   (502) staff       (20)     5492 2024-04-30 16:45:08.000000 githc-0.2.0/gh.py
+drwxr-xr-x   0 chris.gravel   (502) staff       (20)        0 2024-04-30 16:48:27.118185 githc-0.2.0/githc.egg-info/
+-rw-r--r--   0 chris.gravel   (502) staff       (20)      793 2024-04-30 16:48:27.000000 githc-0.2.0/githc.egg-info/PKG-INFO
+-rw-r--r--   0 chris.gravel   (502) staff       (20)      205 2024-04-30 16:48:27.000000 githc-0.2.0/githc.egg-info/SOURCES.txt
+-rw-r--r--   0 chris.gravel   (502) staff       (20)        1 2024-04-30 16:48:27.000000 githc-0.2.0/githc.egg-info/dependency_links.txt
+-rw-r--r--   0 chris.gravel   (502) staff       (20)       31 2024-04-30 16:48:27.000000 githc-0.2.0/githc.egg-info/entry_points.txt
+-rw-r--r--   0 chris.gravel   (502) staff       (20)        1 2024-04-30 16:48:27.000000 githc-0.2.0/githc.egg-info/top_level.txt
+-rw-r--r--   0 chris.gravel   (502) staff       (20)       79 2024-04-30 16:48:27.119753 githc-0.2.0/setup.cfg
+-rw-r--r--   0 chris.gravel   (502) staff       (20)      949 2024-04-30 16:45:56.000000 githc-0.2.0/setup.py
```

### Comparing `githc-0.1.3/LICENSE.md` & `githc-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `githc-0.1.3/PKG-INFO` & `githc-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: githc
-Version: 0.1.3
+Version: 0.2.0
 Summary: Git history checkout tool
 Home-page: https://github.com/cpagravel/gh
 Download-URL: https://github.com/cpagravel/gh/archive/0.1.3.tar.gz
 Author: Chris Gravel
 Author-email: cpagravel@gmail.com
 License: MIT
 Keywords: git,git history,git checkout,git workflow
```

### Comparing `githc-0.1.3/README.md` & `githc-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `githc-0.1.3/gh.py` & `githc-0.2.0/gh.py`

 * *Files 10% similar despite different names*

```diff
@@ -147,27 +147,40 @@
   group.add_argument(
       "-c",
       type=check_valid_ref(item_count),
       metavar="REF_INT",
       dest="checkout",
       help=("eq to " + Colors.colorize("git checkout ", Colors.GREEN) + Colors.colorize(
           "<BRANCH_REF>", Colors.RED)))
+  group.add_argument(
+      "-D",
+      type=check_valid_ref(item_count),
+      metavar="REF_INT",
+      dest="delete",
+      help=("eq to " + Colors.colorize("git branch -D ", Colors.GREEN) + Colors.colorize(
+          "<BRANCH_REF>", Colors.RED)))
 
   args = parser.parse_args()
 
   if args.debug:
     LOGGER.setLevel(logging.DEBUG)
 
   if args.REF is not None:  # print branch name
     LOGGER.info(checkout_history[args.REF])
   elif args.checkout is not None:  # checkout branch
     command = f"git checkout {checkout_history[args.checkout]}"
     (output, err) = bash(command)
     if err:
       LOGGER.error(err.decode())
     LOGGER.info(output.decode())
+  elif args.delete is not None:  # delete branch
+    command = f"git branch -D {checkout_history[args.delete]}"
+    (output, err) = bash(command)
+    if err:
+      LOGGER.error(err.decode())
+    LOGGER.info(output.decode())
   else:
     display_list(checkout_history, args.verbose)
 
 
 if __name__ == "__main__":
   main()
```

### Comparing `githc-0.1.3/githc.egg-info/PKG-INFO` & `githc-0.2.0/githc.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: githc
-Version: 0.1.3
+Version: 0.2.0
 Summary: Git history checkout tool
 Home-page: https://github.com/cpagravel/gh
 Download-URL: https://github.com/cpagravel/gh/archive/0.1.3.tar.gz
 Author: Chris Gravel
 Author-email: cpagravel@gmail.com
 License: MIT
 Keywords: git,git history,git checkout,git workflow
```

### Comparing `githc-0.1.3/setup.py` & `githc-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name="githc",
     packages={".": "githc"},
-    version="0.1.3",
+    version="0.2.0",
     license="MIT",
     description="Git history checkout tool",
     author="Chris Gravel",
     author_email="cpagravel@gmail.com",
     url="https://github.com/cpagravel/gh",
     download_url="https://github.com/cpagravel/gh/archive/0.1.3.tar.gz",
     keywords=["git", "git history", "git checkout", "git workflow"],
```

