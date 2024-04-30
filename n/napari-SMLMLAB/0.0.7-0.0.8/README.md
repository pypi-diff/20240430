# Comparing `tmp/napari_smlmlab-0.0.7.tar.gz` & `tmp/napari_smlmlab-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\turnerp\PycharmProjects\napari-SMLMLAB\dist\.tmp-eb76f6l8\napari_smlmlab-0.0.7.tar", last modified: Mon Apr 29 14:33:00 2024, max compression
+gzip compressed data, was "C:\Users\turnerp\PycharmProjects\napari-SMLMLAB\dist\.tmp-ql_o0j0m\napari_smlmlab-0.0.8.tar", last modified: Tue Apr 30 11:08:13 2024, max compression
```

## Comparing `napari_smlmlab-0.0.7.tar` & `napari_smlmlab-0.0.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 14:33:00.032905 napari_smlmlab-0.0.7/
--rw-rw-rw-   0        0        0     1515 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      101 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     4645 2024-04-29 14:33:00.032905 napari_smlmlab-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2854 2024-04-25 14:22:00.000000 napari_smlmlab-0.0.7/README.md
--rw-rw-rw-   0        0        0     1243 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0     1819 2024-04-29 14:33:00.032905 napari_smlmlab-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-29 14:32:59.970417 napari_smlmlab-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2024-04-29 14:33:00.032905 napari_smlmlab-0.0.7/src/napari_SMLMLAB.egg-info/
--rw-rw-rw-   0        0        0     4645 2024-04-29 14:32:59.000000 napari_smlmlab-0.0.7/src/napari_SMLMLAB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      731 2024-04-29 14:32:59.000000 napari_smlmlab-0.0.7/src/napari_SMLMLAB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 14:32:59.000000 napari_smlmlab-0.0.7/src/napari_SMLMLAB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-29 14:32:59.000000 napari_smlmlab-0.0.7/src/napari_SMLMLAB.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      148 2024-04-29 14:32:59.000000 napari_smlmlab-0.0.7/src/napari_SMLMLAB.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-29 14:32:59.000000 napari_smlmlab-0.0.7/src/napari_SMLMLAB.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-29 14:33:00.017284 napari_smlmlab-0.0.7/src/smlmlab/
--rw-rw-rw-   0        0        0      102 2024-04-29 14:32:52.000000 napari_smlmlab-0.0.7/src/smlmlab/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 14:33:00.017284 napari_smlmlab-0.0.7/src/smlmlab/_tests/
--rw-rw-rw-   0        0        0        0 2024-04-24 10:36:50.000000 napari_smlmlab-0.0.7/src/smlmlab/_tests/__init__.py
--rw-rw-rw-   0        0        0     2176 2024-04-25 13:50:35.000000 napari_smlmlab-0.0.7/src/smlmlab/_tests/test_widget.py
--rw-rw-rw-   0        0        0    14085 2024-04-29 14:27:11.000000 napari_smlmlab-0.0.7/src/smlmlab/_widget.py
--rw-rw-rw-   0        0        0    36584 2024-04-29 11:00:01.000000 napari_smlmlab-0.0.7/src/smlmlab/gui.py
--rw-rw-rw-   0        0        0      502 2024-04-25 13:52:37.000000 napari_smlmlab-0.0.7/src/smlmlab/napari.yaml
-drwxrwxrwx   0        0        0        0 2024-04-29 14:33:00.032905 napari_smlmlab-0.0.7/src/smlmlab/utils/
--rw-rw-rw-   0        0        0        0 2024-04-24 11:59:46.000000 napari_smlmlab-0.0.7/src/smlmlab/utils/__init__.py
--rw-rw-rw-   0        0        0     9793 2024-04-25 12:48:07.000000 napari_smlmlab-0.0.7/src/smlmlab/utils/compute_utils.py
--rw-rw-rw-   0        0        0    28891 2024-04-29 14:30:59.000000 napari_smlmlab-0.0.7/src/smlmlab/utils/events_utils.py
--rw-rw-rw-   0        0        0    21212 2024-04-29 07:50:18.000000 napari_smlmlab-0.0.7/src/smlmlab/utils/import_utils.py
--rw-rw-rw-   0        0        0    31463 2024-04-26 16:23:10.000000 napari_smlmlab-0.0.7/src/smlmlab/utils/loc_utils.py
--rw-rw-rw-   0        0        0    24786 2024-04-26 20:50:24.000000 napari_smlmlab-0.0.7/src/smlmlab/utils/picasso_utils.py
--rw-rw-rw-   0        0        0     9607 2024-04-29 10:09:03.000000 napari_smlmlab-0.0.7/src/smlmlab/utils/undrift_utils.py
--rw-rw-rw-   0        0        0     8197 2024-04-26 20:55:11.000000 napari_smlmlab-0.0.7/src/smlmlab/utils/viewer_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-30 11:08:13.532135 napari_smlmlab-0.0.8/
+-rw-rw-rw-   0        0        0     1515 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      101 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     4645 2024-04-30 11:08:13.532135 napari_smlmlab-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2854 2024-04-25 14:22:00.000000 napari_smlmlab-0.0.8/README.md
+-rw-rw-rw-   0        0        0     1243 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0     1819 2024-04-30 11:08:13.532135 napari_smlmlab-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 11:08:13.469648 napari_smlmlab-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2024-04-30 11:08:13.532135 napari_smlmlab-0.0.8/src/napari_SMLMLAB.egg-info/
+-rw-rw-rw-   0        0        0     4645 2024-04-30 11:08:13.000000 napari_smlmlab-0.0.8/src/napari_SMLMLAB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      731 2024-04-30 11:08:13.000000 napari_smlmlab-0.0.8/src/napari_SMLMLAB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 11:08:13.000000 napari_smlmlab-0.0.8/src/napari_SMLMLAB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-30 11:08:13.000000 napari_smlmlab-0.0.8/src/napari_SMLMLAB.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      148 2024-04-30 11:08:13.000000 napari_smlmlab-0.0.8/src/napari_SMLMLAB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-30 11:08:13.000000 napari_smlmlab-0.0.8/src/napari_SMLMLAB.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 11:08:13.516513 napari_smlmlab-0.0.8/src/smlmlab/
+-rw-rw-rw-   0        0        0      102 2024-04-30 11:08:04.000000 napari_smlmlab-0.0.8/src/smlmlab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 11:08:13.516513 napari_smlmlab-0.0.8/src/smlmlab/_tests/
+-rw-rw-rw-   0        0        0        0 2024-04-24 10:36:50.000000 napari_smlmlab-0.0.8/src/smlmlab/_tests/__init__.py
+-rw-rw-rw-   0        0        0     2176 2024-04-25 13:50:35.000000 napari_smlmlab-0.0.8/src/smlmlab/_tests/test_widget.py
+-rw-rw-rw-   0        0        0    14371 2024-04-30 11:06:04.000000 napari_smlmlab-0.0.8/src/smlmlab/_widget.py
+-rw-rw-rw-   0        0        0    36584 2024-04-29 11:00:01.000000 napari_smlmlab-0.0.8/src/smlmlab/gui.py
+-rw-rw-rw-   0        0        0      502 2024-04-25 13:52:37.000000 napari_smlmlab-0.0.8/src/smlmlab/napari.yaml
+drwxrwxrwx   0        0        0        0 2024-04-30 11:08:13.532135 napari_smlmlab-0.0.8/src/smlmlab/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-24 11:59:46.000000 napari_smlmlab-0.0.8/src/smlmlab/utils/__init__.py
+-rw-rw-rw-   0        0        0     9793 2024-04-25 12:48:07.000000 napari_smlmlab-0.0.8/src/smlmlab/utils/compute_utils.py
+-rw-rw-rw-   0        0        0    29078 2024-04-30 10:33:27.000000 napari_smlmlab-0.0.8/src/smlmlab/utils/events_utils.py
+-rw-rw-rw-   0        0        0    21257 2024-04-30 08:13:50.000000 napari_smlmlab-0.0.8/src/smlmlab/utils/import_utils.py
+-rw-rw-rw-   0        0        0    31463 2024-04-26 16:23:10.000000 napari_smlmlab-0.0.8/src/smlmlab/utils/loc_utils.py
+-rw-rw-rw-   0        0        0    24786 2024-04-26 20:50:24.000000 napari_smlmlab-0.0.8/src/smlmlab/utils/picasso_utils.py
+-rw-rw-rw-   0        0        0     9607 2024-04-29 10:09:03.000000 napari_smlmlab-0.0.8/src/smlmlab/utils/undrift_utils.py
+-rw-rw-rw-   0        0        0     8197 2024-04-26 20:55:11.000000 napari_smlmlab-0.0.8/src/smlmlab/utils/viewer_utils.py
```

### Comparing `napari_smlmlab-0.0.7/LICENSE` & `napari_smlmlab-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.7/PKG-INFO` & `napari_smlmlab-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-SMLMLAB
-Version: 0.0.7
+Version: 0.0.8
 Summary: Napari widget for BP04 Practical
 Home-page: https://github.com/piedrro/napari-SMLMLAB
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/piedrro/napari-SMLMLAB/issues
 Project-URL: Documentation, https://github.com/piedrro/napari-SMLMLAB#README.md
