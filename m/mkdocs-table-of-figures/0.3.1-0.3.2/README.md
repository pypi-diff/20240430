# Comparing `tmp/mkdocs-table-of-figures-0.3.1.tar.gz` & `tmp/mkdocs-table-of-figures-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-table-of-figures-0.3.1.tar", last modified: Mon Apr 29 19:01:09 2024, max compression
+gzip compressed data, was "mkdocs-table-of-figures-0.3.2.tar", last modified: Tue Apr 30 12:11:51 2024, max compression
```

## Comparing `mkdocs-table-of-figures-0.3.1.tar` & `mkdocs-table-of-figures-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 brt       (1000) brt       (1000)        0 2024-04-29 19:01:09.166821 mkdocs-table-of-figures-0.3.1/
--rwxrwxrwx   0 brt       (1000) brt       (1000)       77 2024-04-28 20:57:06.000000 mkdocs-table-of-figures-0.3.1/MANIFEST.in
--rwxrwxrwx   0 brt       (1000) brt       (1000)     7853 2024-04-29 19:01:09.165820 mkdocs-table-of-figures-0.3.1/PKG-INFO
--rwxrwxrwx   0 brt       (1000) brt       (1000)     2279 2024-04-29 18:55:38.000000 mkdocs-table-of-figures-0.3.1/changelog.md
--rwxrwxrwx   0 brt       (1000) brt       (1000)     1075 2024-04-28 20:57:06.000000 mkdocs-table-of-figures-0.3.1/license
-drwxrwxrwx   0 brt       (1000) brt       (1000)        0 2024-04-29 19:01:09.109732 mkdocs-table-of-figures-0.3.1/mkdocs_table_of_figures/
--rwxrwxrwx   0 brt       (1000) brt       (1000)        0 2024-04-28 20:57:06.000000 mkdocs-table-of-figures-0.3.1/mkdocs_table_of_figures/__init__.py
--rwxrwxrwx   0 brt       (1000) brt       (1000)    14549 2024-04-29 18:43:17.000000 mkdocs-table-of-figures-0.3.1/mkdocs_table_of_figures/plugin.py
-drwxrwxrwx   0 brt       (1000) brt       (1000)        0 2024-04-29 19:01:09.155308 mkdocs-table-of-figures-0.3.1/mkdocs_table_of_figures.egg-info/
--rwxrwxrwx   0 brt       (1000) brt       (1000)     7853 2024-04-29 19:01:08.000000 mkdocs-table-of-figures-0.3.1/mkdocs_table_of_figures.egg-info/PKG-INFO
--rwxrwxrwx   0 brt       (1000) brt       (1000)      417 2024-04-29 19:01:08.000000 mkdocs-table-of-figures-0.3.1/mkdocs_table_of_figures.egg-info/SOURCES.txt
--rwxrwxrwx   0 brt       (1000) brt       (1000)        1 2024-04-29 19:01:08.000000 mkdocs-table-of-figures-0.3.1/mkdocs_table_of_figures.egg-info/dependency_links.txt
--rwxrwxrwx   0 brt       (1000) brt       (1000)       83 2024-04-29 19:01:08.000000 mkdocs-table-of-figures-0.3.1/mkdocs_table_of_figures.egg-info/entry_points.txt
--rwxrwxrwx   0 brt       (1000) brt       (1000)       14 2024-04-29 19:01:08.000000 mkdocs-table-of-figures-0.3.1/mkdocs_table_of_figures.egg-info/requires.txt
--rwxrwxrwx   0 brt       (1000) brt       (1000)       24 2024-04-29 19:01:08.000000 mkdocs-table-of-figures-0.3.1/mkdocs_table_of_figures.egg-info/top_level.txt
--rwxrwxrwx   0 brt       (1000) brt       (1000)     7344 2024-04-29 19:00:33.000000 mkdocs-table-of-figures-0.3.1/readme.md
--rwxrwxrwx   0 brt       (1000) brt       (1000)       38 2024-04-29 19:01:09.166821 mkdocs-table-of-figures-0.3.1/setup.cfg
--rwxrwxrwx   0 brt       (1000) brt       (1000)     1135 2024-04-29 18:19:53.000000 mkdocs-table-of-figures-0.3.1/setup.py
+drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-30 12:11:51.366422 mkdocs-table-of-figures-0.3.2/
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       77 2024-04-23 06:07:49.000000 mkdocs-table-of-figures-0.3.2/MANIFEST.in
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     8699 2024-04-30 12:11:51.364421 mkdocs-table-of-figures-0.3.2/PKG-INFO
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     2351 2024-04-30 12:09:59.000000 mkdocs-table-of-figures-0.3.2/changelog.md
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1075 2024-04-23 06:07:49.000000 mkdocs-table-of-figures-0.3.2/license
+drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-30 12:11:51.276763 mkdocs-table-of-figures-0.3.2/mkdocs_table_of_figures/
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-23 06:07:49.000000 mkdocs-table-of-figures-0.3.2/mkdocs_table_of_figures/__init__.py
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)    16853 2024-04-30 12:09:52.000000 mkdocs-table-of-figures-0.3.2/mkdocs_table_of_figures/plugin.py
+drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-30 12:11:51.349274 mkdocs-table-of-figures-0.3.2/mkdocs_table_of_figures.egg-info/
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     8699 2024-04-30 12:11:50.000000 mkdocs-table-of-figures-0.3.2/mkdocs_table_of_figures.egg-info/PKG-INFO
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)      417 2024-04-30 12:11:50.000000 mkdocs-table-of-figures-0.3.2/mkdocs_table_of_figures.egg-info/SOURCES.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        1 2024-04-30 12:11:50.000000 mkdocs-table-of-figures-0.3.2/mkdocs_table_of_figures.egg-info/dependency_links.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       83 2024-04-30 12:11:50.000000 mkdocs-table-of-figures-0.3.2/mkdocs_table_of_figures.egg-info/entry_points.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       14 2024-04-30 12:11:50.000000 mkdocs-table-of-figures-0.3.2/mkdocs_table_of_figures.egg-info/requires.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       24 2024-04-30 12:11:50.000000 mkdocs-table-of-figures-0.3.2/mkdocs_table_of_figures.egg-info/top_level.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     8212 2024-04-30 12:11:19.000000 mkdocs-table-of-figures-0.3.2/readme.md
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       38 2024-04-30 12:11:51.367420 mkdocs-table-of-figures-0.3.2/setup.cfg
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1135 2024-04-30 11:14:41.000000 mkdocs-table-of-figures-0.3.2/setup.py
```

### Comparing `mkdocs-table-of-figures-0.3.1/PKG-INFO` & `mkdocs-table-of-figures-0.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-table-of-figures
-Version: 0.3.1
+Version: 0.3.2
 Summary: A MkDocs plugin listing all figures to create a table of figures page
 Home-page: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures
 Author: Thibaud Briard
 Author-email: thibaud.brrd@eduge.ch
 License: MIT
 Keywords: mkdocs
 Platform: UNKNOWN
