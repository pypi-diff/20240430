# Comparing `tmp/pyprojectlib-0.0.2.tar.gz` & `tmp/pyprojectlib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprojectlib-0.0.2.tar", last modified: Tue Nov 14 00:50:35 2023, max compression
+gzip compressed data, was "pyprojectlib-0.0.3.tar", last modified: Tue Apr 30 16:02:55 2024, max compression
```

## Comparing `pyprojectlib-0.0.2.tar` & `pyprojectlib-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-11-14 00:50:35.595315 pyprojectlib-0.0.2/
--rw-rw-rw-   0        0        0    35821 2023-08-08 21:22:00.000000 pyprojectlib-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     7233 2023-11-14 00:50:35.594306 pyprojectlib-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     6435 2023-11-13 12:35:15.000000 pyprojectlib-0.0.2/README.md
--rw-rw-rw-   0        0        0      954 2023-11-14 00:50:22.000000 pyprojectlib-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-11-14 00:50:35.595315 pyprojectlib-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-11-14 00:50:35.559226 pyprojectlib-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-11-14 00:50:35.569008 pyprojectlib-0.0.2/src/pyprojectlib/
--rw-rw-rw-   0        0        0     6366 2023-11-14 00:15:32.000000 pyprojectlib-0.0.2/src/pyprojectlib/__init__.py
--rw-rw-rw-   0        0        0     5276 2023-11-13 04:33:11.000000 pyprojectlib-0.0.2/src/pyprojectlib/cli.py
--rw-rw-rw-   0        0        0     1451 2023-11-13 22:38:00.000000 pyprojectlib-0.0.2/src/pyprojectlib/constants.py
--rw-rw-rw-   0        0        0     4058 2023-11-14 00:07:35.000000 pyprojectlib-0.0.2/src/pyprojectlib/helper.py
--rw-rw-rw-   0        0        0        0 2023-11-11 03:12:10.000000 pyprojectlib-0.0.2/src/pyprojectlib/py.typed
--rw-rw-rw-   0        0        0     8122 2023-11-14 00:49:50.000000 pyprojectlib-0.0.2/src/pyprojectlib/pypackage.py
--rw-rw-rw-   0        0        0     4321 2023-11-13 11:45:23.000000 pyprojectlib-0.0.2/src/pyprojectlib/pyproject.py
--rw-rw-rw-   0        0        0     7978 2023-11-13 11:48:42.000000 pyprojectlib-0.0.2/src/pyprojectlib/pyrepo.py
--rw-rw-rw-   0        0        0     1617 2023-11-13 05:08:24.000000 pyprojectlib-0.0.2/src/pyprojectlib/pyuser.py
-drwxrwxrwx   0        0        0        0 2023-11-14 00:50:35.593304 pyprojectlib-0.0.2/src/pyprojectlib.egg-info/
--rw-rw-rw-   0        0        0     7233 2023-11-14 00:50:35.000000 pyprojectlib-0.0.2/src/pyprojectlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2023-11-14 00:50:35.000000 pyprojectlib-0.0.2/src/pyprojectlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-14 00:50:35.000000 pyprojectlib-0.0.2/src/pyprojectlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-11-14 00:50:35.000000 pyprojectlib-0.0.2/src/pyprojectlib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      123 2023-11-14 00:50:35.000000 pyprojectlib-0.0.2/src/pyprojectlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-11-14 00:50:35.000000 pyprojectlib-0.0.2/src/pyprojectlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 16:02:55.624151 pyprojectlib-0.0.3/
+-rw-rw-rw-   0        0        0    35821 2023-08-08 21:22:00.000000 pyprojectlib-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     7232 2024-04-30 16:02:55.622133 pyprojectlib-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6461 2024-04-30 15:38:54.000000 pyprojectlib-0.0.3/README.md
+-rw-rw-rw-   0        0        0      925 2024-04-30 16:02:17.000000 pyprojectlib-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-30 16:02:55.624151 pyprojectlib-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 16:02:55.523317 pyprojectlib-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-30 16:02:55.560283 pyprojectlib-0.0.3/src/pyprojectlib/
+-rw-rw-rw-   0        0        0     6366 2023-11-14 00:15:32.000000 pyprojectlib-0.0.3/src/pyprojectlib/__init__.py
+-rw-rw-rw-   0        0        0     5382 2024-04-30 15:41:06.000000 pyprojectlib-0.0.3/src/pyprojectlib/cli.py
+-rw-rw-rw-   0        0        0     1475 2024-04-30 15:25:10.000000 pyprojectlib-0.0.3/src/pyprojectlib/constants.py
+-rw-rw-rw-   0        0        0     4058 2023-11-14 00:07:35.000000 pyprojectlib-0.0.3/src/pyprojectlib/helper.py
+-rw-rw-rw-   0        0        0        0 2023-11-11 03:12:10.000000 pyprojectlib-0.0.3/src/pyprojectlib/py.typed
+-rw-rw-rw-   0        0        0     9119 2024-04-30 15:57:21.000000 pyprojectlib-0.0.3/src/pyprojectlib/pypackage.py
+-rw-rw-rw-   0        0        0     4321 2023-11-13 11:45:23.000000 pyprojectlib-0.0.3/src/pyprojectlib/pyproject.py
+-rw-rw-rw-   0        0        0     8083 2024-04-30 15:57:42.000000 pyprojectlib-0.0.3/src/pyprojectlib/pyrepo.py
+-rw-rw-rw-   0        0        0     1617 2023-11-13 05:08:24.000000 pyprojectlib-0.0.3/src/pyprojectlib/pyuser.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:02:55.618804 pyprojectlib-0.0.3/src/pyprojectlib.egg-info/
+-rw-rw-rw-   0        0        0     7232 2024-04-30 16:02:55.000000 pyprojectlib-0.0.3/src/pyprojectlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2024-04-30 16:02:55.000000 pyprojectlib-0.0.3/src/pyprojectlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 16:02:55.000000 pyprojectlib-0.0.3/src/pyprojectlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-30 16:02:55.000000 pyprojectlib-0.0.3/src/pyprojectlib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      123 2024-04-30 16:02:55.000000 pyprojectlib-0.0.3/src/pyprojectlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-30 16:02:55.000000 pyprojectlib-0.0.3/src/pyprojectlib.egg-info/top_level.txt
```

### Comparing `pyprojectlib-0.0.2/LICENSE.txt` & `pyprojectlib-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyprojectlib-0.0.2/PKG-INFO` & `pyprojectlib-0.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: pyprojectlib
-Version: 0.0.2
-Author-email: Jason Krist <jkrist2696@gmail.com>
-License: GPL-3.0-only
-Project-URL: Homepage, https://github.com/jkrist2696/pyprojectlib
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: Unix
-Requires-Python: >=3.12.0
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: cleandoc>=0.0.13
-Requires-Dist: GitPython>=3.1.40
-Requires-Dist: pipreqs>=0.4.13
-Requires-Dist: pytest>=7.4.3
-Requires-Dist: build
-Requires-Dist: twine
-Requires-Dist: tomli
-Requires-Dist: tomli-w
-Requires-Dist: types-requests
-Requires-Dist: types-setuptools
-
 # PyProjectLib
 
 
 ## Description
 
 Python package for managing local python projects and repositories
 
