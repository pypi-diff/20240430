# Comparing `tmp/leanblueprint-0.0.6.tar.gz` & `tmp/leanblueprint-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leanblueprint-0.0.6.tar", last modified: Wed Mar 20 17:05:59 2024, max compression
+gzip compressed data, was "leanblueprint-0.0.7.tar", last modified: Tue Apr 30 03:05:32 2024, max compression
```

## Comparing `leanblueprint-0.0.6.tar` & `leanblueprint-0.0.7.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxr-x   0 pmassot   (1001) pmassot   (1001)        0 2024-03-20 17:05:59.314749 leanblueprint-0.0.6/
--rw-rw-r--   0 pmassot   (1001) pmassot   (1001)    11357 2024-03-20 15:41:43.000000 leanblueprint-0.0.6/LICENSE
--rw-rw-r--   0 pmassot   (1001) pmassot   (1001)      158 2024-03-20 15:41:43.000000 leanblueprint-0.0.6/MANIFEST.in
--rw-rw-r--   0 pmassot   (1001) pmassot   (1001)       36 2024-03-20 15:41:43.000000 leanblueprint-0.0.6/NOTICE
--rw-r--r--   0 pmassot   (1001) pmassot   (1001)     9319 2024-03-20 17:05:59.314749 leanblueprint-0.0.6/PKG-INFO
--rw-rw-r--   0 pmassot   (1001) pmassot   (1001)     8648 2024-03-20 15:41:43.000000 leanblueprint-0.0.6/README.md
-drwxrwxr-x   0 pmassot   (1001) pmassot   (1001)        0 2024-03-20 17:05:59.314749 leanblueprint-0.0.6/leanblueprint/
-drwxrwxr-x   0 pmassot   (1001) pmassot   (1001)        0 2024-03-20 17:05:59.314749 leanblueprint-0.0.6/leanblueprint/Packages/
--rw-rw-r--   0 pmassot   (1001) pmassot   (1001)        0 2024-03-20 15:41:43.000000 leanblueprint-0.0.6/leanblueprint/Packages/__init__.py
--rw-rw-r--   0 pmassot   (1001) pmassot   (1001)    11578 2024-03-20 15:41:43.000000 leanblueprint-0.0.6/leanblueprint/Packages/blueprint.py
-drwxrwxr-x   0 pmassot   (1001) pmassot   (1001)        0 2024-03-20 17:05:59.314749 leanblueprint-0.0.6/leanblueprint/Packages/renderer_templates/
--rw-rw-r--   0 pmassot   (1001) pmassot   (1001)       49 2024-01-05 22:34:23.000000 leanblueprint-0.0.6/leanblueprint/Packages/renderer_templates/blueprint.jinja2s
--rw-rw-r--   0 pmassot   (1001) pmassot   (1001)        0 2023-12-22 18:49:25.000000 leanblueprint-0.0.6/leanblueprint/__init__.py
--rw-rw-r--   0 pmassot   (1001) pmassot   (1001)    14653 2024-03-20 15:41:43.000000 leanblueprint-0.0.6/leanblueprint/client.py
-drwxrwxr-x   0 pmassot   (1001) pmassot   (1001)        0 2024-03-20 17:05:59.314749 leanblueprint-0.0.6/leanblueprint/static/
--rw-rw-r--   0 pmassot   (1001) pmassot   (1001)      103 2024-01-04 16:46:15.000000 leanblueprint-0.0.6/leanblueprint/static/blueprint.css
-drwxrwxr-x   0 pmassot   (1001) pmassot   (1001)        0 2024-03-20 17:05:59.314749 leanblueprint-0.0.6/leanblueprint/templates/
--rw-rw-r--   0 pmassot   (1001) pmassot   (1001)     2923 2024-03-20 15:41:43.000000 leanblueprint-0.0.6/leanblueprint/templates/blueprint.yml
--rw-rw-r--   0 pmassot   (1001) pmassot   (1001)      364 2024-03-20 15:41:43.000000 leanblueprint-0.0.6/leanblueprint/templates/content.tex
--rw-rw-r--   0 pmassot   (1001) pmassot   (1001)      483 2024-03-20 15:41:43.000000 leanblueprint-0.0.6/leanblueprint/templates/extra_styles.css
--rw-rw-r--   0 pmassot   (1001) pmassot   (1001)      182 2024-03-20 15:41:43.000000 leanblueprint-0.0.6/leanblueprint/templates/latexmkrc
-drwxrwxr-x   0 pmassot   (1001) pmassot   (1001)        0 2024-03-20 17:05:59.314749 leanblueprint-0.0.6/leanblueprint/templates/macros/
--rw-rw-r--   0 pmassot   (1001) pmassot   (1001)      143 2024-03-20 15:41:43.000000 leanblueprint-0.0.6/leanblueprint/templates/macros/common.tex
--rw-rw-r--   0 pmassot   (1001) pmassot   (1001)     1077 2024-03-20 16:57:20.000000 leanblueprint-0.0.6/leanblueprint/templates/macros/print.tex
--rw-rw-r--   0 pmassot   (1001) pmassot   (1001)      261 2024-03-20 15:41:43.000000 leanblueprint-0.0.6/leanblueprint/templates/macros/web.tex
--rw-rw-r--   0 pmassot   (1001) pmassot   (1001)      340 2024-03-20 15:41:43.000000 leanblueprint-0.0.6/leanblueprint/templates/plastex.cfg
--rw-rw-r--   0 pmassot   (1001) pmassot   (1001)     1125 2024-03-20 15:41:43.000000 leanblueprint-0.0.6/leanblueprint/templates/print.tex
--rw-rw-r--   0 pmassot   (1001) pmassot   (1001)      643 2024-03-20 15:41:43.000000 leanblueprint-0.0.6/leanblueprint/templates/web.tex
-drwxrwxr-x   0 pmassot   (1001) pmassot   (1001)        0 2024-03-20 17:05:59.314749 leanblueprint-0.0.6/leanblueprint.egg-info/
--rw-r--r--   0 pmassot   (1001) pmassot   (1001)     9319 2024-03-20 17:05:59.000000 leanblueprint-0.0.6/leanblueprint.egg-info/PKG-INFO
--rw-rw-r--   0 pmassot   (1001) pmassot   (1001)      904 2024-03-20 17:05:59.000000 leanblueprint-0.0.6/leanblueprint.egg-info/SOURCES.txt
--rw-rw-r--   0 pmassot   (1001) pmassot   (1001)        1 2024-03-20 17:05:59.000000 leanblueprint-0.0.6/leanblueprint.egg-info/dependency_links.txt
--rw-rw-r--   0 pmassot   (1001) pmassot   (1001)       64 2024-03-20 17:05:59.000000 leanblueprint-0.0.6/leanblueprint.egg-info/entry_points.txt
--rw-rw-r--   0 pmassot   (1001) pmassot   (1001)        1 2024-02-09 20:44:25.000000 leanblueprint-0.0.6/leanblueprint.egg-info/not-zip-safe
--rw-rw-r--   0 pmassot   (1001) pmassot   (1001)      113 2024-03-20 17:05:59.000000 leanblueprint-0.0.6/leanblueprint.egg-info/requires.txt
--rw-rw-r--   0 pmassot   (1001) pmassot   (1001)       14 2024-03-20 17:05:59.000000 leanblueprint-0.0.6/leanblueprint.egg-info/top_level.txt
--rw-rw-r--   0 pmassot   (1001) pmassot   (1001)      797 2024-03-20 17:05:59.318749 leanblueprint-0.0.6/setup.cfg
--rw-rw-r--   0 pmassot   (1001) pmassot   (1001)       70 2024-03-20 15:41:43.000000 leanblueprint-0.0.6/setup.py
+drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-04-30 03:05:32.888896 leanblueprint-0.0.7/
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)    11357 2024-03-02 23:37:31.000000 leanblueprint-0.0.7/LICENSE
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      158 2024-03-02 23:37:31.000000 leanblueprint-0.0.7/MANIFEST.in
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)       36 2024-03-02 23:37:31.000000 leanblueprint-0.0.7/NOTICE
+-rw-r--r--   0 pmassot   (1000) pmassot   (1000)     9361 2024-04-30 03:05:32.888896 leanblueprint-0.0.7/PKG-INFO
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)     8690 2024-04-30 01:47:25.000000 leanblueprint-0.0.7/README.md
+drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-04-30 03:05:32.888896 leanblueprint-0.0.7/leanblueprint/
+drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-04-30 03:05:32.888896 leanblueprint-0.0.7/leanblueprint/Packages/
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)        0 2024-03-02 23:37:31.000000 leanblueprint-0.0.7/leanblueprint/Packages/__init__.py
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)    11578 2024-03-20 01:48:19.000000 leanblueprint-0.0.7/leanblueprint/Packages/blueprint.py
+drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-04-30 03:05:32.888896 leanblueprint-0.0.7/leanblueprint/Packages/renderer_templates/
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)       49 2024-03-02 22:17:10.000000 leanblueprint-0.0.7/leanblueprint/Packages/renderer_templates/blueprint.jinja2s
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)        0 2020-05-23 12:35:34.000000 leanblueprint-0.0.7/leanblueprint/__init__.py
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)    15180 2024-04-30 02:43:23.000000 leanblueprint-0.0.7/leanblueprint/client.py
+drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-04-30 03:05:32.888896 leanblueprint-0.0.7/leanblueprint/static/
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      103 2024-01-05 14:42:04.000000 leanblueprint-0.0.7/leanblueprint/static/blueprint.css
+drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-04-30 03:05:32.888896 leanblueprint-0.0.7/leanblueprint/templates/
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)       34 2024-04-29 19:18:12.000000 leanblueprint-0.0.7/leanblueprint/templates/blueprint.sty
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)     2825 2024-04-30 01:49:45.000000 leanblueprint-0.0.7/leanblueprint/templates/blueprint.yml
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      364 2024-03-02 23:37:31.000000 leanblueprint-0.0.7/leanblueprint/templates/content.tex
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      483 2024-03-02 23:37:31.000000 leanblueprint-0.0.7/leanblueprint/templates/extra_styles.css
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      182 2024-03-02 23:37:31.000000 leanblueprint-0.0.7/leanblueprint/templates/latexmkrc
+drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-04-30 03:05:32.888896 leanblueprint-0.0.7/leanblueprint/templates/macros/
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      143 2024-03-02 23:37:31.000000 leanblueprint-0.0.7/leanblueprint/templates/macros/common.tex
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)     1077 2024-04-29 19:18:12.000000 leanblueprint-0.0.7/leanblueprint/templates/macros/print.tex
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      261 2024-03-02 23:37:31.000000 leanblueprint-0.0.7/leanblueprint/templates/macros/web.tex
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      340 2024-03-02 23:37:31.000000 leanblueprint-0.0.7/leanblueprint/templates/plastex.cfg
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)     1125 2024-03-02 23:37:31.000000 leanblueprint-0.0.7/leanblueprint/templates/print.tex
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      643 2024-03-02 23:37:31.000000 leanblueprint-0.0.7/leanblueprint/templates/web.tex
+drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-04-30 03:05:32.888896 leanblueprint-0.0.7/leanblueprint.egg-info/
+-rw-r--r--   0 pmassot   (1000) pmassot   (1000)     9361 2024-04-30 03:05:32.000000 leanblueprint-0.0.7/leanblueprint.egg-info/PKG-INFO
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      942 2024-04-30 03:05:32.000000 leanblueprint-0.0.7/leanblueprint.egg-info/SOURCES.txt
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)        1 2024-04-30 03:05:32.000000 leanblueprint-0.0.7/leanblueprint.egg-info/dependency_links.txt
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)       64 2024-04-30 03:05:32.000000 leanblueprint-0.0.7/leanblueprint.egg-info/entry_points.txt
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)        1 2024-01-30 23:24:22.000000 leanblueprint-0.0.7/leanblueprint.egg-info/not-zip-safe
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      113 2024-04-30 03:05:32.000000 leanblueprint-0.0.7/leanblueprint.egg-info/requires.txt
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)       14 2024-04-30 03:05:32.000000 leanblueprint-0.0.7/leanblueprint.egg-info/top_level.txt
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      797 2024-04-30 03:05:32.892896 leanblueprint-0.0.7/setup.cfg
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)       70 2024-03-02 23:37:31.000000 leanblueprint-0.0.7/setup.py
```

### Comparing `leanblueprint-0.0.6/LICENSE` & `leanblueprint-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `leanblueprint-0.0.6/PKG-INFO` & `leanblueprint-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: leanblueprint
-Version: 0.0.6
+Version: 0.0.7
 Summary: Lean prover blueprint plasTeX plugin.
 Home-page: https://github.com/PatrickMassot/leanblueprint
 Author: Patrick Massot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: plasTeX>=3.1
 Requires-Dist: plastexshowmore>=0.0.2
-Requires-Dist: plastexdepgraph>=0.0.3
+Requires-Dist: plastexdepgraph>=0.0.4
 Requires-Dist: click
 Requires-Dist: rich
 Requires-Dist: rich-click
 Requires-Dist: Jinja2>=3.1.0
 Requires-Dist: GitPython>=3.1.28
 
 # Lean blueprints
@@ -30,19 +30,27 @@
 This package depends on `plastexdepgraph` which requires graphviz and its development libraries. 
 If you have a user-friendly OS, it is as simple as 
 `sudo apt install graphviz libgraphviz-dev`. 
 See https://pygraphviz.github.io/documentation/stable/install.html otherwise.
 
 Then, assuming you have a sane python environment, you only need to run:
 ```
