# Comparing `tmp/skeletonkey-0.2.11.tar.gz` & `tmp/skeletonkey-0.2.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skeletonkey-0.2.11.tar", last modified: Mon Apr 22 19:24:44 2024, max compression
+gzip compressed data, was "skeletonkey-0.2.12.tar", last modified: Tue Apr 30 18:37:28 2024, max compression
```

## Comparing `skeletonkey-0.2.11.tar` & `skeletonkey-0.2.12.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:24:44.697034 skeletonkey-0.2.11/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-22 19:24:42.000000 skeletonkey-0.2.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-04-22 19:24:44.697034 skeletonkey-0.2.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-04-22 19:24:42.000000 skeletonkey-0.2.11/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 19:24:44.697034 skeletonkey-0.2.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-22 19:24:44.000000 skeletonkey-0.2.11/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:24:44.693033 skeletonkey-0.2.11/skeletonkey/
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-22 19:24:42.000000 skeletonkey-0.2.11/skeletonkey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14825 2024-04-22 19:24:42.000000 skeletonkey-0.2.11/skeletonkey/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-22 19:24:42.000000 skeletonkey-0.2.11/skeletonkey/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-04-22 19:24:42.000000 skeletonkey-0.2.11/skeletonkey/instantiate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:24:44.693033 skeletonkey-0.2.11/skeletonkey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-04-22 19:24:44.000000 skeletonkey-0.2.11/skeletonkey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-22 19:24:44.000000 skeletonkey-0.2.11/skeletonkey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 19:24:44.000000 skeletonkey-0.2.11/skeletonkey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-22 19:24:44.000000 skeletonkey-0.2.11/skeletonkey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-22 19:24:44.000000 skeletonkey-0.2.11/skeletonkey.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:37:28.331837 skeletonkey-0.2.12/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-30 18:37:25.000000 skeletonkey-0.2.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-04-30 18:37:28.327837 skeletonkey-0.2.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-04-30 18:37:25.000000 skeletonkey-0.2.12/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 18:37:28.331837 skeletonkey-0.2.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-30 18:37:28.000000 skeletonkey-0.2.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:37:28.327837 skeletonkey-0.2.12/skeletonkey/
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-30 18:37:25.000000 skeletonkey-0.2.12/skeletonkey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16499 2024-04-30 18:37:25.000000 skeletonkey-0.2.12/skeletonkey/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-30 18:37:25.000000 skeletonkey-0.2.12/skeletonkey/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-04-30 18:37:25.000000 skeletonkey-0.2.12/skeletonkey/instantiate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:37:28.327837 skeletonkey-0.2.12/skeletonkey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-04-30 18:37:28.000000 skeletonkey-0.2.12/skeletonkey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-30 18:37:28.000000 skeletonkey-0.2.12/skeletonkey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 18:37:28.000000 skeletonkey-0.2.12/skeletonkey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-30 18:37:28.000000 skeletonkey-0.2.12/skeletonkey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 18:37:28.000000 skeletonkey-0.2.12/skeletonkey.egg-info/top_level.txt
```

### Comparing `skeletonkey-0.2.11/LICENSE` & `skeletonkey-0.2.12/LICENSE`

 * *Files identical despite different names*

### Comparing `skeletonkey-0.2.11/PKG-INFO` & `skeletonkey-0.2.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skeletonkey
-Version: 0.2.11
+Version: 0.2.12
 Summary: A bare-bones configuration managment tool.
 Home-page: https://github.com/sizemore0125/skeletonkey
 Author: Logan Sizemore
 Author-email: sizemore0125@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `skeletonkey-0.2.11/README.md` & `skeletonkey-0.2.12/README.md`

 * *Files identical despite different names*

### Comparing `skeletonkey-0.2.11/setup.py` & `skeletonkey-0.2.12/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="skeletonkey",
-    version='v0.2.11',
+    version='v0.2.12',
     description="A bare-bones configuration managment tool.",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sizemore0125/skeletonkey",
     author="Logan Sizemore",
     author_email="sizemore0125@gmail.com",
```

### Comparing `skeletonkey-0.2.11/skeletonkey/__init__.py` & `skeletonkey-0.2.12/skeletonkey/__init__.py`

 * *Files identical despite different names*

### Comparing `skeletonkey-0.2.11/skeletonkey/config.py` & `skeletonkey-0.2.12/skeletonkey/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,15 +35,45 @@
         if len(args) == 1:
             if not isinstance(args[0], dict):
                 raise ValueError("Supplied arg must be a dictionary")
             self._init_from_dict(args[0])
         else:
             self._init_from_dict(kwargs)
 
