# Comparing `tmp/mkdocs-table-of-figures-0.3.2.tar.gz` & `tmp/mkdocs-table-of-figures-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-table-of-figures-0.3.2.tar", last modified: Tue Apr 30 12:11:51 2024, max compression
+gzip compressed data, was "mkdocs-table-of-figures-0.3.3.tar", last modified: Tue Apr 30 15:15:40 2024, max compression
```

## Comparing `mkdocs-table-of-figures-0.3.2.tar` & `mkdocs-table-of-figures-0.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-30 12:11:51.366422 mkdocs-table-of-figures-0.3.2/
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       77 2024-04-23 06:07:49.000000 mkdocs-table-of-figures-0.3.2/MANIFEST.in
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     8699 2024-04-30 12:11:51.364421 mkdocs-table-of-figures-0.3.2/PKG-INFO
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     2351 2024-04-30 12:09:59.000000 mkdocs-table-of-figures-0.3.2/changelog.md
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1075 2024-04-23 06:07:49.000000 mkdocs-table-of-figures-0.3.2/license
-drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-30 12:11:51.276763 mkdocs-table-of-figures-0.3.2/mkdocs_table_of_figures/
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-23 06:07:49.000000 mkdocs-table-of-figures-0.3.2/mkdocs_table_of_figures/__init__.py
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)    16853 2024-04-30 12:09:52.000000 mkdocs-table-of-figures-0.3.2/mkdocs_table_of_figures/plugin.py
-drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-30 12:11:51.349274 mkdocs-table-of-figures-0.3.2/mkdocs_table_of_figures.egg-info/
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     8699 2024-04-30 12:11:50.000000 mkdocs-table-of-figures-0.3.2/mkdocs_table_of_figures.egg-info/PKG-INFO
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)      417 2024-04-30 12:11:50.000000 mkdocs-table-of-figures-0.3.2/mkdocs_table_of_figures.egg-info/SOURCES.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        1 2024-04-30 12:11:50.000000 mkdocs-table-of-figures-0.3.2/mkdocs_table_of_figures.egg-info/dependency_links.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       83 2024-04-30 12:11:50.000000 mkdocs-table-of-figures-0.3.2/mkdocs_table_of_figures.egg-info/entry_points.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       14 2024-04-30 12:11:50.000000 mkdocs-table-of-figures-0.3.2/mkdocs_table_of_figures.egg-info/requires.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       24 2024-04-30 12:11:50.000000 mkdocs-table-of-figures-0.3.2/mkdocs_table_of_figures.egg-info/top_level.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     8212 2024-04-30 12:11:19.000000 mkdocs-table-of-figures-0.3.2/readme.md
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       38 2024-04-30 12:11:51.367420 mkdocs-table-of-figures-0.3.2/setup.cfg
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1135 2024-04-30 11:14:41.000000 mkdocs-table-of-figures-0.3.2/setup.py
+drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-30 15:15:40.346527 mkdocs-table-of-figures-0.3.3/
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       77 2024-04-23 06:07:49.000000 mkdocs-table-of-figures-0.3.3/MANIFEST.in
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     8699 2024-04-30 15:15:40.343525 mkdocs-table-of-figures-0.3.3/PKG-INFO
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     2449 2024-04-30 15:14:46.000000 mkdocs-table-of-figures-0.3.3/changelog.md
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1075 2024-04-23 06:07:49.000000 mkdocs-table-of-figures-0.3.3/license
+drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-30 15:15:40.250301 mkdocs-table-of-figures-0.3.3/mkdocs_table_of_figures/
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-23 06:07:49.000000 mkdocs-table-of-figures-0.3.3/mkdocs_table_of_figures/__init__.py
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)    16843 2024-04-30 15:03:07.000000 mkdocs-table-of-figures-0.3.3/mkdocs_table_of_figures/plugin.py
+drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-30 15:15:40.331525 mkdocs-table-of-figures-0.3.3/mkdocs_table_of_figures.egg-info/
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     8699 2024-04-30 15:15:39.000000 mkdocs-table-of-figures-0.3.3/mkdocs_table_of_figures.egg-info/PKG-INFO
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)      417 2024-04-30 15:15:39.000000 mkdocs-table-of-figures-0.3.3/mkdocs_table_of_figures.egg-info/SOURCES.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        1 2024-04-30 15:15:39.000000 mkdocs-table-of-figures-0.3.3/mkdocs_table_of_figures.egg-info/dependency_links.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       83 2024-04-30 15:15:39.000000 mkdocs-table-of-figures-0.3.3/mkdocs_table_of_figures.egg-info/entry_points.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       14 2024-04-30 15:15:39.000000 mkdocs-table-of-figures-0.3.3/mkdocs_table_of_figures.egg-info/requires.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       24 2024-04-30 15:15:39.000000 mkdocs-table-of-figures-0.3.3/mkdocs_table_of_figures.egg-info/top_level.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     8212 2024-04-30 12:11:19.000000 mkdocs-table-of-figures-0.3.3/readme.md
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       38 2024-04-30 15:15:40.347526 mkdocs-table-of-figures-0.3.3/setup.cfg
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1135 2024-04-30 15:09:36.000000 mkdocs-table-of-figures-0.3.3/setup.py
```

### Comparing `mkdocs-table-of-figures-0.3.2/PKG-INFO` & `mkdocs-table-of-figures-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-table-of-figures
-Version: 0.3.2
+Version: 0.3.3
 Summary: A MkDocs plugin listing all figures to create a table of figures page
 Home-page: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures
 Author: Thibaud Briard
 Author-email: thibaud.brrd@eduge.ch
 License: MIT
 Keywords: mkdocs
 Platform: UNKNOWN