-pip install git+https://github.com/PatrickMassot/leanblueprint.git@client
+pip install leanblueprint
 ```
 Note this will automatically install plasTeX and the other needed python
 packages.
 
+## Upgrading
+
+```
+pip install -U leanblueprint
+```
+
+will upgrade to the latest version.
+
 ## Starting a blueprint
 
 This package provides a command line tool `leanblueprint` that automates in
 particular the creation of a blueprint for your Lean project. This tool is not
 mandatory in any way. Its goal is to make it easy to create a blueprint without
 worrying about choosing a file layout or a continuous integration and deployment
 setup. As every one–size-fits-all tool, it is fairly opinionated. It assumes in
@@ -109,15 +117,15 @@
 `leanblueprint pdf` before `leanblueprint web` to get it to work in the web
 version (and redo it when you add a reference).
 
 ## Editing the blueprint
 
 Assuming you used the `leanblueprint` command line tool to create your blueprint
 (or at least that you use the same file layout), the source of your blueprint
-will be in the `blueprint/src` subfolder of you Lean project folder.
+will be in the `blueprint/src` subfolder of your Lean project folder.
 
 Here you will find two main TeX files: `web.tex` and `print.tex`. The first one
 is intended for plasTeX while the second one is intended for a traditional TeX
 compiler such as `xelatex` or `lualatex`. 
 Each of them includes `macros/common.tex` for all TeX macros that make sense
 for both kinds of outputs (this should be most of your macros). 
 Macros that should behave differently depending on the target format should go
```

