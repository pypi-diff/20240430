# Comparing `tmp/snipinator-1.3.1.tar.gz` & `tmp/snipinator-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/gdrive/code/snipinator.develop/develop/dist/.tmp-sme1l8pz/snipinator-1.3.1.tar", last modified: Mon Apr 22 15:34:03 2024, max compression
+gzip compressed data, was "/mnt/c/gdrive/code/snipinator.develop/develop/dist/.tmp-89aqwtpv/snipinator-1.4.0.tar", last modified: Tue Apr 30 19:05:23 2024, max compression
```

## Comparing `snipinator-1.3.1.tar` & `snipinator-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-22 15:34:03.904261 snipinator-1.3.1/
--rwxrwxrwx   0 realz     (1000) realz     (1000)     1102 2024-03-21 17:40:02.000000 snipinator-1.3.1/LICENSE.md
--rwxrwxrwx   0 realz     (1000) realz     (1000)    36850 2024-04-22 15:34:03.895716 snipinator-1.3.1/PKG-INFO
--rwxrwxrwx   0 realz     (1000) realz     (1000)    29974 2024-04-22 15:32:53.000000 snipinator-1.3.1/README.md
--rwxrwxrwx   0 realz     (1000) realz     (1000)     4199 2024-04-22 15:32:54.000000 snipinator-1.3.1/pyproject.toml
--rwxrwxrwx   0 realz     (1000) realz     (1000)       38 2024-04-22 15:34:03.904261 snipinator-1.3.1/setup.cfg
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-22 15:34:03.791354 snipinator-1.3.1/snipinator/
--rwxrwxrwx   0 realz     (1000) realz     (1000)      514 2024-03-27 14:51:50.000000 snipinator-1.3.1/snipinator/__init__.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)    18915 2024-04-16 05:46:20.000000 snipinator-1.3.1/snipinator/cli.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)    32718 2024-04-19 08:57:30.000000 snipinator-1.3.1/snipinator/snipinate copy.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)    32450 2024-04-22 15:32:54.000000 snipinator-1.3.1/snipinator/snipinate.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)      866 2024-03-21 17:40:02.000000 snipinator-1.3.1/snipinator/snipinate_test.py
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-22 15:34:03.878841 snipinator-1.3.1/snipinator.egg-info/
--rwxrwxrwx   0 realz     (1000) realz     (1000)    36850 2024-04-22 15:34:03.000000 snipinator-1.3.1/snipinator.egg-info/PKG-INFO
--rwxrwxrwx   0 realz     (1000) realz     (1000)      364 2024-04-22 15:34:03.000000 snipinator-1.3.1/snipinator.egg-info/SOURCES.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)        1 2024-04-22 15:34:03.000000 snipinator-1.3.1/snipinator.egg-info/dependency_links.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)       51 2024-04-22 15:34:03.000000 snipinator-1.3.1/snipinator.egg-info/entry_points.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)     1820 2024-04-22 15:34:03.000000 snipinator-1.3.1/snipinator.egg-info/requires.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)       11 2024-04-22 15:34:03.000000 snipinator-1.3.1/snipinator.egg-info/top_level.txt
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-30 19:05:23.823352 snipinator-1.4.0/
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     1102 2024-04-30 19:04:32.000000 snipinator-1.4.0/LICENSE.md
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    45946 2024-04-30 19:05:23.813512 snipinator-1.4.0/PKG-INFO
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    38974 2024-04-30 19:04:32.000000 snipinator-1.4.0/README.md
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     4199 2024-04-30 19:04:32.000000 snipinator-1.4.0/pyproject.toml
+-rwxrwxrwx   0 realz     (1000) realz     (1000)       38 2024-04-30 19:05:23.823352 snipinator-1.4.0/setup.cfg
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-30 19:05:23.681312 snipinator-1.4.0/snipinator/
+-rwxrwxrwx   0 realz     (1000) realz     (1000)      514 2024-03-27 14:51:50.000000 snipinator-1.4.0/snipinator/__init__.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    18915 2024-04-26 18:29:05.000000 snipinator-1.4.0/snipinator/cli.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    34778 2024-04-30 19:04:32.000000 snipinator-1.4.0/snipinator/snipinate.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)      866 2024-03-21 17:40:02.000000 snipinator-1.4.0/snipinator/snipinate_test.py
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-30 19:05:23.797223 snipinator-1.4.0/snipinator.egg-info/
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    45946 2024-04-30 19:05:23.000000 snipinator-1.4.0/snipinator.egg-info/PKG-INFO
+-rwxrwxrwx   0 realz     (1000) realz     (1000)      335 2024-04-30 19:05:23.000000 snipinator-1.4.0/snipinator.egg-info/SOURCES.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)        1 2024-04-30 19:05:23.000000 snipinator-1.4.0/snipinator.egg-info/dependency_links.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)       51 2024-04-30 19:05:23.000000 snipinator-1.4.0/snipinator.egg-info/entry_points.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     1820 2024-04-30 19:05:23.000000 snipinator-1.4.0/snipinator.egg-info/requires.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)       11 2024-04-30 19:05:23.000000 snipinator-1.4.0/snipinator.egg-info/top_level.txt
```

### Comparing `snipinator-1.3.1/LICENSE.md` & `snipinator-1.4.0/LICENSE.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 MIT License
 
 Copyright (c) 2024 Azriel Fasten.
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software is furnished to do so,
+subject to the following conditions:
 
-The above copyright notice and this permission notice (including the next paragraph) shall be included in all copies or substantial portions of the Software.
+The above copyright notice and this permission notice (including the next
+paragraph) shall be included in all copies or substantial portions of the
+Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `snipinator-1.3.1/PKG-INFO` & `snipinator-1.4.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,171 +1,55 @@
-Metadata-Version: 2.1
-Name: snipinator
-Version: 1.3.1
-Summary: Python code snippets for markdown files, e.g READMEs, from actual (testable) code.
-Author-email: AYF <realazthat@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2024 Azriel Fasten.
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice (including the next paragraph) shall be included in all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/realazthat/snipinator
-Project-URL: Documentation, https://github.com/realazthat/snipinator
-Project-URL: Repository, https://github.com/realazthat/snipinator
-Keywords: github,testing,markdown,readme,snippets,documentation,jinja2,templates,preprocessor,documentation-tool,include,readme-template,readme-md,dynamic-documentation
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: colorama<1,>=0.4
-Requires-Dist: defusedxml<1,>=0.7
-Requires-Dist: importlib-metadata; python_version < "3.8"
-Requires-Dist: Jinja2<4,>=3
-Requires-Dist: markdown-it-py<4,>=3
-Requires-Dist: MarkupSafe<3,>=2
-Requires-Dist: mdurl<1
-Requires-Dist: pexpect<5,>4
-Requires-Dist: ptyprocess<0.8,>=0.7
-Requires-Dist: Pygments<3,>=2
-Requires-Dist: rich<14,>=13
-Requires-Dist: rich-argparse<2,>=1
-Requires-Dist: types-colorama<1,>=0.4
-Provides-Extra: prod
-Requires-Dist: colorama==0.4.6; extra == "prod"
-Requires-Dist: defusedxml==0.7.1; extra == "prod"
-Requires-Dist: jinja2==3.1.3; extra == "prod"
-Requires-Dist: markdown-it-py==3.0.0; extra == "prod"
-Requires-Dist: markupsafe==2.1.5; extra == "prod"
-Requires-Dist: mdurl==0.1.2; extra == "prod"
-Requires-Dist: pexpect==4.9.0; extra == "prod"
-Requires-Dist: ptyprocess==0.7.0; extra == "prod"
-Requires-Dist: pygments==2.17.2; extra == "prod"
-Requires-Dist: rich==13.7.1; extra == "prod"
-Requires-Dist: rich-argparse==1.4.0; extra == "prod"
-Requires-Dist: types-colorama==0.4.15.20240311; extra == "prod"
-Requires-Dist: typing-extensions==4.10.0; extra == "prod"
-Provides-Extra: dev
-Requires-Dist: argcomplete==3.2.3; extra == "dev"
-Requires-Dist: autoflake==2.3.1; extra == "dev"
-Requires-Dist: build==1.0.3; extra == "dev"
-Requires-Dist: certifi==2024.2.2; extra == "dev"
-Requires-Dist: cffi==1.16.0; extra == "dev"
-Requires-Dist: cfgv==3.4.0; extra == "dev"
-Requires-Dist: changeguard==0.3.1; extra == "dev"
-Requires-Dist: charset-normalizer==3.3.2; extra == "dev"
-Requires-Dist: click==8.1.7; extra == "dev"
-Requires-Dist: colorama==0.4.6; extra == "dev"
-Requires-Dist: cryptography==42.0.5; extra == "dev"
-Requires-Dist: defusedxml==0.7.1; extra == "dev"
-Requires-Dist: distlib==0.3.8; extra == "dev"
-Requires-Dist: docutils==0.20.1; extra == "dev"
-Requires-Dist: filelock==3.13.1; extra == "dev"
-Requires-Dist: identify==2.5.35; extra == "dev"
-Requires-Dist: idna==3.6; extra == "dev"
-Requires-Dist: importlib-metadata==7.0.2; extra == "dev"
-Requires-Dist: importlib-resources==6.3.1; extra == "dev"
-Requires-Dist: isort==5.13.2; extra == "dev"
-Requires-Dist: jaraco-classes==3.3.1; extra == "dev"
-Requires-Dist: jeepney==0.8.0; extra == "dev"
-Requires-Dist: jinja2==3.1.3; extra == "dev"
-Requires-Dist: keyring==24.3.1; extra == "dev"
-Requires-Dist: markdown-it-py==3.0.0; extra == "dev"
-Requires-Dist: markupsafe==2.1.5; extra == "dev"
-Requires-Dist: mdformat==0.7.17; extra == "dev"
-Requires-Dist: mdformat-gfm==0.3.0; extra == "dev"
-Requires-Dist: mdformat-tables==0.4.1; extra == "dev"
-Requires-Dist: mdit-py-plugins==0.4.0; extra == "dev"
-Requires-Dist: mdurl==0.1.2; extra == "dev"
-Requires-Dist: more-itertools==10.2.0; extra == "dev"
-Requires-Dist: mypy==1.8.0; extra == "dev"
-Requires-Dist: mypy-extensions==1.0.0; extra == "dev"
-Requires-Dist: nh3==0.2.15; extra == "dev"
-Requires-Dist: nodeenv==1.8.0; extra == "dev"
-Requires-Dist: packaging==23.2; extra == "dev"
-Requires-Dist: pathspec==0.12.1; extra == "dev"
-Requires-Dist: pexpect==4.9.0; extra == "dev"
-Requires-Dist: pip-licenses==4.3.4; extra == "dev"
-Requires-Dist: pip-tools==7.3.0; extra == "dev"
-Requires-Dist: pkginfo==1.9.6; extra == "dev"
-Requires-Dist: platformdirs==4.2.0; extra == "dev"
-Requires-Dist: pre-commit==3.5.0; extra == "dev"
-Requires-Dist: prettytable==3.10.0; extra == "dev"
-Requires-Dist: ptyprocess==0.7.0; extra == "dev"
-Requires-Dist: pycparser==2.21; extra == "dev"
-Requires-Dist: pyflakes==3.2.0; extra == "dev"
-Requires-Dist: pygments==2.17.2; extra == "dev"
-Requires-Dist: pyproject-hooks==1.0.0; extra == "dev"
-Requires-Dist: pyright==1.1.352; extra == "dev"
-Requires-Dist: pyyaml==6.0.1; extra == "dev"
-Requires-Dist: readme-renderer==43.0; extra == "dev"
-Requires-Dist: requests==2.31.0; extra == "dev"
-Requires-Dist: requests-toolbelt==1.0.0; extra == "dev"
-Requires-Dist: rfc3986==2.0.0; extra == "dev"
-Requires-Dist: rich==13.7.1; extra == "dev"
-Requires-Dist: rich-argparse==1.4.0; extra == "dev"
-Requires-Dist: secretstorage==3.3.3; extra == "dev"
-Requires-Dist: toml-sort==0.23.1; extra == "dev"
-Requires-Dist: tomli==2.0.1; extra == "dev"
-Requires-Dist: tomlkit==0.12.4; extra == "dev"
-Requires-Dist: twine==5.0.0; extra == "dev"
-Requires-Dist: types-colorama==0.4.15.20240311; extra == "dev"
-Requires-Dist: types-pyyaml==6.0.12.20240311; extra == "dev"
-Requires-Dist: typing-extensions==4.10.0; extra == "dev"
-Requires-Dist: urllib3==2.2.1; extra == "dev"
-Requires-Dist: virtualenv==20.25.0; extra == "dev"
-Requires-Dist: wcwidth==0.2.13; extra == "dev"
-Requires-Dist: wheel==0.43.0; extra == "dev"
-Requires-Dist: xmltodict==0.13.0; extra == "dev"
-Requires-Dist: yapf==0.40.2; extra == "dev"
-Requires-Dist: yq==3.2.3; extra == "dev"
-Requires-Dist: zipp==3.17.0; extra == "dev"
-
 <!--
 
 WARNING: This file is auto-generated by snipinator. Do not edit directly.
 SOURCE: `README.md.jinja2`.
 
 -->
 <!--
 
 
 
 
+
+
+
 -->
 
-# <div align="center">![Snipinator][22]</div>
+# <div align="center">[![Snipinator][22]][56]</div>
 
 <div align="center">
 
 <!-- Icons from https://lucide.dev/icons/users -->
 <!-- Icons from https://lucide.dev/icons/laptop-minimal -->
 
 ![**Audience:** Developers][19] ![**Platform:** Linux][20]
 
 </div>
 
 <p align="center">
   <strong>
-    <a href="#-features">🎇Features</a> &nbsp;&bull;&nbsp;
-    <a href="#-installation">🛠️Installation</a> &nbsp;&bull;&nbsp;
-    <a href="#-usage">🔧Usage</a> &nbsp;&bull;&nbsp;
-    <a href="#-command-line-options">💻CLI</a> &nbsp;&bull;&nbsp;
-    <a href="#-examples">💡Examples</a> &nbsp;&bull;&nbsp;
-    <a href="#-api">🤖API</a> &nbsp;&bull;&nbsp;
-    <a href="#-requirements">✅Requirements</a> &nbsp;&bull;&nbsp;
+    <a href="https://github.com/realazthat/snipinator">🏠Home</a>
+    &nbsp;&bull;&nbsp;
+    <a href="#-features">🎇Features</a>
+    &nbsp;&bull;&nbsp;
+    <a href="#-installation">🔨Installation</a>
+    &nbsp;&bull;&nbsp;
+    <a href="#-usage">🚜Usage</a>
+    &nbsp;&bull;&nbsp;
+    <a href="#-command-line-options">💻CLI</a>
+    &nbsp;&bull;&nbsp;
+    <a href="#-examples">💡Examples</a>
+  </strong>
+</p>
+<p align="center">
+  <strong>
+    <a href="#-jinja2-api">🤖Jinja2 API</a>
+    &nbsp;&bull;&nbsp;
+    <a href="#-requirements">✅Requirements</a>
+    &nbsp;&bull;&nbsp;
     <a href="#-gotchas-and-limitations">🚸Gotchas</a>
   </strong>
 </p>
 
 <div align="center">
 
 ![Top language][9] [![GitHub License][3]][21] [![PyPI - Version][4]][5]
@@ -186,16 +70,16 @@
 
 </div>
 
 <img src=".github/demo.gif" alt="Demo" width="100%">
 
 ## ❔ What
 
-What it does: **Snipinator** lets you take a `EXAMPLE.md` template and include
-snippets from your (working and tested) codebase.
+What it does: **Snipinator** lets you take a `EXAMPLE.md` template
+and include snippets from your (working and tested) codebase.
 
 Turn this ([./snipinator/examples/EXAMPLE.md.jinja2](./snipinator/examples/EXAMPLE.md.jinja2)):
 
 <!---->
 ```md
 # A README
 