+    def update(self, update_config: dict|'Config'):
+        """
+        Take a config in some format and place those values into the config.
+        This will overwrite values if they are present or create them if they are not.
+
+        Args:
+            update_config (dict|Config): The keys/values to place into the config. If this is a dictionary,
+            it is expected that the keys are in dot notation.
+        """
+        if not isinstance(update_config, Config):
+            update_config = config_to_nested_config(Config(update_config))
+        self._update_from_config(update_config)
+
+
+    def _update_from_config(self, update_config: 'Config'):
+        """
+        Recursively place all of the values from update_config into self, overwriting them if they
+        exist and adding them if they do not.        
+        """
+
+        for k, v in update_config.__dict__.items():
+            if isinstance(v, Config):
+                if k not in self.__dict__.keys():
+                    self[k] = Config({})
 
+                self[k]._update_from_config(update_config[k])
+            
+            else:
+                self[k] = update_config[k]
+
+        
     def _init_from_dict(self, dictionary: dict):
         """
         Initialize the config from a dictionary
 
         Args:
             dictionary (dict): The dictionary to be converted.
         """
@@ -348,25 +378,39 @@
         if isinstance(value, dict):
             add_args_from_dict(arg_parser, value, f"{prefix}{key}.")
         else:
             if key.startswith("$"):
                 if key[1:] in os.environ:
                     value = os.environ[key[1:]]
                 arg_parser.add_argument(
-                    f"--{prefix}{key[1:]}", default=value, type=type(value)
+                    f"--{prefix}{key[1:]}", default=value
                 )
             elif key.startswith("?"):
                 arg_parser.add_argument(
                     f"--{prefix}{key[1:]}", default=value, action='store_true'
                 )
             else:
                 arg_parser.add_argument(
-                    f"--{prefix}{key}", default=value, type=type(value)
+                    f"--{prefix}{key}", default=value
                 )
 
+def update_flat_config_types(flat_config: Config) -> Config:
+    """
+    Given a flat config containing some string values, parse those string values as if they were
+    yaml arguemnts into the corresponding python type and return an updated config.
+
+    Args:
+        config (Config): The flat Config whose values should be parsed
+    """
+    return Config({
+        key: yaml.safe_load(value) if isinstance(value, str) else value
+        for key, value in vars(flat_config).items()
+    })
+        
+
 
 def get_command_line_config(arg_parser: argparse.ArgumentParser, config_argument_keyword: str="config") -> Tuple[str, List[str]]:
     """
     Check to see if the user specified an alternative config via the command line. If so,
     return the path of that config, and the remaining arguments. Otherwise, return None
     and the remaining arguments.
```

### Comparing `skeletonkey-0.2.11/skeletonkey/core.py` & `skeletonkey-0.2.12/skeletonkey/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Callable, Optional
 
 from .config import (
     get_command_line_config,
     load_yaml_config,
     add_args_from_dict,
     add_yaml_extension,
+    update_flat_config_types,
     config_to_nested_config,
     Config
 )
 
 
 def get_config_dir_path(config_path: str) -> str:
     """
@@ -81,14 +82,15 @@
     config = load_yaml_config(config_path, config_name)
 
     def _parse_config(main: Callable):
         @functools.wraps(main)
         def _inner_function():
             add_args_from_dict(parser, config)
             args = parser.parse_args(remaining_args)
+            args = update_flat_config_types(args)
             args = config_to_nested_config(args)
             return main(args)
 
         return _inner_function
 
     return _parse_config
```

### Comparing `skeletonkey-0.2.11/skeletonkey/instantiate.py` & `skeletonkey-0.2.12/skeletonkey/instantiate.py`

 * *Files identical despite different names*

### Comparing `skeletonkey-0.2.11/skeletonkey.egg-info/PKG-INFO` & `skeletonkey-0.2.12/skeletonkey.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skeletonkey
-Version: 0.2.11
+Version: 0.2.12
 Summary: A bare-bones configuration managment tool.
 Home-page: https://github.com/sizemore0125/skeletonkey
 Author: Logan Sizemore
 Author-email: sizemore0125@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

