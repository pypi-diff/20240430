# Comparing `tmp/fsrs-1.2.0.tar.gz` & `tmp/fsrs-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs-1.2.0.tar", last modified: Wed Dec 27 16:40:06 2023, max compression
+gzip compressed data, was "fsrs-2.0.0.tar", last modified: Tue Apr 30 02:42:52 2024, max compression
```

## Comparing `fsrs-1.2.0.tar` & `fsrs-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 16:40:06.640496 fsrs-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2023-12-27 16:39:58.000000 fsrs-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2023-12-27 16:40:06.640496 fsrs-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2023-12-27 16:39:58.000000 fsrs-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      593 2023-12-27 16:39:58.000000 fsrs-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-27 16:40:06.640496 fsrs-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-27 16:39:58.000000 fsrs-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 16:40:06.636496 fsrs-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 16:40:06.640496 fsrs-1.2.0/src/fsrs/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-12-27 16:39:58.000000 fsrs-1.2.0/src/fsrs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2023-12-27 16:39:58.000000 fsrs-1.2.0/src/fsrs/fsrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2023-12-27 16:39:58.000000 fsrs-1.2.0/src/fsrs/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 16:40:06.640496 fsrs-1.2.0/src/fsrs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2023-12-27 16:40:06.000000 fsrs-1.2.0/src/fsrs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      245 2023-12-27 16:40:06.000000 fsrs-1.2.0/src/fsrs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 16:40:06.000000 fsrs-1.2.0/src/fsrs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-12-27 16:40:06.000000 fsrs-1.2.0/src/fsrs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 16:40:06.640496 fsrs-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2023-12-27 16:39:58.000000 fsrs-1.2.0/tests/test_fsrs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:52.385321 fsrs-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-30 02:42:45.000000 fsrs-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-04-30 02:42:52.385321 fsrs-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-30 02:42:45.000000 fsrs-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-30 02:42:45.000000 fsrs-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 02:42:52.385321 fsrs-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 02:42:45.000000 fsrs-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:52.385321 fsrs-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:52.385321 fsrs-2.0.0/src/fsrs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-30 02:42:45.000000 fsrs-2.0.0/src/fsrs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-04-30 02:42:45.000000 fsrs-2.0.0/src/fsrs/fsrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-04-30 02:42:45.000000 fsrs-2.0.0/src/fsrs/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:52.385321 fsrs-2.0.0/src/fsrs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-04-30 02:42:52.000000 fsrs-2.0.0/src/fsrs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-30 02:42:52.000000 fsrs-2.0.0/src/fsrs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 02:42:52.000000 fsrs-2.0.0/src/fsrs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-30 02:42:52.000000 fsrs-2.0.0/src/fsrs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:52.385321 fsrs-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-30 02:42:45.000000 fsrs-2.0.0/tests/test_fsrs.py
```

### Comparing `fsrs-1.2.0/LICENSE` & `fsrs-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fsrs-1.2.0/PKG-INFO` & `fsrs-2.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsrs
-Version: 1.2.0
+Version: 2.0.0
 Summary: Free Spaced Repetition Scheduler
 Author-email: Jarrett Ye <jarrett.ye@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Open Spaced Repetition
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,30 +31,34 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## About The Project
 
