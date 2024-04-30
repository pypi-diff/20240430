# Comparing `tmp/planetMagFields-1.4.1.tar.gz` & `tmp/planetmagfields-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetMagFields-1.4.1.tar", last modified: Wed Feb 21 04:38:57 2024, max compression
+gzip compressed data, was "planetmagfields-1.4.2.tar", last modified: Tue Apr 30 14:53:45 2024, max compression
```

## Comparing `planetMagFields-1.4.1.tar` & `planetmagfields-1.4.2.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 ankit     (1000) ankit     (1000)        0 2024-02-21 04:38:57.865475 planetMagFields-1.4.1/
--rw-r--r--   0 ankit     (1000) ankit     (1000)    35149 2024-02-17 18:23:14.000000 planetMagFields-1.4.1/LICENSE
--rw-r--r--   0 ankit     (1000) ankit     (1000)     7641 2024-02-21 04:38:57.865475 planetMagFields-1.4.1/PKG-INFO
--rw-r--r--   0 ankit     (1000) ankit     (1000)     6127 2024-02-21 04:38:18.000000 planetMagFields-1.4.1/README.md
-drwxr-xr-x   0 ankit     (1000) ankit     (1000)        0 2024-02-21 04:38:57.865475 planetMagFields-1.4.1/planetMagFields.egg-info/
--rw-r--r--   0 ankit     (1000) ankit     (1000)     7641 2024-02-21 04:38:57.000000 planetMagFields-1.4.1/planetMagFields.egg-info/PKG-INFO
--rw-r--r--   0 ankit     (1000) ankit     (1000)     1012 2024-02-21 04:38:57.000000 planetMagFields-1.4.1/planetMagFields.egg-info/SOURCES.txt
--rw-r--r--   0 ankit     (1000) ankit     (1000)        1 2024-02-21 04:38:57.000000 planetMagFields-1.4.1/planetMagFields.egg-info/dependency_links.txt
--rw-r--r--   0 ankit     (1000) ankit     (1000)       56 2024-02-21 04:38:57.000000 planetMagFields-1.4.1/planetMagFields.egg-info/requires.txt
--rw-r--r--   0 ankit     (1000) ankit     (1000)       16 2024-02-21 04:38:57.000000 planetMagFields-1.4.1/planetMagFields.egg-info/top_level.txt
-drwxr-xr-x   0 ankit     (1000) ankit     (1000)        0 2024-02-21 04:38:57.855475 planetMagFields-1.4.1/planetmagfields/
--rw-r--r--   0 ankit     (1000) ankit     (1000)      157 2024-02-20 20:52:38.000000 planetMagFields-1.4.1/planetmagfields/__init__.py
-drwxr-xr-x   0 ankit     (1000) ankit     (1000)        0 2024-02-21 04:38:57.865475 planetMagFields-1.4.1/planetmagfields/data/
--rw-r--r--   0 ankit     (1000) ankit     (1000)    39975 2024-02-17 18:23:14.000000 planetMagFields-1.4.1/planetmagfields/data/earth_igrf13.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)      109 2024-02-17 18:23:14.000000 planetMagFields-1.4.1/planetmagfields/data/ganymede_kivelson2002.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)     3600 2024-02-19 23:08:07.000000 planetMagFields-1.4.1/planetmagfields/data/jupiter_jrm09.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)    29760 2024-02-17 18:23:14.000000 planetMagFields-1.4.1/planetmagfields/data/jupiter_jrm33.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)      340 2024-02-17 18:23:14.000000 planetMagFields-1.4.1/planetmagfields/data/jupiter_vip4.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)       46 2024-02-17 18:23:14.000000 planetMagFields-1.4.1/planetmagfields/data/mercury_anderson2012.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)      157 2024-02-17 18:23:14.000000 planetMagFields-1.4.1/planetmagfields/data/mercury_thebault2018.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)      161 2024-02-17 18:23:14.000000 planetMagFields-1.4.1/planetmagfields/data/mercury_wardinski2019.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)      167 2024-02-19 23:08:07.000000 planetMagFields-1.4.1/planetmagfields/data/neptune_connerny1991.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)      169 2024-02-17 18:23:14.000000 planetMagFields-1.4.1/planetmagfields/data/saturn_cassini11+.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)      153 2024-02-17 18:23:14.000000 planetMagFields-1.4.1/planetmagfields/data/saturn_cassini11.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)       37 2024-02-17 18:23:14.000000 planetMagFields-1.4.1/planetmagfields/data/saturn_cassinisoi.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)      176 2024-02-19 23:08:07.000000 planetMagFields-1.4.1/planetmagfields/data/uranus_connerny1987.dat
--rw-r--r--   0 ankit     (1000) ankit     (1000)     4812 2024-02-17 18:23:14.000000 planetMagFields-1.4.1/planetmagfields/libbfield.py
--rw-r--r--   0 ankit     (1000) ankit     (1000)     3819 2024-02-20 22:16:08.000000 planetMagFields-1.4.1/planetmagfields/libdata.py
--rw-r--r--   0 ankit     (1000) ankit     (1000)    14085 2024-02-20 23:54:48.000000 planetMagFields-1.4.1/planetmagfields/libgauss.py
--rw-r--r--   0 ankit     (1000) ankit     (1000)    11376 2024-02-21 00:06:21.000000 planetMagFields-1.4.1/planetmagfields/planet.py
--rw-r--r--   0 ankit     (1000) ankit     (1000)     6719 2024-02-20 23:54:37.000000 planetMagFields-1.4.1/planetmagfields/plotlib.py
--rw-r--r--   0 ankit     (1000) ankit     (1000)     7011 2024-02-17 18:23:14.000000 planetMagFields-1.4.1/planetmagfields/potextra.py
--rw-r--r--   0 ankit     (1000) ankit     (1000)     1030 2024-02-19 19:22:09.000000 planetMagFields-1.4.1/planetmagfields/utils.py
--rw-r--r--   0 ankit     (1000) ankit     (1000)     1558 2024-02-21 04:33:00.000000 planetMagFields-1.4.1/pyproject.toml
--rw-r--r--   0 ankit     (1000) ankit     (1000)       38 2024-02-21 04:38:57.865475 planetMagFields-1.4.1/setup.cfg
--rw-r--r--   0 ankit     (1000) ankit     (1000)     1229 2024-02-17 18:23:14.000000 planetMagFields-1.4.1/setup.py
+drwxr-xr-x   0 ankit     (1000) ankit     (1000)        0 2024-04-30 14:53:45.856647 planetmagfields-1.4.2/
+-rw-r--r--   0 ankit     (1000) ankit     (1000)    35149 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/LICENSE
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     8562 2024-04-30 14:53:45.856647 planetmagfields-1.4.2/PKG-INFO
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     7048 2024-04-29 13:24:10.000000 planetmagfields-1.4.2/README.md
+drwxr-xr-x   0 ankit     (1000) ankit     (1000)        0 2024-04-30 14:53:45.856647 planetmagfields-1.4.2/planetMagFields.egg-info/
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     8562 2024-04-30 14:53:45.000000 planetmagfields-1.4.2/planetMagFields.egg-info/PKG-INFO
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     1035 2024-04-30 14:53:45.000000 planetmagfields-1.4.2/planetMagFields.egg-info/SOURCES.txt
+-rw-r--r--   0 ankit     (1000) ankit     (1000)        1 2024-04-30 14:53:45.000000 planetmagfields-1.4.2/planetMagFields.egg-info/dependency_links.txt
+-rw-r--r--   0 ankit     (1000) ankit     (1000)       56 2024-04-30 14:53:45.000000 planetmagfields-1.4.2/planetMagFields.egg-info/requires.txt
+-rw-r--r--   0 ankit     (1000) ankit     (1000)       16 2024-04-30 14:53:45.000000 planetmagfields-1.4.2/planetMagFields.egg-info/top_level.txt
+drwxr-xr-x   0 ankit     (1000) ankit     (1000)        0 2024-04-30 14:53:45.846647 planetmagfields-1.4.2/planetmagfields/
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      159 2024-04-30 14:51:50.000000 planetmagfields-1.4.2/planetmagfields/__init__.py
+drwxr-xr-x   0 ankit     (1000) ankit     (1000)        0 2024-04-30 14:53:45.856647 planetmagfields-1.4.2/planetmagfields/data/
+-rw-r--r--   0 ankit     (1000) ankit     (1000)    39975 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/planetmagfields/data/earth_igrf13.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      109 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/planetmagfields/data/ganymede_kivelson2002.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     3600 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/planetmagfields/data/jupiter_jrm09.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)    29760 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/planetmagfields/data/jupiter_jrm33.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      340 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/planetmagfields/data/jupiter_vip4.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)       46 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/planetmagfields/data/mercury_anderson2012.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      157 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/planetmagfields/data/mercury_thebault2018.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      161 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/planetmagfields/data/mercury_wardinski2019.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      167 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/planetmagfields/data/neptune_connerny1991.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      169 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/planetmagfields/data/saturn_cassini11+.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      153 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/planetmagfields/data/saturn_cassini11.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)       37 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/planetmagfields/data/saturn_cassinisoi.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      176 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/planetmagfields/data/uranus_connerny1987.dat
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     4701 2024-02-26 00:30:26.000000 planetmagfields-1.4.2/planetmagfields/libbfield.py
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     3863 2024-02-26 01:09:53.000000 planetmagfields-1.4.2/planetmagfields/libdata.py
+-rw-r--r--   0 ankit     (1000) ankit     (1000)    14085 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/planetmagfields/libgauss.py
+-rw-r--r--   0 ankit     (1000) ankit     (1000)    11746 2024-04-30 14:44:50.000000 planetmagfields-1.4.2/planetmagfields/planet.py
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     6725 2024-04-30 14:45:13.000000 planetmagfields-1.4.2/planetmagfields/plotlib.py
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     7835 2024-02-26 01:04:13.000000 planetmagfields-1.4.2/planetmagfields/potextra.py
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     1030 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/planetmagfields/utils.py
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     1558 2024-04-30 14:52:06.000000 planetmagfields-1.4.2/pyproject.toml
+-rw-r--r--   0 ankit     (1000) ankit     (1000)       38 2024-04-30 14:53:45.856647 planetmagfields-1.4.2/setup.cfg
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     1229 2024-02-22 17:26:25.000000 planetmagfields-1.4.2/setup.py
+drwxr-xr-x   0 ankit     (1000) ankit     (1000)        0 2024-04-30 14:53:45.856647 planetmagfields-1.4.2/tests/
+-rw-r--r--   0 ankit     (1000) ankit     (1000)      856 2024-04-29 13:24:53.000000 planetmagfields-1.4.2/tests/test_planetBr.py
```

### Comparing `planetMagFields-1.4.1/LICENSE` & `planetmagfields-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `planetMagFields-1.4.1/PKG-INFO` & `planetmagfields-1.4.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetMagFields
-Version: 1.4.1
+Version: 1.4.2
 Summary: Routines to easily access information about magnetic fields of planets in our solar system and visualize them in both 2D and 3D
 Author: Barik, Ankit
 Author-email: Ankit Barik <ankit.barik@gmail.com>
 Maintainer-email: Ankit Barik <ankit.barik@gmail.com>, Regupathi Angappan <rangapp1@jhu.edu>
 Project-URL: Homepage, https://ankitbarik.github.io/planetMagFields/
 Project-URL: Issues, https://github.com/AnkitBarik/planetMagFields/issues
 Keywords: Spherical Harmonics,Planetary Science,Spectra,Magnetic Field,Visualization,3D visualization
@@ -46,14 +46,16 @@
 
 [Features and examples](#features-and-examples)
 
 [Jupyter notebook](#jupyter-notebook)
 
 [Documentation](#documentation)
 
+[Code contribution and reporting issues](#code-contribution-and-reporting-issues)
+
 [Acknowledgements](#acknowledgements)
 
 # Prerequisites
 
 `planetMagFields` requires [NumPy](https://numpy.org/), [Matplotlib](https://matplotlib.org/) and [SciPy](https://www.scipy.org/). Other than that, the following external libraries are used for a few different functions:
 
  - 2D plotting for map projections other than Hammer : [Cartopy](https://scitools.org.uk/cartopy/docs/latest/) library
@@ -185,11 +187,21 @@
 </p>
 
 # Documentation
 
 Full list of features with examples as well as the magnetic field models used are described in detail in the documentation,
 available here: https://ankitbarik.github.io/planetMagFields/
 
+# Code contribution and reporting issues
+
+`planetMagFields` is an open source project and anyone is welcome to contribute to it. If you wish to contribute to this project, please follow the guidelines below:
+
+ - Please make sure the tests pass before opening a pull request. 
+ - Please follow Python [PEP-8](https://peps.python.org/pep-0008/) guidelines when it comes to code style.
+ - If you wish to add new data file, please name it following the convention `<planet>_<model>.dat`, where `planet` and `model` denote the names of the planet and the magnetic field model being used. See the `data` directory for examples.
+ - If you implement a new feature or data source, please update the documentation accordingly. 
+
+Please report any bugs or other issues through [GitHub Issues](https://github.com/AnkitBarik/planetMagFields/issues). 
 
 # Acknowledgements
 
 I would like to thank [Regupathi Angappan](https://github.com/reguang) for motivating me to create this package, testing it and for writing the Jupyter notebook. I thank [Jon Aurnou](https://epss.ucla.edu/people/faculty/543/) for testing it out and pointing out runtime errors. I would like to thank [Thomas Gastine](https://github.com/tgastine) for comparing the plots with real data and pointing out a normalization error which has been fixed. Thanks a lot to [Arthus](https://github.com/arthus701) for adding the `setup.py`.
```

