# Comparing `tmp/zhinst_timing_models-24.1.54288-py3-none-any.whl.zip` & `tmp/zhinst_timing_models-24.4.57831-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5851 bytes, number of entries: 8
--rw-r--r--  2.0 unx      544 b- defN 20-Feb-02 00:00 zhinst/timing_models/__init__.py
+Zip file size: 6424 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      584 b- defN 20-Feb-02 00:00 zhinst/timing_models/__init__.py
 -rw-r--r--  2.0 unx      421 b- defN 20-Feb-02 00:00 zhinst/timing_models/_version.py
--rw-r--r--  2.0 unx     7858 b- defN 20-Feb-02 00:00 zhinst/timing_models/feedback_model.py
+-rw-r--r--  2.0 unx     9930 b- defN 20-Feb-02 00:00 zhinst/timing_models/feedback_model.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 zhinst/timing_models/py.typed
-?rw-r--r--  2.0 unx     1798 b- defN 20-Feb-02 00:00 zhinst_timing_models-24.1.54288.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 zhinst_timing_models-24.1.54288.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1101 b- defN 20-Feb-02 00:00 zhinst_timing_models-24.1.54288.dist-info/licenses/LICENSE.txt
-?rw-r--r--  2.0 unx      733 b- defN 20-Feb-02 00:00 zhinst_timing_models-24.1.54288.dist-info/RECORD
-8 files, 12542 bytes uncompressed, 4545 bytes compressed:  63.8%
+?rw-r--r--  2.0 unx     1941 b- defN 20-Feb-02 00:00 zhinst_timing_models-24.4.57831.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 zhinst_timing_models-24.4.57831.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1101 b- defN 20-Feb-02 00:00 zhinst_timing_models-24.4.57831.dist-info/licenses/LICENSE.txt
+?rw-r--r--  2.0 unx      733 b- defN 20-Feb-02 00:00 zhinst_timing_models-24.4.57831.dist-info/RECORD
+8 files, 14797 bytes uncompressed, 5118 bytes compressed:  65.4%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: zhinst/timing_models/feedback_model.py
 Comment: 
 
 Filename: zhinst/timing_models/py.typed
 Comment: 
 
-Filename: zhinst_timing_models-24.1.54288.dist-info/METADATA
+Filename: zhinst_timing_models-24.4.57831.dist-info/METADATA
 Comment: 
 
-Filename: zhinst_timing_models-24.1.54288.dist-info/WHEEL
+Filename: zhinst_timing_models-24.4.57831.dist-info/WHEEL
 Comment: 
 
-Filename: zhinst_timing_models-24.1.54288.dist-info/licenses/LICENSE.txt
+Filename: zhinst_timing_models-24.4.57831.dist-info/licenses/LICENSE.txt
 Comment: 
 
-Filename: zhinst_timing_models-24.1.54288.dist-info/RECORD
+Filename: zhinst_timing_models-24.4.57831.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zhinst/timing_models/__init__.py

```diff
@@ -5,19 +5,21 @@
 from zhinst.timing_models.feedback_model import (
     FeedbackPath,
     PQSCMode,
     QAType,
     QCCSFeedbackModel,
     QCCSSystemDescription,
     SGType,
+    TriggerSource,
     get_feedback_system_description,
 )
 
 __all__ = [
-    "QCCSFeedbackModel",
-    "get_feedback_system_description",
-    "SGType",
-    "QAType",
-    "PQSCMode",
     "FeedbackPath",
+    "PQSCMode",
+    "QAType",
+    "QCCSFeedbackModel",
     "QCCSSystemDescription",
+    "SGType",
+    "TriggerSource",
+    "get_feedback_system_description",
 ]
```

## zhinst/timing_models/_version.py

```diff
@@ -8,9 +8,9 @@
     VERSION_TUPLE = object
 
 version: str
 __version__: str
 __version_tuple__: VERSION_TUPLE
 version_tuple: VERSION_TUPLE
 
-__version__ = version = '24.1.54288'
-__version_tuple__ = version_tuple = (24, 1, 54288)
+__version__ = version = '24.4.57831'
+__version_tuple__ = version_tuple = (24, 4, 57831)
```

