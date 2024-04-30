# Comparing `tmp/arbmaster-0.1.0.tar.gz` & `tmp/arbmaster-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\239294\OneDrive - V\344ster\345s Stad\Skrivbordet\arbmaster\dist\.tmp-0qbgaa5j\arbmaster-0.1.0.tar", last modified: Tue Apr 30 16:59:03 2024, max compression
+gzip compressed data, was "C:\Users\239294\OneDrive - V\344ster\345s Stad\Skrivbordet\project\dist\.tmp-uefw6v4q\arbmaster-0.1.1.tar", last modified: Tue Apr 30 19:47:47 2024, max compression
```

## Comparing `arbmaster-0.1.0.tar` & `arbmaster-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 16:59:03.141747 arbmaster-0.1.0/
--rw-rw-rw-   0        0        0     1086 2024-04-27 12:49:42.000000 arbmaster-0.1.0/LICENCE
--rw-rw-rw-   0        0        0     1912 2024-04-30 16:59:03.134838 arbmaster-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1342 2024-04-30 15:20:35.000000 arbmaster-0.1.0/README.md
--rw-rw-rw-   0        0        0      660 2024-04-30 16:58:53.000000 arbmaster-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-30 16:59:03.143051 arbmaster-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-30 16:59:03.039822 arbmaster-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-30 16:59:03.095778 arbmaster-0.1.0/src/arbmaster/
--rw-rw-rw-   0        0        0      168 2024-04-29 18:17:42.000000 arbmaster-0.1.0/src/arbmaster/__init__.py
--rw-rw-rw-   0        0        0     1347 2024-04-29 19:57:30.000000 arbmaster-0.1.0/src/arbmaster/calc.py
--rw-rw-rw-   0        0        0     5346 2024-04-29 21:10:32.000000 arbmaster-0.1.0/src/arbmaster/client.py
--rw-rw-rw-   0        0        0     6671 2024-04-28 11:35:15.000000 arbmaster-0.1.0/src/arbmaster/constants.py
--rw-rw-rw-   0        0        0     4225 2024-04-29 19:37:11.000000 arbmaster-0.1.0/src/arbmaster/ext.py
--rw-rw-rw-   0        0        0      527 2024-04-30 15:25:16.000000 arbmaster-0.1.0/src/arbmaster/logger.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:59:03.134838 arbmaster-0.1.0/src/arbmaster.egg-info/
--rw-rw-rw-   0        0        0     1912 2024-04-30 16:59:02.000000 arbmaster-0.1.0/src/arbmaster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      418 2024-04-30 16:59:03.000000 arbmaster-0.1.0/src/arbmaster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 16:59:03.000000 arbmaster-0.1.0/src/arbmaster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-30 16:59:03.000000 arbmaster-0.1.0/src/arbmaster.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-30 16:59:03.000000 arbmaster-0.1.0/src/arbmaster.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-30 16:59:03.130484 arbmaster-0.1.0/tests/
--rw-rw-rw-   0        0        0     1581 2024-04-29 21:39:40.000000 arbmaster-0.1.0/tests/test_calc.py
--rw-rw-rw-   0        0        0     3440 2024-04-30 15:23:09.000000 arbmaster-0.1.0/tests/test_client.py
--rw-rw-rw-   0        0        0     4542 2024-04-29 21:39:14.000000 arbmaster-0.1.0/tests/test_ext.py
+drwxrwxrwx   0        0        0        0 2024-04-30 19:47:47.032640 arbmaster-0.1.1/
+-rw-rw-rw-   0        0        0     1086 2024-04-30 17:51:08.000000 arbmaster-0.1.1/LICENCE
+-rw-rw-rw-   0        0        0     1912 2024-04-30 19:47:47.016938 arbmaster-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1342 2024-04-30 17:51:08.000000 arbmaster-0.1.1/README.md
+-rw-rw-rw-   0        0        0      660 2024-04-30 19:47:22.000000 arbmaster-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-30 19:47:47.035632 arbmaster-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 19:47:46.756690 arbmaster-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-30 19:47:46.886711 arbmaster-0.1.1/src/arbmaster/
+-rw-rw-rw-   0        0        0      168 2024-04-30 19:41:10.000000 arbmaster-0.1.1/src/arbmaster/__init__.py
+-rw-rw-rw-   0        0        0     1553 2024-04-30 19:29:20.000000 arbmaster-0.1.1/src/arbmaster/calc.py
+-rw-rw-rw-   0        0        0     5346 2024-04-30 17:51:08.000000 arbmaster-0.1.1/src/arbmaster/client.py
+-rw-rw-rw-   0        0        0     6671 2024-04-30 17:51:08.000000 arbmaster-0.1.1/src/arbmaster/constants.py
+-rw-rw-rw-   0        0        0     4363 2024-04-30 18:33:36.000000 arbmaster-0.1.1/src/arbmaster/ext.py
+-rw-rw-rw-   0        0        0      527 2024-04-30 17:51:08.000000 arbmaster-0.1.1/src/arbmaster/logger.py
+drwxrwxrwx   0        0        0        0 2024-04-30 19:47:47.016938 arbmaster-0.1.1/src/arbmaster.egg-info/
+-rw-rw-rw-   0        0        0     1912 2024-04-30 19:47:46.000000 arbmaster-0.1.1/src/arbmaster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      418 2024-04-30 19:47:46.000000 arbmaster-0.1.1/src/arbmaster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 19:47:46.000000 arbmaster-0.1.1/src/arbmaster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-30 19:47:46.000000 arbmaster-0.1.1/src/arbmaster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-30 19:47:46.000000 arbmaster-0.1.1/src/arbmaster.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 19:47:47.000472 arbmaster-0.1.1/tests/
+-rw-rw-rw-   0        0        0     1581 2024-04-30 17:51:09.000000 arbmaster-0.1.1/tests/test_calc.py
+-rw-rw-rw-   0        0        0     3440 2024-04-30 17:51:09.000000 arbmaster-0.1.1/tests/test_client.py
+-rw-rw-rw-   0        0        0     4542 2024-04-30 17:51:09.000000 arbmaster-0.1.1/tests/test_ext.py
```

### Comparing `arbmaster-0.1.0/LICENCE` & `arbmaster-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `arbmaster-0.1.0/PKG-INFO` & `arbmaster-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arbmaster
-Version: 0.1.0
+Version: 0.1.1
 Summary: Odds api automated arbitrage calculator
 Author: Rashoo18
 License: MIT License
 Project-URL: Homepage, https://github.com/Rashoo18/arbmaster
 Project-URL: Issues, https://github.com/Rashoo18/arbmaster/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `arbmaster-0.1.0/README.md` & `arbmaster-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `arbmaster-0.1.0/pyproject.toml` & `arbmaster-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "arbmaster"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
   "requests-cache",
   "colorlog",
 ]
 requires-python = ">=3.8"
 authors = [
   { name = "Rashoo18" },
```

