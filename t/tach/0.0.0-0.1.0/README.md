# Comparing `tmp/tach-0.0.0.tar.gz` & `tmp/tach-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tach-0.0.0.tar", last modified: Mon Apr 29 23:05:56 2024, max compression
+gzip compressed data, was "tach-0.1.0.tar", last modified: Tue Apr 30 02:38:57 2024, max compression
```

## Comparing `tach-0.0.0.tar` & `tach-0.1.0.tar`

### file list

```diff
@@ -1,51 +1,50 @@
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-29 23:05:56.011223 tach-0.0.0/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)    35149 2024-01-31 20:12:51.000000 tach-0.0.0/LICENSE
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     7270 2024-04-29 23:05:56.010937 tach-0.0.0/PKG-INFO
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     5928 2024-04-28 01:11:25.000000 tach-0.0.0/README.md
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-29 23:05:56.003467 tach-0.0.0/modguard/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-04-27 02:35:46.000000 tach-0.0.0/modguard/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2887 2024-04-28 04:44:11.000000 tach-0.0.0/modguard/add.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     7226 2024-04-27 23:04:58.000000 tach-0.0.0/modguard/check.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     6449 2024-04-28 04:55:08.000000 tach-0.0.0/modguard/cli.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-29 23:05:56.003734 tach-0.0.0/modguard/colors/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      251 2024-04-27 02:35:46.000000 tach-0.0.0/modguard/colors/__init__.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-29 23:05:56.003996 tach-0.0.0/modguard/constants/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      110 2024-04-27 02:35:46.000000 tach-0.0.0/modguard/constants/__init__.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-29 23:05:56.004799 tach-0.0.0/modguard/core/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      259 2024-04-27 02:35:46.000000 tach-0.0.0/modguard/core/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      706 2024-04-27 02:35:46.000000 tach-0.0.0/modguard/core/config.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     3071 2024-04-27 02:35:46.000000 tach-0.0.0/modguard/core/module.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-29 23:05:56.005064 tach-0.0.0/modguard/errors/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      204 2024-04-28 01:00:48.000000 tach-0.0.0/modguard/errors/__init__.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-29 23:05:56.005970 tach-0.0.0/modguard/filesystem/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1000 2024-04-28 00:56:50.000000 tach-0.0.0/modguard/filesystem/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2468 2024-04-28 04:42:24.000000 tach-0.0.0/modguard/filesystem/module.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1260 2024-04-28 01:14:46.000000 tach-0.0.0/modguard/filesystem/project.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     8867 2024-04-27 23:04:58.000000 tach-0.0.0/modguard/filesystem/service.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     3800 2024-04-27 23:04:58.000000 tach-0.0.0/modguard/init.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1454 2024-02-13 23:42:10.000000 tach-0.0.0/modguard/loading.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-29 23:05:56.007815 tach-0.0.0/modguard/parsing/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      407 2024-04-27 02:35:46.000000 tach-0.0.0/modguard/parsing/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      425 2024-02-13 20:36:09.000000 tach-0.0.0/modguard/parsing/ast_visitor.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1065 2024-04-27 02:35:46.000000 tach-0.0.0/modguard/parsing/config.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     4288 2024-04-27 02:35:46.000000 tach-0.0.0/modguard/parsing/imports.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1833 2024-04-27 02:35:46.000000 tach-0.0.0/modguard/parsing/interface.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      893 2024-04-27 02:35:46.000000 tach-0.0.0/modguard/parsing/modules.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     3268 2024-04-27 02:35:46.000000 tach-0.0.0/modguard/show.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1551 2024-04-29 23:05:37.000000 tach-0.0.0/pyproject.toml
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       38 2024-04-29 23:05:56.011288 tach-0.0.0/setup.cfg
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-29 23:05:56.010579 tach-0.0.0/tach.egg-info/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     7270 2024-04-29 23:05:55.000000 tach-0.0.0/tach.egg-info/PKG-INFO
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      928 2024-04-29 23:05:55.000000 tach-0.0.0/tach.egg-info/SOURCES.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        1 2024-04-29 23:05:55.000000 tach-0.0.0/tach.egg-info/dependency_links.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       47 2024-04-29 23:05:55.000000 tach-0.0.0/tach.egg-info/entry_points.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       50 2024-04-29 23:05:55.000000 tach-0.0.0/tach.egg-info/requires.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        9 2024-04-29 23:05:55.000000 tach-0.0.0/tach.egg-info/top_level.txt
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-29 23:05:56.010348 tach-0.0.0/tests/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     3295 2024-04-27 23:50:15.000000 tach-0.0.0/tests/test_add.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     3604 2024-04-27 03:12:45.000000 tach-0.0.0/tests/test_check.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     3642 2024-04-27 02:35:46.000000 tach-0.0.0/tests/test_cli.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2327 2024-04-27 02:35:46.000000 tach-0.0.0/tests/test_init.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     3439 2024-04-27 02:35:46.000000 tach-0.0.0/tests/test_module_trie.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     3549 2024-04-27 02:35:46.000000 tach-0.0.0/tests/test_parsing.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        1 2024-04-27 02:35:46.000000 tach-0.0.0/tests/test_show.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-30 02:38:57.598312 tach-0.1.0/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)    35149 2024-01-31 20:12:51.000000 tach-0.1.0/LICENSE
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     6881 2024-04-30 02:38:57.598073 tach-0.1.0/PKG-INFO
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     5559 2024-04-30 02:38:41.000000 tach-0.1.0/README.md
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1515 2024-04-30 02:38:41.000000 tach-0.1.0/pyproject.toml
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       38 2024-04-30 02:38:57.598367 tach-0.1.0/setup.cfg
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-30 02:38:57.593650 tach-0.1.0/tach/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-04-30 02:38:41.000000 tach-0.1.0/tach/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     5960 2024-04-30 02:38:41.000000 tach-0.1.0/tach/add.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     7308 2024-04-30 02:38:41.000000 tach-0.1.0/tach/check.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     5647 2024-04-30 02:38:41.000000 tach-0.1.0/tach/cli.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-30 02:38:57.594549 tach-0.1.0/tach/colors/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      251 2024-04-30 02:38:41.000000 tach-0.1.0/tach/colors/__init__.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-30 02:38:57.594673 tach-0.1.0/tach/constants/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      144 2024-04-30 02:38:41.000000 tach-0.1.0/tach/constants/__init__.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-30 02:38:57.595062 tach-0.1.0/tach/core/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      258 2024-04-30 02:38:41.000000 tach-0.1.0/tach/core/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      729 2024-04-30 02:38:41.000000 tach-0.1.0/tach/core/config.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     3086 2024-04-30 02:38:41.000000 tach-0.1.0/tach/core/package.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-30 02:38:57.595185 tach-0.1.0/tach/errors/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      172 2024-04-30 02:38:41.000000 tach-0.1.0/tach/errors/__init__.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-30 02:38:57.595701 tach-0.1.0/tach/filesystem/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      917 2024-04-30 02:38:41.000000 tach-0.1.0/tach/filesystem/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      406 2024-04-30 02:38:41.000000 tach-0.1.0/tach/filesystem/package.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1248 2024-04-30 02:38:41.000000 tach-0.1.0/tach/filesystem/project.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     8949 2024-04-30 02:38:41.000000 tach-0.1.0/tach/filesystem/service.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     3895 2024-04-30 02:38:41.000000 tach-0.1.0/tach/init.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1454 2024-04-30 02:38:41.000000 tach-0.1.0/tach/loading.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-30 02:38:57.596740 tach-0.1.0/tach/parsing/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      396 2024-04-30 02:38:41.000000 tach-0.1.0/tach/parsing/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      425 2024-04-30 02:38:41.000000 tach-0.1.0/tach/parsing/ast_visitor.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1064 2024-04-30 02:38:41.000000 tach-0.1.0/tach/parsing/config.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     4268 2024-04-30 02:38:41.000000 tach-0.1.0/tach/parsing/imports.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1825 2024-04-30 02:38:41.000000 tach-0.1.0/tach/parsing/interface.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      900 2024-04-30 02:38:41.000000 tach-0.1.0/tach/parsing/packages.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-30 02:38:57.597803 tach-0.1.0/tach.egg-info/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     6881 2024-04-30 02:38:57.000000 tach-0.1.0/tach.egg-info/PKG-INFO
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      826 2024-04-30 02:38:57.000000 tach-0.1.0/tach.egg-info/SOURCES.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        1 2024-04-30 02:38:57.000000 tach-0.1.0/tach.egg-info/dependency_links.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       39 2024-04-30 02:38:57.000000 tach-0.1.0/tach.egg-info/entry_points.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       50 2024-04-30 02:38:57.000000 tach-0.1.0/tach.egg-info/requires.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        5 2024-04-30 02:38:57.000000 tach-0.1.0/tach.egg-info/top_level.txt
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-30 02:38:57.597629 tach-0.1.0/tests/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     3130 2024-04-30 02:38:41.000000 tach-0.1.0/tests/test_add.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     3618 2024-04-30 02:38:41.000000 tach-0.1.0/tests/test_check.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     3301 2024-04-30 02:38:41.000000 tach-0.1.0/tests/test_cli.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2315 2024-04-30 02:38:41.000000 tach-0.1.0/tests/test_init.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     3477 2024-04-30 02:38:41.000000 tach-0.1.0/tests/test_module_trie.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     3545 2024-04-30 02:38:41.000000 tach-0.1.0/tests/test_parsing.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        1 2024-04-30 02:38:41.000000 tach-0.1.0/tests/test_show.py
```

### Comparing `tach-0.0.0/LICENSE` & `tach-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tach-0.0.0/modguard/check.py` & `tach-0.1.0/tach/check.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import re
 from dataclasses import dataclass, field
 from typing import Optional
 
