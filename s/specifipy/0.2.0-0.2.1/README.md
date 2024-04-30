# Comparing `tmp/specifipy-0.2.0.tar.gz` & `tmp/specifipy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specifipy-0.2.0.tar", max compression
+gzip compressed data, was "specifipy-0.2.1.tar", max compression
```

## Comparing `specifipy-0.2.0.tar` & `specifipy-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,20 @@
--rw-r--r--   0        0        0      787 2024-04-28 19:56:32.102478 specifipy-0.2.0/LICENSE
--rw-r--r--   0        0        0      475 2024-04-28 19:58:37.523622 specifipy-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-21 19:38:27.704635 specifipy-0.2.0/specifipy/__init__.py
--rw-r--r--   0        0        0        0 2022-11-23 00:36:11.690401 specifipy-0.2.0/specifipy/file_scanners/__init__.py
--rw-r--r--   0        0        0      169 2022-11-23 00:46:48.013676 specifipy-0.2.0/specifipy/file_scanners/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2917 2022-11-23 01:17:49.081765 specifipy-0.2.0/specifipy/file_scanners/__pycache__/directory_scanner.cpython-310.pyc
--rw-r--r--   0        0        0     3115 2024-04-28 19:44:17.209269 specifipy-0.2.0/specifipy/file_scanners/directory_scanner.py
--rw-r--r--   0        0        0        0 2022-11-13 01:23:17.772427 specifipy-0.2.0/specifipy/parsers/__init__.py
--rw-r--r--   0        0        0      159 2022-11-21 19:38:37.871943 specifipy-0.2.0/specifipy/parsers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3561 2024-04-28 19:40:35.952716 specifipy-0.2.0/specifipy/parsers/__pycache__/diagram_generator_d2.cpython-310.pyc
--rw-r--r--   0        0        0     2959 2024-04-28 19:56:33.750492 specifipy-0.2.0/specifipy/parsers/__pycache__/generic_parser.cpython-310.pyc
--rw-r--r--   0        0        0      656 2022-11-21 21:38:53.247387 specifipy-0.2.0/specifipy/parsers/__pycache__/results.cpython-310.pyc
--rw-r--r--   0        0        0     3653 2024-04-28 19:49:06.246888 specifipy-0.2.0/specifipy/parsers/diagram_generator_d2.py
--rw-r--r--   0        0        0     4710 2024-04-28 19:44:05.813223 specifipy-0.2.0/specifipy/parsers/generic_parser.py
--rw-r--r--   0        0        0      372 2022-11-21 21:26:32.295737 specifipy-0.2.0/specifipy/parsers/results.py
--rw-r--r--   0        0        0        0 2022-11-13 12:43:58.920266 specifipy-0.2.0/specifipy/parsers/structure/__init__.py
--rw-r--r--   0        0        0      169 2022-11-21 19:39:10.949975 specifipy-0.2.0/specifipy/parsers/structure/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2263 2024-04-28 19:56:33.750492 specifipy-0.2.0/specifipy/parsers/structure/__pycache__/code_structure_definitions.cpython-310.pyc
--rw-r--r--   0        0        0     1368 2024-04-28 18:51:56.757737 specifipy-0.2.0/specifipy/parsers/structure/code_structure_definitions.py
--rw-r--r--   0        0        0      702 2022-11-13 17:06:58.000000 specifipy-0.2.0/specifipy/resources/icons/class_icon.png
--rw-r--r--   0        0        0      657 2022-11-13 21:47:07.995000 specifipy-0.2.0/specifipy/resources/icons/field_icon.png
--rw-r--r--   0        0        0     1058 2022-11-13 19:49:27.078750 specifipy-0.2.0/specifipy/resources/icons/function_icon.png
--rw-r--r--   0        0        0     1177 2022-11-13 19:51:34.909185 specifipy-0.2.0/specifipy/resources/icons/param_icon.png
--rw-r--r--   0        0        0      814 1970-01-01 00:00:00.000000 specifipy-0.2.0/setup.py
--rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 specifipy-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      787 2024-04-28 19:56:32.102478 specifipy-0.2.1/LICENSE
+-rw-r--r--   0        0        0      475 2024-04-29 14:28:56.073415 specifipy-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-21 19:38:27.704635 specifipy-0.2.1/specifipy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:19:27.669788 specifipy-0.2.1/specifipy/diagram_engines/__init__.py
+-rw-r--r--   0        0        0      440 2024-04-29 23:56:13.768169 specifipy-0.2.1/specifipy/diagram_engines/hashable_connection.py
+-rw-r--r--   0        0        0        0 2022-11-23 00:36:11.690401 specifipy-0.2.1/specifipy/file_scanners/__init__.py
+-rw-r--r--   0        0        0     4196 2024-04-29 23:23:55.544508 specifipy-0.2.1/specifipy/file_scanners/directory_scanner.py
+-rw-r--r--   0        0        0        0 2022-11-13 01:23:17.772427 specifipy-0.2.1/specifipy/parsers/__init__.py
+-rw-r--r--   0        0        0      159 2022-11-21 19:38:37.871943 specifipy-0.2.1/specifipy/parsers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3232 2024-04-29 23:50:20.980382 specifipy-0.2.1/specifipy/parsers/__pycache__/generic_parser.cpython-310.pyc
+-rw-r--r--   0        0        0      656 2022-11-21 21:38:53.247387 specifipy-0.2.1/specifipy/parsers/__pycache__/results.cpython-310.pyc
+-rw-r--r--   0        0        0     5253 2024-04-29 23:23:55.532508 specifipy-0.2.1/specifipy/parsers/diagram_generator_d2.py
+-rw-r--r--   0        0        0     5572 2024-04-29 14:18:05.944043 specifipy-0.2.1/specifipy/parsers/generic_parser.py
+-rw-r--r--   0        0        0      372 2022-11-21 21:26:32.295737 specifipy-0.2.1/specifipy/parsers/results.py
+-rw-r--r--   0        0        0        0 2022-11-13 12:43:58.920266 specifipy-0.2.1/specifipy/parsers/structure/__init__.py
+-rw-r--r--   0        0        0      169 2022-11-21 19:39:10.949975 specifipy-0.2.1/specifipy/parsers/structure/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2751 2024-04-29 23:50:20.980382 specifipy-0.2.1/specifipy/parsers/structure/__pycache__/code_structure_definitions.cpython-310.pyc
+-rw-r--r--   0        0        0     1946 2024-04-29 14:16:50.909123 specifipy-0.2.1/specifipy/parsers/structure/code_structure_definitions.py
+-rw-r--r--   0        0        0      808 1970-01-01 00:00:00.000000 specifipy-0.2.1/setup.py
+-rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 specifipy-0.2.1/PKG-INFO
```

### Comparing `specifipy-0.2.0/LICENSE` & `specifipy-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `specifipy-0.2.0/specifipy/file_scanners/directory_scanner.py` & `specifipy-0.2.1/specifipy/file_scanners/directory_scanner.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import os
 
+from py_d2 import D2Diagram
+
+from specifipy.diagram_engines.hashable_connection import D2HashableConnection
 from specifipy.parsers.diagram_generator_d2 import DiagramGenerator
 
 
 class DirectoryScanner:
     scan_path: str = None
     full_dir_paths: list[str] = []
     full_file_paths: list[str] = []
@@ -50,20 +53,45 @@
         ]
 
         self.do_recursive_directory_scanning()
 
     def show_vars(self):
         print(self.full_dir_paths, self.full_file_paths)
 
-    def make_diagrams(self):
+    def make_diagrams(
+        self,
+        collect_files=True,
+        file_name_containers=False,
+        base_path: str | None = None,
+    ):
         diagram_generator = DiagramGenerator()
+        diagrams: list[D2Diagram] = []
         for f in self.full_file_paths:
             name = f.split("/")[-1]
             with open(f) as python_file:
-                diagram_generator.generate_diagram(python_file.read(), name)
+                diagram = diagram_generator.generate_diagram(
+                    python_file.read(),
+                    name,
+                    base_path=base_path,
+                    save_file=not collect_files,
+                    file_name_container=file_name_containers,
+                )
+                if collect_files and diagram:
+                    diagrams.append(diagram)
+        if diagrams:
+            classes = sum([diagram.shapes for diagram in diagrams], [])
+            connections = [
+                D2HashableConnection(x.shape_1, x.shape_2, x.label, x.direction)
+                for x in sum([diagram.connections for diagram in diagrams], [])
+            ]
+            diagram_generator.save_diagram_to_file(
+                base_path if base_path else "./",
+                D2Diagram(classes, list(set(connections))),
+                "code_diagrams",
+            )
 
     def do_recursive_directory_scanning(self):
         new_found_directory_paths: list[str] = []
         if self.full_dir_paths:
             directory_path: str
             for directory_path in self.full_dir_paths:
                 for file_system_element in os.listdir(directory_path):
```

