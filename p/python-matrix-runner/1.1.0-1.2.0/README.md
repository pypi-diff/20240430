# Comparing `tmp/python-matrix-runner-1.1.0.tar.gz` & `tmp/python_matrix_runner-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-matrix-runner-1.1.0.tar", last modified: Tue May 24 08:38:58 2022, max compression
+gzip compressed data, was "python_matrix_runner-1.2.0.tar", last modified: Tue Apr 30 09:34:11 2024, max compression
```

## Comparing `python-matrix-runner-1.1.0.tar` & `python_matrix_runner-1.2.0.tar`

### file list

```diff
@@ -1,26 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 08:38:58.652888 python-matrix-runner-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1522 2022-05-24 08:38:44.000000 python-matrix-runner-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    22776 2022-05-24 08:38:58.652888 python-matrix-runner-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    21862 2022-05-24 08:38:44.000000 python-matrix-runner-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 08:38:58.648888 python-matrix-runner-1.1.0/matrix_runner/
--rw-r--r--   0 runner    (1001) docker     (121)     2926 2022-05-24 08:38:44.000000 python-matrix-runner-1.1.0/matrix_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2299 2022-05-24 08:38:44.000000 python-matrix-runner-1.1.0/matrix_runner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6218 2022-05-24 08:38:44.000000 python-matrix-runner-1.1.0/matrix_runner/_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     3804 2022-05-24 08:38:44.000000 python-matrix-runner-1.1.0/matrix_runner/action.py
--rw-r--r--   0 runner    (1001) docker     (121)     3635 2022-05-24 08:38:44.000000 python-matrix-runner-1.1.0/matrix_runner/axis.py
--rw-r--r--   0 runner    (1001) docker     (121)    11178 2022-05-24 08:38:44.000000 python-matrix-runner-1.1.0/matrix_runner/command.py
--rw-r--r--   0 runner    (1001) docker     (121)      289 2022-05-24 08:38:44.000000 python-matrix-runner-1.1.0/matrix_runner/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      963 2022-05-24 08:38:44.000000 python-matrix-runner-1.1.0/matrix_runner/filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-05-24 08:38:44.000000 python-matrix-runner-1.1.0/matrix_runner/inspect.py
--rw-r--r--   0 runner    (1001) docker     (121)     3478 2022-05-24 08:38:44.000000 python-matrix-runner-1.1.0/matrix_runner/preferences.py
--rw-r--r--   0 runner    (1001) docker     (121)     6981 2022-05-24 08:38:44.000000 python-matrix-runner-1.1.0/matrix_runner/report.py
--rw-r--r--   0 runner    (1001) docker     (121)    12627 2022-05-24 08:38:44.000000 python-matrix-runner-1.1.0/matrix_runner/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 08:38:58.652888 python-matrix-runner-1.1.0/python_matrix_runner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    22776 2022-05-24 08:38:58.000000 python-matrix-runner-1.1.0/python_matrix_runner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      591 2022-05-24 08:38:58.000000 python-matrix-runner-1.1.0/python_matrix_runner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-24 08:38:58.000000 python-matrix-runner-1.1.0/python_matrix_runner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-05-24 08:38:58.000000 python-matrix-runner-1.1.0/python_matrix_runner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-05-24 08:38:58.000000 python-matrix-runner-1.1.0/python_matrix_runner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-05-24 08:38:58.000000 python-matrix-runner-1.1.0/python_matrix_runner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-24 08:38:58.652888 python-matrix-runner-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2544 2022-05-24 08:38:44.000000 python-matrix-runner-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:34:11.157076 python_matrix_runner-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-30 09:34:03.000000 python_matrix_runner-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    24239 2024-04-30 09:34:11.157076 python_matrix_runner-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22672 2024-04-30 09:34:03.000000 python_matrix_runner-1.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:34:11.153076 python_matrix_runner-1.2.0/matrix_runner/
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-30 09:34:03.000000 python_matrix_runner-1.2.0/matrix_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-30 09:34:03.000000 python_matrix_runner-1.2.0/matrix_runner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-30 09:34:03.000000 python_matrix_runner-1.2.0/matrix_runner/_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-30 09:34:03.000000 python_matrix_runner-1.2.0/matrix_runner/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-30 09:34:03.000000 python_matrix_runner-1.2.0/matrix_runner/axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11460 2024-04-30 09:34:03.000000 python_matrix_runner-1.2.0/matrix_runner/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-30 09:34:03.000000 python_matrix_runner-1.2.0/matrix_runner/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-30 09:34:03.000000 python_matrix_runner-1.2.0/matrix_runner/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-30 09:34:03.000000 python_matrix_runner-1.2.0/matrix_runner/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-30 09:34:03.000000 python_matrix_runner-1.2.0/matrix_runner/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-04-30 09:34:03.000000 python_matrix_runner-1.2.0/matrix_runner/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13856 2024-04-30 09:34:03.000000 python_matrix_runner-1.2.0/matrix_runner/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:34:11.157076 python_matrix_runner-1.2.0/python_matrix_runner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24239 2024-04-30 09:34:11.000000 python_matrix_runner-1.2.0/python_matrix_runner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-30 09:34:11.000000 python_matrix_runner-1.2.0/python_matrix_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:34:11.000000 python_matrix_runner-1.2.0/python_matrix_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-30 09:34:11.000000 python_matrix_runner-1.2.0/python_matrix_runner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-30 09:34:11.000000 python_matrix_runner-1.2.0/python_matrix_runner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-30 09:34:11.000000 python_matrix_runner-1.2.0/python_matrix_runner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:34:11.157076 python_matrix_runner-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-30 09:34:03.000000 python_matrix_runner-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:34:11.157076 python_matrix_runner-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12264 2024-04-30 09:34:03.000000 python_matrix_runner-1.2.0/tests/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-30 09:34:03.000000 python_matrix_runner-1.2.0/tests/test_axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21290 2024-04-30 09:34:03.000000 python_matrix_runner-1.2.0/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-30 09:34:03.000000 python_matrix_runner-1.2.0/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-30 09:34:03.000000 python_matrix_runner-1.2.0/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-30 09:34:03.000000 python_matrix_runner-1.2.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-30 09:34:03.000000 python_matrix_runner-1.2.0/tests/test_matrix_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9743 2024-04-30 09:34:03.000000 python_matrix_runner-1.2.0/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16076 2024-04-30 09:34:03.000000 python_matrix_runner-1.2.0/tests/test_runner.py
```

### Comparing `python-matrix-runner-1.1.0/LICENSE` & `python_matrix_runner-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-matrix-runner-1.1.0/PKG-INFO` & `python_matrix_runner-1.2.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: python-matrix-runner
-Version: 1.1.0
-Summary: Helper to run command with matrix configurations
-Home-page: https://github.com/energy6/python-matrix-runner
-Author: Jonatan Antoni
-Author-email: jonatan@familie-antoni.de
-License: BSD 3-Clause License
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Build Tools
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
-License-File: LICENSE
-
 |build-badge| |test-badge| |cov-badge| |python-badge| |wheel-badge| |pypi-badge| |license-badge|
 
 Matrix Runner for Python
 ========================
 
 Allows easy top level command line interface generation for matrix configurations.
 