### Comparing `arbmaster-0.1.0/src/arbmaster/calc.py` & `arbmaster-0.1.1/src/arbmaster/calc.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 from typing import Dict, List
 
 class ArbitrageCalc:
     
-    def __init__(self, odds: Dict[str, list], stake: float = 100) -> None:
+    def __init__(self, odds: Dict[str, list], stake: float = 100) -> None:        
         self.odds = [v[0]["price"] for v in odds.values() if len(v) >= 1]
         self.probability: float = self._calc_prob(self.odds)
         
         self.stakes: List[float] = self._calc_stakes(stake)
         self.payout: float = self._calc_payout()
         self.profit: float = self._calc_profit()
         self.roi: str = self._calc_roi()
     
     def is_arbitrage(self) -> bool:
-        return self.probability < 1
+        return 0 < self.probability < 1
     
     def _calc_prob(self, odds) -> float:
-        p = 0
+        p = 0.0
         for odd in odds:
-            p += 1 / odd
+            if odd is not None:
+                p += 1 / odd
         return p
     
     def _calc_stakes(self, stake: float) -> List[float]:
         stakes: List[float] = []
         for odd in self.odds:
-            bet = (stake * (1 / odd)) / self.probability
-            stakes.append(bet)
+            if self.is_arbitrage():
+                bet = (stake * (1 / odd)) / self.probability
+                stakes.append(bet)
         return stakes
     
     def _calc_payout(self) -> float:
-        payout: float = 0
-        for odd, stake in zip(self.odds, self.stakes):
-            payout = stake * odd
+        payout: float = 0.0
+        if self.is_arbitrage():
+            for odd, stake in zip(self.odds, self.stakes):
+                payout = stake * odd
         return round(payout, 2)
     
     def _calc_profit(self) -> float:
-        return round(self.payout - sum(self.stakes), 2)
+        return round(self.payout - sum(self.stakes), 2) if self.is_arbitrage() else 0.0
     
     def _calc_roi(self) -> str:
-        return "{:.2f}%".format((self.profit / sum(self.stakes)) * 100)
+        return "{:.2f}%".format((self.profit / sum(self.stakes)) * 100) if self.is_arbitrage() else "0.0%"
```

### Comparing `arbmaster-0.1.0/src/arbmaster/client.py` & `arbmaster-0.1.1/src/arbmaster/client.py`

 * *Files identical despite different names*

### Comparing `arbmaster-0.1.0/src/arbmaster/constants.py` & `arbmaster-0.1.1/src/arbmaster/constants.py`

 * *Files identical despite different names*

### Comparing `arbmaster-0.1.0/src/arbmaster/ext.py` & `arbmaster-0.1.1/src/arbmaster/ext.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,19 +31,19 @@
             "key": self.key,
             "title": self.title,
             "price": price
         }
 
 class Odds:
     def __init__(self, bookmakers: List[Bookmaker]) -> None:
-        home = max([b.home_odds for b in bookmakers])
-        away = max([b.away_odds for b in bookmakers])
+        home = max([b.home_odds for b in bookmakers if b.home_odds is not None], default=None)
+        away = max([b.away_odds for b in bookmakers if b.away_odds is not None], default=None)
         draw = max([b.draw_odds for b in bookmakers if b.draw_odds is not None], default=None)
-        self.home = [bm.json(home) for bm in bookmakers if bm.home_odds == home]
-        self.away = [bm.json(away) for bm in bookmakers if bm.away_odds == away]
+        self.home = [bm.json(home) for bm in bookmakers if bm.home_odds == home] if home is not None else []
+        self.away = [bm.json(away) for bm in bookmakers if bm.away_odds == away] if away is not None else []
         self.draw = [bm.json(draw) for bm in bookmakers if bm.draw_odds == draw] if draw is not None else []
 
     @classmethod
     def new(cls, odds_data: Dict[str, Any]) -> "Odds":
         home = [Bookmaker(bm['key'], bm['title'], bm['price'], 0) for bm in odds_data['home_team']]
         away = [Bookmaker(bm['key'], bm['title'], 0, bm['price']) for bm in odds_data['away_team']]
         draw = [Bookmaker(bm['key'], bm['title'], 0, 0, bm['price']) for bm in odds_data['draw'] if len(odds_data['draw']) >= 1]
```

### Comparing `arbmaster-0.1.0/src/arbmaster/logger.py` & `arbmaster-0.1.1/src/arbmaster/logger.py`

 * *Files identical despite different names*

### Comparing `arbmaster-0.1.0/src/arbmaster.egg-info/PKG-INFO` & `arbmaster-0.1.1/src/arbmaster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arbmaster
-Version: 0.1.0
+Version: 0.1.1
 Summary: Odds api automated arbitrage calculator
 Author: Rashoo18
 License: MIT License
 Project-URL: Homepage, https://github.com/Rashoo18/arbmaster
 Project-URL: Issues, https://github.com/Rashoo18/arbmaster/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `arbmaster-0.1.0/tests/test_calc.py` & `arbmaster-0.1.1/tests/test_calc.py`

 * *Files identical despite different names*

### Comparing `arbmaster-0.1.0/tests/test_client.py` & `arbmaster-0.1.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `arbmaster-0.1.0/tests/test_ext.py` & `arbmaster-0.1.1/tests/test_ext.py`

 * *Files identical despite different names*