```

### Comparing `mkdocs-table-of-figures-0.3.2/changelog.md` & `mkdocs-table-of-figures-0.3.3/changelog.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on Keep a Changelog, and this project adheres to Semantic Versioning.
 
+## [0.3.3] - 2024-04-30
+
+### Fixed
+
+- pairs figures styles to work with `mkdocs-with-pdfs`
+
 ## [0.3.2] - 2024-04-30
 
 ### Added
 
 - support for pair of images
 
 ## [0.3.1] - 2024-04-29
```

### Comparing `mkdocs-table-of-figures-0.3.2/license` & `mkdocs-table-of-figures-0.3.3/license`

 * *Files identical despite different names*

### Comparing `mkdocs-table-of-figures-0.3.2/mkdocs_table_of_figures/plugin.py` & `mkdocs-table-of-figures-0.3.3/mkdocs_table_of_figures/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,15 +204,15 @@
                                 self.figures.append({"number": self.counter, "description": match.group(1), "link": link, "type": self.config.image_type_name, "section": section})
                                 replacement = f'<figure id="figure-{self.counter}" class="figure-image" markdown="span">\n  <img src="{config.site_url + match.group(2) if match.group(2).startswith("/") else match.group(2)}" alt="{match.group(1)}">\n  <figcaption>{self.config.figure_label} {self.counter} — {match.group(1)}</figcaption>\n</figure>'
                                 if self.keep_md_format:
                                     replacement = f'<figure id="figure-{self.counter}" class="figure-image" markdown="span">\n![{match.group(1)}]({match.group(2)}){match.group(3) if match.group(3) else ""}\n<figcaption>{self.config.figure_label} {self.counter} — {match.group(1)}</figcaption>\n</figure>'
                             elif match.re.pattern == pattern_pair and match.group(1):
                                 link += f'-{self.counter + 1}'
                                 self.figures.append({"number": [self.counter, self.counter + 1], "description": f'{"← " if self.config.show_pair_description_arrows else ""}{match.group(1)}</br>{"→ " if self.config.show_pair_description_arrows else ""}{match.group(4)}' if match.group(4) else match.group(1), "link": link, "type": self.config.pair_type_name, "section": section})