@@ -117,30 +93,34 @@
 
     if __name__ == "__main__":
         main()
 
 Can be executed as::
 
     $ ./build.py --help
-    usage: build.py [-h] [--silent | --verbose | --debug] [--pairwise] [--slice <HERE>/<TOTAL>]
-                    [--alpha ALPHA] action [action ...]
+    usage: build.py [-h] [--silent | --verbose | --debug] [--pairwise] [--slice <HERE>/<TOTAL>] [--extra-args EXTRA_ARGS] 
+                    [--alpha ALPHA] [--dump-args DUMP_ARGS] action [action ...]
 
     positional arguments:
       action                Action(s) to run: dump
 
     optional arguments:
       -h, --help            show this help message and exit
       --silent              Silent mode, only errors are shown.
       --verbose             Verbose log output.
       --debug               Debug log output.
       --pairwise, -2        Reduce number of combinations using pairwise algorithm.
       --slice <HERE>/<TOTAL>
                             Cut set of combinations into <TOTAL> number of slices and run ony <HERE>th one.
+      --extra-args EXTRA_ARGS
+                            Extra arguments for all actions.
       --alpha ALPHA, -a ALPHA
                             A configuration axis: value1|v1, value2|v2, value3|v3
+      --dump-args DUMP_ARGS 
+                            Extra arguments for dump action.
 
     $ ./build.py -a v[23] dump
     [value2](dump:dump_config) /usr/bin/sh -c echo 'Config(alpha=<MyAlphaAxisValue.Value2: ('value2', 'v2')>)'
     [value2](dump:dump_config) (Hello, World): Config(alpha=<MyAlphaAxisValue.Value2: (value2, v2)>)
     [value2](dump:dump_config) /usr/bin/sh succeeded with exit code 0
     [value3](dump:dump_config) /usr/bin/sh -c echo 'Config(alpha=<MyAlphaAxisValue.Value3: ('value3', 'v3')>)'
     [value3](dump:dump_config) Config(alpha=<MyAlphaAxisValue.Value3: (value3, v3)>)
