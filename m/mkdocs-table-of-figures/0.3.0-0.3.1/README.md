# Comparing `tmp/mkdocs-table-of-figures-0.3.0.tar.gz` & `tmp/mkdocs-table-of-figures-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-table-of-figures-0.3.0.tar", last modified: Mon Apr 29 08:20:37 2024, max compression
+gzip compressed data, was "mkdocs-table-of-figures-0.3.1.tar", last modified: Mon Apr 29 19:01:09 2024, max compression
```

## Comparing `mkdocs-table-of-figures-0.3.0.tar` & `mkdocs-table-of-figures-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-29 08:20:37.299451 mkdocs-table-of-figures-0.3.0/
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       77 2024-04-23 06:07:49.000000 mkdocs-table-of-figures-0.3.0/MANIFEST.in
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     7295 2024-04-29 08:20:37.297451 mkdocs-table-of-figures-0.3.0/PKG-INFO
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     2023 2024-04-29 07:54:58.000000 mkdocs-table-of-figures-0.3.0/changelog.md
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1075 2024-04-23 06:07:49.000000 mkdocs-table-of-figures-0.3.0/license
-drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-29 08:20:37.207121 mkdocs-table-of-figures-0.3.0/mkdocs_table_of_figures/
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-23 06:07:49.000000 mkdocs-table-of-figures-0.3.0/mkdocs_table_of_figures/__init__.py
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)    14143 2024-04-29 08:05:41.000000 mkdocs-table-of-figures-0.3.0/mkdocs_table_of_figures/plugin.py
-drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-29 08:20:37.282668 mkdocs-table-of-figures-0.3.0/mkdocs_table_of_figures.egg-info/
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     7295 2024-04-29 08:20:36.000000 mkdocs-table-of-figures-0.3.0/mkdocs_table_of_figures.egg-info/PKG-INFO
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)      417 2024-04-29 08:20:36.000000 mkdocs-table-of-figures-0.3.0/mkdocs_table_of_figures.egg-info/SOURCES.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        1 2024-04-29 08:20:36.000000 mkdocs-table-of-figures-0.3.0/mkdocs_table_of_figures.egg-info/dependency_links.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       83 2024-04-29 08:20:36.000000 mkdocs-table-of-figures-0.3.0/mkdocs_table_of_figures.egg-info/entry_points.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       14 2024-04-29 08:20:36.000000 mkdocs-table-of-figures-0.3.0/mkdocs_table_of_figures.egg-info/requires.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       24 2024-04-29 08:20:36.000000 mkdocs-table-of-figures-0.3.0/mkdocs_table_of_figures.egg-info/top_level.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     6774 2024-04-29 08:04:51.000000 mkdocs-table-of-figures-0.3.0/readme.md
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       38 2024-04-29 08:20:37.300452 mkdocs-table-of-figures-0.3.0/setup.cfg
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1135 2024-04-29 07:55:08.000000 mkdocs-table-of-figures-0.3.0/setup.py
+drwxrwxrwx   0 brt       (1000) brt       (1000)        0 2024-04-29 19:01:09.166821 mkdocs-table-of-figures-0.3.1/
+-rwxrwxrwx   0 brt       (1000) brt       (1000)       77 2024-04-28 20:57:06.000000 mkdocs-table-of-figures-0.3.1/MANIFEST.in
+-rwxrwxrwx   0 brt       (1000) brt       (1000)     7853 2024-04-29 19:01:09.165820 mkdocs-table-of-figures-0.3.1/PKG-INFO
+-rwxrwxrwx   0 brt       (1000) brt       (1000)     2279 2024-04-29 18:55:38.000000 mkdocs-table-of-figures-0.3.1/changelog.md
+-rwxrwxrwx   0 brt       (1000) brt       (1000)     1075 2024-04-28 20:57:06.000000 mkdocs-table-of-figures-0.3.1/license
+drwxrwxrwx   0 brt       (1000) brt       (1000)        0 2024-04-29 19:01:09.109732 mkdocs-table-of-figures-0.3.1/mkdocs_table_of_figures/
+-rwxrwxrwx   0 brt       (1000) brt       (1000)        0 2024-04-28 20:57:06.000000 mkdocs-table-of-figures-0.3.1/mkdocs_table_of_figures/__init__.py
+-rwxrwxrwx   0 brt       (1000) brt       (1000)    14549 2024-04-29 18:43:17.000000 mkdocs-table-of-figures-0.3.1/mkdocs_table_of_figures/plugin.py
+drwxrwxrwx   0 brt       (1000) brt       (1000)        0 2024-04-29 19:01:09.155308 mkdocs-table-of-figures-0.3.1/mkdocs_table_of_figures.egg-info/
+-rwxrwxrwx   0 brt       (1000) brt       (1000)     7853 2024-04-29 19:01:08.000000 mkdocs-table-of-figures-0.3.1/mkdocs_table_of_figures.egg-info/PKG-INFO
+-rwxrwxrwx   0 brt       (1000) brt       (1000)      417 2024-04-29 19:01:08.000000 mkdocs-table-of-figures-0.3.1/mkdocs_table_of_figures.egg-info/SOURCES.txt
+-rwxrwxrwx   0 brt       (1000) brt       (1000)        1 2024-04-29 19:01:08.000000 mkdocs-table-of-figures-0.3.1/mkdocs_table_of_figures.egg-info/dependency_links.txt
+-rwxrwxrwx   0 brt       (1000) brt       (1000)       83 2024-04-29 19:01:08.000000 mkdocs-table-of-figures-0.3.1/mkdocs_table_of_figures.egg-info/entry_points.txt
+-rwxrwxrwx   0 brt       (1000) brt       (1000)       14 2024-04-29 19:01:08.000000 mkdocs-table-of-figures-0.3.1/mkdocs_table_of_figures.egg-info/requires.txt
+-rwxrwxrwx   0 brt       (1000) brt       (1000)       24 2024-04-29 19:01:08.000000 mkdocs-table-of-figures-0.3.1/mkdocs_table_of_figures.egg-info/top_level.txt
+-rwxrwxrwx   0 brt       (1000) brt       (1000)     7344 2024-04-29 19:00:33.000000 mkdocs-table-of-figures-0.3.1/readme.md
+-rwxrwxrwx   0 brt       (1000) brt       (1000)       38 2024-04-29 19:01:09.166821 mkdocs-table-of-figures-0.3.1/setup.cfg
+-rwxrwxrwx   0 brt       (1000) brt       (1000)     1135 2024-04-29 18:19:53.000000 mkdocs-table-of-figures-0.3.1/setup.py
```

### Comparing `mkdocs-table-of-figures-0.3.0/PKG-INFO` & `mkdocs-table-of-figures-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-table-of-figures
-Version: 0.3.0
+Version: 0.3.1
 Summary: A MkDocs plugin listing all figures to create a table of figures page
 Home-page: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures
 Author: Thibaud Briard
 Author-email: thibaud.brrd@eduge.ch
 License: MIT
 Keywords: mkdocs
 Platform: UNKNOWN
