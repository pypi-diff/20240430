# Comparing `tmp/bible_reference-1.1.tar.gz` & `tmp/bible_reference-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bible_reference-1.1.tar", last modified: Sat Sep 26 18:32:04 2020, max compression
+gzip compressed data, was "bible_reference-1.2.tar", last modified: Tue Apr 30 09:38:27 2024, max compression
```

## Comparing `bible_reference-1.1.tar` & `bible_reference-1.2.tar`

### file list

```diff
@@ -1,16 +1,33 @@
-drwxr-xr-x   0 diedrich  (1001) staff       (20)        0 2020-09-26 18:32:04.000000 bible_reference-1.1/
--rw-r--r--   0 diedrich  (1001) staff       (20)     3773 2020-09-26 18:32:04.000000 bible_reference-1.1/PKG-INFO
--rw-r--r--   0 diedrich  (1001) staff       (20)     2546 2020-09-26 17:49:57.000000 bible_reference-1.1/README.md
-drwxr-xr-x   0 diedrich  (1001) staff       (20)        0 2020-09-26 18:32:04.000000 bible_reference-1.1/bible_reference/
--rw-r--r--   0 diedrich  (1001) staff       (20)     1501 2020-09-26 17:15:04.000000 bible_reference-1.1/bible_reference/__init__.py
--rw-r--r--   0 diedrich  (1001) staff       (20)    17399 2020-09-26 18:21:12.000000 bible_reference-1.1/bible_reference/bible_reference.py
--rw-r--r--   0 diedrich  (1001) staff       (20)     1462 2020-09-26 17:55:14.000000 bible_reference-1.1/bible_reference/canons.py
--rw-r--r--   0 diedrich  (1001) staff       (20)     5786 2020-09-26 11:49:40.000000 bible_reference-1.1/bible_reference/infofile.py
--rw-r--r--   0 diedrich  (1001) staff       (20)     1919 2020-09-26 18:04:51.000000 bible_reference-1.1/bible_reference/naming_schemes.py
-drwxr-xr-x   0 diedrich  (1001) staff       (20)        0 2020-09-26 18:32:04.000000 bible_reference-1.1/bible_reference.egg-info/
--rw-r--r--   0 diedrich  (1001) staff       (20)     3773 2020-09-26 18:32:03.000000 bible_reference-1.1/bible_reference.egg-info/PKG-INFO
--rw-r--r--   0 diedrich  (1001) staff       (20)      325 2020-09-26 18:32:03.000000 bible_reference-1.1/bible_reference.egg-info/SOURCES.txt
--rw-r--r--   0 diedrich  (1001) staff       (20)        1 2020-09-26 18:32:03.000000 bible_reference-1.1/bible_reference.egg-info/dependency_links.txt
--rw-r--r--   0 diedrich  (1001) staff       (20)       16 2020-09-26 18:32:03.000000 bible_reference-1.1/bible_reference.egg-info/top_level.txt
--rw-r--r--   0 diedrich  (1001) staff       (20)       38 2020-09-26 18:32:04.000000 bible_reference-1.1/setup.cfg
--rw-r--r--   0 diedrich  (1001) staff       (20)      929 2020-09-26 18:31:41.000000 bible_reference-1.1/setup.py
+drwxr-xr-x   0 diedrich  (1001) staff       (20)        0 2024-04-30 09:38:27.276358 bible_reference-1.2/
+-rw-r--r--   0 diedrich  (1001) staff       (20)    35147 2018-09-21 09:22:35.000000 bible_reference-1.2/LICENSE
+-rw-r--r--   0 diedrich  (1001) staff       (20)     3073 2024-04-30 09:38:27.275750 bible_reference-1.2/PKG-INFO
+-rw-r--r--   0 diedrich  (1001) staff       (20)     2546 2020-09-26 17:49:57.000000 bible_reference-1.2/README.md
+drwxr-xr-x   0 diedrich  (1001) staff       (20)        0 2024-04-30 09:38:27.272954 bible_reference-1.2/bible_reference/
+-rw-r--r--   0 diedrich  (1001) staff       (20)      719 2018-08-30 21:16:20.000000 bible_reference-1.2/bible_reference/BHS.canon
+-rw-r--r--   0 diedrich  (1001) staff       (20)     1558 2020-09-26 17:06:05.000000 bible_reference-1.2/bible_reference/KingJames.canon
+-rw-r--r--   0 diedrich  (1001) staff       (20)     1145 2020-03-12 14:55:04.000000 bible_reference-1.2/bible_reference/LXX.canon
+-rw-r--r--   0 diedrich  (1001) staff       (20)      924 2020-09-26 18:24:48.000000 bible_reference-1.2/bible_reference/Luther84.names
+-rw-r--r--   0 diedrich  (1001) staff       (20)      816 2018-08-27 06:40:09.000000 bible_reference-1.2/bible_reference/Luther84_abbr.names
+-rw-r--r--   0 diedrich  (1001) staff       (20)      970 2018-08-31 13:20:23.000000 bible_reference-1.2/bible_reference/RGG.names
+-rw-r--r--   0 diedrich  (1001) staff       (20)      629 2020-03-12 14:53:37.000000 bible_reference-1.2/bible_reference/RGG_abbr.names
+-rw-r--r--   0 diedrich  (1001) staff       (20)      125 2018-08-31 13:21:07.000000 bible_reference-1.2/bible_reference/RGG_lang.names
+-rw-r--r--   0 diedrich  (1001) staff       (20)     1137 2020-09-26 18:30:06.000000 bible_reference-1.2/bible_reference/SBL.names
+-rw-r--r--   0 diedrich  (1001) staff       (20)      882 2020-09-26 18:02:23.000000 bible_reference-1.2/bible_reference/SBL_abbr.names
+-rw-r--r--   0 diedrich  (1001) staff       (20)     1853 2020-09-26 18:00:33.000000 bible_reference-1.2/bible_reference/SBL_both.info
+-rw-r--r--   0 diedrich  (1001) staff       (20)     1551 2021-02-22 15:30:08.000000 bible_reference-1.2/bible_reference/__init__.py
+-rw-r--r--   0 diedrich  (1001) staff       (20)    17206 2023-08-18 17:05:35.000000 bible_reference-1.2/bible_reference/bible_reference.py
+-rw-r--r--   0 diedrich  (1001) staff       (20)     1462 2020-09-26 17:55:14.000000 bible_reference-1.2/bible_reference/canons.py
+-rw-r--r--   0 diedrich  (1001) staff       (20)     1538 2020-09-26 17:07:09.000000 bible_reference-1.2/bible_reference/default.canon
+-rw-r--r--   0 diedrich  (1001) staff       (20)      629 2020-03-12 14:53:37.000000 bible_reference-1.2/bible_reference/default.names
+-rw-r--r--   0 diedrich  (1001) staff       (20)       17 2020-03-12 14:55:04.000000 bible_reference-1.2/bible_reference/empty_first_col.info
+-rw-r--r--   0 diedrich  (1001) staff       (20)     5786 2020-09-26 11:49:40.000000 bible_reference-1.2/bible_reference/infofile.py
+-rw-r--r--   0 diedrich  (1001) staff       (20)     1561 2018-08-30 21:04:54.000000 bible_reference-1.2/bible_reference/internal_booknames.info
+-rw-r--r--   0 diedrich  (1001) staff       (20)     1538 2020-09-26 17:07:09.000000 bible_reference-1.2/bible_reference/luther.canon
+-rw-r--r--   0 diedrich  (1001) staff       (20)     1919 2020-09-26 18:04:51.000000 bible_reference-1.2/bible_reference/naming_schemes.py
+drwxr-xr-x   0 diedrich  (1001) staff       (20)        0 2024-04-30 09:38:27.275250 bible_reference-1.2/bible_reference.egg-info/
+-rw-r--r--   0 diedrich  (1001) staff       (20)     3073 2024-04-30 09:38:27.000000 bible_reference-1.2/bible_reference.egg-info/PKG-INFO
+-rw-r--r--   0 diedrich  (1001) staff       (20)      825 2024-04-30 09:38:27.000000 bible_reference-1.2/bible_reference.egg-info/SOURCES.txt
+-rw-r--r--   0 diedrich  (1001) staff       (20)        1 2024-04-30 09:38:27.000000 bible_reference-1.2/bible_reference.egg-info/dependency_links.txt
+-rw-r--r--   0 diedrich  (1001) staff       (20)       16 2024-04-30 09:38:27.000000 bible_reference-1.2/bible_reference.egg-info/top_level.txt
+-rw-r--r--   0 diedrich  (1001) staff       (20)       38 2024-04-30 09:38:27.276470 bible_reference-1.2/setup.cfg
+-rw-r--r--   0 diedrich  (1001) staff       (20)      867 2024-04-30 09:37:00.000000 bible_reference-1.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bible_reference-1.1/PKG-INFO` & `bible_reference-1.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,94 +1,78 @@
-Metadata-Version: 2.1
-Name: bible_reference
-Version: 1.1
-Summary: This module implements classes that I have developed to parse and output Bible references.
-Home-page: https://github.com/dvorberg/bible_reference
-Author: Diedrich Vorberg
-Author-email: diedrich@tux4web.de
-License: UNKNOWN
-Description: # bible_reference
-        Parse, sort and pretty-print Bible references.
-        
-        This module implements classes that I have developed to parse and
-        output Bible references. With some 3,000 years of literary history,
-        that’s not as simple a task as one might think, especially when
-        dealing with several languages. Rudimentary datafiles for English are
-        supplied, but the most detailed representation is for my native 
-        German.
-        
-        **If you have any questions or suggestions, contact me at 
-        Diedrich Vorberg ‹[diedrich@tux4web.de](mailto:diedrich@tux4web.de)›!**
-        
-        # Some introduction
-        
-        ## infofile.py
-        
-        Information is stored in a special CSV-like textfile format documented
-        in the infofile.py.
-        
-        ## bible_reference.py
-        
-        ### bible_reference.Canon
-        
-        A canon is the representation of an order of Biblical Books loaded
-        from a .canon (info-) file. 
-        
-        There is an internal (default) naming-scheme for Biblical books that
-        consists of mostly tow-letter English abbreviations. That’s hardcoded
-        in the info-files, not so much in the Python code. The order
-        of the books in the .canon file will be the sort order of the books.
-        **These internal names are refered to throughout the code as a book’s `intid`.**
-        
-        ### bible_reference.BiblicalBook
-        
-        Implement comparison (that is: sorting) of biblical books by canon
-        order.
-        
-        ### bible_reference.NamingScheme
-        
-        Return an intid for a Biblical book and provide unified
-        human-readable representations.
-        
-        ### bible_reference.bible_reference_re()
-        
-        Return a regular expression object matching Bible references that use
-        names from any of the naming schemes. Ordinals will not be checked
-        (“9.Cor” will match) nor key plausibility (meaning, ambigious naming
-        schemes will yield undefined results).
-        
-        The resulting regex should match German („1.Kor 2,12“) and English
-        (1Cor 2:12) biblical references. **Your milage for English references
-        may vary, for it has not been tested extensively.**
-        
-        ### bible_reference.BibleReference
-        
-        Here is where it all comes together. An instance is created using
-        
-        ```python
-        br = BibleReference(BiblicalBook("Jn"), 3, 16)
-        ```
-        
-        or
-        
-        ```python
-        from bible_reference import BibleReference
-        from bible_reference.naming_schemes import RGG, Luther84_abbr
-        
-        br = BibleReference.parse("Joh 3,16", [ Luther84_abbr, RGG, ])
-        ```
-        
-        For represenration, the first naming scheme passed to the constructor
-        is used by default.
-        
-        
-        There is a directory postgresql/ containing example code on how to use
-        this for sorting biblical references in the a relational database in
-        canonical order. See [postgresql/README.md](postgresql/README.md)
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=2.7
-Description-Content-Type: text/markdown
+# bible_reference
+Parse, sort and pretty-print Bible references.
+
+This module implements classes that I have developed to parse and
+output Bible references. With some 3,000 years of literary history,
+that’s not as simple a task as one might think, especially when
+dealing with several languages. Rudimentary datafiles for English are
+supplied, but the most detailed representation is for my native 
+German.
+
+**If you have any questions or suggestions, contact me at 
+Diedrich Vorberg ‹[diedrich@tux4web.de](mailto:diedrich@tux4web.de)›!**
+
+# Some introduction
+
+## infofile.py
+
+Information is stored in a special CSV-like textfile format documented
+in the infofile.py.
+
+## bible_reference.py
+
+### bible_reference.Canon
+
+A canon is the representation of an order of Biblical Books loaded
+from a .canon (info-) file. 
+
+There is an internal (default) naming-scheme for Biblical books that
+consists of mostly tow-letter English abbreviations. That’s hardcoded
+in the info-files, not so much in the Python code. The order
+of the books in the .canon file will be the sort order of the books.
+**These internal names are refered to throughout the code as a book’s `intid`.**
+
+### bible_reference.BiblicalBook
+
+Implement comparison (that is: sorting) of biblical books by canon
+order.
+
+### bible_reference.NamingScheme
+
+Return an intid for a Biblical book and provide unified
+human-readable representations.
+
+### bible_reference.bible_reference_re()
+
+Return a regular expression object matching Bible references that use
+names from any of the naming schemes. Ordinals will not be checked
+(“9.Cor” will match) nor key plausibility (meaning, ambigious naming
+schemes will yield undefined results).
+
+The resulting regex should match German („1.Kor 2,12“) and English
+(1Cor 2:12) biblical references. **Your milage for English references
+may vary, for it has not been tested extensively.**
+
+### bible_reference.BibleReference
+
+Here is where it all comes together. An instance is created using
+
+```python
+br = BibleReference(BiblicalBook("Jn"), 3, 16)
+```
+
+or
+
+```python
+from bible_reference import BibleReference
+from bible_reference.naming_schemes import RGG, Luther84_abbr
+
+br = BibleReference.parse("Joh 3,16", [ Luther84_abbr, RGG, ])
+```
+
+For represenration, the first naming scheme passed to the constructor
+is used by default.
+
+
+There is a directory postgresql/ containing example code on how to use
+this for sorting biblical references in the a relational database in
+canonical order. See [postgresql/README.md](postgresql/README.md)
```

### Comparing `bible_reference-1.1/README.md` & `bible_reference-1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: bible_reference
+Version: 1.2
+Summary: This module implements classes that I have developed to parse and output Bible references.
+Home-page: https://github.com/dvorberg/bible_reference
+Author: Diedrich Vorberg
+Author-email: diedrich@tux4web.de
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # bible_reference
 Parse, sort and pretty-print Bible references.
 
 This module implements classes that I have developed to parse and
 output Bible references. With some 3,000 years of literary history,
 that’s not as simple a task as one might think, especially when
 dealing with several languages. Rudimentary datafiles for English are