### Comparing `leanblueprint-0.0.6/README.md` & `leanblueprint-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,27 @@
 This package depends on `plastexdepgraph` which requires graphviz and its development libraries. 
 If you have a user-friendly OS, it is as simple as 
 `sudo apt install graphviz libgraphviz-dev`. 
 See https://pygraphviz.github.io/documentation/stable/install.html otherwise.
 
 Then, assuming you have a sane python environment, you only need to run:
 ```
-pip install git+https://github.com/PatrickMassot/leanblueprint.git@client
+pip install leanblueprint
 ```
 Note this will automatically install plasTeX and the other needed python
 packages.
 
+## Upgrading
+
+```
+pip install -U leanblueprint
+```
+
+will upgrade to the latest version.
+
 ## Starting a blueprint
 
 This package provides a command line tool `leanblueprint` that automates in
 particular the creation of a blueprint for your Lean project. This tool is not
 mandatory in any way. Its goal is to make it easy to create a blueprint without
 worrying about choosing a file layout or a continuous integration and deployment
 setup. As every one–size-fits-all tool, it is fairly opinionated. It assumes in
@@ -87,15 +95,15 @@
 `leanblueprint pdf` before `leanblueprint web` to get it to work in the web
 version (and redo it when you add a reference).
 
 ## Editing the blueprint
 
 Assuming you used the `leanblueprint` command line tool to create your blueprint
 (or at least that you use the same file layout), the source of your blueprint