@@ -256,25 +140,25 @@
 - 🥇🔖📜 First-class support for **Markdown** templates (with `backtickify`,
   `decomentify`).
 - 📦🐚🖨️ Can include **[shell](#shell) output**.
   - Supports ANSI colors :heart: :green_heart: :blue_heart: with SVG output
     :camera:.
 - ⚙️🔗🗃️ More robust **references/links** to local files using [path()](#path).
 
-## 🛠️ Installation
+## 🔨 Installation
 
 ```bash
 # Install from pypi (https://pypi.org/project/snipinator/)
 pip install snipinator
 
 # Install from git (https://github.com/realazthat/snipinator)
-pip install git+https://github.com/realazthat/snipinator.git@v1.3.1
+pip install git+https://github.com/realazthat/snipinator.git@v1.4.0
 ```
 
-## 🔧 Usage
+## 🚜 Usage
 
 Example template README:
 ([./snipinator/examples/EXAMPLE.md.jinja2](./snipinator/examples/EXAMPLE.md.jinja2)):
 
 <!---->
 ```md
 # A README
@@ -345,61 +229,64 @@
   - Template:
     [./snipinator/examples/LONG-EXAMPLE.md.jinja2](./snipinator/examples/LONG-EXAMPLE.md.jinja2).
   - Generated:
     [./snipinator/examples/LONG-EXAMPLE.generated.md](./snipinator/examples/LONG-EXAMPLE.generated.md).
   - Generation script:
     [./snipinator/examples/long-example.sh](./snipinator/examples/long-example.sh).
 - Projects using Snipinator:
-  - [github.com/realazthat/snipinator](https://github.com/realazthat/snipinator),
-    See
+  - [realazthat/snipinator](https://github.com/realazthat/snipinator), See
     [snipinator/README.md.jinja2](https://github.com/realazthat/snipinator/blob/61cb88593baa099dc375cf5fd40679e4be673fc5/README.md.jinja2).
-  - [github.com/realazthat/changeguard](https://github.com/realazthat/changeguard),
-    See
+  - [realazthat/changeguard](https://github.com/realazthat/changeguard), See
     [changeguard/README.md.jinja2](https://github.com/realazthat/changeguard/blob/87d5104b52e651bb9195a3d46dd7f050acbcb534/README.md.jinja2).
-  - [github.com/realazthat/comfy-catapult](https://github.com/realazthat/comfy-catapult),
+  - [realazthat/comfy-catapult](https://github.com/realazthat/comfy-catapult),
     See
     [comfy-catapult/README.md.jinja2](https://github.com/realazthat/comfy-catapult/blob/ff353d48b25fa7b9c35fa11b31d5f2b3039c41c8/README.md.jinja2).
-  - [github.com/realazthat/comfylowda](https://github.com/realazthat/comfylowda),
-    See
+  - [realazthat/comfylowda](https://github.com/realazthat/comfylowda), See
     [comfylowda/README.md.jinja2](https://github.com/realazthat/comfylowda/blob/e01a32c38107aa0b89ccea21c4678d193a186a78/README.md.jinja2).
-  - [github.com/realazthat/excalidraw-brute-export-cli](https://github.com/realazthat/excalidraw-brute-export-cli),
+  - [realazthat/excalidraw-brute-export-cli](https://github.com/realazthat/excalidraw-brute-export-cli),
     See
     [excalidraw-brute-export-cli/README.md.jinja2](https://github.com/realazthat/excalidraw-brute-export-cli/blob/54a3b5b08b644e61c721ab565c576094234c5cc7/README.md.jinja2).
 
-## 🤖 API
+## 🤖 Jinja2 API
+
+The regular Jinja2 v3 template syntax is supported. For more information, see
+[Template Designer Documentation](https://jinja.palletsprojects.com/en/3.1.x/templates/).
 
-(Jinja2) Functions made available:
+Additional (Jinja2) functions made available:
 
-### pysnippet
+### 🐍✂ pysnippet
 
 Used several times in
 [./snipinator/examples/LONG-EXAMPLE.md.jinja2](./snipinator/examples/LONG-EXAMPLE.md.jinja2).
 
 Documentation:
 
 <!---->
 ```py
 def pysnippet(path: str,
               symbol: Optional[str],
               *,
               escape: bool = False,
               indent: Union[str, int, None] = None,
+              indented: Union[str, int, None] = None,
               backtickify: Union[bool, str] = False,
               decomentify: Union[bool, Literal['nl']] = False,
               _ctx: _Context) -> Union[str, markupsafe.Markup]:
   """Return a python snippet, allowing you to specify a class or function.
 
   Args:
       path (str): The path to the file.
       symbol (Optional[str]): The symbol to extract. If None, the entire file is
         returned. Defaults to None.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
       indent (Union[str, int, None], optional): Should indent? By how much, or
         with what prefix? Defaults to None.
+      indented (Union[str, int, None], optional): Indents every line except the
+        first. By how much, or with what prefix? Defaults to None.
       backtickify (Union[bool, str], optional): Should surround with backticks?
         With what language? Defaults to False.
       decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
         HTML comments around this call, setting this to true will add
         correspondingcomments to uncomment the output. This allows you to have
         the Jinja2 call unmolested by markdown formatters, because they will be
         inside of a comment section. "nl" adds additional newlines after the
@@ -409,41 +296,44 @@
 
   Returns:
       Union[str, markupsafe.Markup]: The snippet.
   """
 ```
 <!---->
 
-### pysignature
+### 🐍📖 pysignature
 
 Used several times in [./README.md.jinja2](./README.md.jinja2).
 
 Documentation:
 
 <!---->
 ```py
 def pysignature(path: str,
                 symbol: str,
                 *,
                 escape: bool = False,
                 indent: Union[str, int, None] = None,
+                indented: Union[str, int, None] = None,
                 backtickify: Union[bool, str] = False,
                 decomentify: Union[bool, Literal['nl']] = False,
                 _ctx: _Context) -> str:
   """Return the signature of a class or function in a python file.
 
   Returns the {class,function} signature and the docstring.
 
   Args:
       path (str): The path to the file.
       symbol (str): The symbol to extract.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
       indent (Union[str, int, None], optional): Should indent? By how much, or
         with what prefix? Defaults to None.
+      indented (Union[str, int, None], optional): Indents every line except the
+        first. By how much, or with what prefix? Defaults to None.
       backtickify (Union[bool, str], optional): Should surround with backticks?
         With what language? Defaults to False.
       decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
         HTML comments around this call, setting this to true will add
         correspondingcomments to uncomment the output. This allows you to have
         the Jinja2 call unmolested by markdown formatters, because they will be
         inside of a comment section. "nl" adds additional newlines after the
@@ -453,37 +343,40 @@
 
   Returns:
       str: The signature and docstring.
   """
 ```
 <!---->
 
-### rawsnippet
+### ✂ rawsnippet
 
 Used several times in [./README.md.jinja2](./README.md.jinja2).
 
 Documentation:
 
 <!---->
 ```py
 def rawsnippet(path: str,
                *,
                escape: bool = False,
                indent: Union[str, int, None] = None,
+               indented: Union[str, int, None] = None,
                backtickify: Union[bool, str] = False,
                decomentify: Union[bool, Literal['nl']] = False,
                _ctx: _Context) -> Union[str, markupsafe.Markup]:
   """Return an entire file as a snippet.
 
   Args:
       path (str): The path to the file.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
       indent (Union[str, int, None], optional): Should indent? By how much, or
         with what prefix? Defaults to None.
+      indented (Union[str, int, None], optional): Indents every line except the
+        first. By how much, or with what prefix? Defaults to None.
       backtickify (Union[bool, str], optional): Should surround with backticks?
         With what language? Defaults to False.
       decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
         HTML comments around this call, setting this to true will add
         correspondingcomments to uncomment the output. This allows you to have
         the Jinja2 call unmolested by markdown formatters, because they will be
         inside of a comment section. "nl" adds additional newlines after the
@@ -494,28 +387,29 @@
   Returns:
       Union[str, markupsafe.Markup]: The snippet.
   """
 
 ```
 <!---->
 
-### snippet
+### ✂ snippet
 
 Example in [./snipinator/examples/LONG-EXAMPLE.md.jinja2](./snipinator/examples/LONG-EXAMPLE.md.jinja2).
 
 Documentation:
 
 <!---->
 ```py
 def snippet(path: str,
             start: str,
             end: str,
             *,
             escape: bool = False,
             indent: Union[str, int, None] = None,
+            indented: Union[str, int, None] = None,
             backtickify: Union[bool, str] = False,
             decomentify: Union[bool, Literal['nl']] = False,
             _ctx: _Context) -> Union[str, markupsafe.Markup]:
   """Returns a _delimited_ snippet from a file.
 
   Does not return the delimiters themselves.
 
@@ -523,14 +417,16 @@
       path (str): The path to the file.
       start (str): A string that indicates the start of the snippet.
       end (str): A string that indicates the end of the snippet.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
       indent (Union[str, int, None], optional): Should indent? By how much, or
         with what prefix? Defaults to None.
+      indented (Union[str, int, None], optional): Indents every line except the
+        first. By how much, or with what prefix? Defaults to None.
       backtickify (Union[bool, str], optional): Should surround with backticks?
         With what language? Defaults to False.
       decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
         HTML comments around this call, setting this to true will add
         correspondingcomments to uncomment the output. This allows you to have
         the Jinja2 call unmolested by markdown formatters, because they will be
         inside of a comment section. "nl" adds additional newlines after the
@@ -541,26 +437,27 @@
   Returns:
       Union[str, markupsafe.Markup]: The snippet.
   """
 
 ```
 <!---->
 
-### shell
+### 🐚 shell
 
 Used several times in [./README.md.jinja2](./README.md.jinja2).
 
 Documentation:
 
 <!---->
 ```py
 def shell(args: str,
           *,
           escape: bool = False,
           indent: Union[str, int, None] = None,
+          indented: Union[str, int, None] = None,
           backtickify: Union[bool, str] = False,
           decomentify: Union[bool, Literal['nl']] = False,
           rich: Union[Literal['svg'], Literal['img+b64+svg'], Literal['raw'],
                       str] = 'raw',
           rich_alt: Optional[str] = None,
           rich_bg_color: Optional[str] = None,
           rich_term: Optional[str] = None,
@@ -572,22 +469,34 @@
 
   Use at your own risk, this can potentially introduce security vulnerabilities.
   Only use if you know what you are doing. Ensure that no untrusted input can
   be injected into the `args` parameter, or, into anything the command might
   access. If an adversary can control the `args` parameter, they can execute
   arbitrary commands on your system.
 
+  Note: On persistent output colors:
+
+  * I found that the environment variables TERM, COLORTERM and FORCE_COLOR,
+    CLI_WIDTH, COLUMNS also influence the outputs for some applications.
+  * Also various library versions used in various programs, e.g colorama,
+    rich-argparse, Pygments might influence the output.
+  * I had to pin all my python packages, and explicitly set TERM, COLORTERM and
+    FORCE_COLOR, CLI_WIDTH, COLUMNS to get the output to be consistent across
+    two different systems, both using Ubuntu, for a single program.
+
   Args:
       args (str): The command to run.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
-      indent (Union[str, int, None], optional): Should indent? By how much, or with
-        what prefix? Defaults to None.
-      backtickify (Union[bool, str], optional): Should surround with backticks? With
-        what language? Defaults to False.
+      indent (Union[str, int, None], optional): Should indent? By how much, or
+        with what prefix? Defaults to None.
+      indented (Union[str, int, None], optional): Indents every line except the
+        first. By how much, or with what prefix? Defaults to None.
+      backtickify (Union[bool, str], optional): Should surround with backticks?
+        With what language? Defaults to False.
       decomentify (bool, optional): Assuming that you will be using HTML
         comments around this call, setting this to true will add corresponding
         uncomments to uncomment the output. This allows you to have the Jinja2
         call unmolested by markdown formatters, because they will be inside of
         a comment section. Defaults to False.
       rich (Union[Literal['svg'], Literal['img+b64+svg'], Literal['raw'], str], optional):
         Optionally outputs colored terminal output as an image.
@@ -603,16 +512,16 @@
         * If 'img+svg' a base64 encoded image will be dumped into the markdown
           with the colored terminal output.
         * If 'raw' the raw (uncolored) terminal output will be dumped into the
           markdown directly.
         * Defaults to 'raw.
       rich_alt (Optional[str], optional): The alt text for the img tag. Defaults
         to None.
-      rich_bg_color (Optional[str], optional): The background color for the terminal
-        output. Valid colors include anything valid for SVG colors. See
+      rich_bg_color (Optional[str], optional): The background color for the
+        terminal output. Valid colors include anything valid for SVG colors. See
         <https://developer.mozilla.org/en-US/docs/Web/CSS/color>. Defaults to
         None (fully transparent).
       rich_term: (Optional[str], optional): Sets the TERM env var. Defaults to
         None, which uses whatever the env vars already have.
       rich_rows (int, optional): The number of rows to use for the terminal
         output. Doesn't seem to have much effect. Defaults to 24.
       rich_cols (int, optional): The number of columns to use for the terminal
@@ -624,26 +533,27 @@
 
   Returns:
       Union[str, markupsafe.Markup]: Returns the output of the command.
   """
 ```
 <!---->
 
-### path
+### 🌀 path
 
 Used several times in [./README.md.jinja2](./README.md.jinja2).
 
 Documentation:
 
 <!---->
 ```py
 def path(path: str,
          *,
          escape: bool = False,
          indent: Union[str, int, None] = None,
+         indented: Union[str, int, None] = None,
          backtickify: Union[bool, str] = False,
          decomentify: Union[bool, Literal['nl']] = False,
          link: Optional[Literal['md', 'html']] = None,
          text: Optional[str] = None,
          _ctx: _Context) -> Union[str, markupsafe.Markup]:
   """Verifies that `path` exists, and just returns `path`.
 
@@ -653,14 +563,16 @@
 
   Args:
       path (str): The path to verify.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
       indent (Union[str, int, None], optional): Should indent? By how much, or
         with what prefix? Defaults to None.
+      indented (Union[str, int, None], optional): Indents every line except the
+        first. By how much, or with what prefix? Defaults to None.
       backtickify (Union[bool, str], optional): Should surround with backticks?
         With what language? Defaults to False.
       decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
         HTML comments around this call, setting this to true will add
         correspondingcomments to uncomment the output. This allows you to have
         the Jinja2 call unmolested by markdown formatters, because they will be
         inside of a comment section. "nl" adds additional newlines after the
@@ -676,52 +588,48 @@
   Returns:
       Union[str, markupsafe.Markup]: Just returns the path. If the path doesn't exist,
         it will raise an error.
   """
 ```
 <!---->
 
-Also see Jinja2 v3
-[Template Designer Documentation](https://jinja.palletsprojects.com/en/3.1.x/templates/).
-
 ## ✅ Requirements
 
 - Linux-like environment
   - Why: Uses pexpect.spawn().
 - Python 3.8+
   - Why: Some dev dependencies require Python 3.8+.
 
-### Tested on
+### Tested Platforms
 
-- WSL2 Ubuntu 20.04, Python 3.8.0
-- Ubuntu 20.04, Python 3.8.0, 3.9.0, 3.10.0, 3.11.0, 3.12.0, tested in GitHub
-  Actions workflow
-  ([build-and-test.yml](./.github/workflows/build-and-test.yml)).
+- WSL2 Ubuntu 20.04, Python `3.8.0`.
+- Ubuntu 20.04, Python `3.8.0, 3.9.0, 3.10.0, 3.11.0, 3.12.0`, tested in GitHub Actions
+  workflow ([build-and-test.yml](./.github/workflows/build-and-test.yml)).
 
 ## 🚸 Gotchas and Limitations
 
 - **Security:** This tool is NOT designed to be used with untrusted input. It is
   designed to be used with your own codebase. Even when using your own input, be
   careful that your own code won't be doing anything that might inadvertently
   include untrusted input.
 - Be careful to escape `{{` and `}}`,
   or `{%` and `%}` or anything jinja2
   is sensitive to, in the templates. You'll have to escape it properly for
   jinja2, which involves using `{% raw %}` and
   `{% endraw %}` tags.
-- Recursion: Snipinator doesn't directly support recursive inclusion of
-  generated content. You can generate the contents of one file first, and
-  include that generated content into another template. This would mean that you
-  have to worry about order of generation.
+- Recursion: Snipinator doesn't directly support recursive
+  inclusion of generated content. You can generate the contents of one file
+  first, and include that generated content into another template. This would
+  mean that you have to worry about order of generation.
 - Embedded Backticks: If there are backticks in the included snippet, it might
   ruin the backticks you have in your markdown. This is why `backtickify`
-  parameter exists in the API, so that Snipinator provides the backticks, and it
-  will detect if there are backticks in the snippet and use a different number
-  of backticks on the entire snippet. So if the snippet contains
-  ` ```My Snippet``` `, Snipinator will use
+  parameter exists in the API, so that Snipinator provides the
+  backticks, and it will detect if there are backticks in the snippet and use a
+  different number of backticks on the entire snippet. So if the snippet
+  contains ` ```My Snippet``` `, Snipinator will use
   ` ````language ```My Snippet``` ```` ` and this is a method that Markdown uses
   to allow embedded backticks inside a code block.
 - Formatting: The `{{` `}}` used to
   surround the snippet calls will unfortunately be formatted by a Markdown
   formatter and make the call invalid. Workarounds:
   - **Decommentify**: Put the snippet call inside a HTML comment, then use
     `decommentify` parameter. See
@@ -737,24 +645,25 @@
     be formatted. However, because of **Embedded Backticks** gotcha, (see
     above), this is not recommended, unless you know for sure that there are no
     embedded backticks.
   - If your formatter supports a comment that disabled formatting, you can
     surround the snippet call with that comment.
 - Editing the wrong file: When you have a template and a generated file, it is
   easy to edit the wrong file. To combat this:
-  - Snipinator provides a warning at the top of the generated file to remind you
-    that it is auto-generated.
-  - Snipinator will optionally chmod the file for you to make it read-only.
+  - Snipinator provides a warning at the top of the generated file
+    to remind you that it is auto-generated.
+  - Snipinator will optionally chmod the file for you to make it
+    read-only.
 - Newlines: This program assumes LF newlines. I don't know if it will work for
   anything else.
 - Combining `backtickify` and `indent`: Doesn't make much sense, but if you do
   it, it will run backtickify first, then indent everything including the
   backticks.
 
-## Versioning
+## 🤏 Versioning
 
 We use SemVer for versioning. For the versions available, see the tags on this
 repository.
 
 ## 🔑 License
 
 This project is licensed under the MIT License - see the
@@ -767,74 +676,117 @@
 - Templating: [Jinja2](https://github.com/pallets/jinja).
 - Snippet inclusion: Python's AST library.
 - Colorful CLI help: [rich-argparse](https://github.com/hamdanal/rich-argparse).
 - ANSI coloring shell output:
   {[pexpect](https://pexpect.readthedocs.io/en/stable/),
   [rich](https://github.com/Textualize/rich)}.
 
-## Related Projects
+## 🤝 Related Projects
+
+Not complete, and not necessarily up to date. Make a PR
+([contributions](#-contributions)) to insert/modify.
 
-- [markdown-code-example-inserter](https://github.com/electrovir/markdown-code-example-inserter)
-  "Syncs code examples with markdown documentation."
-- [ARMmbed/snippet](https://github.com/ARMmbed/snippet) "A Python3 tool to
-  extract code snippets from source files".
-- [SimonCropp/MarkdownSnippets](https://github.com/SimonCropp/MarkdownSnippets)
-  "Extracts snippets from code files and merges them into markdown documents".
-- [shiftkey/scribble](https://github.com/shiftkey/scribble) "Making
-  documentation for .NET projects easy and fun".
+| Project                                                           | Stars     | Last Update  | Language   | Platform         | Similarity X Obviousness |
+| ----------------------------------------------------------------- | --------- | ------------ | ---------- | ---------------- | ------------------------ |
+| [mdx-js/mdx][54]                                                  | 16.8k     | `2024/04/17` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
+| [zakhenry/embedme][24]                                            | 222       | `2023/11/08` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
+| [cmacmackin/markdown-include][53]                                 | 95        | `2023/02/07` | Python     | N/A              | ⭐⭐⭐⭐⭐               |
+| [SimonCropp/MarkdownSnippets][31]                                 | 23        | `2024/04/23` | .NET       | N/A              | ⭐⭐⭐⭐⭐               |
+| [endocode/snippetextractor][41]                                   | 4         | `2014/08/16` | C++        | N/A              | ⭐⭐⭐⭐⭐               |
+| [polywrap/doc-snippets][45]                                       | 3         | `2023/09/26` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
+| [JulianCataldo/remark-embed][34]                                  | 2         | `2022/09/22` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
+| [xrd/oreilly-snippets][47]                                        | 2         | `2015/10/15` | Ruby       | N/A              | ⭐⭐⭐⭐⭐               |
+| [DamonOehlman/injectcode][48]                                     | 1         | `2021/08/01` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
+| [electrovir/markdown-code-example-inserter][25]                   | 1         | `2024/02/19` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
+| [andersfischernielsen/Simple-Embedded-Markdown-Code-Snippets][46] | 1         | `2021/02/12` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
+| [ildar-shaimordanov/git-markdown-snippet][36]                     | 0         | `2021/09/14` | Perl       | N/A              | ⭐⭐⭐⭐⭐               |
+| [teyc/markdown-snippet][50]                                       | 0         | `2024/01/22` | Powershell | N/A              | ⭐⭐⭐⭐⭐               |
+| [marc-bouvier-graveyard/baldir_markdown][51]                      | 0         | `2020/06/15` | Python     | N/A              | ⭐⭐⭐⭐⭐               |
+| [dineshsonachalam/markdown-autodocs][26]                          | 176       | `2022/09/19` | JS         | GH Action        | ⭐⭐⭐⭐                 |
+| [tokusumi/markdown-embed-code][29]                                | 28        | `2022/01/05` | Python     | VSCode Extension | ⭐⭐⭐⭐                 |
+| [sammndhr/gridsome-remark-embed-snippet][37]                      | 2         | `2021/06/14` | JS         | [Gridsome][38]   | ⭐⭐⭐⭐                 |
+| [NativeScript/markdown-snippet-injector][44]                      | 4         | `2019/01/24` | JS         | N/A              | ⭐⭐⭐⭐                 |
+| [fuxingloh/remark-code-import-replace][49]                        | 0         | `2022/12/21` | JS         | Remark?          | ⭐⭐⭐⭐                 |
+| [szkiba/mdcode][55]                                               | 15        | `2014/02/12` | Go         | N/A              | ⭐⭐⭐                   |
+| [devincornell/pymddoc][43]                                        | 0         | `2023/12/01` | Python     | Python           | ⭐⭐⭐                   |
+| [shiftkey/scribble][32] ([docs][33])                              | 40        | `2013/08/08` | .NET       | N/A              | ⭐⭐                     |
+| [calebpeterson/jest-transformer-test-md][35]                      | 2         | `2020/08/21` | JS         | Jest Tests       | ⭐⭐                     |
+| [tjstankus/commitate][52]                                         | 0         | `2014/05/29` | Ruby       | N/A              | ⭐                       |
+| [GitHub Docs: Creating a permanent link to a code snippet][23]    | N/A       | N/A          | N/A        | N/A              | ⭐                       |
+| [javierfernandes/markdown-exercises][42]                          | 1         | `2017/05/01` | JS         | N/A              | ⭐                       |
+| [gatsby-remark-embed-snippet][39]                                 | N/A (55k) | `2024/01/23` | JS         | [Gatsby][40]     | ⭐                       |
+| [ARMmbed/snippet][30]                                             | 6         | `2021/08/05` | Python     | N/A              | ?                        |
+| [drewavis/markdowninclude][28]                                    | 1         | `2024/04/06` | JS         | VSCode Extension | ?                        |
+| [romnn/embedme][27]                                               | 0         | `2024/04/18` | Go         | N/A              | ?                        |
 
 ## 🫡 Contributions
 
 ### Development environment: Linux-like
 
 - For running `pre.sh` (Linux-like environment).
+
+  - From [./.github/dependencies.yml](./.github/dependencies.yml), which is used for
+    the GH Action to do a fresh install of everything:
+
+    ```yaml
+    bash: scripts.
+    findutils: scripts.
+    grep: tests.
+    xxd: tests.
+    git: scripts, tests.
+    xxhash: scripts (changeguard).
+    rsync: out-of-directory test.
+    expect: for `unbuffer`, useful to grab and compare ansi color symbols.
+    jq: dependency for [yq](https://github.com/kislyuk/yq), which is used to generate
+      the README; the README generator needs to use `tomlq` (which is a part of `yq`)
+      to query `pyproject.toml`.
+    
+    ```
+
   - Requires `pyenv`, or an exact matching version of python as in
-    `.python-version` (which is currently
-    `3.8.0
-`).
-  - `jq`, ([installation](https://jqlang.github.io/jq/)) required for
-    [yq](https://github.com/kislyuk/yq), which is itself required for our
-    `./README.md` generation, which uses `tomlq` (from the
-    [yq](https://github.com/kislyuk/yq) package) to include version strings from
-    `./pyproject.toml`.
-  - `bash`, `grep`, `awk`, `sed` `xxd`, `git`, `xxhash` (for tests/workflows).
-  - Requires nodejs (for act).
-  - Requires Go (to run act).
-  - docker (for act).
+    [.python-version](.python-version) (which is currently
+    `3.8.0`).
+  - act (to run the GH Action locally):
+    - Requires nodejs.
+    - Requires Go.
+    - docker.
+  - Generate animation:
+    - docker
 
 ### Commit Process
 
 1. (Optionally) Fork the `develop` branch.
 2. Stage your files: `git add path/to/file.py`.
-3. `bash scripts/pre.sh`, this will format, lint, and test the code.
-4. `git status` check if anything changed (generated `./README.md`
-   for example), if so, `git add` the changes, and go back to the previous step.
+3. `bash ./scripts/pre.sh`, this will format, lint, and test the code.
+4. `git status` check if anything changed (generated
+   [./README.md](./README.md) for example), if so, `git add` the
+   changes, and go back to the previous step.
 5. `git commit -m "..."`.
 6. Make a PR to `develop` (or push to develop if you have the rights).
 
-## ⛙ Release Process
+## 🔄🚀 Release Process
 
 These instructions are for maintainers of the project.
 
 1. In the `develop` branch, run `bash ./scripts/pre.sh` to ensure
    everything is in order.
-2. In the `develop` branch, bump the version in `./pyproject.toml`,
-   following semantic versioning principles. Also modify the
-   `last_unstable_release` and `last_stable_release` in the
-   `[tool.changeguard-project-metadata]` table as appropriate. Run
-   `bash scripts/pre.sh` to ensure everything is in order.
+2. In the `develop` branch, bump the version in
+   [./pyproject.toml](./pyproject.toml), following semantic versioning
+   principles. Also modify the `last_unstable_release` and `last_stable_release`
+   in the `[tool.snipinator-project-metadata]` table as appropriate. Run
+   `bash ./scripts/pre.sh` to ensure everything is in order.
 3. In the `develop` branch, commit these changes with a message like
    `"Prepare release X.Y.Z"`. (See the contributions section
    [above](#commit-process)).
 4. Merge the `develop` branch into the `master` branch:
    `git checkout master && git merge develop --no-ff`.
 5. `master` branch: Tag the release: Create a git tag for the release with
    `git tag -a vX.Y.Z -m "Version X.Y.Z"`.
 6. Publish to PyPI: Publish the release to PyPI with
-   `bash scripts/deploy-to-pypi.sh`.
+   `bash ./scripts/deploy-to-pypi.sh`.
 7. Push to GitHub: Push the commit and tags to GitHub with
    `git push && git push --tags`.
 8. The `--no-ff` option adds a commit to the master branch for the merge, so
    refork the develop branch from the master branch:
    `git checkout develop && git merge master`.
 9. Push the develop branch to GitHub: `git push origin develop`.
 
@@ -844,42 +796,82 @@
   https://github.com/realazthat/snipinator/actions/workflows/build-and-test.yml
 [3]:
   https://img.shields.io/github/license/realazthat/snipinator?style=plastic&color=0A1E1E
 [4]:
   https://img.shields.io/pypi/v/snipinator?style=plastic&color=0A1E1E
 [5]: https://pypi.org/project/snipinator/
 [6]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.3.1/master?style=plastic
+  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.4.0/master?style=plastic
 [7]:
   https://img.shields.io/github/last-commit/realazthat/snipinator/master?style=plastic
 [8]:
   https://img.shields.io/pypi/pyversions/snipinator?style=plastic&color=0A1E1E
 [9]:
   https://img.shields.io/github/languages/top/realazthat/snipinator.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E
 [10]:
-  https://github.com/realazthat/snipinator/compare/v1.3.1...master
+  https://github.com/realazthat/snipinator/compare/v1.4.0...master
 [11]:
   https://img.shields.io/github/actions/workflow/status/realazthat/snipinator/build-and-test.yml?branch=develop&style=plastic
 [12]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.3.1/develop?style=plastic
+  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.4.0/develop?style=plastic
 [13]:
-  https://github.com/realazthat/snipinator/compare/v1.3.1...develop
+  https://github.com/realazthat/snipinator/compare/v1.4.0...develop
 [14]:
   https://img.shields.io/github/last-commit/realazthat/snipinator/develop?style=plastic
 [15]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.3.1/develop?style=plastic
+  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.4.0/develop?style=plastic
 [16]:
-  https://github.com/realazthat/snipinator/compare/v1.3.1...develop
+  https://github.com/realazthat/snipinator/compare/v1.4.0...develop
 [17]: https://github.com/realazthat/snipinator/tree/master
 [18]: https://github.com/realazthat/snipinator/tree/develop
 
 <!-- Logo from https://lucide.dev/icons/users -->
 
 [19]:
   https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
 
 <!-- Logo from https://lucide.dev/icons/laptop-minimal -->
 
 [20]:
   https://img.shields.io/badge/Platform-Linux-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
 [21]: ./LICENSE.md
 [22]: ./.github/logo-exported.svg
+[23]:
+  https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-a-permanent-link-to-a-code-snippet
+[24]: https://github.com/zakhenry/embedme
+[25]: https://github.com/electrovir/markdown-code-example-inserter
+[26]: https://github.com/dineshsonachalam/markdown-autodocs
+[27]: https://github.com/romnn/embedme
+[28]: https://github.com/drewavis/markdowninclude
+[29]: https://github.com/tokusumi/markdown-embed-code
+[30]: https://github.com/ARMmbed/snippet
+[31]: https://github.com/SimonCropp/MarkdownSnippets
+[32]: https://github.com/shiftkey/scribble
+[33]:
+  https://github.com/shiftkey/scribble/blob/master/docs/features/code-snippets.md
+[34]: https://github.com/JulianCataldo/remark-embed
+[35]: https://github.com/calebpeterson/jest-transformer-test-md
+[36]: https://github.com/ildar-shaimordanov/git-markdown-snippet
+[37]: https://github.com/sammndhr/gridsome-remark-embed-snippet
+[38]: https://gridsome.org/
+[39]:
+  https://github.com/gatsbyjs/gatsby/tree/master/packages/gatsby-remark-embed-snippet
+[40]: https://github.com/gatsbyjs/gatsby
+[41]: https://github.com/endocode/snippetextractor
+[42]: https://github.com/javierfernandes/markdown-exercises
+[43]: https://github.com/devincornell/pymddoc
+[44]: https://github.com/NativeScript/markdown-snippet-injector
+[45]: https://github.com/polywrap/doc-snippets
+[46]:
+  https://github.com/andersfischernielsen/Simple-Embedded-Markdown-Code-Snippets
+[47]: https://github.com/xrd/oreilly-snippets
+[48]: https://github.com/DamonOehlman/injectcode
+[49]: https://github.com/fuxingloh/remark-code-import-replace
+[50]: https://github.com/teyc/markdown-snippet
+[51]: https://github.com/marc-bouvier-graveyard/baldir_markdown
+[52]: https://github.com/tjstankus/commitate
+[53]: https://github.com/cmacmackin/markdown-include
+[54]: https://github.com/mdx-js/mdx
+[55]:
+  https://github.com/szkiba/mdcode
+  "Extracts code blocks from README and produces tests; a similar approach, but quite different"
+[56]: https://github.com/realazthat/snipinator
```

### Comparing `snipinator-1.3.1/pyproject.toml` & `snipinator-1.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "snipinator"
-version = "1.3.1"
+version = "1.4.0"
 description = "Python code snippets for markdown files, e.g READMEs, from actual (testable) code."
 authors = [{name = "AYF", email = "realazthat@gmail.com"}]
 license = {file = "LICENSE.md"}
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Operating System :: OS Independent",
@@ -159,11 +159,11 @@
 Documentation = "https://github.com/realazthat/snipinator"
 Repository = "https://github.com/realazthat/snipinator"
 
 [tool.setuptools]
 packages = ["snipinator"]
 
 [tool.snipinator-project-metadata]
-last_unstable_release = "1.3.1"
-last_stable_release = "1.3.1"
+last_unstable_release = "1.4.0"
+last_stable_release = "1.4.0"
 
 [tool.tomlsort]
```

### Comparing `snipinator-1.3.1/snipinator/__init__.py` & `snipinator-1.4.0/snipinator/__init__.py`

 * *Files identical despite different names*

### Comparing `snipinator-1.3.1/snipinator/cli.py` & `snipinator-1.4.0/snipinator/cli.py`

 * *Files identical despite different names*

### Comparing `snipinator-1.3.1/snipinator/snipinate copy.py` & `snipinator-1.4.0/snipinator/snipinate.py`

 * *Files 8% similar despite different names*

```diff
@@ -118,28 +118,31 @@
 
 
 def pysignature(path: str,
                 symbol: str,
                 *,
                 escape: bool = False,
                 indent: Union[str, int, None] = None,
+                indented: Union[str, int, None] = None,
                 backtickify: Union[bool, str] = False,
                 decomentify: Union[bool, Literal['nl']] = False,
                 _ctx: _Context) -> str:
   """Return the signature of a class or function in a python file.
 
   Returns the {class,function} signature and the docstring.
 
   Args:
       path (str): The path to the file.
       symbol (str): The symbol to extract.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
       indent (Union[str, int, None], optional): Should indent? By how much, or
         with what prefix? Defaults to None.
+      indented (Union[str, int, None], optional): Indents every line except the
+        first. By how much, or with what prefix? Defaults to None.
       backtickify (Union[bool, str], optional): Should surround with backticks?
         With what language? Defaults to False.
       decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
         HTML comments around this call, setting this to true will add
         correspondingcomments to uncomment the output. This allows you to have
         the Jinja2 call unmolested by markdown formatters, because they will be
         inside of a comment section. "nl" adds additional newlines after the
@@ -152,39 +155,43 @@
   """
   path_ = _CheckPath(path=path, cwd=_ctx.cwd)
   source = path_.read_text()
   signature = _GetSymbolSignature(source=source, path=str(path_), symbol=symbol)
 
   signature = _Backtickify(signature, backtickify=backtickify)
   signature = _Indent(signature, indent=indent)
+  signature = _Indented(signature, indented=indented)
   signature = _Decomentify(signature, decomentify=decomentify)
   if not escape:
     return markupsafe.Markup(signature)
   else:
     return signature
 
 
 def pysnippet(path: str,
               symbol: Optional[str],
               *,
               escape: bool = False,
               indent: Union[str, int, None] = None,
+              indented: Union[str, int, None] = None,
               backtickify: Union[bool, str] = False,
               decomentify: Union[bool, Literal['nl']] = False,
               _ctx: _Context) -> Union[str, markupsafe.Markup]:
   """Return a python snippet, allowing you to specify a class or function.
 
   Args:
       path (str): The path to the file.
       symbol (Optional[str]): The symbol to extract. If None, the entire file is
         returned. Defaults to None.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
       indent (Union[str, int, None], optional): Should indent? By how much, or
         with what prefix? Defaults to None.
+      indented (Union[str, int, None], optional): Indents every line except the
+        first. By how much, or with what prefix? Defaults to None.
       backtickify (Union[bool, str], optional): Should surround with backticks?
         With what language? Defaults to False.
       decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
         HTML comments around this call, setting this to true will add
         correspondingcomments to uncomment the output. This allows you to have
         the Jinja2 call unmolested by markdown formatters, because they will be
         inside of a comment section. "nl" adds additional newlines after the
@@ -200,36 +207,40 @@
   if symbol is None:
     snippet = path_.read_text()
   else:
     snippet = _GetSymbolSource(path=path_, symbol=symbol)
 
   snippet = _Backtickify(snippet, backtickify=backtickify)
   snippet = _Indent(snippet, indent=indent)
+  snippet = _Indented(snippet, indented=indented)
   snippet = _Decomentify(snippet, decomentify=decomentify)
   if not escape:
     return markupsafe.Markup(snippet)
   else:
     return snippet
 
 
 def rawsnippet(path: str,
                *,
                escape: bool = False,
                indent: Union[str, int, None] = None,
+               indented: Union[str, int, None] = None,
                backtickify: Union[bool, str] = False,
                decomentify: Union[bool, Literal['nl']] = False,
                _ctx: _Context) -> Union[str, markupsafe.Markup]:
   """Return an entire file as a snippet.
 
   Args:
       path (str): The path to the file.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
       indent (Union[str, int, None], optional): Should indent? By how much, or
         with what prefix? Defaults to None.
+      indented (Union[str, int, None], optional): Indents every line except the
+        first. By how much, or with what prefix? Defaults to None.
       backtickify (Union[bool, str], optional): Should surround with backticks?
         With what language? Defaults to False.
       decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
         HTML comments around this call, setting this to true will add
         correspondingcomments to uncomment the output. This allows you to have
         the Jinja2 call unmolested by markdown formatters, because they will be
         inside of a comment section. "nl" adds additional newlines after the
@@ -241,27 +252,29 @@
       Union[str, markupsafe.Markup]: The snippet.
   """
 
   path_ = _CheckPath(path=path, cwd=_ctx.cwd)
   snippet = path_.read_text()
   snippet = _Backtickify(snippet, backtickify=backtickify)
   snippet = _Indent(snippet, indent=indent)
+  snippet = _Indented(snippet, indented=indented)
   snippet = _Decomentify(snippet, decomentify=decomentify)
   if not escape:
     return markupsafe.Markup(snippet)
   else:
     return snippet
 
 
 def snippet(path: str,
             start: str,
             end: str,
             *,
             escape: bool = False,
             indent: Union[str, int, None] = None,
+            indented: Union[str, int, None] = None,
             backtickify: Union[bool, str] = False,
             decomentify: Union[bool, Literal['nl']] = False,
             _ctx: _Context) -> Union[str, markupsafe.Markup]:
   """Returns a _delimited_ snippet from a file.
 
   Does not return the delimiters themselves.
 
@@ -269,14 +282,16 @@
       path (str): The path to the file.
       start (str): A string that indicates the start of the snippet.
       end (str): A string that indicates the end of the snippet.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
       indent (Union[str, int, None], optional): Should indent? By how much, or
         with what prefix? Defaults to None.
+      indented (Union[str, int, None], optional): Indents every line except the
+        first. By how much, or with what prefix? Defaults to None.
       backtickify (Union[bool, str], optional): Should surround with backticks?
         With what language? Defaults to False.
       decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
         HTML comments around this call, setting this to true will add
         correspondingcomments to uncomment the output. This allows you to have
         the Jinja2 call unmolested by markdown formatters, because they will be
         inside of a comment section. "nl" adds additional newlines after the
@@ -301,25 +316,27 @@
     raise ValueError(
         f'Searched for {json.dumps(end)} in {json.dumps(str(path))} but not found'
     )
   snippet_start += len(start)
   snippet = full_source[snippet_start:snippet_end]
   snippet = _Backtickify(snippet, backtickify=backtickify)
   snippet = _Indent(snippet, indent=indent)
+  snippet = _Indented(snippet, indented=indented)
   snippet = _Decomentify(snippet, decomentify=decomentify)
   if not escape:
     return markupsafe.Markup(snippet)
   else:
     return snippet
 
 
 def path(path: str,
          *,
          escape: bool = False,
          indent: Union[str, int, None] = None,
+         indented: Union[str, int, None] = None,
          backtickify: Union[bool, str] = False,
          decomentify: Union[bool, Literal['nl']] = False,
          link: Optional[Literal['md', 'html']] = None,
          text: Optional[str] = None,
          _ctx: _Context) -> Union[str, markupsafe.Markup]:
   """Verifies that `path` exists, and just returns `path`.
 
@@ -329,14 +346,16 @@
 
   Args:
       path (str): The path to verify.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
       indent (Union[str, int, None], optional): Should indent? By how much, or
         with what prefix? Defaults to None.
+      indented (Union[str, int, None], optional): Indents every line except the
+        first. By how much, or with what prefix? Defaults to None.
       backtickify (Union[bool, str], optional): Should surround with backticks?
         With what language? Defaults to False.
       decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
         HTML comments around this call, setting this to true will add
         correspondingcomments to uncomment the output. This allows you to have
         the Jinja2 call unmolested by markdown formatters, because they will be
         inside of a comment section. "nl" adds additional newlines after the
@@ -354,26 +373,29 @@
         it will raise an error.
   """
   _CheckPath(path=path, cwd=_ctx.cwd)
 
   if not Path(path).exists():
     raise FileNotFoundError(f'File not found: {json.dumps(path)}')
 
-  if text is None:
-    text = path
-  output: str = text
+  text_str: str = path if text is None else text
+  output: str = text_str
 
   if link == 'md':
-    output = f'[{text}]({path})'
+    # TODO: escape text_str for markdown?
+    # TODO: urllib.quote() the URL?
+    output = f'[{html.escape(text_str, quote=True)}]({html.escape(path, quote=True)})'
   elif link == 'html':
-    output = f'<a href="{text}">{path}</a>'
+    # TODO: urllib.quote() the URL?
+    output = f'<a href="{html.escape(path, quote=True)}">{html.escape(text_str, quote=True)}</a>'
   elif link is None:
-    output = text
+    output = text_str
   output = _Backtickify(output, backtickify=backtickify)
   output = _Indent(output, indent=indent)
+  output = _Indented(output, indented=indented)
   output = _Decomentify(output, decomentify=decomentify)
   if not escape:
     return markupsafe.Markup(output)
   else:
     return output
 
 
@@ -483,14 +505,15 @@
   return svg
 
 
 def shell(args: str,
           *,
           escape: bool = False,
           indent: Union[str, int, None] = None,
+          indented: Union[str, int, None] = None,
           backtickify: Union[bool, str] = False,
           decomentify: Union[bool, Literal['nl']] = False,
           rich: Union[Literal['svg'], Literal['img+b64+svg'], Literal['raw'],
                       str] = 'raw',
           rich_alt: Optional[str] = None,
           rich_bg_color: Optional[str] = None,
           rich_term: Optional[str] = None,
@@ -504,30 +527,32 @@
   Only use if you know what you are doing. Ensure that no untrusted input can
   be injected into the `args` parameter, or, into anything the command might
   access. If an adversary can control the `args` parameter, they can execute
   arbitrary commands on your system.
 
   Note: On persistent output colors:
 
-  * I found that the environment variables TERM and COLORTERM, and FORCE_COLOR
-    also influence the output colors for some applications.
-  * I don't know for sure, but the system, environment variables, version of
-    colorama, rich-argparse, Pygments might influence the output colors.
+  * I found that the environment variables TERM, COLORTERM and FORCE_COLOR,
+    CLI_WIDTH, COLUMNS also influence the outputs for some applications.
+  * Also various library versions used in various programs, e.g colorama,
+    rich-argparse, Pygments might influence the output.
   * I had to pin all my python packages, and explicitly set TERM, COLORTERM and
-    FORCE_COLOR to get the colors to be consistent across two different systems,
-    both using Ubuntu.
+    FORCE_COLOR, CLI_WIDTH, COLUMNS to get the output to be consistent across
+    two different systems, both using Ubuntu, for a single program.
 
   Args:
       args (str): The command to run.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
-      indent (Union[str, int, None], optional): Should indent? By how much, or with
-        what prefix? Defaults to None.
-      backtickify (Union[bool, str], optional): Should surround with backticks? With
-        what language? Defaults to False.
+      indent (Union[str, int, None], optional): Should indent? By how much, or
+        with what prefix? Defaults to None.
+      indented (Union[str, int, None], optional): Indents every line except the
+        first. By how much, or with what prefix? Defaults to None.
+      backtickify (Union[bool, str], optional): Should surround with backticks?
+        With what language? Defaults to False.
       decomentify (bool, optional): Assuming that you will be using HTML
         comments around this call, setting this to true will add corresponding
         uncomments to uncomment the output. This allows you to have the Jinja2
         call unmolested by markdown formatters, because they will be inside of
         a comment section. Defaults to False.
       rich (Union[Literal['svg'], Literal['img+b64+svg'], Literal['raw'], str], optional):
         Optionally outputs colored terminal output as an image.
@@ -543,16 +568,16 @@
         * If 'img+svg' a base64 encoded image will be dumped into the markdown
           with the colored terminal output.
         * If 'raw' the raw (uncolored) terminal output will be dumped into the
           markdown directly.
         * Defaults to 'raw.
       rich_alt (Optional[str], optional): The alt text for the img tag. Defaults
         to None.
-      rich_bg_color (Optional[str], optional): The background color for the terminal
-        output. Valid colors include anything valid for SVG colors. See
+      rich_bg_color (Optional[str], optional): The background color for the
+        terminal output. Valid colors include anything valid for SVG colors. See
         <https://developer.mozilla.org/en-US/docs/Web/CSS/color>. Defaults to
         None (fully transparent).
       rich_term: (Optional[str], optional): Sets the TERM env var. Defaults to
         None, which uses whatever the env vars already have.
       rich_rows (int, optional): The number of rows to use for the terminal
         output. Doesn't seem to have much effect. Defaults to 24.
       rich_cols (int, optional): The number of columns to use for the terminal
@@ -645,14 +670,15 @@
   else:
     raise ValueError(
         f'Unsupported rich format: {json.dumps(rich)}, it should be "raw",'
         ' "svg", or "img+svg", or a file path ending with ".svg"')
 
   output = _Backtickify(output, backtickify=backtickify)
   output = _Indent(output, indent=indent)
+  output = _Indented(output, indented=indented)
   output = _Decomentify(output, decomentify=decomentify)
   if not escape:
     return markupsafe.Markup(output)
   else:
     return output
 
 
@@ -831,14 +857,22 @@
     return textwrap.indent(text, ' ' * indent)
   elif isinstance(indent, str):
     return textwrap.indent(text, indent)
   else:
     return text
 
 
+def _Indented(text: str, *, indented: Union[str, int, None]) -> str:
+  if indented is None:
+    return text
+  indent_str = ' ' * indented if isinstance(indented, int) else indented
+  lines = text.splitlines()
+  return '\n'.join([lines[0]] + [indent_str + line for line in lines[1:]])
+
+
 def _CountSequentialBackticks(text: str) -> int:
   """Find the largest number of sequential backticks in the text."""
   for backticks in range(1, len(text)):
     search = '`' * backticks
     if search not in text:
       return backticks - 1
   return 0
```

### Comparing `snipinator-1.3.1/snipinator/snipinate_test.py` & `snipinator-1.4.0/snipinator/snipinate_test.py`

 * *Files identical despite different names*

### Comparing `snipinator-1.3.1/snipinator.egg-info/PKG-INFO` & `snipinator-1.4.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,33 @@
 Metadata-Version: 2.1
 Name: snipinator
-Version: 1.3.1
+Version: 1.4.0
 Summary: Python code snippets for markdown files, e.g READMEs, from actual (testable) code.
 Author-email: AYF <realazthat@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Azriel Fasten.
         
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+        Permission is hereby granted, free of charge, to any person obtaining a copy of
+        this software and associated documentation files (the "Software"), to deal in
+        the Software without restriction, including without limitation the rights to
+        use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+        the Software, and to permit persons to whom the Software is furnished to do so,
+        subject to the following conditions:
         
-        The above copyright notice and this permission notice (including the next paragraph) shall be included in all copies or substantial portions of the Software.
+        The above copyright notice and this permission notice (including the next
+        paragraph) shall be included in all copies or substantial portions of the
+        Software.
         
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+        FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+        COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+        IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+        CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
 Project-URL: Homepage, https://github.com/realazthat/snipinator
 Project-URL: Documentation, https://github.com/realazthat/snipinator
 Project-URL: Repository, https://github.com/realazthat/snipinator
 Keywords: github,testing,markdown,readme,snippets,documentation,jinja2,templates,preprocessor,documentation-tool,include,readme-template,readme-md,dynamic-documentation
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
@@ -136,36 +148,51 @@
 
 -->
 <!--
 
 
 
 
+
+
+
 -->
 
-# <div align="center">![Snipinator][22]</div>
+# <div align="center">[![Snipinator][22]][56]</div>
 
 <div align="center">
 
 <!-- Icons from https://lucide.dev/icons/users -->
 <!-- Icons from https://lucide.dev/icons/laptop-minimal -->
 
 ![**Audience:** Developers][19] ![**Platform:** Linux][20]
 
 </div>
 
 <p align="center">
   <strong>
-    <a href="#-features">🎇Features</a> &nbsp;&bull;&nbsp;
-    <a href="#-installation">🛠️Installation</a> &nbsp;&bull;&nbsp;
-    <a href="#-usage">🔧Usage</a> &nbsp;&bull;&nbsp;
-    <a href="#-command-line-options">💻CLI</a> &nbsp;&bull;&nbsp;
-    <a href="#-examples">💡Examples</a> &nbsp;&bull;&nbsp;
-    <a href="#-api">🤖API</a> &nbsp;&bull;&nbsp;
-    <a href="#-requirements">✅Requirements</a> &nbsp;&bull;&nbsp;
+    <a href="https://github.com/realazthat/snipinator">🏠Home</a>
+    &nbsp;&bull;&nbsp;
+    <a href="#-features">🎇Features</a>
+    &nbsp;&bull;&nbsp;
+    <a href="#-installation">🔨Installation</a>
+    &nbsp;&bull;&nbsp;
+    <a href="#-usage">🚜Usage</a>
+    &nbsp;&bull;&nbsp;
+    <a href="#-command-line-options">💻CLI</a>
+    &nbsp;&bull;&nbsp;
+    <a href="#-examples">💡Examples</a>
+  </strong>
+</p>
+<p align="center">
+  <strong>
+    <a href="#-jinja2-api">🤖Jinja2 API</a>
+    &nbsp;&bull;&nbsp;
+    <a href="#-requirements">✅Requirements</a>
+    &nbsp;&bull;&nbsp;
     <a href="#-gotchas-and-limitations">🚸Gotchas</a>
   </strong>
 </p>
 
 <div align="center">
 
 ![Top language][9] [![GitHub License][3]][21] [![PyPI - Version][4]][5]
@@ -186,16 +213,16 @@
 
 </div>
 
 <img src=".github/demo.gif" alt="Demo" width="100%">
 
 ## ❔ What
 
-What it does: **Snipinator** lets you take a `EXAMPLE.md` template and include
-snippets from your (working and tested) codebase.
+What it does: **Snipinator** lets you take a `EXAMPLE.md` template
+and include snippets from your (working and tested) codebase.
 
 Turn this ([./snipinator/examples/EXAMPLE.md.jinja2](./snipinator/examples/EXAMPLE.md.jinja2)):
 
 <!---->
 ```md
 # A README
 
@@ -256,25 +283,25 @@
 - 🥇🔖📜 First-class support for **Markdown** templates (with `backtickify`,
   `decomentify`).
 - 📦🐚🖨️ Can include **[shell](#shell) output**.
   - Supports ANSI colors :heart: :green_heart: :blue_heart: with SVG output
     :camera:.
 - ⚙️🔗🗃️ More robust **references/links** to local files using [path()](#path).
 
-## 🛠️ Installation
+## 🔨 Installation
 
 ```bash
 # Install from pypi (https://pypi.org/project/snipinator/)
 pip install snipinator
 
 # Install from git (https://github.com/realazthat/snipinator)
-pip install git+https://github.com/realazthat/snipinator.git@v1.3.1
+pip install git+https://github.com/realazthat/snipinator.git@v1.4.0
 ```
 
-## 🔧 Usage
+## 🚜 Usage
 
 Example template README:
 ([./snipinator/examples/EXAMPLE.md.jinja2](./snipinator/examples/EXAMPLE.md.jinja2)):
 
 <!---->
 ```md
 # A README
@@ -345,61 +372,64 @@
   - Template:
     [./snipinator/examples/LONG-EXAMPLE.md.jinja2](./snipinator/examples/LONG-EXAMPLE.md.jinja2).
   - Generated:
     [./snipinator/examples/LONG-EXAMPLE.generated.md](./snipinator/examples/LONG-EXAMPLE.generated.md).
   - Generation script:
     [./snipinator/examples/long-example.sh](./snipinator/examples/long-example.sh).
 - Projects using Snipinator:
-  - [github.com/realazthat/snipinator](https://github.com/realazthat/snipinator),
-    See
+  - [realazthat/snipinator](https://github.com/realazthat/snipinator), See
     [snipinator/README.md.jinja2](https://github.com/realazthat/snipinator/blob/61cb88593baa099dc375cf5fd40679e4be673fc5/README.md.jinja2).
-  - [github.com/realazthat/changeguard](https://github.com/realazthat/changeguard),
-    See
+  - [realazthat/changeguard](https://github.com/realazthat/changeguard), See
     [changeguard/README.md.jinja2](https://github.com/realazthat/changeguard/blob/87d5104b52e651bb9195a3d46dd7f050acbcb534/README.md.jinja2).
-  - [github.com/realazthat/comfy-catapult](https://github.com/realazthat/comfy-catapult),
+  - [realazthat/comfy-catapult](https://github.com/realazthat/comfy-catapult),
     See
     [comfy-catapult/README.md.jinja2](https://github.com/realazthat/comfy-catapult/blob/ff353d48b25fa7b9c35fa11b31d5f2b3039c41c8/README.md.jinja2).
-  - [github.com/realazthat/comfylowda](https://github.com/realazthat/comfylowda),
-    See
+  - [realazthat/comfylowda](https://github.com/realazthat/comfylowda), See
     [comfylowda/README.md.jinja2](https://github.com/realazthat/comfylowda/blob/e01a32c38107aa0b89ccea21c4678d193a186a78/README.md.jinja2).
-  - [github.com/realazthat/excalidraw-brute-export-cli](https://github.com/realazthat/excalidraw-brute-export-cli),
+  - [realazthat/excalidraw-brute-export-cli](https://github.com/realazthat/excalidraw-brute-export-cli),
     See
     [excalidraw-brute-export-cli/README.md.jinja2](https://github.com/realazthat/excalidraw-brute-export-cli/blob/54a3b5b08b644e61c721ab565c576094234c5cc7/README.md.jinja2).
 
-## 🤖 API
+## 🤖 Jinja2 API
+
+The regular Jinja2 v3 template syntax is supported. For more information, see
+[Template Designer Documentation](https://jinja.palletsprojects.com/en/3.1.x/templates/).
 
-(Jinja2) Functions made available:
+Additional (Jinja2) functions made available:
 
-### pysnippet
+### 🐍✂ pysnippet
 
 Used several times in
 [./snipinator/examples/LONG-EXAMPLE.md.jinja2](./snipinator/examples/LONG-EXAMPLE.md.jinja2).
 
 Documentation:
 
 <!---->
 ```py
 def pysnippet(path: str,
               symbol: Optional[str],
               *,
               escape: bool = False,
               indent: Union[str, int, None] = None,
+              indented: Union[str, int, None] = None,
               backtickify: Union[bool, str] = False,
               decomentify: Union[bool, Literal['nl']] = False,
               _ctx: _Context) -> Union[str, markupsafe.Markup]:
   """Return a python snippet, allowing you to specify a class or function.
 
   Args:
       path (str): The path to the file.
       symbol (Optional[str]): The symbol to extract. If None, the entire file is
         returned. Defaults to None.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
       indent (Union[str, int, None], optional): Should indent? By how much, or
         with what prefix? Defaults to None.
+      indented (Union[str, int, None], optional): Indents every line except the
+        first. By how much, or with what prefix? Defaults to None.
       backtickify (Union[bool, str], optional): Should surround with backticks?
         With what language? Defaults to False.
       decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
         HTML comments around this call, setting this to true will add
         correspondingcomments to uncomment the output. This allows you to have
         the Jinja2 call unmolested by markdown formatters, because they will be
         inside of a comment section. "nl" adds additional newlines after the
@@ -409,41 +439,44 @@
 
   Returns:
       Union[str, markupsafe.Markup]: The snippet.
   """
 ```
 <!---->
 
-### pysignature
+### 🐍📖 pysignature
 
 Used several times in [./README.md.jinja2](./README.md.jinja2).
 
 Documentation:
 
 <!---->
 ```py
 def pysignature(path: str,
                 symbol: str,
                 *,
                 escape: bool = False,
                 indent: Union[str, int, None] = None,
+                indented: Union[str, int, None] = None,
                 backtickify: Union[bool, str] = False,
                 decomentify: Union[bool, Literal['nl']] = False,
                 _ctx: _Context) -> str:
   """Return the signature of a class or function in a python file.
 
   Returns the {class,function} signature and the docstring.
 
   Args:
       path (str): The path to the file.
       symbol (str): The symbol to extract.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
       indent (Union[str, int, None], optional): Should indent? By how much, or
         with what prefix? Defaults to None.
+      indented (Union[str, int, None], optional): Indents every line except the
+        first. By how much, or with what prefix? Defaults to None.
       backtickify (Union[bool, str], optional): Should surround with backticks?
         With what language? Defaults to False.
       decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
         HTML comments around this call, setting this to true will add
         correspondingcomments to uncomment the output. This allows you to have
         the Jinja2 call unmolested by markdown formatters, because they will be
         inside of a comment section. "nl" adds additional newlines after the
@@ -453,37 +486,40 @@
 
   Returns:
       str: The signature and docstring.
   """
 ```
 <!---->
 
-### rawsnippet
+### ✂ rawsnippet
 
 Used several times in [./README.md.jinja2](./README.md.jinja2).
 
 Documentation:
 
 <!---->
 ```py
 def rawsnippet(path: str,
                *,
                escape: bool = False,
                indent: Union[str, int, None] = None,
+               indented: Union[str, int, None] = None,
                backtickify: Union[bool, str] = False,
                decomentify: Union[bool, Literal['nl']] = False,
                _ctx: _Context) -> Union[str, markupsafe.Markup]:
   """Return an entire file as a snippet.
 
   Args:
       path (str): The path to the file.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
       indent (Union[str, int, None], optional): Should indent? By how much, or
         with what prefix? Defaults to None.
+      indented (Union[str, int, None], optional): Indents every line except the
+        first. By how much, or with what prefix? Defaults to None.
       backtickify (Union[bool, str], optional): Should surround with backticks?
         With what language? Defaults to False.
       decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
         HTML comments around this call, setting this to true will add
         correspondingcomments to uncomment the output. This allows you to have
         the Jinja2 call unmolested by markdown formatters, because they will be
         inside of a comment section. "nl" adds additional newlines after the
@@ -494,28 +530,29 @@
   Returns:
       Union[str, markupsafe.Markup]: The snippet.
   """
 
 ```
 <!---->
 
-### snippet
+### ✂ snippet
 
 Example in [./snipinator/examples/LONG-EXAMPLE.md.jinja2](./snipinator/examples/LONG-EXAMPLE.md.jinja2).
 
 Documentation:
 
 <!---->
 ```py
 def snippet(path: str,
             start: str,
             end: str,
             *,
             escape: bool = False,
             indent: Union[str, int, None] = None,
+            indented: Union[str, int, None] = None,
             backtickify: Union[bool, str] = False,
             decomentify: Union[bool, Literal['nl']] = False,
             _ctx: _Context) -> Union[str, markupsafe.Markup]:
   """Returns a _delimited_ snippet from a file.
 
   Does not return the delimiters themselves.
 
@@ -523,14 +560,16 @@
       path (str): The path to the file.
       start (str): A string that indicates the start of the snippet.
       end (str): A string that indicates the end of the snippet.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
       indent (Union[str, int, None], optional): Should indent? By how much, or
         with what prefix? Defaults to None.
+      indented (Union[str, int, None], optional): Indents every line except the
+        first. By how much, or with what prefix? Defaults to None.
       backtickify (Union[bool, str], optional): Should surround with backticks?
         With what language? Defaults to False.
       decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
         HTML comments around this call, setting this to true will add
         correspondingcomments to uncomment the output. This allows you to have
         the Jinja2 call unmolested by markdown formatters, because they will be
         inside of a comment section. "nl" adds additional newlines after the
@@ -541,26 +580,27 @@
   Returns:
       Union[str, markupsafe.Markup]: The snippet.
   """
 
 ```
 <!---->
 
-### shell
+### 🐚 shell
 
 Used several times in [./README.md.jinja2](./README.md.jinja2).
 
 Documentation:
 
 <!---->
 ```py
 def shell(args: str,
           *,
           escape: bool = False,
           indent: Union[str, int, None] = None,
+          indented: Union[str, int, None] = None,
           backtickify: Union[bool, str] = False,
           decomentify: Union[bool, Literal['nl']] = False,
           rich: Union[Literal['svg'], Literal['img+b64+svg'], Literal['raw'],
                       str] = 'raw',
           rich_alt: Optional[str] = None,
           rich_bg_color: Optional[str] = None,
           rich_term: Optional[str] = None,
@@ -572,22 +612,34 @@
 
   Use at your own risk, this can potentially introduce security vulnerabilities.
   Only use if you know what you are doing. Ensure that no untrusted input can
   be injected into the `args` parameter, or, into anything the command might
   access. If an adversary can control the `args` parameter, they can execute
   arbitrary commands on your system.
 
+  Note: On persistent output colors:
+
+  * I found that the environment variables TERM, COLORTERM and FORCE_COLOR,
+    CLI_WIDTH, COLUMNS also influence the outputs for some applications.
+  * Also various library versions used in various programs, e.g colorama,
+    rich-argparse, Pygments might influence the output.
+  * I had to pin all my python packages, and explicitly set TERM, COLORTERM and
+    FORCE_COLOR, CLI_WIDTH, COLUMNS to get the output to be consistent across
+    two different systems, both using Ubuntu, for a single program.
+
   Args:
       args (str): The command to run.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
-      indent (Union[str, int, None], optional): Should indent? By how much, or with
-        what prefix? Defaults to None.
-      backtickify (Union[bool, str], optional): Should surround with backticks? With
-        what language? Defaults to False.
+      indent (Union[str, int, None], optional): Should indent? By how much, or
+        with what prefix? Defaults to None.
+      indented (Union[str, int, None], optional): Indents every line except the
+        first. By how much, or with what prefix? Defaults to None.
+      backtickify (Union[bool, str], optional): Should surround with backticks?
+        With what language? Defaults to False.
       decomentify (bool, optional): Assuming that you will be using HTML
         comments around this call, setting this to true will add corresponding
         uncomments to uncomment the output. This allows you to have the Jinja2
         call unmolested by markdown formatters, because they will be inside of
         a comment section. Defaults to False.
       rich (Union[Literal['svg'], Literal['img+b64+svg'], Literal['raw'], str], optional):
         Optionally outputs colored terminal output as an image.
@@ -603,16 +655,16 @@
         * If 'img+svg' a base64 encoded image will be dumped into the markdown
           with the colored terminal output.
         * If 'raw' the raw (uncolored) terminal output will be dumped into the
           markdown directly.
         * Defaults to 'raw.
       rich_alt (Optional[str], optional): The alt text for the img tag. Defaults
         to None.
-      rich_bg_color (Optional[str], optional): The background color for the terminal
-        output. Valid colors include anything valid for SVG colors. See
+      rich_bg_color (Optional[str], optional): The background color for the
+        terminal output. Valid colors include anything valid for SVG colors. See
         <https://developer.mozilla.org/en-US/docs/Web/CSS/color>. Defaults to
         None (fully transparent).
       rich_term: (Optional[str], optional): Sets the TERM env var. Defaults to
         None, which uses whatever the env vars already have.
       rich_rows (int, optional): The number of rows to use for the terminal
         output. Doesn't seem to have much effect. Defaults to 24.
       rich_cols (int, optional): The number of columns to use for the terminal
@@ -624,26 +676,27 @@
 
   Returns:
       Union[str, markupsafe.Markup]: Returns the output of the command.
   """
 ```
 <!---->
 
-### path
+### 🌀 path
 
 Used several times in [./README.md.jinja2](./README.md.jinja2).
 
 Documentation:
 
 <!---->
 ```py
 def path(path: str,
          *,
          escape: bool = False,
          indent: Union[str, int, None] = None,
+         indented: Union[str, int, None] = None,
          backtickify: Union[bool, str] = False,
          decomentify: Union[bool, Literal['nl']] = False,
          link: Optional[Literal['md', 'html']] = None,
          text: Optional[str] = None,
          _ctx: _Context) -> Union[str, markupsafe.Markup]:
   """Verifies that `path` exists, and just returns `path`.
 
@@ -653,14 +706,16 @@
 
   Args:
       path (str): The path to verify.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
       indent (Union[str, int, None], optional): Should indent? By how much, or
         with what prefix? Defaults to None.
+      indented (Union[str, int, None], optional): Indents every line except the
+        first. By how much, or with what prefix? Defaults to None.
       backtickify (Union[bool, str], optional): Should surround with backticks?
         With what language? Defaults to False.
       decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
         HTML comments around this call, setting this to true will add
         correspondingcomments to uncomment the output. This allows you to have
         the Jinja2 call unmolested by markdown formatters, because they will be
         inside of a comment section. "nl" adds additional newlines after the
@@ -676,52 +731,48 @@
   Returns:
       Union[str, markupsafe.Markup]: Just returns the path. If the path doesn't exist,
         it will raise an error.
   """
 ```
 <!---->
 
-Also see Jinja2 v3
-[Template Designer Documentation](https://jinja.palletsprojects.com/en/3.1.x/templates/).
-
 ## ✅ Requirements
 
 - Linux-like environment
   - Why: Uses pexpect.spawn().
 - Python 3.8+
   - Why: Some dev dependencies require Python 3.8+.
 
-### Tested on
+### Tested Platforms
 
-- WSL2 Ubuntu 20.04, Python 3.8.0
-- Ubuntu 20.04, Python 3.8.0, 3.9.0, 3.10.0, 3.11.0, 3.12.0, tested in GitHub
-  Actions workflow
-  ([build-and-test.yml](./.github/workflows/build-and-test.yml)).
+- WSL2 Ubuntu 20.04, Python `3.8.0`.
+- Ubuntu 20.04, Python `3.8.0, 3.9.0, 3.10.0, 3.11.0, 3.12.0`, tested in GitHub Actions
+  workflow ([build-and-test.yml](./.github/workflows/build-and-test.yml)).
 
 ## 🚸 Gotchas and Limitations
 
 - **Security:** This tool is NOT designed to be used with untrusted input. It is
   designed to be used with your own codebase. Even when using your own input, be
   careful that your own code won't be doing anything that might inadvertently
   include untrusted input.
 - Be careful to escape `{{` and `}}`,
   or `{%` and `%}` or anything jinja2
   is sensitive to, in the templates. You'll have to escape it properly for
   jinja2, which involves using `{% raw %}` and
   `{% endraw %}` tags.
-- Recursion: Snipinator doesn't directly support recursive inclusion of
-  generated content. You can generate the contents of one file first, and
-  include that generated content into another template. This would mean that you
-  have to worry about order of generation.
+- Recursion: Snipinator doesn't directly support recursive
+  inclusion of generated content. You can generate the contents of one file
+  first, and include that generated content into another template. This would
+  mean that you have to worry about order of generation.
 - Embedded Backticks: If there are backticks in the included snippet, it might
   ruin the backticks you have in your markdown. This is why `backtickify`
-  parameter exists in the API, so that Snipinator provides the backticks, and it
-  will detect if there are backticks in the snippet and use a different number
-  of backticks on the entire snippet. So if the snippet contains
-  ` ```My Snippet``` `, Snipinator will use
+  parameter exists in the API, so that Snipinator provides the
+  backticks, and it will detect if there are backticks in the snippet and use a
+  different number of backticks on the entire snippet. So if the snippet
+  contains ` ```My Snippet``` `, Snipinator will use
   ` ````language ```My Snippet``` ```` ` and this is a method that Markdown uses
   to allow embedded backticks inside a code block.
 - Formatting: The `{{` `}}` used to
   surround the snippet calls will unfortunately be formatted by a Markdown
   formatter and make the call invalid. Workarounds:
   - **Decommentify**: Put the snippet call inside a HTML comment, then use
     `decommentify` parameter. See
@@ -737,24 +788,25 @@
     be formatted. However, because of **Embedded Backticks** gotcha, (see
     above), this is not recommended, unless you know for sure that there are no
     embedded backticks.
   - If your formatter supports a comment that disabled formatting, you can
     surround the snippet call with that comment.
 - Editing the wrong file: When you have a template and a generated file, it is
   easy to edit the wrong file. To combat this:
-  - Snipinator provides a warning at the top of the generated file to remind you
-    that it is auto-generated.
-  - Snipinator will optionally chmod the file for you to make it read-only.
+  - Snipinator provides a warning at the top of the generated file
+    to remind you that it is auto-generated.
+  - Snipinator will optionally chmod the file for you to make it
+    read-only.
 - Newlines: This program assumes LF newlines. I don't know if it will work for
   anything else.
 - Combining `backtickify` and `indent`: Doesn't make much sense, but if you do
   it, it will run backtickify first, then indent everything including the
   backticks.
 
-## Versioning
+## 🤏 Versioning
 
 We use SemVer for versioning. For the versions available, see the tags on this
 repository.
 
 ## 🔑 License
 
 This project is licensed under the MIT License - see the
@@ -767,74 +819,117 @@
 - Templating: [Jinja2](https://github.com/pallets/jinja).
 - Snippet inclusion: Python's AST library.
 - Colorful CLI help: [rich-argparse](https://github.com/hamdanal/rich-argparse).
 - ANSI coloring shell output:
   {[pexpect](https://pexpect.readthedocs.io/en/stable/),
   [rich](https://github.com/Textualize/rich)}.
 
-## Related Projects
+## 🤝 Related Projects
+
+Not complete, and not necessarily up to date. Make a PR
+([contributions](#-contributions)) to insert/modify.
 
-- [markdown-code-example-inserter](https://github.com/electrovir/markdown-code-example-inserter)
-  "Syncs code examples with markdown documentation."
-- [ARMmbed/snippet](https://github.com/ARMmbed/snippet) "A Python3 tool to
-  extract code snippets from source files".
-- [SimonCropp/MarkdownSnippets](https://github.com/SimonCropp/MarkdownSnippets)
-  "Extracts snippets from code files and merges them into markdown documents".
-- [shiftkey/scribble](https://github.com/shiftkey/scribble) "Making
-  documentation for .NET projects easy and fun".
+| Project                                                           | Stars     | Last Update  | Language   | Platform         | Similarity X Obviousness |
+| ----------------------------------------------------------------- | --------- | ------------ | ---------- | ---------------- | ------------------------ |
+| [mdx-js/mdx][54]                                                  | 16.8k     | `2024/04/17` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
+| [zakhenry/embedme][24]                                            | 222       | `2023/11/08` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
+| [cmacmackin/markdown-include][53]                                 | 95        | `2023/02/07` | Python     | N/A              | ⭐⭐⭐⭐⭐               |
+| [SimonCropp/MarkdownSnippets][31]                                 | 23        | `2024/04/23` | .NET       | N/A              | ⭐⭐⭐⭐⭐               |
+| [endocode/snippetextractor][41]                                   | 4         | `2014/08/16` | C++        | N/A              | ⭐⭐⭐⭐⭐               |
+| [polywrap/doc-snippets][45]                                       | 3         | `2023/09/26` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
+| [JulianCataldo/remark-embed][34]                                  | 2         | `2022/09/22` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
+| [xrd/oreilly-snippets][47]                                        | 2         | `2015/10/15` | Ruby       | N/A              | ⭐⭐⭐⭐⭐               |
+| [DamonOehlman/injectcode][48]                                     | 1         | `2021/08/01` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
+| [electrovir/markdown-code-example-inserter][25]                   | 1         | `2024/02/19` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
+| [andersfischernielsen/Simple-Embedded-Markdown-Code-Snippets][46] | 1         | `2021/02/12` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
+| [ildar-shaimordanov/git-markdown-snippet][36]                     | 0         | `2021/09/14` | Perl       | N/A              | ⭐⭐⭐⭐⭐               |
+| [teyc/markdown-snippet][50]                                       | 0         | `2024/01/22` | Powershell | N/A              | ⭐⭐⭐⭐⭐               |
+| [marc-bouvier-graveyard/baldir_markdown][51]                      | 0         | `2020/06/15` | Python     | N/A              | ⭐⭐⭐⭐⭐               |
+| [dineshsonachalam/markdown-autodocs][26]                          | 176       | `2022/09/19` | JS         | GH Action        | ⭐⭐⭐⭐                 |
+| [tokusumi/markdown-embed-code][29]                                | 28        | `2022/01/05` | Python     | VSCode Extension | ⭐⭐⭐⭐                 |
+| [sammndhr/gridsome-remark-embed-snippet][37]                      | 2         | `2021/06/14` | JS         | [Gridsome][38]   | ⭐⭐⭐⭐                 |
+| [NativeScript/markdown-snippet-injector][44]                      | 4         | `2019/01/24` | JS         | N/A              | ⭐⭐⭐⭐                 |
+| [fuxingloh/remark-code-import-replace][49]                        | 0         | `2022/12/21` | JS         | Remark?          | ⭐⭐⭐⭐                 |
+| [szkiba/mdcode][55]                                               | 15        | `2014/02/12` | Go         | N/A              | ⭐⭐⭐                   |
+| [devincornell/pymddoc][43]                                        | 0         | `2023/12/01` | Python     | Python           | ⭐⭐⭐                   |
+| [shiftkey/scribble][32] ([docs][33])                              | 40        | `2013/08/08` | .NET       | N/A              | ⭐⭐                     |
+| [calebpeterson/jest-transformer-test-md][35]                      | 2         | `2020/08/21` | JS         | Jest Tests       | ⭐⭐                     |
+| [tjstankus/commitate][52]                                         | 0         | `2014/05/29` | Ruby       | N/A              | ⭐                       |
+| [GitHub Docs: Creating a permanent link to a code snippet][23]    | N/A       | N/A          | N/A        | N/A              | ⭐                       |
+| [javierfernandes/markdown-exercises][42]                          | 1         | `2017/05/01` | JS         | N/A              | ⭐                       |
+| [gatsby-remark-embed-snippet][39]                                 | N/A (55k) | `2024/01/23` | JS         | [Gatsby][40]     | ⭐                       |
+| [ARMmbed/snippet][30]                                             | 6         | `2021/08/05` | Python     | N/A              | ?                        |
+| [drewavis/markdowninclude][28]                                    | 1         | `2024/04/06` | JS         | VSCode Extension | ?                        |
+| [romnn/embedme][27]                                               | 0         | `2024/04/18` | Go         | N/A              | ?                        |
 
 ## 🫡 Contributions
 
 ### Development environment: Linux-like
 
 - For running `pre.sh` (Linux-like environment).
+
+  - From [./.github/dependencies.yml](./.github/dependencies.yml), which is used for
+    the GH Action to do a fresh install of everything:
+
+    ```yaml
+    bash: scripts.
+    findutils: scripts.
+    grep: tests.
+    xxd: tests.
+    git: scripts, tests.
+    xxhash: scripts (changeguard).
+    rsync: out-of-directory test.
+    expect: for `unbuffer`, useful to grab and compare ansi color symbols.
+    jq: dependency for [yq](https://github.com/kislyuk/yq), which is used to generate
+      the README; the README generator needs to use `tomlq` (which is a part of `yq`)
+      to query `pyproject.toml`.
+    
+    ```
+
   - Requires `pyenv`, or an exact matching version of python as in
-    `.python-version` (which is currently
-    `3.8.0
-`).
-  - `jq`, ([installation](https://jqlang.github.io/jq/)) required for
-    [yq](https://github.com/kislyuk/yq), which is itself required for our
-    `./README.md` generation, which uses `tomlq` (from the
-    [yq](https://github.com/kislyuk/yq) package) to include version strings from
-    `./pyproject.toml`.
-  - `bash`, `grep`, `awk`, `sed` `xxd`, `git`, `xxhash` (for tests/workflows).
-  - Requires nodejs (for act).
-  - Requires Go (to run act).
-  - docker (for act).
+    [.python-version](.python-version) (which is currently
+    `3.8.0`).
+  - act (to run the GH Action locally):
+    - Requires nodejs.
+    - Requires Go.
+    - docker.
+  - Generate animation:
+    - docker
 
 ### Commit Process
 
 1. (Optionally) Fork the `develop` branch.
 2. Stage your files: `git add path/to/file.py`.
-3. `bash scripts/pre.sh`, this will format, lint, and test the code.
-4. `git status` check if anything changed (generated `./README.md`
-   for example), if so, `git add` the changes, and go back to the previous step.
+3. `bash ./scripts/pre.sh`, this will format, lint, and test the code.
+4. `git status` check if anything changed (generated
+   [./README.md](./README.md) for example), if so, `git add` the
+   changes, and go back to the previous step.
 5. `git commit -m "..."`.
 6. Make a PR to `develop` (or push to develop if you have the rights).
 
-## ⛙ Release Process
+## 🔄🚀 Release Process
 
 These instructions are for maintainers of the project.
 
 1. In the `develop` branch, run `bash ./scripts/pre.sh` to ensure
    everything is in order.
-2. In the `develop` branch, bump the version in `./pyproject.toml`,
-   following semantic versioning principles. Also modify the
-   `last_unstable_release` and `last_stable_release` in the
-   `[tool.changeguard-project-metadata]` table as appropriate. Run
-   `bash scripts/pre.sh` to ensure everything is in order.
+2. In the `develop` branch, bump the version in
+   [./pyproject.toml](./pyproject.toml), following semantic versioning
+   principles. Also modify the `last_unstable_release` and `last_stable_release`
+   in the `[tool.snipinator-project-metadata]` table as appropriate. Run
+   `bash ./scripts/pre.sh` to ensure everything is in order.
 3. In the `develop` branch, commit these changes with a message like
    `"Prepare release X.Y.Z"`. (See the contributions section
    [above](#commit-process)).
 4. Merge the `develop` branch into the `master` branch:
    `git checkout master && git merge develop --no-ff`.
 5. `master` branch: Tag the release: Create a git tag for the release with
    `git tag -a vX.Y.Z -m "Version X.Y.Z"`.
 6. Publish to PyPI: Publish the release to PyPI with
-   `bash scripts/deploy-to-pypi.sh`.
+   `bash ./scripts/deploy-to-pypi.sh`.
 7. Push to GitHub: Push the commit and tags to GitHub with
    `git push && git push --tags`.
 8. The `--no-ff` option adds a commit to the master branch for the merge, so
    refork the develop branch from the master branch:
    `git checkout develop && git merge master`.
 9. Push the develop branch to GitHub: `git push origin develop`.
 
@@ -844,42 +939,82 @@
   https://github.com/realazthat/snipinator/actions/workflows/build-and-test.yml
 [3]:
   https://img.shields.io/github/license/realazthat/snipinator?style=plastic&color=0A1E1E
 [4]:
   https://img.shields.io/pypi/v/snipinator?style=plastic&color=0A1E1E
 [5]: https://pypi.org/project/snipinator/
 [6]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.3.1/master?style=plastic
+  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.4.0/master?style=plastic
 [7]:
   https://img.shields.io/github/last-commit/realazthat/snipinator/master?style=plastic
 [8]:
   https://img.shields.io/pypi/pyversions/snipinator?style=plastic&color=0A1E1E
 [9]:
   https://img.shields.io/github/languages/top/realazthat/snipinator.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E
 [10]:
-  https://github.com/realazthat/snipinator/compare/v1.3.1...master
+  https://github.com/realazthat/snipinator/compare/v1.4.0...master
 [11]:
   https://img.shields.io/github/actions/workflow/status/realazthat/snipinator/build-and-test.yml?branch=develop&style=plastic
 [12]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.3.1/develop?style=plastic
+  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.4.0/develop?style=plastic
 [13]:
-  https://github.com/realazthat/snipinator/compare/v1.3.1...develop
+  https://github.com/realazthat/snipinator/compare/v1.4.0...develop
 [14]:
   https://img.shields.io/github/last-commit/realazthat/snipinator/develop?style=plastic
 [15]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.3.1/develop?style=plastic
+  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.4.0/develop?style=plastic
 [16]:
-  https://github.com/realazthat/snipinator/compare/v1.3.1...develop
+  https://github.com/realazthat/snipinator/compare/v1.4.0...develop
 [17]: https://github.com/realazthat/snipinator/tree/master
 [18]: https://github.com/realazthat/snipinator/tree/develop
 
 <!-- Logo from https://lucide.dev/icons/users -->
 
 [19]:
   https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
 
 <!-- Logo from https://lucide.dev/icons/laptop-minimal -->
 
 [20]:
   https://img.shields.io/badge/Platform-Linux-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
 [21]: ./LICENSE.md
 [22]: ./.github/logo-exported.svg
+[23]:
+  https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-a-permanent-link-to-a-code-snippet
+[24]: https://github.com/zakhenry/embedme
+[25]: https://github.com/electrovir/markdown-code-example-inserter
+[26]: https://github.com/dineshsonachalam/markdown-autodocs
+[27]: https://github.com/romnn/embedme
+[28]: https://github.com/drewavis/markdowninclude
+[29]: https://github.com/tokusumi/markdown-embed-code
+[30]: https://github.com/ARMmbed/snippet
+[31]: https://github.com/SimonCropp/MarkdownSnippets
+[32]: https://github.com/shiftkey/scribble
+[33]:
+  https://github.com/shiftkey/scribble/blob/master/docs/features/code-snippets.md
+[34]: https://github.com/JulianCataldo/remark-embed
+[35]: https://github.com/calebpeterson/jest-transformer-test-md
+[36]: https://github.com/ildar-shaimordanov/git-markdown-snippet
+[37]: https://github.com/sammndhr/gridsome-remark-embed-snippet
+[38]: https://gridsome.org/
+[39]:
+  https://github.com/gatsbyjs/gatsby/tree/master/packages/gatsby-remark-embed-snippet
+[40]: https://github.com/gatsbyjs/gatsby
+[41]: https://github.com/endocode/snippetextractor
+[42]: https://github.com/javierfernandes/markdown-exercises
+[43]: https://github.com/devincornell/pymddoc
+[44]: https://github.com/NativeScript/markdown-snippet-injector
+[45]: https://github.com/polywrap/doc-snippets
+[46]:
+  https://github.com/andersfischernielsen/Simple-Embedded-Markdown-Code-Snippets
+[47]: https://github.com/xrd/oreilly-snippets
+[48]: https://github.com/DamonOehlman/injectcode
+[49]: https://github.com/fuxingloh/remark-code-import-replace
+[50]: https://github.com/teyc/markdown-snippet
+[51]: https://github.com/marc-bouvier-graveyard/baldir_markdown
+[52]: https://github.com/tjstankus/commitate
+[53]: https://github.com/cmacmackin/markdown-include
+[54]: https://github.com/mdx-js/mdx
+[55]:
+  https://github.com/szkiba/mdcode
+  "Extracts code blocks from README and produces tests; a similar approach, but quite different"
+[56]: https://github.com/realazthat/snipinator
```

### Comparing `snipinator-1.3.1/snipinator.egg-info/requires.txt` & `snipinator-1.4.0/snipinator.egg-info/requires.txt`

 * *Files identical despite different names*

