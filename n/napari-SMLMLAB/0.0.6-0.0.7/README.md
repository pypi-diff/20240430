# Comparing `tmp/napari_smlmlab-0.0.6.tar.gz` & `tmp/napari_smlmlab-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\turnerp\PycharmProjects\napari-SMLMLAB\dist\.tmp-666jea7q\napari_smlmlab-0.0.6.tar", last modified: Mon Apr 29 11:26:09 2024, max compression
+gzip compressed data, was "C:\Users\turnerp\PycharmProjects\napari-SMLMLAB\dist\.tmp-eb76f6l8\napari_smlmlab-0.0.7.tar", last modified: Mon Apr 29 14:33:00 2024, max compression
```

## Comparing `napari_smlmlab-0.0.6.tar` & `napari_smlmlab-0.0.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 11:26:09.600597 napari_smlmlab-0.0.6/
--rw-rw-rw-   0        0        0     1515 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      101 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     4645 2024-04-29 11:26:09.599600 napari_smlmlab-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2854 2024-04-25 14:22:00.000000 napari_smlmlab-0.0.6/README.md
--rw-rw-rw-   0        0        0     1243 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0     1819 2024-04-29 11:26:09.603396 napari_smlmlab-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-29 11:26:09.535225 napari_smlmlab-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2024-04-29 11:26:09.597606 napari_smlmlab-0.0.6/src/napari_SMLMLAB.egg-info/
--rw-rw-rw-   0        0        0     4645 2024-04-29 11:26:09.000000 napari_smlmlab-0.0.6/src/napari_SMLMLAB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      731 2024-04-29 11:26:09.000000 napari_smlmlab-0.0.6/src/napari_SMLMLAB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 11:26:09.000000 napari_smlmlab-0.0.6/src/napari_SMLMLAB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-29 11:26:09.000000 napari_smlmlab-0.0.6/src/napari_SMLMLAB.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      148 2024-04-29 11:26:09.000000 napari_smlmlab-0.0.6/src/napari_SMLMLAB.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-29 11:26:09.000000 napari_smlmlab-0.0.6/src/napari_SMLMLAB.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-29 11:26:09.566468 napari_smlmlab-0.0.6/src/smlmlab/
--rw-rw-rw-   0        0        0      102 2024-04-29 11:26:03.000000 napari_smlmlab-0.0.6/src/smlmlab/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:26:09.566468 napari_smlmlab-0.0.6/src/smlmlab/_tests/
--rw-rw-rw-   0        0        0        0 2024-04-24 10:36:50.000000 napari_smlmlab-0.0.6/src/smlmlab/_tests/__init__.py
--rw-rw-rw-   0        0        0     2176 2024-04-25 13:50:35.000000 napari_smlmlab-0.0.6/src/smlmlab/_tests/test_widget.py
--rw-rw-rw-   0        0        0    12984 2024-04-29 11:24:47.000000 napari_smlmlab-0.0.6/src/smlmlab/_widget.py
--rw-rw-rw-   0        0        0    36584 2024-04-29 11:00:01.000000 napari_smlmlab-0.0.6/src/smlmlab/gui.py
--rw-rw-rw-   0        0        0      502 2024-04-25 13:52:37.000000 napari_smlmlab-0.0.6/src/smlmlab/napari.yaml
-drwxrwxrwx   0        0        0        0 2024-04-29 11:26:09.594613 napari_smlmlab-0.0.6/src/smlmlab/utils/
--rw-rw-rw-   0        0        0        0 2024-04-24 11:59:46.000000 napari_smlmlab-0.0.6/src/smlmlab/utils/__init__.py
--rw-rw-rw-   0        0        0     9793 2024-04-25 12:48:07.000000 napari_smlmlab-0.0.6/src/smlmlab/utils/compute_utils.py
--rw-rw-rw-   0        0        0    27637 2024-04-29 08:31:32.000000 napari_smlmlab-0.0.6/src/smlmlab/utils/events_utils.py
--rw-rw-rw-   0        0        0    21212 2024-04-29 07:50:18.000000 napari_smlmlab-0.0.6/src/smlmlab/utils/import_utils.py
--rw-rw-rw-   0        0        0    31463 2024-04-26 16:23:10.000000 napari_smlmlab-0.0.6/src/smlmlab/utils/loc_utils.py
--rw-rw-rw-   0        0        0    24786 2024-04-26 20:50:24.000000 napari_smlmlab-0.0.6/src/smlmlab/utils/picasso_utils.py
--rw-rw-rw-   0        0        0     9607 2024-04-29 10:09:03.000000 napari_smlmlab-0.0.6/src/smlmlab/utils/undrift_utils.py
--rw-rw-rw-   0        0        0     8197 2024-04-26 20:55:11.000000 napari_smlmlab-0.0.6/src/smlmlab/utils/viewer_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 14:33:00.032905 napari_smlmlab-0.0.7/
+-rw-rw-rw-   0        0        0     1515 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      101 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     4645 2024-04-29 14:33:00.032905 napari_smlmlab-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2854 2024-04-25 14:22:00.000000 napari_smlmlab-0.0.7/README.md
+-rw-rw-rw-   0        0        0     1243 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0     1819 2024-04-29 14:33:00.032905 napari_smlmlab-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-29 14:32:59.970417 napari_smlmlab-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2024-04-29 14:33:00.032905 napari_smlmlab-0.0.7/src/napari_SMLMLAB.egg-info/
+-rw-rw-rw-   0        0        0     4645 2024-04-29 14:32:59.000000 napari_smlmlab-0.0.7/src/napari_SMLMLAB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      731 2024-04-29 14:32:59.000000 napari_smlmlab-0.0.7/src/napari_SMLMLAB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 14:32:59.000000 napari_smlmlab-0.0.7/src/napari_SMLMLAB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-29 14:32:59.000000 napari_smlmlab-0.0.7/src/napari_SMLMLAB.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      148 2024-04-29 14:32:59.000000 napari_smlmlab-0.0.7/src/napari_SMLMLAB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-29 14:32:59.000000 napari_smlmlab-0.0.7/src/napari_SMLMLAB.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 14:33:00.017284 napari_smlmlab-0.0.7/src/smlmlab/
+-rw-rw-rw-   0        0        0      102 2024-04-29 14:32:52.000000 napari_smlmlab-0.0.7/src/smlmlab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 14:33:00.017284 napari_smlmlab-0.0.7/src/smlmlab/_tests/
+-rw-rw-rw-   0        0        0        0 2024-04-24 10:36:50.000000 napari_smlmlab-0.0.7/src/smlmlab/_tests/__init__.py
+-rw-rw-rw-   0        0        0     2176 2024-04-25 13:50:35.000000 napari_smlmlab-0.0.7/src/smlmlab/_tests/test_widget.py
+-rw-rw-rw-   0        0        0    14085 2024-04-29 14:27:11.000000 napari_smlmlab-0.0.7/src/smlmlab/_widget.py
+-rw-rw-rw-   0        0        0    36584 2024-04-29 11:00:01.000000 napari_smlmlab-0.0.7/src/smlmlab/gui.py
+-rw-rw-rw-   0        0        0      502 2024-04-25 13:52:37.000000 napari_smlmlab-0.0.7/src/smlmlab/napari.yaml
+drwxrwxrwx   0        0        0        0 2024-04-29 14:33:00.032905 napari_smlmlab-0.0.7/src/smlmlab/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-24 11:59:46.000000 napari_smlmlab-0.0.7/src/smlmlab/utils/__init__.py
+-rw-rw-rw-   0        0        0     9793 2024-04-25 12:48:07.000000 napari_smlmlab-0.0.7/src/smlmlab/utils/compute_utils.py
+-rw-rw-rw-   0        0        0    28891 2024-04-29 14:30:59.000000 napari_smlmlab-0.0.7/src/smlmlab/utils/events_utils.py
+-rw-rw-rw-   0        0        0    21212 2024-04-29 07:50:18.000000 napari_smlmlab-0.0.7/src/smlmlab/utils/import_utils.py
+-rw-rw-rw-   0        0        0    31463 2024-04-26 16:23:10.000000 napari_smlmlab-0.0.7/src/smlmlab/utils/loc_utils.py
+-rw-rw-rw-   0        0        0    24786 2024-04-26 20:50:24.000000 napari_smlmlab-0.0.7/src/smlmlab/utils/picasso_utils.py
+-rw-rw-rw-   0        0        0     9607 2024-04-29 10:09:03.000000 napari_smlmlab-0.0.7/src/smlmlab/utils/undrift_utils.py
+-rw-rw-rw-   0        0        0     8197 2024-04-26 20:55:11.000000 napari_smlmlab-0.0.7/src/smlmlab/utils/viewer_utils.py
```

### Comparing `napari_smlmlab-0.0.6/LICENSE` & `napari_smlmlab-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.6/PKG-INFO` & `napari_smlmlab-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-SMLMLAB
-Version: 0.0.6
+Version: 0.0.7
 Summary: Napari widget for BP04 Practical
 Home-page: https://github.com/piedrro/napari-SMLMLAB
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/piedrro/napari-SMLMLAB/issues
 Project-URL: Documentation, https://github.com/piedrro/napari-SMLMLAB#README.md