```

### Comparing `napari_smlmlab-0.0.7/README.md` & `napari_smlmlab-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.7/pyproject.toml` & `napari_smlmlab-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.7/setup.cfg` & `napari_smlmlab-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.7/src/napari_SMLMLAB.egg-info/PKG-INFO` & `napari_smlmlab-0.0.8/src/napari_SMLMLAB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-SMLMLAB
-Version: 0.0.7
+Version: 0.0.8
 Summary: Napari widget for BP04 Practical
 Home-page: https://github.com/piedrro/napari-SMLMLAB
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/piedrro/napari-SMLMLAB/issues
 Project-URL: Documentation, https://github.com/piedrro/napari-SMLMLAB#README.md
```

### Comparing `napari_smlmlab-0.0.7/src/napari_SMLMLAB.egg-info/SOURCES.txt` & `napari_smlmlab-0.0.8/src/napari_SMLMLAB.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.7/src/smlmlab/_tests/test_widget.py` & `napari_smlmlab-0.0.8/src/smlmlab/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.7/src/smlmlab/_widget.py` & `napari_smlmlab-0.0.8/src/smlmlab/_widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -125,27 +125,21 @@
                             print("reformatting shapes to ndim=2")
 
                         shapes = shapes_layer.data.copy()
                         shapes = [shape[:, -2:] for shape in shapes]
                         shapes_layer.data = []
                         shapes_layer.add(shapes, shape_type=shape_type)
 
