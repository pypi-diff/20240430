# Comparing `tmp/phylo-match-0.0.9.tar.gz` & `tmp/phylo_match-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phylo-match-0.0.9.tar", last modified: Thu Jun 23 17:18:51 2022, max compression
+gzip compressed data, was "phylo_match-0.1.0.tar", last modified: Mon Apr 29 18:40:53 2024, max compression
```

## Comparing `phylo-match-0.0.9.tar` & `phylo_match-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 williamspear   (501) staff       (20)        0 2022-06-23 17:18:51.281198 phylo-match-0.0.9/
--rw-r--r--   0 williamspear   (501) staff       (20)    32474 2022-06-23 17:16:36.000000 phylo-match-0.0.9/COPYING
--rw-r--r--   0 williamspear   (501) staff       (20)     3801 2022-06-23 17:18:51.281273 phylo-match-0.0.9/PKG-INFO
--rw-r--r--   0 williamspear   (501) staff       (20)     3335 2022-06-23 17:17:21.000000 phylo-match-0.0.9/README.md
-drwxr-xr-x   0 williamspear   (501) staff       (20)        0 2022-06-23 17:18:51.280650 phylo-match-0.0.9/phylo_match.egg-info/
--rw-r--r--   0 williamspear   (501) staff       (20)     3801 2022-06-23 17:18:51.000000 phylo-match-0.0.9/phylo_match.egg-info/PKG-INFO
--rw-r--r--   0 williamspear   (501) staff       (20)      341 2022-06-23 17:18:51.000000 phylo-match-0.0.9/phylo_match.egg-info/SOURCES.txt
--rw-r--r--   0 williamspear   (501) staff       (20)        1 2022-06-23 17:18:51.000000 phylo-match-0.0.9/phylo_match.egg-info/dependency_links.txt
--rw-r--r--   0 williamspear   (501) staff       (20)       52 2022-06-23 17:18:51.000000 phylo-match-0.0.9/phylo_match.egg-info/entry_points.txt
--rw-r--r--   0 williamspear   (501) staff       (20)       47 2022-06-23 17:18:51.000000 phylo-match-0.0.9/phylo_match.egg-info/requires.txt
--rw-r--r--   0 williamspear   (501) staff       (20)        1 2022-06-23 17:18:51.000000 phylo-match-0.0.9/phylo_match.egg-info/top_level.txt
--rw-r--r--   0 williamspear   (501) staff       (20)      213 2022-06-23 17:16:36.000000 phylo-match-0.0.9/pyproject.toml
--rw-r--r--   0 williamspear   (501) staff       (20)      704 2022-06-23 17:18:51.281591 phylo-match-0.0.9/setup.cfg
-drwxr-xr-x   0 williamspear   (501) staff       (20)        0 2022-06-23 17:18:51.279419 phylo-match-0.0.9/src/
-drwxr-xr-x   0 williamspear   (501) staff       (20)        0 2022-06-23 17:18:51.281099 phylo-match-0.0.9/src/python/
--rw-r--r--   0 williamspear   (501) staff       (20)        0 2022-06-23 17:16:36.000000 phylo-match-0.0.9/src/python/__init__.py
--rw-r--r--   0 williamspear   (501) staff       (20)     1065 2022-06-23 17:16:36.000000 phylo-match-0.0.9/src/python/definitions.py
--rw-r--r--   0 williamspear   (501) staff       (20)    24653 2022-06-23 17:16:36.000000 phylo-match-0.0.9/src/python/gui.py
--rw-r--r--   0 williamspear   (501) staff       (20)     8340 2022-06-23 17:16:36.000000 phylo-match-0.0.9/src/python/match.py
+drwxr-xr-x   0 williamspear   (501) staff       (20)        0 2024-04-29 18:40:53.169985 phylo_match-0.1.0/
+-rw-r--r--   0 williamspear   (501) staff       (20)    32474 2022-06-23 17:16:36.000000 phylo_match-0.1.0/COPYING
+-rw-r--r--   0 williamspear   (501) staff       (20)     4714 2024-04-29 18:40:53.169910 phylo_match-0.1.0/PKG-INFO
+-rw-r--r--   0 williamspear   (501) staff       (20)     4126 2024-04-29 18:38:43.000000 phylo_match-0.1.0/README.md
+drwxr-xr-x   0 williamspear   (501) staff       (20)        0 2024-04-29 18:40:53.167660 phylo_match-0.1.0/phylo_match/
+-rw-r--r--   0 williamspear   (501) staff       (20)        0 2024-04-28 04:50:14.000000 phylo_match-0.1.0/phylo_match/__init__.py
+drwxr-xr-x   0 williamspear   (501) staff       (20)        0 2024-04-29 18:40:53.169020 phylo_match-0.1.0/phylo_match/definitions/
+-rw-r--r--   0 williamspear   (501) staff       (20)        0 2022-06-23 17:16:36.000000 phylo_match-0.1.0/phylo_match/definitions/__init__.py
+-rw-r--r--   0 williamspear   (501) staff       (20)     1065 2022-06-23 17:16:36.000000 phylo_match-0.1.0/phylo_match/definitions/definitions.py
+-rw-r--r--   0 williamspear   (501) staff       (20)    27936 2024-04-29 18:26:17.000000 phylo_match-0.1.0/phylo_match/gui.py
+drwxr-xr-x   0 williamspear   (501) staff       (20)        0 2024-04-29 18:40:53.169391 phylo_match-0.1.0/phylo_match/match/
+-rw-r--r--   0 williamspear   (501) staff       (20)        0 2024-04-28 04:50:14.000000 phylo_match-0.1.0/phylo_match/match/__init__.py
+-rw-r--r--   0 williamspear   (501) staff       (20)     8622 2024-04-29 18:19:49.000000 phylo_match-0.1.0/phylo_match/match/match.py
+drwxr-xr-x   0 williamspear   (501) staff       (20)        0 2024-04-29 18:40:53.169702 phylo_match-0.1.0/phylo_match.egg-info/
+-rw-r--r--   0 williamspear   (501) staff       (20)     4714 2024-04-29 18:40:53.000000 phylo_match-0.1.0/phylo_match.egg-info/PKG-INFO
+-rw-r--r--   0 williamspear   (501) staff       (20)      429 2024-04-29 18:40:53.000000 phylo_match-0.1.0/phylo_match.egg-info/SOURCES.txt
+-rw-r--r--   0 williamspear   (501) staff       (20)        1 2024-04-29 18:40:53.000000 phylo_match-0.1.0/phylo_match.egg-info/dependency_links.txt
+-rw-r--r--   0 williamspear   (501) staff       (20)       53 2024-04-29 18:40:53.000000 phylo_match-0.1.0/phylo_match.egg-info/entry_points.txt
+-rw-r--r--   0 williamspear   (501) staff       (20)       47 2024-04-29 18:40:53.000000 phylo_match-0.1.0/phylo_match.egg-info/requires.txt
+-rw-r--r--   0 williamspear   (501) staff       (20)       12 2024-04-29 18:40:53.000000 phylo_match-0.1.0/phylo_match.egg-info/top_level.txt
+-rw-r--r--   0 williamspear   (501) staff       (20)      213 2022-06-23 17:16:36.000000 phylo_match-0.1.0/pyproject.toml
+-rw-r--r--   0 williamspear   (501) staff       (20)      705 2024-04-29 18:40:53.170257 phylo_match-0.1.0/setup.cfg
```

### Comparing `phylo-match-0.0.9/COPYING` & `phylo_match-0.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `phylo-match-0.0.9/PKG-INFO` & `phylo_match-0.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: phylo-match
-Version: 0.0.9
-Summary: For matching species databases
-Home-page: https://github.com/spearw/phylo-match
-Author: William Spear
-Author-email: spearw@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: COPYING
-
 # Phylo-Match
 
 Phylo-Match is a package for correcting misspellings or disparate labelings in phylogenetic trees
 
 ## Installation
 
 This project was built with python v3.8 (python3). Later versions should be fine, but no guarantees for earlier. Not compatible with python 2.
@@ -40,44 +26,59 @@
 ```
 
 Install Phylo-Match:
 ```bash
 pip3 install phylo-match
 ```
 