@@ -41,22 +41,24 @@
       section_label: "Section of the figure" # Optional --> Default : Section
 
       temp_dir: "folder_name" # Optional --> Default : temp_figures
       file: "file_name" # Optional --> Default : figures.md
 
       follow_nav_structure: true # Optional --> Default : true
       
+      on_pair: true # Optional --> Default : false
       on_mermaid: true # Optional --> Default : false
       on_codeblock: true # Optional --> Default : false
       on_table: true # Optional --> Default : false
 
       show_type: true # Optional --> Default : false
       show_section: true # Optional --> Default : false
 
       image_type_name: Image Figure # Optional --> Default : Image
+      pair_type_name: Pair of Images Figure # Optional --> Default : Pair
       mermaid_type_name: Mermaid Figure # Optional --> Default : Mermaid
       codeblock_type_name: Codeblock Figure # Optional --> Default : Codeblock
       table_type_name: Table Figure # Optional --> Default : Table
 ```
 
 As you can see, every option is optional, but if you want to generate a table of figures in another language than English, you will need to set up label options.
 
@@ -64,20 +66,22 @@
 - `figure_label` - This is the name given to every figure right before the auto-incremented number.
 - `description_label` - This is the label given to the column containing the description of each figure (alt text).
 - `type_label` - This is the label given to the cloumn containing the type of each figure (image, mermaid, codeblock, table).
 - `section_label` - This is the label given to the cloumn containing the section of each figure (the location relative to headings and pages navigation).
 - `temp_dir` - The temporary directory used to store the table of figures `Markdown` file before rendering to HTML. Only set this option if you already have a `temp_figures` folder in the root directory (same as `mkdocs.yml`), which you should not normally have.
 - `file` - The name of the `Markdown` file containing the table of figures. Only set this option if you already have a `figures.md` file in the `docs` directory.
 - `follow_nav_structure` - To order the figures in function of the navigation instead of alphabetical files order.
+- `on_pair` - To enable pair of image support, to use when 2 comparative image need to be next to each others.
 - `on_mermaid` - To enable `mermaid` diagrams support, need to use of `md_in_html` `Markdown` extension.
 - `on_codeblock` - To enable code blocks support, need to use of `md_in_html` `Markdown` extension.
 - `on_table` - To enable tables support, need to use of `md_in_html` `Markdown` extension.
 - `show_type` - To enable the column showing info about the type of each figure (image, mermaid, codeblock, table).
 - `show_section` - To enable the column showing info about the section of each figure (the location relative to headings and pages navigation)
 - `image_type_name` - The label shown for each figure of type image
+- `pair_type_name` - The label shown for each figure of type pair of image
 - `mermaid_type_name` - The label shown for each figure of type mermaid
 - `codeblock_type_name` - The label shown for each figure of type codeblock
 - `table_type_name` - The label shown for each figure of type table
 
 ## Usage
 
 The plugin will only look for `Markdown` image composed of alt text. If you don't set any alt text for the `Markdown` image it will be ignored.
@@ -96,15 +100,33 @@
   - md_in_html
 ```
 
 Using the command `mkdocs build` or `mkdocs serve` will trigger the plugin if it has been set correctly in the config file.
 
 ## Support
 
