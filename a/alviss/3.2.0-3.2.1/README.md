# Comparing `tmp/alviss-3.2.0.tar.gz` & `tmp/alviss-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alviss-3.2.0.tar", last modified: Mon Apr 22 11:41:08 2024, max compression
+gzip compressed data, was "alviss-3.2.1.tar", last modified: Tue Apr 30 10:09:22 2024, max compression
```

## Comparing `alviss-3.2.0.tar` & `alviss-3.2.1.tar`

### file list

```diff
@@ -1,52 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:41:08.136387 alviss-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-22 11:40:58.000000 alviss-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-04-22 11:41:08.136387 alviss-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10661 2024-04-22 11:40:58.000000 alviss-3.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:41:08.128387 alviss-3.2.0/alviss/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-22 11:40:58.000000 alviss-3.2.0/alviss/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:41:08.132387 alviss-3.2.0/alviss/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:40:58.000000 alviss-3.2.0/alviss/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:41:08.132387 alviss-3.2.0/alviss/cli/render/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:40:58.000000 alviss-3.2.0/alviss/cli/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-22 11:40:58.000000 alviss-3.2.0/alviss/cli/render/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:41:08.132387 alviss-3.2.0/alviss/cli/stubber/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:40:58.000000 alviss-3.2.0/alviss/cli/stubber/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-22 11:40:58.000000 alviss-3.2.0/alviss/cli/stubber/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:41:08.132387 alviss-3.2.0/alviss/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-22 11:40:58.000000 alviss-3.2.0/alviss/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-22 11:40:58.000000 alviss-3.2.0/alviss/loaders/autoloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    17478 2024-04-22 11:40:58.000000 alviss-3.2.0/alviss/loaders/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-22 11:40:58.000000 alviss-3.2.0/alviss/loaders/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-22 11:40:58.000000 alviss-3.2.0/alviss/loaders/jsonfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-22 11:40:58.000000 alviss-3.2.0/alviss/loaders/yamlfile.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-22 11:40:58.000000 alviss-3.2.0/alviss/quickloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:41:08.132387 alviss-3.2.0/alviss/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 11:40:58.000000 alviss-3.2.0/alviss/renderers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:41:08.132387 alviss-3.2.0/alviss/renderers/static/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-22 11:40:58.000000 alviss-3.2.0/alviss/renderers/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-22 11:40:58.000000 alviss-3.2.0/alviss/renderers/static/_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-22 11:40:58.000000 alviss-3.2.0/alviss/renderers/static/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:41:08.132387 alviss-3.2.0/alviss/structs/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-22 11:40:58.000000 alviss-3.2.0/alviss/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-22 11:40:58.000000 alviss-3.2.0/alviss/structs/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-22 11:40:58.000000 alviss-3.2.0/alviss/structs/baseconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-22 11:40:58.000000 alviss-3.2.0/alviss/structs/cfgstub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-22 11:40:58.000000 alviss-3.2.0/alviss/structs/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-22 11:40:58.000000 alviss-3.2.0/alviss/structs/singletonconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:41:08.132387 alviss-3.2.0/alviss/stubber/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-22 11:40:58.000000 alviss-3.2.0/alviss/stubber/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:41:08.136387 alviss-3.2.0/alviss/stubber/stubmaker/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-22 11:40:58.000000 alviss-3.2.0/alviss/stubber/stubmaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-22 11:40:58.000000 alviss-3.2.0/alviss/stubber/stubmaker/_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)    10023 2024-04-22 11:40:58.000000 alviss-3.2.0/alviss/stubber/stubmaker/_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-22 11:40:58.000000 alviss-3.2.0/alviss/stubber/stubmaker/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:41:08.136387 alviss-3.2.0/alviss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-04-22 11:41:08.000000 alviss-3.2.0/alviss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-22 11:41:08.000000 alviss-3.2.0/alviss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 11:41:08.000000 alviss-3.2.0/alviss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-22 11:41:08.000000 alviss-3.2.0/alviss.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-22 11:41:08.000000 alviss-3.2.0/alviss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-22 11:41:08.000000 alviss-3.2.0/alviss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-22 11:40:58.000000 alviss-3.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 11:41:08.136387 alviss-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-22 11:40:58.000000 alviss-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:22.769177 alviss-3.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-30 10:09:12.000000 alviss-3.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-04-30 10:09:22.769177 alviss-3.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10661 2024-04-30 10:09:12.000000 alviss-3.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:22.761177 alviss-3.2.1/alviss/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:22.761177 alviss-3.2.1/alviss/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:22.761177 alviss-3.2.1/alviss/cli/render/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/cli/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/cli/render/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:22.761177 alviss-3.2.1/alviss/cli/stubber/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/cli/stubber/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/cli/stubber/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:22.765177 alviss-3.2.1/alviss/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/loaders/autoloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17478 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/loaders/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/loaders/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/loaders/jsonfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/loaders/yamlfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/quickloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:22.765177 alviss-3.2.1/alviss/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/renderers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:22.765177 alviss-3.2.1/alviss/renderers/static/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/renderers/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/renderers/static/_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/renderers/static/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:22.765177 alviss-3.2.1/alviss/structs/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/structs/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/structs/baseconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/structs/cfgstub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/structs/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/structs/singletonconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:22.765177 alviss-3.2.1/alviss/stubber/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/stubber/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:22.769177 alviss-3.2.1/alviss/stubber/stubmaker/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/stubber/stubmaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/stubber/stubmaker/_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10606 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/stubber/stubmaker/_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/stubber/stubmaker/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:22.769177 alviss-3.2.1/alviss/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-30 10:09:12.000000 alviss-3.2.1/alviss/utils/kwfields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:22.769177 alviss-3.2.1/alviss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-04-30 10:09:22.000000 alviss-3.2.1/alviss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-30 10:09:22.000000 alviss-3.2.1/alviss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 10:09:22.000000 alviss-3.2.1/alviss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-30 10:09:22.000000 alviss-3.2.1/alviss.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 10:09:22.000000 alviss-3.2.1/alviss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-30 10:09:22.000000 alviss-3.2.1/alviss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-30 10:09:12.000000 alviss-3.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 10:09:22.769177 alviss-3.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-30 10:09:12.000000 alviss-3.2.1/setup.py
```

### Comparing `alviss-3.2.0/LICENSE` & `alviss-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alviss-3.2.0/PKG-INFO` & `alviss-3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alviss
-Version: 3.2.0
+Version: 3.2.1
 Summary: Configuration file reader with some nifty bells and whistles added
 Author-email: Thordur Matthiasson <thordurm@ccpgames.com>
 License: MIT License
         
         Copyright (c) 2019-2024 CCP Games
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `alviss-3.2.0/README.md` & `alviss-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `alviss-3.2.0/alviss/cli/render/main.py` & `alviss-3.2.1/alviss/cli/render/main.py`

 * *Files identical despite different names*

### Comparing `alviss-3.2.0/alviss/cli/stubber/main.py` & `alviss-3.2.1/alviss/cli/stubber/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,14 +10,19 @@
     parser = argparse.ArgumentParser(description='Generates Python dataclass stubs based on the given alviss type descriptor file.',
                                      epilog=f'Alviss version {version}')
 
     parser.add_argument('file', help='The Alviss config type descriptor file to generate strubs from.')
     parser.add_argument('-o', '--output', help='File to write the generated stub code to (otherwise its just printed to stdout)',
                         default='', nargs='?')
     parser.add_argument('-f', '--force-overwrite', help='Overwrite existing output file if it exists', action='store_true')