```

### Comparing `bible_reference-1.1/bible_reference/__init__.py` & `bible_reference-1.2/bible_reference/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,11 +28,13 @@
 output Bible references. With some 3,000 years of literary history
 that’s not as simple a task as one might think, especially when
 dealing with several languages. Rudimentary datafiles for English are
 supplied, but the most detailed representation is for my native tongue
 German.
 """
 
-from .bible_reference import here, Canon, NamingScheme, BiblicalBook, \
+from .bible_reference import here, \
+    Canon, NamingScheme, BiblicalBook, \
     BibleReference, BibleReferenceParser, \
-    CanonMismatch, BibleReferenceParseError
+    CanonMismatch, BibleReferenceParseError, \
+    default_naming_scheme, default_canon
```

### Comparing `bible_reference-1.1/bible_reference/bible_reference.py` & `bible_reference-1.2/bible_reference/bible_reference.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 """
 Main module containing classes Canons, biblical Books, naming
 schemes and the class that binds it all together: BibleReference.
 """
 
 from __future__ import print_function, unicode_literals
-import re, os.path as op, collections, numbers, functools
+import re, os.path as op, collections.abc, numbers, functools
 
 from .infofile import Infofile
 
 class CanonMismatch(Exception):
     """
     Raised, if biblical books sorted, that are not in the same canon.
     """
@@ -60,16 +60,16 @@
         match = reference_int_re.match(s)
         if match is None:
             raise ValueError(
                 "invalid literal for reference_int() with base 10: '%s'" % s)
         else:
             q, = match.groups()
             return int(q)
-    
-    
+
+
 class Canon:
     """
     A canon is the representation of an order of Biblical Books loaded
     from a .canon (info-) file.
     """
     def __init__(self, name):
         self.name = name
@@ -98,15 +98,15 @@
     def __init__(self, intid, canon=default_canon):
         self.intid = intid
         self.canon = canon
 
         match = ordinal_re.match(intid)
         ordinal, name = match.groups()
         self.has_ordinal = bool(ordinal)
-        
+
     def __eq__(self, other):
         return (self.intid == other.intid)
 
     def __lt__(self, other):
         assert other.canon == self.canon, CanonMismatch
         return self.canon.index[self.intid] < self.canon.index[other.intid]
 
@@ -128,22 +128,22 @@
             (1Cor, 2. Macc), specify which unicode characters should go
             between the number and the name.
         @verse_delimiter: Characer(s) put between chapter and verse
             in a reference, as in “John 2<verse_delimiter>12”.
         """
         if not name:
             self.name = "<%s %i>" % ( self.__class__.__name__, id(self), )
