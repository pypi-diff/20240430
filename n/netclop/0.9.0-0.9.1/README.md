# Comparing `tmp/netclop-0.9.0.tar.gz` & `tmp/netclop-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netclop-0.9.0.tar", max compression
+gzip compressed data, was "netclop-0.9.1.tar", max compression
```

## Comparing `netclop-0.9.0.tar` & `netclop-0.9.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1073 2024-01-19 15:14:14.969018 netclop-0.9.0/LICENSE
--rw-r--r--   0        0        0     2079 2024-02-14 17:17:35.560515 netclop-0.9.0/README.md
--rw-r--r--   0        0        0       89 2024-02-03 23:32:01.877863 netclop-0.9.0/netclop/__init__.py
--rw-r--r--   0        0        0     4543 2024-02-06 16:05:02.148859 netclop-0.9.0/netclop/cli.py
--rw-r--r--   0        0        0      408 2024-02-05 17:28:52.598586 netclop-0.9.0/netclop/config/default_config.yaml
--rw-r--r--   0        0        0      618 2024-02-04 16:35:41.238652 netclop-0.9.0/netclop/config_loader.py
--rw-r--r--   0        0        0      153 2024-02-03 23:10:21.637289 netclop-0.9.0/netclop/constants.py
--rw-r--r--   0        0        0     7208 2024-02-06 16:05:54.225168 netclop-0.9.0/netclop/networkops.py
--rw-r--r--   0        0        0     6808 2024-02-14 17:14:28.444368 netclop-0.9.0/netclop/plot.py
--rw-r--r--   0        0        0     3857 2024-02-03 23:32:40.821792 netclop-0.9.0/netclop/sigcore.py
--rw-r--r--   0        0        0      651 2024-02-14 17:16:28.482796 netclop-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     2860 1970-01-01 00:00:00.000000 netclop-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-01-19 15:14:14.969018 netclop-0.9.1/LICENSE
+-rw-r--r--   0        0        0     2080 2024-02-16 22:27:19.750473 netclop-0.9.1/README.md
+-rw-r--r--   0        0        0       89 2024-02-03 23:32:01.877863 netclop-0.9.1/netclop/__init__.py
+-rw-r--r--   0        0        0     4543 2024-02-06 16:05:02.148859 netclop-0.9.1/netclop/cli.py
+-rw-r--r--   0        0        0      408 2024-02-05 17:28:52.598586 netclop-0.9.1/netclop/config/default_config.yaml
+-rw-r--r--   0        0        0      618 2024-02-04 16:35:41.238652 netclop-0.9.1/netclop/config_loader.py
+-rw-r--r--   0        0        0      153 2024-02-03 23:10:21.637289 netclop-0.9.1/netclop/constants.py
+-rw-r--r--   0        0        0     7208 2024-02-06 16:05:54.225168 netclop-0.9.1/netclop/networkops.py
+-rw-r--r--   0        0        0     6741 2024-02-16 22:27:19.750709 netclop-0.9.1/netclop/plot.py
+-rw-r--r--   0        0        0     3857 2024-02-03 23:32:40.821792 netclop-0.9.1/netclop/sigcore.py
+-rw-r--r--   0        0        0      651 2024-02-16 22:31:01.993449 netclop-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     2861 1970-01-01 00:00:00.000000 netclop-0.9.1/PKG-INFO
```

### Comparing `netclop-0.9.0/LICENSE` & `netclop-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netclop-0.9.0/README.md` & `netclop-0.9.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 ##### Options
 * `--output`, `-o` Path to the output file where the node list will be written.
 * `--significance-cluster`, `-sc` Perform significance clustering to delineate noise
 * `--res` Specifies the H3 grid resolution (range 0-15) used for domain discretization.
 * `--markov-time`, `-mt` Tuning parameter of the spatial scale of detected structure."
 * `--variable-markov-time`/`--static-markov-time` Allows for dynamic adjustment of Markov time with varying network density.
-* `--cooling-rate`, `-cr` Cooling rate of simulated annealing
+* `--cooling-rate`, `-cr` Cooling rate of simulated annealing.
 
 #### Plot
 Plots a node list.
 
 ```
 netclop plot NODE_PATH [OPTIONS]
 ```
```

### Comparing `netclop-0.9.0/netclop/cli.py` & `netclop-0.9.1/netclop/cli.py`

 * *Files identical despite different names*

### Comparing `netclop-0.9.0/netclop/config_loader.py` & `netclop-0.9.1/netclop/config_loader.py`

 * *Files identical despite different names*

### Comparing `netclop-0.9.0/netclop/networkops.py` & `netclop-0.9.1/netclop/networkops.py`

 * *Files identical despite different names*

### Comparing `netclop-0.9.0/netclop/plot.py` & `netclop-0.9.1/netclop/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
             )
         else:
             # Default to significant colors
             gdf["color"] = gdf["module"].apply(
                 lambda x: modules_colors[x]["significant"]
             )
 
-        self.gdf = gdf.sort_values(by=["module", "significant"], ascending=[True, False])
+        self.gdf = gdf
 
     @classmethod
     def from_file(cls, path: Path) -> typing.Self:
         """Make GeoDataFrame from file."""
         df = pd.read_csv(path)
         return cls.from_dataframe(df)
```

### Comparing `netclop-0.9.0/netclop/sigcore.py` & `netclop-0.9.1/netclop/sigcore.py`

 * *Files identical despite different names*

### Comparing `netclop-0.9.0/pyproject.toml` & `netclop-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "netclop"
-version = "0.9.0"
+version = "0.9.1"
 description = "Network clustering operations for geophysical fluid transport"
 authors = ["KarstenEconomou <economoukarsten@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 click = "^8.1.7"
```

### Comparing `netclop-0.9.0/PKG-INFO` & `netclop-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netclop
-Version: 0.9.0
+Version: 0.9.1
 Summary: Network clustering operations for geophysical fluid transport
 Author: KarstenEconomou
 Author-email: economoukarsten@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
@@ -64,15 +64,15 @@
 
 ##### Options
 * `--output`, `-o` Path to the output file where the node list will be written.
 * `--significance-cluster`, `-sc` Perform significance clustering to delineate noise
 * `--res` Specifies the H3 grid resolution (range 0-15) used for domain discretization.
 * `--markov-time`, `-mt` Tuning parameter of the spatial scale of detected structure."
 * `--variable-markov-time`/`--static-markov-time` Allows for dynamic adjustment of Markov time with varying network density.
-* `--cooling-rate`, `-cr` Cooling rate of simulated annealing
+* `--cooling-rate`, `-cr` Cooling rate of simulated annealing.
 
 #### Plot
 Plots a node list.
 
 ```
 netclop plot NODE_PATH [OPTIONS]
 ```
```