-This plugin currently supports markdown images, `mermaid` diagrams, code blocks and table.
+### Image like support
+
+This plugin currently supports markdown images, pairs of images, `mermaid` diagrams, code blocks and table.
+
+To make a pair of image you need to follow this structure:
+
+``` markdown
+| ![Version A](./image_a.png) | ![Version B](./image_a.png) |
+```
+
+There is no need to put any alt text for the second image. it will then generate a single description for the two image:
+
+``` markdown
+| ![Two versions of an image](./image_a.png) | ![](./image_a.png) |
+```
+
+To make it work space are needed between the images and the table separator `|`
+
+### Non-image like support
 
 To make a `mermaid` diagram, code block or table detectable by this plugin, you need to give it a title at the line just below it like this:
 
 ``` markdown
     ``` php
     <?php
       $var = 42;
@@ -140,17 +162,17 @@
 It will not work if there is a line between the element and the title.
 
 I highly recommend using `mkdocs-material` to use `mermaid` diagrams. For more info about `mermaid` diagrams, I invite you to check `mkdocs-material` and `mermaid`'s official documentation.
 
 I also recommend to add this stylesheet to prevent mermaid size from being reduced or code blocks from having code centered by mkdocs-material.
 
 ``` css
-figure.figure-mermaid {
+figure.figure-mermaid, figure.figure-codeblock {
     margin: 0 1em;
-    width: 100%;
+    width: calc(100% - 2em);
 }
 
 figure.figure-codeblock code {
     text-align: initial;
 }
 ```
```

### Comparing `mkdocs-table-of-figures-0.3.1/changelog.md` & `mkdocs-table-of-figures-0.3.2/changelog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on Keep a Changelog, and this project adheres to Semantic Versioning.
 
+## [0.3.2] - 2024-04-30
+
+### Added
+
+- support for pair of images
+
 ## [0.3.1] - 2024-04-29
 
 ### Added
 
 - support for custom attribute on image using `glightbox` and `mkdocs-material` plugins with `attr_list` and `md_in_html` enable
 
 ### Fixed
```

### Comparing `mkdocs-table-of-figures-0.3.1/license` & `mkdocs-table-of-figures-0.3.2/license`

 * *Files identical despite different names*

### Comparing `mkdocs-table-of-figures-0.3.1/mkdocs_table_of_figures/plugin.py` & `mkdocs-table-of-figures-0.3.2/mkdocs_table_of_figures/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,23 +21,26 @@
     file = c.Type(str, default='figures.md')
     title_label = c.Type(str, default='Table of Figures')
     figure_label = c.Type(str, default='Figure')
     description_label = c.Type(str, default='Description')
     type_label = c.Type(str, default='Type')
     section_label = c.Type(str, default='Section')
     follow_nav_structure = c.Type(bool, default=True)
+    on_pair = c.Type(bool, default=False)
     on_mermaid = c.Type(bool, default=False)
     on_codeblock = c.Type(bool, default=False)
     on_table = c.Type(bool, default=False)
     show_type = c.Type(bool, default=False)
     image_type_name = c.Type(str, default='Image')