### Comparing `specifipy-0.2.0/specifipy/parsers/__pycache__/generic_parser.cpython-310.pyc` & `specifipy-0.2.1/specifipy/parsers/__pycache__/generic_parser.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 28 19:07:19 2024 UTC, .py size: 4650 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 679e 2e66 2a12 0000  o.......g..f*...
+00000000: 6f0d 0d0a 0000 0000 1dac 2f66 c415 0000  o........./f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 4700  m.Z.m.Z.m.Z...G.
 00000060: 6404 6405 8400 6405 8302 5a09 6401 5300  d.d...d...Z.d.S.
 00000070: 2906 e900 0000 004e 2901 da0d 5061 7273  )......N)...Pars
@@ -52,134 +52,151 @@
 00000330: 6e63 65da 0652 6574 7572 6eda 0576 616c  nce..Return..val
 00000340: 7565 da0c 4e61 6d65 436f 6e73 7461 6e74  ue..NameConstant
 00000350: da09 416e 6e41 7373 6967 6eda 0a61 6e6e  ..AnnAssign..ann
 00000360: 6f74 6174 696f 6e29 0372 0b00 0000 720e  otation).r....r.
 00000370: 0000 00da 046e 6f64 6572 0a00 0000 720a  .....noder....r.
 00000380: 0000 0072 0c00 0000 da1a 6765 745f 7265  ...r......get_re
 00000390: 7475 726e 5f74 7970 655f 616e 6e6f 7461  turn_type_annota