@@ -208,15 +188,15 @@
 ~~~~~~
 
 Actions are used to capture different workflow steps, such as `compile` and
 `run` for unit tests. A step is simply defined by decorating a function
 with ``@matrix_action``::
 
     @matrix_action
-    def dump(config: Config <, results: List[Result]>):
+    def dump(config: Config<, results: List[Result]><, extra_args: List[str] = None>):
         """Dump configuration to console"""
         pre_process()
         yield dump_config(config, 'Hello', 'World')
         post_process(<results>)
 
 The function itself needs to return a ``Generator`` generating a list of
 Command_'s. The function is called once in preparation for each matrix
@@ -224,14 +204,17 @@
 
 The ``config`` argument gives access to the selected _Config permutation. It
 can be used to generate the commands depending on the actual configuration.
 
 The optional ``results`` argument can be used to gain access to the list of
 Command_ results gathered so far, e.g. for adding post-processing.
 
+The optional ``extra_args`` named-argument can be used to receive a list additional
+command line arguments provided via `--extra-args` or `--<action>-args`.
+
 The function needs to ``yield`` Command_'s, i.e. ``dump_config`` needs to be
 an annotated command function. Pre and post processing code can be added
 around.
 
 Command
 ~~~~~~~
 
@@ -454,15 +437,16 @@
 ~~~~~~~~~~~~
 
 Running one or more configurations from the command line using Matrix Runner is
 trivial. The generated interface looks like this::
 
     $ ./build.py --help
     usage: build.py [-h] [--silent | --verbose | --debug] [--pairwise] [--slice <HERE>/<TOTAL>]
-                    [[--<axis> <AXIS>] ...] action [action ...]
+                    [--extra-args EXTRA_ARGS] [[--<axis> <AXIS>] ...] 
+                    [--<action>-args <ACTION>_ARGS] action [action ...]
 
 The positional argument ``action`` can be one or multiple define Action_'s to
 be executed in the given order, e.g. either ``build`` and ``run`` separately or
 both in a sequence.
 
 The optional arguments are a combination of static ones used to parametrize
 Matrix Runner itself and dynamic ones generated from the defined Axis_:
@@ -475,20 +459,24 @@
   algorithm. This enables combinatorial `all-pairs testing`_ to reduce the
   overall number of configuration in logarithmic manner while retaining a high
   probability of detecting issues.
 - ``--slice <HERE>/<TOTAL>`` cuts the set of combinations into ``TOTAL`` number
   of slices and executes only the ``HERE``'th one. This can be used to run the
   overall set of combinations in parallel. Slicing is applied after
   ``--pairwise`` reduction.
+- ``--extra-args EXTRA_ARGS`` can be used to provide custom arguments passed
+  on to all action functions taking an `extra_args`` named-argument.
 - ``-<a> <AXIS>``, ``--<axis> <AXIS>`` reduce number of combinations to
   selected ``AXIS`` values for ``axis`` Axis values can be given as one of
   their string representations *or* an fnmatch.fnmatch_ pattern matching at
   least one of these. In case of pattern matching *all* matching values are
   selected. This argument can be given multiple time which adds the values in a
   cumulative way.
+- ``--<action>-args <ACTION>_ARGS`` can be used to provide custom arguments passed
+  specifically to the <action> functions taking an `extra_args`` named-argument.
 
 The console output has two parts. While executing the actions the output from
 the associated commands is forwarded like this::
 
     [<AXIS>](<ACTION>) <pre processing log>
     [<AXIS>](<ACTION>:<COMMAND>) <command line>
     [<AXIS>](<ACTION>:<COMMAND>) <stdout/stderr from command>
```

### Comparing `python-matrix-runner-1.1.0/README.rst` & `python_matrix_runner-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,48 @@
+Metadata-Version: 2.1
+Name: python-matrix-runner
+Version: 1.2.0
+Summary: Helper to run command with matrix configurations
+Home-page: https://github.com/energy6/python-matrix-runner
+Author: Jonatan Antoni
+Author-email: jonatan@familie-antoni.de
+License: BSD 3-Clause License
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Build Tools
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: allpairspy~=2.5
+Requires-Dist: ansicolors~=1.1
+Requires-Dist: colorama~=0.4
+Requires-Dist: colorlog~=6.7
+Requires-Dist: filelock~=3.12
+Requires-Dist: junitparser~=2.8
+Requires-Dist: lxml~=4.9
+Requires-Dist: parameterized~=0.9
+Requires-Dist: psutil~=5.9
+Requires-Dist: tabulate~=0.9
+Provides-Extra: dev
+Requires-Dist: coverage~=6.5; extra == "dev"
+Requires-Dist: pylint~=2.17; extra == "dev"
+Requires-Dist: restructuredtext_lint~=1.4; extra == "dev"
+Requires-Dist: setuptools~=68.2; extra == "dev"
+Requires-Dist: unittest-xml-reporting~=3.2; extra == "dev"
+
 |build-badge| |test-badge| |cov-badge| |python-badge| |wheel-badge| |pypi-badge| |license-badge|
 
 Matrix Runner for Python
 ========================
 
 Allows easy top level command line interface generation for matrix configurations.
 
