# Comparing `tmp/AutoGitSemVer-0.7.1-py3-none-any.whl.zip` & `tmp/AutoGitSemVer-0.7.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 16199 bytes, number of entries: 11
--rw-r--r--  2.0 unx     2433 b- defN 24-Mar-18 20:02 BuildBinary.py
--rw-r--r--  2.0 unx     2756 b- defN 24-Mar-18 20:02 AutoGitSemVer/AutoGitSemVerSchema.json
--rw-r--r--  2.0 unx     6207 b- defN 24-Mar-18 20:02 AutoGitSemVer/EntryPoint.py
--rw-r--r--  2.0 unx    23413 b- defN 24-Mar-18 20:02 AutoGitSemVer/Lib.py
--rw-r--r--  2.0 unx      882 b- defN 24-Mar-18 20:03 AutoGitSemVer/__init__.py
--rw-r--r--  2.0 unx     1071 b- defN 24-Mar-18 20:03 AutoGitSemVer-0.7.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx    18035 b- defN 24-Mar-18 20:03 AutoGitSemVer-0.7.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-18 20:03 AutoGitSemVer-0.7.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       63 b- defN 24-Mar-18 20:03 AutoGitSemVer-0.7.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       26 b- defN 24-Mar-18 20:03 AutoGitSemVer-0.7.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      931 b- defN 24-Mar-18 20:03 AutoGitSemVer-0.7.1.dist-info/RECORD
-11 files, 55909 bytes uncompressed, 14615 bytes compressed:  73.9%
+Zip file size: 16214 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     2433 b- defN 24-Apr-29 22:54 BuildBinary.py
+-rw-r--r--  2.0 unx     2756 b- defN 24-Apr-29 22:54 AutoGitSemVer/AutoGitSemVerSchema.json
+-rw-r--r--  2.0 unx     6207 b- defN 24-Apr-29 22:54 AutoGitSemVer/EntryPoint.py
+-rw-r--r--  2.0 unx    23413 b- defN 24-Apr-29 22:54 AutoGitSemVer/Lib.py
+-rw-r--r--  2.0 unx      882 b- defN 24-Apr-29 22:54 AutoGitSemVer/__init__.py
+-rw-r--r--  2.0 unx     1071 b- defN 24-Apr-29 22:54 AutoGitSemVer-0.7.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    18050 b- defN 24-Apr-29 22:54 AutoGitSemVer-0.7.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-29 22:54 AutoGitSemVer-0.7.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       63 b- defN 24-Apr-29 22:54 AutoGitSemVer-0.7.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       26 b- defN 24-Apr-29 22:54 AutoGitSemVer-0.7.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      931 b- defN 24-Apr-29 22:54 AutoGitSemVer-0.7.2.dist-info/RECORD
+11 files, 55924 bytes uncompressed, 14630 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: AutoGitSemVer/Lib.py
 Comment: 
 
 Filename: AutoGitSemVer/__init__.py
 Comment: 
 
-Filename: AutoGitSemVer-0.7.1.dist-info/LICENSE.txt
+Filename: AutoGitSemVer-0.7.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: AutoGitSemVer-0.7.1.dist-info/METADATA
+Filename: AutoGitSemVer-0.7.2.dist-info/METADATA
 Comment: 
 
-Filename: AutoGitSemVer-0.7.1.dist-info/WHEEL
+Filename: AutoGitSemVer-0.7.2.dist-info/WHEEL
 Comment: 
 
-Filename: AutoGitSemVer-0.7.1.dist-info/entry_points.txt
+Filename: AutoGitSemVer-0.7.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: AutoGitSemVer-0.7.1.dist-info/top_level.txt
+Filename: AutoGitSemVer-0.7.2.dist-info/top_level.txt
 Comment: 
 
-Filename: AutoGitSemVer-0.7.1.dist-info/RECORD
+Filename: AutoGitSemVer-0.7.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## AutoGitSemVer/__init__.py

```diff
@@ -13,11 +13,11 @@
 # ----------------------------------------------------------------------
 # pylint: disable=missing-module-docstring,invalid-name
 
 # ----------------------------------------------------------------------
 # Note that this value will be overwritten by calls to `python ../../Build.py update_version` based
 # on changes observed in the git repository. The default value below will be used until the value
 # here is explicitly updated as part of a commit.
-__version__ = "0.7.1"
+__version__ = "0.7.2"
 
 
 from .Lib import GenerateStyle, GetSemanticVersion, GetSemanticVersionResult
```

