# Comparing `tmp/labgym-2.4.4.tar.gz` & `tmp/labgym-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labgym-2.4.4.tar", last modified: Tue Apr 16 02:19:47 2024, max compression
+gzip compressed data, was "labgym-2.4.5.tar", last modified: Tue Apr 30 21:57:18 2024, max compression
```

## Comparing `labgym-2.4.4.tar` & `labgym-2.4.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    31919 2024-04-16 02:19:42.956648 labgym-2.4.4/LICENSE.txt
--rw-r--r--   0        0        0      417 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/COPYRIGHT.txt
--rw-r--r--   0        0        0      131 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/NOTICE.txt
--rw-r--r--   0        0        0      882 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/__init__.py
--rw-r--r--   0        0        0     1985 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/__main__.py
--rw-r--r--   0        0        0    87666 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/analyzebehaviors.py
--rw-r--r--   0        0        0   173802 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/analyzebehaviorsdetector.py
--rw-r--r--   0        0        0    68079 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/categorizers.py
--rw-r--r--   0        0        0    13019 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/detector.py
--rw-r--r--   0        0        0      859 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/detectors/__init__.py
--rw-r--r--   0        0        0      889 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/gui/__init__.py
--rw-r--r--   0        0        0      904 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/gui/analysis/__init__.py
--rw-r--r--   0        0        0     2115 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/gui/analysis/analysis_module.py
--rw-r--r--   0        0        0    67907 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/gui/analysis/analyze_behaviors.py
--rw-r--r--   0        0        0     7276 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/gui/analysis/behavior_plot.py
--rw-r--r--   0        0        0     9322 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/gui/analysis/mine_results.py
--rw-r--r--   0        0        0     4833 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/gui/main_window.py
--rw-r--r--   0        0        0    22593 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/gui/preprocessing.py
--rw-r--r--   0        0        0      904 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/gui/training/__init__.py
--rw-r--r--   0        0        0    51881 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/gui/training/behavior_examples.py
--rw-r--r--   0        0        0    33348 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/gui/training/categorizers.py
--rw-r--r--   0        0        0    22300 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/gui/training/detectors.py
--rw-r--r--   0        0        0     5203 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/gui/training/training_module.py
--rw-r--r--   0        0        0     4473 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/gui/utils.py
--rw-r--r--   0        0        0     8091 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/minedata.py
--rw-r--r--   0        0        0      859 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/models/__init__.py
--rw-r--r--   0        0        0    49154 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/tools.py
--rw-r--r--   0        0        0      131 2024-04-16 02:19:42.960648 labgym-2.4.4/NOTICE.txt
--rw-r--r--   0        0        0    13320 2024-04-16 02:19:42.960648 labgym-2.4.4/README.md
--rw-r--r--   0        0        0     2172 2024-04-16 02:19:47.984604 labgym-2.4.4/pyproject.toml
--rw-r--r--   0        0        0      859 2024-04-16 02:19:42.968648 labgym-2.4.4/tests/__init__.py
--rw-r--r--   0        0        0     1165 2024-04-16 02:19:42.968648 labgym-2.4.4/tests/test_main.py
--rw-r--r--   0        0        0     1093 2024-04-16 02:19:42.968648 labgym-2.4.4/tests/test_tools.py
--rw-r--r--   0        0        0    14874 1970-01-01 00:00:00.000000 labgym-2.4.4/PKG-INFO
+-rw-r--r--   0        0        0    31919 2024-04-30 21:57:12.443982 labgym-2.4.5/LICENSE.txt
+-rw-r--r--   0        0        0      417 2024-04-30 21:57:12.443982 labgym-2.4.5/LabGym/COPYRIGHT.txt
+-rw-r--r--   0        0        0      131 2024-04-30 21:57:12.443982 labgym-2.4.5/LabGym/NOTICE.txt
+-rw-r--r--   0        0        0      882 2024-04-30 21:57:12.443982 labgym-2.4.5/LabGym/__init__.py
+-rw-r--r--   0        0        0     1985 2024-04-30 21:57:12.443982 labgym-2.4.5/LabGym/__main__.py
+-rw-r--r--   0        0        0    87666 2024-04-30 21:57:12.443982 labgym-2.4.5/LabGym/analyzebehaviors.py
+-rw-r--r--   0        0        0   173802 2024-04-30 21:57:12.443982 labgym-2.4.5/LabGym/analyzebehaviorsdetector.py
+-rw-r--r--   0        0        0    68079 2024-04-30 21:57:12.443982 labgym-2.4.5/LabGym/categorizers.py
+-rw-r--r--   0        0        0    13019 2024-04-30 21:57:12.447982 labgym-2.4.5/LabGym/detector.py
+-rw-r--r--   0        0        0      859 2024-04-30 21:57:12.447982 labgym-2.4.5/LabGym/detectors/__init__.py
+-rw-r--r--   0        0        0      889 2024-04-30 21:57:12.447982 labgym-2.4.5/LabGym/gui/__init__.py
+-rw-r--r--   0        0        0      904 2024-04-30 21:57:12.447982 labgym-2.4.5/LabGym/gui/analysis/__init__.py
+-rw-r--r--   0        0        0     2115 2024-04-30 21:57:12.447982 labgym-2.4.5/LabGym/gui/analysis/analysis_module.py
+-rw-r--r--   0        0        0    67907 2024-04-30 21:57:12.447982 labgym-2.4.5/LabGym/gui/analysis/analyze_behaviors.py
+-rw-r--r--   0        0        0     7276 2024-04-30 21:57:12.447982 labgym-2.4.5/LabGym/gui/analysis/behavior_plot.py
+-rw-r--r--   0        0        0     9322 2024-04-30 21:57:12.447982 labgym-2.4.5/LabGym/gui/analysis/mine_results.py
+-rw-r--r--   0        0        0     4833 2024-04-30 21:57:12.447982 labgym-2.4.5/LabGym/gui/main_window.py
+-rw-r--r--   0        0        0    22593 2024-04-30 21:57:12.447982 labgym-2.4.5/LabGym/gui/preprocessing.py
+-rw-r--r--   0        0        0      904 2024-04-30 21:57:12.447982 labgym-2.4.5/LabGym/gui/training/__init__.py
+-rw-r--r--   0        0        0    51881 2024-04-30 21:57:12.447982 labgym-2.4.5/LabGym/gui/training/behavior_examples.py
+-rw-r--r--   0        0        0    33321 2024-04-30 21:57:12.447982 labgym-2.4.5/LabGym/gui/training/categorizers.py
+-rw-r--r--   0        0        0    22300 2024-04-30 21:57:12.447982 labgym-2.4.5/LabGym/gui/training/detectors.py
+-rw-r--r--   0        0        0     5203 2024-04-30 21:57:12.447982 labgym-2.4.5/LabGym/gui/training/training_module.py
+-rw-r--r--   0        0        0     4473 2024-04-30 21:57:12.447982 labgym-2.4.5/LabGym/gui/utils.py
+-rw-r--r--   0        0        0     8091 2024-04-30 21:57:12.447982 labgym-2.4.5/LabGym/minedata.py
+-rw-r--r--   0        0        0      859 2024-04-30 21:57:12.447982 labgym-2.4.5/LabGym/models/__init__.py
+-rw-r--r--   0        0        0    49154 2024-04-30 21:57:12.447982 labgym-2.4.5/LabGym/tools.py
+-rw-r--r--   0        0        0      131 2024-04-30 21:57:12.447982 labgym-2.4.5/NOTICE.txt
+-rw-r--r--   0        0        0    13320 2024-04-30 21:57:12.447982 labgym-2.4.5/README.md
+-rw-r--r--   0        0        0     2172 2024-04-30 21:57:18.136057 labgym-2.4.5/pyproject.toml
+-rw-r--r--   0        0        0      859 2024-04-30 21:57:12.455982 labgym-2.4.5/tests/__init__.py
+-rw-r--r--   0        0        0     1165 2024-04-30 21:57:12.455982 labgym-2.4.5/tests/test_main.py
+-rw-r--r--   0        0        0     1093 2024-04-30 21:57:12.455982 labgym-2.4.5/tests/test_tools.py
+-rw-r--r--   0        0        0    14874 1970-01-01 00:00:00.000000 labgym-2.4.5/PKG-INFO
```

### Comparing `labgym-2.4.4/LICENSE.txt` & `labgym-2.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `labgym-2.4.4/LabGym/__init__.py` & `labgym-2.4.5/LabGym/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 210 Washtenaw Avenue, Room 5403
 Ann Arbor, MI 48109-2216
 USA
 
 Email: bingye@umich.edu
 """
 
-__version__ = "2.4.4"
+__version__ = "2.4.5"
```