@@ -40,90 +16,93 @@
 ### Command Line Usage: "ppl"
 
 usage: ppl [-h] {new,push,pack} ...
 
 Package for managing local python projects and repositories
 
 positional arguments:
-*  {new,push,pack}  Command to execute (options below)
-    *    new            Create a new repo, project, or user of a repo
-    *    push           Save your python project in a local repository
-    *    pack           Package python project into a distributable module
+
+* {new,push,pack}  Command to execute (options below)
+    * new            Create a new repo, project, or user of a repo
+    * push           Save your python project in a local repository
+    * pack           Package python project into a distributable module
 
 ### Command Line Usage: "ppl">"new"
 
 usage: ppl new [-h] {repo,proj,user} ...
 
 positional arguments:
-*    {repo,proj,user}  Create something (options below)
-    *     repo            Create a new empty repository
-    *     proj            Create a new empty project
-    *     user            Add a new user to a local repository
+
+* {repo,proj,user}  Create something (options below)
+    * repo            Create a new empty repository
+    * proj            Create a new empty project
+    * user            Add a new user to a local repository
 
 ### Command Line Usage: "ppl">"new">"repo"
 
-usage: ppl new repo [-h] [-name NAME] [-email EMAIL] [-gituser GITUSER] repopath
+usage: ppl new repo repopath [-h] [-name NAME] [-email EMAIL] [-gituser GITUSER]
 
 positional arguments:
-*    repopath    Path to local python repository. Directory name = repo name.
+* repopath    Path to local python repository. Directory name = repo name.
 
 options:
-*    -name NAME, -n NAME             Your full name
-*    -email EMAIL, -e EMAIL          Your email address
-*    -gituser GITUSER, -g GITUSER    Your username on Github
+* -name NAME, -n NAME             Your full name
+* -email EMAIL, -e EMAIL          Your email address
+* -gituser GITUSER, -g GITUSER    Your username on Github
 
 ### Command Line Usage: "ppl">"new">"project"
 
-usage: ppl new proj [-h] projpath
+usage: ppl new proj projpath [-h]
 
 positional arguments:
-*    projpath    Path to python project. Directory name = project name.
+* projpath    Path to python project. Directory name = project name.
 
 ### Command Line Usage: "ppl">"new">"user"
 
-usage: ppl new user [-h] [-name NAME] [-email EMAIL] [-gituser GITUSER] repopath
+usage: ppl new user repopath [-h] [-name NAME] [-email EMAIL] [-gituser GITUSER]
 
 positional arguments:
-*    repopath              Path to local python repository. Directory name = repo name.
+* repopath              Path to local python repository. Directory name = repo name.
 
 options:
-*    -name NAME, -n NAME             Your full name
-*    -email EMAIL, -e EMAIL          Your email address
-*    -gituser GITUSER, -g GITUSER    Your username on Github
+* -name NAME, -n NAME             Your full name
+* -email EMAIL, -e EMAIL          Your email address
+* -gituser GITUSER, -g GITUSER    Your username on Github
 
 ### Command Line Usage: "ppl">"push"
-usage: ppl push [-h] [-relpath RELPATH] [-noclean] [-nodoc] [-notest] [-version VERSION] [-name NAME] [-email EMAIL] [-gituser GITUSER] repopath projpath
+usage: ppl push repopath projpath [-h] [-relpath RELPATH] [-noclean] [-nodoc] [-notest] [-version VERSION] [-name NAME] [-email EMAIL] [-gituser GITUSER]
 
 positional arguments:
-*    repopath              Path to local python repository. Directory name = repo name.
-*    projpath              Path to python project. Directory name = project name.
+* repopath              Path to local python repository. Directory name = repo name.
+* projpath              Path to python project. Directory name = project name.
 
 options:
-*    -relpath RELPATH, -r RELPATH    Relative path from repository basedir to add project
-*    -noclean, -nc                   Flag to prevent checking py files for cleanliness
-*    -nodoc, -nd                     Flag to prevent html documentation creation
-*    -notest, -nt                    Flag to prevent pytest from running
-*    -version VERSION, -v VERSION    Version number of python project (X.Y.Z)
-*    -name NAME, -n NAME             Your full name
-*    -email EMAIL, -e EMAIL          Your email address
-*    -gituser GITUSER, -g GITUSER    Your username on Github
+* -relpath RELPATH, -r RELPATH    Relative path from repository basedir to add project
+* -noclean, -nc                   Flag to prevent checking py files for cleanliness
+* -nodoc, -nd                     Flag to prevent html documentation creation
+* -notest, -nt                    Flag to prevent pytest from running
+* -version VERSION, -v VERSION    Version number of python project (X.Y.Z)
+* -name NAME, -n NAME             Your full name
+* -email EMAIL, -e EMAIL          Your email address
+* -gituser GITUSER, -g GITUSER    Your username on Github
 
 ### Command Line Usage: "ppl">"pack"
-usage: ppl pack [-h] [-upload] [-install] [-version VERSION] [-name NAME] [-email EMAIL] [-gituser GITUSER] projpath
+usage: ppl pack projpath [-h] [-upload] [-install] [-version VERSION] [-name NAME] [-email EMAIL] [-gituser GITUSER] [-pyversion PYTHONVERSION]
 
 positional arguments:
-*    projpath              Path to python project. Directory name = project name.
+* projpath              Path to python project. Directory name = project name.
 
 options:
-*    -upload, -u                     Flag to upload python module to PYPI after packaging it
-*    -install, -i                    Flag to install python module after packaging it
-*    -version VERSION, -v VERSION    Version number of python project (X.Y.Z)
-*    -name NAME, -n NAME             Your full name
-*    -email EMAIL, -e EMAIL          Your email address
-*    -gituser GITUSER, -g GITUSER    Your username on Github
+* -upload, -u                         Flag to upload python module to PYPI after packaging it
+* -install, -i                        Flag to install python module after packaging it
+* -version VERSION, -v VERSION        Version number of python project (X.Y.Z)
+* -name NAME, -n NAME                 Your full name
+* -email EMAIL, -e EMAIL              Your email address
+* -gituser GITUSER, -g GITUSER        Your username on Github
+* -pyversion PYVERSION, -p PYVERSION  Minimum version of Python required
 
 ### Python In-Line Usage
 
 * Example below can be ran as a standalone code example
 * Example includes standard Python packages shutil, os, and sys
 * In-line usage of pypackagelib is shown when calling "ppl."
```

### Comparing `pyprojectlib-0.0.2/pyproject.toml` & `pyprojectlib-0.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -12,18 +12,17 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     'Operating System :: Microsoft :: Windows',
     'Operating System :: Unix',
 ]
 
 name = "pyprojectlib"
-version = "0.0.2"
+version = "0.0.3"
 authors = [{ name = "Jason Krist", email = "jkrist2696@gmail.com" }]
 description = ""
-requires-python = ">=3.12.0"
 dependencies = ["cleandoc>=0.0.13","GitPython>=3.1.40","pipreqs>=0.4.13","pytest>=7.4.3","build","twine","tomli","tomli-w","types-requests","types-setuptools"]
 [tool.setuptools.package-data]
 pyprojectlib = ["*.typed", ".template"]
 [project.scripts]
 ppl="pyprojectlib:cli_main"
 [project.urls]
 "Homepage" = "https://github.com/jkrist2696/pyprojectlib"
```

### Comparing `pyprojectlib-0.0.2/src/pyprojectlib/__init__.py` & `pyprojectlib-0.0.3/src/pyprojectlib/__init__.py`

 * *Files identical despite different names*

### Comparing `pyprojectlib-0.0.2/src/pyprojectlib/cli.py` & `pyprojectlib-0.0.3/src/pyprojectlib/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 PROJNAME = "proj"
 USERNAME = "user"
 REPOPATHNAME = "repopath"
 PROJPATHNAME = "projpath"
 NAMENAME = "name"
 EMNAME = "email"
 GUNAME = "gituser"
+PYVERNAME = "pyversion"
 RELNAME = "relpath"
 NCNAME = "noclean"
 NDNAME = "nodoc"
 NTNAME = "notest"
 VERNAME = "version"
 UPNAME = "upload"
 INNAME = "install"
@@ -44,18 +45,15 @@
 RELPATH_H = "Relative path from repository basedir to add project"
 NOCLEAN_H = "Flag to prevent checking py files for cleanliness"
 NODOC_H = "Flag to prevent html documentation creation"
 NOTEST_H = "Flag to prevent pytest from running"
 NAME_H = "Your full name"
 EMAIL_H = "Your email address"
 GITU_H = "Your username on Github"
-
-
-def create_parser():
-    """create parser object"""
+PYVERS_H = "Minimum version of Python required"
 
 
 def cli_parse():
     """Run command line parsing"""
 
     parser = ArgumentParser(prog=PROG, description=DESC_H)
     subparsers = parser.add_subparsers(dest=CMDNAME, help=COMMAND_H)
@@ -90,14 +88,15 @@
     pack_parser.add_argument(PROJPATHNAME, type=str, help=PROJPATH_H)
     pack_parser.add_argument(f"-{UPNAME}", "-u", action="store_true", help=UPLOAD_H)
     pack_parser.add_argument(f"-{INNAME}", "-i", action="store_true", help=INSTALL_H)
     pack_parser.add_argument(f"-{VERNAME}", "-v", type=str, default="", help=VERSION_H)
     pack_parser.add_argument(f"-{NAMENAME}", "-n", type=str, default="", help=NAME_H)
     pack_parser.add_argument(f"-{EMNAME}", "-e", type=str, default="", help=EMAIL_H)
     pack_parser.add_argument(f"-{GUNAME}", "-g", type=str, default="", help=GITU_H)
+    pack_parser.add_argument(f"-{PYVERNAME}", "-p", type=str, default="", help=PYVERS_H)
 
     args = parser.parse_args()
     argitems = vars(args).items()
     args_str = "\n    ".join([f"{key.ljust(8)}: {value}" for key, value in argitems])
     print(f"\nCommand Line Args:\n    {args_str}\n")
     helpdict: dict[str, str] = {}
     helpdict[CMDNAME] = parser.format_help()
