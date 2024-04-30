# Comparing `tmp/monisha-0.0.60.tar.gz` & `tmp/monisha-0.0.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monisha-0.0.60.tar", last modified: Tue Apr 30 06:23:29 2024, max compression
+gzip compressed data, was "monisha-0.0.62.tar", last modified: Tue Apr 30 19:32:08 2024, max compression
```

## Comparing `monisha-0.0.60.tar` & `monisha-0.0.62.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:29.563874 monisha-0.0.60/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-30 06:23:21.000000 monisha-0.0.60/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:29.555874 monisha-0.0.60/Monisha/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:29.559874 monisha-0.0.60/Monisha/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function01.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function02.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function03.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function04.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function05.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function06.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function07.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function08.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function09.py
--rw-r--r--   0 runner    (1001) docker     (127)    60105 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function10.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function11.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function12.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function13.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function14.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function15.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function16.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function17.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/functions/function18.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:29.559874 monisha-0.0.60/Monisha/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/scripts/en.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/scripts/eo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-30 06:23:21.000000 monisha-0.0.60/Monisha/scripts/es.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-30 06:23:29.563874 monisha-0.0.60/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-30 06:23:21.000000 monisha-0.0.60/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:29.559874 monisha-0.0.60/monisha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-30 06:23:29.000000 monisha-0.0.60/monisha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-30 06:23:29.000000 monisha-0.0.60/monisha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:23:29.000000 monisha-0.0.60/monisha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 06:23:29.000000 monisha-0.0.60/monisha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 06:23:29.000000 monisha-0.0.60/monisha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 06:23:29.563874 monisha-0.0.60/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-30 06:23:21.000000 monisha-0.0.60/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:32:08.005797 monisha-0.0.62/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-30 19:32:03.000000 monisha-0.0.62/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:32:08.001797 monisha-0.0.62/Monisha/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:32:08.005797 monisha-0.0.62/Monisha/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function02.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function04.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function06.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function07.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function08.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function09.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60666 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function14.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function15.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function17.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/functions/function18.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:32:08.005797 monisha-0.0.62/Monisha/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/scripts/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/scripts/eo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-30 19:32:03.000000 monisha-0.0.62/Monisha/scripts/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-30 19:32:08.005797 monisha-0.0.62/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-30 19:32:03.000000 monisha-0.0.62/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:32:08.005797 monisha-0.0.62/monisha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-30 19:32:07.000000 monisha-0.0.62/monisha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-30 19:32:07.000000 monisha-0.0.62/monisha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:32:07.000000 monisha-0.0.62/monisha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 19:32:07.000000 monisha-0.0.62/monisha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 19:32:07.000000 monisha-0.0.62/monisha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 19:32:08.005797 monisha-0.0.62/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-30 19:32:03.000000 monisha-0.0.62/setup.py
```

### Comparing `monisha-0.0.60/LICENSE` & `monisha-0.0.62/LICENSE`

 * *Files identical despite different names*

### Comparing `monisha-0.0.60/Monisha/__init__.py` & `monisha-0.0.62/Monisha/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 appname = "monisha"
-version = "0.0.60"
+version = "0.0.62"
 
 install = ["hachoir"]
 
 DATA01 = "clintonabrahamc@gmail.com"
 DATA02 = ['Natural Language :: English',
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
```

### Comparing `monisha-0.0.60/Monisha/functions/__init__.py` & `monisha-0.0.62/Monisha/functions/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .function04 import Eimes, Mimeo, Mimes
 from .function03 import progress, Progress
 from .function06 import Skeys, Uname
 from .function07 import Cmd, Wosd
 from .function18 import Metadatas
 from .function15 import Location
 from .function17 import Filename
+from .function09 import Storage
 from .function16 import FMagic
 from .function10 import Fonts
 from .function11 import con2s
 from .function12 import YKeys
 from .function05 import Doxo
-from .function09 import Sage
 from .function13 import Guid
 from .function08 import Num
```

### Comparing `monisha-0.0.60/Monisha/functions/function01.py` & `monisha-0.0.62/Monisha/functions/function01.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.60/Monisha/functions/function02.py` & `monisha-0.0.62/Monisha/functions/function02.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.60/Monisha/functions/function03.py` & `monisha-0.0.62/Monisha/functions/function03.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.60/Monisha/functions/function04.py` & `monisha-0.0.62/Monisha/functions/function04.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #============================================================================================================================
 
 class Eimes(object):
 
+    DATA00 = (".DMY", ".TMP")
+
     DATA01 = (".TXT", ".PDF", ".APK", ".EXE", ".ZIP", ".RAR", ".TAR", ".ISO")
 
     DATA02 = (".MKV", ".MP4", ".MOV", ".WMV", ".3GP", ".MPG", ".WEBM", ".AVI", ".FLV", ".M4V", ".GIF")
 
     DATA03 = (".MP3", ".M4A", ".M4B", ".FLAC", ".WAV", ".AIF", ".OGG", ".AAC", ".DTS", ".MID", ".AMR", ".MKA")
 
     DATA04 = (".JPG", ".JPX", ".PNG", ".WEBP", ".CR2", ".TIF", ".BMP", ".JXR", ".PSD", ".ICO", ".HEIC", ".JPEG")
```

### Comparing `monisha-0.0.60/Monisha/functions/function06.py` & `monisha-0.0.62/Monisha/functions/function06.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.60/Monisha/functions/function07.py` & `monisha-0.0.62/Monisha/functions/function07.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.60/Monisha/functions/function10.py` & `monisha-0.0.62/Monisha/functions/function10.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from ..scripts import Scripted
+#================================================================================
 
 class Fonts:
-    def FS01(text):
-        outgoing = text
-        return outgoing
+    def FS01(texted):
+        return texted
 
-    def FS02(text):
+    def FS02(texted):
         style = {
             'a': '𝚊',
             'b': '𝚋',
             'c': '𝚌',
             'd': '𝚍',
             'e': '𝚎',
             'f': '𝚏',
@@ -55,19 +56,18 @@
             'U': '𝚄',
             'V': '𝚅',
             'W': '𝚆',
             'X': '𝚇',
             'Y': '𝚈',
             'Z': '𝚉'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS03(text):
+    def FS03(texted):
         style = {
             'a': '𝕒',
             'b': '𝕓',
             'c': '𝕔',
             'd': '𝕕',
             'e': '𝕖',
             'f': '𝕗',
@@ -124,19 +124,18 @@
             '4': '𝟜',
             '5': '𝟝',
             '6': '𝟞',
             '7': '𝟟',
             '8': '𝟠',
             '9': '𝟡'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS04(text):
+    def FS04(texted):
         style = {
             'a': '𝐚',
             'b': '𝐛',
             'c': '𝐜',
             'd': '𝐝',
             'e': '𝐞',
             'f': '𝐟',
@@ -193,19 +192,18 @@
             '4': '𝟒',
             '5': '𝟓',
             '6': '𝟔',
             '7': '𝟕',
             '8': '𝟖',
             '9': '𝟗'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS05(text):
+    def FS05(texted):
         style = {
             'a': '𝒂',
             'b': '𝒃',
             'c': '𝒄',
             'd': '𝒅',
             'e': '𝒆',
             'f': '𝒇',
@@ -252,19 +250,18 @@
             'U': '𝑼',
             'V': '𝑽',
             'W': '𝑾',
             'X': '𝑿',
             'Y': '𝒀',
             'Z': '𝒁'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS06(text):
+    def FS06(texted):
         style = {
             'a': '𝑎',
             'b': '𝑏',
             'c': '𝑐',
             'd': '𝑑',
             'e': '𝑒',
             'f': '𝑓',
@@ -311,19 +308,18 @@
             'U': '𝑈',
             'V': '𝑉',
             'W': '𝑊',
             'X': '𝑋',
             'Y': '𝑌',
             'Z': '𝑍'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS07(text):
+    def FS07(texted):
         style = {
             'a': 'ᴀ',
             'b': 'ʙ',
             'c': 'ᴄ',
             'd': 'ᴅ',
             'e': 'ᴇ',
             'f': 'ғ',
@@ -380,19 +376,18 @@
             '4': '𝟺',
             '5': '𝟻',
             '6': '𝟼',
             '7': '𝟽',
             '8': '𝟾',
             '9': '𝟿'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS08(text):
+    def FS08(texted):
         style = {
             'a': '𝒶',
             'b': '𝒷',
             'c': '𝒸',
             'd': '𝒹',
             'e': 'ℯ',
             'f': '𝒻',
@@ -439,19 +434,18 @@
             'U': '𝒰',
             'V': '𝒱',
             'W': '𝒲',
             'X': '𝒳',
             'Y': '𝒴',
             'Z': '𝒵'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS09(text):
+    def FS09(texted):
         style = {
             'a': '𝓪',
             'b': '𝓫',
             'c': '𝓬',
             'd': '𝓭',
             'e': '𝓮',
             'f': '𝓯',
@@ -498,19 +492,18 @@
             'U': '𝓤',
             'V': '𝓥',
             'W': '𝓦',
             'X': '𝓧',
             'Y': '𝓨',
             'Z': '𝓩'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS10(text):
+    def FS10(texted):
         style = {
             'a': 'ᵃ',
             'b': 'ᵇ',
             'c': 'ᶜ',
             'd': 'ᵈ',
             'e': 'ᵉ',
             'f': 'ᶠ',
@@ -557,19 +550,18 @@
             'U': 'ᵘ',
             'V': 'ᵛ',
             'W': 'ʷ',
             'X': 'ˣ',
             'Y': 'ʸ',
             'Z': 'ᶻ'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS11(text):
+    def FS11(texted):
         style = {
             'a': 'ᗩ',
             'b': 'ᗷ',
             'c': 'ᑕ',
             'd': 'ᗪ',
             'e': 'ᗴ',
             'f': 'ᖴ',
@@ -616,19 +608,18 @@
             'U': 'ᑌ',
             'V': 'ᐯ',
             'W': 'ᗯ',
             'X': '᙭',
             'Y': 'Y',
             'Z': 'ᘔ'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS12(text):
+    def FS12(texted):
         style = {
             'a': '𝗮',
             'b': '𝗯',
             'c': '𝗰',
             'd': '𝗱',
             'e': '𝗲',
             'f': '𝗳',
@@ -685,19 +676,18 @@
             '4': '𝟰',
             '5': '𝟱',
             '6': '𝟲',
             '7': '𝟳',
             '8': '𝟴',
             '9': '𝟵'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS13(text):
+    def FS13(texted):
         style = {
             'a': '𝙖',
             'b': '𝙗',
             'c': '𝙘',
             'd': '𝙙',
             'e': '𝙚',
             'f': '𝙛',
@@ -744,19 +734,18 @@
             'U': '𝙐',
             'V': '𝙑',
             'W': '𝙒',
             'X': '𝙓',
             'Y': '𝙔',
             'Z': '𝙕'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS14(text):
+    def FS14(texted):
         style = {
             'a': '𝘢',
             'b': '𝘣',
             'c': '𝘤',
             'd': '𝘥',
             'e': '𝘦',
             'f': '𝘧',
@@ -803,19 +792,18 @@
             'U': '𝘜',
             'V': '𝘝',
             'W': '𝘞',
             'X': '𝘟',
             'Y': '𝘠',
             'Z': '𝘡'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS15(text):
+    def FS15(texted):
         style = {
             'a': '𝖺',
             'b': '𝖻',
             'c': '𝖼',
             'd': '𝖽',
             'e': '𝖾',
             'f': '𝖿',
@@ -862,19 +850,18 @@
             'U': '𝖴',
             'V': '𝖵',
             'W': '𝖶',
             'X': '𝖷',
             'Y': '𝖸',
             'Z': '𝖹'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS16(text):
+    def FS16(texted):
         style = {
             'a': 'Ⓐ︎',
             'b': 'Ⓑ︎',
             'c': 'Ⓒ︎',
             'd': 'Ⓓ︎',
             'e': 'Ⓔ︎',
             'f': 'Ⓕ︎',
@@ -931,19 +918,18 @@
             '4': '④',
             '5': '⑤',
             '6': '⑥',
             '7': '⑦',
             '8': '⑧',
             '9': '⑨'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS17(text):
+    def FS17(texted):
         style = {
             'a': '🅐︎',
             'b': '🅑︎',
             'c': '🅒︎',
             'd': '🅓︎',
             'e': '🅔︎',
             'f': '🅕︎',
@@ -1000,19 +986,18 @@
             '4': '➍',
             '5': '➎',
             '6': '➏',
             '7': '➐',
             '8': '➑',
             '9': '➒'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS18(text):
+    def FS18(texted):
         style = {
             'a': '𝔞',
             'b': '𝔟',
             'c': '𝔠',
             'd': '𝔡',
             'e': '𝔢',
             'f': '𝔣',
@@ -1059,20 +1044,18 @@
             'U': '𝔘',
             'V': '𝔙',
             'W': '𝔚',
             'X': '𝔛',
             'Y': '𝔜',
             'Z': 'ℨ'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-
-    def FS19(text):
+    def FS19(texted):
         style = {
             'a': '𝖆',
             'b': '𝖇',
             'c': '𝖈',
             'd': '𝖉',
             'e': '𝖊',
             'f': '𝖋',
@@ -1119,19 +1102,18 @@
             'U': '𝖀',
             'V': '𝖁',
             'W': '𝖂',
             'X': '𝖃',
             'Y': '𝖄',
             'Z': '𝖅'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS20(text):
+    def FS20(texted):
         style = {
             'a': 'a͜͡',
             'b': 'b͜͡',
             'c': 'c͜͡',
             'd': 'd͜͡',
             'e': 'e͜͡',
             'f': 'f͜͡',
@@ -1178,19 +1160,18 @@
             'U': 'U͜͡',
             'V': 'V͜͡',
             'W': 'W͜͡',
             'X': 'X͜͡',
             'Y': 'Y͜͡',
             'Z': 'Z͜͡'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS21(text):
+    def FS21(texted):
         style = {
             'a': 'ă̈',
             'b': 'b̆̈',
             'c': 'c̆̈',
             'd': 'd̆̈',
             'e': 'ĕ̈',
             'f': 'f̆̈',
@@ -1237,19 +1218,18 @@
             'U': 'Ŭ̈',
             'V': 'V̆̈',
             'W': 'W̆̈',
             'X': 'X̆̈',
             'Y': 'Y̆̈',
             'Z': 'Z̆̈'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS22(text):
+    def FS22(texted):
         style = {
             'a': 'ȃ̈',
             'b': 'b̑̈',
             'c': 'c̑̈',
             'd': 'd̑̈',
             'e': 'ȇ̈',
             'f': 'f̑̈',
@@ -1296,19 +1276,18 @@
             'U': 'Ȗ̈',
             'V': 'V̑̈',
             'W': 'W̑̈',
             'X': 'X̑̈',
             'Y': 'Y̑̈',
             'Z': 'Z̑̈'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS23(text):
+    def FS23(texted):
         style = {
             'a': '🇦 ',
             'b': '🇧 ',
             'c': '🇨 ',
             'd': '🇩 ',
             'e': '🇪 ',
             'f': '🇫 ',
@@ -1355,19 +1334,18 @@
             'U': '🇺 ',
             'V': '🇻 ',
             'W': '🇼 ',
             'X': '🇽 ',
             'Y': '🇾 ',
             'Z': '🇿 '
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS24(text):
+    def FS24(texted):
         style = {
             'a': '🄰',
             'b': '🄱',
             'c': '🄲',
             'd': '🄳',
             'e': '🄴',
             'f': '🄵',
@@ -1414,19 +1392,18 @@
             'U': '🅄',
             'V': '🅅',
             'W': '🅆',
             'X': '🅇',
             'Y': '🅈',
             'Z': '🅉'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS25(text):
+    def FS25(texted):
         style = {
             'a': '🅰︎',
             'b': '🅱︎',
             'c': '🅲︎',
             'd': '🅳︎',
             'e': '🅴︎',
             'f': '🅵︎',
@@ -1473,19 +1450,18 @@
             'U': '🆄︎',
             'V': '🆅︎',
             'W': '🆆︎',
             'X': '🆇︎',
             'Y': '🆈︎',
             'Z': '🆉︎'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS26(text):
+    def FS26(texted):
         style = {
             'a': 'ꪖ',
             'b': '᥇',
             'c': 'ᥴ',
             'd': 'ᦔ',
             'e': 'ꫀ',
             'f': 'ᠻ',
@@ -1532,19 +1508,18 @@
             'U': 'ꪊ',
             'V': 'ꪜ',
             'W': '᭙',
             'X': '᥊',
             'Y': 'ꪗ',
             'Z': 'ɀ'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS27(text):
+    def FS27(texted):
         style = {
             'a': '卂',
             'b': '乃',
             'c': '匚',
             'd': 'ᗪ',
             'e': '乇',
             'f': '千',
@@ -1591,19 +1566,18 @@
             'U': 'ㄩ',
             'V': 'ᐯ',
             'W': '山',
             'X': '乂',
             'Y': 'ㄚ',
             'Z': '乙'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS28(text):
+    def FS28(texted):
         style = {
             'a': 'a̾',
             'b': 'b̾',
             'c': 'c̾',
             'd': 'd̾',
             'e': 'e̾',
             'f': 'f̾',
@@ -1650,19 +1624,18 @@
             'U': 'U̾',
             'V': 'V̾',
             'W': 'W̾',
             'X': 'X̾',
             'Y': 'Y̾',
             'Z': 'Z̾'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS29(text):
+    def FS29(texted):
         style = {
             'a': 'ḁͦ',
             'b': 'b̥ͦ',
             'c': 'c̥ͦ',
             'd': 'd̥ͦ',
             'e': 'e̥ͦ',
             'f': 'f̥ͦ',
@@ -1709,19 +1682,18 @@
             'U': 'U̥ͦ',
             'V': 'V̥ͦ',
             'W': 'W̥ͦ',
             'X': 'X̥ͦ',
             'Y': 'Y̥ͦ',
             'Z': 'Z̥ͦ'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS30(text):
+    def FS30(texted):
         style = {
             'a': 'a͟',
             'b': 'b͟',
             'c': 'c͟',
             'd': 'd͟',
             'e': 'e͟',
             'f': 'f͟',
@@ -1768,19 +1740,18 @@
             'U': 'U͟',
             'V': 'V͟',
             'W': 'W͟',
             'X': 'X͟',
             'Y': 'Y͟',
             'Z': 'Z͟'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS31(text):
+    def FS31(texted):
         style = {
             'a': 'ꍏ',
             'b': 'ꌃ',
             'c': 'ꏳ',
             'd': 'ꀷ',
             'e': 'ꏂ',
             'f': 'ꎇ',
@@ -1827,19 +1798,18 @@
             'U': 'ꀎ',
             'V': '꒦',
             'W': 'ꅐ',
             'X': 'ꉧ',
             'Y': 'ꌩ',
             'Z': 'ꁴ'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS32(text):
+    def FS32(texted):
         style = {
             'a': 'a҉',
             'b': 'b҉',
             'c': 'c҉',
             'd': 'd҉',
             'e': 'e҉',
             'f': 'f҉',
@@ -1886,19 +1856,18 @@
             'U': 'U҉',
             'V': 'V҉',
             'W': 'W҉',
             'X': 'X҉',
             'Y': 'Y҉',
             'Z': 'Z҉'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS33(text):
+    def FS33(texted):
         style = {
             'a': 'a҈',
             'b': 'b҈',
             'c': 'c҈',
             'd': 'd҈',
             'e': 'e҈',
             'f': 'f҈',
@@ -1945,19 +1914,18 @@
             'U': 'U҈',
             'V': 'V҈',
             'W': 'W҈',
             'X': 'X҈',
             'Y': 'Y҈',
             'Z': 'Z҈'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS34(text):
+    def FS34(texted):
         style = {
             'a': 'a̸',
             'b': 'b̸',
             'c': 'c̸',
             'd': 'd̸',
             'e': 'e̸',
             'f': 'f̸',
@@ -2004,19 +1972,18 @@
             'U': 'U̸',
             'V': 'V̸',
             'W': 'W̸',
             'X': 'X̸',
             'Y': 'Y̸',
             'Z': 'Z̸'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS35(text):
+    def FS35(texted):
         style = {
             'a': 'a⃠',
             'b': 'b⃠',
             'c': 'c⃠',
             'd': 'd⃠',
             'e': 'e⃠',
             'f': 'f⃠',
@@ -2063,19 +2030,18 @@
             'U': 'U⃠',
             'V': 'V⃠',
             'W': 'W⃠',
             'X': 'X⃠',
             'Y': 'Y⃠',
             'Z': 'Z⃠'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS36(text):
+    def FS36(texted):
         style = {
             'a': 'a̺͆',
             'b': 'b̺͆',
             'c': 'c̺͆',
             'd': 'd̺͆',
             'e': 'e̺͆',
             'f': 'f̺͆',
@@ -2122,19 +2088,18 @@
             'U': 'U̺͆',
             'V': 'V̺͆',
             'W': 'W̺͆',
             'X': 'X̺͆',
             'Y': 'Y̺͆',
             'Z': 'Z̺͆'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS37(text):
+    def FS37(texted):
         style = {
             'a': 'a͎',
             'b': 'b͎',
             'c': 'c͎',
             'd': 'd͎',
             'e': 'e͎',
             'f': 'f͎',
@@ -2181,19 +2146,18 @@
             'U': 'U͎',
             'V': 'V͎',
             'W': 'W͎',
             'X': 'X͎',
             'Y': 'Y͎',
             'Z': 'Z͎'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS38(text):
+    def FS38(texted):
         style = {
             'a': 'ል',
             'b': 'ጌ',
             'c': 'ር',
             'd': 'ዕ',
             'e': 'ቿ',
             'f': 'ቻ',
@@ -2240,19 +2204,18 @@
             'U': 'ሁ',
             'V': 'ሀ',
             'W': 'ሠ',
             'X': 'ሸ',
             'Y': 'ሃ',
             'Z': 'ጊ'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS39(text):
+    def FS39(texted):
         style = {
             'a': 'a̶',
             'b': 'b̶',
             'c': 'c̶',
             'd': 'd̶',
             'e': 'e̶',
             'f': 'f̶',
@@ -2299,19 +2262,18 @@
             'U': 'U̶',
             'V': 'V̶',
             'W': 'W̶',
             'X': 'X̶',
             'Y': 'Y̶',
             'Z': 'Z̶'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
-    def FS40(text):
+    def FS40(texted):
         style = {
             'a': 'a༙',
             'b': 'b༙',
             'c': 'c༙',
             'd': 'd༙',
             'e': 'e༙',
             'f': 'f༙',
@@ -2358,11 +2320,11 @@
             'U': 'U༙',
             'V': 'V༙',
             'W': 'W༙',
             'X': 'X༙',
             'Y': 'Y༙',
             'Z': 'Z༙'
         }
-        for i, o in style.items():
-            text = text.replace(i, o)
-        return text
+        texted = Scripted.DATA01.join(style.get(chao, chao) for chao in texted)
+        return texted
 
+#================================================================================
```

### Comparing `monisha-0.0.60/Monisha/functions/function14.py` & `monisha-0.0.62/Monisha/functions/function14.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.60/Monisha/functions/function15.py` & `monisha-0.0.62/Monisha/functions/function15.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 import os
+from .function04 import Eimes
+from .function09 import Storage
 #=================================================================================================
 
 class Messages:
     def __init__(self, **kwargs):
+        self.numfiles = kwargs.get('numfiles', 0)
         self.filesize = kwargs.get('filesize', 0)
+        self.allfiles = kwargs.get('allfiles', [])
         self.location = kwargs.get('location', None)
 
 #=================================================================================================
 
 class Location:
 
-    async def get00(dlocation, files=[]):
+    async def get00(dlocation, skip=Eimes.DATA00, files=[]):
         for patho in sorted(os.listdir(dlocation)):
             filez = os.path.join(dlocation, patho)
-            files.append(filez)
+            if filez.upper().endswith(skip):
+                continue
+            else:
+                files.append(filez)
 
-        return files
+        return Messages(allfiles=files, numfiles=len(files))
 
 #=================================================================================================
 
     async def get01(flocation, exo):
         try:
             location = str(flocation)
             filesize = int(os.path.getsize(location))
```

### Comparing `monisha-0.0.60/Monisha/functions/function16.py` & `monisha-0.0.62/Monisha/functions/function16.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.60/Monisha/functions/function17.py` & `monisha-0.0.62/Monisha/functions/function17.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.60/Monisha/functions/function18.py` & `monisha-0.0.62/Monisha/functions/function18.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.60/Monisha/scripts/es.py` & `monisha-0.0.62/Monisha/scripts/es.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.60/PKG-INFO` & `monisha-0.0.62/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.60
+Version: 0.0.62
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.60 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.62 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
```

### Comparing `monisha-0.0.60/monisha.egg-info/PKG-INFO` & `monisha-0.0.62/monisha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.60
+Version: 0.0.62
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.60 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.62 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
```

### Comparing `monisha-0.0.60/monisha.egg-info/SOURCES.txt` & `monisha-0.0.62/monisha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monisha-0.0.60/setup.py` & `monisha-0.0.62/setup.py`

 * *Files identical despite different names*