-from modguard import filesystem as fs
-from modguard.core import ModuleTrie, ModuleNode, ProjectConfig
-from modguard.parsing import build_module_trie, get_project_imports
+from tach import filesystem as fs
+from tach.core import PackageTrie, PackageNode, ProjectConfig
+from tach.parsing import build_package_trie, get_project_imports
 
 
 @dataclass
 class ErrorInfo:
     location: str = ""
     import_mod_path: str = ""
     source_tag: str = ""
@@ -52,80 +52,82 @@
         return cls(ok=True)
 
     @classmethod
     def fail(cls, error_info: ErrorInfo) -> "CheckResult":
         return cls(ok=False, error_info=error_info)
 
 
-def is_top_level_module_import(mod_path: str, module: ModuleNode) -> bool:
-    return mod_path == module.full_path
+def is_top_level_package_import(mod_path: str, package: PackageNode) -> bool:
+    return mod_path == package.full_path
 
 
-def import_matches_interface_members(mod_path: str, module: ModuleNode) -> bool:
+def import_matches_interface_members(mod_path: str, package: PackageNode) -> bool:
     mod_path_basename = mod_path.rsplit(".", 1)[-1]
-    return mod_path_basename in module.interface_members
+    return mod_path_basename in package.interface_members
 
 
 def check_import(
     project_config: ProjectConfig,
-    module_trie: ModuleTrie,
+    package_trie: PackageTrie,
     import_mod_path: str,
     file_mod_path: str,
-    file_nearest_module: Optional[ModuleNode] = None,
+    file_nearest_package: Optional[PackageNode] = None,
 ) -> CheckResult:
-    import_nearest_module = module_trie.find_nearest(import_mod_path)
-    if import_nearest_module is None:
+    import_nearest_package = package_trie.find_nearest(import_mod_path)
+    if import_nearest_package is None:
         # This shouldn't happen since we intend to filter out any external imports,
         # but we should allow external imports if they have made it here.
         return CheckResult.success()
 
-    # Lookup file_mod_path if module not given
-    if file_nearest_module is None:
-        file_nearest_module = module_trie.find_nearest(file_mod_path)
-    # If module not found, we should fail since the implication is that
-    # an external module is importing directly from our project
-    if file_nearest_module is None:
+    # Lookup file_mod_path if package not given
+    if file_nearest_package is None:
+        file_nearest_package = package_trie.find_nearest(file_mod_path)
+    # If package not found, we should fail since the implication is that
+    # an external package is importing directly from our project
+    if file_nearest_package is None:
         return CheckResult.fail(
             error_info=ErrorInfo(
-                exception_message=f"Module '{file_mod_path}' not found in project."
+                exception_message=f"Package containing '{file_mod_path}' not found in project."
             )
         )
 
-    # Imports within the same module are always allowed
-    if import_nearest_module == file_nearest_module:
+    # Imports within the same package are always allowed
+    if import_nearest_package == file_nearest_package:
         return CheckResult.success()
 
-    import_module_config = import_nearest_module.config
-    if import_module_config and import_module_config.strict:
-        if not is_top_level_module_import(
-            import_mod_path, import_nearest_module
+    import_package_config = import_nearest_package.config
+    if import_package_config and import_package_config.strict:
+        if not is_top_level_package_import(
+            import_mod_path, import_nearest_package
         ) and not import_matches_interface_members(
-            import_mod_path, import_nearest_module
+            import_mod_path, import_nearest_package
         ):
-            # In strict mode, import must be of the module itself or one of the
+            # In strict mode, import must be of the package itself or one of the
             # interface members (defined in __all__)
             return CheckResult.fail(
                 error_info=ErrorInfo(
                     location=file_mod_path,
                     exception_message=(
-                        f"Module '{import_nearest_module.full_path}' is in strict mode. "
-                        "Only imports from the root of this module are allowed. "
+                        f"Package '{import_nearest_package.full_path}' is in strict mode. "
+                        "Only imports from the root of this package are allowed. "
                         f"The import '{import_mod_path}' (in '{file_mod_path}') "
                         f"is not included in __all__."
                     ),
                 )
             )
 
     # The import must be explicitly allowed based on the tags and top-level config
-    if not file_nearest_module.config or not import_nearest_module.config:
+    if not file_nearest_package.config or not import_nearest_package.config:
         return CheckResult.fail(
-            error_info=ErrorInfo(exception_message="Could not find config for modules.")
+            error_info=ErrorInfo(
+                exception_message="Could not find config for packages."
+            )
         )
-    file_tags = file_nearest_module.config.tags
-    import_tags = import_nearest_module.config.tags
+    file_tags = file_nearest_package.config.tags
+    import_tags = import_nearest_package.config.tags
 
     for file_tag in file_tags:
         dependency_tags = (
             project_config.constraints[file_tag].depends_on
             if file_tag in project_config.constraints
             else []
         )
@@ -163,35 +165,35 @@
             ErrorInfo(exception_message=f"The path {root} is not a valid directory.")
         ]
 
     # This 'canonicalizes' the path arguments, resolving directory traversal
     root = fs.canonical(root)
     exclude_paths = list(map(fs.canonical, exclude_paths)) if exclude_paths else None
 
