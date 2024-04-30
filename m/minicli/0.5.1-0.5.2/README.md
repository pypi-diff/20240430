# Comparing `tmp/minicli-0.5.1.tar.gz` & `tmp/minicli-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minicli-0.5.1.tar", last modified: Wed Jul 20 10:50:02 2022, max compression
+gzip compressed data, was "minicli-0.5.2.tar", last modified: Tue Apr 30 07:07:49 2024, max compression
```

## Comparing `minicli-0.5.1.tar` & `minicli-0.5.2.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2022-07-20 10:50:02.028563 minicli-0.5.1/
--rw-r--r--   0 ybon      (1000) ybon      (1000)       18 2017-08-25 15:50:17.000000 minicli-0.5.1/MANIFEST.in
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1088 2022-07-20 10:50:02.028563 minicli-0.5.1/PKG-INFO
--rw-r--r--   0 ybon      (1000) ybon      (1000)      376 2018-05-30 18:41:13.000000 minicli-0.5.1/README.md
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2022-07-20 10:50:02.028563 minicli-0.5.1/example/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      623 2018-05-30 08:45:20.000000 minicli-0.5.1/example/__init__.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2022-07-20 10:50:02.028563 minicli-0.5.1/minicli/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7590 2022-07-20 10:46:59.000000 minicli-0.5.1/minicli/__init__.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2022-07-20 10:50:02.028563 minicli-0.5.1/minicli.egg-info/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1088 2022-07-20 10:50:01.000000 minicli-0.5.1/minicli.egg-info/PKG-INFO
--rw-r--r--   0 ybon      (1000) ybon      (1000)      234 2022-07-20 10:50:02.000000 minicli-0.5.1/minicli.egg-info/SOURCES.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)        1 2022-07-20 10:50:01.000000 minicli-0.5.1/minicli.egg-info/dependency_links.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)       43 2022-07-20 10:50:01.000000 minicli-0.5.1/minicli.egg-info/requires.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)       16 2022-07-20 10:50:01.000000 minicli-0.5.1/minicli.egg-info/top_level.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)      787 2022-07-20 10:50:02.028563 minicli-0.5.1/setup.cfg
--rw-r--r--   0 ybon      (1000) ybon      (1000)       38 2020-09-03 10:58:38.000000 minicli-0.5.1/setup.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2024-04-30 07:07:49.667599 minicli-0.5.2/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)       18 2017-08-25 15:50:17.000000 minicli-0.5.2/MANIFEST.in
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1179 2024-04-30 07:07:49.667599 minicli-0.5.2/PKG-INFO
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      376 2018-05-30 18:41:13.000000 minicli-0.5.2/README.md
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2024-04-30 07:07:49.664265 minicli-0.5.2/example/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      623 2018-05-30 08:45:20.000000 minicli-0.5.2/example/__init__.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2024-04-30 07:07:49.664265 minicli-0.5.2/minicli/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8046 2024-04-30 07:05:50.000000 minicli-0.5.2/minicli/__init__.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2024-04-30 07:07:49.664265 minicli-0.5.2/minicli.egg-info/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1179 2024-04-30 07:07:49.000000 minicli-0.5.2/minicli.egg-info/PKG-INFO
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      252 2024-04-30 07:07:49.000000 minicli-0.5.2/minicli.egg-info/SOURCES.txt
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        1 2024-04-30 07:07:49.000000 minicli-0.5.2/minicli.egg-info/dependency_links.txt
+-rw-r--r--   0 ybon      (1000) ybon      (1000)       43 2024-04-30 07:07:49.000000 minicli-0.5.2/minicli.egg-info/requires.txt
+-rw-r--r--   0 ybon      (1000) ybon      (1000)       16 2024-04-30 07:07:49.000000 minicli-0.5.2/minicli.egg-info/top_level.txt
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      787 2024-04-30 07:07:49.667599 minicli-0.5.2/setup.cfg
+-rw-r--r--   0 ybon      (1000) ybon      (1000)       38 2020-09-03 10:58:38.000000 minicli-0.5.2/setup.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2024-04-30 07:07:49.664265 minicli-0.5.2/tests/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    13985 2024-04-30 07:06:13.000000 minicli-0.5.2/tests/test_cli.py
```

### Comparing `minicli-0.5.1/PKG-INFO` & `minicli-0.5.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minicli
-Version: 0.5.1
+Version: 0.5.2
 Summary: Minimalist CLI
 Home-page: https://github.com/pyrates/minicli
 Author: Pyrates
 License: WTFPL
 Keywords: cli command line interface
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -13,15 +13,17 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Requires-Dist: pytest==7.1.2; extra == "test"
 Provides-Extra: doc
+Requires-Dist: mkdocs==1.1.2; extra == "doc"
 
 # Minicli
 
 Expose functions in the command line. Minimalist and pythonic.
 
 Supports annotations and async functions.