-will be in the `blueprint/src` subfolder of you Lean project folder.
+will be in the `blueprint/src` subfolder of your Lean project folder.
 
 Here you will find two main TeX files: `web.tex` and `print.tex`. The first one
 is intended for plasTeX while the second one is intended for a traditional TeX
 compiler such as `xelatex` or `lualatex`. 
 Each of them includes `macros/common.tex` for all TeX macros that make sense
 for both kinds of outputs (this should be most of your macros). 
 Macros that should behave differently depending on the target format should go
```

### Comparing `leanblueprint-0.0.6/leanblueprint/Packages/blueprint.py` & `leanblueprint-0.0.7/leanblueprint/Packages/blueprint.py`

 * *Files identical despite different names*

### Comparing `leanblueprint-0.0.6/leanblueprint/client.py` & `leanblueprint-0.0.7/leanblueprint/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,15 +218,15 @@
                 "Could not guess GitHub information. Will not propose to setup continuous integration.")
             can_try_ci = False
 
     out_dir = Path(repo.working_dir)/"blueprint"
     if out_dir.exists():
         error("There is already a blueprint folder. Aborting blueprint creation.")
 
-    console.print("We will now ask some questions to configure your blueprint. All answers can ce changed later by editing either the plastex.cfg file or the tex files.")
+    console.print("We will now ask some questions to configure your blueprint. All answers can be changed later by editing either the plastex.cfg file or the tex files.")
     config: Dict[str, Any] = dict()
 
     if 'master' in repo.branches:
         config['master_branch'] = "master"
     elif 'main' in repo.branches:
         config['master_branch'] = "main"
     else:
@@ -237,15 +237,15 @@
 
     console.print("\nGeneral information about the project", style="title")
     config['title'] = ask("Project title", default="My formalization project")
     if len(libs) > 1:
         config['lib_name'] = ask(
             "Lean library name", choices=libs, default=default_lib or libs[0])
     else:
-        config['lib_name'] = default=default_lib or libs[0]
+        config['lib_name'] = default_lib or libs[0]
     config['author'] = ask(
         "Author ([info]use \\and to separate authors if needed[/])", default=name)
 
     config['github'] = ask("Url of github repository", default=github)
     config['home'] = ask("Url of project website", default=githubIO)
     config['dochome'] = ask(
         "Url of project API documentation", default=doc_home)
@@ -277,36 +277,41 @@
         tpl = env.get_template(tpl_name)
         path = out_dir/"src"/tpl_name
         path.parent.mkdir(exist_ok=True)
         tpl.stream(config).dump(str(path))
 
     if platform.system() == 'Windows':
         console.print(
-            "\nBlueprint source sucessfully created in the blueprint folder.\n")
+            "\nBlueprint source successfully created in the blueprint folder.\n")
     else:
         console.print(
-            "\nBlueprint source sucessfully created in the blueprint folder :tada:\n")
+            "\nBlueprint source successfully created in the blueprint folder :tada:\n")
 