-        else:            
+        else:
             self.name = name
 
-        if not isinstance(name_by_intid, collections.Mapping):
+        if not isinstance(name_by_intid, collections.abc.Mapping):
             raise TypeError("name_by_intid must be Mapping type")
         else:
             self.name_by_intid = name_by_intid
-        
+
         self.ordinal_delimiter = ordinal_delimiter
         self.verse_delimiter = verse_delimiter
 
         self._intid_by_name = None
 
     @classmethod
     def internal(cls, name, ordinal_delimiter=".", verse_delimiter=","):
@@ -161,28 +161,28 @@
 
     @classmethod
     def from_infofile(cls, filepath, name=None,
                       ordinal_delimiter=".", verse_delimiter=","):
         """
         @filepath: Path to .info file, formatted like the .names files
             from this project.
-        @name: The name of this naming scheme . 
+        @name: The name of this naming scheme .
         @ordinal_delimiter: If the book has an ordinal in its name
             (1Cor, 2. Macc), specify which unicode characters should go
             between the number and the name.
         @verse_delimiter: Unicode characters but between chapter and verse
             in a reference, as in “John 2<verse_delimiter>12”.
         """
         if name is None:
             fname = op.basename(filepath)
             name, ext = op.splitext(fname)
 
         return cls(dict(Infofile(filepath)), name,
                    ordinal_delimiter, verse_delimiter)
