# Comparing `tmp/fancylog-0.3.0rc0.tar.gz` & `tmp/fancylog-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fancylog-0.3.0rc0.tar", last modified: Wed Jan  4 13:47:34 2023, max compression
+gzip compressed data, was "fancylog-0.4.1.tar", last modified: Tue Apr 30 16:34:57 2024, max compression
```

## Comparing `fancylog-0.3.0rc0.tar` & `fancylog-0.4.1.tar`

### file list

```diff
@@ -1,24 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 13:47:34.983090 fancylog-0.3.0rc0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-01-04 13:47:17.000000 fancylog-0.3.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-01-04 13:47:34.983090 fancylog-0.3.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-01-04 13:47:17.000000 fancylog-0.3.0rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 13:47:34.983090 fancylog-0.3.0rc0/fancylog/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-01-04 13:47:17.000000 fancylog-0.3.0rc0/fancylog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10446 2023-01-04 13:47:17.000000 fancylog-0.3.0rc0/fancylog/fancylog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 13:47:34.983090 fancylog-0.3.0rc0/fancylog/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 13:47:17.000000 fancylog-0.3.0rc0/fancylog/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-01-04 13:47:17.000000 fancylog-0.3.0rc0/fancylog/tools/git.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 13:47:34.983090 fancylog-0.3.0rc0/fancylog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-01-04 13:47:34.000000 fancylog-0.3.0rc0/fancylog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-01-04 13:47:34.000000 fancylog-0.3.0rc0/fancylog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-04 13:47:34.000000 fancylog-0.3.0rc0/fancylog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-01-04 13:47:34.000000 fancylog-0.3.0rc0/fancylog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-04 13:47:34.000000 fancylog-0.3.0rc0/fancylog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-01-04 13:47:17.000000 fancylog-0.3.0rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-01-04 13:47:34.983090 fancylog-0.3.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-01-04 13:47:17.000000 fancylog-0.3.0rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 13:47:34.983090 fancylog-0.3.0rc0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 13:47:17.000000 fancylog-0.3.0rc0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 13:47:34.983090 fancylog-0.3.0rc0/tests/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 13:47:17.000000 fancylog-0.3.0rc0/tests/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-04 13:47:17.000000 fancylog-0.3.0rc0/tests/tests/test_DUMMY.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:34:57.228139 fancylog-0.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:34:57.224138 fancylog-0.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:34:57.224138 fancylog-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-30 16:34:51.000000 fancylog-0.4.1/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-30 16:34:51.000000 fancylog-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-30 16:34:51.000000 fancylog-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-30 16:34:51.000000 fancylog-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-30 16:34:51.000000 fancylog-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-30 16:34:57.228139 fancylog-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-30 16:34:51.000000 fancylog-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:34:57.228139 fancylog-0.4.1/fancylog/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-30 16:34:51.000000 fancylog-0.4.1/fancylog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-04-30 16:34:51.000000 fancylog-0.4.1/fancylog/fancylog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:34:57.228139 fancylog-0.4.1/fancylog/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:34:51.000000 fancylog-0.4.1/fancylog/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-30 16:34:51.000000 fancylog-0.4.1/fancylog/tools/git.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:34:57.228139 fancylog-0.4.1/fancylog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-30 16:34:57.000000 fancylog-0.4.1/fancylog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-30 16:34:57.000000 fancylog-0.4.1/fancylog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 16:34:57.000000 fancylog-0.4.1/fancylog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-30 16:34:57.000000 fancylog-0.4.1/fancylog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 16:34:57.000000 fancylog-0.4.1/fancylog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-30 16:34:51.000000 fancylog-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 16:34:57.228139 fancylog-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:34:57.228139 fancylog-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:34:51.000000 fancylog-0.4.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:34:57.228139 fancylog-0.4.1/tests/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:34:51.000000 fancylog-0.4.1/tests/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-30 16:34:51.000000 fancylog-0.4.1/tests/tests/test_general.py
```

### Comparing `fancylog-0.3.0rc0/README.md` & `fancylog-0.4.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 [![Python Version](https://img.shields.io/pypi/pyversions/cellfinder.svg)](https://pypi.org/project/cellfinder)
 [![PyPI](https://img.shields.io/pypi/v/fancylog.svg)](https://pypi.org/project/fancylog)
 [![Downloads](https://pepy.tech/badge/fancylog)](https://pepy.tech/project/fancylog)
 [![Wheel](https://img.shields.io/pypi/wheel/fancylog.svg)](https://pypi.org/project/fancylog)
-[![Development Status](https://img.shields.io/pypi/status/fancylog.svg)](https://github.com/adamltyson/fancylog)
+[![Development Status](https://img.shields.io/pypi/status/fancylog.svg)](https://github.com/neuroinformatics-unit/fancylog)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
-[![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](https://github.com/adamltyson/fancylog)
+[![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](https://github.com/neuroinformatics-unit/fancylog)
 
 # fancylog
 Fancier logging with python.
 
 Uses the standard python logging library, but (optionally) in addition:
 * Logs code when using the multiprocessing module using
 [multiprocessing-logging](https://github.com/jruere/multiprocessing-logging)
-* Uses [gitpython](https://github.com/gitpython-developers/GitPython)
+* Uses [GitPython](https://github.com/gitpython-developers/GitPython)
 to log information about the git environment.
 * Logs the command-line arguments used to run the software
 * Logs object attributes
 
 
 #### To install
 ```bash
 pip install fancylog
 ```
 
+N.B. For the git logging to work, you need to have [git](https://git-scm.com/) and the
+[GitPython](https://github.com/gitpython-developers/GitPython) package
+installed. The latter can be installed along with `fancylog` using:
+
+```bash
+pip install fancylog[git]
+```
+
 #### To run example
 ```bash
-git clone https://github.com/adamltyson/fancylog
+git clone https://github.com/neuroinformatics-unit/fancylog
 pip install -e .
 python fancylog/example.py /path/to/output/log/dir
 ```
 
 If you run the example, you should get a log file that resembles
 [this](fancylog_2019-10-18_15-30-12.log)
```

### Comparing `fancylog-0.3.0rc0/fancylog/fancylog.py` & `fancylog-0.4.1/fancylog/fancylog.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-"""
-fancylog
+"""fancylog
 ===============
 
 Wrapper around the standard logging module, with additional information.
 
 """
 
+import contextlib
 import logging
 import os
 import sys
 from datetime import datetime
 from importlib.util import find_spec
 
 from rich.logging import RichHandler
@@ -18,32 +18,32 @@
     GitEnvironmentError,
     GitPythonError,
     get_git_info,
 )
 
 
 def start_logging(
-    output_dir=None,
-    package=None,
+    output_dir,
+    package,
     variables=None,
     verbose=True,
     file_log_level="DEBUG",
     filename=None,
     log_header="LOG",
     multiprocessing_aware=False,
     write_header=True,
     write_git=True,
     write_cli_args=True,
     write_variables=True,
     log_to_file=True,
     log_to_console=True,
     timestamp=True,
+    logger_name=None,
 ):
-    """
-    Prepares the log file, and then begins logging.
+    """Prepares the log file, and then begins logging.
 
     :param output_dir: Directory to save the log file
     :param package: What python package are we logging?
     :param variables: List of objects whose attributes we want to log at the
     beginning of the log file
     :param verbose: If true, all info (i.e. 'DEBUG') is printed to
     console. Else, only 'INFO' and above. Default: True
@@ -56,24 +56,22 @@
     :param write_git: Write information about the git repository.
     Default: True
     :param write_cli_args: Log the command-line arguments. Default: True
     :param write_variables: Write the attributes of selected objects.
     Default: True
     :param log_to_file: If True, write a log file, otherwise just print to
     terminal.
-    :param timestamp: If True, add a timestamp to the filename
     :param log_to_console: Print logs to the console or not: Default: True
+    :param timestamp: If True, add a timestamp to the filename
+    :param logger_name: If None, logger uses default logger. Otherwise,
+        logger name is set to `logger_name`.
     :return: Path to the logging file#
     """
-
     output_dir = str(output_dir)
-    if verbose:
-        print_log_level = "DEBUG"
-    else:
-        print_log_level = "INFO"
+    print_log_level = "DEBUG" if verbose else "INFO"
 
     if log_to_file:
         if filename is None:
             filename = package.__name__
         if timestamp:
             filename = datetime.now().strftime(filename + "_%Y-%m-%d_%H-%M-%S")
         logging_file = filename + ".log"
@@ -99,14 +97,15 @@
 
     setup_logging(
         logging_file,
         print_level=print_log_level,
         file_level=file_log_level,
         multiprocessing_aware=multiprocessing_aware,
         log_to_console=log_to_console,
+        logger_name=logger_name,
     )
     return logging_file
 
 
 class LoggingHeader:
     def __init__(
         self,
@@ -116,49 +115,43 @@
         output_dir,
         write_header=True,
         write_git=True,
         write_cli_args=True,
         write_variables=True,
         log_header=None,
     ):
-
-        self.file = open(file, "w", encoding="utf-8")
         self.program = program
-        if write_header:
-            self.write_log_header(output_dir, log_header)
-        if write_git:
-            self.write_git_info(self.program.__name__)
-        if write_cli_args:
-            self.write_command_line_arguments()
-        if write_variables and variable_objects:
-            self.write_variables(variable_objects)
 
-        self.file.close()
+        with open(file, "w", encoding="utf-8") as self.file:
+            if write_header:
+                self.write_log_header(output_dir, log_header)
+            if write_git:
+                self.write_git_info(self.program.__name__)
+            if write_cli_args:
+                self.write_command_line_arguments()
+            if write_variables and variable_objects:
+                self.write_variables(variable_objects)
 
     def write_git_info(self, program_name, header="GIT INFO"):
         self.write_separated_section_header(header)
         try:
             program_path = find_spec(program_name).submodule_search_locations[
                 0
             ]
             program_path = os.path.split(program_path)[0]
             git_info = get_git_info(program_path)
 
-            self.file.write("Commit hash: {} \n".format(git_info.head.hash))
+            self.file.write(f"Commit hash: {git_info.head.hash} \n")
+            self.file.write(f"Commit message: {git_info.head.message} \n")
+            self.file.write(f"Commit date & time: {git_info.head.datetime} \n")
             self.file.write(
-                "Commit message: {} \n".format(git_info.head.message)
+                f"Commit author: {git_info.head.committer_name} \n"
             )
             self.file.write(
-                "Commit date & time: {} \n".format(git_info.head.datetime)
-            )
-            self.file.write(
-                "Commit author: {} \n".format(git_info.head.committer_name)
-            )
-            self.file.write(
-                "Commit author email: {}".format(git_info.head.committer_email)
+                f"Commit author email: {git_info.head.committer_email}"
             )
 
         except GitPythonError:
             self.file.write(
                 "Gitpython is not installed. "
                 "Cannot check if software is in a git repository"
             )
@@ -195,24 +188,20 @@
                     self.file.write(f"{attr}: {value}\n")
 
     def write_log_header(self, output_dir, log_header):
         if log_header is None:
             log_header = "LOG"
         self.write_separated_section_header(log_header, top_sep=False)
         self.file.write(
-            "Analysis carried out: "
-            + datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
-            + "\n"
+            "Ran at : " + datetime.now().strftime("%Y-%m-%d_%H-%M-%S") + "\n"
         )
         self.file.write("Output directory: " + output_dir + "\n")
         self.file.write("Current directory: " + os.getcwd() + "\n")
-        try:
+        with contextlib.suppress(AttributeError):
             self.file.write(f"Version: {self.program.__version__}")
-        except AttributeError:
-            pass
 
     def write_separated_section_header(
         self,
         section_header,
         top_sep=True,
         bottom_sep=True,
         top_separator="\n\n",
@@ -231,30 +220,36 @@
         self, section_header, lateral_separator="**************"
     ):
         self.file.write(
             f"{lateral_separator}  {section_header}  {lateral_separator}"
         )
 
 
-def initalise_logger(
+def initialise_logger(
     filename,
     print_level="INFO",
     file_level="DEBUG",
     log_to_console=True,
+    logger_name=None,
 ):
-    """
-    Sets up (possibly multiprocessing aware) logging.
+    """Sets up (possibly multiprocessing aware) logging.
     :param filename: Where to save the logs to
     :param print_level: What level of logging to print to console.
     Default: 'INFO'
     :param file_level: What level of logging to print to file.
     Default: 'DEBUG'
     :param log_to_console: Print logs to the console or not
+    :param logger_name: If None, logger uses default logger. Otherwise,
+    logger name is set to `logger_name`.
     """
-    logger = logging.getLogger()
+    if logger_name:
+        logger = logging.getLogger(logger_name)
+    else:
+        logger = logging.getLogger()
+
     logger.setLevel(getattr(logging, file_level))
 
     formatter = logging.Formatter(
         "%(asctime)s - %(levelname)s"
         " - %(processName)s %(filename)s:%(lineno)s"
         " - %(message)s"
     )
@@ -277,33 +272,34 @@
 
 def setup_logging(
     filename,
     print_level="INFO",
     file_level="DEBUG",
     multiprocessing_aware=True,
     log_to_console=True,
+    logger_name=None,
 ):
-    """
-    Sets up (possibly multiprocessing aware) logging.
+    """Sets up (possibly multiprocessing aware) logging.
     :param filename: Where to save the logs to
     :param print_level: What level of logging to print to console.
     Default: 'INFO'
     :param file_level: What level of logging to print to file.
     Default: 'DEBUG'
     :param multiprocessing_aware: Default: True
     :param log_to_console: Print logs to the console or no.
     Default: True
-
+    :param logger_name: If None, logger uses default logger. Otherwise,
+        logger name is set to `logger_name`.
     """
-
-    initalise_logger(
+    initialise_logger(
         filename,
         print_level=print_level,
         file_level=file_level,
         log_to_console=log_to_console,
+        logger_name=logger_name,
     )
     if multiprocessing_aware:
         try:
             import multiprocessing_logging
 
             multiprocessing_logging.install_mp_handler()
             logging.info("Starting logging")
@@ -319,13 +315,12 @@
             )
     else:
         logging.info("Starting logging")
         logging.info("Not logging multiple processes")
 
 
 def disable_logging():
-    """
-    Prevents any more logging. Saves remembering that logging.disable() with
+    """Prevents any more logging. Saves remembering that logging.disable() with
     no argument doesn't work.
     :return:
     """
     logging.disable(2**63 - 1)
```

### Comparing `fancylog-0.3.0rc0/fancylog/tools/git.py` & `fancylog-0.4.1/fancylog/tools/git.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,75 +1,65 @@
-"""
-git
+"""git
 ===============
 
 Wrappers around gitpython to return information about the git repository
 for debugging
 
 """
 
 
 class GitPythonError(Exception):
-    """
-    Exception if gitpython cannot be found (Typical in production
+    """Exception if gitpython cannot be found (Typical in production
     environments).
     """
 
     pass
 
 
 class GitEnvironmentError(Exception):
-    """
-    Exception if gitpython  fails (Typical in production environments).
-    """
+    """Exception if gitpython  fails (Typical in production environments)."""
 
     pass
 
 
 class GitHead:
-    """
-    Class to parse a repo.head.commit object from gitpython, and return
+    """Class to parse a repo.head.commit object from gitpython, and return
     more informative properties
     """
 
     def __init__(self, head_commit):
         self.hash = head_commit.hexsha
         self.committer_name = head_commit.committer.name
         self.committer_email = head_commit.committer.email
         self.message = head_commit.summary
         self.datetime = head_commit.authored_datetime.strftime(
             "Date: %Y-%m-%d, Time: %H-%M-%S"
         )
 
 
 class GitInfo:
-    """
-    Class to parse a repo object from gitpython, and return more informative
+    """Class to parse a repo object from gitpython, and return more informative
     properties
     """
 
     def __init__(self, repo):
         self.head = GitHead(repo.head.commit)
 
 
 def get_git_info(repo_path):
-    """
-    Returns a class with useful information about the git repository.
+    """Returns a class with useful information about the git repository.
     (if there is one). Will only work with "dev" installs (otherwise
     gitpython is not installed)
     :return:
     """
-
     try:
         import git
 
-    except ImportError:
-        raise GitPythonError
-        return None
+    except ImportError as exc:
+        raise GitPythonError from exc
 
     try:
         repo = git.Repo(repo_path)
         return GitInfo(repo)
 
-    except git.InvalidGitRepositoryError:
-        raise GitEnvironmentError
-        return None
+    except git.InvalidGitRepositoryError as exc:
+        raise GitEnvironmentError from exc
```

