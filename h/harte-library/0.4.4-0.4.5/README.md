# Comparing `tmp/harte-library-0.4.4.tar.gz` & `tmp/harte_library-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harte-library-0.4.4.tar", last modified: Sun Mar 24 17:24:51 2024, max compression
+gzip compressed data, was "harte_library-0.4.5.tar", last modified: Tue Apr 30 12:48:51 2024, max compression
```

## Comparing `harte-library-0.4.4.tar` & `harte_library-0.4.5.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:24:51.780993 harte-library-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-24 17:24:34.000000 harte-library-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-03-24 17:24:51.780993 harte-library-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-03-24 17:24:34.000000 harte-library-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:24:51.780993 harte-library-0.4.4/harte/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 17:24:34.000000 harte-library-0.4.4/harte/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-03-24 17:24:34.000000 harte-library-0.4.4/harte/harte.lark
--rw-r--r--   0 runner    (1001) docker     (127)    11367 2024-03-24 17:24:34.000000 harte-library-0.4.4/harte/harte.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-03-24 17:24:34.000000 harte-library-0.4.4/harte/interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-03-24 17:24:34.000000 harte-library-0.4.4/harte/mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-03-24 17:24:34.000000 harte-library-0.4.4/harte/parse_harte.py
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-03-24 17:24:34.000000 harte-library-0.4.4/harte/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:24:51.780993 harte-library-0.4.4/harte_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-03-24 17:24:51.000000 harte-library-0.4.4/harte_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-24 17:24:51.000000 harte-library-0.4.4/harte_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 17:24:51.000000 harte-library-0.4.4/harte_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-24 17:24:51.000000 harte-library-0.4.4/harte_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-24 17:24:51.000000 harte-library-0.4.4/harte_library.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 17:24:51.780993 harte-library-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-24 17:24:34.000000 harte-library-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:24:51.780993 harte-library-0.4.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 17:24:34.000000 harte-library-0.4.4/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-03-24 17:24:34.000000 harte-library-0.4.4/test/test_harte.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:48:51.330247 harte_library-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-30 12:48:31.000000 harte_library-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5991 2024-04-30 12:48:51.330247 harte_library-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-04-30 12:48:31.000000 harte_library-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:48:51.326247 harte_library-0.4.5/harte/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:48:31.000000 harte_library-0.4.5/harte/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-30 12:48:31.000000 harte_library-0.4.5/harte/harte.lark
+-rw-r--r--   0 runner    (1001) docker     (127)    11367 2024-04-30 12:48:31.000000 harte_library-0.4.5/harte/harte.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-30 12:48:31.000000 harte_library-0.4.5/harte/interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-30 12:48:31.000000 harte_library-0.4.5/harte/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-30 12:48:31.000000 harte_library-0.4.5/harte/parse_harte.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-04-30 12:48:31.000000 harte_library-0.4.5/harte/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:48:51.330247 harte_library-0.4.5/harte_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5991 2024-04-30 12:48:51.000000 harte_library-0.4.5/harte_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-30 12:48:51.000000 harte_library-0.4.5/harte_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 12:48:51.000000 harte_library-0.4.5/harte_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-30 12:48:51.000000 harte_library-0.4.5/harte_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-30 12:48:51.000000 harte_library-0.4.5/harte_library.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 12:48:51.330247 harte_library-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-30 12:48:31.000000 harte_library-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:48:51.330247 harte_library-0.4.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:48:31.000000 harte_library-0.4.5/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-30 12:48:31.000000 harte_library-0.4.5/test/test_harte.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-30 12:48:31.000000 harte_library-0.4.5/test/test_interval.py
```

### Comparing `harte-library-0.4.4/LICENSE` & `harte_library-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `harte-library-0.4.4/PKG-INFO` & `harte_library-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harte-library
-Version: 0.4.4
+Version: 0.4.5
 Summary: Library for parsing Harte chords and converting them to Music21
 Author: Andrea Poltronieri
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -22,15 +22,15 @@
 
 The **Harte Library** is an extension of the [music21 library](http://web.mit.edu/music21/) tailored for working with music chords encoded according to the [Harte Notation](https://ismir2005.ismir.net/proceedings/1080.pdf).
 
 This project is a component of [ChoCo](https://github.com/smashub/choco), a comprehensive dataset containing over 20,000 timed chord annotations sourced from integrated and standardized scores and tracks.
 
 The library has the following dependencies:
 
-- [music21](http://web.mit.edu/music21/): as an extension of the library itself;
+- [music21](http://web.mit.edu/music21/): the base library the *harte-library* extends;
 - [Lark](https://github.com/lark-parser/lark): for parsing the chords in Harte.
 
 ## 🛠️ Installation
 
 The library is available on PyPi. To install, simply execute the following command:
 
 ```bash