-    module_trie = build_module_trie(
+    package_trie = build_package_trie(
         root, exclude_paths=exclude_paths, exclude_hidden_paths=exclude_hidden_paths
     )
 
     errors: list[ErrorInfo] = []
     for file_path in fs.walk_pyfiles(
         root, exclude_paths=exclude_paths, exclude_hidden_paths=exclude_hidden_paths
     ):
         mod_path = fs.file_to_module_path(file_path)
-        nearest_module = module_trie.find_nearest(mod_path)
-        if nearest_module is None:
+        nearest_package = package_trie.find_nearest(mod_path)
+        if nearest_package is None:
             continue
         import_mod_paths = get_project_imports(root, file_path)
         # This should only give us imports from within our project
         # (excluding stdlib, builtins, and 3rd party packages)
         for import_mod_path in import_mod_paths:
             check_result = check_import(
                 project_config=project_config,
-                module_trie=module_trie,
+                package_trie=package_trie,
                 import_mod_path=import_mod_path,
-                file_nearest_module=nearest_module,
+                file_nearest_package=nearest_package,
                 file_mod_path=mod_path,
             )
             if check_result.ok or check_result.error_info is None:
                 continue
 
             errors.append(check_result.error_info)
```

### Comparing `tach-0.0.0/modguard/cli.py` & `tach-0.1.0/tach/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,92 +1,79 @@
 import argparse
 import sys
 from typing import Optional
 
-from modguard.add import add_modules
-from modguard.check import check, ErrorInfo
-from modguard import filesystem as fs
-from modguard.init import init_project
-from modguard.loading import stop_spinner, start_spinner
-from modguard.parsing import parse_project_config, build_module_trie
-from modguard.show import show
-from modguard.colors import BCOLORS
+from tach.add import add_packages
+from tach.check import check, ErrorInfo
+from tach import filesystem as fs
+from tach.constants import CONFIG_FILE_NAME
+from tach.init import init_project
+from tach.loading import stop_spinner, start_spinner
+from tach.parsing import parse_project_config
+from tach.colors import BCOLORS
 
 
 def print_errors(error_list: list[ErrorInfo]) -> None:
     sorted_results = sorted(error_list, key=lambda e: e.location)
     for error in sorted_results:
         print(
             f"❌ {BCOLORS.FAIL}{error.location}{BCOLORS.WARNING}: {error.message}",
             file=sys.stderr,
         )
 
 
-# todo default to full path from project root
-# todo mutate module trie (insert)
-#
-
-
 def add_base_arguments(parser: argparse.ArgumentParser) -> None:
     parser.add_argument(
         "-e",
         "--exclude",
         required=False,
         type=str,
         metavar="file_or_path,...",
         help="Comma separated path list to exclude. tests/, ci/, etc.",
     )
 
 
 def build_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(
-        prog="modguard",
+        prog="tach",
         add_help=True,
-        epilog="Make sure modguard is run from the root of your Python project,"
-        " and `modguard.yml` is present",
+        epilog="Make sure tach is run from the root of your Python project,"
+        " and `tach.yml` is present",
     )
     subparsers = parser.add_subparsers(title="commands", dest="command")
     init_parser = subparsers.add_parser(
         "init",
-        prog="modguard init",
-        help="Initialize boundaries between top-level modules and write dependencies to "
-        "`modguard.yml`",
-        description="Initialize boundaries between top-level modules and write dependencies to "
-        "`modguard.yml`",
+        prog="tach init",
+        help="Initialize boundaries between top-level packages and write dependencies to "
+        "`tach.yml`",
+        description="Initialize boundaries between top-level packages and write dependencies to "
+        "`tach.yml`",
+    )
+    init_parser.add_argument(
+        "-d",
+        "--depth",
+        type=int,
+        nargs="?",
+        default=None,
+        help="The number of child directories to search for packages to initialize",
     )
     add_base_arguments(init_parser)
     check_parser = subparsers.add_parser(
         "check",
-        prog="modguard check",
-        help="Check existing boundaries against your dependencies and module interfaces",
-        description="Check existing boundaries against your dependencies and module interfaces",
+        prog="tach check",
+        help="Check existing boundaries against your dependencies and package interfaces",
+        description="Check existing boundaries against your dependencies and package interfaces",
     )
     add_base_arguments(check_parser)
-    show_parser = subparsers.add_parser(
-        "show",
-        prog="modguard show",
-        help="Show your existing boundaries",
-        description="Show your existing boundaries",
-    )
-    add_base_arguments(show_parser)
-    show_parser.add_argument(
-        "-w",
-        "--write",
-        required=False,
-        dest="write",
-        action="store_true",
-        default=False,
-        help="Write the output to an `interface.yaml` file",
-    )
     add_parser = subparsers.add_parser(
         "add",
-        prog="modguard add",
+        prog="tach add",
         help="Create a new module boundary around an existing file or folder",
         description="Initialize boundaries between top-level modules and write dependencies to "
-        "`modguard.yml`",
+        "`tach.yml`",
     )
     add_parser.add_argument(
         "path",
         type=str,
         metavar="file_or_path,...",
         help="The path(s) of the file or directory to create a module boundary around. "
         "Use a comma-separated list for multiple.",
@@ -99,25 +86,27 @@
         metavar="tag,...",
         help="The tag for the module to be initialized with."
         "Use a comma-separated list for multiple.",
     )
     return parser
 
 
-def parse_arguments(args: list[str]) -> argparse.Namespace:
+def parse_arguments(
+    args: list[str],
+) -> tuple[argparse.Namespace, argparse.ArgumentParser]:
     parser = build_parser()
     parsed_args = parser.parse_args(args)
 
     if args[0] not in ["init", "add"]:
         fs.validate_project_config_path()
 
-    return parsed_args
+    return parsed_args, parser
 
 
-def modguard_check(
+def tach_check(
     exclude_paths: Optional[list[str]] = None,
 ):
     try:
         project_config = parse_project_config()
         if exclude_paths is not None and project_config.exclude is not None:
             exclude_paths.extend(project_config.exclude)
         else:
@@ -133,84 +122,66 @@
         print(str(e))
         sys.exit(1)
 
     stop_spinner()
     if result:
         print_errors(result)
         sys.exit(1)
-    print(f"✅ {BCOLORS.OKGREEN}All modules safely guarded!")
+    print(f"✅ {BCOLORS.OKGREEN}All package dependencies validated!")
     sys.exit(0)
 
 
-def modguard_show(
-    write_file: bool,
-    exclude_paths: Optional[list[str]] = None,
-    exclude_hidden_paths: Optional[bool] = True,
-):
+def tach_init(depth: Optional[int] = None, exclude_paths: Optional[list[str]] = None):
     try:
-        mt = build_module_trie(
-            ".", exclude_paths=exclude_paths, exclude_hidden_paths=exclude_hidden_paths
-        )
-        _, pretty_result = show(mt, write_file=write_file)
-    except Exception as e:
-        stop_spinner()
-        print(str(e))
-        sys.exit(1)
-    stop_spinner()
-    print(pretty_result)
-    sys.exit(0)
-
-
-def modguard_init(exclude_paths: Optional[list[str]] = None):
-    try:
-        warnings = init_project(root=".", exclude_paths=exclude_paths)
+        warnings = init_project(root=".", depth=depth, exclude_paths=exclude_paths)
     except Exception as e:
         stop_spinner()
         print(str(e))
         sys.exit(1)
 
     stop_spinner()
     if warnings:
         print("\n".join(warnings))
-    print(f"✅ {BCOLORS.OKGREEN}Modguard initialized.")
+    print(f"✅ {BCOLORS.OKGREEN}Initialized {CONFIG_FILE_NAME}.yml.")
     sys.exit(0)
 
 
-def modguard_add(paths: set[str], tags: Optional[set[str]] = None) -> None:
+def tach_add(paths: set[str], tags: Optional[set[str]] = None) -> None:
     try:
-        warnings = add_modules(paths, tags)
+        warnings = add_packages(paths, tags)
     except Exception as e:
         stop_spinner()
         print(str(e))
         sys.exit(1)
 
     stop_spinner()
     if warnings:
         print("\n".join(warnings))
-    print(f"✅ {BCOLORS.OKGREEN}Modguard initialized.")
+    if len(paths) > 1:
+        print(f"✅ {BCOLORS.OKGREEN}Packages added.")
+    else:
+        print(f"✅ {BCOLORS.OKGREEN}Package added.")
     sys.exit(0)
 
 
 def main() -> None:
-    args = parse_arguments(sys.argv[1:])
+    args, parser = parse_arguments(sys.argv[1:])
     if args.command == "add":
         paths = set(args.path.split(","))
         tags = set(args.tags.split(",")) if args.tags else None
-        modguard_add(paths=paths, tags=tags)
+        tach_add(paths=paths, tags=tags)
         return
     exclude_paths = args.exclude.split(",") if args.exclude else None
     if args.command == "init":
         start_spinner("Initializing...")
-        modguard_init(exclude_paths=exclude_paths)
+        tach_init(depth=args.depth, exclude_paths=exclude_paths)
     elif args.command == "check":
         start_spinner("Scanning...")
-        modguard_check(exclude_paths=exclude_paths)
-    elif args.command == "show":
-        start_spinner("Scanning...")
-        modguard_show(write_file=args.write, exclude_paths=exclude_paths)
+        tach_check(exclude_paths=exclude_paths)
     else:
         print("Unrecognized command")
+        parser.print_help()
         exit(1)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `tach-0.0.0/modguard/core/config.py` & `tach-0.1.0/tach/core/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from pydantic import BaseModel, Field
 
 
 class Config(BaseModel):
     model_config = {"extra": "forbid"}
 
 
-class ModuleConfig(Config):
+class PackageConfig(Config):
     """
-    Configuration for a single module within a project.
+    Configuration for a single package within a project.
     """
 
     tags: List[str]
     strict: bool = False
 
 
 class ScopeDependencyRules(Config):
@@ -26,9 +26,9 @@
 
 class ProjectConfig(Config):
     """
     Configuration applied globally to a project.
     """
 
     constraints: Dict[str, ScopeDependencyRules] = Field(default_factory=dict)
-    exclude: Optional[List[str]] = Field(default_factory=list)
+    exclude: Optional[List[str]] = Field(default_factory=lambda: ["tests", "docs"])
     exclude_hidden_paths: Optional[bool] = True
```

### Comparing `tach-0.0.0/modguard/core/module.py` & `tach-0.1.0/tach/core/package.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,86 +1,86 @@
 from collections import deque
 from dataclasses import dataclass, field
 from typing import Optional, Generator
 
-from modguard.core.config import ModuleConfig
+from tach.core.config import PackageConfig
 
 
 @dataclass
-class ModuleNode:
+class PackageNode:
     """
-    A node in the module trie.
+    A node in the package trie.
 
-    If 'is_end_of_path' is True, this node represents a module in the project,
+    If 'is_end_of_path' is True, this node represents a package in the project,
     and must have 'config' and 'full_path' set.
 
-    If 'is_end_of_path' is False, this node does not represent a real module,
+    If 'is_end_of_path' is False, this node does not represent a real package,
     and must have 'config' None and 'full_path' as the empty string.
     """
 
     is_end_of_path: bool
     full_path: str
-    config: Optional[ModuleConfig]
+    config: Optional[PackageConfig]
     interface_members: list[str] = field(default_factory=list)
-    children: dict[str, "ModuleNode"] = field(default_factory=dict)
+    children: dict[str, "PackageNode"] = field(default_factory=dict)
 
     @classmethod
-    def empty(cls) -> "ModuleNode":
-        return ModuleNode(is_end_of_path=False, full_path="", config=None)
+    def empty(cls) -> "PackageNode":
+        return PackageNode(is_end_of_path=False, full_path="", config=None)
 
     def fill(
-        self, config: ModuleConfig, full_path: str, interface_members: list[str]
+        self, config: PackageConfig, full_path: str, interface_members: list[str]
     ) -> None:
         self.is_end_of_path = True
         self.config = config
         self.full_path = full_path
         self.interface_members = interface_members
 
 
 @dataclass
-class ModuleTrie:
+class PackageTrie:
     """
-    The core data structure for modguard, representing the modules in a project
-    with a trie structure for module prefix lookups.
+    The core data structure for tach, representing the packages in a project
+    with a trie structure for package prefix lookups.
     """
 
-    root: ModuleNode = field(default_factory=ModuleNode.empty)
+    root: PackageNode = field(default_factory=PackageNode.empty)
 
     def __iter__(self):
-        return module_trie_iterator(self)
+        return package_trie_iterator(self)
 
     @staticmethod
     def _split_mod_path(path: str) -> list[str]:
         # By default "".split(".") -> ['']
         # so we want to remove any whitespace path components
         return [part for part in path.split(".") if part]
 
-    def get(self, path: str) -> Optional[ModuleNode]:
+    def get(self, path: str) -> Optional[PackageNode]:
         node = self.root
         parts = self._split_mod_path(path)
 
         for part in parts:
             if part not in node.children:
                 return None
             node = node.children[part]
 
         return node if node.is_end_of_path else None
 
-    def insert(self, config: ModuleConfig, path: str, interface_members: list[str]):
+    def insert(self, config: PackageConfig, path: str, interface_members: list[str]):
         node = self.root
         parts = self._split_mod_path(path)
 
         for part in parts:
             if part not in node.children:
-                node.children[part] = ModuleNode.empty()
+                node.children[part] = PackageNode.empty()
             node = node.children[part]
 
         node.fill(config, path, interface_members)
 
-    def find_nearest(self, path: str) -> Optional[ModuleNode]:
+    def find_nearest(self, path: str) -> Optional[PackageNode]:
         node = self.root
         parts = self._split_mod_path(path)
         nearest_parent = node
 
         for part in parts:
             if part in node.children:
                 node = node.children[part]
@@ -88,15 +88,15 @@
                     nearest_parent = node
             else:
                 break
 
         return nearest_parent if nearest_parent.is_end_of_path else None
 
 
-def module_trie_iterator(trie: ModuleTrie) -> Generator[ModuleNode, None, None]:
+def package_trie_iterator(trie: PackageTrie) -> Generator[PackageNode, None, None]:
     stack = deque([trie.root])
 
     while stack:
         node = stack.popleft()
         if node.is_end_of_path:
             yield node
```

### Comparing `tach-0.0.0/modguard/filesystem/project.py` & `tach-0.1.0/tach/filesystem/project.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 import sys
 from pathlib import Path
 from typing import Optional
 
-from modguard.colors import BCOLORS
-from modguard.constants import CONFIG_FILE_NAME
+from tach.colors import BCOLORS
+from tach.constants import CONFIG_FILE_NAME
 
 
-def print_no_modguard_yml() -> None:
+def print_no_config_yml() -> None:
     print(
         f"{BCOLORS.FAIL} {CONFIG_FILE_NAME}.(yml|yaml) not found in {os.getcwd()}",
         file=sys.stderr,
     )
 
 
 def get_project_config_path(root: str = ".") -> str:
@@ -35,11 +35,11 @@
         if get_project_config_path(str(parent)):
             return str(parent)
 
 
 def validate_project_config_path(root: str = ".") -> str:
     project_config_path = get_project_config_path(root)
     if not project_config_path:
-        print_no_modguard_yml()
+        print_no_config_yml()
         sys.exit(1)
     else:
         return project_config_path
```

### Comparing `tach-0.0.0/modguard/filesystem/service.py` & `tach-0.1.0/tach/filesystem/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import sys
 import threading
 from collections import defaultdict
 from dataclasses import dataclass
 from functools import lru_cache
 from pathlib import Path
 from typing import Optional, Generator
-from modguard import errors
+from tach import errors
 
 
 @dataclass
 class FileInfo:
     path: str
     content: Optional[str] = None
     canonical_path: Optional[str] = None
@@ -111,22 +111,22 @@
         return cached_file.ast
 
     if cached_file and cached_file.content:
         content = cached_file.content
         try:
             ast_result = ast.parse(cached_file.content)
         except SyntaxError as e:
-            raise errors.ModguardParseError(f"Syntax error in {path}: {e}")
+            raise errors.TachParseError(f"Syntax error in {path}: {e}")
     else:
         with open(path, "r") as f:
             content = f.read()
         try:
             ast_result = ast.parse(content)
         except SyntaxError as e:
-            raise errors.ModguardParseError(f"Syntax error in {path}: {e}")
+            raise errors.TachParseError(f"Syntax error in {path}: {e}")
 
     if cached_file:
         cached_file.content = content
         cached_file.ast = ast_result
     else:
         _set_cached_file(path, FileInfo(path=path, content=content, ast=ast_result))
 
@@ -139,23 +139,25 @@
     exclude_paths: Optional[list[str]] = None,
     exclude_hidden_paths: Optional[bool] = True,
 ) -> Generator[str, None, None]:
     canonical_root = canonical(root)
     base_depth = 0 if canonical_root == "." else canonical_root.count(os.path.sep) + 1
     for dirpath, _, filenames in os.walk(canonical_root):
         dirpath = canonical(dirpath)
+        dirpath_for_matching = f"{dirpath}/"
 
         if dirpath == canonical_root:
             continue
 
         if exclude_hidden_paths and os.path.basename(dirpath).startswith("."):
             continue
 
         if exclude_paths is not None and any(
-            dirpath.startswith(exclude_path) or re.match(exclude_path, dirpath)
+            dirpath_for_matching.startswith(exclude_path)
+            or re.match(exclude_path, dirpath_for_matching)
             for exclude_path in exclude_paths
         ):
             # Treat excluded paths as invisible
             continue
 
         if depth:
             # Ignore anything past requested depth
@@ -183,28 +185,28 @@
         exclude_hidden_paths=exclude_hidden_paths,
     ):
         init_file_ending = f"{os.path.sep}__init__.py"
         if filepath.endswith(init_file_ending):
             yield filepath[: -len(init_file_ending)]
 
 