## Comparing `AutoGitSemVer-0.7.1.dist-info/LICENSE.txt` & `AutoGitSemVer-0.7.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `AutoGitSemVer-0.7.1.dist-info/METADATA` & `AutoGitSemVer-0.7.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoGitSemVer
-Version: 0.7.1
+Version: 0.7.2
 Summary: Calculates a semantic version based on git changes.
 Author-email: David Brownell <db@DavidBrownell.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/davidbrownell/AutoGitSemVer
 Project-URL: Documentation, https://github.com/davidbrownell/AutoGitSemVer
 Project-URL: Repository, https://github.com/davidbrownell/AutoGitSemVer
 Classifier: Development Status :: 4 - Beta
@@ -20,25 +20,25 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: System :: System Shells
 Classifier: Topic :: Terminals
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: dbrownell-Common
-Requires-Dist: GitPython ==3.*
-Requires-Dist: jsonschema ==4.*
-Requires-Dist: rtyaml ==1.*
-Requires-Dist: semantic-version ==2.*
+Requires-Dist: dbrownell-Common ==0.*
+Requires-Dist: GitPython ~=3.1
+Requires-Dist: jsonschema ~=4.21
+Requires-Dist: rtyaml ~=1.0
+Requires-Dist: semantic-version ~=2.10
 Provides-Extra: dev
-Requires-Dist: dbrownell-DevTools ; extra == 'dev'
+Requires-Dist: dbrownell-DevTools ==0.* ; extra == 'dev'
 Provides-Extra: package