@@ -93,15 +93,15 @@
 from harte.harte import Harte
 
 chord = Harte('D:(b3,5,7,9)')
 
 pretty_harte = chord.prettify()  # D:minmaj7(9)
 ```
 
-## 🤝 Contributing
+## 🤝 Contributing
 
 We welcome contributions from the community to enhance the Harte Library. Whether you want to report a bug, suggest a new feature, or contribute code, your help is greatly appreciated!
 
 ## 🐞 Reporting Issues
 
 If you encounter any bugs, have feature requests, or have suggestions for improvements, please open an [issue](https://github.com/andreamust/harte-library/issues) with detailed information about the problem or suggestion.
```

### Comparing `harte-library-0.4.4/README.md` & `harte_library-0.4.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 The **Harte Library** is an extension of the [music21 library](http://web.mit.edu/music21/) tailored for working with music chords encoded according to the [Harte Notation](https://ismir2005.ismir.net/proceedings/1080.pdf).
 
 This project is a component of [ChoCo](https://github.com/smashub/choco), a comprehensive dataset containing over 20,000 timed chord annotations sourced from integrated and standardized scores and tracks.
 
 The library has the following dependencies:
 
-- [music21](http://web.mit.edu/music21/): as an extension of the library itself;
+- [music21](http://web.mit.edu/music21/): the base library the *harte-library* extends;
 - [Lark](https://github.com/lark-parser/lark): for parsing the chords in Harte.
 
 ## 🛠️ Installation
 
 The library is available on PyPi. To install, simply execute the following command:
 
 ```bash
@@ -78,15 +78,15 @@
 from harte.harte import Harte
 
 chord = Harte('D:(b3,5,7,9)')
 
 pretty_harte = chord.prettify()  # D:minmaj7(9)
 ```
 
-## 🤝 Contributing
+## 🤝 Contributing
 
 We welcome contributions from the community to enhance the Harte Library. Whether you want to report a bug, suggest a new feature, or contribute code, your help is greatly appreciated!
 
 ## 🐞 Reporting Issues
 
 If you encounter any bugs, have feature requests, or have suggestions for improvements, please open an [issue](https://github.com/andreamust/harte-library/issues) with detailed information about the problem or suggestion.
```

### Comparing `harte-library-0.4.4/harte/harte.lark` & `harte_library-0.4.5/harte/harte.lark`

 * *Files identical despite different names*

### Comparing `harte-library-0.4.4/harte/harte.py` & `harte_library-0.4.5/harte/harte.py`

 * *Files identical despite different names*

### Comparing `harte-library-0.4.4/harte/interval.py` & `harte_library-0.4.5/harte/interval.py`

 * *Files identical despite different names*

### Comparing `harte-library-0.4.4/harte/mappings.py` & `harte_library-0.4.5/harte/mappings.py`

 * *Files identical despite different names*

### Comparing `harte-library-0.4.4/harte/parse_harte.py` & `harte_library-0.4.5/harte/parse_harte.py`

 * *Files identical despite different names*

### Comparing `harte-library-0.4.4/harte/utils.py` & `harte_library-0.4.5/harte/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Utility functions for processing Harte Chords
 """
 
 # pylint: disable=consider-iterating-dictionary
+# pylint: disable=too-many-branches
 
 import re
 from typing import List
 
 from harte.mappings import SHORTHAND_DEGREES
 
 
@@ -17,40 +18,44 @@
     :type harte_interval: str
     :return: the music21-shaped interval corresponding to the Harte interval
     format as a string
     :rtype: str
     """
     regex = r"([#]+)?([b]+)?(\d+)"
     matches = re.findall(regex, harte_interval)[0]
+    n_sharp, n_flat = len(matches[0]), len(matches[1])
 
     base_degree = int(matches[2]) if int(matches[2]) < 8 else int(matches[2]) - 7
 
     if base_degree in [1, 4, 5]:
-        if len(matches[0]) == 0 and len(matches[1]) == 0:
+        if n_sharp == 0 and n_flat == 0:
             modifier = "P"
-        elif len(matches[1]) == 1 and len(matches[0]) == 0:
+        elif n_sharp == 1 and n_flat == 0:
             modifier = "A"
-        elif len(matches[0]) == 1 and len(matches[1]) == 0:
+        elif n_sharp == 0 and n_flat == 1:
             modifier = "d"
-        elif len(matches[0]) >= 2 and len(matches[1]) == 0:
+        elif n_sharp == 2 and n_flat == 0:
             new_sharps = matches[0].replace("##", "")
             return convert_interval(f"{new_sharps}{base_degree + 1}")
-        elif len(matches[1]) >= 2 and len(matches[0]) == 0:
+        elif n_sharp == 0 and n_flat == 2:
             new_flats = matches[1].replace("bb", "")
+            if base_degree == 1:
+                base_degree = 8
+                new_flats += "b"
             return convert_interval(f"{new_flats}{base_degree - 1}")
         else:
-            raise ValueError(f"The degree {harte_interval} cannot " f"be parsed.")
+            raise ValueError(f"The degree {harte_interval} cannot be parsed.")
     else:
-        if len(matches[0]) == 0 and len(matches[1]) == 0:
+        if n_sharp == 0 and n_flat == 0:
             modifier = "M"
-        elif len(matches[0]) == 1 and len(matches[1]) == 0:
+        elif n_sharp == 1 and n_flat == 0:
             modifier = "A"
-        elif len(matches[1]) == 1 and len(matches[0]) == 0:
+        elif n_sharp == 0 and n_flat == 1:
             modifier = "m"
-        elif len(matches[1]) == 2 and len(matches[0]) == 0:
+        elif n_sharp == 0 and n_flat == 2:
             modifier = "d"
         else:
             raise ValueError(f"The degree {harte_interval} cannot " f"be parsed.")
 
     return modifier + str(base_degree)
```

### Comparing `harte-library-0.4.4/harte_library.egg-info/PKG-INFO` & `harte_library-0.4.5/harte_library.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harte-library
-Version: 0.4.4
+Version: 0.4.5
 Summary: Library for parsing Harte chords and converting them to Music21
 Author: Andrea Poltronieri
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -22,15 +22,15 @@
 
 The **Harte Library** is an extension of the [music21 library](http://web.mit.edu/music21/) tailored for working with music chords encoded according to the [Harte Notation](https://ismir2005.ismir.net/proceedings/1080.pdf).
 
 This project is a component of [ChoCo](https://github.com/smashub/choco), a comprehensive dataset containing over 20,000 timed chord annotations sourced from integrated and standardized scores and tracks.
 
 The library has the following dependencies:
 
-- [music21](http://web.mit.edu/music21/): as an extension of the library itself;
+- [music21](http://web.mit.edu/music21/): the base library the *harte-library* extends;
 - [Lark](https://github.com/lark-parser/lark): for parsing the chords in Harte.
 
 ## 🛠️ Installation
 
 The library is available on PyPi. To install, simply execute the following command:
 
 ```bash
@@ -93,15 +93,15 @@
 from harte.harte import Harte
 
 chord = Harte('D:(b3,5,7,9)')
 
 pretty_harte = chord.prettify()  # D:minmaj7(9)
 ```
 
-## 🤝 Contributing
+## 🤝 Contributing
 
 We welcome contributions from the community to enhance the Harte Library. Whether you want to report a bug, suggest a new feature, or contribute code, your help is greatly appreciated!
 
 ## 🐞 Reporting Issues
 
 If you encounter any bugs, have feature requests, or have suggestions for improvements, please open an [issue](https://github.com/andreamust/harte-library/issues) with detailed information about the problem or suggestion.
```

### Comparing `harte-library-0.4.4/setup.py` & `harte_library-0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="harte-library",
-    version="0.4.4",
+    version="0.4.5",
     author="Andrea Poltronieri",
     description="Library for parsing Harte chords and converting them to Music21",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `harte-library-0.4.4/test/test_harte.py` & `harte_library-0.4.5/test/test_harte.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,16 +49,16 @@
     the intervals from a chord.
 
     :param chord: Input chord
     :type chord: str
     :param intervals: Intervals that should be part of the chord
     :type intervals: List[str]
     """
-    chord = Harte(chord)
-    annotated_intervals = chord.annotateIntervals(
+    chord = Harte(chord)  # type: ignore
+    annotated_intervals = chord.annotateIntervals(  # type: ignore
         inPlace=False, returnList=True, stripSpecifiers=False
     )
     assert set(intervals) == set(annotated_intervals)
 
 
 @pytest.mark.parametrize(
     "chord,pitches",
@@ -74,9 +74,9 @@
     object.
 
     :param chord: Input chord
     :type chord: str
     :param pitches: Pitches that should be part of the chord
     :type pitches: List[str]
     """
-    chord = Harte(chord)
-    assert [p.name for p in chord.pitches] == pitches
+    chord = Harte(chord)  # type: ignore
+    assert [p.name for p in chord.pitches] == pitches  # type: ignore
```