### Comparing `planetMagFields-1.4.1/README.md` & `planetmagfields-1.4.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 [Features and examples](#features-and-examples)
 
 [Jupyter notebook](#jupyter-notebook)
 
 [Documentation](#documentation)
 
+[Code contribution and reporting issues](#code-contribution-and-reporting-issues)
+
 [Acknowledgements](#acknowledgements)
 
 # Prerequisites
 
 `planetMagFields` requires [NumPy](https://numpy.org/), [Matplotlib](https://matplotlib.org/) and [SciPy](https://www.scipy.org/). Other than that, the following external libraries are used for a few different functions:
 
  - 2D plotting for map projections other than Hammer : [Cartopy](https://scitools.org.uk/cartopy/docs/latest/) library
@@ -152,11 +154,21 @@
 </p>
 
 # Documentation
 
 Full list of features with examples as well as the magnetic field models used are described in detail in the documentation,
 available here: https://ankitbarik.github.io/planetMagFields/
 
+# Code contribution and reporting issues
+
+`planetMagFields` is an open source project and anyone is welcome to contribute to it. If you wish to contribute to this project, please follow the guidelines below:
+
+ - Please make sure the tests pass before opening a pull request. 
+ - Please follow Python [PEP-8](https://peps.python.org/pep-0008/) guidelines when it comes to code style.
+ - If you wish to add new data file, please name it following the convention `<planet>_<model>.dat`, where `planet` and `model` denote the names of the planet and the magnetic field model being used. See the `data` directory for examples.
+ - If you implement a new feature or data source, please update the documentation accordingly. 
+
+Please report any bugs or other issues through [GitHub Issues](https://github.com/AnkitBarik/planetMagFields/issues). 
 
 # Acknowledgements
 
 I would like to thank [Regupathi Angappan](https://github.com/reguang) for motivating me to create this package, testing it and for writing the Jupyter notebook. I thank [Jon Aurnou](https://epss.ucla.edu/people/faculty/543/) for testing it out and pointing out runtime errors. I would like to thank [Thomas Gastine](https://github.com/tgastine) for comparing the plots with real data and pointing out a normalization error which has been fixed. Thanks a lot to [Arthus](https://github.com/arthus701) for adding the `setup.py`.
```

### Comparing `planetMagFields-1.4.1/planetMagFields.egg-info/PKG-INFO` & `planetmagfields-1.4.2/planetMagFields.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetMagFields
-Version: 1.4.1
+Version: 1.4.2
 Summary: Routines to easily access information about magnetic fields of planets in our solar system and visualize them in both 2D and 3D
 Author: Barik, Ankit
 Author-email: Ankit Barik <ankit.barik@gmail.com>
 Maintainer-email: Ankit Barik <ankit.barik@gmail.com>, Regupathi Angappan <rangapp1@jhu.edu>
 Project-URL: Homepage, https://ankitbarik.github.io/planetMagFields/
 Project-URL: Issues, https://github.com/AnkitBarik/planetMagFields/issues
 Keywords: Spherical Harmonics,Planetary Science,Spectra,Magnetic Field,Visualization,3D visualization
@@ -46,14 +46,16 @@
 
 [Features and examples](#features-and-examples)
 
 [Jupyter notebook](#jupyter-notebook)
 
 [Documentation](#documentation)
 
+[Code contribution and reporting issues](#code-contribution-and-reporting-issues)
+
 [Acknowledgements](#acknowledgements)
 
 # Prerequisites
 
 `planetMagFields` requires [NumPy](https://numpy.org/), [Matplotlib](https://matplotlib.org/) and [SciPy](https://www.scipy.org/). Other than that, the following external libraries are used for a few different functions:
 
  - 2D plotting for map projections other than Hammer : [Cartopy](https://scitools.org.uk/cartopy/docs/latest/) library
@@ -185,11 +187,21 @@
 </p>
 
 # Documentation
 
 Full list of features with examples as well as the magnetic field models used are described in detail in the documentation,
 available here: https://ankitbarik.github.io/planetMagFields/
 
+# Code contribution and reporting issues
+
+`planetMagFields` is an open source project and anyone is welcome to contribute to it. If you wish to contribute to this project, please follow the guidelines below:
+
+ - Please make sure the tests pass before opening a pull request. 
+ - Please follow Python [PEP-8](https://peps.python.org/pep-0008/) guidelines when it comes to code style.
+ - If you wish to add new data file, please name it following the convention `<planet>_<model>.dat`, where `planet` and `model` denote the names of the planet and the magnetic field model being used. See the `data` directory for examples.
+ - If you implement a new feature or data source, please update the documentation accordingly. 
+
+Please report any bugs or other issues through [GitHub Issues](https://github.com/AnkitBarik/planetMagFields/issues). 
 
 # Acknowledgements
 
 I would like to thank [Regupathi Angappan](https://github.com/reguang) for motivating me to create this package, testing it and for writing the Jupyter notebook. I thank [Jon Aurnou](https://epss.ucla.edu/people/faculty/543/) for testing it out and pointing out runtime errors. I would like to thank [Thomas Gastine](https://github.com/tgastine) for comparing the plots with real data and pointing out a normalization error which has been fixed. Thanks a lot to [Arthus](https://github.com/arthus701) for adding the `setup.py`.
```

### Comparing `planetMagFields-1.4.1/planetMagFields.egg-info/SOURCES.txt` & `planetmagfields-1.4.2/planetMagFields.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -23,8 +23,9 @@
 planetmagfields/data/mercury_anderson2012.dat
 planetmagfields/data/mercury_thebault2018.dat
 planetmagfields/data/mercury_wardinski2019.dat
 planetmagfields/data/neptune_connerny1991.dat
 planetmagfields/data/saturn_cassini11+.dat
 planetmagfields/data/saturn_cassini11.dat
 planetmagfields/data/saturn_cassinisoi.dat
-planetmagfields/data/uranus_connerny1987.dat
+planetmagfields/data/uranus_connerny1987.dat
+tests/test_planetBr.py
```

### Comparing `planetMagFields-1.4.1/planetmagfields/data/earth_igrf13.dat` & `planetmagfields-1.4.2/planetmagfields/data/earth_igrf13.dat`

 * *Files identical despite different names*

### Comparing `planetMagFields-1.4.1/planetmagfields/data/jupiter_jrm09.dat` & `planetmagfields-1.4.2/planetmagfields/data/jupiter_jrm09.dat`

 * *Files identical despite different names*

### Comparing `planetMagFields-1.4.1/planetmagfields/data/jupiter_jrm33.dat` & `planetmagfields-1.4.2/planetmagfields/data/jupiter_jrm33.dat`

 * *Files identical despite different names*

### Comparing `planetMagFields-1.4.1/planetmagfields/libbfield.py` & `planetmagfields-1.4.2/planetmagfields/libbfield.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,18 +38,15 @@
         Dipole tilt co-latitude in degrees
     dipPhi : float
         Dipole longitude in degrees
     """
 
     p2D,th2D = get_grid(nphi=nphi,ntheta=ntheta)
 
-    m0file = ( (planet.name == "mercury" and planet.model == "anderson2012")
-            or (planet.name == "saturn") )
-
-    if m0file:
+    if planet.mmax == 0:
         Br = getBm0(planet.lmax,
                     planet.glm,
                     r,
                     p2D,
                     th2D) * 1e-3
         dipTheta = 0.
         dipPhi = 0.
```

### Comparing `planetMagFields-1.4.1/planetmagfields/libdata.py` & `planetmagfields-1.4.2/planetmagfields/libdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,14 +124,17 @@
 
 
     # Insert (0,0) -> 0 for less confusion
 
     glm = np.insert(g,0,0.)
     hlm = np.insert(h,0,0.)
 
+    # Ensure type int
+    lmax = int(lmax)
+
     if mmax == 0:
         idx = np.arange(lmax+1)
     else:
         idx = gen_idx(lmax)
         mmax = lmax
 
     return glm,hlm,lmax,idx,mmax
```

### Comparing `planetMagFields-1.4.1/planetmagfields/libgauss.py` & `planetmagfields-1.4.2/planetmagfields/libgauss.py`

 * *Files identical despite different names*

### Comparing `planetMagFields-1.4.1/planetmagfields/planet.py` & `planetmagfields-1.4.2/planetmagfields/planet.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,20 +113,20 @@
 
         plt.figure(figsize=(12,6.75))
 
         if r is None:
             r = self.r
 
         if r == self.r:
-            ax,cbar = plotSurf(self.p2D,self.th2D,self.Br,levels=levels,cmap=cmap,proj=proj)
+            ax,cbar,proj = plotSurf(self.p2D,self.th2D,self.Br,levels=levels,cmap=cmap,proj=proj)
         else:
             self.p2D, self.th2D, self.Br, self.dipTheta, self.dipPhi = \
                     getBr(planet=self,r=r,info=False)
             self.r = r
-            ax,cbar = plotSurf(self.p2D,self.th2D,self.Br,levels=levels,cmap=cmap,proj=proj)
+            ax,cbar,proj = plotSurf(self.p2D,self.th2D,self.Br,levels=levels,cmap=cmap,proj=proj)
 
         cbar.ax.set_xlabel(r'Radial magnetic field ($\mu$T)',fontsize=25)
         cbar.ax.tick_params(labelsize=20)
 
         if r==1:
             radLabel = '  Surface'
         else:
@@ -144,14 +144,27 @@
 
         if self.name == 'earth':
             title = title + ', %d' %self.year
 
         ax.set_title(title,fontsize=25,pad=20)
         plt.tight_layout()
 
+
+    def extrapolate(self,rout):
+        from .potextra import get_pol_from_Gauss, extrapot
+
+        # Create poloidal potential from glm and glm
+        bpol = get_pol_from_Gauss(self.name,self.glm,self.hlm,
+                                  self.lmax,self.idx)
+
+        br,btheta,bphi = extrapot(bpol,self.idx,self.lmax,1,rout,self.nphi)
+
+        return br,btheta,bphi
+
+
     def writeVtsFile(self,potExtra=False,ratio_out=2,nrout=32):
         """
         Writes an unstructured vtk (.vts) file for 3D visualization. Uses the
         SHTns library for potential extrapolation and the pyevtk library for
         writing the vtk file.
 
         Parameters
@@ -168,15 +181,15 @@
         -------
         None
         """
         from .potextra import extrapot, writeVts
 
         rout = np.linspace(1,ratio_out,nrout)
         if potExtra:
-            brout, btout, bpout = extrapot(self.lmax,1.,self.Br,rout)
+            brout, btout, bpout = self.extrapolate(rout)
         else:
             brout = self.Br
             btout = np.zeros_like(self.Br)
             bpout = np.zeros_like(self.Br)
 
         writeVts(self.name,brout,btout,bpout,rout,self.theta,self.phi)
```

### Comparing `planetMagFields-1.4.1/planetmagfields/plotlib.py` & `planetmagfields-1.4.2/planetmagfields/plotlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
             transform=ccrs.PlateCarree(),cmap=cmap,norm=divnorm,extend='both')
 
     cbar = plt.colorbar(cont,orientation='horizontal',fraction=0.06, pad=0.04,ticks=[-bmax,0,bmax])
 
     ax.axis('equal')
     ax.axis('off')
 
-    return ax, cbar
+    return ax, cbar, proj
 
 def plotB_subplot(ax,p2D,th2D,B,planetname="earth",levels=60,cmap='RdBu_r',proj='Mollweide'):
     """
     Plots subplot of magnetic field on a surface defined by 2D arrays
     of longitude and co-latitude. The subplot is defined by the axes handle ax.
 
     Parameters
```

### Comparing `planetMagFields-1.4.1/planetmagfields/potextra.py` & `planetmagfields-1.4.2/planetmagfields/potextra.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,35 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import numpy as np
 
-def extrapot(rcmb,brcmb,rout,lmax=None):
+def get_pol_from_Gauss(planetname,glm,hlm,lmax,idx):
+
+    bpol = np.zeros(len(glm),dtype=np.complex128)
+
+    for l in range(1,lmax+1):
+        for m in range(l+1):
+
+            if planetname in ["earth"]:
+                fac_m = 1.
+            else:
+                fac_m = (-1)**m
+
+            if m == 0:
+                norm = np.sqrt((4*np.pi/(2*l+1)))/l
+            else:
+                norm = np.sqrt((2*np.pi/(2*l+1)))/l
+
+            bpol[idx[l,m]] = norm*fac_m*(glm[idx[l,m]] - 1j*hlm[idx[l,m]])
+
+    return bpol
+
+
+def extrapot(bpol,idx,lmax,rcmb,rout,nphi=None):
     """
     This function extrapolates a potential field to an array of desired radial
     levels. It uses the SHTns library (https://bitbucket.org/nschaeff/shtns)
     for spherical harmonic transforms.
 
     Parameters
     ----------
@@ -28,41 +50,50 @@
         3D array of extrapolated radial magnetic field, shape : (nphi,ntheta,nr)
     btout : ndarray(float, ndim=3)
         3D array of extrapolated co-latitudinal magnetic field, shape : (nphi,ntheta,nr)
     bpout : ndarray(float, ndim=3)
         3D array of extrapolated azimuthal magnetic field, shape : (nphi,ntheta,nr)
     """
 
-    nphi, ntheta = brcmb.shape
+    # nphi, ntheta = brcmb.shape
     nrout = len(rout)
 
-    polar_opt = 1e-10
+    polar_opt = 1e-15
+
+    if nphi is None:
+        nphi   = int(max(256,lmax*3))
+    ntheta = nphi//2
 
-    if lmax is None:
-        lmax = int(nphi/3)
     mmax = lmax
 
     try:
         import shtns
     except ImportError:
         print("Potential extrapolation requires the SHTns library")
         print("It can be obtained here: https://bitbucket.org/nschaeff/shtns")
 
-    norm=shtns.sht_orthonormal | shtns.SHT_NO_CS_PHASE
+    norm=shtns.sht_orthonormal
 
     sh = shtns.sht(lmax,mmax=mmax,norm=norm)
     ntheta, nphi = sh.set_grid(ntheta, nphi, polar_opt=polar_opt)
 
-
     L = sh.l * (sh.l + 1)
 
-    brlm = sh.analys(brcmb.T)
-    bpolcmb = np.zeros_like(brlm)
-    bpolcmb[1:] = rcmb**2 * brlm[1:]/L[1:]
-    btor = np.zeros_like(brlm)
+    # Take care of shtns index convention
+
+    bpolcmb = sh.spec_array()
+
+    for l in range(1,lmax+1):
+        for m in range(l+1):
+            bpolcmb[sh.idx(l,m)] = bpol[idx[l,m]]
+
+    # brlm = sh.analys(brcmb.T)
+    # bpolcmb = np.zeros_like(brlm)
+    # bpolcmb[1:] = rcmb**2 * brlm[1:]/L[1:]
+    btor = np.zeros_like(bpolcmb)
 
     brout = np.zeros([ntheta,nphi,nrout])
     btout = np.zeros([ntheta,nphi,nrout])
     bpout = np.zeros([ntheta,nphi,nrout])
 
     for k,radius in enumerate(rout):
         print(("%d/%d" %(k,nrout)))
@@ -73,17 +104,17 @@
         brout[...,k] = sh.synth(brlm)
 
         dbpoldr = -sh.l/radius * bpol
         slm = dbpoldr
 
         btout[...,k], bpout[...,k] = sh.synth(slm,btor)
 
-    brout = np.transpose(brout,(1,0,2))
-    btout = np.transpose(btout,(1,0,2))
-    bpout = np.transpose(bpout,(1,0,2))
+    brout = np.transpose(brout,(1,0,2))*1e-3 # Convert to microteslas
+    btout = np.transpose(btout,(1,0,2))*1e-3 # Convert to microteslas
+    bpout = np.transpose(bpout,(1,0,2))*1e-3 # Convert to microteslas
 
     return brout, btout, bpout
 
 def get_grid(r,theta,phi):
     """
     Produces a 3D grid for storing values of extrapolated field. Used in producing
     vtk file for 3D visualization.
```

### Comparing `planetMagFields-1.4.1/planetmagfields/utils.py` & `planetmagfields-1.4.2/planetmagfields/utils.py`

 * *Files identical despite different names*

### Comparing `planetMagFields-1.4.1/pyproject.toml` & `planetmagfields-1.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "planetMagFields"
-version = "1.4.1"
+version = "1.4.2"
 authors = [
   { name="Ankit Barik", email="ankit.barik@gmail.com" },
 ]
 maintainers = [
   { name="Ankit Barik", email="ankit.barik@gmail.com" },
   { name="Regupathi Angappan", email="rangapp1@jhu.edu" },
 ]
```

### Comparing `planetMagFields-1.4.1/setup.py` & `planetmagfields-1.4.2/setup.py`

 * *Files identical despite different names*