-                    # if event.action == "added":
-                    #     shape_indices = np.arange(len(shapes_layer.data))
-                    #     if len(shape_indices) > 1:
-                    #         print(shape_indices)
-                    #         shape_indices = shape_indices[:-1]
-                    #         shapes = shapes_layer.data.copy()
-                    #         new_shapes = []
-                    #         for index in range(len(shapes)):
-                    #             if index not in shape_indices:
-                    #                 new_shapes.append(shapes[index])
-                    #
-                    #         self.shapes_layer.data = []
-                    #         self.shapes_layer.data = new_shapes
+                    if event.action == "added":
+                        n_shapes = len(shapes)
+                        if n_shapes > 1:
+                            shapes = shapes_layer.data.copy()
+                            shape_types = shapes_layer.shape_type.copy()
+                            shapes_layer.data = []
+                            shapes_layer.add(shapes[-1], shape_type=shape_types[-1])
 
                     if shape_type == "line":
                         self.gui.plot_mode.setCurrentIndex(0)
 
                     if shape_type == "rectangle":
                         self.gui.plot_mode.setCurrentIndex(2)
 
@@ -192,15 +186,15 @@
                             img = self.dataset_dict[dataset][channel]["data"][current_frame]
 
                             x, y = np.linspace(x1, x2, num), np.linspace(y1, y2, num)
                             coords = np.vstack((x, y))
 
                             line_profile = map_coordinates(img, coords, order=1, mode="nearest")
 
-                            plot_dataset[channel][shape_index] = line_profile
+                            plot_dataset[channel] = {channel.capitalize(): line_profile}
 
                         if shape_type == "rectangle" and plot_mode == 2:
                             if shape.shape[-1] == 3:
                                 dat = shape[:, 1:]
                             else:
                                 dat = shape
 
@@ -208,51 +202,53 @@
                             x1, y1 = int(x1), int(y1)
                             x2, y2 = int(x2), int(y2)
 
                             img = self.dataset_dict[dataset][channel]["data"]
 
                             box_data = img[:, y1:y2, x1:x2]
 
-                            line_profile = np.mean(box_data, axis=(1, 2))
+                            box_profile = np.mean(box_data, axis=(1, 2))
 
-                            plot_dataset[channel][shape_index] = line_profile
+                            plot_dataset[channel] = {channel.capitalize(): box_profile}
 