-                                replacement = f'<figure id="figure-{self.counter}-{self.counter + 1}" class="figure-image" markdown>\n<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 1em;" markdown>\n<div style="display: flex; justify-content: flex-end; align-items: center;" markdown="span">\n![{match.group(1)}]({match.group(2)}){match.group(3) if match.group(3) else ""}\n</div>\n<div style="display: flex; justify-content: flex-start; align-items: center;" markdown="span">\n![{match.group(4)}]({match.group(5)}){match.group(6) if match.group(6) else ""}\n</div>\n</div>\n<figcaption>{self.config.figure_label} {self.counter} & {self.counter + 1} — {match.group(1)}{(" <span>|</span> " + match.group(4)) if match.group(4) else ""}</figcaption>\n</figure>'
+                                replacement = f'<figure id="figure-{self.counter}-{self.counter + 1}" class="figure-pair" markdown>\n<div style="display: flex; align-items: center;" markdown="span">\n<div style="flex: 1; display: flex; justify-content: flex-end; margin-right: 0.5em" markdown="span">![{match.group(1)}]({match.group(2)}){match.group(3) if match.group(3) else ""}</div><div style="flex: 1; display: flex; justify-content: flex-start; margin-left: 0.5em" markdown="span">![{match.group(4)}]({match.group(5)}){match.group(6) if match.group(6) else ""}</div>\n</div>\n<figcaption>{self.config.figure_label} {self.counter} & {self.counter + 1} — {match.group(1)}{(" <span>|</span> " + match.group(4)) if match.group(4) else ""}</figcaption>\n</figure>'
                             elif (match.re.pattern == pattern_mermaid and match.group(4)) or (self.config.on_mermaid and match.re.pattern == pattern_codeblock and match.group(2) == 'mermaid' and match.group(4)):
                                 self.figures.append({"number": self.counter, "description": match.group(4), "link": link, "type": self.config.mermaid_type_name, "section": section})
                                 replacement = f'<figure id="figure-{self.counter}" class="figure-mermaid" markdown>\n{match.group(1)}\n<figcaption>{self.config.figure_label} {self.counter} — {match.group(4)}</figcaption>\n</figure>'
                             elif match.re.pattern == pattern_codeblock and match.group(2) != 'mermaid' and match.group(4):
                                 self.figures.append({"number": self.counter, "description": match.group(4), "link": link, "type": self.config.codeblock_type_name, "section": section})
                                 replacement = f'<figure id="figure-{self.counter}" class="figure-codeblock" markdown>\n{match.group(1)}\n<figcaption>{self.config.figure_label} {self.counter} — {match.group(4)}</figcaption>\n</figure>'
                             elif match.re.pattern == pattern_table and match.group(2):
```

### Comparing `mkdocs-table-of-figures-0.3.2/mkdocs_table_of_figures.egg-info/PKG-INFO` & `mkdocs-table-of-figures-0.3.3/mkdocs_table_of_figures.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-table-of-figures
-Version: 0.3.2
+Version: 0.3.3
 Summary: A MkDocs plugin listing all figures to create a table of figures page
 Home-page: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures
 Author: Thibaud Briard
 Author-email: thibaud.brrd@eduge.ch
 License: MIT
 Keywords: mkdocs
 Platform: UNKNOWN
```

### Comparing `mkdocs-table-of-figures-0.3.2/readme.md` & `mkdocs-table-of-figures-0.3.3/readme.md`

 * *Files identical despite different names*

### Comparing `mkdocs-table-of-figures-0.3.2/setup.py` & `mkdocs-table-of-figures-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import io
 
 from setuptools import setup, find_packages
 
 setup(
     name='mkdocs-table-of-figures',
-    version='0.3.2',
+    version='0.3.3',
     description='A MkDocs plugin listing all figures to create a table of figures page',
     long_description=io.open('readme.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
     keywords='mkdocs',
     url='https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures',
     author='Thibaud Briard',
     author_email='thibaud.brrd@eduge.ch',
```

