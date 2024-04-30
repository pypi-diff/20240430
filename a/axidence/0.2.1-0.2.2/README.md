# Comparing `tmp/axidence-0.2.1.tar.gz` & `tmp/axidence-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axidence-0.2.1.tar", max compression
+gzip compressed data, was "axidence-0.2.2.tar", max compression
```

## Comparing `axidence-0.2.1.tar` & `axidence-0.2.2.tar`

### file list

```diff
@@ -1,27 +1,30 @@
--rw-r--r--   0        0        0     1522 2024-04-28 13:07:20.656960 axidence-0.2.1/LICENSE
--rw-r--r--   0        0        0     1046 2024-04-28 13:07:20.656960 axidence-0.2.1/README.md
--rw-r--r--   0        0        0      181 2024-04-28 13:07:20.656960 axidence-0.2.1/axidence/__init__.py
--rw-r--r--   0        0        0     6907 2024-04-28 13:07:20.656960 axidence-0.2.1/axidence/context.py
--rw-r--r--   0        0        0     2173 2024-04-28 13:07:20.656960 axidence-0.2.1/axidence/dtypes.py
--rw-r--r--   0        0        0     2001 2024-04-28 13:07:20.656960 axidence-0.2.1/axidence/plugin.py
--rw-r--r--   0        0        0      179 2024-04-28 13:07:20.656960 axidence-0.2.1/axidence/plugins/__init__.py
--rw-r--r--   0        0        0      259 2024-04-28 13:07:20.656960 axidence-0.2.1/axidence/plugins/cuts/__init__.py
--rw-r--r--   0        0        0      412 2024-04-28 13:07:20.656960 axidence-0.2.1/axidence/plugins/cuts/cut_event_building.py
--rw-r--r--   0        0        0     1001 2024-04-28 13:07:20.656960 axidence-0.2.1/axidence/plugins/cuts/cut_isolated_s1.py
--rw-r--r--   0        0        0      981 2024-04-28 13:07:20.656960 axidence-0.2.1/axidence/plugins/cuts/cut_isolated_s2.py
--rw-r--r--   0        0        0      545 2024-04-28 13:07:20.656960 axidence-0.2.1/axidence/plugins/cuts/cut_pairing_exists.py
--rw-r--r--   0        0        0      107 2024-04-28 13:07:20.660960 axidence-0.2.1/axidence/plugins/isolated/__init__.py
--rw-r--r--   0        0        0     1674 2024-04-28 13:07:20.660960 axidence-0.2.1/axidence/plugins/isolated/isolated_s1.py
--rw-r--r--   0        0        0     2918 2024-04-28 13:07:20.660960 axidence-0.2.1/axidence/plugins/isolated/isolated_s2.py
--rw-r--r--   0        0        0      113 2024-04-28 13:07:20.660960 axidence-0.2.1/axidence/plugins/pairing/__init__.py
--rw-r--r--   0        0        0     7253 2024-04-28 13:07:20.660960 axidence-0.2.1/axidence/plugins/pairing/events_paired.py
--rw-r--r--   0        0        0    19628 2024-04-28 13:07:20.660960 axidence-0.2.1/axidence/plugins/pairing/peaks_paired.py
--rw-r--r--   0        0        0      295 2024-04-28 13:07:20.660960 axidence-0.2.1/axidence/plugins/salting/__init__.py
--rw-r--r--   0        0        0     6638 2024-04-28 13:07:20.660960 axidence-0.2.1/axidence/plugins/salting/event_building.py
--rw-r--r--   0        0        0     1728 2024-04-28 13:07:20.660960 axidence-0.2.1/axidence/plugins/salting/event_fields.py
--rw-r--r--   0        0        0     8038 2024-04-28 13:07:20.660960 axidence-0.2.1/axidence/plugins/salting/events_salting.py
--rw-r--r--   0        0        0     4028 2024-04-28 13:07:20.660960 axidence-0.2.1/axidence/plugins/salting/peak_correlation.py
--rw-r--r--   0        0        0     2678 2024-04-28 13:07:20.660960 axidence-0.2.1/axidence/plugins/salting/peaks_salted.py
--rw-r--r--   0        0        0     2593 2024-04-28 13:07:20.660960 axidence-0.2.1/axidence/utils.py
--rw-r--r--   0        0        0      907 2024-04-28 13:07:20.660960 axidence-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2417 1970-01-01 00:00:00.000000 axidence-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1522 2024-04-30 21:22:48.104117 axidence-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1046 2024-04-30 21:22:48.104117 axidence-0.2.2/README.md
+-rw-r--r--   0        0        0      206 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/__init__.py
+-rw-r--r--   0        0        0     8260 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/context.py
+-rw-r--r--   0        0        0     2239 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/dtypes.py
+-rw-r--r--   0        0        0     2001 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugin.py
+-rw-r--r--   0        0        0      219 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/__init__.py
+-rw-r--r--   0        0        0      259 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/cuts/__init__.py
+-rw-r--r--   0        0        0      959 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/cuts/cut_event_building.py
+-rw-r--r--   0        0        0     1001 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/cuts/cut_isolated_s1.py
+-rw-r--r--   0        0        0      981 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/cuts/cut_isolated_s2.py
+-rw-r--r--   0        0        0      545 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/cuts/cut_pairing_exists.py
+-rw-r--r--   0        0        0      107 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/isolated/__init__.py
+-rw-r--r--   0        0        0     1674 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/isolated/isolated_s1.py
+-rw-r--r--   0        0        0     2918 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/isolated/isolated_s2.py
+-rw-r--r--   0        0        0       47 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/meta/__init__.py
+-rw-r--r--   0        0        0      505 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/meta/run_meta.py
+-rw-r--r--   0        0        0      113 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/pairing/__init__.py
+-rw-r--r--   0        0        0     7404 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/pairing/events_paired.py
+-rw-r--r--   0        0        0    33786 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/pairing/peaks_paired.py
+-rw-r--r--   0        0        0      295 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/salting/__init__.py
+-rw-r--r--   0        0        0     7283 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/salting/event_building.py
+-rw-r--r--   0        0        0     1935 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/salting/event_fields.py
+-rw-r--r--   0        0        0     7813 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/salting/events_salting.py
+-rw-r--r--   0        0        0     4841 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/salting/peak_correlation.py
+-rw-r--r--   0        0        0     3109 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/plugins/salting/peaks_salted.py
+-rw-r--r--   0        0        0     1964 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/samplers.py
+-rw-r--r--   0        0        0     2593 2024-04-30 21:22:48.108117 axidence-0.2.2/axidence/utils.py
+-rw-r--r--   0        0        0      933 2024-04-30 21:22:48.108117 axidence-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2456 1970-01-01 00:00:00.000000 axidence-0.2.2/PKG-INFO
```

### Comparing `axidence-0.2.1/LICENSE` & `axidence-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `axidence-0.2.1/README.md` & `axidence-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `axidence-0.2.1/axidence/context.py` & `axidence-0.2.2/axidence/context.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 from immutabledict import immutabledict
 from tqdm import tqdm