```

### Comparing `napari_smlmlab-0.0.6/README.md` & `napari_smlmlab-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.6/pyproject.toml` & `napari_smlmlab-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.6/setup.cfg` & `napari_smlmlab-0.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.6/src/napari_SMLMLAB.egg-info/PKG-INFO` & `napari_smlmlab-0.0.7/src/napari_SMLMLAB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-SMLMLAB
-Version: 0.0.6
+Version: 0.0.7
 Summary: Napari widget for BP04 Practical
 Home-page: https://github.com/piedrro/napari-SMLMLAB
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/piedrro/napari-SMLMLAB/issues
 Project-URL: Documentation, https://github.com/piedrro/napari-SMLMLAB#README.md
```

### Comparing `napari_smlmlab-0.0.6/src/napari_SMLMLAB.egg-info/SOURCES.txt` & `napari_smlmlab-0.0.7/src/napari_SMLMLAB.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.6/src/smlmlab/_tests/test_widget.py` & `napari_smlmlab-0.0.7/src/smlmlab/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.6/src/smlmlab/_widget.py` & `napari_smlmlab-0.0.7/src/smlmlab/_widget.py`

 * *Files 9% similar despite different names*

```diff
@@ -61,18 +61,27 @@
         self.gui.picasso_vis_size.currentIndexChanged.connect(partial(self.draw_molecules, update_vis=True))
         self.gui.picasso_vis_size.currentIndexChanged.connect(partial(self.draw_bounding_boxes, update_vis=True))
         self.gui.picasso_vis_opacity.currentIndexChanged.connect(partial(self.draw_molecules, update_vis=True))
         self.gui.picasso_vis_opacity.currentIndexChanged.connect(partial(self.draw_bounding_boxes, update_vis=True))
         self.gui.picasso_vis_edge_width.currentIndexChanged.connect(partial(self.draw_molecules, update_vis=True))
         self.gui.picasso_vis_edge_width.currentIndexChanged.connect(partial(self.draw_bounding_boxes, update_vis=True))
 