@@ -93,30 +134,34 @@
 
     if __name__ == "__main__":
         main()
 
 Can be executed as::
 
     $ ./build.py --help
-    usage: build.py [-h] [--silent | --verbose | --debug] [--pairwise] [--slice <HERE>/<TOTAL>]
-                    [--alpha ALPHA] action [action ...]
+    usage: build.py [-h] [--silent | --verbose | --debug] [--pairwise] [--slice <HERE>/<TOTAL>] [--extra-args EXTRA_ARGS] 
+                    [--alpha ALPHA] [--dump-args DUMP_ARGS] action [action ...]
 
     positional arguments:
       action                Action(s) to run: dump
 
     optional arguments:
       -h, --help            show this help message and exit
       --silent              Silent mode, only errors are shown.
       --verbose             Verbose log output.
       --debug               Debug log output.
       --pairwise, -2        Reduce number of combinations using pairwise algorithm.
       --slice <HERE>/<TOTAL>
                             Cut set of combinations into <TOTAL> number of slices and run ony <HERE>th one.
+      --extra-args EXTRA_ARGS
+                            Extra arguments for all actions.
       --alpha ALPHA, -a ALPHA
                             A configuration axis: value1|v1, value2|v2, value3|v3
+      --dump-args DUMP_ARGS 
+                            Extra arguments for dump action.
 
     $ ./build.py -a v[23] dump
     [value2](dump:dump_config) /usr/bin/sh -c echo 'Config(alpha=<MyAlphaAxisValue.Value2: ('value2', 'v2')>)'
     [value2](dump:dump_config) (Hello, World): Config(alpha=<MyAlphaAxisValue.Value2: (value2, v2)>)
     [value2](dump:dump_config) /usr/bin/sh succeeded with exit code 0
     [value3](dump:dump_config) /usr/bin/sh -c echo 'Config(alpha=<MyAlphaAxisValue.Value3: ('value3', 'v3')>)'
     [value3](dump:dump_config) Config(alpha=<MyAlphaAxisValue.Value3: (value3, v3)>)
@@ -184,15 +229,15 @@
 ~~~~~~
 
 Actions are used to capture different workflow steps, such as `compile` and
 `run` for unit tests. A step is simply defined by decorating a function
 with ``@matrix_action``::
 
     @matrix_action
-    def dump(config: Config <, results: List[Result]>):
+    def dump(config: Config<, results: List[Result]><, extra_args: List[str] = None>):
         """Dump configuration to console"""
         pre_process()
         yield dump_config(config, 'Hello', 'World')
         post_process(<results>)
 
 The function itself needs to return a ``Generator`` generating a list of
 Command_'s. The function is called once in preparation for each matrix
@@ -200,14 +245,17 @@
 
 The ``config`` argument gives access to the selected _Config permutation. It
 can be used to generate the commands depending on the actual configuration.
 
 The optional ``results`` argument can be used to gain access to the list of
 Command_ results gathered so far, e.g. for adding post-processing.
 
+The optional ``extra_args`` named-argument can be used to receive a list additional
+command line arguments provided via `--extra-args` or `--<action>-args`.
+
 The function needs to ``yield`` Command_'s, i.e. ``dump_config`` needs to be
 an annotated command function. Pre and post processing code can be added
 around.
 
 Command
 ~~~~~~~
 
@@ -430,15 +478,16 @@
 ~~~~~~~~~~~~
 
 Running one or more configurations from the command line using Matrix Runner is
 trivial. The generated interface looks like this::
 
     $ ./build.py --help
     usage: build.py [-h] [--silent | --verbose | --debug] [--pairwise] [--slice <HERE>/<TOTAL>]
-                    [[--<axis> <AXIS>] ...] action [action ...]
+                    [--extra-args EXTRA_ARGS] [[--<axis> <AXIS>] ...] 
+                    [--<action>-args <ACTION>_ARGS] action [action ...]
 
 The positional argument ``action`` can be one or multiple define Action_'s to
 be executed in the given order, e.g. either ``build`` and ``run`` separately or
 both in a sequence.
 
 The optional arguments are a combination of static ones used to parametrize
 Matrix Runner itself and dynamic ones generated from the defined Axis_:
@@ -451,20 +500,24 @@
   algorithm. This enables combinatorial `all-pairs testing`_ to reduce the
   overall number of configuration in logarithmic manner while retaining a high
   probability of detecting issues.
 - ``--slice <HERE>/<TOTAL>`` cuts the set of combinations into ``TOTAL`` number
   of slices and executes only the ``HERE``'th one. This can be used to run the
   overall set of combinations in parallel. Slicing is applied after
   ``--pairwise`` reduction.
+- ``--extra-args EXTRA_ARGS`` can be used to provide custom arguments passed
+  on to all action functions taking an `extra_args`` named-argument.
 - ``-<a> <AXIS>``, ``--<axis> <AXIS>`` reduce number of combinations to
   selected ``AXIS`` values for ``axis`` Axis values can be given as one of
   their string representations *or* an fnmatch.fnmatch_ pattern matching at
   least one of these. In case of pattern matching *all* matching values are
   selected. This argument can be given multiple time which adds the values in a
   cumulative way.
+- ``--<action>-args <ACTION>_ARGS`` can be used to provide custom arguments passed
+  specifically to the <action> functions taking an `extra_args`` named-argument.
 
 The console output has two parts. While executing the actions the output from
 the associated commands is forwarded like this::
 
     [<AXIS>](<ACTION>) <pre processing log>
     [<AXIS>](<ACTION>:<COMMAND>) <command line>
     [<AXIS>](<ACTION>:<COMMAND>) <stdout/stderr from command>
```

### Comparing `python-matrix-runner-1.1.0/matrix_runner/__init__.py` & `python_matrix_runner-1.2.0/matrix_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `python-matrix-runner-1.1.0/matrix_runner/__main__.py` & `python_matrix_runner-1.2.0/matrix_runner/__main__.py`

 * *Files identical despite different names*

### Comparing `python-matrix-runner-1.1.0/matrix_runner/_helper.py` & `python_matrix_runner-1.2.0/matrix_runner/_helper.py`

 * *Files identical despite different names*

### Comparing `python-matrix-runner-1.1.0/matrix_runner/action.py` & `python_matrix_runner-1.2.0/matrix_runner/action.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,20 +42,24 @@
 
     def __str__(self):
         return self._name
 
     def __repr__(self):
         return self._name
 
-    def __call__(self, config: Config) -> List[Result]:
+    def __call__(self, config: Config, extra_args: List[str] = None) -> List[Result]:
         results = []
         params = [config]
-        if len(signature(self._fn).parameters) >= 2:
+        kvparams = {}
+        fnsign = dict(signature(self._fn).parameters)
+        if fnsign.pop('extra_args', None) and extra_args:
+            kvparams['extra_args'] = extra_args
+        if len(fnsign) >= 2:
             params += [results]
-        cmds = self._fn(*params)
+        cmds = self._fn(*params, **kvparams)
         try:
             for cmd in cmds:
                 results.append(cmd())
         except RuntimeError as e:
             logging.error(e)
             logging.debug(e, exc_info=True)
             results.append(Result())
```

### Comparing `python-matrix-runner-1.1.0/matrix_runner/axis.py` & `python_matrix_runner-1.2.0/matrix_runner/axis.py`

 * *Files identical despite different names*

### Comparing `python-matrix-runner-1.1.0/matrix_runner/command.py` & `python_matrix_runner-1.2.0/matrix_runner/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,15 +271,21 @@
         with lock(cmdline[0]):
             return self._execute_with_retry(cmdline, result)
 
     def _execute(self, cmdline: List[AnyStr], result: Result) -> bool:
         cmdline = self._resolve_cmdline(cmdline)
         logging.warning(" ".join(cmdline), extra=self.extra)
 
-        success = self._execute_with_lock(cmdline, result)
+        success = False
+        try:
+            success = self._execute_with_lock(cmdline, result)
+        except FileNotFoundError as e:
+            result.success = False
+            logging.debug("FileNotFoundError", exc_info=e, extra=self.extra)
+            logging.error("Executing command '%s' failed!", cmdline[0], extra=self.extra)
 
         if self._test_report:
             if isinstance(self._test_report, Callable):
                 self._test_report = self._test_report(result)
             result.test_report = self._test_report.apply(result)
 
         return success