-                    if set(["donor", "acceptor"]).issubset(plot_dataset.keys()):
-                        plot_dataset = self.calculate_fret(plot_dataset)
+                if set(["donor", "acceptor"]).issubset(plot_dataset.keys()):
+                    plot_dataset = self.calculate_fret(plot_dataset)
+                    try:
+                        plot_dataset["fret data"] = {"Donor": plot_dataset["donor"]["Donor"],
+                                                     "Acceptor": plot_dataset["acceptor"]["Acceptor"]}#
+                    except:
+                        pass
 
         except:
             print(traceback.format_exc())
 
         return plot_dataset
 
     def calculate_fret(self, plot_dataset):
         try:
             donor_data = plot_dataset["donor"]
             acceptor_data = plot_dataset["acceptor"]
 
             for shape_index, (donor, acceptor) in enumerate(zip(donor_data.values(), acceptor_data.values())):
-                if "fret" not in plot_dataset.keys():
-                    plot_dataset["fret"] = {}
+                if "fret efficiency" not in plot_dataset.keys():
+                    plot_dataset["fret efficiency"] = {}
 
                 fret = acceptor / (donor + acceptor)
-                plot_dataset["fret"][shape_index] = fret
+                plot_dataset["fret efficiency"] = {"FRET Efficiency": fret}
 
         except:
             print(traceback.format_exc())
 
         return plot_dataset
 
     def draw_line_plot(self):
         try:
             plot_mode = self.gui.plot_mode.currentIndex()
             plot_channel = self.gui.plot_channel.currentText()
 
-            if "efficiency" in plot_channel.lower():
-                plot_channel = "fret"
-
             plot_dataset = self.get_plot_data()
 
             self.graph_canvas.clear()
 
             if plot_channel.lower() in plot_dataset.keys():
                 plot_data = plot_dataset[plot_channel.lower()]
 
@@ -262,24 +258,33 @@
                         plot_title = "Line profile(s)"
                     if plot_mode == 1:
                         plot_title = "Line profile(s)"
                     if plot_mode == 2:
                         plot_title = "Single Molecule Time Series"
 
                     ax = self.graph_canvas.addPlot(title=plot_title)
+                    #add legend
+                    ax.addLegend()
 
-                    for y_data in plot_data.values():
+                    for label, data in plot_data.items():
 
-                        y_data  = np.array(y_data)
+                        y_data  = np.array(data)
                         x_data = np.arange(len(y_data))
 
+                        if label.lower() == "donor":
+                            colour = (255, 0, 0)
+                        if label.lower() == "acceptor":
+                            colour = (0, 255, 0)
+                        if label.lower() == "fret efficiency":
+                            colour = (0, 0, 255)
+
                         if plot_mode in [0, 1]:
-                            ax.plot(x_data, y_data, pen=(255, 0, 0), symbol="o", symbolPen=(255, 0, 0))
+                            ax.plot(x_data, y_data, pen=colour, symbol="o", symbolPen=(255, 255, 255))
                         else:
-                            ax.plot(x_data, y_data, pen=(255, 0, 0))
+                            ax.plot(x_data, y_data, pen=colour)
 
                         if plot_mode == 1:
                             try:
                                 fitX, fitY, peak_width = self.fit_custom_gaussian(x_data, y_data)
                                 ax.plot(fitX, fitY, pen=(0, 255, 0))
                                 text = pg.TextItem(f"Peak FWHM {peak_width:.2f}", color=(200, 200, 200))
                                 ax.addItem(text)
```

### Comparing `napari_smlmlab-0.0.7/src/smlmlab/gui.py` & `napari_smlmlab-0.0.8/src/smlmlab/gui.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.7/src/smlmlab/utils/compute_utils.py` & `napari_smlmlab-0.0.8/src/smlmlab/utils/compute_utils.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.7/src/smlmlab/utils/events_utils.py` & `napari_smlmlab-0.0.8/src/smlmlab/utils/events_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -289,15 +289,17 @@
 
             self.draw_molecules(update_vis=True)
             self.update_overlay_text()
 
         except:
             print(traceback.format_exc())
 
