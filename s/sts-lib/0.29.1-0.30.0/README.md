# Comparing `tmp/sts_lib-0.29.1.tar.gz` & `tmp/sts_lib-0.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sts_lib-0.29.1.tar", last modified: Fri Apr 26 12:43:40 2024, max compression
+gzip compressed data, was "sts_lib-0.30.0.tar", last modified: Tue Apr 30 13:22:29 2024, max compression
```

## Comparing `sts_lib-0.29.1.tar` & `sts_lib-0.30.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 12:43:40.066478 sts_lib-0.29.1/
--rw-rw-rw-   0        0        0    11358 2024-04-19 09:05:26.000000 sts_lib-0.29.1/LICENSE
--rw-rw-rw-   0        0        0       13 2024-04-19 09:05:26.000000 sts_lib-0.29.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6916 2024-04-26 12:43:40.066478 sts_lib-0.29.1/PKG-INFO
--rw-rw-rw-   0        0        0     5463 2024-04-26 12:29:18.000000 sts_lib-0.29.1/README.md
--rw-rw-rw-   0        0        0     1728 2024-04-26 12:43:40.068475 sts_lib-0.29.1/setup.cfg
--rw-rw-rw-   0        0        0       65 2024-04-19 09:05:26.000000 sts_lib-0.29.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-26 12:43:39.999503 sts_lib-0.29.1/sts/
--rw-rw-rw-   0        0        0    52455 2024-04-26 12:41:58.000000 sts_lib-0.29.1/sts/__init__.py
--rw-rw-rw-   0        0        0       89 2024-04-19 09:05:26.000000 sts_lib-0.29.1/sts/__main__.py
--rw-rw-rw-   0        0        0     7551 2024-04-23 13:05:20.000000 sts_lib-0.29.1/sts/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-26 12:43:40.013530 sts_lib-0.29.1/sts/data/
-drwxrwxrwx   0        0        0        0 2024-04-26 12:43:40.029518 sts_lib-0.29.1/sts/data/config/
--rw-rw-rw-   0        0        0      915 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/config/_default.json
--rw-rw-rw-   0        0        0      608 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/config/hk2s.json
--rw-rw-rw-   0        0        0      346 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/config/hk2t.json
--rw-rw-rw-   0        0        0      410 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/config/jp2t.json
--rw-rw-rw-   0        0        0      419 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/config/s2hk.json
--rw-rw-rw-   0        0        0      267 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/config/s2t.json
--rw-rw-rw-   0        0        0      417 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/config/s2tw.json
--rw-rw-rw-   0        0        0      608 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/config/s2twp.json
--rw-rw-rw-   0        0        0      247 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/config/t2hk.json
--rw-rw-rw-   0        0        0      261 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/config/t2jp.json
--rw-rw-rw-   0        0        0      267 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/config/t2s.json
--rw-rw-rw-   0        0        0      245 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/config/t2tw.json
--rw-rw-rw-   0        0        0      606 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/config/tw2s.json
--rw-rw-rw-   0        0        0      670 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/config/tw2sp.json
--rw-rw-rw-   0        0        0      344 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/config/tw2t.json
-drwxrwxrwx   0        0        0        0 2024-04-26 12:43:40.052494 sts_lib-0.29.1/sts/data/dictionary/
--rw-rw-rw-   0        0        0      595 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/dictionary/HKVariants.txt
--rw-rw-rw-   0        0        0     2865 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/dictionary/HKVariantsRevPhrases.txt
--rw-rw-rw-   0        0        0      103 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/dictionary/JPShinjitaiCharacters.txt
--rw-rw-rw-   0        0        0     2720 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/dictionary/JPShinjitaiPhrases.txt
--rw-rw-rw-   0        0        0     3307 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/dictionary/JPVariants.txt
--rw-rw-rw-   0        0        0    38333 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/dictionary/STCharacters.txt
--rw-rw-rw-   0        0        0  1053351 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/dictionary/STPhrases.txt
--rw-rw-rw-   0        0        0    38740 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/dictionary/TSCharacters.txt
--rw-rw-rw-   0        0        0     5438 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/dictionary/TSPhrases.txt
--rw-rw-rw-   0        0        0     8014 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/dictionary/TWPhrasesIT.txt
--rw-rw-rw-   0        0        0     2205 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/dictionary/TWPhrasesName.txt
--rw-rw-rw-   0        0        0      608 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/dictionary/TWPhrasesOther.txt
--rw-rw-rw-   0        0        0      351 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/dictionary/TWVariants.txt
--rw-rw-rw-   0        0        0     1143 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/dictionary/TWVariantsRevPhrases.txt
--rw-rw-rw-   0        0        0    22760 2024-04-26 12:35:06.000000 sts_lib-0.29.1/sts/data/htmlpage.tpl.html
-drwxrwxrwx   0        0        0        0 2024-04-26 12:43:40.055489 sts_lib-0.29.1/sts/data/scheme/
--rw-rw-rw-   0        0        0    21633 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/scheme/st_multi.txt
--rw-rw-rw-   0        0        0      436 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/scheme/ts_multi.txt
--rw-rw-rw-   0        0        0     2108 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/scheme/variant.txt
-drwxrwxrwx   0        0        0        0 2024-04-26 12:43:40.063481 sts_lib-0.29.1/sts_lib.egg-info/
--rw-rw-rw-   0        0        0     6916 2024-04-26 12:43:39.000000 sts_lib-0.29.1/sts_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1325 2024-04-26 12:43:39.000000 sts_lib-0.29.1/sts_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 12:43:39.000000 sts_lib-0.29.1/sts_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-04-26 12:43:39.000000 sts_lib-0.29.1/sts_lib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      202 2024-04-26 12:43:39.000000 sts_lib-0.29.1/sts_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-26 12:43:39.000000 sts_lib-0.29.1/sts_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 13:22:29.275998 sts_lib-0.30.0/
+-rw-rw-rw-   0        0        0    11358 2024-04-19 09:05:26.000000 sts_lib-0.30.0/LICENSE
+-rw-rw-rw-   0        0        0       13 2024-04-19 09:05:26.000000 sts_lib-0.30.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6916 2024-04-30 13:22:29.275998 sts_lib-0.30.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5463 2024-04-29 19:01:51.000000 sts_lib-0.30.0/README.md
+-rw-rw-rw-   0        0        0     1728 2024-04-30 13:22:29.277996 sts_lib-0.30.0/setup.cfg
+-rw-rw-rw-   0        0        0       65 2024-04-19 09:05:26.000000 sts_lib-0.30.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 13:22:29.234227 sts_lib-0.30.0/sts/
+-rw-rw-rw-   0        0        0    52950 2024-04-30 13:22:07.000000 sts_lib-0.30.0/sts/__init__.py
+-rw-rw-rw-   0        0        0       89 2024-04-19 09:05:26.000000 sts_lib-0.30.0/sts/__main__.py
+-rw-rw-rw-   0        0        0     7551 2024-04-30 13:21:35.000000 sts_lib-0.30.0/sts/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-30 13:22:29.235226 sts_lib-0.30.0/sts/data/
+drwxrwxrwx   0        0        0        0 2024-04-30 13:22:29.247209 sts_lib-0.30.0/sts/data/config/
+-rw-rw-rw-   0        0        0      915 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/config/_default.json
+-rw-rw-rw-   0        0        0      608 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/config/hk2s.json
+-rw-rw-rw-   0        0        0      346 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/config/hk2t.json
+-rw-rw-rw-   0        0        0      410 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/config/jp2t.json
+-rw-rw-rw-   0        0        0      419 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/config/s2hk.json
+-rw-rw-rw-   0        0        0      267 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/config/s2t.json
+-rw-rw-rw-   0        0        0      417 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/config/s2tw.json
+-rw-rw-rw-   0        0        0      607 2024-04-30 13:22:07.000000 sts_lib-0.30.0/sts/data/config/s2twp.json
+-rw-rw-rw-   0        0        0      247 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/config/t2hk.json
+-rw-rw-rw-   0        0        0      261 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/config/t2jp.json
+-rw-rw-rw-   0        0        0      267 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/config/t2s.json
+-rw-rw-rw-   0        0        0      245 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/config/t2tw.json
+-rw-rw-rw-   0        0        0      606 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/config/tw2s.json
+-rw-rw-rw-   0        0        0      670 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/config/tw2sp.json
+-rw-rw-rw-   0        0        0      344 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/config/tw2t.json
+drwxrwxrwx   0        0        0        0 2024-04-30 13:22:29.263198 sts_lib-0.30.0/sts/data/dictionary/
+-rw-rw-rw-   0        0        0      595 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/dictionary/HKVariants.txt
+-rw-rw-rw-   0        0        0     2865 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/dictionary/HKVariantsRevPhrases.txt
+-rw-rw-rw-   0        0        0      103 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/dictionary/JPShinjitaiCharacters.txt
+-rw-rw-rw-   0        0        0     2720 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/dictionary/JPShinjitaiPhrases.txt
+-rw-rw-rw-   0        0        0     3307 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/dictionary/JPVariants.txt
+-rw-rw-rw-   0        0        0    38333 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/dictionary/STCharacters.txt
+-rw-rw-rw-   0        0        0  1053351 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/dictionary/STPhrases.txt
+-rw-rw-rw-   0        0        0    38740 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/dictionary/TSCharacters.txt
+-rw-rw-rw-   0        0        0     5438 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/dictionary/TSPhrases.txt
+-rw-rw-rw-   0        0        0     8014 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/dictionary/TWPhrasesIT.txt
+-rw-rw-rw-   0        0        0     2205 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/dictionary/TWPhrasesName.txt
+-rw-rw-rw-   0        0        0      608 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/dictionary/TWPhrasesOther.txt
+-rw-rw-rw-   0        0        0      351 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/dictionary/TWVariants.txt
+-rw-rw-rw-   0        0        0     1143 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/dictionary/TWVariantsRevPhrases.txt
+-rw-rw-rw-   0        0        0    22625 2024-04-30 13:22:07.000000 sts_lib-0.30.0/sts/data/htmlpage.tpl.html
+drwxrwxrwx   0        0        0        0 2024-04-30 13:22:29.266180 sts_lib-0.30.0/sts/data/scheme/
+-rw-rw-rw-   0        0        0    21633 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/scheme/st_multi.txt
+-rw-rw-rw-   0        0        0      436 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/scheme/ts_multi.txt
+-rw-rw-rw-   0        0        0     2108 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/scheme/variant.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 13:22:29.273998 sts_lib-0.30.0/sts_lib.egg-info/
+-rw-rw-rw-   0        0        0     6916 2024-04-30 13:22:29.000000 sts_lib-0.30.0/sts_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1325 2024-04-30 13:22:29.000000 sts_lib-0.30.0/sts_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 13:22:29.000000 sts_lib-0.30.0/sts_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-30 13:22:29.000000 sts_lib-0.30.0/sts_lib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      202 2024-04-30 13:22:29.000000 sts_lib-0.30.0/sts_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-30 13:22:29.000000 sts_lib-0.30.0/sts_lib.egg-info/top_level.txt
```

### Comparing `sts_lib-0.29.1/LICENSE` & `sts_lib-0.30.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.1/PKG-INFO` & `sts_lib-0.30.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-lib
-Version: 0.29.1
+Version: 0.30.0
 Summary: An open library for flexible simplified-traditional Chinese text conversion.
 Home-page: https://github.com/danny0838/sts-lib
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
```

### Comparing `sts_lib-0.29.1/README.md` & `sts_lib-0.30.0/README.md`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.1/setup.cfg` & `sts_lib-0.30.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.1/sts/__init__.py` & `sts_lib-0.30.0/sts/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,18 +44,19 @@
         @_lazyprop.setter
         def _lazyprop(self, value):
             setattr(self, attr_name, value)
 
         return _lazyprop
 
 
-__version__ = '0.29.1'
+__version__ = '0.30.0'
 
 StsDictMatch = namedtuple('StsDictMatch', ['conv', 'start', 'end'])
 StsDictConv = namedtuple('StsDictConv', ['key', 'values'])
+StsConvExclude = namedtuple('StsConvExclude', ['text'])
 
 
 class StreamList(list):
     """Convert an iterable into a serializable "list".
 
     This turns an iterable into an iterator that can be serialized as a JSON
     Array incrementally (i.e. without read into the memory as a whole).
@@ -575,18 +576,20 @@
         i = max(len(Unicode.split(key)) for key in self._dict)
         i = min(i, min(len(parts), maxpos) - pos)
         while i >= 1:
             end = pos + i
             current_parts = parts[pos:end]
             current = ''.join(current_parts)
             try:
-                conv = StsDictConv(current_parts, self._dict[current])
-            except KeyError:
+                match = self._dict[current]
+                assert match
+            except (KeyError, AssertionError):
                 pass
             else:
+                conv = StsDictConv(current_parts, match)
                 return StsDictMatch(conv, pos, end)
             i -= 1
         return None
 
     def apply(self, parts):
         """Convert text using the dictionary.
 
@@ -753,18 +756,20 @@
             i = self.key_head_length - 1
         i = min(i, min(len(parts), maxpos) - pos)
         while i >= 1:
             end = pos + i
             current_parts = parts[pos:end]
             current = ''.join(current_parts)
             try:
-                conv = StsDictConv(current_parts, self._dict[current])
-            except KeyError:
+                match = self._dict[current]
+                assert match
+            except (KeyError, AssertionError):
                 pass
             else:
+                conv = StsDictConv(current_parts, match)
                 return StsDictMatch(conv, pos, end)
             i -= 1
         return None
 
 
 class Trie(StsDict):
     """An STS dictionary with trie (prefix tree) format.
@@ -1425,15 +1430,15 @@
             for k, v in m.groupdict().items():
                 if self.exclude_return_group_pattern.search(k) and v is not None:
                     t = v
                     break
             else:
                 t = m.group(0)
             if t:
-                yield t
+                yield StsConvExclude(text=t)
 
             index = end
 
         t = text[index:]
         if t:
             yield from self.table.apply(t)
 
@@ -1445,35 +1450,41 @@
         formatter = getattr(self, f'_convert_formatted_{format}')
         yield from formatter(conv)
 
     def _convert_formatted_txt(self, parts):
         for part in parts:
             if isinstance(part, str):
                 yield part
+            elif isinstance(part, StsConvExclude):
+                yield part.text
             else:
-                yield part[1][0]
+                yield part.values[0]
 
     def _convert_formatted_txtm(self, parts, start='{{', end='}}', sep='->', vsep='|'):
         for part in parts:
             if isinstance(part, str):
                 yield part
+            elif isinstance(part, StsConvExclude):
+                yield part.text
             else:
                 olds, news = part
                 old = ''.join(olds)
 
                 if len(news) == 1 and old == news[0]:
                     yield f'{start}{old}{end}'
                 else:
                     new = vsep.join(news)
                     yield f'{start}{old}{sep}{new}{end}'
 
     def _convert_formatted_html(self, parts):
         for part in parts:
             if isinstance(part, str):
                 yield html.escape(part)
+            elif isinstance(part, StsConvExclude):
+                yield part.text
             else:
                 olds, news = part
                 old = ''.join(olds)
                 content = f'<del hidden>{html.escape(old)}</del>'
                 for i, v in enumerate(news):
                     hidden = '' if i == 0 else ' hidden'
                     content += f'<ins{hidden}>{html.escape(v)}</ins>'
```