@@ -157,14 +157,26 @@
 You can place the stylesheet in your `mkdocs.yml` at extra-css option
 
 ``` yml
 extra_css:
   - fix-mermaid-figure.css
 ```
 
+### Custom attributes
+
+To use custom attributes on images, like this :
+
+``` markdown
+![Image alt](image.png){ width="300" }
+```
+
+it require `glightbox` and `attr_list` and `md_in_html` from `mkdocs-material`. More details on `mkdocs-material` documentation : [https://squidfunk.github.io/mkdocs-material/reference/images/?h=image#image-alignment-left](https://squidfunk.github.io/mkdocs-material/reference/images/?h=image#image-alignment-left).
+
+Note that `align=left` and `align=right` attributes will be overriden by figures style from `mkdocs-material`.
+
 ## License
 
 This project is under MIT license. See the `license` file for more details.
 
 ## See Also
 
 - [GitLab Repo](http://www.gitlab.org/cfpt-mkdocs-plugins/mkdocs-table-of-figures/)
```

### Comparing `mkdocs-table-of-figures-0.3.0/changelog.md` & `mkdocs-table-of-figures-0.3.1/changelog.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on Keep a Changelog, and this project adheres to Semantic Versioning.
 
+## [0.3.1] - 2024-04-29
+
+### Added
+
+- support for custom attribute on image using `glightbox` and `mkdocs-material` plugins with `attr_list` and `md_in_html` enable
+
+### Fixed
+
+- removed extra `>` from section where image have no heading before
+
 ## [0.3.0] - 2024-04-29
 
 ### Added
 
 - table column containing info abtout the type of figure
 - table column containing info abtout the section where the figure is located
```

### Comparing `mkdocs-table-of-figures-0.3.0/license` & `mkdocs-table-of-figures-0.3.1/license`

 * *Files identical despite different names*

### Comparing `mkdocs-table-of-figures-0.3.0/mkdocs_table_of_figures/plugin.py` & `mkdocs-table-of-figures-0.3.1/mkdocs_table_of_figures/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,15 @@
                 if self.config.follow_nav_structure and self.nav_structure:
                     found, counter = self.count_previous_figures(page, self.nav_structure)
                     if found:
                         self.counter = counter + 1
 
                 original = markdown
                 try:
-                    pattern_img = r'!\[(.*?)\]\((.+?)\)'
+                    pattern_img = r'!\[(.*?)\]\((.+?)\)(.*)'
                     pattern_mermaid = r'^(``` ?(mermaid)\r?\n(.*?)```)$\r?\n^(.*?)$'
                     pattern_codeblock = r'^(``` ?([^\r\n]*)\r?\n(.*?)```)$\r?\n^(.*?)$'
                     pattern_table = r'^((?:\|[^|\r\n]*)+\|\r?\n(?:\|[-: ]*)+\|(?:\r?\n(?:\|[^|\r\n]*)+\|)*)\r?\n^([^|]*?)$'
                     
                     matches = []
                     matches.extend(re.finditer(pattern_img, markdown, flags= re.IGNORECASE))
                     matches.extend(re.finditer(pattern_mermaid, markdown, flags= re.MULTILINE | re.DOTALL)) if self.config.on_mermaid and not self.config.on_codeblock else None
@@ -173,26 +173,32 @@
                                             section = header_title
                                     else:
                                         header_level = 0
                                     if header_level <= 1:
                                         break
                             current_section = page
                             if current_section.parent is None:
-                                section = config.site_name + ' > ' + ((current_section.title + ' > ') if header_level != 1 else '') + section
+                                if section != '':
+                                    section = config.site_name + ' > ' + ((current_section.title + ' > ') if header_level != 1 else '') + section
+                                else:
+                                    section = config.site_name + ((' > ' + current_section.title) if header_level != 1 else '')
                             while current_section.parent is not None:
                                 current_section = current_section.parent
-                                section = current_section.title + ' > ' +  section
+                                if section != '':
+                                    section = current_section.title + ' > ' +  section
+                                else:
+                                    section = current_section.title
                             # Generate link
                             link = f'{self.file_relative_path}{page.file.src_uri}#figure-{self.counter}'
                             replacement = match.group(0)
                             if match.re.pattern == pattern_img and match.group(1):
                                 self.figures.append({"number": self.counter, "description": match.group(1), "link": link, "type": self.config.image_type_name, "section": section})
                                 replacement = f'<figure id="figure-{self.counter}" class="figure-image" markdown="span">\n  <img src="{config.site_url + match.group(2) if match.group(2).startswith("/") else match.group(2)}" alt="{match.group(1)}">\n  <figcaption>{self.config.figure_label} {self.counter} — {match.group(1)}</figcaption>\n</figure>'
                                 if self.keep_md_format:
-                                    replacement = f'<figure id="figure-{self.counter}" class="figure-image" markdown="span">\n![{match.group(1)}]({match.group(2)})\n<figcaption>{self.config.figure_label} {self.counter} — {match.group(1)}</figcaption>\n</figure>'
+                                    replacement = f'<figure id="figure-{self.counter}" class="figure-image" markdown="span">\n![{match.group(1)}]({match.group(2)}){match.group(3)}\n<figcaption>{self.config.figure_label} {self.counter} — {match.group(1)}</figcaption>\n</figure>'
                             elif (match.re.pattern == pattern_mermaid and match.group(4)) or (self.config.on_mermaid and match.re.pattern == pattern_codeblock and match.group(2) == 'mermaid' and match.group(4)):
                                 self.figures.append({"number": self.counter, "description": match.group(4), "link": link, "type": self.config.mermaid_type_name, "section": section})
                                 replacement = f'<figure id="figure-{self.counter}" class="figure-mermaid" markdown>\n{match.group(1)}\n<figcaption>{self.config.figure_label} {self.counter} — {match.group(4)}</figcaption>\n</figure>'
                             elif match.re.pattern == pattern_codeblock and match.group(2) != 'mermaid' and match.group(4):
                                 self.figures.append({"number": self.counter, "description": match.group(4), "link": link, "type": self.config.codeblock_type_name, "section": section})
                                 replacement = f'<figure id="figure-{self.counter}" class="figure-codeblock" markdown>\n{match.group(1)}\n<figcaption>{self.config.figure_label} {self.counter} — {match.group(4)}</figcaption>\n</figure>'
                             elif match.re.pattern == pattern_table and match.group(2):
```

### Comparing `mkdocs-table-of-figures-0.3.0/mkdocs_table_of_figures.egg-info/PKG-INFO` & `mkdocs-table-of-figures-0.3.1/mkdocs_table_of_figures.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-table-of-figures
-Version: 0.3.0
+Version: 0.3.1
 Summary: A MkDocs plugin listing all figures to create a table of figures page
 Home-page: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures
 Author: Thibaud Briard
 Author-email: thibaud.brrd@eduge.ch
 License: MIT
 Keywords: mkdocs
 Platform: UNKNOWN
@@ -157,14 +157,26 @@
 You can place the stylesheet in your `mkdocs.yml` at extra-css option
 
 ``` yml
 extra_css:
   - fix-mermaid-figure.css
 ```
 
+### Custom attributes
+
+To use custom attributes on images, like this :
+
+``` markdown
+![Image alt](image.png){ width="300" }
+```
+
+it require `glightbox` and `attr_list` and `md_in_html` from `mkdocs-material`. More details on `mkdocs-material` documentation : [https://squidfunk.github.io/mkdocs-material/reference/images/?h=image#image-alignment-left](https://squidfunk.github.io/mkdocs-material/reference/images/?h=image#image-alignment-left).
+
+Note that `align=left` and `align=right` attributes will be overriden by figures style from `mkdocs-material`.
+
 ## License
 
 This project is under MIT license. See the `license` file for more details.
 
 ## See Also
 
 - [GitLab Repo](http://www.gitlab.org/cfpt-mkdocs-plugins/mkdocs-table-of-figures/)
```

### Comparing `mkdocs-table-of-figures-0.3.0/readme.md` & `mkdocs-table-of-figures-0.3.1/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -138,14 +138,26 @@
 You can place the stylesheet in your `mkdocs.yml` at extra-css option
 
 ``` yml
 extra_css:
   - fix-mermaid-figure.css
 ```
 
+### Custom attributes
+
+To use custom attributes on images, like this :
+
+``` markdown
+![Image alt](image.png){ width="300" }
+```
+
+it require `glightbox` and `attr_list` and `md_in_html` from `mkdocs-material`. More details on `mkdocs-material` documentation : [https://squidfunk.github.io/mkdocs-material/reference/images/?h=image#image-alignment-left](https://squidfunk.github.io/mkdocs-material/reference/images/?h=image#image-alignment-left).
+
+Note that `align=left` and `align=right` attributes will be overriden by figures style from `mkdocs-material`.
+
 ## License
 
 This project is under MIT license. See the `license` file for more details.
 
 ## See Also
 
 - [GitLab Repo](http://www.gitlab.org/cfpt-mkdocs-plugins/mkdocs-table-of-figures/)
```

### Comparing `mkdocs-table-of-figures-0.3.0/setup.py` & `mkdocs-table-of-figures-0.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import io
 
 from setuptools import setup, find_packages
 
 setup(
     name='mkdocs-table-of-figures',
-    version='0.3.0',
+    version='0.3.1',
     description='A MkDocs plugin listing all figures to create a table of figures page',
     long_description=io.open('readme.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
     keywords='mkdocs',
     url='https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures',
     author='Thibaud Briard',
     author_email='thibaud.brrd@eduge.ch',
```

