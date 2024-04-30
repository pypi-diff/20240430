# Comparing `tmp/hipack-8.tar.gz` & `tmp/hipack-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hipack-8.tar", last modified: Thu Jul 23 16:34:34 2015, max compression
+gzip compressed data, was "dist/hipack-9.tar", last modified: Sun Jul 26 21:59:11 2015, max compression
```

## Comparing `hipack-8.tar` & `hipack-9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 aperez    (1000) aperez    (1000)        0 2015-07-23 16:34:34.000000 hipack-8/
-drwxr-xr-x   0 aperez    (1000) aperez    (1000)        0 2015-07-23 16:34:34.000000 hipack-8/hipack.egg-info/
--rw-r--r--   0 aperez    (1000) aperez    (1000)     5770 2015-07-23 16:34:34.000000 hipack-8/hipack.egg-info/PKG-INFO
--rw-r--r--   0 aperez    (1000) aperez    (1000)      547 2015-07-23 16:34:34.000000 hipack-8/hipack.egg-info/SOURCES.txt
--rw-r--r--   0 aperez    (1000) aperez    (1000)        1 2015-07-23 16:34:34.000000 hipack-8/hipack.egg-info/dependency_links.txt
--rw-r--r--   0 aperez    (1000) aperez    (1000)       47 2015-07-23 16:34:34.000000 hipack-8/hipack.egg-info/pbr.json
--rw-r--r--   0 aperez    (1000) aperez    (1000)       11 2015-07-23 16:34:34.000000 hipack-8/hipack.egg-info/requires.txt
--rw-r--r--   0 aperez    (1000) aperez    (1000)        7 2015-07-23 16:34:34.000000 hipack-8/hipack.egg-info/top_level.txt
-drwxr-xr-x   0 aperez    (1000) aperez    (1000)        0 2015-07-23 16:34:34.000000 hipack-8/test/
--rw-r--r--   0 aperez    (1000) aperez    (1000)      300 2014-10-22 09:23:21.000000 hipack-8/test/drove-01.conf
--rw-r--r--   0 aperez    (1000) aperez    (1000)       41 2014-10-22 09:23:30.000000 hipack-8/test/drove-02.conf
--rw-r--r--   0 aperez    (1000) aperez    (1000)      409 2014-11-05 17:27:39.000000 hipack-8/test/omni-01.conf
--rw-r--r--   0 aperez    (1000) aperez    (1000)      962 2015-03-05 11:04:31.000000 hipack-8/test/test_files.py
--rw-r--r--   0 aperez    (1000) aperez    (1000)    13831 2015-03-05 11:05:36.000000 hipack-8/test/test_parser.py
--rw-r--r--   0 aperez    (1000) aperez    (1000)      174 2014-10-21 09:08:39.000000 hipack-8/test/wcfg-test-00.conf
--rw-r--r--   0 aperez    (1000) aperez    (1000)       34 2014-10-21 09:08:39.000000 hipack-8/test/wcfg-test-01.conf
--rw-r--r--   0 aperez    (1000) aperez    (1000)        5 2014-10-21 09:08:39.000000 hipack-8/test/wcfg-test-02.conf
--rw-r--r--   0 aperez    (1000) aperez    (1000)       10 2014-10-21 09:08:39.000000 hipack-8/test/wcfg-test-03.conf
--rw-r--r--   0 aperez    (1000) aperez    (1000)      236 2014-10-21 09:08:39.000000 hipack-8/test/wcfg-test-04.conf
--rw-r--r--   0 aperez    (1000) aperez    (1000)      182 2014-10-21 09:08:39.000000 hipack-8/test/wcfg-test-05.conf
--rw-r--r--   0 aperez    (1000) aperez    (1000)        6 2014-10-21 09:08:39.000000 hipack-8/test/wcfg-test-06.conf
--rw-r--r--   0 aperez    (1000) aperez    (1000)       15 2014-10-21 09:08:39.000000 hipack-8/test/wcfg-test-07.conf
--rw-r--r--   0 aperez    (1000) aperez    (1000)       37 2014-10-21 09:08:39.000000 hipack-8/test/wcfg-test-08.conf
--rw-r--r--   0 aperez    (1000) aperez    (1000)       94 2014-10-21 09:08:39.000000 hipack-8/test/wcfg-test-09.conf
--rw-r--r--   0 aperez    (1000) aperez    (1000)       39 2014-11-05 17:48:56.000000 hipack-8/MANIFEST.in
--rw-r--r--   0 aperez    (1000) aperez    (1000)     3686 2015-07-23 14:58:22.000000 hipack-8/README.rst
--rwxr-xr-x   0 aperez    (1000) aperez    (1000)     2766 2015-07-23 16:31:08.000000 hipack-8/hipack
--rw-r--r--   0 aperez    (1000) aperez    (1000)    12029 2015-07-23 16:27:58.000000 hipack-8/hipack.py
--rw-r--r--   0 aperez    (1000) aperez    (1000)     2115 2015-07-23 16:11:00.000000 hipack-8/setup.py
--rw-r--r--   0 aperez    (1000) aperez    (1000)     5770 2015-07-23 16:34:34.000000 hipack-8/PKG-INFO
--rw-r--r--   0 aperez    (1000) aperez    (1000)       59 2015-07-23 16:34:34.000000 hipack-8/setup.cfg
+drwxr-xr-x   0 aperez    (1000) aperez    (1000)        0 2015-07-26 21:59:11.000000 hipack-9/
+drwxr-xr-x   0 aperez    (1000) aperez    (1000)        0 2015-07-26 21:59:11.000000 hipack-9/hipack.egg-info/
+-rw-r--r--   0 aperez    (1000) aperez    (1000)     5770 2015-07-26 21:59:11.000000 hipack-9/hipack.egg-info/PKG-INFO
+-rw-r--r--   0 aperez    (1000) aperez    (1000)      547 2015-07-26 21:59:11.000000 hipack-9/hipack.egg-info/SOURCES.txt
+-rw-r--r--   0 aperez    (1000) aperez    (1000)        1 2015-07-26 21:59:11.000000 hipack-9/hipack.egg-info/dependency_links.txt
+-rw-r--r--   0 aperez    (1000) aperez    (1000)       47 2015-07-26 21:59:11.000000 hipack-9/hipack.egg-info/pbr.json
+-rw-r--r--   0 aperez    (1000) aperez    (1000)       11 2015-07-26 21:59:11.000000 hipack-9/hipack.egg-info/requires.txt
+-rw-r--r--   0 aperez    (1000) aperez    (1000)        7 2015-07-26 21:59:11.000000 hipack-9/hipack.egg-info/top_level.txt
+drwxr-xr-x   0 aperez    (1000) aperez    (1000)        0 2015-07-26 21:59:11.000000 hipack-9/test/
+-rw-r--r--   0 aperez    (1000) aperez    (1000)      300 2015-07-26 21:35:08.000000 hipack-9/test/drove-01.conf
+-rw-r--r--   0 aperez    (1000) aperez    (1000)       41 2014-10-22 09:23:30.000000 hipack-9/test/drove-02.conf
+-rw-r--r--   0 aperez    (1000) aperez    (1000)      409 2014-11-05 17:27:39.000000 hipack-9/test/omni-01.conf
+-rw-r--r--   0 aperez    (1000) aperez    (1000)      962 2015-03-05 11:04:31.000000 hipack-9/test/test_files.py
+-rw-r--r--   0 aperez    (1000) aperez    (1000)    13805 2015-07-26 21:55:42.000000 hipack-9/test/test_parser.py
+-rw-r--r--   0 aperez    (1000) aperez    (1000)      174 2014-10-21 09:08:39.000000 hipack-9/test/wcfg-test-00.conf
+-rw-r--r--   0 aperez    (1000) aperez    (1000)       34 2014-10-21 09:08:39.000000 hipack-9/test/wcfg-test-01.conf
+-rw-r--r--   0 aperez    (1000) aperez    (1000)        5 2014-10-21 09:08:39.000000 hipack-9/test/wcfg-test-02.conf
+-rw-r--r--   0 aperez    (1000) aperez    (1000)       10 2014-10-21 09:08:39.000000 hipack-9/test/wcfg-test-03.conf
+-rw-r--r--   0 aperez    (1000) aperez    (1000)      236 2014-10-21 09:08:39.000000 hipack-9/test/wcfg-test-04.conf
+-rw-r--r--   0 aperez    (1000) aperez    (1000)      182 2014-10-21 09:08:39.000000 hipack-9/test/wcfg-test-05.conf
+-rw-r--r--   0 aperez    (1000) aperez    (1000)        6 2014-10-21 09:08:39.000000 hipack-9/test/wcfg-test-06.conf
+-rw-r--r--   0 aperez    (1000) aperez    (1000)       15 2014-10-21 09:08:39.000000 hipack-9/test/wcfg-test-07.conf
+-rw-r--r--   0 aperez    (1000) aperez    (1000)       37 2014-10-21 09:08:39.000000 hipack-9/test/wcfg-test-08.conf
+-rw-r--r--   0 aperez    (1000) aperez    (1000)       94 2014-10-21 09:08:39.000000 hipack-9/test/wcfg-test-09.conf
+-rw-r--r--   0 aperez    (1000) aperez    (1000)       39 2014-11-05 17:48:56.000000 hipack-9/MANIFEST.in
+-rw-r--r--   0 aperez    (1000) aperez    (1000)     3686 2015-07-23 14:58:22.000000 hipack-9/README.rst
+-rwxr-xr-x   0 aperez    (1000) aperez    (1000)     2984 2015-07-24 06:12:21.000000 hipack-9/hipack
+-rw-r--r--   0 aperez    (1000) aperez    (1000)    14184 2015-07-26 21:58:17.000000 hipack-9/hipack.py
+-rw-r--r--   0 aperez    (1000) aperez    (1000)     2115 2015-07-23 16:11:00.000000 hipack-9/setup.py
+-rw-r--r--   0 aperez    (1000) aperez    (1000)     5770 2015-07-26 21:59:11.000000 hipack-9/PKG-INFO
+-rw-r--r--   0 aperez    (1000) aperez    (1000)       59 2015-07-26 21:59:11.000000 hipack-9/setup.cfg
```

### Comparing `hipack-8/hipack.egg-info/PKG-INFO` & `hipack-9/hipack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: hipack
-Version: 8
+Version: 9
 Summary: Serialization library or the HiPack interchange format
 Home-page: https://github.com/aperezdc/hipack-python
 Author: Adrian Perez de Castro
 Author-email: aperez@igalia.com
 License: Dual GPL3 / MIT
 Description: ===============
          hipack-python