+    pair_type_name = c.Type(str, default='Pair')
     mermaid_type_name = c.Type(str, default='Mermaid')
     codeblock_type_name = c.Type(str, default='Codeblock')
     table_type_name = c.Type(str, default='Table')
     show_section = c.Type(bool, default=False)
+    show_pair_description_arrows = c.Type(bool, default=False)
 
 # The plugin itself
 class TableOfFigures(base_plugin[TableOfFiguresConfig]):
     def __init__(self):
         self._logger = logging.getLogger('mkdocs.table-of-figures')
         self._logger.setLevel(logging.INFO)
 
@@ -47,15 +50,14 @@
         self.counter = 1
         self.figures = []
         self.file_directories_count = 0
         self.file_relative_path = ''
         self.page = None
         self.nav_structure = None
         self.docs_dir = None
-        #self.mermaid_dir ='assets/mermaids/'
         self.keep_md_format = False
         self.listening = True
 
     def on_config(self, config):
         self.file_directories_count = self.config.file.count('/')
         self.file_relative_path = '../' * self.file_directories_count
         self.docs_dir = config.docs_dir
@@ -96,60 +98,68 @@
             if nav_item.is_page:
                 if nav_item == page:
                     found = True
                 elif os.path.exists(os.path.join(self.docs_dir, nav_item.file.src_uri)):
                     with open(os.path.join(self.docs_dir, nav_item.file.src_uri), 'r', errors='ignore') as file:
                         markdown = file.read()
 
-                    pattern_img = r'!\[([^\]]+?)\]\((.+?)\)'
+                    pattern_img = r'(?<!\| )!\[([^\]]+?)\]\((.+?)\)'
+                    pattern_pair = r'\| ?!\[([^\]]+?)\]\((.+?)\)(\{.*\})? ?\| ?!\[(.*?)\]\((.+?)\)(\{.*\})? ? \|'
                     pattern_mermaid = r'^(``` ?(mermaid)\r?\n(.*?)```)$\r?\n^([^\n]+?)$'
                     pattern_codeblock = r'^(``` ?([^\r\n]*)\r?\n(.*?)```)$\r?\n^([^\n]+?)$'
                     pattern_table = r'^((?:\|[^|\r\n]*)+\|\r?\n(?:\|[-: ]*)+\|(?:\r?\n(?:\|[^|\r\n]*)+\|)*)\r?\n^([^|\n]+?)$'
                     
                     matches = []
                     matches.extend(re.finditer(pattern_img, markdown, flags= re.IGNORECASE))
+                    matches.extend(re.finditer(pattern_pair, markdown, flags= re.IGNORECASE))
                     matches.extend(re.finditer(pattern_mermaid, markdown, flags= re.MULTILINE | re.DOTALL)) if self.config.on_mermaid and not self.config.on_codeblock else None
                     matches.extend(re.finditer(pattern_codeblock, markdown, flags= re.MULTILINE | re.DOTALL)) if self.config.on_codeblock else None
                     matches.extend(re.finditer(pattern_table, markdown, flags= re.MULTILINE | re.DOTALL)) if self.config.on_table else None
+                    
+                    pair_pattern = sum(1 for match in matches if match.re.pattern == pattern_pair)
+                    addon = len(matches) + pair_pattern
+
 
-                    addon = len(matches)
             elif nav_item.is_section:
                 found, addon = self.count_previous_figures(page, nav_item.children, depth + 1)
             
             counter += addon
             if found:
                 break
         return found, counter
 
     def on_page_markdown(self, markdown, page, config, files):
         if self.listening:
             if self.page == page.file:
                 self._logger.info(f'Populating table of figure file {self.config.file} with {len(self.figures)} figure{"s" if self.counter else ""} ')
                 markdown += f'| {self.config.figure_label} |{" " + self.config.type_label + " |" if self.config.show_type else ""} {self.config.description_label} |{" " + self.config.section_label + " |" if self.config.show_section else ""}\n'
                 markdown += f'| -------------------------- |{" :-------------------------------: |" if self.config.show_type else ""} ------------------------------- |{" ------------------------------- |" if self.config.show_section else ""}\n'
-                figures = sorted(self.figures, key=lambda figure: figure["number"])
+                figures = sorted(self.figures, key=lambda figure: figure["number"][0] if isinstance(figure["number"], list) else figure["number"])
                 for figure in figures:
-                    markdown += f'| [{self.config.figure_label} {figure["number"]}]({figure["link"]}) |{" **" + figure["type"] + "** |" if self.config.show_type else ""} {figure["description"]} |{" `" + figure["section"]  + "` |" if self.config.show_section else ""}\n'
+                    number = f'{figure["number"][0]} & {figure["number"][1]}' if isinstance(figure["number"], list) else f'{figure["number"]}'
+                    markdown += f'| [{self.config.figure_label} {number}]({figure["link"]}) |{" **" + figure["type"] + "** |" if self.config.show_type else ""} {figure["description"]} |{" `" + figure["section"]  + "` |" if self.config.show_section else ""}\n'
                 
                 self.listening = False
             else:
                 if self.config.follow_nav_structure and self.nav_structure:
                     found, counter = self.count_previous_figures(page, self.nav_structure)
                     if found:
                         self.counter = counter + 1
 
                 original = markdown
                 try:
-                    pattern_img = r'!\[(.*?)\]\((.+?)\)(.*)'
+                    pattern_img = r'(?<!\| )!\[(.*?)\]\((.+?)\)({.*})?'
+                    pattern_pair = r'\| ?!\[(.*?)\]\((.+?)\)(\{.*\})? ?\| ?!\[(.*?)\]\((.+?)\)(\{.*\})? ? \|'
                     pattern_mermaid = r'^(``` ?(mermaid)\r?\n(.*?)```)$\r?\n^(.*?)$'
                     pattern_codeblock = r'^(``` ?([^\r\n]*)\r?\n(.*?)```)$\r?\n^(.*?)$'
                     pattern_table = r'^((?:\|[^|\r\n]*)+\|\r?\n(?:\|[-: ]*)+\|(?:\r?\n(?:\|[^|\r\n]*)+\|)*)\r?\n^([^|]*?)$'
                     
                     matches = []
                     matches.extend(re.finditer(pattern_img, markdown, flags= re.IGNORECASE))
+                    matches.extend(re.finditer(pattern_pair, markdown, flags= re.IGNORECASE)) if self.config.on_pair else None
                     matches.extend(re.finditer(pattern_mermaid, markdown, flags= re.MULTILINE | re.DOTALL)) if self.config.on_mermaid and not self.config.on_codeblock else None
                     matches.extend(re.finditer(pattern_codeblock, markdown, flags= re.MULTILINE | re.DOTALL)) if self.config.on_codeblock else None
                     matches.extend(re.finditer(pattern_table, markdown, flags= re.MULTILINE | re.DOTALL)) if self.config.on_table else None
                     matches = sorted(matches, key=lambda x: x.start())
 
                     position_offset = 0
                     for match in matches:
@@ -190,30 +200,34 @@
                             # Generate link
                             link = f'{self.file_relative_path}{page.file.src_uri}#figure-{self.counter}'
                             replacement = match.group(0)
                             if match.re.pattern == pattern_img and match.group(1):
                                 self.figures.append({"number": self.counter, "description": match.group(1), "link": link, "type": self.config.image_type_name, "section": section})
                                 replacement = f'<figure id="figure-{self.counter}" class="figure-image" markdown="span">\n  <img src="{config.site_url + match.group(2) if match.group(2).startswith("/") else match.group(2)}" alt="{match.group(1)}">\n  <figcaption>{self.config.figure_label} {self.counter} — {match.group(1)}</figcaption>\n</figure>'
                                 if self.keep_md_format:
-                                    replacement = f'<figure id="figure-{self.counter}" class="figure-image" markdown="span">\n![{match.group(1)}]({match.group(2)}){match.group(3)}\n<figcaption>{self.config.figure_label} {self.counter} — {match.group(1)}</figcaption>\n</figure>'
+                                    replacement = f'<figure id="figure-{self.counter}" class="figure-image" markdown="span">\n![{match.group(1)}]({match.group(2)}){match.group(3) if match.group(3) else ""}\n<figcaption>{self.config.figure_label} {self.counter} — {match.group(1)}</figcaption>\n</figure>'
+                            elif match.re.pattern == pattern_pair and match.group(1):
+                                link += f'-{self.counter + 1}'
+                                self.figures.append({"number": [self.counter, self.counter + 1], "description": f'{"← " if self.config.show_pair_description_arrows else ""}{match.group(1)}</br>{"→ " if self.config.show_pair_description_arrows else ""}{match.group(4)}' if match.group(4) else match.group(1), "link": link, "type": self.config.pair_type_name, "section": section})
+                                replacement = f'<figure id="figure-{self.counter}-{self.counter + 1}" class="figure-image" markdown>\n<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 1em;" markdown>\n<div style="display: flex; justify-content: flex-end; align-items: center;" markdown="span">\n![{match.group(1)}]({match.group(2)}){match.group(3) if match.group(3) else ""}\n</div>\n<div style="display: flex; justify-content: flex-start; align-items: center;" markdown="span">\n![{match.group(4)}]({match.group(5)}){match.group(6) if match.group(6) else ""}\n</div>\n</div>\n<figcaption>{self.config.figure_label} {self.counter} & {self.counter + 1} — {match.group(1)}{(" <span>|</span> " + match.group(4)) if match.group(4) else ""}</figcaption>\n</figure>'
                             elif (match.re.pattern == pattern_mermaid and match.group(4)) or (self.config.on_mermaid and match.re.pattern == pattern_codeblock and match.group(2) == 'mermaid' and match.group(4)):
                                 self.figures.append({"number": self.counter, "description": match.group(4), "link": link, "type": self.config.mermaid_type_name, "section": section})
                                 replacement = f'<figure id="figure-{self.counter}" class="figure-mermaid" markdown>\n{match.group(1)}\n<figcaption>{self.config.figure_label} {self.counter} — {match.group(4)}</figcaption>\n</figure>'
                             elif match.re.pattern == pattern_codeblock and match.group(2) != 'mermaid' and match.group(4):
                                 self.figures.append({"number": self.counter, "description": match.group(4), "link": link, "type": self.config.codeblock_type_name, "section": section})
                                 replacement = f'<figure id="figure-{self.counter}" class="figure-codeblock" markdown>\n{match.group(1)}\n<figcaption>{self.config.figure_label} {self.counter} — {match.group(4)}</figcaption>\n</figure>'
                             elif match.re.pattern == pattern_table and match.group(2):
                                 self.figures.append({"number": self.counter, "description": match.group(2), "link": link, "type": self.config.table_type_name, "section": section})
                                 replacement = f'<figure id="figure-{self.counter}" class="figure-table" markdown>\n{match.group(1)}\n<figcaption>{self.config.figure_label} {self.counter} — {match.group(2)}</figcaption>\n</figure>'
                             
                             if replacement == match.group(0):
                                 self._logger.debug(f'Ignoring image/diagram at {self.file_relative_path}{page.file.src_uri}')
                             else:
                                 self._logger.debug(f'Formating image/diagram as figure at {self.file_relative_path}{page.file.src_uri}')
-                                self.counter += 1
+                                self.counter += (2 if match.re.pattern == pattern_pair else 1)
                                 markdown = markdown[:match.start() + position_offset] + replacement + markdown[match.end() + position_offset:]
                                 position_offset += len(replacement) - len(match.group(0))
                         except Exception as error:
                             self._logger.warning(error)
                             markdown = checkpoint
                             
                 except Exception as error:
```

### Comparing `mkdocs-table-of-figures-0.3.1/mkdocs_table_of_figures.egg-info/PKG-INFO` & `mkdocs-table-of-figures-0.3.2/mkdocs_table_of_figures.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-table-of-figures
-Version: 0.3.1
+Version: 0.3.2
 Summary: A MkDocs plugin listing all figures to create a table of figures page
 Home-page: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures
 Author: Thibaud Briard
 Author-email: thibaud.brrd@eduge.ch
 License: MIT
 Keywords: mkdocs
 Platform: UNKNOWN
@@ -41,22 +41,24 @@
       section_label: "Section of the figure" # Optional --> Default : Section
 
       temp_dir: "folder_name" # Optional --> Default : temp_figures
       file: "file_name" # Optional --> Default : figures.md
 
       follow_nav_structure: true # Optional --> Default : true
       
+      on_pair: true # Optional --> Default : false
       on_mermaid: true # Optional --> Default : false
       on_codeblock: true # Optional --> Default : false
       on_table: true # Optional --> Default : false
 
       show_type: true # Optional --> Default : false
       show_section: true # Optional --> Default : false
 
       image_type_name: Image Figure # Optional --> Default : Image