### Comparing `labgym-2.4.4/LabGym/__main__.py` & `labgym-2.4.5/LabGym/__main__.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.4/LabGym/analyzebehaviors.py` & `labgym-2.4.5/LabGym/analyzebehaviors.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.4/LabGym/analyzebehaviorsdetector.py` & `labgym-2.4.5/LabGym/analyzebehaviorsdetector.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.4/LabGym/categorizers.py` & `labgym-2.4.5/LabGym/categorizers.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.4/LabGym/detector.py` & `labgym-2.4.5/LabGym/detector.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.4/LabGym/detectors/__init__.py` & `labgym-2.4.5/LabGym/detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.4/LabGym/gui/__init__.py` & `labgym-2.4.5/LabGym/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.4/LabGym/gui/analysis/__init__.py` & `labgym-2.4.5/LabGym/gui/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.4/LabGym/gui/analysis/analysis_module.py` & `labgym-2.4.5/LabGym/gui/analysis/analysis_module.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.4/LabGym/gui/analysis/analyze_behaviors.py` & `labgym-2.4.5/LabGym/gui/analysis/analyze_behaviors.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.4/LabGym/gui/analysis/behavior_plot.py` & `labgym-2.4.5/LabGym/gui/analysis/behavior_plot.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.4/LabGym/gui/analysis/mine_results.py` & `labgym-2.4.5/LabGym/gui/analysis/mine_results.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.4/LabGym/gui/main_window.py` & `labgym-2.4.5/LabGym/gui/main_window.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.4/LabGym/gui/preprocessing.py` & `labgym-2.4.5/LabGym/gui/preprocessing.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.4/LabGym/gui/training/__init__.py` & `labgym-2.4.5/LabGym/gui/training/__init__.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.4/LabGym/gui/training/behavior_examples.py` & `labgym-2.4.5/LabGym/gui/training/behavior_examples.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.4/LabGym/gui/training/categorizers.py` & `labgym-2.4.5/LabGym/gui/training/categorizers.py`

 * *Files 0% similar despite different names*