```

### Comparing `minicli-0.5.1/example/__init__.py` & `minicli-0.5.2/example/__init__.py`

 * *Files identical despite different names*

### Comparing `minicli-0.5.1/minicli/__init__.py` & `minicli-0.5.2/minicli/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import argparse
 import asyncio
+import sys
+import warnings
 import inspect
 
 NO_DEFAULT = inspect._empty
 NARGS = ...
 _wrapper_functions = []
 _wrapper_generators = []
 _registry = []
 
 
 class Cli:
-
     def __init__(self, command, **extra):
         self.extra = extra
         self.command = command
         self.inspect()
-        if not hasattr(command, '_cli'):
+        if not hasattr(command, "_cli"):
             command._cli = self
             _registry.append(self)
 
     def __call__(self, *args, **kwargs):
         """Run original command."""
         try:
             res = self.command(*args, **kwargs)
@@ -40,114 +41,116 @@
                 args.append(value)
             else:
                 kwargs[name] = value
         return self(*args, **kwargs)
 
     @property
     def help(self):
-        return self.command.__doc__ or ''
+        return self.command.__doc__ or ""
 
     @property
     def short_help(self):
-        return self.help.split('\n\n')[0]
+        return self.help.split("\n\n")[0]
 
     def inspect(self):
         self.__doc__ = inspect.getdoc(self.command)
         self.spec = inspect.signature(self.command)
         self._async = inspect.iscoroutinefunction(self.command)
 
     def parse_parameter_help(self, name):
         try:
-            return (self.help.split(':{}:'.format(name), 1)[1]
-                             .split('\n')[0].strip())
+            return self.help.split(":{}:".format(name), 1)[1].split("\n")[0].strip()
         except IndexError:
-            return ''
+            return ""
 
-    def init_parser(self, subparsers):
-        kwargs = {
-            'help': self.short_help,
-            'conflict_handler': 'resolve'
-        }
+    def create_name(self, kwargs):
         name = self.command.__name__
-        if '_' in name:
-            kwargs['aliases'] = [name]
-            name = name.replace('_', '-')
-        kwargs['name'] = name
-        kwargs.update(self.extra.get('__self__', {}))
+        if "_" in name:
+            kwargs["aliases"] = [name]
+            name = name.replace("_", "-")
+        kwargs["name"] = name
+
+    def init_parser(self, subparsers):
+        kwargs = {"help": self.short_help, "conflict_handler": "resolve"}
+        self.create_name(kwargs)
+        kwargs.update(self.extra.get("__self__", {}))
         self.parser = subparsers.add_parser(**kwargs)
         self.set_defaults(func=self.invoke)
         for arg_name, parameter in self.spec.parameters.items():
             kwargs = {}
             default = parameter.default
             if parameter.kind == parameter.VAR_POSITIONAL:
                 default = NARGS
             type_ = parameter.annotation
             if type_ != inspect._empty:
-                kwargs['type'] = type_
+                kwargs["type"] = type_
             kwargs.update(self.extra.get(arg_name, {}))
-            if 'help' not in kwargs:
-                kwargs['help'] = self.parse_parameter_help(arg_name)
-            if 'default' not in kwargs:
-                kwargs['default'] = default
+            if "help" not in kwargs:
+                kwargs["help"] = self.parse_parameter_help(arg_name)
+            if "default" not in kwargs:
+                kwargs["default"] = default
             self.add_argument(arg_name, **kwargs)
 
     def add_argument(self, arg_name, **kwargs):
         args, kwargs = make_argument(arg_name, **kwargs)
         self.parser.add_argument(*args, **kwargs)
 
     def set_defaults(self, **kwargs):
         self.parser.set_defaults(**kwargs)
 
 
 def cli(*args, **kwargs):
     if not args:
         # User-friendlyness: allow using @cli() without any argument.
         if kwargs:  # Overriding parser arguments with only kwargs.
-            return lambda f: cli(f, '__self__', **kwargs)
+            return lambda f: cli(f, "__self__", **kwargs)
         return cli
     if not callable(args[0]):
         # We are overriding an argument from the decorator.
         return lambda f: cli(f, *args, **kwargs)
     func = args[0]
     extra = {}
-    if hasattr(func, '_cli') and len(args) > 1 and kwargs:
+    if hasattr(func, "_cli") and len(args) > 1 and kwargs:
         # Chaining cli(xxx) calls.
         extra = func._cli.extra
     if len(args) > 1:
         extra[args[1]] = kwargs
     Cli(func, **extra)
     return func
 
 
 def run(*input, **shared):
+    if len(input) and callable(input[0]):
+        _run_single(*input, **shared)
+        return
     parser = argparse.ArgumentParser(add_help=False)
     for arg_name, kwargs in shared.items():
         if not isinstance(kwargs, dict):
-            kwargs = {'default': kwargs}
+            kwargs = {"default": kwargs}
         args, kwargs = make_argument(arg_name, **kwargs)
         parser.add_argument(*args, **kwargs)
     # shared must be parsed before actual commands so they can be passed to
     # before wrapper
     parsed, extras = parser.parse_known_args(input or None)