+    parser.add_argument('-n', '--class-name',
+                        help='The name of the resulting "final" stub class generated when outputting to a file (default is "AlvissConfigStub"). Set to "None" to skip generating the "final" class.',
+                        default='AlvissConfigStub')
+    parser.add_argument('-x', '--export-all', help='Make all stub class names public and export via __all__ when outputting to a file.',
+                        action='store_true')
 
     loudness_group = parser.add_mutually_exclusive_group()
     loudness_group.add_argument('-s', '--silent', action='store_true',
                                 help='Only outputs the resulting rendered code (and errors print to stderr)')
     loudness_group.add_argument('-v', '--verbose', action="store_true",
                                 help='Spits out DEBUG level logs')
 
@@ -33,20 +38,24 @@
     try:
         if args.output:
             if not args.silent:
                 print(f'Writing output to: {args.output}...')
 
             stubber.SimpleStubMaker().render_stub_classes_to_file(input_file=args.file,
                                                                   output_file=args.output,
-                                                                  overwrite_existing=args.force_overwrite)
+                                                                  overwrite_existing=args.force_overwrite,
+                                                                  is_private=not args.export_all)
         else:
             if not args.silent:
                 print(f'Printing results:')
                 print(f'==================================================')
-            print(stubber.SimpleStubMaker().render_stub_classes_from_descriptor_file(args.file))
+            cls_name = 'AlvissConfigStub' if args.class_name is None else args.class_name
+            if cls_name.lower().strip() == 'none':
+                cls_name = ''
+            print(stubber.SimpleStubMaker().render_stub_classes_from_descriptor_file(args.file, class_name=cls_name, is_private=not args.export_all))
 
             if not args.silent:
                 print(f'==================================================')
 
         if not args.silent:
             print(f'Done!')