```

### Comparing `python-matrix-runner-1.1.0/matrix_runner/filter.py` & `python_matrix_runner-1.2.0/matrix_runner/filter.py`

 * *Files identical despite different names*

### Comparing `python-matrix-runner-1.1.0/matrix_runner/inspect.py` & `python_matrix_runner-1.2.0/matrix_runner/inspect.py`

 * *Files identical despite different names*

### Comparing `python-matrix-runner-1.1.0/matrix_runner/preferences.py` & `python_matrix_runner-1.2.0/matrix_runner/preferences.py`

 * *Files identical despite different names*

### Comparing `python-matrix-runner-1.1.0/matrix_runner/report.py` & `python_matrix_runner-1.2.0/matrix_runner/report.py`

 * *Files identical despite different names*

### Comparing `python-matrix-runner-1.1.0/matrix_runner/runner.py` & `python_matrix_runner-1.2.0/matrix_runner/runner.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import inspect
 import logging
 import sys
 
 from argparse import ArgumentParser, Action as ArgumentAction, Namespace
 from itertools import product
 from pathlib import Path
+from shlex import split
 from types import GeneratorType
 from typing import Union, Iterable, Mapping, List, MutableMapping
 
 from allpairspy import AllPairs
 from colorlog import ColoredFormatter
 from tabulate import tabulate
 
@@ -158,24 +159,39 @@
 
         if "slice" in self._axes.keys():
             logging.warning("Axis slice shadows built-in --slice flag!")
         else:
             parser.add_argument("--slice", type=Slice, metavar='<HERE>/<TOTAL>',
                                 help="Cut set of combinations into <TOTAL> number of slices "
                                      "and run ony <HERE>th one.")
+            
+        if "extra-args" in self._axes.keys():
+            logging.warning("Axis extra-args shadows built-in --extra-args flag!")
+        else:
+            parser.add_argument("--extra-args", type=split, action=_AppendAxisValuesAction,
+                                help="Extra arguments for all actions.")
 
         for axis in self._axes.values():
             flags = ["--" + axis.name]
             if axis.abbrev:
                 flags += ["-" + axis.abbrev]
             parser.add_argument(*flags, type=axis.converter(), action=_AppendAxisValuesAction,
                                 help=f"{axis.desc}: {', '.join([join(v) for v in axis])}")
         action_help = f"Action(s) to be executed: {', '.join(self._actions.keys())}"
         parser.add_argument("action", choices=list(self._actions.values()) + [[]], nargs='*',
                             metavar="action", type=self._actions.get, help=action_help)