-    shared = {k: getattr(parsed, k, None) for k in shared.keys()
-              if hasattr(parsed, k)}
+    shared = {k: getattr(parsed, k, None) for k in shared.keys() if hasattr(parsed, k)}
     # No command is known when calling parse_known_args, prevent argparse to
     # display the help and exit.
-    parser.add_argument('-h', '--help', action='store_true',
-                        help='Show this help message and exit')
-    subparsers = parser.add_subparsers(title='Available commands', metavar='')
+    parser.add_argument(
+        "-h", "--help", action="store_true", help="Show this help message and exit"
+    )
+    subparsers = parser.add_subparsers(title="Available commands", metavar="")
     for cmd in _registry:
         cmd.init_parser(subparsers)
 
     # Parse all possible args before calling any func, to prevent considering
     # a wrong argument passed by mistake as a chained command.
     commands = []
     while extras:
         command, extras = parser.parse_known_args(args=extras)
-        if not command or not hasattr(command, 'func'):
+        if not command or not hasattr(command, "func"):
             # No argument given, just display help.
             parser.print_help()
             parser.exit()  # Mimic original behaviour.
         commands.append(command)
 
     # Now call commands for real.
     prepare_wrappers(**shared)
@@ -155,17 +158,32 @@
     try:
         for command in commands:
             command.func(command, **shared)
     finally:
         call_wrappers()
 
 
+def _run_single(method, *input, **shared):
+    cli(method)
+    name = method.__name__
+    run(name, *input or sys.argv[1:], **shared)
+
+
+def command(*args, **kwargs):
+    """For pyminiCLI retrocomaptibility."""
+    warnings.warn(
+        "This function is only to ease migration "
+        " from pyminiCLI. Use run() instead.",
+        DeprecationWarning,
+    )
+    return run(*args, **kwargs)
+
+
 def wrap(func):
-    if not (inspect.isgeneratorfunction(func)
-            or inspect.isasyncgenfunction(func)):
+    if not (inspect.isgeneratorfunction(func) or inspect.isasyncgenfunction(func)):
         raise ValueError(f'"{func}" needs to yield')
     _wrapper_functions.append(func)
     return func
 
 
 def call_wrappers():
     for wrapper in _wrapper_generators:
@@ -196,30 +214,29 @@
         _wrapper_generators.append(func(*args, **kwargs))
 
 
 def make_argument(arg_name, default=NO_DEFAULT, **kwargs):
     name = kwargs.pop("name", arg_name)
     args = [name]
     if default not in (NO_DEFAULT, NARGS):
-        if '_' not in name and name[0] != 'h':
-            args.append('-{}'.format(name[0]))
-        args[0] = '--{}'.format(name.replace('_', '-'))
-        kwargs['dest'] = arg_name
-        kwargs['default'] = default
-        type_ = kwargs.pop('type',
-                           type(default) if default is not None else None)
+        if "_" not in name and name[0] != "h":
+            args.append("-{}".format(name[0]))
+        args[0] = "--{}".format(name.replace("_", "-"))
+        kwargs["dest"] = arg_name
+        kwargs["default"] = default
+        type_ = kwargs.pop("type", type(default) if default is not None else None)
         if type_ == bool:
-            action = 'store_false' if default else 'store_true'
-            kwargs['action'] = action
+            action = "store_false" if default else "store_true"
+            kwargs["action"] = action
         elif type_ in (list, tuple):
-            kwargs['action'] = 'append'
-            nargs = kwargs.get('nargs')
+            kwargs["action"] = "append"
+            nargs = kwargs.get("nargs")
             if nargs:
-                kwargs['nargs'] = nargs
+                kwargs["nargs"] = nargs
         elif callable(type_):
-            kwargs['type'] = type_
+            kwargs["type"] = type_
         elif callable(default):
-            kwargs['type'] = type_
-            kwargs['default'] = ''
+            kwargs["type"] = type_
+            kwargs["default"] = ""
     elif default == NARGS:
-        kwargs['nargs'] = '*'
+        kwargs["nargs"] = "*"
     return args, kwargs
```

### Comparing `minicli-0.5.1/minicli.egg-info/PKG-INFO` & `minicli-0.5.2/minicli.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minicli
-Version: 0.5.1
+Version: 0.5.2
 Summary: Minimalist CLI
 Home-page: https://github.com/pyrates/minicli
 Author: Pyrates
 License: WTFPL
 Keywords: cli command line interface
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -13,15 +13,17 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Requires-Dist: pytest==7.1.2; extra == "test"
 Provides-Extra: doc
+Requires-Dist: mkdocs==1.1.2; extra == "doc"
 
 # Minicli
 
 Expose functions in the command line. Minimalist and pythonic.
 
 Supports annotations and async functions.
```

### Comparing `minicli-0.5.1/setup.cfg` & `minicli-0.5.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = minicli
-version = 0.5.1
+version = 0.5.2
 description = Minimalist CLI
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pyrates/minicli
 keywords = cli command line interface
 license = WTFPL
 author = Pyrates
```

