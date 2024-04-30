# Comparing `tmp/google-re2-1.0.tar.gz` & `tmp/google-re2-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-re2-1.0.tar", last modified: Mon Oct 24 16:31:18 2022, max compression
+gzip compressed data, was "google-re2-1.1.tar", last modified: Mon Jul 31 16:01:23 2023, max compression
```

## Comparing `google-re2-1.0.tar` & `google-re2-1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 16:31:18.130456 google-re2-1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     2126 2022-10-24 16:31:18.130456 google-re2-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-10-24 16:31:14.000000 google-re2-1.0/README
--rw-r--r--   0 runner    (1001) docker     (121)    11187 2022-10-24 16:31:17.000000 google-re2-1.0/_re2.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 16:31:18.130456 google-re2-1.0/google_re2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2126 2022-10-24 16:31:18.000000 google-re2-1.0/google_re2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-10-24 16:31:18.000000 google-re2-1.0/google_re2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-24 16:31:18.000000 google-re2-1.0/google_re2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-10-24 16:31:18.000000 google-re2-1.0/google_re2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    17442 2022-10-24 16:31:14.000000 google-re2-1.0/re2.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-24 16:31:18.130456 google-re2-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5166 2022-10-24 16:31:14.000000 google-re2-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:01:23.511251 google-re2-1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-31 16:01:19.000000 google-re2-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-31 16:01:23.511251 google-re2-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-31 16:01:19.000000 google-re2-1.1/README
+-rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-07-31 16:01:19.000000 google-re2-1.1/_re2.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:01:23.511251 google-re2-1.1/google_re2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-31 16:01:23.000000 google-re2-1.1/google_re2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-31 16:01:23.000000 google-re2-1.1/google_re2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 16:01:23.000000 google-re2-1.1/google_re2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-31 16:01:23.000000 google-re2-1.1/google_re2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17577 2023-07-31 16:01:19.000000 google-re2-1.1/re2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 16:01:23.511251 google-re2-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-31 16:01:19.000000 google-re2-1.1/setup.py
```

### Comparing `google-re2-1.0/PKG-INFO` & `google-re2-1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: google-re2
-Version: 1.0
+Version: 1.1
 Summary: RE2 Python bindings
 Home-page: https://github.com/google/re2
 Author: The RE2 Authors
 Author-email: re2-dev@googlegroups.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: C++
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: ~=3.7
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: ~=3.8
 Description-Content-Type: text/plain
+License-File: LICENSE
 
 A drop-in replacement for the re module.
 
 It uses RE2 under the hood, of course, so various PCRE features
 (e.g. backreferences, look-around assertions) are not supported.
 See https://github.com/google/re2/wiki/Syntax for the canonical
 reference, but known syntactic "gotchas" relative to Python are:
```

### Comparing `google-re2-1.0/_re2.cc` & `google-re2-1.1/_re2.cc`

 * *Files 3% similar despite different names*

```diff
@@ -6,33 +6,38 @@
 #include <string>
 #include <tuple>
 #include <utility>
 #include <vector>
 
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
-#include "re2/stringpiece.h"
+#include "absl/strings/string_view.h"
 #include "re2/filtered_re2.h"
 #include "re2/re2.h"
 #include "re2/set.h"
 