```

### Comparing `hipack-8/hipack.egg-info/SOURCES.txt` & `hipack-9/hipack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hipack-8/test/test_files.py` & `hipack-9/test/test_files.py`

 * *Files identical despite different names*

### Comparing `hipack-8/test/test_parser.py` & `hipack-9/test/test_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,14 +52,15 @@
         )
         self.check_numbers(numbers, six.integer_types)
 
     def test_parse_valid_hex_numbers(self):
         numbers = (
             (u"0x1", 1),
             (u"0X1", 1),
+            (u"-0x3", -0x3),
             (u"0xcafe", 0xCAFE),
             (u"0XCAFE", 0xCAFE),
             (u"0xCAFE", 0xCAFE),
             (u"0xCaFe", 0xCAFE),
             (u"0x1234", 0x1234),
             (u"0xC00FFEE", 0xC00FFEE),
             (u"0xdeadbeef", 0xdeadbeef),
@@ -67,21 +68,23 @@
         self.check_numbers(numbers, six.integer_types)
 
     def test_parse_valid_octal_numbers(self):
         numbers = (
             (u"01", 0o1),
             (u"01234567", 0o1234567),
             (u"042", 0o42),
+            (u"-032", -0o32),
         )
         self.check_numbers(numbers, six.integer_types)
 
     def test_parse_valid_float_numbers(self):
         numbers = (
             (u"1.", 1.0),
             (u".5", 0.5),
+            (u"0.1", 0.1),
             (u"1.5", 1.5),
             (u"1e3", 1e3),
             (u"1e-3", 1e-3),
             (u"1.e3", 1e3),
             (u"1.e-3", 1e-3),
             (u".5e3", 0.5e3),
             (u".5e-3", 0.5e-3),
@@ -92,16 +95,16 @@
             for item, value in numbers:
                 yield (item, value)
                 yield (u"+" + item, value)
                 yield (u"-" + item, -value)
 
         self.check_numbers(gen_signs(), float)
 
-    def test_parse_valid_identifiers(self):
-        identifiers = (
+    def test_parse_valid_keys(self):
+        keys = (
             # Typical definition of identifiers.
             u"foo",
             u"ident-with-dashes",
             u"-leading-dash",
             u"trailing-dash-",
             u"ident_with_underscores",
             u"_leading_underscore",
@@ -113,18 +116,18 @@
             u"空手",
             u"→",
             # Mixed.
             u"arrow→",
             u"Trømso",
             u"Güedángaños",
         )
-        for item in identifiers:
-            ident = self.parser(item).parse_identifier()
-            self.assertEquals(item, ident)
-            self.assertTrue(isinstance(ident, six.text_type))
+        for item in keys:
+            key = self.parser(item).parse_key()
+            self.assertEquals(item, key)
+            self.assertTrue(isinstance(key, six.text_type))
 
     def check_strings(self, strings, type_):
         for item in strings:
             if isinstance(item, tuple):
                 item, expected = item
             else:
                 expected = item
@@ -137,15 +140,14 @@
             u"",
             u"this is a string",
             u" another with leading space",
             u"yet one more with trailing space ",
             u"unicode: this → that, Trømso, Java™, ☺",
             (u"escaped backslash: \\\\", u"escaped backslash: \\"),
             (u"escaped double quote: \\\"", u"escaped double quote: \""),
-            (u"escaped UTF-8: \\☺", u"escaped UTF-8: ☺"),
         )
         self.check_strings(strings, six.text_type)
 
     def test_parse_valid_arrays(self):
         arrays = (
             (u"[]", []),
             (u"[ ]", []),
@@ -216,15 +218,15 @@
 
     def test_parse_invalid_numbers(self):
         invalid_numbers = (
             u"", u"-", u"+", u"-+", u"a", u"☺", u"-.", u".", u"e", u".e",
             u"+e", u"-e", u"-.e", u"+.e", u"e+", u"e-", u".-e", u".+e",
             u"--", u"++", u"+1e3.", u"..1", u"1.2.", u"1..2", u"\"foo\"",
             u"True", u"False", u"{}", u"[]", u"()", u"0xx00", "0.1AeA3",
-            "-0x3", "-032", u"ee", u"1ee", u"1e1e1", u"0.1x2", u"1x.0",
+            u"ee", u"1ee", u"1e1e1", u"0.1x2", u"1x.0",
         )
         for item in invalid_numbers:
             with self.assertRaises(hipack.ParseError):
                 self.parser(item).parse_number()
 
     def test_parse_invalid_booleans(self):
         invalid_booleans = (
```

### Comparing `hipack-8/README.rst` & `hipack-9/README.rst`

 * *Files identical despite different names*

### Comparing `hipack-8/hipack` & `hipack-9/hipack`

 * *Files 23% similar despite different names*

```diff
@@ -58,39 +58,42 @@
     "yaml":
         (load_yaml, save_yaml),
     "msgpack":
         (load_msgpack, save_msgpack),
 }
 
 
-import optparse
-parser = optparse.OptionParser("[-f format] [-t format] < input > output")
-parser.add_option("-f", "--from", dest="from_format", default="json",
-        help="Read input in the specified FORMAT [default: %default]",
-        metavar="FORMAT")
-parser.add_option("-t", "--to", dest="to_format", default="hipack",
-        help="Write output in the specified FORMAT [default: %default]",
-        metavar="FORMAT")
-parser.add_option("--formats", default=False, action="store_true",
-        help="Print list of supported formats and exit")
-parser.add_option("--hipack-module-version", default=False,
-        action="store_true", dest="hipack_module_version",
+import argparse, sys
+parser = argparse.ArgumentParser()
+parser.add_argument('input', nargs='?', type=argparse.FileType('r'),
+        help='Input file or - [default: stdin]', default=sys.stdin)
+parser.add_argument('output', nargs='?', type=argparse.FileType('w'),
+        help='Output file [default: stdout]', default=sys.stdout)
+parser.add_argument('-f', '--from', dest='from_format', default='json',
+        help='Read input in the specified FORMAT [default: %(default)s]',
+        metavar='FORMAT')
+parser.add_argument('-t', '--to', dest='to_format', default='hipack',
+        help='Write output in the specified FORMAT [default: %(default)s]',
+        metavar='FORMAT')
+parser.add_argument('--formats', default=False, action='store_true',
+        help='Print list of supported formats and exit')
+parser.add_argument('--hipack-module-version', default=False,
+        action='store_true', dest='hipack_module_version',
         help="Show the version of the hipack Python module")
 
 if __name__ == "__main__":
-    import sys
-    options, args = parser.parse_args()
-    if options.formats:
+    args = parser.parse_args()
+    if args.formats:
         [print_(name) for name in sorted(formats.keys())]
-    elif options.hipack_module_version:
+    elif args.hipack_module_version:
         print_(hipack.__version__)
     else:
         try:
-            load = formats[options.from_format][0]
+            load = formats[args.from_format][0]
         except KeyError:
             raise SystemExit("No such format: " + options.from_format)
         try:
-            save = formats[options.to_format][1]
+            save = formats[args.to_format][1]
         except KeyError:
             raise SystemExit("No such format: " + options.to_format)
 
-        save(load(sys.stdin), sys.stdout)
+        save(load(args.input), args.output)
```

### Comparing `hipack-8/setup.py` & `hipack-9/setup.py`

 * *Files identical despite different names*

### Comparing `hipack-8/PKG-INFO` & `hipack-9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: hipack
-Version: 8
+Version: 9
 Summary: Serialization library or the HiPack interchange format
 Home-page: https://github.com/aperezdc/hipack-python
 Author: Adrian Perez de Castro
 Author-email: aperez@igalia.com
 License: Dual GPL3 / MIT
 Description: ===============
          hipack-python
```