-def walk_modules(
+def walk_configured_packages(
     root: str,
     depth: Optional[int] = None,
     exclude_paths: Optional[list[str]] = None,
     exclude_hidden_paths: Optional[bool] = True,
 ) -> Generator[str, None, None]:
     for dirpath in walk_pypackages(
         root,
         depth=depth,
         exclude_paths=exclude_paths,
         exclude_hidden_paths=exclude_hidden_paths,
     ):
-        module_yml_path = os.path.join(dirpath, "module.yml")
-        if os.path.isfile(module_yml_path):
+        package_yml_path = os.path.join(dirpath, "package.yml")
+        if os.path.isfile(package_yml_path):
             yield dirpath
 
 
 @lru_cache(maxsize=None)
 def file_to_module_path(file_path: str) -> str:
     # Assuming that the file_path has been 'canonicalized' and does not traverse multiple directories
     file_path = file_path.lstrip("./")
@@ -261,15 +263,15 @@
         return file_path, member_name
 
     init_file_path = fs_path[:last_sep_index] + "/__init__.py"
     if path_exists_case_sensitive(Path(init_file_path)):
         member_name = fs_path[last_sep_index + 1 :]
         return init_file_path, member_name
 
-    raise errors.ModguardParseError(
+    raise errors.TachParseError(
         f"Failed to translate module path {mod_path} into file path"
     )
 
 
 if hasattr(sys, "stdlib_module_names"):
     stdlib_module_names = getattr(sys, "stdlib_module_names")
 else:
```

### Comparing `tach-0.0.0/modguard/init.py` & `tach-0.1.0/tach/init.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 import os
 from dataclasses import field, dataclass
 from typing import Optional
 
 import yaml
 
-from modguard import errors
-from modguard import filesystem as fs
-from modguard.check import check
-from modguard.constants import MODULE_FILE_NAME, CONFIG_FILE_NAME
-from modguard.core import ProjectConfig, ScopeDependencyRules
+from tach import errors
+from tach import filesystem as fs
+from tach.check import check
+from tach.constants import PACKAGE_FILE_NAME, CONFIG_FILE_NAME
+from tach.core import ProjectConfig, ScopeDependencyRules
 
-__module_yml_template = """tags: ['{dir_name}']\n"""
+__package_yml_template = """tags: ['{dir_name}']\n"""
 
 
 @dataclass
-class ModuleInitResult:
-    module_paths: list[str] = field(default_factory=list)
+class PackageInitResult:
+    package_paths: list[str] = field(default_factory=list)
     warnings: list[str] = field(default_factory=list)
 
 
-def init_modules(
+def init_packages(
     root: str, depth: int, exclude_paths: Optional[list[str]] = None
-) -> ModuleInitResult:
-    module_paths: list[str] = []
+) -> PackageInitResult:
+    package_paths: list[str] = []
     warnings: list[str] = []
     for dir_path in fs.walk_pypackages(root, depth=depth, exclude_paths=exclude_paths):
-        module_yml_path = os.path.join(dir_path, f"{MODULE_FILE_NAME}.yml")
-        module_paths.append(dir_path)
-        if os.path.exists(module_yml_path):
-            warnings.append(f"Module file '{module_yml_path}' already exists.")
+        package_yml_path = os.path.join(dir_path, f"{PACKAGE_FILE_NAME}.yml")
+        package_paths.append(dir_path)
+        if os.path.exists(package_yml_path):
+            warnings.append(f"Package file '{package_yml_path}' already exists.")
             continue
-        module_yml_content = __module_yml_template.format(
+        package_yml_content = __package_yml_template.format(
             dir_name=dir_path.replace(os.path.sep, ".")
         )
-        fs.write_file(module_yml_path, module_yml_content)
+        fs.write_file(package_yml_path, package_yml_content)
 
-    return ModuleInitResult(module_paths=module_paths, warnings=warnings)
+    return PackageInitResult(package_paths=package_paths, warnings=warnings)
 
 
 @dataclass
 class InitRootResult:
     warnings: list[str] = field(default_factory=list)
 
 
@@ -61,50 +61,55 @@
                     error.source_tag, ScopeDependencyRules(depends_on=[])
                 ).depends_on
             )
             project_config.constraints[error.source_tag] = ScopeDependencyRules(
                 depends_on=list(existing_dependencies | set(error.invalid_tags))
             )
 
-    modguard_yml_path = os.path.join(root, f"{CONFIG_FILE_NAME}.yml")
-    modguard_yml_content = yaml.dump(project_config.model_dump())
-    fs.write_file(modguard_yml_path, modguard_yml_content)
+    tach_yml_path = os.path.join(root, f"{CONFIG_FILE_NAME}.yml")
+    tach_yml_content = yaml.dump(project_config.model_dump())
+    fs.write_file(tach_yml_path, tach_yml_content)
 
     check_errors = check(
         root, project_config=project_config, exclude_paths=exclude_paths
     )
     if check_errors:
         return InitRootResult(
             warnings=[
-                "Could not auto-detect all dependencies, use 'modguard check' to finish initialization manually."
+                "Could not auto-detect all dependencies, use 'tach check' to finish initialization manually."
             ]
         )
 
     return InitRootResult(warnings=[])
 
 
 def init_project(
     root: str, depth: Optional[int] = None, exclude_paths: Optional[list[str]] = None
 ) -> list[str]:
     if not os.path.isdir(root):
-        raise errors.ModguardSetupError(f"The path {root} is not a directory.")
+        raise errors.TachSetupError(f"The path {root} is not a directory.")
+
+    if exclude_paths is None:
+        exclude_paths = ["tests/", "docs/"]
 
     warnings: list[str] = []
 
     if depth is None:
-        module_init_result = init_modules(root, depth=1, exclude_paths=exclude_paths)
-        warnings.extend(module_init_result.warnings)
-        if len(module_init_result.module_paths) == 1:
-            result = init_modules(
-                module_init_result.module_paths[0], depth=1, exclude_paths=exclude_paths
+        package_init_result = init_packages(root, depth=1, exclude_paths=exclude_paths)
+        warnings.extend(package_init_result.warnings)
+        if len(package_init_result.package_paths) == 1:
+            result = init_packages(
+                package_init_result.package_paths[0],
+                depth=1,
+                exclude_paths=exclude_paths,
             )
             warnings.extend(result.warnings)
     else:
-        module_init_result = init_modules(
+        package_init_result = init_packages(
             root, depth=depth, exclude_paths=exclude_paths
         )
-        warnings.extend(module_init_result.warnings)
+        warnings.extend(package_init_result.warnings)
 
     init_root_result = init_root(root, exclude_paths=exclude_paths)
     warnings.extend(init_root_result.warnings)
 
     return warnings
```

### Comparing `tach-0.0.0/modguard/loading.py` & `tach-0.1.0/tach/loading.py`

 * *Files identical despite different names*

### Comparing `tach-0.0.0/modguard/parsing/config.py` & `tach-0.1.0/tach/parsing/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Optional
 
 import yaml
 
-from modguard.core import ProjectConfig, ModuleConfig
-from modguard import filesystem as fs
+from tach.core import ProjectConfig, PackageConfig
+from tach import filesystem as fs
 
 
 def parse_project_config(root: str = ".") -> ProjectConfig:
     file_path = fs.validate_project_config_path(root)
     with open(file_path, "r") as f:
         result = yaml.safe_load(f)
         if not result or not isinstance(result, dict):
-            raise ValueError(f"Empty or invalid module config file: {file_path}")
+            raise ValueError(f"Empty or invalid project config file: {file_path}")
     # We want to error on type issues here for now
     project_config = ProjectConfig(**result)  # type: ignore
     return project_config
 
 
-def parse_module_config(root: str = ".") -> Optional[ModuleConfig]:
-    file_path = fs.validate_module_config(root)
+def parse_package_config(root: str = ".") -> Optional[PackageConfig]:
+    file_path = fs.validate_package_config(root)
     if file_path:
         with open(file_path, "r") as f:
             result = yaml.safe_load(f)
             if not result or not isinstance(result, dict):
-                raise ValueError(f"Empty or invalid module config file: {file_path}")
+                raise ValueError(f"Empty or invalid package config file: {file_path}")
         # We want to error on type issues here for now
-        return ModuleConfig(**result)  # type: ignore
+        return PackageConfig(**result)  # type: ignore
```

### Comparing `tach-0.0.0/modguard/parsing/imports.py` & `tach-0.1.0/tach/parsing/imports.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import ast
 import re
 from typing import Optional
 from dataclasses import dataclass, field
 
-from modguard import filesystem as fs
+from tach import filesystem as fs
 
 
 @dataclass
 class IgnoreDirective:
     lineno: int
     modules: list[str] = field(default_factory=list)
 
 
-MODGUARD_IGNORE_REGEX = re.compile(r"# *modguard-ignore(( [\w.]+)*)$")
+TACH_IGNORE_REGEX = re.compile(r"# *tach-ignore(( [\w.]+)*)$")
 
 
 def get_ignore_directives(file_content: str) -> dict[int, IgnoreDirective]:
     ignores: dict[int, IgnoreDirective] = {}
     lines = file_content.splitlines()
     for lineno, line in enumerate(lines):
         normal_lineno = lineno + 1
-        match = MODGUARD_IGNORE_REGEX.match(line)
+        match = TACH_IGNORE_REGEX.match(line)
         if match:
             ignored_modules = match.group(1)
             if ignored_modules:
                 ignores[normal_lineno] = IgnoreDirective(
                     lineno=lineno + 1, modules=ignored_modules.split()
                 )
             else:
@@ -71,15 +71,15 @@
         if ignored_modules is not None and len(ignored_modules) == 0:
             # Empty ignore list signifies blanket ignore of following import
             return
 
         for name_node in node.names:
             local_mod_path = f"{'.' * node.level}{node.module or ''}.{name_node.asname or name_node.name}"
             if ignored_modules is not None and (local_mod_path in ignored_modules):
-                # This import is ignored by a modguard-ignore directive
+                # This import is ignored by a tach-ignore directive
                 continue
 
             global_mod_path = (
                 f"{base_mod_path}.{name_node.name}" if node.module else name_node.name
             )
             if fs.is_project_import(self.project_root, global_mod_path):
                 self.imports.append(global_mod_path)
```

### Comparing `tach-0.0.0/modguard/parsing/interface.py` & `tach-0.1.0/tach/parsing/interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import ast
 import os
 from typing import Any
 
-from modguard import filesystem as fs
-from modguard.parsing.ast_visitor import EarlyExitNodeVisitor
+from tach import filesystem as fs
+from tach.parsing.ast_visitor import EarlyExitNodeVisitor
 
 
 class InterfaceVisitor(EarlyExitNodeVisitor):
     def __init__(self, *args: Any, **kwargs: Any):
         super().__init__(*args, **kwargs)
         self.members: list[str] = []
```

### Comparing `tach-0.0.0/pyproject.toml` & `tach-0.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "tach"
-version = "0.0.0"
+version = "0.1.0"
 authors = [
   { name="Caelean Barnes", email="caeleanb@gmail.com" },
   { name="Evan Doyle", email="evanmdoyle@gmail.com" },
 ]
-description = "A Python tool to maintain clean dependencies across python modules."
+description = "A Python tool to maintain a modular package architecture."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
     "Development Status :: 4 - Beta",
@@ -25,26 +25,26 @@
     "Topic :: Software Development :: Quality Assurance",
 ]
 dependencies = [
     "pyyaml==6.0.1",
     "pydantic==2.7.1",
     "stdlib-list==0.10.0"
 ]
-keywords = ['python', 'module', 'guard', 'enforcement', 'enforcer', 'decorator', 'subclass', 'domain', 'architecture']
+keywords = ['python', 'module', 'package', 'guard', 'enforcement', 'boundary', 'enforcer', 'domain', 'architecture']
 
 
 [project.urls]
-Homepage = "https://github.com/never-over/modguard"
-Issues = "https://github.com/never-over/modguard/issues"
+Homepage = "https://github.com/never-over/tach"
+Issues = "https://github.com/never-over/tach/issues"
 
 
 [tool.pyright]
-include = ["modguard"]
+include = ["tach"]
 exclude = ["**/__pycache__", ".venv"]
-strict = ["modguard"]
+strict = ["tach"]
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project.scripts]
-modguard = "modguard.cli:main"
+tach = "tach.cli:main"
```

### Comparing `tach-0.0.0/tests/test_check.py` & `tach-0.1.0/tests/test_check.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import pytest
-from modguard.core import (
-    ModuleConfig,
-    ModuleTrie,
-    ModuleNode,
+from tach.core import (
+    PackageConfig,
+    PackageTrie,
+    PackageNode,
     ProjectConfig,
     ScopeDependencyRules,
 )
-from modguard.check import check_import
+from tach.check import check_import
 
 
 @pytest.fixture
-def test_config() -> ModuleConfig:
-    return ModuleConfig(tags=["test"], strict=False)
+def test_config() -> PackageConfig:
+    return PackageConfig(tags=["test"], strict=False)
 
 
 @pytest.fixture
 def project_config() -> ProjectConfig:
     return ProjectConfig(
         constraints={
             "domain_one": ScopeDependencyRules(
@@ -24,52 +24,52 @@
             "domain_two": ScopeDependencyRules(depends_on=["domain_one"]),
             "domain_three": ScopeDependencyRules(depends_on=[]),
         }
     )
 
 
 @pytest.fixture
-def module_trie() -> ModuleTrie:
-    return ModuleTrie(
-        root=ModuleNode(
+def package_trie() -> PackageTrie:
+    return PackageTrie(
+        root=PackageNode(
             is_end_of_path=False,
             full_path="",
             config=None,
             children={
-                "domain_one": ModuleNode(
+                "domain_one": PackageNode(
                     is_end_of_path=True,
                     full_path="domain_one",
-                    config=ModuleConfig(tags=["domain_one"], strict=True),
+                    config=PackageConfig(tags=["domain_one"], strict=True),
                     interface_members=["public_fn"],
                     children={
-                        "subdomain": ModuleNode(
+                        "subdomain": PackageNode(
                             is_end_of_path=True,
                             full_path="domain_one.subdomain",
-                            config=ModuleConfig(tags=["domain_one"], strict=True),
+                            config=PackageConfig(tags=["domain_one"], strict=True),
                             children={},
                         )
                     },
                 ),
-                "domain_two": ModuleNode(
+                "domain_two": PackageNode(
                     is_end_of_path=True,
                     full_path="domain_two",
-                    config=ModuleConfig(tags=["domain_two"], strict=False),
+                    config=PackageConfig(tags=["domain_two"], strict=False),
                     children={
-                        "subdomain": ModuleNode(
+                        "subdomain": PackageNode(
                             is_end_of_path=True,
                             full_path="domain_two.subdomain",
-                            config=ModuleConfig(tags=["domain_two"], strict=False),
+                            config=PackageConfig(tags=["domain_two"], strict=False),
                             children={},
                         )
                     },
                 ),
-                "domain_three": ModuleNode(
+                "domain_three": PackageNode(
                     is_end_of_path=True,
                     full_path="domain_three",
-                    config=ModuleConfig(tags=["domain_three"], strict=False),
+                    config=PackageConfig(tags=["domain_three"], strict=False),
                     children={},
                 ),
             },
         )
     )
 
 
@@ -91,16 +91,16 @@
         ("domain_two.subdomain", "domain_one.core", False),
         ("domain_two", "domain_three", False),
         ("domain_two", "domain_two.subdomain", False),
         ("external", "domain_three", False),
     ],
 )
 def test_check_import(
-    project_config, module_trie, file_mod_path, import_mod_path, expected_result
+    project_config, package_trie, file_mod_path, import_mod_path, expected_result
 ):
     result = check_import(
         project_config=project_config,
-        module_trie=module_trie,
+        package_trie=package_trie,
         file_mod_path=file_mod_path,
         import_mod_path=import_mod_path,
     )
     assert result.ok == expected_result
```

### Comparing `tach-0.0.0/tests/test_cli.py` & `tach-0.1.0/tests/test_cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,100 +1,91 @@
 from unittest.mock import Mock
 import pytest
 
-from modguard import cli
-from modguard.check import ErrorInfo
-from modguard.constants import CONFIG_FILE_NAME
-from modguard.core import ProjectConfig
+from tach import cli
+from tach.check import ErrorInfo
+from tach.constants import CONFIG_FILE_NAME
+from tach.core import ProjectConfig
 
 
 @pytest.fixture
 def mock_check(mocker) -> Mock:
     mock = Mock(return_value=[])  # default to a return with no errors
-    mocker.patch("modguard.cli.check", mock)
+    mocker.patch("tach.cli.check", mock)
     return mock
 
 
 @pytest.fixture
 def mock_isdir(mocker) -> None:
     def mock_isdir(path: str) -> bool:
         if path == "valid_dir":
             return True
         else:
             return False
 
-    mocker.patch("modguard.filesystem.project.os.path.isdir", mock_isdir)
+    mocker.patch("tach.filesystem.project.os.path.isdir", mock_isdir)
 
 
 @pytest.fixture
 def mock_path_exists(mocker) -> None:
     def mock_path_exists(path: str) -> bool:
         if CONFIG_FILE_NAME in path:
             return True
         else:
             return False
 
-    mocker.patch("modguard.filesystem.project.os.path.exists", mock_path_exists)
+    mocker.patch("tach.filesystem.project.os.path.exists", mock_path_exists)
 
 
 @pytest.fixture
 def mock_project_config(mocker) -> None:
     def mock_project_config() -> ProjectConfig:
         return ProjectConfig()
 
-    mocker.patch("modguard.cli.parse_project_config", mock_project_config)
+    mocker.patch("tach.cli.parse_project_config", mock_project_config)
 
 
-def test_execute_with_modguard_yml(
+def test_execute_with_tach_yml(
     capfd, mock_path_exists, mock_check, mock_project_config
 ):
     # Test with a valid path as mocked
-    args = cli.parse_arguments(["check"])
+    args, _ = cli.parse_arguments(["check"])
     assert args.command == "check"
     with pytest.raises(SystemExit) as sys_exit:
-        cli.modguard_check()
+        cli.tach_check()
     captured = capfd.readouterr()
     assert sys_exit.value.code == 0
     assert "✅" in captured.out
-    assert "All modules safely guarded!" in captured.out
+    assert "All package dependencies validated!" in captured.out
 
 
 def test_execute_with_error(capfd, mock_path_exists, mock_check, mock_project_config):
     # Mock an error returned from check
     location = "valid_dir/file.py"
     message = "Import valid_dir in valid_dir/file.py is blocked by boundary"
     mock_check.return_value = [
         ErrorInfo(
             exception_message="Import valid_dir in valid_dir/file.py is blocked by boundary",
         )
     ]
     with pytest.raises(SystemExit) as sys_exit:
-        cli.modguard_check()
+        cli.tach_check()
     captured = capfd.readouterr()
     assert sys_exit.value.code == 1
     assert location in captured.err
     assert message in captured.err
 
 
-def test_execute_with_no_modguard_yml(capfd):
+def test_execute_with_no_tach_yml(capfd):
     with pytest.raises(SystemExit) as sys_exit:
-        # Test with no modguard.yml mocked
+        # Test with no tach.yml mocked
         cli.parse_arguments(["check"])
     captured = capfd.readouterr()
     assert sys_exit.value.code == 1
-    assert "modguard.(yml|yaml) not found" in captured.err
-
-
-def test_show_with_no_modguard_yml(capfd):
-    with pytest.raises(SystemExit) as sys_exit:
-        # Test with no modguard.yml mocked
-        cli.parse_arguments(["show"])
-    captured = capfd.readouterr()
-    assert sys_exit.value.code == 1
-    assert "modguard.(yml|yaml) not found" in captured.err
+    assert "tach.(yml|yaml) not found" in captured.err
 
 
 def test_invalid_command(capfd):
     with pytest.raises(SystemExit) as sys_exit:
         # Test with an invalid command
         cli.parse_arguments(["help"])
     captured = capfd.readouterr()
@@ -103,14 +94,14 @@
 
 
 def test_execute_with_valid_exclude(
     capfd, mock_isdir, mock_path_exists, mock_check, mock_project_config
 ):
     with pytest.raises(SystemExit) as sys_exit:
         # Test with a valid path as mocked
-        args = cli.parse_arguments(["check", "--exclude", "valid_dir"])
+        args, _ = cli.parse_arguments(["check", "--exclude", "valid_dir"])
         exclude_paths = args.exclude.split(",")
-        cli.modguard_check(exclude_paths=exclude_paths)
+        cli.tach_check(exclude_paths=exclude_paths)
     captured = capfd.readouterr()
     assert sys_exit.value.code == 0
     assert "✅" in captured.out
-    assert "All modules safely guarded!" in captured.out
+    assert "All package dependencies validated!" in captured.out
```

### Comparing `tach-0.0.0/tests/test_init.py` & `tach-0.1.0/tests/test_init.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 import tempfile
 import shutil
 import os
-from modguard import errors, filesystem as fs
-from modguard.init import init_project
+from tach import errors, filesystem as fs
+from tach.init import init_project
 
 
 def init_project_from_root(root) -> None:
     # Save the current working directory
     saved_directory = os.getcwd()
     try:
         # Navigate to the root directory and call init_project
@@ -63,9 +63,9 @@
     # Call init_project with the test root
     init_project_from_root(test_root)
 
     # TODO: test new behavior
 
 
 def test_init_project_with_invalid_root():
-    with pytest.raises(errors.ModguardSetupError):
+    with pytest.raises(errors.TachSetupError):
         init_project("nonexistent_directory")
```

### Comparing `tach-0.0.0/tests/test_module_trie.py` & `tach-0.1.0/tests/test_module_trie.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,113 +1,113 @@
 import pytest
 
-from modguard.core import ModuleTrie, ModuleNode, ModuleConfig
+from tach.core import PackageTrie, PackageNode, PackageConfig
 
 
 @pytest.fixture
-def test_config() -> ModuleConfig:
-    return ModuleConfig(tags=["test"], strict=False)
+def test_config() -> PackageConfig:
+    return PackageConfig(tags=["test"], strict=False)
 
 
 @pytest.fixture
-def module_trie() -> ModuleTrie:
-    return ModuleTrie(
-        root=ModuleNode(
+def package_trie() -> PackageTrie:
+    return PackageTrie(
+        root=PackageNode(
             is_end_of_path=False,
             full_path="",
             config=None,
             children={
-                "domain_one": ModuleNode(
+                "domain_one": PackageNode(
                     is_end_of_path=True,
                     full_path="domain_one",
-                    config=ModuleConfig(tags=["test"], strict=False),
+                    config=PackageConfig(tags=["test"], strict=False),
                     children={
-                        "subdomain": ModuleNode(
+                        "subdomain": PackageNode(
                             is_end_of_path=True,
                             full_path="domain_one.subdomain",
-                            config=ModuleConfig(tags=["test"], strict=False),
+                            config=PackageConfig(tags=["test"], strict=False),
                             children={},
                         )
                     },
                 ),
-                "domain_two": ModuleNode(
+                "domain_two": PackageNode(
                     is_end_of_path=True,
                     full_path="domain_two",
-                    config=ModuleConfig(tags=["test"], strict=False),
+                    config=PackageConfig(tags=["test"], strict=False),
                     children={
-                        "subdomain": ModuleNode(
+                        "subdomain": PackageNode(
                             is_end_of_path=True,
                             full_path="domain_two.subdomain",
-                            config=ModuleConfig(tags=["test"], strict=False),
+                            config=PackageConfig(tags=["test"], strict=False),
                             children={},
                         )
                     },
                 ),
-                "domain_three": ModuleNode(
+                "domain_three": PackageNode(
                     is_end_of_path=True,
                     full_path="domain_three",
-                    config=ModuleConfig(tags=["test"], strict=False),
+                    config=PackageConfig(tags=["test"], strict=False),
                     children={},
                 ),
             },
         )
     )
 
 
 def test_iterate_over_empty_trie():
-    assert list(ModuleTrie()) == []
+    assert list(PackageTrie()) == []
 
 
-def test_iterate_over_populated_trie(module_trie):
-    assert set((node.full_path for node in module_trie)) == {
+def test_iterate_over_populated_trie(package_trie):
+    assert set((node.full_path for node in package_trie)) == {
         "domain_one",
         "domain_one.subdomain",
         "domain_two",
         "domain_two.subdomain",
         "domain_three",
     }
 
 
-def test_get_nonexistent_path(module_trie):
-    assert module_trie.get("fakepath") is None
+def test_get_nonexistent_path(package_trie):
+    assert package_trie.get("fakepath") is None
 
 
 def test_get_nonexistent_empty_path():
-    trie = ModuleTrie()
+    trie = PackageTrie()
     assert trie.get("") is None
 
 
-def test_get_actual_path(module_trie):
-    assert module_trie.get("domain_one") is not None
+def test_get_actual_path(package_trie):
+    assert package_trie.get("domain_one") is not None
 
 
 def test_insert_empty_path(test_config):
-    trie = ModuleTrie()
+    trie = PackageTrie()
     trie.insert(test_config, "", [])
     assert set((node.full_path for node in trie)) == {""}
 
 
 def test_insert_single_level_path(test_config):
-    trie = ModuleTrie()
+    trie = PackageTrie()
     trie.insert(test_config, "domain", [])
     assert set((node.full_path for node in trie)) == {"domain"}
 
 
 def test_insert_multi_level_path(test_config):
-    trie = ModuleTrie()
+    trie = PackageTrie()
     trie.insert(test_config, "domain.subdomain", [])
     assert set((node.full_path for node in trie)) == {"domain.subdomain"}
 
 
-def test_find_nearest_at_root(module_trie):
-    module = module_trie.find_nearest("other_domain")
-    assert module is None
+def test_find_nearest_at_root(package_trie):
+    package = package_trie.find_nearest("other_domain")
+    assert package is None
 
 
-def test_find_nearest_in_single_domain(module_trie):
-    module = module_trie.find_nearest("domain_one.thing")
-    assert module.full_path == "domain_one"
+def test_find_nearest_in_single_domain(package_trie):
+    package = package_trie.find_nearest("domain_one.thing")
+    assert package.full_path == "domain_one"
 
 
-def test_find_nearest_in_nested_domain(module_trie):
-    module = module_trie.find_nearest("domain_two.subdomain.thing")
-    assert module.full_path == "domain_two.subdomain"
+def test_find_nearest_in_nested_domain(package_trie):
+    package = package_trie.find_nearest("domain_two.subdomain.thing")
+    assert package.full_path == "domain_two.subdomain"
```

### Comparing `tach-0.0.0/tests/test_parsing.py` & `tach-0.1.0/tests/test_parsing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 
 import pytest
 from pydantic import ValidationError
 
-from modguard.check import check, ErrorInfo
-from modguard.core.config import ModuleConfig, ScopeDependencyRules, ProjectConfig
-from modguard.parsing.config import parse_project_config, parse_module_config
-from modguard.filesystem import file_to_module_path
-from modguard import filesystem as fs
+from tach.check import check, ErrorInfo
+from tach.core.config import PackageConfig, ScopeDependencyRules, ProjectConfig
+from tach.parsing.config import parse_project_config, parse_package_config
+from tach.filesystem import file_to_module_path
+from tach import filesystem as fs
 
 
 def test_file_to_mod_path():
     assert file_to_module_path("__init__.py") == ""
     assert file_to_module_path("domain_one/__init__.py") == "domain_one"
     assert file_to_module_path("domain_one/interface.py") == "domain_one.interface"
 
@@ -43,47 +43,47 @@
         )
         assert results == []
     finally:
         # Make sure not to dirty the test directory state
         fs.chdir(current_dir)
 
 
-def test_parse_valid_strict_module_config():
-    result = parse_module_config("example/valid/domain_one")
-    assert result == ModuleConfig(strict=True, tags=["one"])
+def test_parse_valid_strict_package_config():
+    result = parse_package_config("example/valid/domain_one")
+    assert result == PackageConfig(strict=True, tags=["one"])
 
 
-def test_parse_valid_multi_tag_module_config():
-    result = parse_module_config("example/valid/domain_two")
-    assert result == ModuleConfig(strict=False, tags=["two", "shared"])
+def test_parse_valid_multi_tag_package_config():
+    result = parse_package_config("example/valid/domain_two")
+    assert result == PackageConfig(strict=False, tags=["two", "shared"])
 
 
-def test_module_with_no_config():
-    result = parse_module_config("example/")
+def test_package_with_no_config():
+    result = parse_package_config("example/")
     assert result is None
 
 
 def test_invalid_project_config():
     with pytest.raises(ValidationError):
         parse_project_config("example/invalid/")
 
 
 def test_empty_project_config():
     with pytest.raises(ValueError):
         parse_project_config("example/invalid/empty")
 
 
-def test_invalid_module_config():
+def test_invalid_package_config():
     with pytest.raises(ValidationError):
-        parse_module_config("example/invalid")
+        parse_package_config("example/invalid")
 
 
-def test_empty_module_config():
+def test_empty_package_config():
     with pytest.raises(ValueError):
-        parse_module_config("example/invalid")
+        parse_package_config("example/invalid")
 
 
 def test_exclude_hidden_paths_fails():
     current_dir = os.getcwd()
     hidden_project = "./example/invalid/hidden/"
     fs.chdir(hidden_project)
     try:
@@ -96,16 +96,16 @@
         )
         assert len(results) == 1
         assert results[0] == ErrorInfo(
             location="hidden",
             import_mod_path="",
             source_tag="",
             allowed_tags=[],
-            exception_message="Module 'unhidden' is in strict mode. Only imports from the root of"
-            " this module are allowed. The import 'unhidden.secret.shhhh' (in 'hidden') is not included in __all__.",
+            exception_message="Package 'unhidden' is in strict mode. Only imports from the root of"
+            " this package are allowed. The import 'unhidden.secret.shhhh' (in 'hidden') is not included in __all__.",
         )
 
         project_config.exclude_hidden_paths = True
         assert check(".", project_config, exclude_hidden_paths=True) == []
     finally:
         # Make sure not to dirty the test directory state
         fs.chdir(current_dir)
```