```diff
@@ -338,14 +338,15 @@
         else:
             label_text += " to identify non-interactive behaviors of each individual in static images."
 
         self.text_categorizertype.SetLabel(label_text)
 
     def set_categorizer_shape(self, event):
         """Set the network shape of the categorizer."""
+        self.channel = 3
         if self.using_animation_analyzer is True:
             dialog = wx.NumberEntryDialog(
                 self,
                 "Input dimension of Animation Analyzer\nlarger dimension = wider network",
                 "Enter a number:",
                 "Animation Analyzer input",
                 32,
@@ -355,15 +356,14 @@
             if dialog.ShowModal() != wx.ID_OK:
                 dialog.Destroy()
                 return
             else:
                 self.dim_tconv = int(dialog.GetValue())
                 dialog.Destroy()
 
-            self.channel = 3
             if self.behavior_mode != BehaviorMode.INTERACT_ADVANCED:
                 dialog = wx.MessageDialog(
                     self,
                     'Grayscale input of Animation Analyzer?\nSelect "Yes" if the color of animals is behavior irrelevant.',
                     "Grayscale Animation Analyzer?",
                     wx.YES_NO | wx.ICON_QUESTION,
                 )
@@ -383,15 +383,14 @@
         if dialog.ShowModal() != wx.ID_OK:
             dialog.Destroy()
             return
         else:
             self.dim_conv = int(dialog.GetValue())
             dialog.Destroy()
 
-        self.channel = 3
         if self.behavior_mode == BehaviorMode.STATIC_IMAGES:
             dialog1 = wx.MessageDialog(
                 self,
                 'Grayscale input?\nSelect "Yes" if the color of animals is behavior irrelevant.',
                 "Grayscale inputs?",
                 wx.YES_NO | wx.ICON_QUESTION,
             )
@@ -437,15 +436,15 @@
         """Select the directory with the training examples."""
         dialog = wx.MessageDialog(
             self,
             "Are the animations (in any) in\ntraining examples background free?",
             "Background-free animations?",
             wx.YES_NO | wx.ICON_QUESTION,
         )
-        self.background_free = dialog.ShowModal == wx.ID_YES
+        self.background_free = dialog.ShowModal() == wx.ID_YES
         dialog.Destroy()
 
         self.include_bodyparts = False
         if self.behavior_mode != BehaviorMode.STATIC_IMAGES:
             dialog = wx.MessageDialog(
                 self,
                 "Do the pattern images in training examples\ninclude body parts?",
```

### Comparing `labgym-2.4.4/LabGym/gui/training/detectors.py` & `labgym-2.4.5/LabGym/gui/training/detectors.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.4/LabGym/gui/training/training_module.py` & `labgym-2.4.5/LabGym/gui/training/training_module.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.4/LabGym/gui/utils.py` & `labgym-2.4.5/LabGym/gui/utils.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.4/LabGym/minedata.py` & `labgym-2.4.5/LabGym/minedata.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.4/LabGym/models/__init__.py` & `labgym-2.4.5/LabGym/models/__init__.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.4/LabGym/tools.py` & `labgym-2.4.5/LabGym/tools.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.4/README.md` & `labgym-2.4.5/README.md`

 * *Files identical despite different names*

### Comparing `labgym-2.4.4/pyproject.toml` & `labgym-2.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dynamic = []
-version = "2.4.4"
+version = "2.4.5"
 
 [project.license]
 text = "GPL-3.0"
 
 [project.urls]
 Homepage = "http://github.com/umyelab/LabGym"
 Documentation = "https://labgym.readthedocs.io/en/latest/"
```

### Comparing `labgym-2.4.4/tests/__init__.py` & `labgym-2.4.5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.4/tests/test_main.py` & `labgym-2.4.5/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.4/tests/test_tools.py` & `labgym-2.4.5/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.4/PKG-INFO` & `labgym-2.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LabGym
-Version: 2.4.4
+Version: 2.4.5
 Summary: Quantify user-defined behaviors.
 Keywords: behavior analysis,behavioral analysis,user defined behaviors
 Author-Email: Yujia Hu <henryhu@umich.edu>, Rohan Satapathy <rohansat@umich.edu>, "M. Victor Struman" <strmark@umich.edu>, Kelly Goss <khgoss@umich.edu>, Isabelle Baker <ibaker@umich.edu>
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