-Requires-Dist: build ==1.* ; extra == 'package'
-Requires-Dist: cx-Freeze ==6.* ; extra == 'package'
-Requires-Dist: twine ==4.* ; extra == 'package'
+Requires-Dist: build ~=1.2 ; extra == 'package'
+Requires-Dist: cx-Freeze ~=6.15 ; extra == 'package'
+Requires-Dist: twine ~=4.0 ; extra == 'package'
 
 # AutoGitSemVer
 
 [![CI](https://github.com/davidbrownell/AutoGitSemVer/actions/workflows/standard.yaml/badge.svg?event=push)](https://github.com/davidbrownell/AutoGitSemVer/actions/workflows/standard.yaml)
 [![Code Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/davidbrownell/f15146b1b8fdc0a5d45ac0eb786a84f7/raw/AutoGitSemVer_coverage.json)](https://github.com/davidbrownell/AutoGitSemVer/actions)
 [![License](https://img.shields.io/github/license/davidbrownell/AutoGitSemVer?color=dark-green)](https://github.com/davidbrownell/AutoGitSemVer/blob/master/LICENSE.txt)
 [![GitHub commit activity](https://img.shields.io/github/commit-activity/y/davidbrownell/AutoGitSemVer?color=dark-green)](https://github.com/davidbrownell/AutoGitSemVer/commits/main/)
```

### html2text {}

```diff
@@ -1,55 +1,55 @@
-Metadata-Version: 2.1 Name: AutoGitSemVer Version: 0.7.1 Summary: Calculates a
+Metadata-Version: 2.1 Name: AutoGitSemVer Version: 0.7.2 Summary: Calculates a
 semantic version based on git changes. Author-email: David Brownell
 DavidBrownell.com> License: MIT License Project-URL: Homepage, https://
 github.com/davidbrownell/AutoGitSemVer Project-URL: Documentation, https://
 github.com/davidbrownell/AutoGitSemVer Project-URL: Repository, https://
 github.com/davidbrownell/AutoGitSemVer Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Natural Language :: English Classifier:
 Operating System :: MacOS Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Topic :: Software Development Classifier: Topic ::
 System :: System Shells Classifier: Topic :: Terminals Classifier: Topic ::
 Utilities Description-Content-Type: text/markdown License-File: LICENSE.txt
-Requires-Dist: dbrownell-Common Requires-Dist: GitPython ==3.* Requires-Dist:
-jsonschema ==4.* Requires-Dist: rtyaml ==1.* Requires-Dist: semantic-version
-==2.* Provides-Extra: dev Requires-Dist: dbrownell-DevTools ; extra == 'dev'
-Provides-Extra: package Requires-Dist: build ==1.* ; extra == 'package'
-Requires-Dist: cx-Freeze ==6.* ; extra == 'package' Requires-Dist: twine ==4.*
-; extra == 'package' # AutoGitSemVer [![CI](https://github.com/davidbrownell/
-AutoGitSemVer/actions/workflows/standard.yaml/badge.svg?event=push)](https://
-github.com/davidbrownell/AutoGitSemVer/actions/workflows/standard.yaml) [![Code
-Coverage](https://img.shields.io/endpoint?url=https://
-gist.githubusercontent.com/davidbrownell/f15146b1b8fdc0a5d45ac0eb786a84f7/raw/
-AutoGitSemVer_coverage.json)](https://github.com/davidbrownell/AutoGitSemVer/
-actions) [![License](https://img.shields.io/github/license/davidbrownell/
-AutoGitSemVer?color=dark-green)](https://github.com/davidbrownell/
-AutoGitSemVer/blob/master/LICENSE.txt) [![GitHub commit activity](https://
-img.shields.io/github/commit-activity/y/davidbrownell/AutoGitSemVer?color=dark-
-green)](https://github.com/davidbrownell/AutoGitSemVer/commits/main/) [![PyPI -
-Python Version](https://img.shields.io/pypi/pyversions/
-AutoGitSemVer?color=dark-green)](https://pypi.org/project/autogitsemver/) [!
-[PyPI - Version](https://img.shields.io/pypi/v/AutoGitSemVer?color=dark-green)]
-(https://pypi.org/project/autogitsemver/) [![PyPI - Downloads](https://
-img.shields.io/pypi/dm/AutoGitSemVer)](https://pypistats.org/packages/
-autogitsemver) # AutoGitSemVer Generate a [semantic version](https://semver.og)
-based on commits made to a [git](https://git-scm.com/) repository. ### Quick
-Start 1. Install via [executable](#installation-via-executable), [pip]
-(#installation-via-pip), or [local development](#local-development) 2. [Run the
-executable](#running-the-executable) 3. [Advanced Configuration](#advanced-
-configuration) ### Overview AutoGitSemVer uses commits in a git repository to
-calculate a semantic version. A commit's title and/or description can be used
-to increment a specific part of the semantic version and configuration files
-can be applied to control how the semantic version is generated. Finally,
-multiple, distinct semantic versions can be generated from different
-directories within the source tree. ### How to use AutoGitSemVer #### Running
-the Executable From a terminal window, run:
+Requires-Dist: dbrownell-Common ==0.* Requires-Dist: GitPython ~=3.1 Requires-
+Dist: jsonschema ~=4.21 Requires-Dist: rtyaml ~=1.0 Requires-Dist: semantic-
+version ~=2.10 Provides-Extra: dev Requires-Dist: dbrownell-DevTools ==0.* ;
+extra == 'dev' Provides-Extra: package Requires-Dist: build ~=1.2 ; extra ==
+'package' Requires-Dist: cx-Freeze ~=6.15 ; extra == 'package' Requires-Dist:
+twine ~=4.0 ; extra == 'package' # AutoGitSemVer [![CI](https://github.com/
+davidbrownell/AutoGitSemVer/actions/workflows/standard.yaml/
+badge.svg?event=push)](https://github.com/davidbrownell/AutoGitSemVer/actions/
+workflows/standard.yaml) [![Code Coverage](https://img.shields.io/
+endpoint?url=https://gist.githubusercontent.com/davidbrownell/
+f15146b1b8fdc0a5d45ac0eb786a84f7/raw/AutoGitSemVer_coverage.json)](https://
+github.com/davidbrownell/AutoGitSemVer/actions) [![License](https://
+img.shields.io/github/license/davidbrownell/AutoGitSemVer?color=dark-green)]
+(https://github.com/davidbrownell/AutoGitSemVer/blob/master/LICENSE.txt) [!
+[GitHub commit activity](https://img.shields.io/github/commit-activity/y/
+davidbrownell/AutoGitSemVer?color=dark-green)](https://github.com/
+davidbrownell/AutoGitSemVer/commits/main/) [![PyPI - Python Version](https://
+img.shields.io/pypi/pyversions/AutoGitSemVer?color=dark-green)](https://
+pypi.org/project/autogitsemver/) [![PyPI - Version](https://img.shields.io/
+pypi/v/AutoGitSemVer?color=dark-green)](https://pypi.org/project/autogitsemver/
+) [![PyPI - Downloads](https://img.shields.io/pypi/dm/AutoGitSemVer)](https://
+pypistats.org/packages/autogitsemver) # AutoGitSemVer Generate a [semantic
+version](https://semver.og) based on commits made to a [git](https://git-
+scm.com/) repository. ### Quick Start 1. Install via [executable]
+(#installation-via-executable), [pip](#installation-via-pip), or [local
+development](#local-development) 2. [Run the executable](#running-the-
+executable) 3. [Advanced Configuration](#advanced-configuration) ### Overview
+AutoGitSemVer uses commits in a git repository to calculate a semantic version.
+A commit's title and/or description can be used to increment a specific part of
+the semantic version and configuration files can be applied to control how the
+semantic version is generated. Finally, multiple, distinct semantic versions
+can be generated from different directories within the source tree. ### How to
+use AutoGitSemVer #### Running the Executable From a terminal window, run:
 SScceennaarriioo CCoommmmaanndd LLiinnee  OOuuttppuutt
                        Loading AutoGitSemVer configuration...DONE! (0, 0:00:00.001464, default configuration info will be used)
                        Enumerating changes...DONE! (0, 0:00:00.193258, 1 change processed, no changes applied [0.00%])
                        Calculating semantic version...
 Standard autogitsemver   0.6.1+20240318122529.BROWNELL08
                        DONE! (0, 0:00:00.054236)
```

## Comparing `AutoGitSemVer-0.7.1.dist-info/RECORD` & `AutoGitSemVer-0.7.2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 BuildBinary.py,sha256=CrOg39LilVUF-xy1KIP8o3KI2m_cYP_VCzBQUDI6-Dc,2433
 AutoGitSemVer/AutoGitSemVerSchema.json,sha256=2n2DRw-JReiYcD9jmw3mjbsKNZjheKIvhVdQz6FmP2s,2756
 AutoGitSemVer/EntryPoint.py,sha256=jpe3CRtmgYl8yu4W0XfqVnJ7IXcJ47oCf0D_EsXcE_s,6207
 AutoGitSemVer/Lib.py,sha256=vaR0ovpm219oCIJ14vXYLnMsl1s-3H9ruqP-DQuD3wA,23413
-AutoGitSemVer/__init__.py,sha256=Ysd8finlRh4qi3fkbWBmmGf6Yu-mLiCW27Xx775xgMs,882
-AutoGitSemVer-0.7.1.dist-info/LICENSE.txt,sha256=6ycKI8SWG920Saey4PGi5YUVLX0C_8hfqJr7Q0sqGI8,1071
-AutoGitSemVer-0.7.1.dist-info/METADATA,sha256=2KesiLkF5Fr_R7SBTl00A8CUGGkqO0AcuxmFkTIkLh0,18035
-AutoGitSemVer-0.7.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-AutoGitSemVer-0.7.1.dist-info/entry_points.txt,sha256=G8GOzgDIIgHgBzYb4RuCBwRUQtSLd7SW-DihP0oTU9Y,63
-AutoGitSemVer-0.7.1.dist-info/top_level.txt,sha256=Q6jMBQnUOSQS-cq3i7AjILoN-JIyZe1D8FBCnOXgKXQ,26
-AutoGitSemVer-0.7.1.dist-info/RECORD,,
+AutoGitSemVer/__init__.py,sha256=q3ClVk8B-b_Pliu_RuoscWhBB8Qdo_ufz_FT2X8wjq4,882
+AutoGitSemVer-0.7.2.dist-info/LICENSE.txt,sha256=6ycKI8SWG920Saey4PGi5YUVLX0C_8hfqJr7Q0sqGI8,1071
+AutoGitSemVer-0.7.2.dist-info/METADATA,sha256=fBuEj5q-CIBlGGmnTA_46hjcDgpfogR72ME7NG8Ss1g,18050
+AutoGitSemVer-0.7.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+AutoGitSemVer-0.7.2.dist-info/entry_points.txt,sha256=G8GOzgDIIgHgBzYb4RuCBwRUQtSLd7SW-DihP0oTU9Y,63
+AutoGitSemVer-0.7.2.dist-info/top_level.txt,sha256=Q6jMBQnUOSQS-cq3i7AjILoN-JIyZe1D8FBCnOXgKXQ,26
+AutoGitSemVer-0.7.2.dist-info/RECORD,,
```

