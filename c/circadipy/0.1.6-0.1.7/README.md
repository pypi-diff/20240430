# Comparing `tmp/circadipy-0.1.6.tar.gz` & `tmp/circadipy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circadipy-0.1.6.tar", last modified: Tue Dec  5 21:31:49 2023, max compression
+gzip compressed data, was "circadipy-0.1.7.tar", last modified: Mon Apr 29 19:16:32 2024, max compression
```

## Comparing `circadipy-0.1.6.tar` & `circadipy-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-12-05 21:31:49.400458 circadipy-0.1.6/
--rw-rw-rw-   0        0        0    35823 2023-12-05 12:37:50.000000 circadipy-0.1.6/LICENSE
--rw-rw-rw-   0        0        0        0 2023-12-05 12:37:50.000000 circadipy-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     2227 2023-12-05 21:31:49.400458 circadipy-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1875 2023-12-05 12:37:50.000000 circadipy-0.1.6/README.md
--rw-rw-rw-   0        0        0       82 2023-12-05 12:37:50.000000 circadipy-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0      547 2023-12-05 21:31:49.416088 circadipy-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-12-05 12:37:50.000000 circadipy-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-05 21:31:49.384828 circadipy-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-12-05 21:31:49.400458 circadipy-0.1.6/src/circadipy/
--rw-rw-rw-   0        0        0        0 2023-12-05 12:37:50.000000 circadipy-0.1.6/src/circadipy/__init__.py
--rw-rw-rw-   0        0        0    76597 2023-12-05 12:37:51.000000 circadipy-0.1.6/src/circadipy/chrono_plotter.py
--rw-rw-rw-   0        0        0    65011 2023-12-05 12:37:51.000000 circadipy-0.1.6/src/circadipy/chrono_reader.py
--rw-rw-rw-   0        0        0    23915 2023-12-05 12:37:51.000000 circadipy-0.1.6/src/circadipy/chrono_rhythm.py
--rw-rw-rw-   0        0        0    16070 2023-12-05 12:37:51.000000 circadipy-0.1.6/src/circadipy/chrono_simulation.py
-drwxrwxrwx   0        0        0        0 2023-12-05 21:31:49.400458 circadipy-0.1.6/src/circadipy.egg-info/
--rw-rw-rw-   0        0        0     2227 2023-12-05 21:31:49.000000 circadipy-0.1.6/src/circadipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-12-05 21:31:49.000000 circadipy-0.1.6/src/circadipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-05 21:31:49.000000 circadipy-0.1.6/src/circadipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-12-05 21:31:49.000000 circadipy-0.1.6/src/circadipy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-12-05 20:47:15.000000 circadipy-0.1.6/src/circadipy.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2024-04-29 19:16:32.825268 circadipy-0.1.7/
+-rw-rw-rw-   0        0        0    35823 2024-04-29 18:19:55.000000 circadipy-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0        0 2024-04-29 18:19:55.000000 circadipy-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     2710 2024-04-29 19:16:32.825268 circadipy-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1930 2024-04-29 18:19:55.000000 circadipy-0.1.7/README.md
+-rw-rw-rw-   0        0        0       82 2024-04-29 18:19:55.000000 circadipy-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0      816 2024-04-29 19:16:32.825268 circadipy-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-29 18:19:55.000000 circadipy-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 19:16:32.809287 circadipy-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2024-04-29 19:16:32.816049 circadipy-0.1.7/src/circadipy/
+-rw-rw-rw-   0        0        0        0 2024-04-29 18:19:55.000000 circadipy-0.1.7/src/circadipy/__init__.py
+-rw-rw-rw-   0        0        0    76597 2024-04-29 18:20:00.000000 circadipy-0.1.7/src/circadipy/chrono_plotter.py
+-rw-rw-rw-   0        0        0    65011 2024-04-29 18:20:00.000000 circadipy-0.1.7/src/circadipy/chrono_reader.py
+-rw-rw-rw-   0        0        0    23915 2024-04-29 18:20:00.000000 circadipy-0.1.7/src/circadipy/chrono_rhythm.py
+-rw-rw-rw-   0        0        0    16070 2024-04-29 18:20:00.000000 circadipy-0.1.7/src/circadipy/chrono_simulation.py
+drwxrwxrwx   0        0        0        0 2024-04-29 19:16:32.824271 circadipy-0.1.7/src/circadipy.egg-info/
+-rw-rw-rw-   0        0        0     2710 2024-04-29 19:16:32.000000 circadipy-0.1.7/src/circadipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2024-04-29 19:16:32.000000 circadipy-0.1.7/src/circadipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 19:16:32.000000 circadipy-0.1.7/src/circadipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      222 2024-04-29 19:16:32.000000 circadipy-0.1.7/src/circadipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-29 19:16:32.000000 circadipy-0.1.7/src/circadipy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-29 19:15:32.000000 circadipy-0.1.7/src/circadipy.egg-info/zip-safe
```

### Comparing `circadipy-0.1.6/LICENSE` & `circadipy-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `circadipy-0.1.6/README.md` & `circadipy-0.1.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-# Welcome to circadipy's page!
+# Welcome to Circadipy!
 =======================================
 
-Introducing **CircadiPy**, the a Python package for chronobiology analysis! 
+Introducing **CircadiPy**, a Python package for chronobiological analysis! 
 With seamless integration of powerful time series plotting libraries, 
-it empowers researchers to visualize and study circadian cycles with unrivaled versatility.
+it enables researchers to visualise and study circadian cycles with unrivalled versatility.
 
-Currently, the package supports the visualization of biological rhythms and their synchronization with external cues using:
+Currently, the package supports the visualisation of biological rhythms and their synchronisation with external cues using
 
-1. Actograms: An actogram is a graphical representation of an organism's activity or physiological data over time. It typically shows activity or physiological measurements (e.g., hormone levels, temperature) along the y-axis and time along the x-axis. Actograms are often used to visualize circadian rhythms and patterns of activity rest cycles.
+1. Actograms: An actogram is a graphical representation of an organism's activity or physiological data over time. It typically shows activity or physiological measurements (e.g. hormone levels, temperature) on the y-axis and time on the x-axis. Actograms are often used to visualise circadian rhythms and patterns of activity/rest cycles.
 
-2. Cosinor Analysis Plot: This plot is used to analyze and display the presence of rhythmic patterns in data. It's a graphical representation of the cosinor analysis, which fits a cosine curve to the data to estimate the rhythm's parameters like amplitude, acrophase (peak time), and period.
+2. Cosinor Analysis Plot: This plot is used to analyse and display the presence of rhythmic patterns in the data. It's a graphical representation of cosinor analysis, which fits a cosine curve to the data to estimate rhythm parameters such as amplitude, acrophase (peak time) and period.
 
-3. Raster Plot: A raster plot displays individual events or occurrences (such as action potentials in neurons) over time. In chronobiology, this can be used to show the timing of specific events in relation to the circadian cycle.
+3. Raster plot: A raster plot shows individual events or occurrences (such as action potentials in neurons) over time. In chronobiology this can be used to show the timing of specific events in relation to the circadian cycle.
 
-4. Histogram: A histogram can be used to show the distribution of events or measurements over a specific time period. For chronobiology, this might represent the distribution of activity bouts or physiological measurements across different time bins.
+4. Histogram: A histogram can be used to show the distribution of events or measurements over a period of time. In chronobiology this could be the distribution of activity bouts or physiological measurements over different time bins.
 
 ------------------------------------------------------------------------------------------------------------------------------
 
-CircadiPy also provides a built-in generator of simulated data, making possible the creation of custom datasets for testing, experimentation and comparison purposes.
+CircadiPy also has a built-in simulated data generator that allows the creation of custom data sets for testing, experimentation and comparison purposes.
+
+Please visit our documentation page for more information: https://circadipy.readthedocs.io/en/latest/
```

### Comparing `circadipy-0.1.6/src/circadipy/chrono_plotter.py` & `circadipy-0.1.7/src/circadipy/chrono_plotter.py`

 * *Files identical despite different names*

### Comparing `circadipy-0.1.6/src/circadipy/chrono_reader.py` & `circadipy-0.1.7/src/circadipy/chrono_reader.py`

 * *Files identical despite different names*

### Comparing `circadipy-0.1.6/src/circadipy/chrono_rhythm.py` & `circadipy-0.1.7/src/circadipy/chrono_rhythm.py`

 * *Files identical despite different names*

### Comparing `circadipy-0.1.6/src/circadipy/chrono_simulation.py` & `circadipy-0.1.7/src/circadipy/chrono_simulation.py`

 * *Files identical despite different names*