```

### Comparing `alviss-3.2.0/alviss/loaders/autoloader.py` & `alviss-3.2.1/alviss/loaders/autoloader.py`

 * *Files identical despite different names*

### Comparing `alviss-3.2.0/alviss/loaders/base.py` & `alviss-3.2.1/alviss/loaders/base.py`

 * *Files identical despite different names*

### Comparing `alviss-3.2.0/alviss/loaders/interface.py` & `alviss-3.2.1/alviss/loaders/interface.py`

 * *Files identical despite different names*

### Comparing `alviss-3.2.0/alviss/loaders/jsonfile.py` & `alviss-3.2.1/alviss/loaders/jsonfile.py`

 * *Files identical despite different names*

### Comparing `alviss-3.2.0/alviss/loaders/yamlfile.py` & `alviss-3.2.1/alviss/loaders/yamlfile.py`

 * *Files identical despite different names*

### Comparing `alviss-3.2.0/alviss/renderers/static/_simple.py` & `alviss-3.2.1/alviss/renderers/static/_simple.py`

 * *Files identical despite different names*

### Comparing `alviss-3.2.0/alviss/renderers/static/interface.py` & `alviss-3.2.1/alviss/renderers/static/interface.py`

 * *Files identical despite different names*

### Comparing `alviss-3.2.0/alviss/structs/baseconfig.py` & `alviss-3.2.1/alviss/structs/baseconfig.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,44 @@
     "BaseConfig",
 ]
 from ccptools.structs import *
 from ccptools.tpu import iters
 from ccptools.tpu import string
 import json
 import yaml
+import collections
+from alviss.utils import *
+
+
+class _KwSafeEmptyDict(EmptyDict):
+    def __getattribute__(self, name):
+        name = unescape_keyword(name)
+        if hasattr(collections.defaultdict, name):
+            return collections.defaultdict.__getattribute__(self, name)
+        if collections.defaultdict.__contains__(self, name):
+            data = collections.defaultdict.__getitem__(self, name)
+            if isinstance(data, dict):
+                return _KwSafeEmptyDict(**data)
+            elif data is None:
+                return Empty
+            else:
+                return data
+        return Empty
+
+    def __getitem__(self, item):
+        item = unescape_keyword(item)
+        if collections.defaultdict.__contains__(self, item):
+            data = collections.defaultdict.__getitem__(self, item)
+            if isinstance(data, dict):
+                return _KwSafeEmptyDict(**data)
+            elif data is None:
+                return Empty
+            else:
+                return data
+        return Empty
 
 
 class BaseConfig(object):
     """This object simplifies accessing configuration values by more-or-less
     behaving like a `ccptools.structs.EmptyDict`.
 
     That is to say, just access any value, no matter how nested it is, via dot
@@ -37,29 +67,29 @@
     ```
 
 
     """
     _secret_keys = {'pass', 'secret', 'token', 'key'}
 
     def __init__(self, **kwargs):