+      pair_type_name: Pair of Images Figure # Optional --> Default : Pair
       mermaid_type_name: Mermaid Figure # Optional --> Default : Mermaid
       codeblock_type_name: Codeblock Figure # Optional --> Default : Codeblock
       table_type_name: Table Figure # Optional --> Default : Table
 ```
 
 As you can see, every option is optional, but if you want to generate a table of figures in another language than English, you will need to set up label options.
 
@@ -64,20 +66,22 @@
 - `figure_label` - This is the name given to every figure right before the auto-incremented number.
 - `description_label` - This is the label given to the column containing the description of each figure (alt text).
 - `type_label` - This is the label given to the cloumn containing the type of each figure (image, mermaid, codeblock, table).
 - `section_label` - This is the label given to the cloumn containing the section of each figure (the location relative to headings and pages navigation).
 - `temp_dir` - The temporary directory used to store the table of figures `Markdown` file before rendering to HTML. Only set this option if you already have a `temp_figures` folder in the root directory (same as `mkdocs.yml`), which you should not normally have.
 - `file` - The name of the `Markdown` file containing the table of figures. Only set this option if you already have a `figures.md` file in the `docs` directory.
 - `follow_nav_structure` - To order the figures in function of the navigation instead of alphabetical files order.
+- `on_pair` - To enable pair of image support, to use when 2 comparative image need to be next to each others.
 - `on_mermaid` - To enable `mermaid` diagrams support, need to use of `md_in_html` `Markdown` extension.
 - `on_codeblock` - To enable code blocks support, need to use of `md_in_html` `Markdown` extension.
 - `on_table` - To enable tables support, need to use of `md_in_html` `Markdown` extension.
 - `show_type` - To enable the column showing info about the type of each figure (image, mermaid, codeblock, table).
 - `show_section` - To enable the column showing info about the section of each figure (the location relative to headings and pages navigation)
 - `image_type_name` - The label shown for each figure of type image
+- `pair_type_name` - The label shown for each figure of type pair of image
 - `mermaid_type_name` - The label shown for each figure of type mermaid
 - `codeblock_type_name` - The label shown for each figure of type codeblock
 - `table_type_name` - The label shown for each figure of type table
 
 ## Usage
 
 The plugin will only look for `Markdown` image composed of alt text. If you don't set any alt text for the `Markdown` image it will be ignored.
@@ -96,15 +100,33 @@
   - md_in_html
 ```
 
 Using the command `mkdocs build` or `mkdocs serve` will trigger the plugin if it has been set correctly in the config file.
 
 ## Support
 
-This plugin currently supports markdown images, `mermaid` diagrams, code blocks and table.
+### Image like support
+
+This plugin currently supports markdown images, pairs of images, `mermaid` diagrams, code blocks and table.
+
+To make a pair of image you need to follow this structure:
+
+``` markdown
+| ![Version A](./image_a.png) | ![Version B](./image_a.png) |
+```
+
+There is no need to put any alt text for the second image. it will then generate a single description for the two image:
+
+``` markdown
+| ![Two versions of an image](./image_a.png) | ![](./image_a.png) |
+```
+
+To make it work space are needed between the images and the table separator `|`
+
+### Non-image like support
 
 To make a `mermaid` diagram, code block or table detectable by this plugin, you need to give it a title at the line just below it like this:
 
 ``` markdown
     ``` php
     <?php
       $var = 42;
@@ -140,17 +162,17 @@
 It will not work if there is a line between the element and the title.
 
 I highly recommend using `mkdocs-material` to use `mermaid` diagrams. For more info about `mermaid` diagrams, I invite you to check `mkdocs-material` and `mermaid`'s official documentation.
 
 I also recommend to add this stylesheet to prevent mermaid size from being reduced or code blocks from having code centered by mkdocs-material.
 
 ``` css
-figure.figure-mermaid {
+figure.figure-mermaid, figure.figure-codeblock {
     margin: 0 1em;
-    width: 100%;
+    width: calc(100% - 2em);
 }
 
 figure.figure-codeblock code {
     text-align: initial;
 }
 ```
```

### Comparing `mkdocs-table-of-figures-0.3.1/readme.md` & `mkdocs-table-of-figures-0.3.2/readme.md`

 * *Files 14% similar despite different names*

```diff
@@ -22,22 +22,24 @@
       section_label: "Section of the figure" # Optional --> Default : Section
 
       temp_dir: "folder_name" # Optional --> Default : temp_figures
       file: "file_name" # Optional --> Default : figures.md
 
       follow_nav_structure: true # Optional --> Default : true
       
+      on_pair: true # Optional --> Default : false
       on_mermaid: true # Optional --> Default : false
       on_codeblock: true # Optional --> Default : false
       on_table: true # Optional --> Default : false
 
       show_type: true # Optional --> Default : false
       show_section: true # Optional --> Default : false
 
       image_type_name: Image Figure # Optional --> Default : Image