### Comparing `sts_lib-0.29.1/sts/cli.py` & `sts_lib-0.30.0/sts/cli.py`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.1/sts/data/config/_default.json` & `sts_lib-0.30.0/sts/data/config/_default.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.1/sts/data/config/hk2s.json` & `sts_lib-0.30.0/sts/data/config/hk2s.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.1/sts/data/config/s2twp.json` & `sts_lib-0.30.0/sts/data/config/s2twp.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 00000160: 2022 2e2e 2f64 6963 7469 6f6e 6172 792f   "../dictionary/
 00000170: 5354 4368 6172 6163 7465 7273 2e74 7874  STCharacters.txt
 00000180: 220d 0a20 2020 2020 2020 2020 205d 0d0a  "..          ]..
 00000190: 2020 2020 2020 2020 7d2c 0d0a 2020 2020          },..    
 000001a0: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
 000001b0: 2022 6d6f 6465 223a 2022 6c6f 6164 222c   "mode": "load",
 000001c0: 0d0a 2020 2020 2020 2020 2020 2273 7263  ..          "src
-000001d0: 223a 205b 200d 0a20 2020 2020 2020 2020  ": [ ..         
-000001e0: 2020 2022 2e2e 2f64 6963 7469 6f6e 6172     "../dictionar
-000001f0: 792f 5457 5068 7261 7365 732e 6c69 7374  y/TWPhrases.list
-00000200: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00000210: 222e 2e2f 6469 6374 696f 6e61 7279 2f54  "../dictionary/T
-00000220: 5756 6172 6961 6e74 732e 7478 7422 0d0a  WVariants.txt"..
-00000230: 2020 2020 2020 2020 2020 5d0d 0a20 2020            ]..   
-00000240: 2020 2020 207d 0d0a 2020 2020 2020 5d0d       }..      ].
-00000250: 0a20 2020 207d 0d0a 2020 5d0d 0a7d 0d0a  .    }..  ]..}..
+000001d0: 223a 205b 0d0a 2020 2020 2020 2020 2020  ": [..          
+000001e0: 2020 222e 2e2f 6469 6374 696f 6e61 7279    "../dictionary
+000001f0: 2f54 5750 6872 6173 6573 2e6c 6973 7422  /TWPhrases.list"
+00000200: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+00000210: 2e2e 2f64 6963 7469 6f6e 6172 792f 5457  ../dictionary/TW
+00000220: 5661 7269 616e 7473 2e74 7874 220d 0a20  Variants.txt".. 
+00000230: 2020 2020 2020 2020 205d 0d0a 2020 2020           ]..    
+00000240: 2020 2020 7d0d 0a20 2020 2020 205d 0d0a      }..      ]..
+00000250: 2020 2020 7d0d 0a20 205d 0d0a 7d0d 0a        }..  ]..}..
```

### Comparing `sts_lib-0.29.1/sts/data/config/tw2s.json` & `sts_lib-0.30.0/sts/data/config/tw2s.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.1/sts/data/config/tw2sp.json` & `sts_lib-0.30.0/sts/data/config/tw2sp.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.1/sts/data/dictionary/HKVariants.txt` & `sts_lib-0.30.0/sts/data/dictionary/HKVariants.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.1/sts/data/dictionary/HKVariantsRevPhrases.txt` & `sts_lib-0.30.0/sts/data/dictionary/HKVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.1/sts/data/dictionary/JPShinjitaiPhrases.txt` & `sts_lib-0.30.0/sts/data/dictionary/JPShinjitaiPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.1/sts/data/dictionary/JPVariants.txt` & `sts_lib-0.30.0/sts/data/dictionary/JPVariants.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.1/sts/data/dictionary/STCharacters.txt` & `sts_lib-0.30.0/sts/data/dictionary/STCharacters.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.1/sts/data/dictionary/STPhrases.txt` & `sts_lib-0.30.0/sts/data/dictionary/STPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.1/sts/data/dictionary/TSCharacters.txt` & `sts_lib-0.30.0/sts/data/dictionary/TSCharacters.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.1/sts/data/dictionary/TSPhrases.txt` & `sts_lib-0.30.0/sts/data/dictionary/TSPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.1/sts/data/dictionary/TWPhrasesIT.txt` & `sts_lib-0.30.0/sts/data/dictionary/TWPhrasesIT.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.1/sts/data/dictionary/TWPhrasesName.txt` & `sts_lib-0.30.0/sts/data/dictionary/TWPhrasesName.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.1/sts/data/dictionary/TWPhrasesOther.txt` & `sts_lib-0.30.0/sts/data/dictionary/TWPhrasesOther.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.1/sts/data/dictionary/TWVariantsRevPhrases.txt` & `sts_lib-0.30.0/sts/data/dictionary/TWVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.1/sts/data/htmlpage.tpl.html` & `sts_lib-0.30.0/sts/data/htmlpage.tpl.html`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 dialog header { margin-bottom: .5em; font-weight: bold; }
 dialog section { margin: .5em 0; }
 dialog section label { display: block; }
 dialog footer { margin-top: 1em; display: flex; gap: .5em 1em; flex-direction: row; flex-wrap: wrap; }
 dialog footer input { flex-grow: 1; }
 body > footer { margin-top: 1em; text-align: center; font-size: small; }
 #viewer { border: thin ridge #0066CC; padding: 0.5em; background-color: #f8f8ee; white-space: pre-wrap; }
-#viewer a { border: thin dotted #AAA; color: unset; text-decoration: none; }
+#viewer a[tabindex] { border: thin dotted #AAA; }
 #viewer a:focus { outline: medium solid blue; }
 #viewer a.single, .single { background-color: #DDDDDD; }  /* 單選字 */
 #viewer a.changed, .changed { background-color: #DDDDFF; }  /* 異動字 */
 #viewer a.unchecked, .unchecked { background-color: #FFFF99; }  /* 未審字 */
 #viewer a.checked, .checked { background-color: #CCFFFF; }  /* 已審字 */
 #viewer a.picked, .picked { background-color: #CCFFCC; }  /* 選定字 */
 #viewer a.editing, .editing { background-color: #FFDDDD; }  /* 編輯中 */
@@ -41,47 +41,47 @@
 .popup a:not([tabindex="0"])::before { content: attr(tabindex) "."; }
 </style>
 <script>
 function* walkThroughAnchors(anchor, direction) {
   let a = anchor;
   if (direction > 0) {
     while (a = a.nextElementSibling) {
-      if (a === anchor) { return; }
       yield a;
     }
     if (a = anchor.parentNode.firstElementChild) {
-      if (a === anchor) { return; }
       yield a;
       while (a = a.nextElementSibling) {
-        if (a === anchor) { return; }
         yield a;
       }
     }
     return;
   }
   if (direction < 0) {
     while (a = a.previousElementSibling) {
-      if (a === anchor) { return; }
       yield a;
     }
     if (a = anchor.parentNode.lastElementChild) {
-      if (a === anchor) { return; }
       yield a;
       while (a = a.previousElementSibling) {
-        if (a === anchor) { return; }
         yield a;
       }
     }
     return;
   }
 }
 
 function moveAnchor(anchor, offset, filter) {
   let i = Math.abs(offset);
   for (const a of walkThroughAnchors(anchor, offset)) {
+    if (a === anchor) {
+      break;
+    }
+    if (!a.matches('a[tabindex]')) {
+      continue;
+    }
     if (typeof filter !== "function" || filter(a)) {
       if (i > 1) {
         i--;
         continue;
       }
       return a;
     }
@@ -345,15 +345,15 @@
       const candCur = anchor.querySelector('ins:not([hidden])');
       const candIdx = Array.prototype.indexOf.call(cands, candCur);
       return a => setCandidate(a, candIdx);
     }
   })();
 
   const viewer = document.querySelector('#viewer');
-  const anchors = viewer.querySelectorAll('a:not(.unmatched)');
+  const anchors = viewer.querySelectorAll('a[tabindex]:not(.unmatched)');
   const charCur = anchor.querySelector('del').textContent;
 
   func(anchor);
 
   let start, end;
   if (["applyBackwardUnchecked", "applyBackward"].includes(mode)) {
     start = 0;
```

### Comparing `sts_lib-0.29.1/sts/data/scheme/st_multi.txt` & `sts_lib-0.30.0/sts/data/scheme/st_multi.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.1/sts/data/scheme/variant.txt` & `sts_lib-0.30.0/sts/data/scheme/variant.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.1/sts_lib.egg-info/PKG-INFO` & `sts_lib-0.30.0/sts_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-lib
-Version: 0.29.1
+Version: 0.30.0
 Summary: An open library for flexible simplified-traditional Chinese text conversion.
 Home-page: https://github.com/danny0838/sts-lib
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
```

### Comparing `sts_lib-0.29.1/sts_lib.egg-info/SOURCES.txt` & `sts_lib-0.30.0/sts_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