-    
+
     @property
     def intid_by_name(self):
         """
         On demand, this will create an internal index matching tuples of
         (string-) ordinals and names to internal ids. For books that
         don’t have an ordnial, the ordinal part will be None.
         """
@@ -190,21 +190,21 @@
             """
             Return the ordinal (or None) of the book and a normalized
             representation of the name (capitalized!)
             """
             intid, name = tpl
             ordinal, name = ordinal_re.match(name).groups()
             return (ordinal, name.capitalize()), intid,
-        
+
         if self._intid_by_name is None:
             self._intid_by_name = dict(
                 [item(tpl) for tpl in self.name_by_intid.items()])
 
         return self._intid_by_name
-        
+
     def name_for(self, biblical_book):
         """
         Return the pretty name for a BiblicalBook object.
         """
         our_name = self.name_by_intid[biblical_book.intid]
 
         if biblical_book.has_ordinal:
@@ -213,15 +213,15 @@
             return ordinal + self.ordinal_delimiter + name
         else:
             return our_name
 
     def intid_of(self, ordinal, name):
         if not ordinal:
             ordinal = None
-            
+
         return self.intid_by_name[(ordinal, name.capitalize(),)]
 
     def book_named(self, ordinal, name, canon):
         """
         Return a BiblicalBook object for the info provided.
         """
         return BiblicalBook(self.intid_of(ordinal, name), canon=canon)