+
 ## Usage
 
 ```bash
 phylo-match
 ```
-Use the gui to select a database file (.csv), and a taxa tree (.nexus) to match the database to. Click run when you are happy with your selection.
+Use the gui to select a database file (.csv), and a taxa tree (.nexus) to match the database to. Enter the number of your species column in the box, if the taxa you are matching are not in the first column (index counts from 0, so enter 0 for first column, 1 for second, etc.)
+
+Click run when you are happy with your selection.
 
-*Phylo-Match does all of its calculations and api requests upfront, so users may have to wait 10-15 minutes after run is clicked, depending on internet speed.*
+*Phylo-Match does all of its calculations and api requests upfront, so users may have to wait 10-15 minutes after run is clicked, depending on internet speed and whether these taxa are already in their local cache.*
 
 *This time can be minimized by unchecking 'Lookup Taxa Info' - a good idea if you're very familiar with the taxa, but the project will not provide information about matches beyond the name.*
 
 Information about the DB's taxa will be on the left-hand side. All similar entries in the .nexus file will appear in the middle of the screen. Click on the name you'd like to change the entry to, manually enter a name on the bottom, or click on 'same species', or 'same genus' for additional options, if available.
 
 Once all selections have been made, a new .csv file will be created in the same directory as the original database .csv file.
 