+[![PyPi](https://img.shields.io/pypi/v/fsrs)](https://pypi.org/project/fsrs/) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
 Py-fsrs is a Python Package implements [Free Spaced Repetition Scheduler algorithm](https://github.com/open-spaced-repetition/free-spaced-repetition-scheduler). It helps developers apply FSRS in their flashcard apps.
 
 ## Getting Started
 
 ```
 pip install fsrs
 ```
 
 ## Usage
 
 Create a card and review it at a given time:
 ```python
+from datetime import datetime, UTC
 from fsrs import *
 f = FSRS()
 card = Card()
-now = datetime(2022, 11, 29, 12, 30, 0, 0)
+# (py-fsrs cards use UTC)
+now = datetime(2022, 11, 29, 12, 30, 0, 0, tzinfo=UTC) 
 scheduling_cards = f.repeat(card, now)
 ```
 
 There are four ratings:
 ```python
 Rating.Again # forget; incorrect response
 Rating.Hard # recall; correct response recalled with serious difficulty
```

### Comparing `fsrs-1.2.0/README.md` & `fsrs-2.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 ## About The Project
 
+[![PyPi](https://img.shields.io/pypi/v/fsrs)](https://pypi.org/project/fsrs/) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
 Py-fsrs is a Python Package implements [Free Spaced Repetition Scheduler algorithm](https://github.com/open-spaced-repetition/free-spaced-repetition-scheduler). It helps developers apply FSRS in their flashcard apps.
 
 ## Getting Started
 
 ```
 pip install fsrs
 ```
 
 ## Usage
 
 Create a card and review it at a given time:
 ```python
+from datetime import datetime, UTC
 from fsrs import *
 f = FSRS()
 card = Card()
-now = datetime(2022, 11, 29, 12, 30, 0, 0)
+# (py-fsrs cards use UTC)
+now = datetime(2022, 11, 29, 12, 30, 0, 0, tzinfo=UTC) 
 scheduling_cards = f.repeat(card, now)
 ```
 
 There are four ratings:
 ```python
 Rating.Again # forget; incorrect response
 Rating.Hard # recall; correct response recalled with serious difficulty
```

### Comparing `fsrs-1.2.0/pyproject.toml` & `fsrs-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fsrs"
-version = "1.2.0"
+version = "2.0.0"
 description = "Free Spaced Repetition Scheduler"
 readme = "README.md"
 authors = [{ name = "Jarrett Ye", email = "jarrett.ye@outlook.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

### Comparing `fsrs-1.2.0/src/fsrs/fsrs.py` & `fsrs-2.0.0/src/fsrs/fsrs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 from .models import *
 import math
+from datetime import timezone
 
 
 class FSRS:
     p: Parameters
     DECAY: float
     FACTOR: float
 
     def __init__(self) -> None:
         self.p = Parameters()
         self.DECAY = -0.5
         self.FACTOR = 0.9 ** (1 / self.DECAY) - 1
 
     def repeat(self, card: Card, now: datetime) -> dict[int, SchedulingInfo]:
+
+        if (now.tzinfo is None) or (now.tzinfo != timezone.utc):
+            raise ValueError("datetime must be timezone-aware and set to UTC")
+
         card = copy.deepcopy(card)
         if card.state == State.New:
             card.elapsed_days = 0
         else:
             card.elapsed_days = (now - card.last_review).days
         card.last_review = now
         card.reps += 1
@@ -59,52 +64,67 @@
         s.hard.difficulty = self.init_difficulty(Rating.Hard)
         s.hard.stability = self.init_stability(Rating.Hard)
         s.good.difficulty = self.init_difficulty(Rating.Good)
         s.good.stability = self.init_stability(Rating.Good)
         s.easy.difficulty = self.init_difficulty(Rating.Easy)
         s.easy.stability = self.init_stability(Rating.Easy)
 
-    def next_ds(self, s: SchedulingCards, last_d: float, last_s: float, retrievability: float):
+    def next_ds(
+        self, s: SchedulingCards, last_d: float, last_s: float, retrievability: float
+    ):
         s.again.difficulty = self.next_difficulty(last_d, Rating.Again)
         s.again.stability = self.next_forget_stability(last_d, last_s, retrievability)
         s.hard.difficulty = self.next_difficulty(last_d, Rating.Hard)
-        s.hard.stability = self.next_recall_stability(last_d, last_s, retrievability, Rating.Hard)
+        s.hard.stability = self.next_recall_stability(
+            last_d, last_s, retrievability, Rating.Hard
+        )
         s.good.difficulty = self.next_difficulty(last_d, Rating.Good)
-        s.good.stability = self.next_recall_stability(last_d, last_s, retrievability, Rating.Good)
+        s.good.stability = self.next_recall_stability(
+            last_d, last_s, retrievability, Rating.Good
+        )
         s.easy.difficulty = self.next_difficulty(last_d, Rating.Easy)
-        s.easy.stability = self.next_recall_stability(last_d, last_s, retrievability, Rating.Easy)
+        s.easy.stability = self.next_recall_stability(
+            last_d, last_s, retrievability, Rating.Easy
+        )
 
     def init_stability(self, r: int) -> float:
-        return max(self.p.w[r-1], 0.1)
+        return max(self.p.w[r - 1], 0.1)
 
     def init_difficulty(self, r: int) -> float:
         return min(max(self.p.w[4] - self.p.w[5] * (r - 3), 1), 10)
 
     def forgetting_curve(self, elapsed_days: int, stability: float) -> float:
         return (1 + self.FACTOR * elapsed_days / stability) ** self.DECAY
 
     def next_interval(self, s: float) -> int:
-        new_interval = s / self.FACTOR * (self.p.request_retention ** (1 / self.DECAY) - 1)
+        new_interval = (
+            s / self.FACTOR * (self.p.request_retention ** (1 / self.DECAY) - 1)
+        )
         return min(max(round(new_interval), 1), self.p.maximum_interval)
 
     def next_difficulty(self, d: float, r: int) -> float:
         next_d = d - self.p.w[6] * (r - 3)
         return min(max(self.mean_reversion(self.p.w[4], next_d), 1), 10)
 
     def mean_reversion(self, init: float, current: float) -> float:
         return self.p.w[7] * init + (1 - self.p.w[7]) * current
 
     def next_recall_stability(self, d: float, s: float, r: float, rating: int) -> float:
         hard_penalty = self.p.w[15] if rating == Rating.Hard else 1
         easy_bonus = self.p.w[16] if rating == Rating.Easy else 1
-        return s * (1 + math.exp(self.p.w[8]) *
-                    (11 - d) *
-                    math.pow(s, -self.p.w[9]) *
-                    (math.exp((1 - r) * self.p.w[10]) - 1) *
-                    hard_penalty *
-                    easy_bonus)
+        return s * (
+            1
+            + math.exp(self.p.w[8])
+            * (11 - d)
+            * math.pow(s, -self.p.w[9])
+            * (math.exp((1 - r) * self.p.w[10]) - 1)
+            * hard_penalty
+            * easy_bonus
+        )
 
     def next_forget_stability(self, d: float, s: float, r: float) -> float:
-        return self.p.w[11] * \
-            math.pow(d, -self.p.w[12]) * \
-            (math.pow(s + 1, self.p.w[13]) - 1) * \
-            math.exp((1 - r) * self.p.w[14])
+        return (
+            self.p.w[11]
+            * math.pow(d, -self.p.w[12])
+            * (math.pow(s + 1, self.p.w[13]) - 1)
+            * math.exp((1 - r) * self.p.w[14])
+        )
```

### Comparing `fsrs-1.2.0/src/fsrs/models.py` & `fsrs-2.0.0/src/fsrs/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, UTC
 import copy
 from typing import Tuple, Optional
 from enum import IntEnum
 
 
 class State(IntEnum):
     New = 0
@@ -18,18 +18,25 @@
     Easy = 4
 
 
 class ReviewLog:
     rating: int
     scheduled_days: int
     elapsed_days: int
-    Review: datetime
+    review: datetime
     state: int
 
-    def __init__(self, rating: int, scheduled_days: int, elapsed_days: int, review: datetime, state: int):
+    def __init__(
+        self,
+        rating: int,
+        scheduled_days: int,
+        elapsed_days: int,
+        review: datetime,
+        state: int,
+    ):
         self.rating = rating
         self.scheduled_days = scheduled_days
         self.elapsed_days = elapsed_days
         self.review = review
         self.state = state
 
 
@@ -41,24 +48,23 @@
     scheduled_days: int
     reps: int
     lapses: int
     state: State
     last_review: datetime
 
     def __init__(self) -> None:
-        self.due = datetime.utcnow()
+        self.due = datetime.now(UTC)
         self.stability = 0
         self.difficulty = 0
         self.elapsed_days = 0
         self.scheduled_days = 0
         self.reps = 0
         self.lapses = 0
         self.state = State.New
 
-    
     def get_retrievability(self, now: datetime) -> Optional[float]:
         DECAY = -0.5
         FACTOR = 0.9 ** (1 / DECAY) - 1
 
         if self.state == State.Review:
             elapsed_days = max(0, (now - self.last_review).days)
             return (1 + FACTOR * elapsed_days / self.stability) ** DECAY
@@ -101,46 +107,98 @@
         elif state == State.Review:
             self.again.state = State.Relearning
             self.hard.state = State.Review
             self.good.state = State.Review
             self.easy.state = State.Review
             self.again.lapses += 1
 
-    def schedule(self, now: datetime, hard_interval: float, good_interval: float, easy_interval: float):
+    def schedule(
+        self,
+        now: datetime,
+        hard_interval: float,
+        good_interval: float,
+        easy_interval: float,
+    ):
         self.again.scheduled_days = 0
         self.hard.scheduled_days = hard_interval
         self.good.scheduled_days = good_interval
         self.easy.scheduled_days = easy_interval
         self.again.due = now + timedelta(minutes=5)
         if hard_interval > 0:
             self.hard.due = now + timedelta(days=hard_interval)
         else:
             self.hard.due = now + timedelta(minutes=10)
         self.good.due = now + timedelta(days=good_interval)
         self.easy.due = now + timedelta(days=easy_interval)
 
     def record_log(self, card: Card, now: datetime) -> dict[int, SchedulingInfo]:
         return {
-            Rating.Again: SchedulingInfo(self.again,
-                                         ReviewLog(Rating.Again, self.again.scheduled_days, card.elapsed_days, now,
-                                                   card.state)),
-            Rating.Hard: SchedulingInfo(self.hard,
-                                        ReviewLog(Rating.Hard, self.hard.scheduled_days, card.elapsed_days, now,
-                                                  card.state)),
-            Rating.Good: SchedulingInfo(self.good,
-                                        ReviewLog(Rating.Good, self.good.scheduled_days, card.elapsed_days, now,
-                                                  card.state)),
-            Rating.Easy: SchedulingInfo(self.easy,
-                                        ReviewLog(Rating.Easy, self.easy.scheduled_days, card.elapsed_days, now,
-                                                  card.state)),
+            Rating.Again: SchedulingInfo(
+                self.again,
+                ReviewLog(
+                    Rating.Again,
+                    self.again.scheduled_days,
+                    card.elapsed_days,
+                    now,
+                    card.state,
+                ),
+            ),
+            Rating.Hard: SchedulingInfo(
+                self.hard,
+                ReviewLog(
+                    Rating.Hard,
+                    self.hard.scheduled_days,
+                    card.elapsed_days,
+                    now,
+                    card.state,
+                ),
+            ),
+            Rating.Good: SchedulingInfo(
+                self.good,
+                ReviewLog(
+                    Rating.Good,
+                    self.good.scheduled_days,
+                    card.elapsed_days,
+                    now,
+                    card.state,
+                ),
+            ),
+            Rating.Easy: SchedulingInfo(
+                self.easy,
+                ReviewLog(
+                    Rating.Easy,
+                    self.easy.scheduled_days,
+                    card.elapsed_days,
+                    now,
+                    card.state,
+                ),
+            ),
         }
 
 
 class Parameters:
     request_retention: float
     maximum_interval: int
     w: Tuple[float, ...]
 
     def __init__(self) -> None:
         self.request_retention = 0.9
         self.maximum_interval = 36500
-        self.w = (0.4, 0.6, 2.4, 5.8, 4.93, 0.94, 0.86, 0.01, 1.49, 0.14, 0.94, 2.18, 0.05, 0.34, 1.26, 0.29, 2.61)
+        self.w = (
+            0.4,
+            0.6,
+            2.4,
+            5.8,
+            4.93,
+            0.94,
+            0.86,
+            0.01,
+            1.49,
+            0.14,
+            0.94,
+            2.18,
+            0.05,
+            0.34,
+            1.26,
+            0.29,
+            2.61,
+        )
```

### Comparing `fsrs-1.2.0/src/fsrs.egg-info/PKG-INFO` & `fsrs-2.0.0/src/fsrs.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsrs
-Version: 1.2.0
+Version: 2.0.0
 Summary: Free Spaced Repetition Scheduler
 Author-email: Jarrett Ye <jarrett.ye@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Open Spaced Repetition
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,30 +31,34 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## About The Project
 
+[![PyPi](https://img.shields.io/pypi/v/fsrs)](https://pypi.org/project/fsrs/) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
 Py-fsrs is a Python Package implements [Free Spaced Repetition Scheduler algorithm](https://github.com/open-spaced-repetition/free-spaced-repetition-scheduler). It helps developers apply FSRS in their flashcard apps.
 
 ## Getting Started
 
 ```
 pip install fsrs
 ```
 
 ## Usage
 
 Create a card and review it at a given time:
 ```python
+from datetime import datetime, UTC
 from fsrs import *
 f = FSRS()
 card = Card()
-now = datetime(2022, 11, 29, 12, 30, 0, 0)
+# (py-fsrs cards use UTC)
+now = datetime(2022, 11, 29, 12, 30, 0, 0, tzinfo=UTC) 
 scheduling_cards = f.repeat(card, now)
 ```
 
 There are four ratings:
 ```python
 Rating.Again # forget; incorrect response
 Rating.Hard # recall; correct response recalled with serious difficulty
```