@@ -229,20 +229,20 @@
     def names(self, canon=None):
         """
         Return the names in this naming scheme as tuple, optionally sorted
         using a canon.
         """
         ret = self.name_by_intid.items()
 
-        # ret is a list of tuples as ( intid, name, )        
+        # ret is a list of tuples as ( intid, name, )
         if canon is not None:
             ret = sorted(ret, key=lambda tpl: canon.index[tpl[0]])
-        
+
         return tuple([tpl[1] for tpl in ret])
-        
+
 
 default_naming_scheme = NamingScheme.internal("default")
 def set_default_naming_scheme(naming_scheme):
     global default_naming_scheme
     default_naming_scheme = naming_scheme
 
 _bible_reference_re_tmpl = r"""
@@ -273,15 +273,15 @@
     Return a regular expression object matching Bible references that
     use names from any of the naming schemes. Ordinals will not be
     checked (“9.Cor” will match) nor key plausibility (meaning,
     ambigious naming schemes will yield undefined results).
     """
     if naming_schemes is None:
         naming_schemes = [ default_naming_scheme, ]
-    
+
     names = set()
     for ns in naming_schemes:
         pairs = [ordinal_re.match(name).groups() for name in ns.names()]
         without_ordinals = [ordinal_name[1] for ordinal_name in pairs]
         names = names.union(set(without_ordinals))
 
     names = "|".join(names)
