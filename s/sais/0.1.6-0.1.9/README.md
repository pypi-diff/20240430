# Comparing `tmp/sais-0.1.6.tar.gz` & `tmp/sais-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sais-0.1.6.tar", last modified: Wed Apr 17 20:39:48 2024, max compression
+gzip compressed data, was "sais-0.1.9.tar", last modified: Tue Apr 30 09:07:43 2024, max compression
```

## Comparing `sais-0.1.6.tar` & `sais-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:39:48.471110 sais-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-04-17 20:39:45.000000 sais-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-04-17 20:39:48.471110 sais-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-17 20:39:45.000000 sais-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:39:48.471110 sais-0.1.6/sais/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-17 20:39:45.000000 sais-0.1.6/sais/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11946 2024-04-17 20:39:45.000000 sais-0.1.6/sais/benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9069 2024-04-17 20:39:45.000000 sais-0.1.6/sais/symbiotic_ais.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:39:48.471110 sais-0.1.6/sais.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-04-17 20:39:48.000000 sais-0.1.6/sais.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-17 20:39:48.000000 sais-0.1.6/sais.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 20:39:48.000000 sais-0.1.6/sais.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-17 20:39:48.000000 sais-0.1.6/sais.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-17 20:39:48.000000 sais-0.1.6/sais.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 20:39:48.471110 sais-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-17 20:39:45.000000 sais-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:43.676727 sais-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-04-30 09:07:40.000000 sais-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-30 09:07:43.676727 sais-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-30 09:07:40.000000 sais-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:43.676727 sais-0.1.9/sais/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-30 09:07:40.000000 sais-0.1.9/sais/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11946 2024-04-30 09:07:40.000000 sais-0.1.9/sais/benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9069 2024-04-30 09:07:40.000000 sais-0.1.9/sais/symbiotic_ais.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:43.676727 sais-0.1.9/sais.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-30 09:07:43.000000 sais-0.1.9/sais.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-30 09:07:43.000000 sais-0.1.9/sais.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:07:43.000000 sais-0.1.9/sais.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-30 09:07:43.000000 sais-0.1.9/sais.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-30 09:07:43.000000 sais-0.1.9/sais.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:07:43.676727 sais-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-30 09:07:40.000000 sais-0.1.9/setup.py
```

### Comparing `sais-0.1.6/LICENSE` & `sais-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sais-0.1.6/PKG-INFO` & `sais-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sais
-Version: 0.1.6
+Version: 0.1.9
 Summary: Symbiotic Artificial Immune Systems
 Home-page: https://github.com/Rqcker/SymbioticAIS
 Author: Junhao
 Author-email: junhao.song23@imperial.ac.uk
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.23.5
@@ -104,20 +104,24 @@
 
 ### Contact
 For any questions or suggestions, please contact us via:
 - [Email](mailto:junhao.song23@imperial.ac.uk)
 - [GitHub Issue](https://github.com/Rqcker/SymbioticAIS/issues)
 
 ### License
-This project is licensed under the [Apache license 2.0 License](LICENSE).
+This project is licensed under the [Apache License 2.0](LICENSE).
 
 ### Citation
 ```
 @misc{song2024sais,
       title={SAIS: A Novel Bio-Inspired Artificial Immune System Based on Symbiotic Paradigm}, 
       author={Junhao Song and Yingfang Yuan and Wei Pang},
       year={2024},
       eprint={2402.07244},
       archivePrefix={arXiv},
       primaryClass={cs.NE}
 }
 ```
+
+### Acknowledgements
+
+We extend our sincere thanks to [Dr. Wei Pang](https://pangwei.eu.org/) for his expert guidance and to [Dr. Yingfang Yuan](https://yuanjames.github.io/) for his pivotal contributions to this project. We also acknowledge Heriot-Watt University and Imperial College London for their support and the academic environment that facilitated our research.
```

### Comparing `sais-0.1.6/README.md` & `sais-0.1.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -93,20 +93,24 @@
 
 ### Contact
 For any questions or suggestions, please contact us via:
 - [Email](mailto:junhao.song23@imperial.ac.uk)
 - [GitHub Issue](https://github.com/Rqcker/SymbioticAIS/issues)
 
 ### License
-This project is licensed under the [Apache license 2.0 License](LICENSE).
+This project is licensed under the [Apache License 2.0](LICENSE).
 
 ### Citation
 ```
 @misc{song2024sais,
       title={SAIS: A Novel Bio-Inspired Artificial Immune System Based on Symbiotic Paradigm}, 
       author={Junhao Song and Yingfang Yuan and Wei Pang},
       year={2024},
       eprint={2402.07244},
       archivePrefix={arXiv},
       primaryClass={cs.NE}
 }
 ```
+
+### Acknowledgements
+
+We extend our sincere thanks to [Dr. Wei Pang](https://pangwei.eu.org/) for his expert guidance and to [Dr. Yingfang Yuan](https://yuanjames.github.io/) for his pivotal contributions to this project. We also acknowledge Heriot-Watt University and Imperial College London for their support and the academic environment that facilitated our research.
```

### Comparing `sais-0.1.6/sais/benchmarks.py` & `sais-0.1.9/sais/benchmarks.py`

 * *Files identical despite different names*

### Comparing `sais-0.1.6/sais/symbiotic_ais.py` & `sais-0.1.9/sais/symbiotic_ais.py`

 * *Files identical despite different names*

### Comparing `sais-0.1.6/sais.egg-info/PKG-INFO` & `sais-0.1.9/sais.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sais
-Version: 0.1.6
+Version: 0.1.9
 Summary: Symbiotic Artificial Immune Systems
 Home-page: https://github.com/Rqcker/SymbioticAIS
 Author: Junhao
 Author-email: junhao.song23@imperial.ac.uk
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.23.5
@@ -104,20 +104,24 @@
 
 ### Contact
 For any questions or suggestions, please contact us via:
 - [Email](mailto:junhao.song23@imperial.ac.uk)
 - [GitHub Issue](https://github.com/Rqcker/SymbioticAIS/issues)
 
 ### License
-This project is licensed under the [Apache license 2.0 License](LICENSE).
+This project is licensed under the [Apache License 2.0](LICENSE).
 
 ### Citation
 ```
 @misc{song2024sais,
       title={SAIS: A Novel Bio-Inspired Artificial Immune System Based on Symbiotic Paradigm}, 
       author={Junhao Song and Yingfang Yuan and Wei Pang},
       year={2024},
       eprint={2402.07244},
       archivePrefix={arXiv},
       primaryClass={cs.NE}
 }
 ```
+
+### Acknowledgements
+
+We extend our sincere thanks to [Dr. Wei Pang](https://pangwei.eu.org/) for his expert guidance and to [Dr. Yingfang Yuan](https://yuanjames.github.io/) for his pivotal contributions to this project. We also acknowledge Heriot-Watt University and Imperial College London for their support and the academic environment that facilitated our research.
```

