# Comparing `tmp/getodo-1.0.2.tar.gz` & `tmp/getodo-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getodo-1.0.2.tar", max compression
+gzip compressed data, was "getodo-2.0.0.tar", max compression
```

## Comparing `getodo-1.0.2.tar` & `getodo-2.0.0.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     1070 2024-03-22 09:03:41.095653 getodo-1.0.2/LICENSE
--rw-r--r--   0        0        0     4107 2024-03-22 09:03:41.095653 getodo-1.0.2/README.md
--rw-r--r--   0        0        0        0 2024-03-22 09:03:41.095653 getodo-1.0.2/getodo/__init__.py
--rw-r--r--   0        0        0       36 2024-03-22 09:03:41.095653 getodo-1.0.2/getodo/__main__.py
--rw-r--r--   0        0        0     5949 2024-03-22 09:03:41.095653 getodo-1.0.2/getodo/cli.py
--rw-r--r--   0        0        0     7726 2024-03-22 09:03:41.095653 getodo-1.0.2/getodo/todoparser.py
--rw-r--r--   0        0        0      499 2024-03-22 09:03:41.095653 getodo-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     4734 1970-01-01 00:00:00.000000 getodo-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-30 17:03:44.134689 getodo-2.0.0/LICENSE
+-rw-r--r--   0        0        0     2636 2024-04-30 17:03:44.134689 getodo-2.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 17:03:44.134689 getodo-2.0.0/getodo/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 17:03:44.134689 getodo-2.0.0/getodo/__main__.py
+-rw-r--r--   0        0        0     6087 2024-04-30 17:03:44.134689 getodo-2.0.0/getodo/getodo.py
+-rw-r--r--   0        0        0      738 2024-04-30 17:03:44.134689 getodo-2.0.0/getodo/getodo_cfg.json
+-rw-r--r--   0        0        0     1768 2024-04-30 17:03:44.134689 getodo-2.0.0/getodo/getodo_cli.py
+-rw-r--r--   0        0        0     2098 2024-04-30 17:03:44.134689 getodo-2.0.0/getodo/utils.py
+-rw-r--r--   0        0        0      410 2024-04-30 17:03:44.134689 getodo-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3180 1970-01-01 00:00:00.000000 getodo-2.0.0/PKG-INFO
```

### Comparing `getodo-1.0.2/LICENSE` & `getodo-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `getodo-1.0.2/PKG-INFO` & `getodo-2.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: getodo
-Version: 1.0.2
+Version: 2.0.0
 Summary: A python program to collect all your TODO(s)
 License: MIT
-Author: vyshnav-vinod
+Author: Vyshnav Vinod
 Author-email: vyshnav.vinod003@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
-Requires-Dist: questionary (>=2.0.1,<3.0.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/markdown
 
 # GETODO
 > A python program to collect all your TODO(s)
 
 `getodo` is a python program that collects all your TODO(s) from a folder/file and list them for you as a file or in the terminal screen. `getodo` makes it easy to keep track of your TODO(s)
 
@@ -45,67 +43,46 @@
 
 - It is recommended to create a [virtual environment](https://docs.python.org/3/tutorial/venv.html) before installing the packages.
 ```
 python3 -m venv venv
 ```
 
 - Install the required packages from `requirements.txt`
->[!NOTE]
->Use can you either `poetry` or `pip` to install the required packages.
 
 ``` 
 pip install -r requirements.txt
 ```
 
 - Run `getodo` using python
-``` python cli.py input_path ```
+``` python getodo_cli.py input_path ```
 
 ## Usage
 
 If you have downloaded via `pip`
 ```
 getodo input_path [options]
 ```
 
 else
 
 ```
-python cli.py input_path [options]
+python getodo_cli.py input_path [options]
 ```
 
 Replace `input_path` with the path to the folder/file you want to parse. You can just type `.` to parse the current directory for TODO(s)
 
 ### Options
 
 `-h, --help` : Display the help command
 
-`-c, --config` : Create a custom config file for getodo. [More Info](https://github.com/vyshnav-vinod/getodo/blob/main/README.md#config)
-
-`--override_config` : Run getodo with the default configs 
-
 `-o, --output` : Write to the file provided here. If no file is specified, the program will write to `todo.txt`
 
 `-t, --term` : Display the TODO's in the terminal with colors
 
-`--add_filetypes` : If you have a filetype that is not currently supported by `getodo` you can use this to specify the filetype and the comment syntax and `getodo` will parse the TODO's
-
 `-i, --ignore` : Ignore parsing the directories/files provided as arguments to this option
 
-
-### Config
-
-when running `getodo`, it will first look for a `getodo_config.toml` file in the root of the directory meant to be parsed. If found, getodo will use the options inside the `getodo_config.toml` file. It includes the path to the output file , the folders and files meant to be ignored by `getodo` and also if any custom filetype is to be parsed as well.
-
-```bash
-python3 getodo.py . -c
-```
-This will start a interactive interface to create the `getodo_config.toml` file and store it in the , in this case, the current directory. Then next time whenever you run `getodo` in that directory, you need not specify any options as `.getodo_config.toml` file will already have them. You can create different config files for different projects, making it easy to just type `getodo.py .` and get your TODO(s).
-
-If there comes a circumstance where you need to ignore some other directories/files or add new filetypes you can use the `--override_config` flag along with the other flags. This will not load the configs from `.getodo_config.toml` and only use the arguments passed. 
-
-
 ## Contributing
 
 All contributions are welcome. You can submit a issue/bug or request for a feature or ask for help in the [issues](https://github.com/vyshnav-vinod/getodo/issues) tab.
 
-If you like to add a new feature or fix a bug, please checkout [CONTRIBUTING]() guidelines.
+If you like to add a new feature or fix a bug, please checkout [CONTRIBUTING](https://github.com/vyshnav-vinod/getodo/blob/main/CONTRIBUTING.md) guidelines.
```