@@ -297,15 +297,15 @@
     def __init__(self, naming_schemes=None, canon=default_canon):
         if naming_schemes is None:
             self.naming_schemes = [ default_naming_scheme, ]
         else:
             self.naming_schemes = naming_schemes
 
         self.canon = canon
-            
+
         self.regex = bible_reference_re(self.naming_schemes)
 
     def parse(self, s):
         """
         Parse s into a BibleReference object. May raise ParseError.
         """
         match = self.regex.match(s)
@@ -327,70 +327,70 @@
 
 @functools.total_ordering
 class BibleReference:
     """
     Represent a bible reference for sorting and representation.
     """
     whitespace_re = re.compile(r"\s+", re.UNICODE)
-    
+
     def __init__(self, book, chapter, verse, range="", naming_scheme=None):
         """
         “Chapter” and “verse” are integers (or none) for sorting, “range”
         is used for representation. Naming schemes can be provided for
         long names (“names”) and abbreviations (“abbrs”).
-        
+
         @book: BiblicalBook instance
         @chapter: (something that parses to an) integer or None
         @verse: (something that parses to an) integer or None
         @range: String, a human-readable representation of the
            chapters/verses referenced. May be ''.
         @naming_scheme: Used for representation. Defaults to
            bible_reference.default_naming_scheme.
         """
         assert isinstance(book, BiblicalBook), TypeError
         self.book = book
-        
+
         if chapter is not None:
-            chapter = reference_int(chapter)            
+            chapter = reference_int(chapter)
         self.chapter = chapter
 
-        if verse is not None:            
+        if verse is not None:
             verse = reference_int(verse)
         self.verse = verse
 
         if range:
             # Normalize the human-readable range: All whitespace are (one)
             # regular space, all dashes are typographically correct “–”s.
             range = range.replace("-", "–")
             range = self.whitespace_re.sub(" ", range)
             range = range.lower()
-            
+
         self._range = range
         self.naming_scheme = naming_scheme or default_naming_scheme
 
     @classmethod
     def parse(BibleReference, s, naming_schemes=None, canon=default_canon):
         """
         Parse the bible reference in s using naming_schemes. The first
         naming scheme is used to construct the BibleReference
         returned.
-        
+
         @param naming_schemes: Defaults to
             bible_reference.default_naming_scheme.
         @param canon: The canon that will be associated with the bible
             references returned. Defaults to the default canon.
         """
         parser = BibleReferenceParser(naming_schemes, canon)
         return parser.parse(s)
-    
+
     @classmethod
     def finditer(BibleReference, s, naming_schemes=None, canon=default_canon):
         """
         Search through `s` for Bible references using `naming_schemes`.
-        
+
         @param naming_schemes: Defaults to
             bible_reference.default_naming_scheme.
         @param canon: The canon that will be associated with the bible
             references returned. Defaults to the default canon.
         """
         parser = BibleReferenceParser(naming_schemes, canon)
         for br in parser.finditer(s):
@@ -407,32 +407,33 @@
                 book = ns.book_named(groups["ordinal"], groups["book"], canon)
                 found_in_naming_scheme = ns
                 break
             except KeyError:
                 pass
 
         if book is None:
-            raise KeyError("Unknown book: %(ordinal)s %(book)s" % groups)
+            raise BibleReferenceParseError(
+                "Unknown book: %(ordinal)s %(book)s" % groups)
 
         chapter = groups["chapter"]