-    if confirm("Modify lakefile to allow checking declarations exist?",
+    console.print("\nLake configuration updating", style="title")
+    console.print("The next two questions are crucial for the blueprint infrastructure. Please use the default answer unless you are really sure you already did the necessary work.")
+
+    if confirm("Modify lakefile and lake-manifest to allow checking declarations exist?",
                default=True):
         with lakefile_path.open("a") as lf:
             lf.write('\nrequire checkdecls from git "https://github.com/PatrickMassot/checkdecls.git"')
-        console.print("Ok, lakefile is edited. Will now get the declaration check library.")
+        console.print("Ok, lakefile is edited. Will now get the declaration check library. Note this may be long if you just created the project and did not yet get Mathlib.")
         subprocess.run("lake update checkdecls",
                        cwd=str(blueprint_root.parent), check=False, shell=True)
 
-    if confirm("Modify lakefile to allow building the documentation on GitHub?",
+    if confirm("Modify lakefile and lake-manifest to allow building the documentation?",
                default=True):
         with lakefile_path.open("a", encoding="utf8") as lf:
             lf.write(dedent('''
 
                 meta if get_config? env = some "dev" then
                 require «doc-gen4» from git
                   "https://github.com/leanprover/doc-gen4" @ "main"'''))
-        console.print("Ok, lakefile is edited.")
+        console.print("Ok, lakefile is edited. Will now get the doc-gen library.")
+        subprocess.run("lake -R -Kenv=dev update doc-gen4",
+                       cwd=str(blueprint_root.parent), check=False, shell=True)
 
 
     workflow_files: List[Path] = []
     if can_try_ci and confirm("Configure continuous integration to compile blueprint?",
                               default=True):
         tpl = env.get_template("blueprint.yml")
         path = Path(repo.working_dir)/".github"/"workflows"
```

### Comparing `leanblueprint-0.0.6/leanblueprint/templates/blueprint.yml` & `leanblueprint-0.0.7/leanblueprint/templates/blueprint.yml`

 * *Files 4% similar despite different names*

```diff
@@ -18,22 +18,19 @@
         uses: actions/checkout@v2
         with:
           fetch-depth: 0
 
       - name: Install elan
         run: curl https://raw.githubusercontent.com/leanprover/elan/master/elan-init.sh -sSf | sh -s -- -y --default-toolchain leanprover/lean4:4.5.0
 
-      - name: Update checkdecls
-        run: ~/.elan/bin/lake update checkdecls
-
       - name: Get cache
-        run: ~/.elan/bin/lake -Kenv=dev exe cache get || true
+        run: ~/.elan/bin/lake exe cache get || true
 
       - name: Build project
-        run: ~/.elan/bin/lake -Kenv=dev build {| lib_name |}
+        run: ~/.elan/bin/lake build {| lib_name |}
 
       - name: Cache mathlib docs
         uses: actions/cache@v3
         with:
           path: |
             .lake/build/doc/Init
             .lake/build/doc/Lake
@@ -43,15 +40,15 @@
             .lake/build/doc/declarations
             !.lake/build/doc/declarations/declaration-data-{| lib_name |}*
           key: MathlibDoc-${{ hashFiles('lake-manifest.json') }}
           restore-keys: |
             MathlibDoc-
 
       - name: Build documentation
-        run: ~/.elan/bin/lake -Kenv=dev build {| lib_name |}:docs
+        run: ~/.elan/bin/lake -R -Kenv=dev build {| lib_name |}:docs
 
       - name: Build blueprint and copy to `docs/blueprint`
         uses: xu-cheng/texlive-action@v2
         with:
           docker_image: ghcr.io/xu-cheng/texlive-full:20231201
           run: |
             apk update
```

### Comparing `leanblueprint-0.0.6/leanblueprint/templates/macros/print.tex` & `leanblueprint-0.0.7/leanblueprint/templates/macros/print.tex`

 * *Files identical despite different names*

### Comparing `leanblueprint-0.0.6/leanblueprint/templates/print.tex` & `leanblueprint-0.0.7/leanblueprint/templates/print.tex`

 * *Files identical despite different names*

### Comparing `leanblueprint-0.0.6/leanblueprint/templates/web.tex` & `leanblueprint-0.0.7/leanblueprint/templates/web.tex`

 * *Files identical despite different names*

### Comparing `leanblueprint-0.0.6/leanblueprint.egg-info/PKG-INFO` & `leanblueprint-0.0.7/leanblueprint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: leanblueprint
-Version: 0.0.6
+Version: 0.0.7
 Summary: Lean prover blueprint plasTeX plugin.
 Home-page: https://github.com/PatrickMassot/leanblueprint
 Author: Patrick Massot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: plasTeX>=3.1
 Requires-Dist: plastexshowmore>=0.0.2
-Requires-Dist: plastexdepgraph>=0.0.3
+Requires-Dist: plastexdepgraph>=0.0.4
 Requires-Dist: click
 Requires-Dist: rich
 Requires-Dist: rich-click
 Requires-Dist: Jinja2>=3.1.0
 Requires-Dist: GitPython>=3.1.28
 
 # Lean blueprints
@@ -30,19 +30,27 @@
 This package depends on `plastexdepgraph` which requires graphviz and its development libraries. 
 If you have a user-friendly OS, it is as simple as 
 `sudo apt install graphviz libgraphviz-dev`. 
 See https://pygraphviz.github.io/documentation/stable/install.html otherwise.
 
 Then, assuming you have a sane python environment, you only need to run:
 ```
-pip install git+https://github.com/PatrickMassot/leanblueprint.git@client
+pip install leanblueprint
 ```
 Note this will automatically install plasTeX and the other needed python
 packages.
 
+## Upgrading
+
+```
+pip install -U leanblueprint
+```
+
+will upgrade to the latest version.
+
 ## Starting a blueprint
 
 This package provides a command line tool `leanblueprint` that automates in
 particular the creation of a blueprint for your Lean project. This tool is not
 mandatory in any way. Its goal is to make it easy to create a blueprint without
 worrying about choosing a file layout or a continuous integration and deployment
 setup. As every one–size-fits-all tool, it is fairly opinionated. It assumes in
@@ -109,15 +117,15 @@
 `leanblueprint pdf` before `leanblueprint web` to get it to work in the web
 version (and redo it when you add a reference).
 
 ## Editing the blueprint
 
 Assuming you used the `leanblueprint` command line tool to create your blueprint
 (or at least that you use the same file layout), the source of your blueprint
-will be in the `blueprint/src` subfolder of you Lean project folder.
+will be in the `blueprint/src` subfolder of your Lean project folder.
 
 Here you will find two main TeX files: `web.tex` and `print.tex`. The first one
 is intended for plasTeX while the second one is intended for a traditional TeX
 compiler such as `xelatex` or `lualatex`. 
 Each of them includes `macros/common.tex` for all TeX macros that make sense
 for both kinds of outputs (this should be most of your macros). 
 Macros that should behave differently depending on the target format should go
```

### Comparing `leanblueprint-0.0.6/leanblueprint.egg-info/SOURCES.txt` & `leanblueprint-0.0.7/leanblueprint.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 leanblueprint.egg-info/not-zip-safe
 leanblueprint.egg-info/requires.txt
 leanblueprint.egg-info/top_level.txt
 leanblueprint/Packages/__init__.py
 leanblueprint/Packages/blueprint.py
 leanblueprint/Packages/renderer_templates/blueprint.jinja2s
 leanblueprint/static/blueprint.css
+leanblueprint/templates/blueprint.sty
 leanblueprint/templates/blueprint.yml
 leanblueprint/templates/content.tex
 leanblueprint/templates/extra_styles.css
 leanblueprint/templates/latexmkrc
 leanblueprint/templates/plastex.cfg
 leanblueprint/templates/print.tex
 leanblueprint/templates/web.tex
```

### Comparing `leanblueprint-0.0.6/setup.cfg` & `leanblueprint-0.0.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = leanblueprint
 description = Lean prover blueprint plasTeX plugin.
 long_description = file: README.md
 long_description_content_type = text/markdown
-version = 0.0.6
+version = 0.0.7
 author = Patrick Massot
 url = https://github.com/PatrickMassot/leanblueprint
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
@@ -17,15 +17,15 @@
 	leanblueprint.Packages
 python_requires = >=3.7
 zip_safe = False
 include_package_data = True
 install_requires = 
 	plasTeX >= 3.1
 	plastexshowmore >= 0.0.2
-	plastexdepgraph >= 0.0.3
+	plastexdepgraph >= 0.0.4
 	click
 	rich
 	rich-click
 	Jinja2 >= 3.1.0
 	GitPython >= 3.1.28
 
 [options.entry_points]
```