+        
+        for action in self._actions.keys():
+            flag = f"{action}-args"
+            if flag in self._axes.keys():
+                logging.warning("Axis %(flag)s shadows built-in --%(flag)s flag!", {'flag': flag})
+            else:
+                parser.add_argument(f"--{flag}", type=split, action=_AppendAxisValuesAction,
+                                    help=f"Extra arguments for {action} action.")
+
         return parser
 
     def _parse_args(self, argv: List[str] = None) -> Namespace:
         """Parse the arguments using the ArgumentParser.
         The list of values for omitted matrix axes defaults to all possible values.
 
         Args:
@@ -211,27 +227,35 @@
             self._matrix = [Config(**dict(m)) for m in product(*axes) if not Filter.match(Config(**dict(m)))]
         if isinstance(args.slice, Slice):
             if args.slice.denominator > len(self._matrix):
                 logging.warning("Deviding %d combination into %d slices results in empty runs!",
                                 len(self._matrix), args.slice.denominator)
             self._matrix = self._matrix[args.slice.numerator-1::args.slice.denominator]
 
+        extra_args = {'*': []}
+        if "extra-args" not in self._axes.keys():
+            extra_args['*'] = args.extra_args or []
+        for action in args.action:            
+            extra_args[action.name] = []
+            if f"{action}-args" not in self._axes.keys():
+                extra_args[action.name] = vars(args)[f"{action}_args"] or []
+
         for config in self._matrix:
-            self.run_config(args.action, config)
+            self.run_config(args.action, config, extra_args)
         return all(r.success for r in reduce_dict(self._records))
 
-    def run_config(self, actions: List[Action], config: Config):
+    def run_config(self, actions: List[Action], config: Config, extra_args: Mapping[str, List[str]]):
         """Run all actions for the given configuration."""
         for action in actions:
             cfg = "][".join([self._axes[k].tostring(vars(config)[k]) for k in sorted(self._axes.keys())])
             fmt = LogFormatter(f"%({prefs.prefix_colors()['config']})s[{cfg}]"
                                f"%({prefs.prefix_colors()['action']})s({action.name}"
                                f"%(cmd)s)%(reset)s %(log_color)s%(message)s")
             with log_formatter(fmt):
-                results = action(config)
+                results = action(config, extra_args=extra_args['*'] + extra_args[action.name])
                 self.record_results(action, config, results)
 
     def record_results(self, action: Action, config: Config, results: List[Result]):
         """Record execution results."""
         self._records_for(config)[action.name] = results
 
     def records_for(self, config: Config) -> Mapping[str, List[Result]]:
```

### Comparing `python-matrix-runner-1.1.0/python_matrix_runner.egg-info/PKG-INFO` & `python_matrix_runner-1.2.0/python_matrix_runner.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-matrix-runner
-Version: 1.1.0
+Version: 1.2.0
 Summary: Helper to run command with matrix configurations
 Home-page: https://github.com/energy6/python-matrix-runner
 Author: Jonatan Antoni
 Author-email: jonatan@familie-antoni.de
 License: BSD 3-Clause License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -12,19 +12,36 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: allpairspy~=2.5
+Requires-Dist: ansicolors~=1.1
+Requires-Dist: colorama~=0.4
+Requires-Dist: colorlog~=6.7
+Requires-Dist: filelock~=3.12
+Requires-Dist: junitparser~=2.8
+Requires-Dist: lxml~=4.9
+Requires-Dist: parameterized~=0.9
+Requires-Dist: psutil~=5.9
+Requires-Dist: tabulate~=0.9
+Provides-Extra: dev
+Requires-Dist: coverage~=6.5; extra == "dev"
+Requires-Dist: pylint~=2.17; extra == "dev"
+Requires-Dist: restructuredtext_lint~=1.4; extra == "dev"
+Requires-Dist: setuptools~=68.2; extra == "dev"
+Requires-Dist: unittest-xml-reporting~=3.2; extra == "dev"
 
 |build-badge| |test-badge| |cov-badge| |python-badge| |wheel-badge| |pypi-badge| |license-badge|
 
 Matrix Runner for Python
 ========================
 
 Allows easy top level command line interface generation for matrix configurations.
@@ -117,30 +134,34 @@
 
     if __name__ == "__main__":
         main()
 
 Can be executed as::
 
     $ ./build.py --help
-    usage: build.py [-h] [--silent | --verbose | --debug] [--pairwise] [--slice <HERE>/<TOTAL>]
-                    [--alpha ALPHA] action [action ...]
+    usage: build.py [-h] [--silent | --verbose | --debug] [--pairwise] [--slice <HERE>/<TOTAL>] [--extra-args EXTRA_ARGS] 
+                    [--alpha ALPHA] [--dump-args DUMP_ARGS] action [action ...]
 
     positional arguments:
       action                Action(s) to run: dump
 
     optional arguments:
       -h, --help            show this help message and exit
       --silent              Silent mode, only errors are shown.
       --verbose             Verbose log output.
       --debug               Debug log output.
       --pairwise, -2        Reduce number of combinations using pairwise algorithm.
       --slice <HERE>/<TOTAL>
                             Cut set of combinations into <TOTAL> number of slices and run ony <HERE>th one.
+      --extra-args EXTRA_ARGS
+                            Extra arguments for all actions.
       --alpha ALPHA, -a ALPHA
                             A configuration axis: value1|v1, value2|v2, value3|v3
+      --dump-args DUMP_ARGS 
+                            Extra arguments for dump action.
 
     $ ./build.py -a v[23] dump
     [value2](dump:dump_config) /usr/bin/sh -c echo 'Config(alpha=<MyAlphaAxisValue.Value2: ('value2', 'v2')>)'
     [value2](dump:dump_config) (Hello, World): Config(alpha=<MyAlphaAxisValue.Value2: (value2, v2)>)
     [value2](dump:dump_config) /usr/bin/sh succeeded with exit code 0
     [value3](dump:dump_config) /usr/bin/sh -c echo 'Config(alpha=<MyAlphaAxisValue.Value3: ('value3', 'v3')>)'
     [value3](dump:dump_config) Config(alpha=<MyAlphaAxisValue.Value3: (value3, v3)>)
@@ -208,15 +229,15 @@
 ~~~~~~
 
 Actions are used to capture different workflow steps, such as `compile` and
 `run` for unit tests. A step is simply defined by decorating a function
 with ``@matrix_action``::
 
     @matrix_action
-    def dump(config: Config <, results: List[Result]>):
+    def dump(config: Config<, results: List[Result]><, extra_args: List[str] = None>):
         """Dump configuration to console"""
         pre_process()
         yield dump_config(config, 'Hello', 'World')
         post_process(<results>)
 
 The function itself needs to return a ``Generator`` generating a list of
 Command_'s. The function is called once in preparation for each matrix
@@ -224,14 +245,17 @@
 
 The ``config`` argument gives access to the selected _Config permutation. It
 can be used to generate the commands depending on the actual configuration.
 
 The optional ``results`` argument can be used to gain access to the list of
 Command_ results gathered so far, e.g. for adding post-processing.
 
+The optional ``extra_args`` named-argument can be used to receive a list additional
+command line arguments provided via `--extra-args` or `--<action>-args`.
+
 The function needs to ``yield`` Command_'s, i.e. ``dump_config`` needs to be
 an annotated command function. Pre and post processing code can be added
 around.
 
 Command
 ~~~~~~~
 
@@ -454,15 +478,16 @@
 ~~~~~~~~~~~~
 
 Running one or more configurations from the command line using Matrix Runner is
 trivial. The generated interface looks like this::
 
     $ ./build.py --help
     usage: build.py [-h] [--silent | --verbose | --debug] [--pairwise] [--slice <HERE>/<TOTAL>]
-                    [[--<axis> <AXIS>] ...] action [action ...]
+                    [--extra-args EXTRA_ARGS] [[--<axis> <AXIS>] ...] 
+                    [--<action>-args <ACTION>_ARGS] action [action ...]
 
 The positional argument ``action`` can be one or multiple define Action_'s to
 be executed in the given order, e.g. either ``build`` and ``run`` separately or
 both in a sequence.
 
 The optional arguments are a combination of static ones used to parametrize
 Matrix Runner itself and dynamic ones generated from the defined Axis_:
@@ -475,20 +500,24 @@
   algorithm. This enables combinatorial `all-pairs testing`_ to reduce the
   overall number of configuration in logarithmic manner while retaining a high
   probability of detecting issues.
 - ``--slice <HERE>/<TOTAL>`` cuts the set of combinations into ``TOTAL`` number
   of slices and executes only the ``HERE``'th one. This can be used to run the
   overall set of combinations in parallel. Slicing is applied after
   ``--pairwise`` reduction.
+- ``--extra-args EXTRA_ARGS`` can be used to provide custom arguments passed
+  on to all action functions taking an `extra_args`` named-argument.
 - ``-<a> <AXIS>``, ``--<axis> <AXIS>`` reduce number of combinations to
   selected ``AXIS`` values for ``axis`` Axis values can be given as one of
   their string representations *or* an fnmatch.fnmatch_ pattern matching at
   least one of these. In case of pattern matching *all* matching values are
   selected. This argument can be given multiple time which adds the values in a
   cumulative way.
+- ``--<action>-args <ACTION>_ARGS`` can be used to provide custom arguments passed
+  specifically to the <action> functions taking an `extra_args`` named-argument.
 
 The console output has two parts. While executing the actions the output from
 the associated commands is forwarded like this::
 
     [<AXIS>](<ACTION>) <pre processing log>
     [<AXIS>](<ACTION>:<COMMAND>) <command line>
     [<AXIS>](<ACTION>:<COMMAND>) <stdout/stderr from command>
```

### Comparing `python-matrix-runner-1.1.0/setup.py` & `python_matrix_runner-1.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,29 +28,29 @@
     name='python-matrix-runner',
     version=version_from_git_tag(),
     packages=['matrix_runner'],
     install_requires=[
         'allpairspy~=2.5',
         'ansicolors~=1.1',
         'colorama~=0.4',
-        'colorlog~=6.6',
-        'filelock~=3.4',
-        'junitparser~=2.2',
-        'lxml~=4.6',
-        'parameterized~=0.8',
-        'psutil~=5.8',
-        'tabulate~=0.8'
+        'colorlog~=6.7',
+        'filelock~=3.12',
+        'junitparser~=2.8',
+        'lxml~=4.9',
+        'parameterized~=0.9',
+        'psutil~=5.9',
+        'tabulate~=0.9'
     ],
     extras_require={
         'dev': [
-            'coverage~=6.2',
-            'pylint~=2.11',
-            'restructuredtext_lint~=1.3',
-            'setuptools~=59.4',
-            'unittest-xml-reporting~=3.0'
+            'coverage~=6.5',
+            'pylint~=2.17',
+            'restructuredtext_lint~=1.4',
+            'setuptools~=68.2',
+            'unittest-xml-reporting~=3.2'
         ]
     },
     entry_points={
         'console_scripts': ['matrix-runner-inspect=matrix_runner.inspect:InspectRunner'],
     },
     python_requires='>=3.8',
     url='https://github.com/energy6/python-matrix-runner',
@@ -67,10 +67,12 @@
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Software Development :: Build Tools"
     ]
 )
```