-            
+
         verse = None
         if groups["verse"] is not None:
             verse = groups["verse"]
         elif groups["verse_range"] is not None:
             verse = groups["verse_range"]
         elif groups["v_start"] is not None:
             verse = groups["v_start"]
 
         # Internally, we use “,” as a verse delimiter.
         if groups["range"]:
             range = groups["range"].replace(":", ",")
         else:
             range = None
-            
+
         return BibleReference(book, chapter, verse, range, naming_schemes[0])
 
     @property
     def range(self):
         if self._range:
             return self._range
         else:
@@ -442,27 +443,27 @@
                 return "%i" % self.chapter
             else:
                 return ""
 
     @range.setter
     def range(self, range):
         # Internally, we use “,” as a verse delimiter.
-        range = range.replace(";", ",") 
+        range = range.replace(";", ",")
         self._range = range
-            
+
     def __str__(self):
         """
         The default string representation
         """
         return self.represent_using(self.naming_scheme)
 
     def __repr__(self):
         return "<%s %s:%s '%s'>" % ( self.book.intid, self.chapter, self.verse,
                                      self.range, )
-    
+
     def represent_using(self, naming_scheme):
         if self.range:
             range = self.range
             if naming_scheme.verse_delimiter != ",":
                 range = range.replace(",", naming_scheme.verse_delimiter)
             return "%s %s" % ( naming_scheme.name_for(self.book), range, )
         else:
@@ -476,15 +477,15 @@
         return (self.book, self.chapter, self.verse,) < (other.book,
                                                          other.chapter,
                                                          other.verse,)
 
     def __eq__(self, other):
         if not isinstance(other, self.__class__):
             return False