-        super().__setattr__('_data', EmptyDict(**kwargs))
+        super().__setattr__('_data', _KwSafeEmptyDict(**kwargs))
 
     def __getattr__(self, item):
-        return EmptyDict.__getattribute__(self._data, item)
+        return _KwSafeEmptyDict.__getattribute__(self._data, item)
 
     def __setattr__(self, key, value):
         if key.startswith('_'):
             super().__setattr__(key, value)
         self.update(**{key: value})
 
     def __str__(self):
-        return EmptyDict.__str__(self._repr_dump(self._data))  # noqa
+        return _KwSafeEmptyDict.__str__(self._repr_dump(self._data))  # noqa
 
     def __repr__(self):
-        return EmptyDict.__repr__(self._repr_dump(self._data))  # noqa
+        return _KwSafeEmptyDict.__repr__(self._repr_dump(self._data))  # noqa
 
     def as_json(self, unmaksed: bool = False) -> str:
         return json.dumps(self.as_dict(unmaksed=unmaksed), indent=4)
 
     def as_yaml(self, unmaksed: bool = False) -> str:
         return yaml.dump(self.as_dict(unmaksed=unmaksed))
 
@@ -83,12 +113,12 @@
         key = string.str_norm(key)
         for sk in cls._secret_keys:
             if sk in key:
                 return True
         return False
 
     def load(self, **kwargs):
-        super().__setattr__('_data', EmptyDict(**kwargs))
+        super().__setattr__('_data', _KwSafeEmptyDict(**kwargs))
 
     def update(self, **kwargs):
-        iters.nested_dict_update(self._data, EmptyDict(**kwargs))
+        iters.nested_dict_update(self._data, _KwSafeEmptyDict(**kwargs))
```

### Comparing `alviss-3.2.0/alviss/structs/errors.py` & `alviss-3.2.1/alviss/structs/errors.py`

 * *Files identical despite different names*

### Comparing `alviss-3.2.0/alviss/stubber/stubmaker/_structs.py` & `alviss-3.2.1/alviss/stubber/stubmaker/_structs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 __all__ = [
     'StubField',
     'StubClass',
 ]
 import dataclasses
 from typing import *
 from alviss.structs.errors import *
+from alviss.utils import *
 import re
 
 import logging
 log = logging.getLogger(__name__)
 
 
 _WORD_PATTERN = re.compile(r'(\w+)')
@@ -86,53 +87,58 @@
             for v in self.value:
                 new_list.append(self._loop_over_type_words(v))
             self.value = new_list
         else:
             self.value = self._loop_over_type_words(self.value)
 
     @property
+    def safe_field_name(self) -> str:
+        return escape_keyword(self.name)
+
+    @property
     def is_required(self) -> bool:
         return self.is_self_required or self.has_required_children
 
     @property
     def has_required_children(self) -> bool:
         if isinstance(self.value, StubClass):
             return self.value.has_required_fields
         return False
 
     @classmethod
     def from_keyval(cls, key: str, value: Union[str, List, Dict], ancestors: Optional[List[str]],
                     is_map_of_stuff: bool = False,
-                    pre_required: bool = False) -> 'StubField':
+                    pre_required: bool = False,
+                    is_private: bool = True) -> 'StubField':
         required = pre_required
 
         if key.endswith('*'):
             required = True
             key = key[:-1].strip()
 
         if isinstance(value, dict):
             if len(value) == 1 and ('${str}' in value or '${str}*' in value):
                 sub_key, sub_val = value.popitem()
                 if sub_key.endswith('*'):
                     required = True
                 return cls.from_keyval(key=key, value=sub_val, pre_required=required,
-                                       ancestors=ancestors, is_map_of_stuff=True)
+                                       ancestors=ancestors, is_map_of_stuff=True, is_private=is_private)
 
             else:
-                value = StubClass.from_dict(input_dict_or_list=value, field_name=key, ancestors=ancestors)
+                value = StubClass.from_dict(input_dict_or_list=value, field_name=key, ancestors=ancestors, is_private=is_private)
                 return cls(name=key, value=value, is_self_required=required,
                            ancestors=ancestors, is_map_of_stuff=is_map_of_stuff)
 
         elif isinstance(value, list):
             if len(value) != 1:
                 raise AlvissStubberSyntaxError('Lists in type descriptor files must have exactly one element',
                                                field_name='.'.join(ancestors+[key]))
 
             if isinstance(value[0], dict):
-                value = StubClass.from_dict(input_dict_or_list=value[0], field_name=key, ancestors=ancestors)
+                value = StubClass.from_dict(input_dict_or_list=value[0], field_name=key, ancestors=ancestors, is_private=is_private)
                 return cls(name=key, value=value, is_self_required=required, ancestors=ancestors,
                            is_dict_list=True, is_map_of_stuff=is_map_of_stuff)
 
             elif isinstance(value[0], str):
                 value = value[0].strip()
 
                 if value.endswith('*'):
@@ -159,69 +165,71 @@
         return cls(name=key, value=value, is_self_required=required, ancestors=ancestors.copy(),
                    is_map_of_stuff=is_map_of_stuff)
 
     def render_field_str(self) -> str:
         if isinstance(self.value, StubClass):
             if self.is_required:
                 if self.is_dict_list:
-                    return f'    {self.name}: List[{self.value.class_name}]'
+                    return f'    {self.safe_field_name}: List[{self.value.class_name}]'
                 elif self.is_map_of_stuff:
-                    return f'    {self.name}: Dict[str, {self.value.class_name}]'
+                    return f'    {self.safe_field_name}: Dict[str, {self.value.class_name}]'
                 else:
-                    return f'    {self.name}: {self.value.class_name}'
+                    return f'    {self.safe_field_name}: {self.value.class_name}'
             else:
                 if self.is_dict_list:
                     type_list = [f'List[{self.value.class_name}]', 'Empty']
                 elif self.is_map_of_stuff:
                     type_list = [f'Dict[str, {self.value.class_name}]', 'Empty']
                 else:
                     type_list = [self.value.class_name, 'Empty']
 
         elif isinstance(self.value, list):
             type_list = self.value
             if not self.is_required:
                 type_list.append('Empty')
         else:
             if self.is_required:
-                return f'    {self.name}: {self.value}'
+                return f'    {self.safe_field_name}: {self.value}'
             else:
                 type_list = [self.value, 'Empty']
 
-        return f'    {self.name}: Union[{", ".join(type_list)}]'
+        return f'    {self.safe_field_name}: Union[{", ".join(type_list)}]'
 
 
 @dataclasses.dataclass
 class StubClass:
     name: str
     ancestors: List[str] = dataclasses.field(default_factory=list)
     fields: List[StubField] = dataclasses.field(default_factory=list)
+    is_private: bool = True
 
     @property
     def has_required_fields(self) -> bool:
         for field in self.fields:
             if field.is_required:
                 return True
         return False
 
     @classmethod
     def from_dict(cls,
                   input_dict_or_list: Union[Dict[str, Any], List[Any]],
                   field_name: str = '',
-                  ancestors: Optional[List[str]] = None) -> 'StubClass':
+                  ancestors: Optional[List[str]] = None,
+                  is_private: bool = True) -> 'StubClass':
         ancestors = ancestors or []
         ancestors.append(field_name)
         if isinstance(input_dict_or_list, dict):
-            fields = [StubField.from_keyval(k, v, ancestors.copy()) for k, v in input_dict_or_list.items()]
+            fields = [StubField.from_keyval(k, v, ancestors.copy(), is_private=is_private) for k, v in input_dict_or_list.items()]
         elif isinstance(input_dict_or_list, list):  # Should you ever get a list...?!?
             log.warning('NOT SURE THIS SHOULD EVER HAPPEN!!!')
-            fields = [StubField.from_keyval('__list__', input_dict_or_list[0], ancestors.copy())]
+            fields = [StubField.from_keyval('__list__', input_dict_or_list[0], ancestors.copy(), is_private=is_private)]
         else:
             raise AlvissStubberSyntaxError(f'Unexpected type fed to StubClass.from_dict: {type(input_dict_or_list)}')
         ancestors.pop()