## zhinst/timing_models/feedback_model.py

```diff
@@ -2,22 +2,24 @@
 
 Typical usage example:
 ```python
 model = QCCSFeedbackModel(
     description=get_feedback_system_description(
         generator_type=SGType.HDAWG,
         analyzer_type=QAType.SHFQA,
+        trigger_source=TriggerSource.ZSYNC,
         pqsc_mode=PQSCMode.DECODER
     )
 )
 ```
 """
 
 from __future__ import annotations
 
+import warnings
 from dataclasses import dataclass
 from enum import IntEnum
 
 import numpy as np
 
 
 class SGType(IntEnum):
@@ -38,24 +40,38 @@
 class PQSCMode(IntEnum):
     """Different handling of feedback data from the PQSC."""
 
     REGISTER_FORWARD = 1
     DECODER = 2
 
 
+class TriggerSource(IntEnum):
+    """Different trigger sources for the QA and SG channels."""
+
+    ZSYNC = 1
+    INTERNAL = 2
+
+
 class FeedbackPath(IntEnum):
     """Different handling of feedback data from the PQSC.
 
     .. versionadded:: 0.3
     """
 
     ZSYNC = 1
     INTERNAL = 3
 
 
+MINIMUM_SAMPLES_INTEGRATION_LENGTH = 4
+MINIMUM_SAMPLES_INTEGRATION_DELAY = 16
+MINIMUM_SAMPLES_UNTIL_READOUT_COMPLETE = (
+    MINIMUM_SAMPLES_INTEGRATION_LENGTH + MINIMUM_SAMPLES_INTEGRATION_DELAY
+)
+
+
 @dataclass
 class QCCSSystemDescription:
     """Describe the behavior of a QCCS system with respect to feedback latency."""
 
     initial_latency_cycles: int
     """[clock cycles] Minimum latency for the smallest amount of
     integration length."""
@@ -74,22 +90,24 @@
     latency, to match the latency seen by the sequencer"""
 
 
 def get_feedback_system_description(  # noqa: C901, PLR0912
     generator_type: SGType,
     analyzer_type: QAType,
     pqsc_mode: PQSCMode | None = None,
+    trigger_source: TriggerSource = TriggerSource.ZSYNC,
     feedback_path: FeedbackPath = FeedbackPath.ZSYNC,
 ) -> QCCSSystemDescription:
     """Returns a QCCSSysDescription object for a given configuration.
 
     Args:
       generator_type: Signal generator used (SHFSG/HDAWG).
       analyzer_type: Quantum analyzer used.
       pqsc_mode: Mode of operation for the PQSC.
+      trigger_source: Select between ZSync via PQSC or internal trigger for the SHFQC.
       feedback_path: Used only when the generator type is SHFQC to select
                      between local feedback or through PQSC
 
     Returns:
       A QCCS system description object to be used in a `QCCSFeedbackModel` object.
 
     Raises:
@@ -100,80 +118,97 @@
 
         Added `feedback_path` argument.
     """
     if analyzer_type not in [QAType.SHFQA, QAType.SHFQC]:
         msg = f"Unknown quantum analyzer type ({analyzer_type})"
         raise ValueError(msg)
 
-    if (
-        pqsc_mode in [PQSCMode.DECODER, PQSCMode.REGISTER_FORWARD]
-        and feedback_path is FeedbackPath.INTERNAL
+    if pqsc_mode in [PQSCMode.DECODER, PQSCMode.REGISTER_FORWARD] and (
+        feedback_path is FeedbackPath.INTERNAL
+        or trigger_source is TriggerSource.INTERNAL
     ):
-        msg = str(
-            f"PQSC mode ({pqsc_mode}) incompatible with"
-            f"selected feedback path ({feedback_path})",
+        msg = (
+            f"PQSC mode ({pqsc_mode.name}) incompatible with "
+            f"selected feedback path ({feedback_path.name}) "
+            f"and/or trigger source ({trigger_source.name})"
         )
         raise ValueError(msg)
 
     if generator_type is SGType.HDAWG:
         if feedback_path == FeedbackPath.INTERNAL:
             msg = "Internal Feedback can only be used with generator=SGType.SHFQC"
             raise ValueError(msg)
+        if trigger_source == TriggerSource.INTERNAL:
+            msg = "Internal trigger can only be used with generator=SGType.SHFQC"
+            raise ValueError(msg)
         if pqsc_mode is PQSCMode.REGISTER_FORWARD:
             return QCCSSystemDescription(
-                initial_latency_cycles=96,
-                initial_steps=4,
-                pattern=[(4, 9), (4, 8), (5, 8), (4, 9), (4, 8), (4, 8)],
+                initial_latency_cycles=100,
+                initial_steps=7,
+                pattern=[(4, 8), (5, 8), (4, 9), (4, 8), (4, 8), (4, 9)],
                 rtlogger_correction=2,
             )
         if pqsc_mode is PQSCMode.DECODER:
             return QCCSSystemDescription(
-                initial_latency_cycles=100,
-                initial_steps=6,
-                pattern=[(4, 8), (5, 9), (4, 8), (4, 8), (4, 9), (4, 8)],
+                initial_latency_cycles=104,
+                initial_steps=8,
+                pattern=[(5, 9), (4, 8), (4, 8), (4, 9), (4, 8), (4, 8)],
                 rtlogger_correction=2,
             )
         msg = f"Unknown PQSC mode ({pqsc_mode})"
         raise ValueError(msg)
 
     if generator_type in [SGType.SHFSG, SGType.SHFQC]:
         if feedback_path is FeedbackPath.INTERNAL:
             if generator_type != SGType.SHFQC:
                 msg = "Internal Feedback can only be used with generator=SGType.SHFQC"
                 raise ValueError(msg)
             if analyzer_type != QAType.SHFQC:
                 msg = "Internal Feedback can only be used with analyzer=QAType.SHFQC"
                 raise ValueError(msg)
             if pqsc_mode is not None:
-                msg = str(
-                    "Internal Feedback can't be used with "
-                    f"the selected pqsc mode ({pqsc_mode})",
+                msg = (
+                    f"Internal Feedback can't be used with "
+                    f"the selected pqsc mode ({pqsc_mode})"
                 )
+
                 raise ValueError(msg)
+            if (
+                trigger_source is TriggerSource.ZSYNC
+            ):  # internal feedback with ZSync trigger
+                return QCCSSystemDescription(
+                    initial_latency_cycles=30,
+                    initial_steps=1,
+                    pattern=[(1, 2)] * 25,
+                    rtlogger_correction=2,
+                )
+
+            # internal feedback with internal trigger
             return QCCSSystemDescription(
-                initial_latency_cycles=25,
-                initial_steps=2,
+                initial_latency_cycles=27,
+                initial_steps=1,
                 pattern=[(1, 2)] * 25,
             )
+
         if pqsc_mode is PQSCMode.REGISTER_FORWARD:
             return QCCSSystemDescription(
-                initial_latency_cycles=92,
-                initial_steps=4,
-                pattern=[(3, 9), (5, 8), (5, 8), (2, 9), (5, 8), (5, 8)],
+                initial_latency_cycles=95,
+                initial_steps=7,
+                pattern=[(5, 8), (5, 8), (3, 9), (5, 8), (5, 8), (2, 9)],
                 rtlogger_correction=2,
             )
         if pqsc_mode is PQSCMode.DECODER:
             return QCCSSystemDescription(
-                initial_latency_cycles=95,
-                initial_steps=6,
-                pattern=[(5, 8), (5, 9), (2, 8), (5, 8), (5, 9), (3, 8)],
+                initial_latency_cycles=100,
+                initial_steps=8,
+                pattern=[(5, 9), (3, 8), (5, 8), (5, 9), (2, 8), (5, 8)],
                 rtlogger_correction=2,
             )
         msg = f"Unknown PQSC mode ({pqsc_mode})"
-        raise ValueError
+        raise ValueError(msg)
 
     msg = f"Unknown signal generator type ({generator_type})"
     raise ValueError(msg)
 
 
 @dataclass
 class QCCSFeedbackModel:
@@ -186,23 +221,43 @@
     Args:
       description: The QCCS system configuration description as returned
                    from get_feedback_system_description()
     """
 
     description: QCCSSystemDescription
 
-    def get_latency(self, length: int) -> int:
+    def get_latency(
+        self,
+        samples: int = 20,
+        length: int | None = None,
+    ) -> int:
         """Provide the expected latency relative to the integration length.
 
         Args:
-          length: Integration length in samples
+            samples:
+              The number of samples from the trigger to the completion of the
+              integration. This includes the samples up to the `startQA()`
+              command, plus the integration length and delay.
+            length: Deprecated
 
         Returns:
           The expected latency in AWG clock cycles
         """
+        if samples is None:
+            samples = length
+            if length is not None:
+                msg = (
+                    "'length' is a deprecated argument.",
+                    " User 'samples_until_integration_complete' instead",
+                )
+                warnings.warn(msg, category=DeprecationWarning, stacklevel=1)
+        if samples < MINIMUM_SAMPLES_UNTIL_READOUT_COMPLETE:
+            msg = "samples_until_integration_complete must be at least 20"
+            raise ValueError(msg)
+
         # before the periodic pattern
         model = np.array(
             [self.description.initial_latency_cycles] * self.description.initial_steps,
             dtype=np.int64,
         )
 
         # build the periodic pattern
@@ -213,15 +268,15 @@
             periodic_mdl = np.concatenate(
                 (periodic_mdl, np.array([acc] * int_steps, dtype=np.int64)),
                 dtype=np.int64,
             )
 
         # from integration samples to generator cc
         def f_calculate_cycles() -> int:
-            index = length // 4
+            index = (samples - MINIMUM_SAMPLES_INTEGRATION_DELAY) // 4
             if index <= self.description.initial_steps:
                 return int(model[index - 1])
 
             index -= self.description.initial_steps + 1
             lat_full_periods = (
                 index // self.description.period_steps
             ) * self.description.latency_in_period_cycles  # latency from full periods
```