-        
+
         return ( self.book == other.book and \
                  self.range == other.range )
 
 
     def int_sort_index(self):
         """
         Return an integer uniqly identifying this biblical reference for
```

### Comparing `bible_reference-1.1/bible_reference/canons.py` & `bible_reference-1.2/bible_reference/canons.py`

 * *Files identical despite different names*

### Comparing `bible_reference-1.1/bible_reference/infofile.py` & `bible_reference-1.2/bible_reference/infofile.py`

 * *Files identical despite different names*

### Comparing `bible_reference-1.1/bible_reference/naming_schemes.py` & `bible_reference-1.2/bible_reference/naming_schemes.py`

 * *Files identical despite different names*

### Comparing `bible_reference-1.1/bible_reference.egg-info/PKG-INFO` & `bible_reference-1.2/bible_reference.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,94 +1,92 @@
 Metadata-Version: 2.1
-Name: bible-reference
-Version: 1.1
+Name: bible_reference
+Version: 1.2
 Summary: This module implements classes that I have developed to parse and output Bible references.
 Home-page: https://github.com/dvorberg/bible_reference
 Author: Diedrich Vorberg
 Author-email: diedrich@tux4web.de
-License: UNKNOWN
-Description: # bible_reference
-        Parse, sort and pretty-print Bible references.
-        
-        This module implements classes that I have developed to parse and
-        output Bible references. With some 3,000 years of literary history,
-        that’s not as simple a task as one might think, especially when
-        dealing with several languages. Rudimentary datafiles for English are
-        supplied, but the most detailed representation is for my native 
-        German.
-        
-        **If you have any questions or suggestions, contact me at 
-        Diedrich Vorberg ‹[diedrich@tux4web.de](mailto:diedrich@tux4web.de)›!**
-        
-        # Some introduction
-        
-        ## infofile.py
-        
-        Information is stored in a special CSV-like textfile format documented
-        in the infofile.py.
-        
-        ## bible_reference.py
-        
-        ### bible_reference.Canon
-        
-        A canon is the representation of an order of Biblical Books loaded
-        from a .canon (info-) file. 
-        
-        There is an internal (default) naming-scheme for Biblical books that
-        consists of mostly tow-letter English abbreviations. That’s hardcoded
-        in the info-files, not so much in the Python code. The order
-        of the books in the .canon file will be the sort order of the books.
-        **These internal names are refered to throughout the code as a book’s `intid`.**
-        
-        ### bible_reference.BiblicalBook
-        
-        Implement comparison (that is: sorting) of biblical books by canon
-        order.
-        
-        ### bible_reference.NamingScheme
-        
-        Return an intid for a Biblical book and provide unified
-        human-readable representations.
-        
-        ### bible_reference.bible_reference_re()
-        
-        Return a regular expression object matching Bible references that use
-        names from any of the naming schemes. Ordinals will not be checked
-        (“9.Cor” will match) nor key plausibility (meaning, ambigious naming
-        schemes will yield undefined results).
-        
-        The resulting regex should match German („1.Kor 2,12“) and English
-        (1Cor 2:12) biblical references. **Your milage for English references
-        may vary, for it has not been tested extensively.**
-        
-        ### bible_reference.BibleReference
-        
-        Here is where it all comes together. An instance is created using
-        
-        ```python
-        br = BibleReference(BiblicalBook("Jn"), 3, 16)
-        ```
-        
-        or
-        
-        ```python
-        from bible_reference import BibleReference
-        from bible_reference.naming_schemes import RGG, Luther84_abbr
-        
-        br = BibleReference.parse("Joh 3,16", [ Luther84_abbr, RGG, ])
-        ```
-        
-        For represenration, the first naming scheme passed to the constructor
-        is used by default.
-        
-        
-        There is a directory postgresql/ containing example code on how to use
-        this for sorting biblical references in the a relational database in
-        canonical order. See [postgresql/README.md](postgresql/README.md)
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=2.7
+Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# bible_reference
+Parse, sort and pretty-print Bible references.
+
+This module implements classes that I have developed to parse and
+output Bible references. With some 3,000 years of literary history,
+that’s not as simple a task as one might think, especially when
+dealing with several languages. Rudimentary datafiles for English are
+supplied, but the most detailed representation is for my native 
+German.
+
+**If you have any questions or suggestions, contact me at 
+Diedrich Vorberg ‹[diedrich@tux4web.de](mailto:diedrich@tux4web.de)›!**
+
+# Some introduction
+
+## infofile.py
+
+Information is stored in a special CSV-like textfile format documented
+in the infofile.py.
+
+## bible_reference.py
+
+### bible_reference.Canon
+
+A canon is the representation of an order of Biblical Books loaded
+from a .canon (info-) file. 
+
+There is an internal (default) naming-scheme for Biblical books that
+consists of mostly tow-letter English abbreviations. That’s hardcoded
+in the info-files, not so much in the Python code. The order
+of the books in the .canon file will be the sort order of the books.
+**These internal names are refered to throughout the code as a book’s `intid`.**
+
+### bible_reference.BiblicalBook
+
+Implement comparison (that is: sorting) of biblical books by canon
+order.
+
+### bible_reference.NamingScheme
+
+Return an intid for a Biblical book and provide unified
+human-readable representations.
+
+### bible_reference.bible_reference_re()
+
+Return a regular expression object matching Bible references that use
+names from any of the naming schemes. Ordinals will not be checked
+(“9.Cor” will match) nor key plausibility (meaning, ambigious naming
+schemes will yield undefined results).
+
+The resulting regex should match German („1.Kor 2,12“) and English
+(1Cor 2:12) biblical references. **Your milage for English references
+may vary, for it has not been tested extensively.**
+
+### bible_reference.BibleReference
+
+Here is where it all comes together. An instance is created using
+
+```python
+br = BibleReference(BiblicalBook("Jn"), 3, 16)
+```
+
+or
+
+```python
+from bible_reference import BibleReference
+from bible_reference.naming_schemes import RGG, Luther84_abbr
+
+br = BibleReference.parse("Joh 3,16", [ Luther84_abbr, RGG, ])
+```
+
+For represenration, the first naming scheme passed to the constructor
+is used by default.
+
+
+There is a directory postgresql/ containing example code on how to use
+this for sorting biblical references in the a relational database in
+canonical order. See [postgresql/README.md](postgresql/README.md)
```

### Comparing `bible_reference-1.1/setup.py` & `bible_reference-1.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="bible_reference", # Replace with your own username
-    version="1.1",
+    version="1.2",
     author="Diedrich Vorberg",
     author_email="diedrich@tux4web.de",
     description="This module implements classes that I have developed to parse and output Bible references.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dvorberg/bible_reference",
-    
+
     packages=setuptools.find_packages(),
-    
+
     package_data={"": ["*.names", "*.canon", "*.info"]},
     include_package_data=True,
-    
+
     classifiers=[
-        "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=2.7',
+    python_requires='>=3',
 )
-
```