+import numpy as np
 import strax
+from strax import CutPlugin, CutList
 import straxen
 
-from axidence import EventsSalting, PeaksSalted
+from axidence import RunMeta, EventsSalting, PeaksSalted
 from axidence import (
     PeakProximitySalted,
     PeakShadowSalted,
     PeakAmbienceSalted,
+    PeakNearestTriggeringSalted,
     PeakSEDensitySalted,
 )
 from axidence import (
     EventsSalted,
     EventBasicsSalted,
     EventShadowSalted,
     EventAmbienceSalted,
+    EventNearestTriggeringSalted,
     EventSEDensitySalted,
+    MainS1Trigger,
+    MainS2Trigger,
     EventBuilding,
 )
 from axidence import (
     IsolatedS1Mask,
     IsolatedS2Mask,
     IsolatedS1,
     IsolatedS2,
@@ -76,15 +82,15 @@
             for attr in assign_attributes[plugin.__name__]:
                 setattr(new_plugin, attr, getattr(p, attr))
 
         # assign the same attributes as the original plugin
         if hasattr(p, "depends_on"):
             new_plugin.depends_on = tuple(d + snake for d in p.depends_on)
         else:
-            raise RuntimeError
+            raise RuntimeError(f"depends_on is not defined for instance of {plugin.__name__}")
 
         if hasattr(p, "provides"):
             new_plugin.provides = tuple(p + snake for p in p.provides)
         else:
             snake_name = strax.camel_to_snake(new_plugin.__name__)
             new_plugin.provides = (snake_name,)
 
@@ -108,14 +114,37 @@
             raise RuntimeError(f"save_when is not defined for instance of {plugin.__name__}")
 
         if isinstance(p.dtype, (dict, immutabledict)):
             new_plugin.dtype = dict(zip([k + snake for k in p.dtype.keys()], p.dtype.values()))
         else:
             new_plugin.dtype = p.dtype
 
+        if isinstance(p, CutPlugin):
+            if hasattr(p, "cut_name"):
+                new_plugin.cut_name = p.cut_name + snake
+            else:
+                raise RuntimeError(f"cut_name is not defined for instance of {plugin.__name__}")
+
+        if isinstance(p, CutList):
+            if hasattr(p, "accumulated_cuts_string"):
+                new_plugin.accumulated_cuts_string = p.accumulated_cuts_string + snake
+            else:
+                raise RuntimeError(
+                    f"accumulated_cuts_string is not defined for instance of {plugin.__name__}"
+                )
+
+        if isinstance(p, CutPlugin) or isinstance(p, CutList):
+            # this will make CutList.cuts to be invalid
+            new_plugin.dtype = np.dtype(
+                [
+                    ((d[0][0], d[0][1] + snake), d[1]) if d[0][1] not in ["time", "endtime"] else d
+                    for d in new_plugin.dtype.descr
+                ]
+            )
+
         new_plugins.append(new_plugin)
     return new_plugins
 
 
 @strax.Context.add_method
 def replication_tree(st, suffixes=["Paired", "Salted"], assign_attributes=None, tqdm_disable=True):
     """Replicate the dependency tree.
@@ -141,24 +170,27 @@
 
 
 @strax.Context.add_method
 def _salt_to_context(self):
     """Register the salted plugins to the context."""
     self.register(
         (
+            RunMeta,
             EventsSalting,
             PeaksSalted,
             PeakProximitySalted,
             PeakShadowSalted,
             PeakAmbienceSalted,
+            PeakNearestTriggeringSalted,
             PeakSEDensitySalted,
             EventsSalted,
             EventBasicsSalted,
             EventShadowSalted,
             EventAmbienceSalted,
+            EventNearestTriggeringSalted,
             EventSEDensitySalted,
         )
     )
 
 
 @strax.Context.add_method
 def _pair_to_context(self):
@@ -177,21 +209,21 @@
         )
     )
 
 
 @strax.Context.add_method
 def salt_to_context(st, assign_attributes=None, tqdm_disable=True):
     """Register the salted plugins to the context."""
-    st.register((EventBuilding,))
+    st.register((MainS1Trigger, MainS2Trigger, EventBuilding))
     st.replication_tree(
         suffixes=["Salted"], assign_attributes=assign_attributes, tqdm_disable=tqdm_disable
     )
     st._salt_to_context()
 
 
 @strax.Context.add_method
 def salt_and_pair_to_context(st, assign_attributes=None, tqdm_disable=True):
     """Register the salted and paired plugins to the context."""
-    st.register((EventBuilding,))
+    st.register((MainS1Trigger, MainS2Trigger, EventBuilding))
     st.replication_tree(assign_attributes=assign_attributes, tqdm_disable=tqdm_disable)
     st._salt_to_context()
     st._pair_to_context()
```

### Comparing `axidence-0.2.1/axidence/dtypes.py` & `axidence-0.2.2/axidence/dtypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 import straxen
 
 from straxen.misc import kind_colors
 
 
 kind_colors.update(
     {
+        "run_meta": "#ffff00",
         "events_salting": "#0080ff",
         "peaks_salted": "#00c0ff",
         "events_salted": "#00ffff",
         "peaks_paired": "#ff00ff",
+        "truth_paired": "#ff00ff",
         "events_paired": "#ffccff",
         "isolated_s1": "#80ff00",
         "isolated_s2": "#80ff00",
     }
 )
```

### Comparing `axidence-0.2.1/axidence/plugin.py` & `axidence-0.2.2/axidence/plugin.py`

 * *Files identical despite different names*

### Comparing `axidence-0.2.1/axidence/plugins/cuts/cut_isolated_s1.py` & `axidence-0.2.2/axidence/plugins/cuts/cut_isolated_s1.py`

 * *Files identical despite different names*

### Comparing `axidence-0.2.1/axidence/plugins/cuts/cut_isolated_s2.py` & `axidence-0.2.2/axidence/plugins/cuts/cut_isolated_s2.py`

 * *Files identical despite different names*

### Comparing `axidence-0.2.1/axidence/plugins/cuts/cut_pairing_exists.py` & `axidence-0.2.2/axidence/plugins/cuts/cut_pairing_exists.py`

 * *Files identical despite different names*

### Comparing `axidence-0.2.1/axidence/plugins/isolated/isolated_s1.py` & `axidence-0.2.2/axidence/plugins/isolated/isolated_s1.py`

 * *Files identical despite different names*

### Comparing `axidence-0.2.1/axidence/plugins/isolated/isolated_s2.py` & `axidence-0.2.2/axidence/plugins/isolated/isolated_s2.py`

 * *Files identical despite different names*

### Comparing `axidence-0.2.1/axidence/plugins/pairing/events_paired.py` & `axidence-0.2.2/axidence/plugins/pairing/events_paired.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,28 +14,28 @@
     used in AC simulation, but just for debug."""
 
     depends_on = "peaks_paired"
     provides = "events_paired"
     data_kind = "events_paired"
     save_when = strax.SaveWhen.EXPLICIT
 
-    paring_event_interval = straxen.URLConfig(
+    paring_time_interval = straxen.URLConfig(
         default=int(1e8),
         type=int,
         help="The interval which separates two events S1 [ns]",
     )
 
     def infer_dtype(self):
         dtype_reference = strax.unpack_dtype(self.deps["peaks_paired"].dtype_for("peaks_paired"))
         required_names = ["time", "endtime", "event_number"]
         dtype = copy_dtype(dtype_reference, required_names)
         return dtype
 
     def get_window_size(self):
-        return 10 * self.paring_event_interval
+        return 10 * self.paring_time_interval
 
     def compute(self, peaks_paired):
         peaks_event_number_sorted = np.sort(peaks_paired, order=("event_number", "time"))
         event_number, event_number_index, event_number_count = np.unique(
             peaks_event_number_sorted["event_number"], return_index=True, return_counts=True
         )
         event_number_index = np.append(event_number_index, len(peaks_event_number_sorted))
@@ -112,14 +112,15 @@
                 ]
         dtype += [
             (
                 ("Type of event indicating whether the isolated S1 becomes main S1", "event_type"),
                 np.int8,
             ),
             (("Event number in this dataset", "event_number"), np.int64),
+            (("Normalization of number of paired events", "normalization"), np.float32),
         ]
         return dtype
 
     def infer_dtype(self):
         return strax.merged_dtype(
             [
                 self.deps["event_info_paired"].dtype_for("event_info_paired"),
@@ -143,14 +144,15 @@
             if np.unique(sp["event_number"]).size != 1:
                 raise ValueError(
                     f"Event {i} has multiple event numbers: "
                     f"{np.unique(sp['event_number'])}. "
                     "Maybe the paired events overlap."
                 )
             result["event_number"][i] = sp["event_number"][0]
+            result["normalization"][i] = sp["normalization"][0]
             for idx, main_peak in zip([event["s1_index"], event["s2_index"]], ["s1_", "s2_"]):
                 if idx >= 0:
                     for n in self.peak_fields:
                         result[main_peak + n][i] = sp[n][idx]
             for idx, main_peak in zip(
                 [event["alt_s1_index"], event["alt_s2_index"]], ["alt_s1_", "alt_s2_"]
             ):
```

### Comparing `axidence-0.2.1/axidence/plugins/salting/event_building.py` & `axidence-0.2.2/axidence/plugins/salting/event_building.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,44 @@
+import warnings
 from typing import Tuple
 import numpy as np
 import strax
 import straxen
 from straxen import Events, EventBasics
 
 from ...utils import needed_dtype, merge_salted_real
 from ...plugin import ExhaustPlugin
 
 
 class EventsSalted(Events, ExhaustPlugin):
     __version__ = "0.1.0"
+    child_plugin = True
     depends_on = ("peaks_salted", "peak_proximity_salted", "peak_basics", "peak_proximity")
     provides = "events_salted"
     data_kind = "events_salted"
     save_when = strax.SaveWhen.EXPLICIT
 
     n_drift_time_window = straxen.URLConfig(
         default=5,
         type=int,
         help="How many max drift time will the event builder extend",
     )
 
+    only_salt_s1 = straxen.URLConfig(
+        default=False,
+        type=bool,
+        help="Whether only salt S1",
+    )
+
+    only_salt_s2 = straxen.URLConfig(
+        default=False,
+        type=bool,
+        help="Whether only salt S2",
+    )
+
     def __init__(self):
         super().__init__()
         self.dtype = super().dtype + [
             (("Salting number of events", "salt_number"), np.int64),
             (("Whether the salting event can trigger", "is_triggering"), bool),
         ]
 
@@ -54,28 +68,38 @@
             raise ValueError(
                 "Expected salt_number to start from 0 because "
                 f"{self.__class__.__name__} is a ExhaustPlugin plugin!"
             )
 
         _peaks = merge_salted_real(peaks_salted, peaks, self._peaks_dtype)
 
-        # use S2s as anchors
-        anchor_peaks = peaks_salted[1::2]
+        if self.only_salt_s1 or self.only_salt_s2:
+            anchor_peaks = peaks_salted
+        else:
+            # use S2s as anchors by default
+            anchor_peaks = peaks_salted[1::2]
+
+        # check if the salting anchor can trigger
+        if self.only_salt_s1:
+            is_triggering = np.full(len(anchor_peaks), False)
+        else:
+            is_triggering = np.full(len(anchor_peaks), False)
+
         if np.unique(anchor_peaks["type"]).size != 1:
             raise ValueError("Expected only one type of anchor peaks!")
 
         # initial the final result
-        n_events = len(peaks_salted) // 2
+        if self.only_salt_s1 or self.only_salt_s2:
+            n_events = len(peaks_salted)
+        else:
+            n_events = len(peaks_salted) // 2
         if np.unique(peaks_salted["salt_number"]).size != n_events:
             raise ValueError("Expected salt_number to be half of the input peaks number!")
         result = np.empty(n_events, self.dtype)
 
-        # check if the salting anchor can trigger
-        is_triggering = self._is_triggering(anchor_peaks)
-
         # prepare for an empty event
         empty_events = np.empty(len(anchor_peaks), dtype=self.dtype)
         empty_events["time"] = anchor_peaks["time"]
         empty_events["endtime"] = anchor_peaks["endtime"]
 
         # build events at once because if a messy environment
         # make the two anchor in the same event
@@ -97,24 +121,25 @@
         if not np.all(np.diff(_result["time"]) >= 0):
             raise ValueError("Expected the result to be sorted!")
         for n in _result.dtype.names:
             result[n] = _result[n]
 
         # assign the most important parameters
         result["is_triggering"] = is_triggering
-        result["salt_number"] = peaks_salted["salt_number"][::2]
-        result["event_number"] = peaks_salted["salt_number"][::2]
+        result["salt_number"] = np.unique(peaks_salted["salt_number"])
+        result["event_number"] = result["salt_number"]
 
         if np.any(np.diff(result["time"]) < 0):
             raise ValueError("Expected time to be sorted!")
         return result
 
 
 class EventBasicsSalted(EventBasics, ExhaustPlugin):
     __version__ = "0.0.0"
+    child_plugin = True
     depends_on: Tuple[str, ...] = (
         "events_salted",
         "peaks_salted",
         "peak_proximity_salted",
         "peak_basics",
         "peak_proximity",
         "peak_positions",
@@ -164,10 +189,11 @@
         result["endtime"] = events_salted["endtime"]
         result["salt_number"] = events_salted["salt_number"]
         result["event_number"] = events_salted["event_number"]
 
         self.fill_events(result, events_salted, split_peaks)
         result["is_triggering"] = events_salted["is_triggering"]
 
-        if np.all(result["s1_salt_number"] < 0) or np.all(result["s2_salt_number"] < 0):
-            raise ValueError("Found zero triggered salted peaks!")
+        for i in [1, 2]:
+            if np.all(result[f"s{i}_salt_number"] < 0):
+                warnings.warn(f"Found zero triggered salted S{i}!")
         return result
```

### Comparing `axidence-0.2.1/axidence/plugins/salting/events_salting.py` & `axidence-0.2.2/axidence/plugins/salting/events_salting.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,76 +1,60 @@
-from typing import Tuple
 import numpy as np
 import strax
+from strax import DownChunkingPlugin
 import straxen
 from straxen import units, EventBasics, EventPositions
 
 from ...utils import copy_dtype
-from ...plugin import RunMetaPlugin
+from ...samplers import SAMPLERS
+from ...plugin import ExhaustPlugin
 
 
-class EventsSalting(EventPositions, EventBasics, RunMetaPlugin):
+class EventsSalting(ExhaustPlugin, DownChunkingPlugin, EventPositions, EventBasics):
     __version__ = "0.0.0"
-    depends_on: Tuple = tuple()
+    child_plugin = True
+    depends_on = "run_meta"
     provides = "events_salting"
     data_kind = "events_salting"
     save_when = strax.SaveWhen.EXPLICIT
 
     salting_seed = straxen.URLConfig(
         default=None,
         type=(int, None),
         help="Seed for salting",
     )
 
     salting_rate = straxen.URLConfig(
-        default=10,
+        default=20,
         type=(int, float),
         help="Rate of salting in Hz",
     )
 
-    real_run_start = straxen.URLConfig(
-        default=None,
-        type=(int, None),
-        help="Real start time of run [ns]",
-    )
-
-    real_run_end = straxen.URLConfig(
-        default=None,
-        type=(int, None),
-        help="Real start time of run [ns]",
-    )
-
-    strict_real_run_time_check = straxen.URLConfig(
-        default=True,
-        type=bool,
-        help="Whether to strictly check the real run time is provided",
-    )
-
     s1_area_range = straxen.URLConfig(
         default=(1, 150),
         type=(list, tuple),
-        help="Range of S1 area",
+        help="Range of S1 area in salting",
     )
 
     s2_area_range = straxen.URLConfig(
         default=(1e2, 2e4),
         type=(list, tuple),
-        help="Range of S2 area",
+        help="Range of S2 area in salting",
     )
 
     s1_distribution = straxen.URLConfig(
-        default="",
+        default="exponential",
         type=str,
-        help="S1 distribution shape",
+        help="S1 distribution shape in salting",
     )
 
     s2_distribution = straxen.URLConfig(
-        default="",
+        default="exponential",
         type=str,
-        help="S2 distribution shape",
+        help="S2 distribution shape in salting",
     )
 
     veto_length_run_start = straxen.URLConfig(
         default=10**9,
         type=int,
         help="Min time delay in [ns] for events towards the run start boundary",
     )
@@ -111,34 +95,39 @@
         required_names += ["s1_area", "s2_area", "s1_n_hits", "s1_tight_coincidence"]
         required_names += ["x", "y", "z", "drift_time", "s2_x", "s2_y", "z_naive"]
         dtype = copy_dtype(dtype_reference, required_names)
         # since event_number is int64 in event_basics
         dtype += [(("Salting number of events", "salt_number"), np.int64)]
         return dtype
 
+    def setup(self):
+        super(EventPositions, self).setup()
+        super(EventsSalting, self).setup()
+
+        self.init_rng()
+
     def init_rng(self):
+        """Initialize the random number generator."""
         if self.salting_seed is None:
             self.rng = np.random.default_rng(seed=int(self.run_id))
         else:
             self.rng = np.random.default_rng(seed=self.salting_seed)
 
-    def sample_time(self):
+    def sample_time(self, start, end):
         """Sample the time according to the start and end of the run."""
-        self.event_time_interval = units.s // self.salting_rate
+        self.event_time_interval = int(units.s // self.salting_rate)
 
         if units.s / self.salting_rate < self.drift_time_max * self.n_drift_time_window * 2:
             raise ValueError("Salting rate is too high according the drift time window!")
 
         time = np.arange(
-            self.run_start + self.veto_length_run_start,
-            self.run_end - self.veto_length_run_end,
+            start + self.veto_length_run_start,
+            end - self.veto_length_run_end,
             self.event_time_interval,
         ).astype(np.int64)
-        self.time_left = self.event_time_interval // 2
-        self.time_right = self.event_time_interval - self.time_left
         return time
 
     def inverse_field_distortion(self, x, y, z):
         # TODO: implement detailed inverse field distortion
         return x, y, z
 
     def set_chunk_splitting(self):
@@ -152,23 +141,17 @@
             )
         )
         self.slices = np.vstack([slices_idx[:-1], slices_idx[1:]]).T.astype(int).tolist()
 
         self.time_left = self.event_time_interval // 2
         self.time_right = self.event_time_interval - self.time_left
 
-    def setup(self):
-        """Sample the features of events."""
-        super(EventPositions, self).setup()
-        super(EventsSalting, self).setup()
-
-        self.init_rng()
-        self.init_run_meta()
-
-        time = self.sample_time()
+    def sampling(self, start, end):
+        """Sample the features of events, (t, x, y, z, S1, S2) et al."""
+        time = self.sample_time(start, end)
         self.n_events = len(time)
         self.events_salting = np.empty(self.n_events, dtype=self.dtype)
         self.events_salting["salt_number"] = np.arange(self.n_events)
         self.events_salting["time"] = time
         self.events_salting["endtime"] = time
 
         self.events_salting["s1_n_hits"] = self.s1_n_hits_tight_coincidence
@@ -193,41 +176,41 @@
         ) / self.electron_drift_velocity
 
         self.events_salting["s1_center_time"] = time - self.events_salting["drift_time"]
         self.events_salting["s2_center_time"] = time
 
         s1_area_range = (float(self.s1_area_range[0]), float(self.s1_area_range[1]))
         s2_area_range = (float(self.s2_area_range[0]), float(self.s2_area_range[1]))
-        self.events_salting["s1_area"] = np.exp(
-            self.rng.uniform(np.log(s1_area_range[0]), np.log(s1_area_range[1]), size=self.n_events)
+        self.events_salting["s1_area"] = SAMPLERS[self.s1_distribution](s1_area_range).sample(
+            self.n_events, self.rng
         )
-        self.events_salting["s1_area"] = np.clip(self.events_salting["s1_area"], *s1_area_range)
-        self.events_salting["s2_area"] = np.exp(
-            self.rng.uniform(np.log(s2_area_range[0]), np.log(s2_area_range[1]), size=self.n_events)
+        self.events_salting["s2_area"] = SAMPLERS[self.s2_distribution](s2_area_range).sample(
+            self.n_events, self.rng
         )
+        # to prevent numerical errors
+        self.events_salting["s1_area"] = np.clip(self.events_salting["s1_area"], *s1_area_range)
         self.events_salting["s2_area"] = np.clip(self.events_salting["s2_area"], *s2_area_range)
 
+        if np.any(np.diff(self.events_salting["time"]) <= 0):
+            raise ValueError("The time is not strictly increasing!")
+
         self.set_chunk_splitting()
 
-    def compute(self, chunk_i):
+    def compute(self, run_meta, start, end):
         """Copy and assign the salting events into chunk."""
-        indices = self.slices[chunk_i]
-
-        if chunk_i == 0:
-            start = self.run_start
-        else:
-            start = self.events_salting["time"][indices[0]] - self.time_left
-
-        if chunk_i == len(self.slices) - 1:
-            end = self.run_end
-        else:
-            end = self.events_salting["time"][indices[1] - 1] + self.time_right
-        return self.chunk(start=start, end=end, data=self.events_salting[indices[0] : indices[1]])
-
-    def is_ready(self, chunk_i):
-        if chunk_i < len(self.slices):
-            return True
-        else:
-            return False
+        self.sampling(start, end)
+        for chunk_i in range(len(self.slices)):
+            indices = self.slices[chunk_i]
+
+            if chunk_i == 0:
+                _start = start
+            else:
+                _start = self.events_salting["time"][indices[0]] - self.time_left
+
+            if chunk_i == len(self.slices) - 1:
+                _end = end
+            else:
+                _end = self.events_salting["time"][indices[1] - 1] + self.time_right
 
-    def source_finished(self):
-        return True
+            yield self.chunk(
+                start=_start, end=_end, data=self.events_salting[indices[0] : indices[1]]
+            )
```

### Comparing `axidence-0.2.1/axidence/plugins/salting/peak_correlation.py` & `axidence-0.2.2/axidence/plugins/salting/peak_correlation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import numba
 import numpy as np
 import strax
-from straxen import PeakProximity, PeakShadow, PeakAmbience, PeakSEDensity
+from straxen import PeakProximity, PeakShadow, PeakAmbience, PeakNearestTriggering, PeakSEDensity
 
 from ...utils import copy_dtype
 
 
 class PeakProximitySalted(PeakProximity):
     __version__ = "0.0.0"
+    child_plugin = True
     depends_on = ("peaks_salted", "peak_basics")
     provides = "peak_proximity_salted"
     data_kind = "peaks_salted"
     save_when = strax.SaveWhen.EXPLICIT
 
     def refer_dtype(self):
         return strax.unpack_dtype(strax.to_numpy_dtype(super(PeakProximitySalted, self).dtype))
@@ -56,14 +57,15 @@
             n_tot[i] = n_left[i] + np.sum(areas[dig[i] : right_i] > threshold)
 
         return n_left, n_tot
 
 
 class PeakShadowSalted(PeakShadow):
     __version__ = "0.0.0"
+    child_plugin = True
     depends_on = ("peaks_salted", "peak_basics", "peak_positions")
     provides = "peak_shadow_salted"
     data_kind = "peaks_salted"
     save_when = strax.SaveWhen.EXPLICIT
 
     def infer_dtype(self):
         dtype = super().infer_dtype()
@@ -76,14 +78,15 @@
         result = self.compute_shadow(peaks, peaks_salted)
         result["salt_number"] = peaks_salted["salt_number"]
         return result
 
 
 class PeakAmbienceSalted(PeakAmbience):
     __version__ = "0.0.0"
+    child_plugin = True
     depends_on = ("peaks_salted", "lone_hits", "peak_basics", "peak_positions")
     provides = "peak_ambience_salted"
     data_kind = "peaks_salted"
     save_when = strax.SaveWhen.EXPLICIT
 
     def infer_dtype(self):
         dtype = super().infer_dtype()
@@ -94,16 +97,38 @@
 
     def compute(self, peaks_salted, lone_hits, peaks):
         result = self.compute_ambience(lone_hits, peaks, peaks_salted)
         result["salt_number"] = peaks_salted["salt_number"]
         return result
 
 
+class PeakNearestTriggeringSalted(PeakNearestTriggering):
+    __version__ = "0.0.0"
+    child_plugin = True
+    depends_on = ("peaks_salted", "peak_proximity_salted", "peak_basics", "peak_proximity")
+    provides = "peak_nearest_triggering_salted"
+    data_kind = "peaks_salted"
+    save_when = strax.SaveWhen.EXPLICIT
+
+    def infer_dtype(self):
+        dtype = super().infer_dtype()
+        dtype += [
+            (("Salting number of peaks", "salt_number"), np.int64),
+        ]
+        return dtype
+
+    def compute(self, peaks_salted, peaks):
+        result = self.compute_triggering(peaks, peaks_salted)
+        result["salt_number"] = peaks_salted["salt_number"]
+        return result
+
+
 class PeakSEDensitySalted(PeakSEDensity):
     __version__ = "0.0.0"
+    child_plugin = True
     depends_on = ("peaks_salted", "peak_basics", "peak_positions")
     provides = "peak_se_density_salted"
     data_kind = "peaks_salted"
     save_when = strax.SaveWhen.EXPLICIT
 
     def infer_dtype(self):
         dtype = super().infer_dtype()
```

### Comparing `axidence-0.2.1/axidence/plugins/salting/peaks_salted.py` & `axidence-0.2.2/axidence/plugins/salting/peaks_salted.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from straxen import PeakBasics
 
 from ...utils import copy_dtype
 
 
 class PeaksSalted(PeakBasics):
     __version__ = "0.0.0"
+    child_plugin = True
     depends_on = "events_salting"
     provides = "peaks_salted"
     data_kind = "peaks_salted"
     save_when = strax.SaveWhen.EXPLICIT
 
     only_salt_s1 = straxen.URLConfig(
         default=False,
@@ -37,14 +38,19 @@
         dtype += [
             (("Reconstructed S2 X position (cm), uncorrected", "x"), np.float32),
             (("Reconstructed S2 Y position (cm), uncorrected", "y"), np.float32),
             (("Salting number of peaks", "salt_number"), np.int64),
         ]
         return dtype
 
+    def setup(self):
+        super().setup()
+        if self.only_salt_s1 and self.only_salt_s2:
+            raise ValueError("Cannot only salt both S1 and S2.")
+
     def compute(self, events_salting):
         """Copy features of events_salting into peaks_salted."""
         peaks_salted = np.empty(len(events_salting) * 2, dtype=self.dtype)
         for n in "center_time area".split():
             peaks_salted[n] = np.vstack(
                 [
                     events_salting[f"s1_{n}"],
@@ -71,8 +77,14 @@
         peaks_salted["type"] = np.vstack(
             [
                 np.full(len(events_salting), 1),
                 np.full(len(events_salting), 2),
             ]
         ).T.flatten()
         peaks_salted["salt_number"] = np.repeat(events_salting["salt_number"], 2)
+
+        # Filter out peaks that are not S1 or S2
+        if self.only_salt_s1:
+            peaks_salted = peaks_salted[peaks_salted["type"] == 1]
+        if self.only_salt_s2:
+            peaks_salted = peaks_salted[peaks_salted["type"] == 2]
         return peaks_salted
```

### Comparing `axidence-0.2.1/axidence/utils.py` & `axidence-0.2.2/axidence/utils.py`

 * *Files identical despite different names*

### Comparing `axidence-0.2.1/pyproject.toml` & `axidence-0.2.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "axidence"
-version = "0.2.1"
+version = "0.2.2"
 description = "strax-based data-driven accidental coincidence background simulation and peak-level salting"
 readme = "README.md"
 license = "BSD-3-Clause"
 authors = [
   "Dacheng Xu, <dx2227@columbia.edu>",
 ]
 requires-python = ">=3.9"
@@ -20,11 +20,12 @@
 ]
 repository = "https://github.com/dachengx/axidence"
 documentation = "https://readthedocs.org/projects/axidence/"
 
 [tool.poetry.dependencies]
 strax = ">=1.6.2"
 straxen = ">=2.2.1"
+GOFevaluation = ">=0.1.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.8", "setuptools>=61.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `axidence-0.2.1/PKG-INFO` & `axidence-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: axidence
-Version: 0.2.1
+Version: 0.2.2
 Summary: strax-based data-driven accidental coincidence background simulation and peak-level salting
 Home-page: https://github.com/dachengx/axidence
 License: BSD-3-Clause
 Author: Dacheng Xu,
 Author-email: dx2227@columbia.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Physics
+Requires-Dist: GOFevaluation (>=0.1.4)
 Requires-Dist: strax (>=1.6.2)
 Requires-Dist: straxen (>=2.2.1)
 Project-URL: Documentation, https://readthedocs.org/projects/axidence/
 Project-URL: Repository, https://github.com/dachengx/axidence
 Description-Content-Type: text/markdown
 
 # Axidence
```