+      pair_type_name: Pair of Images Figure # Optional --> Default : Pair
       mermaid_type_name: Mermaid Figure # Optional --> Default : Mermaid
       codeblock_type_name: Codeblock Figure # Optional --> Default : Codeblock
       table_type_name: Table Figure # Optional --> Default : Table
 ```
 
 As you can see, every option is optional, but if you want to generate a table of figures in another language than English, you will need to set up label options.
 
@@ -45,20 +47,22 @@
 - `figure_label` - This is the name given to every figure right before the auto-incremented number.
 - `description_label` - This is the label given to the column containing the description of each figure (alt text).
 - `type_label` - This is the label given to the cloumn containing the type of each figure (image, mermaid, codeblock, table).
 - `section_label` - This is the label given to the cloumn containing the section of each figure (the location relative to headings and pages navigation).
 - `temp_dir` - The temporary directory used to store the table of figures `Markdown` file before rendering to HTML. Only set this option if you already have a `temp_figures` folder in the root directory (same as `mkdocs.yml`), which you should not normally have.
 - `file` - The name of the `Markdown` file containing the table of figures. Only set this option if you already have a `figures.md` file in the `docs` directory.
 - `follow_nav_structure` - To order the figures in function of the navigation instead of alphabetical files order.
+- `on_pair` - To enable pair of image support, to use when 2 comparative image need to be next to each others.
 - `on_mermaid` - To enable `mermaid` diagrams support, need to use of `md_in_html` `Markdown` extension.
 - `on_codeblock` - To enable code blocks support, need to use of `md_in_html` `Markdown` extension.
 - `on_table` - To enable tables support, need to use of `md_in_html` `Markdown` extension.
 - `show_type` - To enable the column showing info about the type of each figure (image, mermaid, codeblock, table).
 - `show_section` - To enable the column showing info about the section of each figure (the location relative to headings and pages navigation)
 - `image_type_name` - The label shown for each figure of type image
+- `pair_type_name` - The label shown for each figure of type pair of image
 - `mermaid_type_name` - The label shown for each figure of type mermaid
 - `codeblock_type_name` - The label shown for each figure of type codeblock
 - `table_type_name` - The label shown for each figure of type table
 
 ## Usage
 
 The plugin will only look for `Markdown` image composed of alt text. If you don't set any alt text for the `Markdown` image it will be ignored.
@@ -77,15 +81,33 @@
   - md_in_html
 ```
 
 Using the command `mkdocs build` or `mkdocs serve` will trigger the plugin if it has been set correctly in the config file.
 
 ## Support
 
-This plugin currently supports markdown images, `mermaid` diagrams, code blocks and table.
+### Image like support
+
+This plugin currently supports markdown images, pairs of images, `mermaid` diagrams, code blocks and table.
+
+To make a pair of image you need to follow this structure:
+
+``` markdown
+| ![Version A](./image_a.png) | ![Version B](./image_a.png) |
+```
+
+There is no need to put any alt text for the second image. it will then generate a single description for the two image:
+
+``` markdown
+| ![Two versions of an image](./image_a.png) | ![](./image_a.png) |
+```
+
+To make it work space are needed between the images and the table separator `|`
+
+### Non-image like support
 
 To make a `mermaid` diagram, code block or table detectable by this plugin, you need to give it a title at the line just below it like this:
 
 ``` markdown
     ``` php
     <?php
       $var = 42;
@@ -121,17 +143,17 @@
 It will not work if there is a line between the element and the title.
 
 I highly recommend using `mkdocs-material` to use `mermaid` diagrams. For more info about `mermaid` diagrams, I invite you to check `mkdocs-material` and `mermaid`'s official documentation.
 
 I also recommend to add this stylesheet to prevent mermaid size from being reduced or code blocks from having code centered by mkdocs-material.
 
 ``` css
-figure.figure-mermaid {
+figure.figure-mermaid, figure.figure-codeblock {
     margin: 0 1em;
-    width: 100%;
+    width: calc(100% - 2em);
 }
 
 figure.figure-codeblock code {
     text-align: initial;
 }
 ```
```

### Comparing `mkdocs-table-of-figures-0.3.1/setup.py` & `mkdocs-table-of-figures-0.3.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import io
 
 from setuptools import setup, find_packages
 
 setup(
     name='mkdocs-table-of-figures',
-    version='0.3.1',
+    version='0.3.2',
     description='A MkDocs plugin listing all figures to create a table of figures page',
     long_description=io.open('readme.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
     keywords='mkdocs',
     url='https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures',
     author='Thibaud Briard',
     author_email='thibaud.brrd@eduge.ch',
```