-000003a0: 7469 6f6e 1100 0000 7314 0000 0006 020c  tion....s.......
-000003b0: 010e 030c 011a 0102 010e 0112 0102 8004  ................
-000003c0: 017a 2847 656e 6572 6963 5061 7273 6572  .z(GenericParser
-000003d0: 2e67 6574 5f72 6574 7572 6e5f 7479 7065  .get_return_type
-000003e0: 5f61 6e6e 6f74 6174 696f 6e72 1a00 0000  _annotationr....
-000003f0: da0e 7061 7273 696e 675f 7265 7375 6c74  ..parsing_result
-00000400: 6304 0000 0000 0000 0000 0000 000d 0000  c...............
-00000410: 000b 0000 0043 0000 0073 0202 0000 7400  .....C...s....t.
-00000420: 7c01 8301 0400 7401 6a02 6b02 7263 0100  |.....t.j.k.rc..
-00000430: 7c01 6a03 7d04 6401 7d05 7404 7c01 6a05  |.j.}.d.}.t.|.j.
-00000440: 8301 6402 6b04 723d 7406 7c01 6a05 6402  ..d.k.r=t.|.j.d.
-00000450: 1900 7401 6a07 8302 7224 7c01 6a05 6402  ..t.j...r$|.j.d.
-00000460: 1900 6a08 7d05 7406 7c01 6a05 6402 1900  ..j.}.t.|.j.d...
-00000470: 7401 6a09 8302 723d 7c01 6a05 6402 1900  t.j...r=|.j.d...
-00000480: 6a0a 6a08 9b00 6403 7c01 6a05 6402 1900  j.j...d.|.j.d...
-00000490: 6a0b 9b00 9d03 7d05 740c 740d 6a0e 7c04  j.....}.t.t.j.|.
-000004a0: 7c01 6a0f 7c01 6a10 7c05 8305 7d06 7c06  |.j.|.j.|...}.|.
-000004b0: 7c02 6a11 7601 7253 7c02 6a11 a012 7c06  |.j.v.rS|.j...|.
-000004c0: a101 0100 7c01 6a13 4400 5d0a 7d07 7c00  ....|.j.D.].}.|.
-000004d0: 6a14 7c07 7c02 7c06 6404 8d03 0100 7156  j.|.|.|.d.....qV
-000004e0: 6400 5300 0400 7401 6a15 6b02 729d 0100  d.S...t.j.k.r...
-000004f0: 7c01 6a03 7d04 7c01 6a16 7d08 6405 6406  |.j.}.|.j.}.d.d.
-00000500: 8400 7c08 6a16 4400 8301 7d09 7417 740d  ..|.j.D...}.t.t.
-00000510: 6a18 7c04 7c01 6a0f 7c01 6a10 7c09 7c03  j.|.|.j.|.j.|.|.
-00000520: 7285 7c03 6a03 6e01 6400 7419 7c00 a01a  r.|.j.n.d.t.|...
-00000530: 7c01 a101 8301 8307 7d0a 7c0a 7c02 6a1b  |.......}.|.|.j.
-00000540: 7601 729b 7c02 6a1b a012 7c0a a101 0100  v.r.|.j...|.....
-00000550: 6400 5300 6400 5300 0400 7401 6a1c 6b02  d.S.d.S...t.j.k.
-00000560: 72d7 0100 7406 7c03 740c 8302 72d3 7c03  r...t.|.t...r.|.
-00000570: 72d5 7c01 6a1d 6a08 7d04 7400 7c01 6a1e  r.|.j.j.}.t.|.j.
-00000580: 8301 7401 6a1f 6b02 73ba 7c01 6a1e 6a08  ..t.j.k.s.|.j.j.
-00000590: 6e04 7c01 6a1e 6a0a 6a08 7d0b 7420 740d  n.|.j.j.j.}.t t.
-000005a0: 6a21 7c04 7c01 6a0f 7c01 6a10 7c03 7c0b  j!|.|.j.|.j.|.|.
-000005b0: 8306 7d0c 7c02 6a22 a012 7c0c a101 0100  ..}.|.j"..|.....
-000005c0: 6400 5300 6400 5300 6400 5300 7401 6a23  d.S.d.S.d.S.t.j#
-000005d0: 6b02 72ff 7406 7c03 740c 8302 72fb 7c03  k.r.t.|.t...r.|.
-000005e0: 72fd 7c01 6a24 6402 1900 6a08 7d04 7425  r.|.j$d...j.}.t%
-000005f0: 740d 6a21 7c04 7c01 6a0f 7c01 6a10 7c03  t.j!|.|.j.|.j.|.
-00000600: 8305 7d0c 7c02 6a22 a012 7c0c a101 0100  ..}.|.j"..|.....
-00000610: 6400 5300 6400 5300 6400 5300 6400 5300  d.S.d.S.d.S.d.S.
-00000620: 2907 4eda 0072 0100 0000 da01 5f29 01da  ).N..r......_)..
-00000630: 0670 6172 656e 7463 0100 0000 0000 0000  .parentc........
-00000640: 0000 0000 0200 0000 0300 0000 5300 0000  ............S...
-00000650: 7312 0000 0067 007c 005d 057d 017c 016a  s....g.|.].}.|.j
-00000660: 0091 0271 0253 0072 0a00 0000 2901 da03  ...q.S.r....)...
-00000670: 6172 6729 02da 022e 30da 0178 720a 0000  arg)....0..xr...
-00000680: 0072 0a00 0000 720c 0000 00da 0a3c 6c69  .r....r......<li
-00000690: 7374 636f 6d70 3e41 0000 0073 0200 0000  stcomp>A...s....
-000006a0: 1200 7a31 4765 6e65 7269 6350 6172 7365  ..z1GenericParse
-000006b0: 722e 5f5f 636c 6173 7369 6679 5f6e 6f64  r.__classify_nod
-000006c0: 652e 3c6c 6f63 616c 733e 2e3c 6c69 7374  e.<locals>.<list
-000006d0: 636f 6d70 3e29 26da 0474 7970 6572 1100  comp>)&..typer..
-000006e0: 0000 da08 436c 6173 7344 6566 da04 6e61  ....ClassDef..na
-000006f0: 6d65 da03 6c65 6eda 0562 6173 6573 7214  me..len..basesr.
-00000700: 0000 00da 044e 616d 65da 0269 64da 0941  .....Name..id..A
-00000710: 7474 7269 6275 7465 7216 0000 00da 0461  ttributer......a
-00000720: 7474 7272 0300 0000 7206 0000 00da 0543  ttrr....r......C
-00000730: 4c41 5353 da06 6c69 6e65 6e6f da0a 656e  LASS..lineno..en
-00000740: 645f 6c69 6e65 6e6f da07 636c 6173 7365  d_lineno..classe
-00000750: 73da 0661 7070 656e 64da 0462 6f64 79da  s..append..body.
-00000760: 1d5f 4765 6e65 7269 6350 6172 7365 725f  ._GenericParser_
-00000770: 5f63 6c61 7373 6966 795f 6e6f 6465 da0b  _classify_node..
-00000780: 4675 6e63 7469 6f6e 4465 66da 0461 7267  FunctionDef..arg
-00000790: 7372 0400 0000 da08 4655 4e43 5449 4f4e  sr......FUNCTION
-000007a0: da03 7374 7272 1b00 0000 da09 6675 6e63  ..strr......func
-000007b0: 7469 6f6e 7372 1800 0000 da06 7461 7267  tionsr......targ
-000007c0: 6574 7219 0000 00da 0953 7562 7363 7269  etr......Subscri
-000007d0: 7074 7207 0000 00da 0b43 4c41 5353 5f46  ptr......CLASS_F
-000007e0: 4945 4c44 da0c 636c 6173 735f 6669 656c  IELD..class_fiel
-000007f0: 6473 da06 4173 7369 676e da07 7461 7267  ds..Assign..targ
-00000800: 6574 7372 0500 0000 290d 720b 0000 0072  etsr....).r....r
-00000810: 1a00 0000 721c 0000 0072 1f00 0000 7226  ....r....r....r&
-00000820: 0000 00da 0d69 6e68 6572 6974 735f 6672  .....inherits_fr
-00000830: 6f6d da10 636c 6173 735f 6465 6669 6e69  om..class_defini
-00000840: 7469 6f6e da08 7375 625f 6e6f 6465 da06  tion..sub_node..
-00000850: 7061 7261 6d73 da0d 7061 7261 6d73 5f73  params..params_s
-00000860: 7472 696e 67da 1366 756e 6374 696f 6e5f  tring..function_
-00000870: 6465 6669 6e69 7469 6f6e da0f 7479 7065  definition..type
-00000880: 5f61 6e6e 6f74 6174 696f 6eda 0566 6965  _annotation..fie
-00000890: 6c64 720a 0000 0072 0a00 0000 720c 0000  ldr....r....r...
-000008a0: 00da 0f5f 5f63 6c61 7373 6966 795f 6e6f  ...__classify_no
-000008b0: 6465 1f00 0000 738a 0000 0006 030c 0106  de....s.........
-000008c0: 0204 010e 0112 010c 0112 0120 0102 0204  ........... ....
-000008d0: 0102 0104 0104 0102 0104 fb0a 080c 010a  ................
-000008e0: 0204 0106 0108 ff04 ff0c 0506 0206 0110  ................
-000008f0: 0102 0104 0102 0104 0104 0102 010c 010c  ................
-00000900: 0104 f90a 0910 0104 ff0c 030e 0108 0210  ................
-00000910: 0308 ff08 0202 fd02 0504 0102 0104 0104  ................
-00000920: 0102 0102 0104 fa10 0808 f008 120e 010c  ................
-00000930: 0202 0104 0102 0104 0104 0102 0104 fb10  ................
-00000940: 0708 f604 ff7a 1d47 656e 6572 6963 5061  .....z.GenericPa
-00000950: 7273 6572 2e5f 5f63 6c61 7373 6966 795f  rser.__classify_
-00000960: 6e6f 6465 da18 736f 7572 6365 5f63 6f64  node..source_cod
-00000970: 655f 6669 6c65 5f63 6f6e 7465 6e74 6302  e_file_contentc.
-00000980: 0000 0000 0000 0000 0000 0005 0000 0005  ................
-00000990: 0000 0043 0000 0073 3600 0000 7400 a001  ...C...s6...t...
-000009a0: 7c01 a101 7d02 7402 6700 6700 6700 8303  |...}.t.g.g.g...
-000009b0: 7d03 7400 a003 7c02 a101 4400 5d08 7d04  }.t...|...D.].}.
-000009c0: 7c00 a004 7c04 7c03 a102 0100 7110 7c03  |...|.|.....q.|.
-000009d0: 5300 7209 0000 0029 0572 1100 0000 da05  S.r....).r......
-000009e0: 7061 7273 6572 0200 0000 7213 0000 0072  parser....r....r
-000009f0: 3300 0000 2905 720b 0000 0072 4800 0000  3...).r....rH...
-00000a00: da04 636f 6465 721c 0000 0072 1a00 0000  ..coder....r....
-00000a10: 720a 0000 0072 0a00 0000 720c 0000 0072  r....r....r....r
-00000a20: 4900 0000 6e00 0000 730a 0000 000a 010c  I...n...s.......
-00000a30: 010e 010e 0104 017a 1347 656e 6572 6963  .......z.Generic
-00000a40: 5061 7273 6572 2e70 6172 7365 7209 0000  Parser.parser...
-00000a50: 0029 0cda 085f 5f6e 616d 655f 5fda 0a5f  .)...__name__.._
-00000a60: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00000a70: 6c6e 616d 655f 5f72 0d00 0000 7211 0000  lname__r....r...
-00000a80: 0072 3400 0000 7237 0000 0072 1b00 0000  .r4...r7...r....
-00000a90: da03 4153 5472 0200 0000 7233 0000 0072  ..ASTr....r3...r
-00000aa0: 4900 0000 720a 0000 0072 0a00 0000 720a  I...r....r....r.
-00000ab0: 0000 0072 0c00 0000 7208 0000 000d 0000  ...r....r.......
-00000ac0: 0073 1800 0000 0800 0801 1803 020f 04ff  .s..............
-00000ad0: 0401 02ff 0201 02ff 0202 0afe 164f 7208  .............Or.
-00000ae0: 0000 0029 0a72 1100 0000 da19 7370 6563  ...).r......spec
-00000af0: 6966 6970 792e 7061 7273 6572 732e 7265  ifipy.parsers.re
-00000b00: 7375 6c74 7372 0200 0000 da36 7370 6563  sultsr.....6spec
-00000b10: 6966 6970 792e 7061 7273 6572 732e 7374  ifipy.parsers.st
-00000b20: 7275 6374 7572 652e 636f 6465 5f73 7472  ructure.code_str
-00000b30: 7563 7475 7265 5f64 6566 696e 6974 696f  ucture_definitio
-00000b40: 6e73 7203 0000 0072 0400 0000 7205 0000  nsr....r....r...
-00000b50: 0072 0600 0000 7207 0000 0072 0800 0000  .r....r....r....
-00000b60: 720a 0000 0072 0a00 0000 720a 0000 0072  r....r....r....r
-00000b70: 0c00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00000b80: 0000 7308 0000 0008 000c 021c 0112 09    ..s............
+000003a0: 7469 6f6e 1100 0000 7318 0000 0006 020c  tion....s.......
+000003b0: 010e 030c 010c 0202 ff0c 0202 020e 0112  ................
+000003c0: 0102 8004 017a 2847 656e 6572 6963 5061  .....z(GenericPa
+000003d0: 7273 6572 2e67 6574 5f72 6574 7572 6e5f  rser.get_return_
+000003e0: 7479 7065 5f61 6e6e 6f74 6174 696f 6e72  type_annotationr
+000003f0: 1a00 0000 da0e 7061 7273 696e 675f 7265  ......parsing_re
+00000400: 7375 6c74 6304 0000 0000 0000 0000 0000  sultc...........
+00000410: 000d 0000 000b 0000 0043 0000 0073 cc02  .........C...s..
+00000420: 0000 7400 7c01 8301 0400 7401 6a02 6b02  ..t.|.....t.j.k.
+00000430: 7274 0100 7c01 6a03 7d04 6401 7d05 7404  rt..|.j.}.d.}.t.
+00000440: 7c01 6a05 8301 6402 6b04 724e 7406 7c01  |.j...d.k.rNt.|.
+00000450: 6a05 6402 1900 7401 6a07 8302 7224 7c01  j.d...t.j...r$|.
+00000460: 6a05 6402 1900 6a08 7d05 7406 7c01 6a05  j.d...j.}.t.|.j.
+00000470: 6402 1900 7401 6a09 8302 724e 740a 7c01  d...t.j...rNt.|.
+00000480: 6a05 6402 1900 6a0b 6403 8302 723d 7c01  j.d...j.d...r=|.
+00000490: 6a05 6402 1900 6a0b 6a08 6e07 7c01 6a05  j.d...j.j.n.|.j.
+000004a0: 6402 1900 6a0b 6a0b 6a08 9b00 6404 7c01  d...j.j.j...d.|.
+000004b0: 6a05 6402 1900 6a0c 9b00 9d03 7d05 740d  j.d...j.....}.t.
+000004c0: 740e 6a0f 7c04 7c01 6a10 7c01 6a11 7c05  t.j.|.|.j.|.j.|.
+000004d0: 8305 7d06 7c06 7c02 6a12 7601 7264 7c02  ..}.|.|.j.v.rd|.
+000004e0: 6a12 a013 7c06 a101 0100 7c01 6a14 4400  j...|.....|.j.D.
+000004f0: 5d0a 7d07 7c00 6a15 7c07 7c02 7c06 6405  ].}.|.j.|.|.|.d.
+00000500: 8d03 0100 7167 6400 5300 0400 7401 6a16  ....qgd.S...t.j.
+00000510: 6b02 72ae 0100 7c01 6a03 7d04 7c01 6a17  k.r...|.j.}.|.j.
+00000520: 7d08 6406 6407 8400 7c08 6a17 4400 8301  }.d.d...|.j.D...
+00000530: 7d09 7418 740e 6a19 7c04 7c01 6a10 7c01  }.t.t.j.|.|.j.|.
+00000540: 6a11 7c09 7c03 7296 7c03 6a03 6e01 6400  j.|.|.r.|.j.n.d.
+00000550: 741a 7c00 a01b 7c01 a101 8301 8307 7d0a  t.|...|.......}.
+00000560: 7c0a 7c02 6a1c 7601 72ac 7c02 6a1c a013  |.|.j.v.r.|.j...
+00000570: 7c0a a101 0100 6400 5300 6400 5300 0400  |.....d.S.d.S...
+00000580: 7401 6a1d 6b02 9001 7218 0100 7406 7c03  t.j.k...r...t.|.
+00000590: 740d 8302 9001 7214 7c03 9001 7216 7c01  t.....r.|...r.|.
+000005a0: 6a1e 6a08 7d04 7406 7c01 6a1f 7401 6a09  j.j.}.t.|.j.t.j.
+000005b0: 7401 6a20 7401 6a21 7401 6a22 6604 8302  t.j t.j!t.j"f...
+000005c0: 73d4 7c01 6a1f 6a08 6e2b 7406 7c01 6a1f  s.|.j.j.n+t.|.j.
+000005d0: 7401 6a09 8302 72df 7c01 6a1f 6a0c 6e20  t.j...r.|.j.j.n 
+000005e0: 7406 7c01 6a1f 7401 6a20 8302 72ed 7401  t.|.j.t.j ..r.t.
+000005f0: a023 7c01 6a1f 6a24 a101 6e12 7406 7c01  .#|.j.j$..n.t.|.
+00000600: 6a1f 7401 6a21 8302 72fa 7401 a023 7c01  j.t.j!..r.t..#|.
+00000610: 6a1f a101 6e05 7401 a023 7c01 6a1f a101  j...n.t..#|.j...
+00000620: 7d0b 7425 740e 6a26 7c04 7c01 6a10 7c01  }.t%t.j&|.|.j.|.
+00000630: 6a11 7c03 7c0b 8306 7d0c 7c02 6a27 a013  j.|.|...}.|.j'..
+00000640: 7c0c a101 0100 6400 5300 6400 5300 6400  |.....d.S.d.S.d.
+00000650: 5300 7401 6a28 6b02 9001 7264 7406 7c03  S.t.j(k...rdt.|.
+00000660: 740d 8302 9001 7260 7c03 9001 7262 7406  t.....r`|...rbt.
+00000670: 7c01 6a29 6402 1900 7401 6a07 8302 9001  |.j)d...t.j.....
+00000680: 7236 7c01 6a29 6402 1900 6a08 6e16 7406  r6|.j)d...j.n.t.
+00000690: 7c01 6a29 6402 1900 7401 6a09 8302 9001  |.j)d...t.j.....
+000006a0: 7246 7c01 6a29 6402 1900 6a0c 6e06 741a  rF|.j)d...j.n.t.
+000006b0: 7c01 6a29 6402 1900 8301 7d04 742a 740e  |.j)d.....}.t*t.
+000006c0: 6a26 7c04 7c01 6a10 7c01 6a11 7c03 8305  j&|.|.j.|.j.|...
+000006d0: 7d0c 7c02 6a27 a013 7c0c a101 0100 6400  }.|.j'..|.....d.
+000006e0: 5300 6400 5300 6400 5300 6400 5300 2908  S.d.S.d.S.d.S.).
+000006f0: 4eda 0072 0100 0000 da02 6964 da01 5f29  N..r......id.._)
+00000700: 01da 0670 6172 656e 7463 0100 0000 0000  ...parentc......
+00000710: 0000 0000 0000 0200 0000 0300 0000 5300  ..............S.
+00000720: 0000 7312 0000 0067 007c 005d 057d 017c  ..s....g.|.].}.|
+00000730: 016a 0091 0271 0253 0072 0a00 0000 2901  .j...q.S.r....).
+00000740: da03 6172 6729 02da 022e 30da 0178 720a  ..arg)....0..xr.
+00000750: 0000 0072 0a00 0000 720c 0000 00da 0a3c  ...r....r......<
+00000760: 6c69 7374 636f 6d70 3e44 0000 0073 0200  listcomp>D...s..
+00000770: 0000 1200 7a31 4765 6e65 7269 6350 6172  ....z1GenericPar
+00000780: 7365 722e 5f5f 636c 6173 7369 6679 5f6e  ser.__classify_n
+00000790: 6f64 652e 3c6c 6f63 616c 733e 2e3c 6c69  ode.<locals>.<li
+000007a0: 7374 636f 6d70 3e29 2bda 0474 7970 6572  stcomp>)+..typer
+000007b0: 1100 0000 da08 436c 6173 7344 6566 da04  ......ClassDef..
+000007c0: 6e61 6d65 da03 6c65 6eda 0562 6173 6573  name..len..bases
+000007d0: 7214 0000 00da 044e 616d 6572 1e00 0000  r......Namer....
+000007e0: da09 4174 7472 6962 7574 65da 0768 6173  ..Attribute..has
+000007f0: 6174 7472 7216 0000 00da 0461 7474 7272  attrr......attrr
+00000800: 0300 0000 7206 0000 00da 0543 4c41 5353  ....r......CLASS
+00000810: da06 6c69 6e65 6e6f da0a 656e 645f 6c69  ..lineno..end_li
+00000820: 6e65 6e6f da07 636c 6173 7365 73da 0661  neno..classes..a
+00000830: 7070 656e 64da 0462 6f64 79da 1d5f 4765  ppend..body.._Ge
+00000840: 6e65 7269 6350 6172 7365 725f 5f63 6c61  nericParser__cla
+00000850: 7373 6966 795f 6e6f 6465 da0b 4675 6e63  ssify_node..Func
+00000860: 7469 6f6e 4465 66da 0461 7267 7372 0400  tionDef..argsr..
+00000870: 0000 da08 4655 4e43 5449 4f4e da03 7374  ....FUNCTION..st
+00000880: 7272 1b00 0000 da09 6675 6e63 7469 6f6e  rr......function
+00000890: 7372 1800 0000 da06 7461 7267 6574 7219  sr......targetr.
+000008a0: 0000 00da 0953 7562 7363 7269 7074 da05  .....Subscript..
+000008b0: 4269 6e4f 70da 0443 616c 6c72 1200 0000  BinOp..Callr....
+000008c0: da05 736c 6963 6572 0700 0000 da0b 434c  ..slicer......CL
+000008d0: 4153 535f 4649 454c 44da 0c63 6c61 7373  ASS_FIELD..class
+000008e0: 5f66 6965 6c64 73da 0641 7373 6967 6eda  _fields..Assign.
+000008f0: 0774 6172 6765 7473 7205 0000 0029 0d72  .targetsr....).r
+00000900: 0b00 0000 721a 0000 0072 1c00 0000 7220  ....r....r....r 
+00000910: 0000 0072 2700 0000 da0d 696e 6865 7269  ...r'.....inheri
+00000920: 7473 5f66 726f 6dda 1063 6c61 7373 5f64  ts_from..class_d
+00000930: 6566 696e 6974 696f 6eda 0873 7562 5f6e  efinition..sub_n
+00000940: 6f64 65da 0670 6172 616d 73da 0d70 6172  ode..params..par
+00000950: 616d 735f 7374 7269 6e67 da13 6675 6e63  ams_string..func
+00000960: 7469 6f6e 5f64 6566 696e 6974 696f 6eda  tion_definition.
+00000970: 0f74 7970 655f 616e 6e6f 7461 7469 6f6e  .type_annotation
+00000980: da05 6669 656c 6472 0a00 0000 720a 0000  ..fieldr....r...
+00000990: 0072 0c00 0000 da0f 5f5f 636c 6173 7369  .r......__classi
+000009a0: 6679 5f6e 6f64 6522 0000 0073 a600 0000  fy_node"...s....
+000009b0: 0603 0c01 0602 0401 0e01 1201 0c01 1201  ................
+000009c0: 4201 0202 0401 0201 0401 0401 0201 04fb  B...............
+000009d0: 0a08 0c01 0a02 0401 0601 08ff 04ff 0c05  ................
+000009e0: 0602 0601 1001 0201 0401 0201 0401 0401  ................
+000009f0: 0201 0c01 0c01 04f9 0a09 1001 04ff 0e03  ................
+00000a00: 1201 0802 0203 0401 1201 02fe 0aff 0c06  ................
+00000a10: 0aff 0c03 10ff 0c03 0eff 0a02 02f4 020e  ................
+00000a20: 0401 0201 0401 0401 0201 0201 04fa 1008  ................
+00000a30: 08e7 0a1b 1201 1004 10ff 1003 10ff 0c02  ................
+00000a40: 02fb 0207 0401 0201 0401 0401 0201 04fb  ................
+00000a50: 1007 08f0 04ff 7a1d 4765 6e65 7269 6350  ......z.GenericP
+00000a60: 6172 7365 722e 5f5f 636c 6173 7369 6679  arser.__classify
+00000a70: 5f6e 6f64 65da 1873 6f75 7263 655f 636f  _node..source_co
+00000a80: 6465 5f66 696c 655f 636f 6e74 656e 7463  de_file_contentc
+00000a90: 0200 0000 0000 0000 0000 0000 0500 0000  ................
+00000aa0: 0500 0000 4300 0000 7336 0000 0074 00a0  ....C...s6...t..
+00000ab0: 017c 01a1 017d 0274 0267 0067 0067 0083  .|...}.t.g.g.g..
+00000ac0: 037d 0374 00a0 037c 02a1 0144 005d 087d  .}.t...|...D.].}
+00000ad0: 047c 00a0 047c 047c 03a1 0201 0071 107c  .|...|.|.....q.|
+00000ae0: 0353 0072 0900 0000 2905 7211 0000 00da  .S.r....).r.....
+00000af0: 0570 6172 7365 7202 0000 0072 1300 0000  .parser....r....
+00000b00: 7234 0000 0029 0572 0b00 0000 724c 0000  r4...).r....rL..
+00000b10: 00da 0463 6f64 6572 1c00 0000 721a 0000  ...coder....r...
+00000b20: 0072 0a00 0000 720a 0000 0072 0c00 0000  .r....r....r....
+00000b30: 724d 0000 0080 0000 0073 0a00 0000 0a01  rM.......s......
+00000b40: 0c01 0e01 0e01 0401 7a13 4765 6e65 7269  ........z.Generi
+00000b50: 6350 6172 7365 722e 7061 7273 6572 0900  cParser.parser..
+00000b60: 0000 290c da08 5f5f 6e61 6d65 5f5f da0a  ..)...__name__..
+00000b70: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00000b80: 616c 6e61 6d65 5f5f 720d 0000 0072 1100  alname__r....r..
+00000b90: 0000 7235 0000 0072 3800 0000 721b 0000  ..r5...r8...r...
+00000ba0: 00da 0341 5354 7202 0000 0072 3400 0000  ...ASTr....r4...
+00000bb0: 724d 0000 0072 0a00 0000 720a 0000 0072  rM...r....r....r
+00000bc0: 0a00 0000 720c 0000 0072 0800 0000 0d00  ....r....r......
+00000bd0: 0000 7318 0000 0008 0008 0118 0302 1204  ..s.............
+00000be0: ff04 0102 ff02 0102 ff02 020a fe16 5e72  ..............^r
+00000bf0: 0800 0000 290a 7211 0000 00da 1973 7065  ....).r......spe
+00000c00: 6369 6669 7079 2e70 6172 7365 7273 2e72  cifipy.parsers.r
+00000c10: 6573 756c 7473 7202 0000 00da 3673 7065  esultsr.....6spe
+00000c20: 6369 6669 7079 2e70 6172 7365 7273 2e73  cifipy.parsers.s
+00000c30: 7472 7563 7475 7265 2e63 6f64 655f 7374  tructure.code_st
+00000c40: 7275 6374 7572 655f 6465 6669 6e69 7469  ructure_definiti
+00000c50: 6f6e 7372 0300 0000 7204 0000 0072 0500  onsr....r....r..
+00000c60: 0000 7206 0000 0072 0700 0000 7208 0000  ..r....r....r...
+00000c70: 0072 0a00 0000 720a 0000 0072 0a00 0000  .r....r....r....
+00000c80: 720c 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000c90: 0000 0073 0800 0000 0800 0c02 1c01 1209  ...s............
```

### Comparing `specifipy-0.2.0/specifipy/parsers/__pycache__/results.cpython-310.pyc` & `specifipy-0.2.1/specifipy/parsers/__pycache__/results.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `specifipy-0.2.0/specifipy/parsers/diagram_generator_d2.py` & `specifipy-0.2.1/specifipy/parsers/diagram_generator_d2.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from specifipy.parsers.generic_parser import GenericParser
 from specifipy.parsers.results import ParsingResult
 from specifipy.parsers.structure.code_structure_definitions import (
     ClassStructureDefinition,
     FieldStructureDefinition,
     FunctionStructureDefinition,
+    StructureEnum,
     TypeAnnotatedFieldStructureDefinition,
 )
 
 
 class DiagramGenerator(GenericParser):
     def __generate_class_definition_d2(
         self,
@@ -27,68 +28,107 @@
 
     def __generate_field_definition_d2(
         self, class_function_element: FieldStructureDefinition
     ) -> D2Shape:
         if isinstance(class_function_element, TypeAnnotatedFieldStructureDefinition):
             result_shape = D2Shape(
                 name=class_function_element.name,
-                label=f"'{class_function_element.type_annotation}'",
+                label=f"'{class_function_element.type_annotation}'"
+                if not "'" in class_function_element.type_annotation
+                else f'"{class_function_element.type_annotation}"',
             )
         else:
             result_shape = D2Shape(name=class_function_element.name)
 
         return result_shape
 
     def __generate_class_function_definition_d2(
         self, method_element: FunctionStructureDefinition
     ) -> D2Shape:
         if method_element.return_type:
             result_shape = D2Shape(
                 name=f"{method_element.name}({', '.join([x for x in method_element.params])})",
-                label=f"'{method_element.return_type}'",
+                label=f"'{method_element.return_type}'"
+                if not "'" in method_element.return_type
+                else f'"{method_element.return_type}"',
             )
         else:
             result_shape = D2Shape(
                 name=f"{method_element.name}({', '.join([x for x in method_element.params])})"
             )
         return result_shape
 
     def generate_diagram(
-        self, source_file_content: str, source_file_name: str, base_path: str = None
-    ):
+        self,
+        source_file_content: str,
+        source_file_name: str,
+        base_path: str = None,
+        save_file: bool = True,
+        file_name_container=False,
+    ) -> D2Diagram | None:
         parsing_result: ParsingResult = self.parse(source_file_content)
-        elements_to_generate = []
-        link_to_generate = []
+        elements_to_generate: list[D2Shape] = []
+        link_to_generate: list[D2Connection] = []
 
         class_element: ClassStructureDefinition
         for class_element in parsing_result.classes:
             class_functions = [
                 self.__generate_class_function_definition_d2(x)
                 for x in parsing_result.functions
                 if x.parent_class == class_element.name
             ]
             class_fields = [
                 self.__generate_field_definition_d2(x)
                 for x in parsing_result.class_fields
                 if x.parent_class == class_element
             ]
+            if file_name_container:
+                class_element.name = (
+                    f'{source_file_name.replace(".", "-")}.{class_element.name}'
+                )
             elements_to_generate.append(
                 self.__generate_class_definition_d2(
                     class_element, fields=class_fields, methods=class_functions
                 )
             )
             if class_element.inherits_from:
+                if file_name_container:
+                    class_element.inherits_from = f'{source_file_name.replace(".", "-")}.{class_element.inherits_from}'
                 link_to_generate.append(
                     D2Connection(
                         shape_1=class_element.name, shape_2=class_element.inherits_from
                     )
                 )
+        self.add_missing_elements_from_links_as_classes(
+            elements_to_generate, link_to_generate
+        )
         diagram = D2Diagram(shapes=elements_to_generate, connections=link_to_generate)
-        print(f"{source_file_name}, diagram '{diagram}'")
         if str(diagram) is not None and str(diagram) != "":
-            with open(
-                f"{base_path if base_path else ''}{source_file_name}.d2",
-                "w",
-                encoding="utf-8",
-            ) as output_file:
-                output_file.write("direction: up\n")
-                output_file.write(str(diagram))
+            if save_file:
+                self.save_diagram_to_file(base_path, diagram, source_file_name)
+            return diagram
+
+    def add_missing_elements_from_links_as_classes(
+        self, elements_to_generate, link_to_generate
+    ):
+        missing_elements = set([link.shape_2 for link in link_to_generate]) - set(
+            [element.name for element in elements_to_generate]
+        )
+        elements_to_generate.extend(
+            [
+                self.__generate_class_definition_d2(
+                    ClassStructureDefinition(
+                        StructureEnum.CLASS, missing_element, 0, 0, None
+                    )
+                )
+                for missing_element in missing_elements
+            ]
+        )
+
+    def save_diagram_to_file(self, base_path, diagram, source_file_name):
+        with open(
+            f"{base_path if base_path else ''}{source_file_name}.d2",
+            "w",
+            encoding="utf-8",
+        ) as output_file:
+            output_file.write("direction: up\n")
+            output_file.write(str(diagram))
```

### Comparing `specifipy-0.2.0/specifipy/parsers/generic_parser.py` & `specifipy-0.2.1/specifipy/parsers/generic_parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                 node: ast.ClassDef
                 name: str = node.name
                 inherits_from = ""
                 if len(node.bases) > 0:
                     if isinstance(node.bases[0], ast.Name):
                         inherits_from = node.bases[0].id
                     if isinstance(node.bases[0], ast.Attribute):
-                        inherits_from = f"{node.bases[0].value.id}_{node.bases[0].attr}"
+                        inherits_from = f"{node.bases[0].value.id if hasattr(node.bases[0].value, 'id') else node.bases[0].value.value.id}_{node.bases[0].attr}"
 
                 class_definition = ClassStructureDefinition(
                     StructureEnum.CLASS,
                     name,
                     node.lineno,
                     node.end_lineno,
                     inherits_from,
@@ -80,31 +80,46 @@
 
             case ast.AnnAssign:
                 if isinstance(parent, ClassStructureDefinition) and parent:
                     node: ast.AnnAssign
                     name: str = node.target.id
                     type_annotation: str = (
                         node.annotation.id
-                        if not type(node.annotation) == ast.Subscript
-                        else node.annotation.value.id
+                        if not isinstance(
+                            node.annotation,
+                            (ast.Attribute, ast.Subscript, ast.BinOp, ast.Call),
+                        )
+                        else node.annotation.attr
+                        if isinstance(node.annotation, ast.Attribute)
+                        else ast.unparse(node.annotation.slice)
+                        if isinstance(node.annotation, ast.Subscript)
+                        else ast.unparse(node.annotation)
+                        if isinstance(node.annotation, ast.BinOp)
+                        else ast.unparse(node.annotation)
                     )
                     field = TypeAnnotatedFieldStructureDefinition(
                         StructureEnum.CLASS_FIELD,
                         name,
                         node.lineno,
                         node.end_lineno,
                         parent,
                         type_annotation,
                     )
                     parsing_result.class_fields.append(field)
 
             case ast.Assign:
                 if isinstance(parent, ClassStructureDefinition) and parent:
                     node: ast.Assign
-                    name: str = node.targets[0].id
+                    name: str = (
+                        node.targets[0].id
+                        if isinstance(node.targets[0], ast.Name)
+                        else node.targets[0].attr
+                        if isinstance(node.targets[0], ast.Attribute)
+                        else str(node.targets[0])
+                    )
                     field = NotTypeAnnotatedFieldStructureDefinition(
                         StructureEnum.CLASS_FIELD,
                         name,
                         node.lineno,
                         node.end_lineno,
                         parent,
                     )
```

### Comparing `specifipy-0.2.0/specifipy/parsers/structure/__pycache__/code_structure_definitions.cpython-310.pyc` & `specifipy-0.2.1/specifipy/parsers/structure/__pycache__/code_structure_definitions.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 28 18:51:56 2024 UTC, .py size: 1368 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 cc9a 2e66 5805 0000  o..........fX...
+00000000: 6f0d 0d0a 0000 0000 d2ab 2f66 9a07 0000  o........./f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 cc00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6403 6404 8400 6404 6502 8303  ..G.d.d...d.e...
 00000050: 5a03 4700 6405 6406 8400 6406 8302 5a04  Z.G.d.d...d...Z.
 00000060: 6500 6a05 4700 6407 6408 8400 6408 8302  e.j.G.d.d...d...
 00000070: 8301 5a06 6500 6a05 4700 6409 640a 8400  ..Z.e.j.G.d.d...
@@ -50,93 +50,123 @@
 00000310: 0000 0065 005a 0164 005a 0255 0065 0365  ...e.Z.d.Z.U.e.e
 00000320: 0464 013c 0064 0253 0029 03da 0944 6f63  .d.<.d.S.)...Doc
 00000330: 7374 7269 6e67 da0b 6465 7363 7269 7074  string..descript
 00000340: 696f 6e4e 7214 0000 0072 0f00 0000 720f  ionNr....r....r.
 00000350: 0000 0072 0f00 0000 7210 0000 0072 1800  ...r....r....r..
 00000360: 0000 1100 0000 f304 0000 000a 000c 0272  ...............r
 00000370: 1800 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00000380: 0000 0000 0003 0000 0040 0000 0073 2e00  .........@...s..
+00000380: 0000 0000 0003 0000 0040 0000 0073 4600  .........@...sF.
 00000390: 0000 6500 5a01 6400 5a02 5500 6503 6504  ..e.Z.d.Z.U.e.e.
 000003a0: 6401 3c00 6505 6504 6402 3c00 6506 6504  d.<.e.e.d.<.e.e.
-000003b0: 6403 3c00 6506 6504 6404 3c00 6405 5300  d.<.e.e.d.<.d.S.
-000003c0: 2906 da13 5374 7275 6374 7572 6544 6566  )...StructureDef
-000003d0: 696e 6974 696f 6eda 0e73 7472 7563 7475  inition..structu
-000003e0: 7265 5f74 7970 6572 1200 0000 da0a 7374  re_typer......st
-000003f0: 6172 745f 6c69 6e65 da08 656e 645f 6c69  art_line..end_li
-00000400: 6e65 4e29 0772 0800 0000 7209 0000 0072  neN).r....r....r
-00000410: 0a00 0000 7203 0000 0072 1600 0000 7215  ....r....r....r.
-00000420: 0000 00da 0369 6e74 720f 0000 0072 0f00  .....intr....r..
-00000430: 0000 720f 0000 0072 1000 0000 721b 0000  ..r....r....r...
-00000440: 0016 0000 0073 0a00 0000 0a00 0802 0801  .....s..........
-00000450: 0801 0c01 721b 0000 0063 0000 0000 0000  ....r....c......
-00000460: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
-00000470: 0000 7217 0000 0029 03da 1843 6c61 7373  ..r....)...Class
-00000480: 5374 7275 6374 7572 6544 6566 696e 6974  StructureDefinit
-00000490: 696f 6eda 0d69 6e68 6572 6974 735f 6672  ion..inherits_fr
-000004a0: 6f6d 4e72 1400 0000 720f 0000 0072 0f00  omNr....r....r..
-000004b0: 0000 720f 0000 0072 1000 0000 7220 0000  ..r....r....r ..
-000004c0: 001e 0000 0072 1a00 0000 7220 0000 0063  .....r....r ...c
-000004d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000004e0: 0300 0000 4000 0000 7336 0000 0065 005a  ....@...s6...e.Z
-000004f0: 0164 005a 0255 0065 0365 0419 0065 0564  .d.Z.U.e.e...e.d
-00000500: 013c 0065 0665 0564 023c 0064 035a 0765  .<.e.e.d.<.d.Z.e
-00000510: 0465 0564 043c 0064 0564 0684 005a 0864  .e.d.<.d.d...Z.d
-00000520: 0353 0029 07da 1b46 756e 6374 696f 6e53  .S.)...FunctionS
-00000530: 7472 7563 7475 7265 4465 6669 6e69 7469  tructureDefiniti
-00000540: 6f6e da06 7061 7261 6d73 da0c 7061 7265  on..params..pare
-00000550: 6e74 5f63 6c61 7373 4eda 0b72 6574 7572  nt_classN..retur
-00000560: 6e5f 7479 7065 6302 0000 0000 0000 0000  n_typec.........
-00000570: 0000 0002 0000 0006 0000 0043 0000 0073  ...........C...s
-00000580: 3000 0000 7c00 6a00 7c00 6a01 7c00 6a02  0...|.j.|.j.|.j.
-00000590: 7c00 6a03 7c00 6a04 6605 7c01 6a00 7c01  |.j.|.j.f.|.j.|.
-000005a0: 6a01 7c01 6a02 7c01 6a03 7c01 6a04 6605  j.|.j.|.j.|.j.f.
-000005b0: 6b02 5300 2901 4e29 0572 1200 0000 7223  k.S.).N).r....r#
-000005c0: 0000 0072 1d00 0000 721e 0000 0072 1c00  ...r....r....r..
-000005d0: 0000 2902 da04 7365 6c66 da05 6f74 6865  ..)...self..othe
-000005e0: 7272 0f00 0000 720f 0000 0072 1000 0000  rr....r....r....
-000005f0: da06 5f5f 6571 5f5f 2900 0000 731a 0000  ..__eq__)...s...
-00000600: 0004 0204 0104 0104 0104 0102 fb04 0704  ................
-00000610: 0104 0104 0104 0102 fb04 fa7a 2246 756e  ...........z"Fun
-00000620: 6374 696f 6e53 7472 7563 7475 7265 4465  ctionStructureDe
-00000630: 6669 6e69 7469 6f6e 2e5f 5f65 715f 5f29  finition.__eq__)
-00000640: 0972 0800 0000 7209 0000 0072 0a00 0000  .r....r....r....
-00000650: da04 6c69 7374 7215 0000 0072 1600 0000  ..listr....r....
-00000660: 7220 0000 0072 2500 0000 7228 0000 0072  r ...r%...r(...r
-00000670: 0f00 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
-00000680: 0000 0072 2200 0000 2300 0000 730a 0000  ...r"...#...s...
-00000690: 000a 000c 0208 010c 010c 0272 2200 0000  ...........r"...
-000006a0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-000006b0: 0003 0000 0040 0000 0072 1700 0000 2903  .....@...r....).
-000006c0: da18 4669 656c 6453 7472 7563 7475 7265  ..FieldStructure
-000006d0: 4465 6669 6e69 7469 6f6e 7224 0000 004e  Definitionr$...N
-000006e0: 2905 7208 0000 0072 0900 0000 720a 0000  ).r....r....r...
-000006f0: 0072 2000 0000 7216 0000 0072 0f00 0000  .r ...r....r....
-00000700: 720f 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
-00000710: 2a00 0000 3900 0000 721a 0000 0072 2a00  *...9...r....r*.
-00000720: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000730: 0000 0003 0000 0040 0000 0072 1700 0000  .......@...r....
-00000740: 2903 da25 5479 7065 416e 6e6f 7461 7465  )..%TypeAnnotate
-00000750: 6446 6965 6c64 5374 7275 6374 7572 6544  dFieldStructureD
-00000760: 6566 696e 6974 696f 6eda 0f74 7970 655f  efinition..type_
-00000770: 616e 6e6f 7461 7469 6f6e 4e72 1400 0000  annotationNr....
-00000780: 720f 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
-00000790: 1000 0000 722b 0000 003e 0000 0072 1a00  ....r+...>...r..
-000007a0: 0000 722b 0000 0063 0000 0000 0000 0000  ..r+...c........
-000007b0: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
-000007c0: 730c 0000 0065 005a 0164 005a 0264 0153  s....e.Z.d.Z.d.S
-000007d0: 0029 02da 284e 6f74 5479 7065 416e 6e6f  .)..(NotTypeAnno
-000007e0: 7461 7465 6446 6965 6c64 5374 7275 6374  tatedFieldStruct
-000007f0: 7572 6544 6566 696e 6974 696f 6e4e 2903  ureDefinitionN).
-00000800: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
-00000810: 0f00 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
-00000820: 0000 0072 2d00 0000 4300 0000 7304 0000  ...r-...C...s...
-00000830: 0008 0004 0272 2d00 0000 290d da0b 6461  .....r-...)...da
-00000840: 7461 636c 6173 7365 73da 0465 6e75 6d72  taclasses..enumr
-00000850: 0200 0000 7203 0000 0072 1100 0000 da09  ....r....r......
-00000860: 6461 7461 636c 6173 7372 1800 0000 721b  dataclassr....r.
-00000870: 0000 0072 2000 0000 7222 0000 0072 2a00  ...r ...r"...r*.
-00000880: 0000 722b 0000 0072 2d00 0000 720f 0000  ..r+...r-...r...
-00000890: 0072 0f00 0000 720f 0000 0072 1000 0000  .r....r....r....
-000008a0: da08 3c6d 6f64 756c 653e 0100 0000 7324  ..<module>....s$
-000008b0: 0000 0008 000c 0110 030e 0704 0510 0104  ................
-000008c0: 0410 0104 0712 0104 0412 0104 1512 0104  ................
-000008d0: 0412 0104 0416 01                        .......
+000003b0: 6403 3c00 6506 6504 6404 3c00 6700 6405  d.<.e.e.d.<.g.d.
+000003c0: a201 5a07 6406 6407 8400 5a08 6408 6409  ..Z.d.d...Z.d.d.
+000003d0: 8400 5a09 640a 5300 290b da13 5374 7275  ..Z.d.S.)...Stru
+000003e0: 6374 7572 6544 6566 696e 6974 696f 6eda  ctureDefinition.
+000003f0: 0e73 7472 7563 7475 7265 5f74 7970 6572  .structure_typer
+00000400: 1200 0000 da0a 7374 6172 745f 6c69 6e65  ......start_line
+00000410: da08 656e 645f 6c69 6e65 2909 da05 6c61  ..end_line)...la
+00000420: 6265 6cda 0563 6c61 7373 da07 636c 6173  bel..class..clas
+00000430: 7365 73da 0573 7479 6c65 da05 7368 6170  ses..style..shap
+00000440: 65da 0964 6972 6563 7469 6f6e da05 7769  e..direction..wi
+00000450: 6474 68da 0668 6569 6768 74da 046c 696e  dth..height..lin
+00000460: 6b63 0100 0000 0000 0000 0000 0000 0200  kc..............
+00000470: 0000 0200 0000 4300 0000 7328 0000 0064  ......C...s(...d
+00000480: 017d 017c 006a 00a0 01a1 007c 006a 0276  .}.|.j.....|.j.v
+00000490: 0072 127c 006a 007c 0117 007c 005f 0064  .r.|.j.|...|._.d
+000004a0: 0053 0064 0053 0029 024e 7503 0000 00e2  .S.d.S.).Nu.....
+000004b0: a080 2903 7212 0000 00da 056c 6f77 6572  ..).r......lower
+000004c0: da14 6432 5f72 6573 6572 7665 645f 6b65  ..d2_reserved_ke
+000004d0: 7977 6f72 6473 2902 da04 7365 6c66 da13  ywords)...self..
+000004e0: 6b65 7977 6f72 645f 6573 6361 7065 5f63  keyword_escape_c
+000004f0: 6861 7272 0f00 0000 720f 0000 0072 1000  harr....r....r..
+00000500: 0000 da11 7361 6e69 7469 7a65 5f64 325f  ....sanitize_d2_
+00000510: 6e61 6d65 732b 0000 0073 0800 0000 0401  names+...s......
+00000520: 1001 1001 04ff 7a25 5374 7275 6374 7572  ......z%Structur
+00000530: 6544 6566 696e 6974 696f 6e2e 7361 6e69  eDefinition.sani
+00000540: 7469 7a65 5f64 325f 6e61 6d65 7363 0100  tize_d2_namesc..
+00000550: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00000560: 0000 4300 0000 730c 0000 007c 00a0 00a1  ..C...s....|....
+00000570: 0001 0064 0053 00a9 014e 2901 722c 0000  ...d.S...N).r,..
+00000580: 0029 0172 2a00 0000 720f 0000 0072 0f00  .).r*...r....r..
+00000590: 0000 7210 0000 00da 0d5f 5f70 6f73 745f  ..r......__post_
+000005a0: 696e 6974 5f5f 3000 0000 7302 0000 000c  init__0...s.....
+000005b0: 017a 2153 7472 7563 7475 7265 4465 6669  .z!StructureDefi
+000005c0: 6e69 7469 6f6e 2e5f 5f70 6f73 745f 696e  nition.__post_in
+000005d0: 6974 5f5f 4e29 0a72 0800 0000 7209 0000  it__N).r....r...
+000005e0: 0072 0a00 0000 7203 0000 0072 1600 0000  .r....r....r....
+000005f0: 7215 0000 00da 0369 6e74 7229 0000 0072  r......intr)...r
+00000600: 2c00 0000 722e 0000 0072 0f00 0000 720f  ,...r....r....r.
+00000610: 0000 0072 0f00 0000 7210 0000 0072 1b00  ...r....r....r..
+00000620: 0000 1600 0000 7310 0000 000a 0008 0208  ......s.........
+00000630: 0108 0108 0108 0308 0d0c 0572 1b00 0000  ...........r....
+00000640: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000650: 0003 0000 0040 0000 0072 1700 0000 2903  .....@...r....).
+00000660: da18 436c 6173 7353 7472 7563 7475 7265  ..ClassStructure
+00000670: 4465 6669 6e69 7469 6f6e da0d 696e 6865  Definition..inhe
+00000680: 7269 7473 5f66 726f 6d4e 7214 0000 0072  rits_fromNr....r
+00000690: 0f00 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
+000006a0: 0000 0072 3000 0000 3400 0000 721a 0000  ...r0...4...r...
+000006b0: 0072 3000 0000 6300 0000 0000 0000 0000  .r0...c.........
+000006c0: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
+000006d0: 3600 0000 6500 5a01 6400 5a02 5500 6503  6...e.Z.d.Z.U.e.
+000006e0: 6504 1900 6505 6401 3c00 6506 6505 6402  e...e.d.<.e.e.d.
+000006f0: 3c00 6403 5a07 6504 6505 6404 3c00 6405  <.d.Z.e.e.d.<.d.
+00000700: 6406 8400 5a08 6403 5300 2907 da1b 4675  d...Z.d.S.)...Fu
+00000710: 6e63 7469 6f6e 5374 7275 6374 7572 6544  nctionStructureD
+00000720: 6566 696e 6974 696f 6eda 0670 6172 616d  efinition..param
+00000730: 73da 0c70 6172 656e 745f 636c 6173 734e  s..parent_classN
+00000740: da0b 7265 7475 726e 5f74 7970 6563 0200  ..return_typec..
+00000750: 0000 0000 0000 0000 0000 0200 0000 0600  ................
+00000760: 0000 4300 0000 7330 0000 007c 006a 007c  ..C...s0...|.j.|
+00000770: 006a 017c 006a 027c 006a 037c 006a 0466  .j.|.j.|.j.|.j.f
+00000780: 057c 016a 007c 016a 017c 016a 027c 016a  .|.j.|.j.|.j.|.j
+00000790: 037c 016a 0466 056b 0253 0072 2d00 0000  .|.j.f.k.S.r-...
+000007a0: 2905 7212 0000 0072 3300 0000 721d 0000  ).r....r3...r...
+000007b0: 0072 1e00 0000 721c 0000 0029 0272 2a00  .r....r....).r*.
+000007c0: 0000 da05 6f74 6865 7272 0f00 0000 720f  ....otherr....r.
+000007d0: 0000 0072 1000 0000 da06 5f5f 6571 5f5f  ...r......__eq__
+000007e0: 3f00 0000 731a 0000 0004 0204 0104 0104  ?...s...........
+000007f0: 0104 0102 fb04 0704 0104 0104 0104 0102  ................
+00000800: fb04 fa7a 2246 756e 6374 696f 6e53 7472  ...z"FunctionStr
+00000810: 7563 7475 7265 4465 6669 6e69 7469 6f6e  uctureDefinition
+00000820: 2e5f 5f65 715f 5f29 0972 0800 0000 7209  .__eq__).r....r.
+00000830: 0000 0072 0a00 0000 da04 6c69 7374 7215  ...r......listr.
+00000840: 0000 0072 1600 0000 7230 0000 0072 3500  ...r....r0...r5.
+00000850: 0000 7237 0000 0072 0f00 0000 720f 0000  ..r7...r....r...
+00000860: 0072 0f00 0000 7210 0000 0072 3200 0000  .r....r....r2...
+00000870: 3900 0000 730a 0000 000a 000c 0208 010c  9...s...........
+00000880: 010c 0272 3200 0000 6300 0000 0000 0000  ...r2...c.......
+00000890: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+000008a0: 0072 1700 0000 2903 da18 4669 656c 6453  .r....)...FieldS
+000008b0: 7472 7563 7475 7265 4465 6669 6e69 7469  tructureDefiniti
+000008c0: 6f6e 7234 0000 004e 2905 7208 0000 0072  onr4...N).r....r
+000008d0: 0900 0000 720a 0000 0072 3000 0000 7216  ....r....r0...r.
+000008e0: 0000 0072 0f00 0000 720f 0000 0072 0f00  ...r....r....r..
+000008f0: 0000 7210 0000 0072 3900 0000 4f00 0000  ..r....r9...O...
+00000900: 721a 0000 0072 3900 0000 6300 0000 0000  r....r9...c.....
+00000910: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
+00000920: 0000 0072 1700 0000 2903 da25 5479 7065  ...r....)..%Type
+00000930: 416e 6e6f 7461 7465 6446 6965 6c64 5374  AnnotatedFieldSt
+00000940: 7275 6374 7572 6544 6566 696e 6974 696f  ructureDefinitio
+00000950: 6eda 0f74 7970 655f 616e 6e6f 7461 7469  n..type_annotati
+00000960: 6f6e 4e72 1400 0000 720f 0000 0072 0f00  onNr....r....r..
+00000970: 0000 720f 0000 0072 1000 0000 723a 0000  ..r....r....r:..
+00000980: 0054 0000 0072 1a00 0000 723a 0000 0063  .T...r....r:...c
+00000990: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000009a0: 0100 0000 4000 0000 730c 0000 0065 005a  ....@...s....e.Z
+000009b0: 0164 005a 0264 0153 0029 02da 284e 6f74  .d.Z.d.S.)..(Not
+000009c0: 5479 7065 416e 6e6f 7461 7465 6446 6965  TypeAnnotatedFie
+000009d0: 6c64 5374 7275 6374 7572 6544 6566 696e  ldStructureDefin
+000009e0: 6974 696f 6e4e 2903 7208 0000 0072 0900  itionN).r....r..
+000009f0: 0000 720a 0000 0072 0f00 0000 720f 0000  ..r....r....r...
+00000a00: 0072 0f00 0000 7210 0000 0072 3c00 0000  .r....r....r<...
+00000a10: 5900 0000 7304 0000 0008 0004 0272 3c00  Y...s........r<.
+00000a20: 0000 290d da0b 6461 7461 636c 6173 7365  ..)...dataclasse
+00000a30: 73da 0465 6e75 6d72 0200 0000 7203 0000  s..enumr....r...
+00000a40: 0072 1100 0000 da09 6461 7461 636c 6173  .r......dataclas
+00000a50: 7372 1800 0000 721b 0000 0072 3000 0000  sr....r....r0...
+00000a60: 7232 0000 0072 3900 0000 723a 0000 0072  r2...r9...r:...r
+00000a70: 3c00 0000 720f 0000 0072 0f00 0000 720f  <...r....r....r.
+00000a80: 0000 0072 1000 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000a90: 653e 0100 0000 7324 0000 0008 000c 0110  e>....s$........
+00000aa0: 030e 0704 0510 0104 0410 0104 1d12 0104  ................
+00000ab0: 0412 0104 1512 0104 0412 0104 0416 01    ...............
```

### Comparing `specifipy-0.2.0/setup.py` & `specifipy-0.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['specifipy',
+ 'specifipy.diagram_engines',
  'specifipy.file_scanners',
  'specifipy.parsers',
  'specifipy.parsers.structure']
 
 package_data = \
-{'': ['*'], 'specifipy': ['resources/icons/*']}
+{'': ['*']}
 
 install_requires = \
 ['docstring-parser>=0.15,<0.16', 'py-d2==1.0.0', 'snakemd>=0.11.0,<0.12.0']
 
 setup_kwargs = {
     'name': 'specifipy',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Python package for auto-generating code diagrams',
     'long_description': 'None',
     'author': 'Bartosz Budzyński',
     'author_email': 'hi@bartosz.blog',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `specifipy-0.2.0/PKG-INFO` & `specifipy-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specifipy
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python package for auto-generating code diagrams
 Author: Bartosz Budzyński
 Author-email: hi@bartosz.blog
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