-        return cls(name=field_name, ancestors=ancestors, fields=fields)
+        return cls(name=field_name, ancestors=ancestors, fields=fields, is_private=is_private)
 
     @staticmethod
     def field_name_to_class_name(field_name: str) -> str:
         if not field_name.isupper() and not field_name.islower():  # Mixed Casing
             tmp = []
             for c in field_name:
                 if c.isupper():
@@ -235,28 +243,32 @@
             field_name = ''.join(tmp)
         parts = field_name.split('_')
         buff = []
         for part in parts:
             if not part:
                 continue
             buff.append(part.capitalize())
-        return ''.join(buff)
+        result = ''.join(buff)
+        return escape_keyword(result)  # Just in case!
 
     @property
     def class_name(self) -> str:
+        start = 'Cfg'
+        if self.is_private:
+            start = '_Cfg'
         if not self.name:
-            return 'CfgStub'
+            return f'{start}Stub'
         else:
             if self.ancestors:
-                return f'Cfg{"".join([self.field_name_to_class_name(a) for a in self.ancestors+[self.name]])}Stub'
+                return f'{start}{"".join([self.field_name_to_class_name(a) for a in self.ancestors+[self.name]])}Stub'
             else:
-                return f'Cfg{self.field_name_to_class_name(self.name)}Stub'
+                return f'{start}{self.field_name_to_class_name(self.name)}Stub'
 
     def render_class_str(self) -> str:
-        lines = [f'class {self.class_name}(_BaseCfgStub):']
+        lines = [f'class {self.class_name}(_BaseCfgStub, dict):']
         for field in self.fields:
             lines.append(field.render_field_str())
         return '\n'.join(lines)
 
     def get_all_sub_stubs(self) -> List['StubClass']:
         lst = []
         for field in self.fields:
```

### Comparing `alviss-3.2.0/alviss/stubber/stubmaker/interface.py` & `alviss-3.2.1/alviss/stubber/stubmaker/interface.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,19 +2,21 @@
     'IStubMaker',
 ]
 from alviss.structs import *
 
 
 class IStubMaker(abc.ABC):
     @abc.abstractmethod
-    def render_stub_classes_from_descriptor_file(self, file: str) -> str:
+    def render_stub_classes_from_descriptor_file(self, file: str, is_private: bool = True,
+                                                 class_name: str = 'AlvissConfigStub') -> str:
         """Renders a Python module file with type hinting stub classes from the
         Alviss config type descriptor file.
         """
         pass
 
     @abc.abstractmethod
-    def render_stub_classes_to_file(self, input_file: str, output_file: str, overwrite_existing: bool = False):
+    def render_stub_classes_to_file(self, input_file: str, output_file: str,
+                                    overwrite_existing: bool = False, is_private: bool = True):
         """Writer the results of the `render_stub_classes_from_descriptor_file`
         call to the given output file.
         """
         pass
```

### Comparing `alviss-3.2.0/alviss.egg-info/PKG-INFO` & `alviss-3.2.1/alviss.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alviss
-Version: 3.2.0
+Version: 3.2.1
 Summary: Configuration file reader with some nifty bells and whistles added
 Author-email: Thordur Matthiasson <thordurm@ccpgames.com>
 License: MIT License
         
         Copyright (c) 2019-2024 CCP Games
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `alviss-3.2.0/alviss.egg-info/SOURCES.txt` & `alviss-3.2.1/alviss.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -31,8 +31,10 @@
 alviss/structs/cfgstub.py
 alviss/structs/errors.py
 alviss/structs/singletonconfig.py
 alviss/stubber/__init__.py
 alviss/stubber/stubmaker/__init__.py
 alviss/stubber/stubmaker/_simple.py
 alviss/stubber/stubmaker/_structs.py
-alviss/stubber/stubmaker/interface.py
+alviss/stubber/stubmaker/interface.py
+alviss/utils/__init__.py
+alviss/utils/kwfields.py
```

### Comparing `alviss-3.2.0/pyproject.toml` & `alviss-3.2.1/pyproject.toml`

 * *Files identical despite different names*