## Comparing `zhinst_timing_models-24.1.54288.dist-info/METADATA` & `zhinst_timing_models-24.4.57831.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: zhinst-timing-models
-Version: 24.1.54288
+Version: 24.4.57831
 Summary: Feedback Data Latency model for PQSC, SHF- and HDAWG systems.
 Author-email: Zurich Instruments <info@zhinst.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Keywords: zhinst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -25,17 +25,18 @@
 
 -----
 
 Feedback Data Latency model for PQSC, SHF- and HDAWG systems.
 
 **Table of Contents**
 
-- [Installation](#installation)
-- [Usage](#usage)
-- [License](#license)
+- [Feedback Latency Model Parameters](#feedback-latency-model-parameters)
+  - [Installation](#installation)
+  - [Usage](#usage)
+  - [License](#license)
 
 ## Installation
 
 ```console
 pip install zhinst-timing-models
 ```
 
@@ -43,22 +44,24 @@
 
 ```python
 from zhinst.timing_models import (
     PQSCMode,
     QAType,
     QCCSFeedbackModel,
     SGType,
+    TriggerSource,
     get_feedback_system_description,
 )
 
 model = QCCSFeedbackModel(
     description=get_feedback_system_description(
         generator_type=SGType.HDAWG,
         analyzer_type=QAType.SHFQA,
         pqsc_mode=PQSCMode.DECODER,
+        trigger_source=TriggerSource.ZSYNC,
         )
     )
 awg_clock_cycles = model.get_latency(...)
 ```
 
 ## License
```

## Comparing `zhinst_timing_models-24.1.54288.dist-info/licenses/LICENSE.txt` & `zhinst_timing_models-24.4.57831.dist-info/licenses/LICENSE.txt`

 * *Files identical despite different names*