+        self.gui.picasso_dataset.currentIndexChanged.connect(lambda: self.update_channel_selector(dataset_selector="picasso_dataset", channel_selector="picasso_channel", ))
+        self.gui.picasso_render_dataset.currentIndexChanged.connect(lambda: self.update_channel_selector(dataset_selector="picasso_render_dataset", channel_selector="picasso_render_channel", ))
+        self.gui.plot_dataset.currentIndexChanged.connect(lambda: self.update_channel_selector(dataset_selector="plot_dataset", channel_selector="plot_channel", efficiency=True, ))
+        self.gui.locs_export_dataset.currentIndexChanged.connect(lambda: self.update_channel_selector(dataset_selector="locs_export_dataset", channel_selector="locs_export_channel", ))
+        self.gui.picasso_undrift_dataset.currentIndexChanged.connect(lambda: self.update_channel_selector(dataset_selector="picasso_undrift_dataset", channel_selector="picasso_undrift_channel", ))
+
         self.gui.plot_mode.currentIndexChanged.connect(self.draw_line_plot)
         self.gui.plot_dataset.currentIndexChanged.connect(self.draw_line_plot)
         self.gui.plot_channel.currentIndexChanged.connect(self.draw_line_plot)
 
+        self.gui.dataset_selector.currentIndexChanged.connect(partial(self.update_active_image,
+            dataset = self.gui.dataset_selector.currentText()))
+
         self.verbose = False
 
         self.dataset_dict = {}
         self.localisation_dict = {"bounding_boxes": {}, "molecules": {}}
         self.traces_dict = {}
         self.plot_dict = {}
         self.contrast_dict = {}