-    def update_channel_selector(self, dataset_selector, channel_selector, event=None, channel_type="all", efficiency=False, block_signals=False, ):
+    def update_channel_selector(self, dataset_selector, channel_selector, event=None, channel_type="all", efficiency=False,
+            all_datasets = True, block_signals=False, ):
+
         try:
             if self.verbose:
                 print(f"Updating channel selector for dataset {dataset_selector} and channel {channel_selector}")
 
             if hasattr(self.gui, channel_selector) and hasattr(self.gui, dataset_selector):
                 channel_selector = getattr(self.gui, channel_selector)
                 dataset_selector = getattr(self.gui, dataset_selector)
@@ -320,21 +322,17 @@
                     for channel in channel_names:
                         if "efficiency" not in channel.lower():
                             if channel in ["da", "dd", "aa", "ad"]:
                                 channel_selector_list.append(channel.upper())
                             elif channel in ["donor", "acceptor"]:
                                 channel_selector_list.append(channel.capitalize())
 
-                            if efficiency == True:
-                                if set(["donor", "acceptor"]).issubset(set(channel_names)):
-                                    channel_selector_list.append("FRET Efficiency")
-                                if set(["dd", "da"]).issubset(set(channel_names)):
-                                    channel_selector_list.append("ALEX Efficiency")
 
-                elif dataset_name == "All Datasets":
+
+                elif dataset_name == "All Datasets" and all_datasets == True:
                     channel_names = []
 
                     for dataset_name in self.dataset_dict.keys():
                         dataset_channels = [channel.lower() for channel in self.dataset_dict[dataset_name].keys()]
                         channel_names.append(dataset_channels)
 
                     channel_names = list(set.intersection(*map(set, channel_names)))
@@ -350,16 +348,26 @@
                                 if set(["donor", "acceptor"]).issubset(set(channel_names)):
                                     channel_selector_list.append("FRET Efficiency")
                                 if set(["dd", "da"]).issubset(set(channel_names)):
                                     channel_selector_list.append("ALEX Efficiency")
 
 
                 if channel_selector_list != []:
-                    channel_selector.clear()
+
                     channel_selector_list = list(set(channel_selector_list))
+
+                    if efficiency == True:
+                        if set(["Donor", "Acceptor"]).issubset(set(channel_selector_list)):
+                            channel_selector_list.append("FRET Data")
+                            channel_selector_list.append("FRET Efficiency")
+                        if set(["DD", "DA"]).issubset(set(channel_selector_list)):
+                            channel_selector_list.append("ALEX Data")
+                            channel_selector_list.append("ALEX Efficiency")
+
+                    channel_selector.clear()
                     channel_selector.addItems(channel_selector_list)
 
                 channel_selector.blockSignals(False)
 
         except:
             print(traceback.format_exc())
```

### Comparing `napari_smlmlab-0.0.7/src/smlmlab/utils/import_utils.py` & `napari_smlmlab-0.0.8/src/smlmlab/utils/import_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -397,27 +397,27 @@
 
             self.closed_import_shared_images()
 
         except:
             print(traceback.format_exc())
             self.update_ui()
 
-    def populate_dataset_combos(self):
+    def populate_dataset_combos(self, all_datasets=False):
         try:
             if self.verbose:
                 print("Populating all dataset combos.")
 
             dataset_names = list(self.dataset_dict.keys())
 
             self.gui.dataset_selector.blockSignals(True)
             self.gui.dataset_selector.clear()
             self.gui.dataset_selector.addItems(dataset_names)
             self.gui.dataset_selector.blockSignals(False)
 
-            if len(dataset_names) > 1:
+            if len(dataset_names) > 1 and all_datasets == True:
                 dataset_names.insert(0, "All Datasets")
 
             self.gui.picasso_dataset.blockSignals(True)
             self.gui.picasso_dataset.clear()
             self.gui.picasso_dataset.addItems(dataset_names)
             self.gui.picasso_dataset.blockSignals(False)
```

### Comparing `napari_smlmlab-0.0.7/src/smlmlab/utils/loc_utils.py` & `napari_smlmlab-0.0.8/src/smlmlab/utils/loc_utils.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.7/src/smlmlab/utils/picasso_utils.py` & `napari_smlmlab-0.0.8/src/smlmlab/utils/picasso_utils.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.7/src/smlmlab/utils/undrift_utils.py` & `napari_smlmlab-0.0.8/src/smlmlab/utils/undrift_utils.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.7/src/smlmlab/utils/viewer_utils.py` & `napari_smlmlab-0.0.8/src/smlmlab/utils/viewer_utils.py`

 * *Files identical despite different names*