```

### Comparing `pyprojectlib-0.0.2/src/pyprojectlib/constants.py` & `pyprojectlib-0.0.3/src/pyprojectlib/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,8 +60,9 @@
     "dist/",
     "docs/conf.txt",  # "src/proj/__pycache__
     "test/__pycache__",
     "test/.mypy_cache/",
     "test/docs",
     "test/examples",
     "test/cleandoc_log.txt",
+    "src/*.egg-info/",
 ]
```

### Comparing `pyprojectlib-0.0.2/src/pyprojectlib/helper.py` & `pyprojectlib-0.0.3/src/pyprojectlib/helper.py`

 * *Files identical despite different names*

### Comparing `pyprojectlib-0.0.2/src/pyprojectlib/pypackage.py` & `pyprojectlib-0.0.3/src/pyprojectlib/pypackage.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Manual Build Steps:
     python -m build
     twine check dist/*
     pip install .
     twine upload dist/*
 
 """
+
 from os import path, mkdir
 from re import split
 from shutil import rmtree
 import pipreqs.pipreqs as pr  # type: ignore # pylint: disable=E0401
 from . import constants as CONS  # type: ignore # pylint: disable=E0611,E0401
 from .helper import prompt_user, run_capture_out
 from .pyuser import User
@@ -55,24 +56,46 @@
     def get_dep_pkgs(self):
         """get dep pkgs"""
         self._get_pipreqs()
         self._get_requirements()
         self._remove_dep_dups()
         self._save_requirements()
 
-    def save_toml(self):
+    def save_toml(self, pyversion: str = ""):
         """save_toml"""
         depstr = ",".join([f'"{pkg}"' for pkg in self.dep_pkgs])
         toml_str = CONS.TOMLSTR_START + f'name = "{self.name}"\n'
         toml_str += f'version = "{self.version}"\n'
         author = self.author
         toml_str += 'authors = [{ name = "'
         toml_str += f'{author.name}", email = "{author.email}" }}]\n'
         toml_str += f'description = "{self.description}"\n'
-        toml_str += f'requires-python = ">={self.pyversion}"\n'
+        if "current" in pyversion.lower():
+            toml_str += f'requires-python = ">={self.pyversion}"\n'
+        elif len(pyversion) > 0:
+            pyvers = pyversion.split(".")
+            helpstr = (
+                "Python version must have 2 numbers with a period between them (X.Y)"
+            )
+            if any([len(pyvers) < 2, len(pyvers) > 2]):
+                raise ValueError(f"pyversion: {pyversion}\n{helpstr}")
+            if not all([pyvers[0].isdigit(), pyvers[1].isdigit()]):
+                raise ValueError(f"pyversion: {pyversion}\n{helpstr}")
+            if any(
+                [
+                    int(pyvers[0]) <= 1,
+                    int(pyvers[0]) >= 4,
+                    int(pyvers[1]) < 0,
+                    int(pyvers[1]) > 12,
+                ]
+            ):
+                raise ValueError(
+                    f"pyversion: {pyversion}\nPython Version must be in range [2.0, 3.12]"
+                )
+            toml_str += f'requires-python = ">={pyversion}"\n'
         toml_str += f"dependencies = [{depstr}]\n"
         # toml_str += '[tool.setuptools.packages.find]\nwhere = ["src"]\n'
         # toml_str += f'exclude = ["*.__pycache__"]\n'
         toml_str += "[tool.setuptools.package-data]\n"
         toml_str += f'{self.name} = ["*.typed", ".template"]\n'
         # toml_str += "[tool.setuptools.exclude-package-data]\n"
         # toml_str += f'{self.name} = ["__pycache__/*", "__pycache__"]\n'
```

### Comparing `pyprojectlib-0.0.2/src/pyprojectlib/pyproject.py` & `pyprojectlib-0.0.3/src/pyprojectlib/pyproject.py`

 * *Files identical despite different names*

### Comparing `pyprojectlib-0.0.2/src/pyprojectlib/pyrepo.py` & `pyprojectlib-0.0.3/src/pyprojectlib/pyrepo.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,19 @@
         self.repoprojpath = path.join(repo.path, self.relpath, self.name)
         self.versiondir = path.join(self.repoprojpath, CONS.VERSIONS_DIR)
         self.version = self.get_version(self.versiondir)
         self.versionpath = path.join(self.versiondir, self.version)
         self.required = [CONS.REQFILE, CONS.READFILE, CONS.TEST_DIR, f"src/{self.name}"]
 
     def update(
-        self, test: bool = True, clean: bool = True, doc: bool = True, git: bool = True
+        self,
+        test: bool = True,
+        clean: bool = True,
+        doc: bool = True,
+        git: bool = True,
     ):
         """check code quality, then copy over new version"""
         self._check_required()
         srcpath = path.join(self.path, "src", self.name)
         if clean:
             logstr = (
                 f'Repo "{self.repo.name}" Project "{self.name}" - '
@@ -147,15 +151,16 @@
         CONS.log().info(logstr)
 
     def package(self, **kwargs):
         """build project into package"""
         upload = kwargs.pop("upload", False)
         install = kwargs.pop("install", False)
         pkg = Package(self.repoprojpath, self.repo.user, **kwargs)
-        pkg.save_toml()
+        pyversion = kwargs.pop("pyversion", "")
+        pkg.save_toml(pyversion=pyversion)
         pkg.build(upload=upload, install=install)
 
     def _prompt(self):
         """prompt"""
         self.relpath = prompt_user("Relative Path in Repo: ", self.relpath)
 
     def _check_args(self):
```

### Comparing `pyprojectlib-0.0.2/src/pyprojectlib/pyuser.py` & `pyprojectlib-0.0.3/src/pyprojectlib/pyuser.py`

 * *Files identical despite different names*

### Comparing `pyprojectlib-0.0.2/src/pyprojectlib.egg-info/PKG-INFO` & `pyprojectlib-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: pyprojectlib
-Version: 0.0.2
+Version: 0.0.3
 Author-email: Jason Krist <jkrist2696@gmail.com>
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/jkrist2696/pyprojectlib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
-Requires-Python: >=3.12.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: cleandoc>=0.0.13
 Requires-Dist: GitPython>=3.1.40
 Requires-Dist: pipreqs>=0.4.13
 Requires-Dist: pytest>=7.4.3
 Requires-Dist: build
@@ -40,90 +39,93 @@
 ### Command Line Usage: "ppl"
 
 usage: ppl [-h] {new,push,pack} ...
 
 Package for managing local python projects and repositories
 
 positional arguments:
-*  {new,push,pack}  Command to execute (options below)
-    *    new            Create a new repo, project, or user of a repo
-    *    push           Save your python project in a local repository
-    *    pack           Package python project into a distributable module
+
+* {new,push,pack}  Command to execute (options below)
+    * new            Create a new repo, project, or user of a repo
+    * push           Save your python project in a local repository
+    * pack           Package python project into a distributable module
 
 ### Command Line Usage: "ppl">"new"
 
 usage: ppl new [-h] {repo,proj,user} ...
 
 positional arguments:
-*    {repo,proj,user}  Create something (options below)
-    *     repo            Create a new empty repository
-    *     proj            Create a new empty project
-    *     user            Add a new user to a local repository
+
+* {repo,proj,user}  Create something (options below)
+    * repo            Create a new empty repository
+    * proj            Create a new empty project
+    * user            Add a new user to a local repository
 
 ### Command Line Usage: "ppl">"new">"repo"
 
-usage: ppl new repo [-h] [-name NAME] [-email EMAIL] [-gituser GITUSER] repopath
+usage: ppl new repo repopath [-h] [-name NAME] [-email EMAIL] [-gituser GITUSER]
 
 positional arguments:
-*    repopath    Path to local python repository. Directory name = repo name.
+* repopath    Path to local python repository. Directory name = repo name.
 
 options:
-*    -name NAME, -n NAME             Your full name
-*    -email EMAIL, -e EMAIL          Your email address
-*    -gituser GITUSER, -g GITUSER    Your username on Github
+* -name NAME, -n NAME             Your full name
+* -email EMAIL, -e EMAIL          Your email address
+* -gituser GITUSER, -g GITUSER    Your username on Github
 
 ### Command Line Usage: "ppl">"new">"project"
 
-usage: ppl new proj [-h] projpath
+usage: ppl new proj projpath [-h]
 
 positional arguments:
-*    projpath    Path to python project. Directory name = project name.
+* projpath    Path to python project. Directory name = project name.
 
 ### Command Line Usage: "ppl">"new">"user"
 
-usage: ppl new user [-h] [-name NAME] [-email EMAIL] [-gituser GITUSER] repopath
+usage: ppl new user repopath [-h] [-name NAME] [-email EMAIL] [-gituser GITUSER]
 
 positional arguments:
-*    repopath              Path to local python repository. Directory name = repo name.
+* repopath              Path to local python repository. Directory name = repo name.
 
 options:
-*    -name NAME, -n NAME             Your full name
-*    -email EMAIL, -e EMAIL          Your email address
-*    -gituser GITUSER, -g GITUSER    Your username on Github
+* -name NAME, -n NAME             Your full name
+* -email EMAIL, -e EMAIL          Your email address
+* -gituser GITUSER, -g GITUSER    Your username on Github
 
 ### Command Line Usage: "ppl">"push"
-usage: ppl push [-h] [-relpath RELPATH] [-noclean] [-nodoc] [-notest] [-version VERSION] [-name NAME] [-email EMAIL] [-gituser GITUSER] repopath projpath
+usage: ppl push repopath projpath [-h] [-relpath RELPATH] [-noclean] [-nodoc] [-notest] [-version VERSION] [-name NAME] [-email EMAIL] [-gituser GITUSER]
 
 positional arguments:
-*    repopath              Path to local python repository. Directory name = repo name.
-*    projpath              Path to python project. Directory name = project name.
+* repopath              Path to local python repository. Directory name = repo name.
+* projpath              Path to python project. Directory name = project name.
 
 options:
-*    -relpath RELPATH, -r RELPATH    Relative path from repository basedir to add project
-*    -noclean, -nc                   Flag to prevent checking py files for cleanliness
-*    -nodoc, -nd                     Flag to prevent html documentation creation
-*    -notest, -nt                    Flag to prevent pytest from running
-*    -version VERSION, -v VERSION    Version number of python project (X.Y.Z)
-*    -name NAME, -n NAME             Your full name
-*    -email EMAIL, -e EMAIL          Your email address
-*    -gituser GITUSER, -g GITUSER    Your username on Github
+* -relpath RELPATH, -r RELPATH    Relative path from repository basedir to add project
+* -noclean, -nc                   Flag to prevent checking py files for cleanliness
+* -nodoc, -nd                     Flag to prevent html documentation creation
+* -notest, -nt                    Flag to prevent pytest from running
+* -version VERSION, -v VERSION    Version number of python project (X.Y.Z)
+* -name NAME, -n NAME             Your full name
+* -email EMAIL, -e EMAIL          Your email address
+* -gituser GITUSER, -g GITUSER    Your username on Github
 
 ### Command Line Usage: "ppl">"pack"
-usage: ppl pack [-h] [-upload] [-install] [-version VERSION] [-name NAME] [-email EMAIL] [-gituser GITUSER] projpath
+usage: ppl pack projpath [-h] [-upload] [-install] [-version VERSION] [-name NAME] [-email EMAIL] [-gituser GITUSER] [-pyversion PYTHONVERSION]
 
 positional arguments:
-*    projpath              Path to python project. Directory name = project name.
+* projpath              Path to python project. Directory name = project name.
 
 options:
-*    -upload, -u                     Flag to upload python module to PYPI after packaging it
-*    -install, -i                    Flag to install python module after packaging it
-*    -version VERSION, -v VERSION    Version number of python project (X.Y.Z)
-*    -name NAME, -n NAME             Your full name
-*    -email EMAIL, -e EMAIL          Your email address
-*    -gituser GITUSER, -g GITUSER    Your username on Github
+* -upload, -u                         Flag to upload python module to PYPI after packaging it
+* -install, -i                        Flag to install python module after packaging it
+* -version VERSION, -v VERSION        Version number of python project (X.Y.Z)
+* -name NAME, -n NAME                 Your full name
+* -email EMAIL, -e EMAIL              Your email address
+* -gituser GITUSER, -g GITUSER        Your username on Github
+* -pyversion PYVERSION, -p PYVERSION  Minimum version of Python required
 
 ### Python In-Line Usage
 
 * Example below can be ran as a standalone code example
 * Example includes standard Python packages shutil, os, and sys
 * In-line usage of pypackagelib is shown when calling "ppl."
```

### Comparing `pyprojectlib-0.0.2/src/pyprojectlib.egg-info/SOURCES.txt` & `pyprojectlib-0.0.3/src/pyprojectlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