```

### Comparing `napari_smlmlab-0.0.6/src/smlmlab/gui.py` & `napari_smlmlab-0.0.7/src/smlmlab/gui.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.6/src/smlmlab/utils/compute_utils.py` & `napari_smlmlab-0.0.7/src/smlmlab/utils/compute_utils.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.6/src/smlmlab/utils/events_utils.py` & `napari_smlmlab-0.0.7/src/smlmlab/utils/events_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -326,14 +326,37 @@
 
                             if efficiency == True:
                                 if set(["donor", "acceptor"]).issubset(set(channel_names)):
                                     channel_selector_list.append("FRET Efficiency")
                                 if set(["dd", "da"]).issubset(set(channel_names)):
                                     channel_selector_list.append("ALEX Efficiency")
 
+                elif dataset_name == "All Datasets":
+                    channel_names = []
+
+                    for dataset_name in self.dataset_dict.keys():
+                        dataset_channels = [channel.lower() for channel in self.dataset_dict[dataset_name].keys()]
+                        channel_names.append(dataset_channels)
+
+                    channel_names = list(set.intersection(*map(set, channel_names)))
+
+                    for channel in channel_names:
+                        if "efficiency" not in channel.lower():
+                            if channel in ["da", "dd", "aa", "ad"]:
+                                channel_selector_list.append(channel.upper())
+                            elif channel in ["donor", "acceptor"]:
+                                channel_selector_list.append(channel.capitalize())
+
+                            if efficiency == True:
+                                if set(["donor", "acceptor"]).issubset(set(channel_names)):
+                                    channel_selector_list.append("FRET Efficiency")
+                                if set(["dd", "da"]).issubset(set(channel_names)):
+                                    channel_selector_list.append("ALEX Efficiency")
+
+
                 if channel_selector_list != []:
                     channel_selector.clear()
                     channel_selector_list = list(set(channel_selector_list))
                     channel_selector.addItems(channel_selector_list)
 
                 channel_selector.blockSignals(False)
```

### Comparing `napari_smlmlab-0.0.6/src/smlmlab/utils/import_utils.py` & `napari_smlmlab-0.0.7/src/smlmlab/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.6/src/smlmlab/utils/loc_utils.py` & `napari_smlmlab-0.0.7/src/smlmlab/utils/loc_utils.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.6/src/smlmlab/utils/picasso_utils.py` & `napari_smlmlab-0.0.7/src/smlmlab/utils/picasso_utils.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.6/src/smlmlab/utils/undrift_utils.py` & `napari_smlmlab-0.0.7/src/smlmlab/utils/undrift_utils.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.6/src/smlmlab/utils/viewer_utils.py` & `napari_smlmlab-0.0.7/src/smlmlab/utils/viewer_utils.py`

 * *Files identical despite different names*