+#ifdef _WIN32
+#include <basetsd.h>
+#define ssize_t SSIZE_T
+#endif
+
 namespace re2_python {
 
 // This is conventional.
 namespace py = pybind11;
 
 // In terms of the pybind11 API, a py::buffer is merely a py::object that
 // supports the buffer interface/protocol and you must explicitly request
 // a py::buffer_info in order to access the actual bytes. Under the hood,
 // the py::buffer_info manages a reference count to the py::buffer, so it
 // must be constructed and subsequently destructed while holding the GIL.
-static inline re2::StringPiece FromBytes(const py::buffer_info& bytes) {
+static inline absl::string_view FromBytes(const py::buffer_info& bytes) {
   char* data = reinterpret_cast<char*>(bytes.ptr);
   ssize_t size = bytes.size;
-  return re2::StringPiece(data, size);
+  return absl::string_view(data, size);
 }
 
 static inline int OneCharLen(const char* ptr) {
   return "\1\1\1\1\1\1\1\1\1\1\1\1\2\2\3\4"[(*ptr & 0xFF) >> 4];
 }
 
 // Helper function for when Python encodes str to bytes and then needs to
@@ -64,15 +69,15 @@
   return len;
 }
 
 std::unique_ptr<RE2> RE2InitShim(py::buffer buffer,
                                  const RE2::Options& options) {
   auto bytes = buffer.request();
   auto pattern = FromBytes(bytes);
-  return std::unique_ptr<RE2>(new RE2(pattern, options));
+  return std::make_unique<RE2>(pattern, options);
 }
 
 py::bytes RE2ErrorShim(const RE2& self) {
   // Return std::string as bytes. That is, without decoding to str.
   return self.error();
 }
 
@@ -110,21 +115,21 @@
                                                       RE2::Anchor anchor,
                                                       py::buffer buffer,
                                                       ssize_t pos,
                                                       ssize_t endpos) {
   auto bytes = buffer.request();
   auto text = FromBytes(bytes);
   const int num_groups = self.NumberOfCapturingGroups() + 1;  // need $0
-  std::vector<re2::StringPiece> groups;
+  std::vector<absl::string_view> groups;
   groups.resize(num_groups);
   py::gil_scoped_release release_gil;
   if (!self.Match(text, pos, endpos, anchor, groups.data(), groups.size())) {
     // Ensure that groups are null before converting to spans!
     for (auto& it : groups) {
-      it = re2::StringPiece();
+      it = absl::string_view();
     }
   }
   std::vector<std::pair<ssize_t, ssize_t>> spans;
   spans.reserve(num_groups);
   for (const auto& it : groups) {
     if (it.data() == NULL) {
       spans.emplace_back(-1, -1);
@@ -198,15 +203,15 @@
 
   bool Compile() {
     std::vector<std::string> atoms;
     filter_.Compile(&atoms);
     RE2::Options options;
     options.set_literal(true);
     options.set_case_sensitive(false);
-    set_ = std::unique_ptr<RE2::Set>(new RE2::Set(options, RE2::UNANCHORED));
+    set_ = std::make_unique<RE2::Set>(options, RE2::UNANCHORED);
     for (int i = 0; i < static_cast<int>(atoms.size()); ++i) {
       if (set_->Add(atoms[i], /*error=*/NULL) != i) {
         // Should never happen: the atom is a literal!
         py::pybind11_fail("set_->Add() failed");
       }
     }
     // Compiling can fail.
@@ -224,14 +229,18 @@
       filter_.AllPotentials(atoms, &matches);
     } else {
       filter_.AllMatches(text, atoms, &matches);
     }
     return matches;
   }
 
+  const RE2& GetRE2(int index) const {
+    return filter_.GetRE2(index);
+  }
+
  private:
   re2::FilteredRE2 filter_;
   std::unique_ptr<RE2::Set> set_;
 };
 
 PYBIND11_MODULE(_re2, module) {
   module.def("CharLenToBytes", &CharLenToBytes);
@@ -317,11 +326,13 @@
       .def("Add", &Set::Add)
       .def("Compile", &Set::Compile)
       .def("Match", &Set::Match);
 
   filter.def(py::init<>())
       .def("Add", &Filter::Add)
       .def("Compile", &Filter::Compile)
-      .def("Match", &Filter::Match);
+      .def("Match", &Filter::Match)
+      .def("GetRE2", &Filter::GetRE2,
+           py::return_value_policy::reference_internal);
 }
 
 }  // namespace re2_python
```

### Comparing `google-re2-1.0/google_re2.egg-info/PKG-INFO` & `google-re2-1.1/google_re2.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: google-re2
-Version: 1.0
+Version: 1.1
 Summary: RE2 Python bindings
 Home-page: https://github.com/google/re2
 Author: The RE2 Authors
 Author-email: re2-dev@googlegroups.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: C++
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: ~=3.7
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: ~=3.8
 Description-Content-Type: text/plain
+License-File: LICENSE
 
 A drop-in replacement for the re module.
 
 It uses RE2 under the hood, of course, so various PCRE features
 (e.g. backreferences, look-around assertions) are not supported.
 See https://github.com/google/re2/wiki/Syntax for the canonical
 reference, but known syntactic "gotchas" relative to Python are:
```

### Comparing `google-re2-1.0/re2.py` & `google-re2-1.1/re2.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,22 +22,17 @@
 
 This module's LRU cache contains a maximum of 128 regular expression objects.
 Each regular expression object's underlying RE2 object uses a maximum of 8MiB
 of memory (by default). Hence, this module's LRU cache uses a maximum of 1GiB
 of memory (by default), but in most cases, it should use much less than that.
 """
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
 import codecs
 import functools
 import itertools
-import struct
 
 import _re2
 
 
 class error(Exception):
   pass
 
@@ -349,26 +344,26 @@
     self._text = text
     self._pos = pos
     self._endpos = endpos
     self._spans = spans
 
   # Python prioritises three-digit octal numbers over group escapes.
   # For example, \100 should not be handled the same way as \g<10>0.
-  _OCTAL_RE = compile(b'\\\\[0-7][0-7][0-7]')
+  _OCTAL_RE = compile('\\\\[0-7][0-7][0-7]')
 
   # Python supports \1 through \99 (inclusive) and \g<...> syntax.
-  _GROUP_RE = compile(b'\\\\[1-9][0-9]?|\\\\g<\\w+>')
+  _GROUP_RE = compile('\\\\[1-9][0-9]?|\\\\g<\\w+>')
 
   @classmethod
   @functools.lru_cache(typed=True)
   def _split(cls, template):
     if isinstance(template, str):
-      backslash = chr(0x5C)  # u'\\'
+      backslash = '\\'
     else:
-      backslash = struct.Struct('B').pack(0x5C)  # b'\\'
+      backslash = b'\\'
     empty = type(template)()
     pieces = [empty]
     index = template.find(backslash)
     while index != -1:
       piece, template = template[:index], template[index:]
       pieces[-1] += piece
       octal_match = cls._OCTAL_RE.match(template)
@@ -414,15 +409,15 @@
 
   def __getitem__(self, group):
     if not isinstance(group, int):
       try:
         group = self._regexp.groupindex[group]
       except KeyError:
         raise IndexError('bad group name')
-    if group < 0 or group > self._regexp.groups:
+    if not 0 <= group <= self._regexp.groups:
       raise IndexError('bad group index')
     span = self._spans[group]
     if span == _NULL_SPAN:
       return None
     return self._text[span[0]:span[1]]
 
   def group(self, *groups):
@@ -442,25 +437,25 @@
     items = []
     for group, index in self._regexp.groupindex.items():
       item = self.__getitem__(index)
       items.append((group, default) if item is None else (group, item))
     return dict(items)
 
   def start(self, group=0):
-    if group < 0 or group > self._regexp.groups:
+    if not 0 <= group <= self._regexp.groups:
       raise IndexError('bad group index')
     return self._spans[group][0]
 
   def end(self, group=0):
-    if group < 0 or group > self._regexp.groups:
+    if not 0 <= group <= self._regexp.groups:
       raise IndexError('bad group index')
     return self._spans[group][1]
 
   def span(self, group=0):
-    if group < 0 or group > self._regexp.groups:
+    if not 0 <= group <= self._regexp.groups:
       raise IndexError('bad group index')
     return self._spans[group]
 
   @property
   def re(self):
     return self._regexp
 
@@ -544,34 +539,44 @@
       matches = self._set.Match(text)
     return matches or None
 
 
 class Filter(object):
   """A Pythonic wrapper around FilteredRE2."""
 
-  __slots__ = ('_filter')
+  __slots__ = ('_filter', '_patterns')
 
   def __init__(self):
     self._filter = _re2.Filter()
+    self._patterns = []
 
   def Add(self, pattern, options=None):
     options = options or Options()
     if isinstance(pattern, str):
       encoded_pattern = _encode(pattern)
       index = self._filter.Add(encoded_pattern, options)
     else:
       index = self._filter.Add(pattern, options)
     if index == -1:
       raise error('failed to add %r to Filter' % pattern)
+    self._patterns.append(pattern)
     return index
 
   def Compile(self):
     if not self._filter.Compile():
       raise error('failed to compile Filter')
 
   def Match(self, text, potential=False):
     if isinstance(text, str):
       encoded_text = _encode(text)
       matches = self._filter.Match(encoded_text, potential)
     else:
       matches = self._filter.Match(text, potential)
     return matches or None
+
+  def re(self, index):
+    if not 0 <= index < len(self._patterns):
+      raise IndexError('bad index')
+    proxy = object.__new__(_Regexp)
+    proxy._pattern = self._patterns[index]
+    proxy._regexp = self._filter.GetRE2(index)
+    return proxy
```

### Comparing `google-re2-1.0/setup.py` & `google-re2-1.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # license that can be found in the LICENSE file.
 
 import os
 import setuptools
 import setuptools.command.build_ext
 import shutil
 import sys
-import sysconfig
 
 long_description = r"""A drop-in replacement for the re module.
 
 It uses RE2 under the hood, of course, so various PCRE features
 (e.g. backreferences, look-around assertions) are not supported.
 See https://github.com/google/re2/wiki/Syntax for the canonical
 reference, but known syntactic "gotchas" relative to Python are:
@@ -42,57 +41,33 @@
   * Building on Windows has not been tested yet and will probably fail.
 """
 
 
 class BuildExt(setuptools.command.build_ext.build_ext):
 
   def build_extension(self, ext):
-    # We will always be setting this when we are using Bazel
-    # because AppleClang never increases the `-std` version.
-    if 'BAZEL_CXXOPTS' not in os.environ:
+    if 'GITHUB_ACTIONS' not in os.environ:
       return super().build_extension(ext)
 
     # For @pybind11_bazel's `python_configure()`.
     os.environ['PYTHON_BIN_PATH'] = sys.executable
 
-    # pyformat: disable
-    bazel_clean = ['bazel', 'clean', '--expunge']
-    bazel_build = ['bazel', 'build', '--compilation_mode=opt', '--', ':all']
-    bazel_test  = ['bazel', 'test',  '--compilation_mode=opt', '--test_output=errors', '--', ':all']
-    # pyformat: enable
-
-    if sysconfig.get_platform().startswith('linux-'):
-      self.spawn(bazel_clean)
-      self.spawn(bazel_build)
-      self.spawn(bazel_test)
-      # This ensures that f'_re2.{importlib.machinery.EXTENSION_SUFFIXES[0]}'
-      # is the filename in the destination directory, which is what's needed.
-      shutil.copyfile('../bazel-bin/python/_re2.so',
-                      self.get_ext_fullpath(ext.name))
-    elif sysconfig.get_platform().startswith('macosx-'):
-      base_bazel_cxxopts = os.environ.get('BAZEL_CXXOPTS')
-      base_bazel_linkopts = os.environ.get('BAZEL_LINKOPTS')
-      for arch in ('x86_64', 'arm64'):
-        os.environ['BAZEL_CXXOPTS'] = (
-            f'{base_bazel_cxxopts}:--target={arch}-apple-macosx'
-            if base_bazel_cxxopts else f'--target={arch}-apple-macosx')
-        os.environ['BAZEL_LINKOPTS'] = (
-            f'{base_bazel_linkopts}:--target={arch}-apple-macosx'
-            if base_bazel_linkopts else f'--target={arch}-apple-macosx')
-        self.spawn(bazel_clean)
-        self.spawn(bazel_build)
-        if arch == os.uname().machine:
-          self.spawn(bazel_test)
-        shutil.copyfile('../bazel-bin/python/_re2.so', f'_re2.{arch}.so')
-      # This ensures that f'_re2.{importlib.machinery.EXTENSION_SUFFIXES[0]}'
-      # is the filename in the destination directory, which is what's needed.
-      self.spawn(['lipo', '-create'] +
-                 [f'_re2.{arch}.so' for arch in ('x86_64', 'arm64')] +
-                 ['-output', self.get_ext_fullpath(ext.name)])
-    self.spawn(['bazel', 'shutdown'])
+    cmd = ['bazel', 'build']
+    if 'BAZEL_CPU' in os.environ:
+      cmd.append(f'--cpu={os.environ["BAZEL_CPU"].lower()}')
+    cmd += ['--compilation_mode=opt', '--', ':all']
+    self.spawn(cmd)
+
+    # This ensures that f'_re2.{importlib.machinery.EXTENSION_SUFFIXES[0]}'
+    # is the filename in the destination directory, which is what's needed.
+    shutil.copyfile('../bazel-bin/python/_re2.so',
+                    self.get_ext_fullpath(ext.name))
+
+    cmd = ['bazel', 'clean', '--expunge']
+    self.spawn(cmd)
 
 
 def include_dirs():
   try:
     import pybind11
     yield pybind11.get_include()
   except ModuleNotFoundError:
@@ -105,26 +80,26 @@
     include_dirs=list(include_dirs()),
     libraries=['re2'],
     extra_compile_args=['-fvisibility=hidden'],
 )
 
 setuptools.setup(
     name='google-re2',
-    version='1.0',
+    version='1.1',
     description='RE2 Python bindings',
     long_description=long_description,
     long_description_content_type='text/plain',
-    url='https://github.com/google/re2',
     author='The RE2 Authors',
     author_email='re2-dev@googlegroups.com',
+    url='https://github.com/google/re2',
+    py_modules=['re2'],
+    ext_modules=[ext_module],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Programming Language :: C++',
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
     ],
     cmdclass={'build_ext': BuildExt},
-    ext_modules=[ext_module],
-    py_modules=['re2'],
-    python_requires='~=3.7',
+    python_requires='~=3.8',
 )
```