+Your matching progress is not saved until a new file is created, so be prepared to start over if you exit halfway through.
+
+Downloaded content will cache immediately upon download, so starting over will take significantly less time.
+
 ## Examples:
 
 The program (correctly) thinks my best bet to match the database taxon Aotus azarae is Aotus azarai from the tree. But if I don't like that option I can click on 'same species' to see other taxa in the tree with the species name "azarae" or 'same genus' to see other members of the genus Aotus.
 
 ![Similar Example](https://github.com/spearw/phylo-match/raw/main/images/similar_example.png)
 
 Here's an example of the 'same species' option at work: The database has Vicunga pacos but the tree has Lama pacos. This is useful if the genus has been split up.
 
 ![Species Example](https://github.com/spearw/phylo-match/raw/main/images/species_example.png)
 
-Here's an example where I might want to use the "Same Genus" option. This can be useful if you don't have many taxa in that genus and it doesn't really matter which species in the genus you use: Here I have data for Cercocebus atys but that taxon isn't in the tree. I could use a different Cercocebus species as a substitute. The 'removed suggestions' in the bottom left tells me that C. agilis is already matched between the data and tree, but C. atys and C. torquatus are sister species, both equally closely related to C. agilis, so I can use C. torquatus instead.
+Here's an example where I might want to use the "Same Genus" option. This can be useful if you don't have many taxa in that genus and it doesn't really matter which species in the genus you use: Here I have data for Cercocebus atys but that taxon isn't in the tree. I could use a different Cercocebus species as a substitute. The 'removed suggestions' in the bottom left tells me that C. agilis is already matched between the data and tree. Since I know that C. atys and C. torquatus are sister species, both equally closely related to C. agilis, I can use C. torquatus instead.
 
 ![Genus Example](https://github.com/spearw/phylo-match/raw/main/images/genus_example.png)
 
 
+## Troubleshooting
+```
+'phylo-match' is not recognized as an internal or external command,
+operable program or batch file.
+```
+This error usually means python has not been added to your PATH variable. See [adding python to PATH](https://realpython.com/add-python-to-path/) tutorial or similar for details.
+
+
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 ## License
-[GPL-3.0](https://choosealicense.com/licenses/gpl-3.0/)
+[GPL-3.0](https://choosealicense.com/licenses/gpl-3.0/)
```

### Comparing `phylo-match-0.0.9/phylo_match.egg-info/PKG-INFO` & `phylo_match-0.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: phylo-match
-Version: 0.0.9
+Version: 0.1.0
 Summary: For matching species databases
 Home-page: https://github.com/spearw/phylo-match
 Author: William Spear
 Author-email: spearw@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: COPYING
+Requires-Dist: diskcache
+Requires-Dist: PyQt6
+Requires-Dist: requests
+Requires-Dist: wikipedia
+Requires-Dist: levenshtein
 
 # Phylo-Match
 
 Phylo-Match is a package for correcting misspellings or disparate labelings in phylogenetic trees
 
 ## Installation
 
@@ -40,44 +45,59 @@
 ```
 
 Install Phylo-Match:
 ```bash
 pip3 install phylo-match
 ```
 
+
 ## Usage
 
 ```bash
 phylo-match
 ```
-Use the gui to select a database file (.csv), and a taxa tree (.nexus) to match the database to. Click run when you are happy with your selection.
+Use the gui to select a database file (.csv), and a taxa tree (.nexus) to match the database to. Enter the number of your species column in the box, if the taxa you are matching are not in the first column (index counts from 0, so enter 0 for first column, 1 for second, etc.)
+
+Click run when you are happy with your selection.
 
-*Phylo-Match does all of its calculations and api requests upfront, so users may have to wait 10-15 minutes after run is clicked, depending on internet speed.*
+*Phylo-Match does all of its calculations and api requests upfront, so users may have to wait 10-15 minutes after run is clicked, depending on internet speed and whether these taxa are already in their local cache.*
 
 *This time can be minimized by unchecking 'Lookup Taxa Info' - a good idea if you're very familiar with the taxa, but the project will not provide information about matches beyond the name.*
 
 Information about the DB's taxa will be on the left-hand side. All similar entries in the .nexus file will appear in the middle of the screen. Click on the name you'd like to change the entry to, manually enter a name on the bottom, or click on 'same species', or 'same genus' for additional options, if available.
 
 Once all selections have been made, a new .csv file will be created in the same directory as the original database .csv file.
 
+Your matching progress is not saved until a new file is created, so be prepared to start over if you exit halfway through.
+
+Downloaded content will cache immediately upon download, so starting over will take significantly less time.
+
 ## Examples:
 
 The program (correctly) thinks my best bet to match the database taxon Aotus azarae is Aotus azarai from the tree. But if I don't like that option I can click on 'same species' to see other taxa in the tree with the species name "azarae" or 'same genus' to see other members of the genus Aotus.
 
 ![Similar Example](https://github.com/spearw/phylo-match/raw/main/images/similar_example.png)
 
 Here's an example of the 'same species' option at work: The database has Vicunga pacos but the tree has Lama pacos. This is useful if the genus has been split up.
 
 ![Species Example](https://github.com/spearw/phylo-match/raw/main/images/species_example.png)
 
-Here's an example where I might want to use the "Same Genus" option. This can be useful if you don't have many taxa in that genus and it doesn't really matter which species in the genus you use: Here I have data for Cercocebus atys but that taxon isn't in the tree. I could use a different Cercocebus species as a substitute. The 'removed suggestions' in the bottom left tells me that C. agilis is already matched between the data and tree, but C. atys and C. torquatus are sister species, both equally closely related to C. agilis, so I can use C. torquatus instead.
+Here's an example where I might want to use the "Same Genus" option. This can be useful if you don't have many taxa in that genus and it doesn't really matter which species in the genus you use: Here I have data for Cercocebus atys but that taxon isn't in the tree. I could use a different Cercocebus species as a substitute. The 'removed suggestions' in the bottom left tells me that C. agilis is already matched between the data and tree. Since I know that C. atys and C. torquatus are sister species, both equally closely related to C. agilis, I can use C. torquatus instead.
 
 ![Genus Example](https://github.com/spearw/phylo-match/raw/main/images/genus_example.png)
 
 
+## Troubleshooting
+```
+'phylo-match' is not recognized as an internal or external command,
+operable program or batch file.
+```
+This error usually means python has not been added to your PATH variable. See [adding python to PATH](https://realpython.com/add-python-to-path/) tutorial or similar for details.
+
+
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 ## License
 [GPL-3.0](https://choosealicense.com/licenses/gpl-3.0/)
```

### Comparing `phylo-match-0.0.9/setup.cfg` & `phylo_match-0.1.0/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = phylo-match
-version = 0.0.9
+version = 0.1.0
 author = William Spear
 author_email = spearw@gmail.com
 description = For matching species databases
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/spearw/phylo-match
 classifiers = 
@@ -21,13 +21,13 @@
 	PyQt6
 	requests
 	wikipedia
 	levenshtein
 
 [options.entry_points]
 console_scripts = 
-	phylo-match = src.python.gui:main
+	phylo-match = phylo_match.gui:main
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `phylo-match-0.0.9/src/python/definitions.py` & `phylo_match-0.1.0/phylo_match/definitions/definitions.py`

 * *Files identical despite different names*

### Comparing `phylo-match-0.0.9/src/python/gui.py` & `phylo_match-0.1.0/phylo_match/gui.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,20 +17,23 @@
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 '''
 
 import sys
 import datetime
 
 from argparse import ArgumentParser
+
+from PyQt6.QtGui import QIntValidator
+from PyQt6.uic.properties import QtWidgets
 from diskcache import Cache
 from PyQt6.QtCore import Qt
 from PyQt6.QtWidgets import QApplication, QWidget, QPushButton, QVBoxLayout, \
     QHBoxLayout, QGridLayout, QLabel, QLineEdit
-from src.python.definitions import *
-from src.python.match import *
+from phylo_match.definitions.definitions import *
+from phylo_match.match.match import *
 from PyQt6.QtWidgets import *
 from PyQt6.QtCore import *
 
 
 class LoadingWindow(QMainWindow):
     def __init__(self, parent=None):
         super(LoadingWindow, self).__init__(parent)
@@ -138,14 +141,23 @@
         self.cache_selection_layout.addWidget(self.cache_file_selection, 4, 0, 1, 1)
 
         # Add lookup checkbox
         self.do_lookup = QCheckBox(checked=True)
         self.do_lookup.setText("Lookup Taxa Info")
         self.options_layout.addWidget(self.do_lookup)
 
+        # Add lookup index selector
+        self.species_index = 0
+        self.lbl_integer = QLabel("Species Index (from 0)")
+        self.species_index_textbox = QLineEdit()
+        self.species_index_textbox.setPlaceholderText("0")
+        self.species_index_textbox.setValidator(QIntValidator(1, 999, self))
+        self.options_layout.addWidget(self.lbl_integer)
+        self.options_layout.addWidget(self.species_index_textbox)
+
         # Add run button
         self.run_button_spacer = QLabel()
         self.run_button = QPushButton("Run")
         self.run_button.setEnabled(False)
         self.run_button.clicked.connect(self.start_match)
         self.run_button_layout.addWidget(self.run_button_spacer)
         self.run_button_layout.addWidget(self.run_button)
@@ -187,16 +199,38 @@
         compare_window = Compare(self)
 
         self.prog_label.setText("Analyzing...")
         self.prog_bar.setValue(0)
         QApplication.processEvents()
 
         self.dialogs.append(compare_window)
-        dbs, tree = read_files(self.db_path, self.nexus_path)
-        taxa_list = match(dbs, tree, "_", 4)
+
+        self.species_index = self.species_index_textbox.text()
+        if self.species_index == '':
+            self.species_index = 0
+        else:
+            self.species_index = int(self.species_index_textbox.text())
+
+        dbs, tree = read_files(self.db_path, self.nexus_path, self.species_index)
+
+        dupes = set()
+        # Check for duplicate entries in dbs
+        for db in dbs:
+            db_dupes = set([x for x in db if db.count(x) > 1])
+            dupes = dupes.union(db_dupes)
+
+        if len(dupes) > 0:
+            msg = QMessageBox()
+            # msg.setIcon(QMessageBox.Critical)
+            msg.setText("Warning: Duplicate Entries")
+            msg.setInformativeText(f"{', '.join(dupes)} appear multiple times")
+            msg.setWindowTitle("Duplicate Entries")
+            msg.exec()
+
+        taxa_list, compare_window.perfect_matches = match(dbs, tree, "_", 4)
 
         # If option for online lookup, do lookup
         if self.do_lookup.isChecked():
             # Cached_info may be cached remotely or locally in future versions
             # cached_info = read_wiki_file(INFO_PATH, INFO_FNAME)
             cache = Cache(self.cache_path)
 
@@ -240,16 +274,16 @@
                 value = get_wiki_section(key)
                 cache.set(key, value)
 
         self.prog_label.setText("Done!")
         QApplication.processEvents()
 
         compare_window.__init__(self)
-
         compare_window.setParent(self)
+        compare_window.species_index = self.species_index
         compare_window.set_db_path(self.db_path)
         compare_window.set_do_lookup(self.do_lookup.isChecked())
 
         compare_window.set_cache(cache)
         compare_window.compare_mismatch(iter(taxa_list))
         self.hide()
 
@@ -290,30 +324,33 @@
         self.taxa_layout = QVBoxLayout()
         self.taxa_layout.setAlignment(Qt.AlignmentFlag.AlignCenter)
         self.main_layout.addLayout(self.taxa_layout, 1, 0)
 
         self.count_layout = QHBoxLayout()
         self.main_layout.addLayout(self.count_layout, 0, 1)
 
-        self.suggestions_layout = QHBoxLayout()
-        self.main_layout.addLayout(self.suggestions_layout, 1, 1)
+        self.suggestions_sub_layout = QHBoxLayout()
+        self.suggestions_scroll_area = QScrollArea()
+
+        self.suggestions_scrolling_layout = QHBoxLayout()
+        self.main_layout.addLayout(self.suggestions_scrolling_layout, 1, 1)
 
         self.manual_entry_layout = QVBoxLayout()
         self.main_layout.addLayout(self.manual_entry_layout, 2, 1, 1, 2)
 
         # Add contents to info_layout
         self.taxa_label = QLabel("animals_animals")
         self.taxa_label.setAlignment(Qt.AlignmentFlag.AlignCenter)
         self.taxa_label.setStyleSheet("padding: 30px; border-radius: 0px; background-color: lightgray; color: black;")
         self.info_layout.addWidget(self.taxa_label, 1)
 
         # Add contents to taxa_layout
-        self.removed_suggestions_label = QLabel()
-        self.removed_suggestions_label.setAlignment(Qt.AlignmentFlag.AlignCenter)
-        self.removed_suggestions_label.setContentsMargins(5, 5, 5, 5)
+        self.removed_suggestions_scroll_area = QScrollArea()
+        self.removed_suggestions_scroll_area.setAlignment(Qt.AlignmentFlag.AlignCenter)
+        self.removed_suggestions_scroll_area.setContentsMargins(5, 5, 5, 5)
         self.removed_suggestions_count = QLabel()
         self.removed_suggestions_count.setAlignment(Qt.AlignmentFlag.AlignCenter)
         self.taxa_layout.addWidget(self.removed_suggestions_count, 1)
 
         # Add contents to count_layout
         self.options_count_label = QHBoxLayout()
         self.options_count_label.setAlignment(Qt.AlignmentFlag.AlignCenter)
@@ -341,14 +378,20 @@
         self.leave_btn.setMaximumWidth(150)
         self.manual_entry_layout.addWidget(self.leave_btn)
         self.manual_entry_layout.setContentsMargins(10, 10, 10, 10)
 
         # Init global variables
         self.removed_suggestions = []
         self.taxa_list = []
+        self.species_index = 0
+
+    def closeEvent(self, *args, **kwargs):
+        print("Force exit by user")
+        ## TODO: Add pop up box with option to save progress
+        quit()
 
     def set_db_path(self, db_path):
         self.db_path = db_path
 
     def set_do_lookup(self, do_lookup):
         self.do_lookup = do_lookup
 
@@ -372,15 +415,15 @@
 
                 self.show_suggestions(next_taxa, taxa_iter, i)
 
                 self.taxa_label.setText(db_taxa)
                 self.show()
         else:
             # End of file, record results
-            write_file(self.taxa_list, self.db_path)
+            write_file(self.taxa_list, self.db_path, self.species_index)
             # Open main menu
             self.parent().show()
             self.close()
 
     def make_confirm_function(self, suggestion, taxa_iter, compare_window):
         def confirm_suggestion():
             self.taxa_list.append(suggestion)
@@ -392,35 +435,35 @@
 
         return confirm_suggestion
 
     def remove_chosen_entries(self, taxa):
 
         taxa_name = taxa[0]
 
-        for taxa_suggestions in taxa:
+        for i, taxa_suggestions in enumerate(taxa):
             if type(taxa_suggestions) != str:
                 for suggestion in taxa_suggestions:
                     # Remove suggestions that have already been chosen
                     # TODO: do this for entire suggestions list at beginning of new taxa to avoid changing once clicking
-                    if suggestion in self.taxa_list:
+                    if suggestion in self.taxa_list or suggestion in self.perfect_matches:
                         self.removed_suggestions.append(suggestion)
-                        taxa_suggestions.remove(suggestion)
                         continue
+                taxa[i] = [x for x in taxa_suggestions if x not in self.removed_suggestions]
         return taxa
 
     def confirm_text(self, suggestion, taxa_iter, compare_window):
         # TODO: close window more intelligently
         self.taxa_list.append(suggestion)
 
         self.line_edit.clear()
         self.removed_suggestions.clear()
 
         self.compare_mismatch(taxa_iter)
 
-    def create_wiki_label(self, taxa):
+    def create_wiki_scroll_area(self, taxa):
         # Create text box from wiki
         label = QLabel()
         label.setScaledContents(True)
         try:
             label.setText(get_wiki_section(taxa, cache=self.cache))
         except:
             label.setText("No information found")
@@ -461,36 +504,73 @@
         btn.setStyleSheet("padding: 20px; border-radius: 15px; background-color: gray;")
         # btn.adjustSize()
         f = self.make_confirm_function(taxa, taxa_iter, self)
         btn.clicked.connect(f)
         taxa_layout.addWidget(btn)
 
         if self.do_lookup:
-            scroll = self.create_wiki_label(taxa)
+            scroll = self.create_wiki_scroll_area(taxa)
             taxa_layout.addWidget(scroll)
 
         taxa_layout.setContentsMargins(10, 5, 10, 5)
 
         return taxa_layout
 
+    def create_removed_suggestions_scroll_area(self, removed_suggestions_text):
+        # Create text box from wiki
+        label = QLabel()
+        label.setScaledContents(True)
+        try:
+            label.setText(removed_suggestions_text)
+        except:
+            label.setText("No entries")
+        label.setWordWrap(True)
+        label.setAlignment(Qt.AlignmentFlag.AlignLeft)
+        label.show()
+
+        # Create scroll area for text box
+        scroll = QScrollArea()
+        scroll.setWidget(label)
+        scroll.setWidgetResizable(True)
+        scroll.setAlignment(Qt.AlignmentFlag.AlignCenter)
+        scroll.setFixedHeight(200)
+        scroll.setMaximumWidth(200)
+
+        return scroll
+
+    def create_suggestions_scroll_area(self):
+        scroll = QScrollArea()
+        widget = QWidget()
+        widget.setContentsMargins(0, 0, 0, 0)
+        widget.setLayout(self.suggestions_sub_layout)
+        scroll.setWidget(widget)
+        scroll.setWidgetResizable(True)
+        scroll.setAlignment(Qt.AlignmentFlag.AlignCenter)
+        scroll.setFixedHeight(400)
+        scroll.setMaximumWidth(800)
+
+        return scroll
+
     def show_suggestions(self, next_taxa, taxa_iter, i):
 
         # Clear old buttons + count_layout
-        for j in reversed(range(self.suggestions_layout.count())):
-            layout = self.suggestions_layout.itemAt(j).layout()
-            self.suggestions_layout.removeItem(layout)
+        for j in reversed(range(self.suggestions_sub_layout.count())):
+            layout = self.suggestions_sub_layout.itemAt(j).layout()
+            self.suggestions_sub_layout.removeItem(layout)
             for k in reversed(range(layout.count())):
                 layout.itemAt(k).widget().setParent(None)
 
+        self.suggestions_scroll_area.setParent(None)
 
-        self.removed_suggestions_label.setParent(None)
+
+        self.removed_suggestions_scroll_area.setParent(None)
         self.removed_suggestions_count.setText(f"Removed Suggestions: {len(self.removed_suggestions)}")
         if self.removed_suggestions:
-            self.removed_suggestions_label.setText(", ".join(self.removed_suggestions))
-            self.taxa_layout.addWidget(self.removed_suggestions_label, 1)
+            self.removed_suggestions_scroll_area = self.create_removed_suggestions_scroll_area(", \n".join(self.removed_suggestions))
+            self.taxa_layout.addWidget(self.removed_suggestions_scroll_area, 1)
 
         num_suggestions = [len(next_taxa[1]), len(next_taxa[2]), len(next_taxa[3])]
 
         if i <= 3:
             category_suggestions = next_taxa[i]
             while not category_suggestions:
                 i += 1
@@ -499,24 +579,27 @@
                 category_suggestions = next_taxa[i]
 
             if i <= 3:
                 # reset and load taxa, if possible
                 self.taxa_info.setParent(None)
 
                 if self.do_lookup:
-                    self.taxa_info = self.create_wiki_label(next_taxa[0])
+                    self.taxa_info = self.create_wiki_scroll_area(next_taxa[0])
                     h_layout = QHBoxLayout()
                     h_layout.addWidget(self.taxa_info)
                     self.taxa_layout.insertLayout(0, h_layout)
 
                 for suggestion in category_suggestions:
 
                     # Add info and image widget to page
                     suggestion_layout = self.create_taxa_layout(suggestion, taxa_iter)
-                    self.suggestions_layout.addLayout(suggestion_layout)
+                    self.suggestions_sub_layout.addLayout(suggestion_layout)
+
+                self.suggestions_scroll_area = self.create_suggestions_scroll_area()
+                self.suggestions_scrolling_layout.addWidget(self.suggestions_scroll_area)
 
 
                 # Check that all category_suggestions were not removed by being previously picked, continue if they were
                 if not category_suggestions:
                     i += 1
                     self.show_suggestions(next_taxa, taxa_iter, i)
```

### Comparing `phylo-match-0.0.9/src/python/match.py` & `phylo_match-0.1.0/phylo_match/match/match.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,47 +28,50 @@
 from Levenshtein import distance as levenshtein_distance
 from functools import lru_cache
 
 
 def match(dbs, tree, db_separator="_", levenshtein_num=4):
 
     output = []
+    perfect_matches = []
     difference_threshold = int(levenshtein_num)
     for db in dbs:
         for db_name in db:
             suggestions = []
             genus_match = []
             species_match = []
+            genus_name = db_name.split(db_separator, 1)[0]
             try:
-                genus_name = db_name.split(db_separator, 1)[0]
                 species_name = db_name.split(db_separator, 1)[1]
             except:
-                break
+                species_name = ""
+                print(f"WARNING: entry [{db_name}] possibly malformed. Check database.")
 
             found_match = False
             for tree_name in tree:
                 if db_name == tree_name:
                     found_match = True
                     break
                 elif levenshtein_distance(db_name, tree_name) < difference_threshold:
                     suggestions.append(tree_name)
-                elif re.match(rf".*{species_name}", tree_name):
+                elif re.match(rf".*[_| ]{species_name}$", tree_name):
                     species_match.append(tree_name)
-                elif re.match(rf"{genus_name}*", tree_name):
+                elif re.match(rf"^{genus_name}[_| ]", tree_name):
                     genus_match.append(tree_name)
 
             if found_match:
                 output.append(db_name)
+                perfect_matches.append(db_name)
             else:
                 output.append([db_name, suggestions, species_match, genus_match])
 
-    return output
+    return output, perfect_matches
 
 
-def read_files(db_path, tree_path):
+def read_files(db_path, tree_path, species_name_index):
     dbs = []
     trees = []
     filenames = []
     if os.path.isdir(db_path):
         filenames = os.listdir(db_path)
     else:
         filenames.append(os.path.basename(db_path))
@@ -76,16 +79,16 @@
 
     for filename in filenames:
         if not filename.startswith('.'):
             with open(os.path.join(db_path, filename), 'r', encoding="utf-8") as f:  # open in readonly mode
                 db = []
                 for line in f:
                     # Get name for every line
-                    name = line.split(",", 1)[0]
-                    db.append(name)
+                    name = line.split(",")[species_name_index]
+                    db.append(name.strip())
 
                 # Remove first line of db (info line)
                 db.pop(0)
                 dbs.append(db)
 
     filenames = []
     if os.path.isdir(tree_path):
@@ -124,15 +127,15 @@
 
 def append_id(filename):
     p = Path(filename)
     return "{0}_{2}{1}".format(Path.joinpath(p.parent, p.stem), p.suffix, time.time())
 
 # Takes the completed taxa_list and writes a new file that includes the new taxa names and the rest of the data from db_path
 # TODO: handle multiple input dbs, perhaps with search
-def write_file(taxa_list, db_path):
+def write_file(taxa_list, db_path, species_index):
 
     outfile_path = append_id(db_path)
 
     with open(outfile_path, "w", encoding="utf-8") as outf:
 
         with open(db_path, 'r', encoding="utf-8") as f:  # open in readonly mode
 
@@ -140,19 +143,19 @@
 
             for line in f:
 
                 if i == 0:
                     outf.write(line)
                     i += 1
                 else:
-                    csv_line = line.split(",")
+                    csv_list = line.strip().split(",")
                     # Replace first line with new name, only if not blank
                     if taxa_list[i - 1] != "":
-                        csv_line[0] = taxa_list[i - 1]
-                    outf.write(",".join(csv_line))
+                        csv_list[species_index] = taxa_list[i - 1]
+                    outf.write(f"{','.join(csv_list)}\n")
                     i += 1
 
 
 def get_wiki_image(search_term):
     WIKI_REQUEST = 'http://en.wikipedia.org/w/api.php?action=query&prop=pageimages&format=json&piprop=original&titles='
     try:
         result = wikipedia.search(search_term, results=1)
```

