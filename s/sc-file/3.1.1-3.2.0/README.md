# Comparing `tmp/sc_file-3.1.1.tar.gz` & `tmp/sc_file-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc_file-3.1.1.tar", max compression
+gzip compressed data, was "sc_file-3.2.0.tar", max compression
```

## Comparing `sc_file-3.1.1.tar` & `sc_file-3.2.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1083 2023-01-22 13:34:34.609366 sc_file-3.1.1/LICENSE
--rw-r--r--   0        0        0      795 2024-04-17 23:28:14.269001 sc_file-3.1.1/pyproject.toml
--rw-r--r--   0        0        0     5065 2024-04-14 14:09:27.400282 sc_file-3.1.1/README.md
--rw-r--r--   0        0        0      186 2024-04-14 13:44:35.652910 sc_file-3.1.1/scfile/__init__.py
--rw-r--r--   0        0        0     1485 2024-04-14 13:10:00.131909 sc_file-3.1.1/scfile/__main__.py
--rw-r--r--   0        0        0     1361 2024-04-14 14:13:20.447282 sc_file-3.1.1/scfile/consts.py
--rw-r--r--   0        0        0     1143 2024-04-14 13:45:32.018913 sc_file-3.1.1/scfile/enums.py
--rw-r--r--   0        0        0      427 2024-03-20 03:27:16.312140 sc_file-3.1.1/scfile/exceptions/__init__.py
--rw-r--r--   0        0        0       84 2024-03-20 03:27:16.312140 sc_file-3.1.1/scfile/exceptions/base.py
--rw-r--r--   0        0        0     1408 2024-03-20 03:27:16.313140 sc_file-3.1.1/scfile/exceptions/basic.py
--rw-r--r--   0        0        0      641 2024-03-20 03:27:16.313140 sc_file-3.1.1/scfile/exceptions/decode.py
--rw-r--r--   0        0        0     1409 2024-03-20 03:27:16.313140 sc_file-3.1.1/scfile/exceptions/mcsa.py
--rw-r--r--   0        0        0      866 2024-03-20 03:27:16.314140 sc_file-3.1.1/scfile/exceptions/ol.py
--rw-r--r--   0        0        0        2 2024-03-20 03:27:16.314140 sc_file-3.1.1/scfile/file/__init__.py
--rw-r--r--   0        0        0      780 2024-03-20 03:27:16.314140 sc_file-3.1.1/scfile/file/base.py
--rw-r--r--   0        0        0      394 2024-03-25 13:19:34.701976 sc_file-3.1.1/scfile/file/data.py
--rw-r--r--   0        0        0     2162 2024-03-20 03:27:16.315140 sc_file-3.1.1/scfile/file/dds/encoder.py
--rw-r--r--   0        0        0     1124 2024-03-20 03:27:16.315140 sc_file-3.1.1/scfile/file/dds/structure.py
--rw-r--r--   0        0        0     3185 2024-03-26 21:28:59.417991 sc_file-3.1.1/scfile/file/decoder.py
--rw-r--r--   0        0        0     1840 2024-03-26 21:28:59.418992 sc_file-3.1.1/scfile/file/encoder.py
--rw-r--r--   0        0        0     7342 2024-04-14 13:11:08.724324 sc_file-3.1.1/scfile/file/mcsa/decoder.py
--rw-r--r--   0        0        0      682 2024-03-26 21:28:59.419991 sc_file-3.1.1/scfile/file/mcsa/flags.py
--rw-r--r--   0        0        0      153 2024-03-20 03:27:16.317139 sc_file-3.1.1/scfile/file/mcsa/versions.py
--rw-r--r--   0        0        0      611 2024-03-20 03:27:16.317139 sc_file-3.1.1/scfile/file/mic/decoder.py
--rw-r--r--   0        0        0     2284 2024-03-26 21:28:59.419991 sc_file-3.1.1/scfile/file/obj/encoder.py
--rw-r--r--   0        0        0      694 2024-03-20 03:27:16.318139 sc_file-3.1.1/scfile/file/ol/converter/base.py
--rw-r--r--   0        0        0      189 2024-03-20 03:27:16.318139 sc_file-3.1.1/scfile/file/ol/converter/bgra8.py
--rw-r--r--   0        0        0      244 2024-03-20 03:27:16.318139 sc_file-3.1.1/scfile/file/ol/converter/rgba32f.py
--rw-r--r--   0        0        0     3864 2024-03-26 21:28:59.419991 sc_file-3.1.1/scfile/file/ol/decoder.py
--rw-r--r--   0        0        0      144 2024-03-20 03:27:16.319140 sc_file-3.1.1/scfile/file/ol/formats.py
--rw-r--r--   0        0        0      295 2024-03-20 03:27:16.319140 sc_file-3.1.1/scfile/file/png/encoder.py
--rw-r--r--   0        0        0        0 2024-03-20 03:27:16.319140 sc_file-3.1.1/scfile/io/__init__.py
--rw-r--r--   0        0        0     1568 2024-03-20 03:27:16.320140 sc_file-3.1.1/scfile/io/base.py
--rw-r--r--   0        0        0      261 2024-03-20 03:27:16.320140 sc_file-3.1.1/scfile/io/binary.py
--rw-r--r--   0        0        0      610 2024-03-20 03:27:16.320140 sc_file-3.1.1/scfile/io/mcsa.py
--rw-r--r--   0        0        0      405 2024-03-20 03:27:16.321141 sc_file-3.1.1/scfile/io/ol.py
--rw-r--r--   0        0        0      122 2024-03-26 21:28:59.420991 sc_file-3.1.1/scfile/types.py
--rw-r--r--   0        0        0     3862 2024-04-14 13:46:22.120912 sc_file-3.1.1/scfile/utils/convert.py
--rw-r--r--   0        0        0     3027 2024-04-02 04:43:06.633771 sc_file-3.1.1/scfile/utils/model.py
--rw-r--r--   0        0        0     6116 1970-01-01 00:00:00.000000 sc_file-3.1.1/setup.py
--rw-r--r--   0        0        0     5579 1970-01-01 00:00:00.000000 sc_file-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-01-22 13:34:34.609366 sc_file-3.2.0/LICENSE
+-rw-r--r--   0        0        0      795 2024-04-30 01:54:55.746800 sc_file-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5065 2024-04-14 14:09:27.400282 sc_file-3.2.0/README.md
+-rw-r--r--   0        0        0      186 2024-04-14 13:44:35.652910 sc_file-3.2.0/scfile/__init__.py
+-rw-r--r--   0        0        0     1485 2024-04-14 13:10:00.131909 sc_file-3.2.0/scfile/__main__.py
+-rw-r--r--   0        0        0     1269 2024-04-30 03:15:55.753849 sc_file-3.2.0/scfile/consts.py
+-rw-r--r--   0        0        0     1143 2024-04-14 13:45:32.018913 sc_file-3.2.0/scfile/enums.py
+-rw-r--r--   0        0        0      427 2024-03-20 03:27:16.312140 sc_file-3.2.0/scfile/exceptions/__init__.py
+-rw-r--r--   0        0        0       84 2024-03-20 03:27:16.312140 sc_file-3.2.0/scfile/exceptions/base.py
+-rw-r--r--   0        0        0     1408 2024-03-20 03:27:16.313140 sc_file-3.2.0/scfile/exceptions/basic.py
+-rw-r--r--   0        0        0      641 2024-03-20 03:27:16.313140 sc_file-3.2.0/scfile/exceptions/decode.py
+-rw-r--r--   0        0        0     1409 2024-03-20 03:27:16.313140 sc_file-3.2.0/scfile/exceptions/mcsa.py
+-rw-r--r--   0        0        0      866 2024-03-20 03:27:16.314140 sc_file-3.2.0/scfile/exceptions/ol.py
+-rw-r--r--   0        0        0        2 2024-03-20 03:27:16.314140 sc_file-3.2.0/scfile/file/__init__.py
+-rw-r--r--   0        0        0      780 2024-03-20 03:27:16.314140 sc_file-3.2.0/scfile/file/base.py
+-rw-r--r--   0        0        0      394 2024-03-25 13:19:34.701976 sc_file-3.2.0/scfile/file/data.py
+-rw-r--r--   0        0        0     2162 2024-03-20 03:27:16.315140 sc_file-3.2.0/scfile/file/dds/encoder.py
+-rw-r--r--   0        0        0     1124 2024-03-20 03:27:16.315140 sc_file-3.2.0/scfile/file/dds/structure.py
+-rw-r--r--   0        0        0     3185 2024-03-26 21:28:59.417991 sc_file-3.2.0/scfile/file/decoder.py
+-rw-r--r--   0        0        0     1840 2024-03-26 21:28:59.418992 sc_file-3.2.0/scfile/file/encoder.py
+-rw-r--r--   0        0        0     6784 2024-04-30 01:57:33.155844 sc_file-3.2.0/scfile/file/mcsa/decoder.py
+-rw-r--r--   0        0        0      682 2024-03-26 21:28:59.419991 sc_file-3.2.0/scfile/file/mcsa/flags.py
+-rw-r--r--   0        0        0      153 2024-03-20 03:27:16.317139 sc_file-3.2.0/scfile/file/mcsa/versions.py
+-rw-r--r--   0        0        0      611 2024-03-20 03:27:16.317139 sc_file-3.2.0/scfile/file/mic/decoder.py
+-rw-r--r--   0        0        0     2327 2024-04-30 03:00:13.820947 sc_file-3.2.0/scfile/file/obj/encoder.py
+-rw-r--r--   0        0        0      694 2024-04-27 19:31:59.469317 sc_file-3.2.0/scfile/file/ol/converter/base.py
+-rw-r--r--   0        0        0      189 2024-03-20 03:27:16.318139 sc_file-3.2.0/scfile/file/ol/converter/bgra8.py
+-rw-r--r--   0        0        0      244 2024-03-20 03:27:16.318139 sc_file-3.2.0/scfile/file/ol/converter/rgba32f.py
+-rw-r--r--   0        0        0     3864 2024-03-26 21:28:59.419991 sc_file-3.2.0/scfile/file/ol/decoder.py
+-rw-r--r--   0        0        0      144 2024-03-20 03:27:16.319140 sc_file-3.2.0/scfile/file/ol/formats.py
+-rw-r--r--   0        0        0      295 2024-03-20 03:27:16.319140 sc_file-3.2.0/scfile/file/png/encoder.py
+-rw-r--r--   0        0        0        0 2024-03-20 03:27:16.319140 sc_file-3.2.0/scfile/io/__init__.py
+-rw-r--r--   0        0        0     1578 2024-04-27 19:35:49.133419 sc_file-3.2.0/scfile/io/base.py
+-rw-r--r--   0        0        0      261 2024-03-20 03:27:16.320140 sc_file-3.2.0/scfile/io/binary.py
+-rw-r--r--   0        0        0     1980 2024-04-30 03:21:38.728106 sc_file-3.2.0/scfile/io/mcsa.py
+-rw-r--r--   0        0        0      405 2024-03-20 03:27:16.321141 sc_file-3.2.0/scfile/io/ol.py
+-rw-r--r--   0        0        0      122 2024-03-26 21:28:59.420991 sc_file-3.2.0/scfile/types.py
+-rw-r--r--   0        0        0     3862 2024-04-14 13:46:22.120912 sc_file-3.2.0/scfile/utils/convert.py
+-rw-r--r--   0        0        0     3157 2024-04-30 03:00:20.451006 sc_file-3.2.0/scfile/utils/model.py
+-rw-r--r--   0        0        0     6116 1970-01-01 00:00:00.000000 sc_file-3.2.0/setup.py
+-rw-r--r--   0        0        0     5579 1970-01-01 00:00:00.000000 sc_file-3.2.0/PKG-INFO
```

### Comparing `sc_file-3.1.1/LICENSE` & `sc_file-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.1/pyproject.toml` & `sc_file-3.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sc-file"
-version = "3.1.1"
+version = "3.2.0"
 description = "Utility & Library for decoding stalcraft assets"
 authors = ["onejeuu <bloodtrail@beber1k.ru>"]
 
 license = "MIT"
 readme = "README.md"
 
 homepage = "https://github.com/onejeuu/sc-file"
```

### Comparing `sc_file-3.1.1/README.md` & `sc_file-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.1/scfile/__main__.py` & `sc_file-3.2.0/scfile/__main__.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.1/scfile/consts.py` & `sc_file-3.2.0/scfile/consts.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,21 +20,21 @@
 
     DDS = [0x44, 0x44, 0x53, 0x20]
     PNG = [0x89, 0x50, 0x4E, 0x47]
 
 
 class Factor:
     """
-    Integer range + 1.
+    Integer range.
     """
 
-    I8 = 0x80
-    U8 = 0x100
-    I16 = 0x8000
-    U16 = 0x10000
+    I8 = 0x7F
+    U8 = 0xFF
+    I16 = 0x7FFF
+    U16 = 0xFFFF
 
 
 class OlString:
     """
     Xor encoded zero-end string.
     """
 
@@ -45,18 +45,17 @@
 
 class McsaModel:
     """
     Mcsa model constants.
     """
 
     ROOT_BONE_ID = -1
-    # I dont know specific limit
-    # This is done for case when file was read incorrectly
+    # There is no known limit
+    # This for case when file was read incorrectly
     # So as not to overflow memory
-    # ? Trees and new year toys have hundreds of thousands of vertices...
     COUNT_LIMIT = 0x100000
 
 
 class McsaSize:
     """
     Count of elements in each mcsa data structure.
     """
```

### Comparing `sc_file-3.1.1/scfile/enums.py` & `sc_file-3.2.0/scfile/enums.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.1/scfile/exceptions/basic.py` & `sc_file-3.2.0/scfile/exceptions/basic.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.1/scfile/exceptions/decode.py` & `sc_file-3.2.0/scfile/exceptions/decode.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.1/scfile/exceptions/mcsa.py` & `sc_file-3.2.0/scfile/exceptions/mcsa.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.1/scfile/exceptions/ol.py` & `sc_file-3.2.0/scfile/exceptions/ol.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.1/scfile/file/base.py` & `sc_file-3.2.0/scfile/file/base.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.1/scfile/file/dds/encoder.py` & `sc_file-3.2.0/scfile/file/dds/encoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.1/scfile/file/dds/structure.py` & `sc_file-3.2.0/scfile/file/dds/structure.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.1/scfile/file/decoder.py` & `sc_file-3.2.0/scfile/file/decoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.1/scfile/file/encoder.py` & `sc_file-3.2.0/scfile/file/encoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.1/scfile/file/mcsa/decoder.py` & `sc_file-3.2.0/scfile/file/mcsa/decoder.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import numpy as np
-
 from scfile import exceptions as exc
 from scfile.consts import Factor, McsaSize, Signature
 from scfile.enums import ByteOrder
 from scfile.enums import StructFormat as F
 from scfile.file.data import ModelData
 from scfile.file.decoder import FileDecoder
 from scfile.file.obj.encoder import ObjEncoder
@@ -81,16 +79,16 @@
         for _ in range(self.meshes_count):
             self._parse_mesh()
 
     def _parse_mesh(self):
         self.mesh = Mesh()
 
         # Name & Material
-        self.mesh.name = self.f.reads().decode()
-        self.mesh.material = self.f.reads().decode()
+        self.mesh.name = self.f.readstring()
+        self.mesh.material = self.f.readstring()
 
         # Skeleton bone indexes
         if self.flags[Flag.SKELETON]:
             self._parse_bone_indexes()
 
         # Counts
         self.count.vertices = self.f.readcounts()
@@ -157,39 +155,36 @@
             self.mesh.bones[index] = self.f.readb(F.I8)
 
     def _parse_locals(self):
         # Possibly local axis and center (6 floats)
         # Quite useless
         self.f.read(6 * 4)
 
-    def _read_vertex_data(self, fmt: str, factor: float, size: int, scale: float = 1.0):
-        data = self.f.readvalues(fmt=fmt, size=size, count=self.count.vertices)
-
-        scaled = np.array(data) * scale / factor
-        reshaped = scaled.reshape(-1, size)
-
-        return reshaped
-
     def _parse_position(self):
-        xyzw = self._read_vertex_data(F.I16, Factor.I16, McsaSize.POSITION, self.scale.position)
+        count = self.count.vertices
+        scale = self.scale.position
+        xyzw = self.f.readvertex(F.I16, Factor.I16, McsaSize.POSITION, count, scale)
 
         for vertex, (x, y, z, _) in zip(self.vertices, xyzw):
             vertex.position.x = x
             vertex.position.y = y
             vertex.position.z = z
 
     def _parse_texture(self):
-        uv = self._read_vertex_data(F.I16, Factor.I16, McsaSize.TEXTURE, self.scale.texture)
+        count = self.count.vertices
+        scale = self.scale.texture
+        uv = self.f.readvertex(F.I16, Factor.I16, McsaSize.TEXTURE, count, scale)
 
         for vertex, (u, v) in zip(self.vertices, uv):
             vertex.texture.u = u
             vertex.texture.v = v
 
     def _parse_normals(self):
-        xyzw = self._read_vertex_data(F.I8, Factor.I8, McsaSize.NORMALS)
+        count = self.count.vertices
+        xyzw = self.f.readvertex(F.I8, Factor.I8, McsaSize.NORMALS, count)
 
         for vertex, (x, y, z, _) in zip(self.vertices, xyzw):
             vertex.normals.x = x
             vertex.normals.y = y
             vertex.normals.z = z
 
     def _skip_vertices(self, size: int = 4):
@@ -223,29 +218,16 @@
         argb = self._read_vertex_data(F.U8, Factor.U8, McsaSize.COLOR)
 
         for vertex, (_, r, g, b) in zip(self.vertices, argb):
             vertex.color.r = r
             vertex.color.g = g
             vertex.color.b = b
 
-    def _read_polygons_data(self):
-        size = McsaSize.POLYGONS
-        count = self.count.polygons * size
-        fmt = F.U16 if count < Factor.U16 else F.U32
-
-        data = self.f.readvalues(fmt=fmt, size=size, count=self.count.polygons)
-
-        # In mcsa vertex indexes 0-based
-        shifted = np.array(data) + 1
-        reshaped = shifted.reshape(-1, size)
-
-        return reshaped
-
     def _parse_polygons(self):
-        abc = self._read_polygons_data()
+        abc = self.f.readpolygons(self.count.polygons)
 
         for polygon, (a, b, c) in zip(self.mesh.polygons, abc):
             polygon.a = a
             polygon.b = b
             polygon.c = c
 
     def _parse_skeleton(self):
```

### Comparing `sc_file-3.1.1/scfile/file/mcsa/flags.py` & `sc_file-3.2.0/scfile/file/mcsa/flags.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.1/scfile/file/mic/decoder.py` & `sc_file-3.2.0/scfile/file/mic/decoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.1/scfile/file/obj/encoder.py` & `sc_file-3.2.0/scfile/file/obj/encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,19 @@
 class ObjEncoder(FileEncoder[ModelData]):
     FLOAT_FORMAT = ".6f"
 
     def serialize(self):
         self.model = self.data.model
         self.flags = self.data.model.flags
 
-        self.offset = 0
         self.model.ensure_unique_names()
 
+        # In obj vertex indexes 1-based
+        self.offset = 1
+
         for mesh in self.model.meshes:
             self.b.writes(f"o {mesh.name}\n")
 
             self._add_geometric_vertices(mesh)
 
             if self.flags.texture:
                 self._add_texture_coordinates(mesh)
```

### Comparing `sc_file-3.1.1/scfile/file/ol/converter/base.py` & `sc_file-3.2.0/scfile/file/ol/converter/base.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.1/scfile/file/ol/decoder.py` & `sc_file-3.2.0/scfile/file/ol/decoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.1/scfile/io/base.py` & `sc_file-3.2.0/scfile/io/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,13 +35,13 @@
     def writeb(self, fmt: str, *v: Any, order: Optional[ByteOrder] = None) -> None:
         """Pack any binary data."""
         order = order or self.order
         data = self.pack(f"{order}{fmt}", *v)
         self.write(data)
 
     def writen(self, count: int = 1, size: int = 4) -> None:
-        """Fill buffer with 4 bytes zeros."""
+        """Fill buffer with zeros by size (4 bytes)."""
         self.write(bytes(size * count))
 
     def writes(self, string: str) -> None:
         """Write utf-8 encoded string."""
         self.write(string.encode("utf-8", errors="replace"))
```

### Comparing `sc_file-3.1.1/scfile/utils/convert.py` & `sc_file-3.2.0/scfile/utils/convert.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.1/scfile/utils/model.py` & `sc_file-3.2.0/scfile/utils/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,17 +61,19 @@
     count: Count = field(default_factory=Count)
     vertices: List[Vertex] = field(default_factory=list)
     polygons: List[Polygon] = field(default_factory=list)
     bones: Dict[int, int] = field(default_factory=dict)
 
     @property
     def offset(self) -> int:
-        return len(self.vertices)
+        """Count of vertices. To shift vertex indexes of polygons."""
+        return self.count.vertices
 
     def resize(self) -> None:
+        """Fills vertices & polygons by their counts."""
         self.vertices = [Vertex() for _ in range(self.count.vertices)]
         self.polygons = [Polygon() for _ in range(self.count.polygons)]
 
 
 @dataclass
 class Bone:
     name: str = "bone"
```

### Comparing `sc_file-3.1.1/setup.py` & `sc_file-3.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'quicktex>=0.2.0,<0.3.0']
 
 entry_points = \
 {'console_scripts': ['build = build:build']}
 
 setup_kwargs = {
     'name': 'sc-file',
-    'version': '3.1.1',
+    'version': '3.2.0',
     'description': 'Utility & Library for decoding stalcraft assets',
     'long_description': '# SC FILE\n\nUtility and Library for decoding and converting stalcraft assets files, such as models and textures into well-known formats.\n\nDesigned for artworks creation and the like.\n\n> [!NOTE]\n> There is not and will not be encoding back into game formats.\n\n> [!WARNING]\n> Do not use game assets directly. \\\n> Any changes in game client can be detected.\n\nYou can use executable program from [Releases](https://github.com/onejeuu/sc-file/releases) page.\n\n# 📁 Formats\n\n| Type    | Source format | Output format |\n| ------- | ------------- | ------------- |\n| Model   | .mcsa         | .obj          |\n| Model   | .mcvd         | .obj          |\n| Texture | .ol           | .dds          |\n| Image   | .mic          | .png          |\n\nModel versions supported: 7.0, 8.0, 10.0\n\nTexture formats supported: DXT1, DXT3, DXT5, RGBA8, BGRA8, RGBA32F, DXN_XY\n\nTexture formats unsupported: Cubemaps (hdri, sky)\n\n# 💻 CLI Utility\n\n## Usage\n\nFrom bash:\n\n```bash\nscfile [FILES]... [OPTIONS]\n```\n\n> [!TIP]\n> You can just drag and drop one or multiple files onto `scfile.exe`.\n\n## Arguments\n\n- `FILES`: **List of file paths to be converted**. Multiple files should be separated by **spaces**. Accepts both full and relative paths. **Does not accept directory**.\n\n## Options\n\n- `-O`, `--output`: **One path to output file or directory**. Can be specified multiple times for different output files or directories. If not specified, file will be saved in same directory with a new suffix. You can specify multiple `FILES` and a single `--output` directory.\n\n## Examples\n\n1. Convert a single file:\n\n   ```bash\n   scfile file.mcsa\n   ```\n\n   _Will be saved in same directory with a new suffix._\n\n2. Convert a single file with a specified path or name:\n\n   ```bash\n   scfile file.mcsa --output path/to/file.obj\n   ```\n\n3. Convert multiple files to a specified directory:\n\n   ```bash\n   scfile file1.mcsa file2.mcsa --output path/to/dir\n   ```\n\n4. Convert multiple files with explicitly specified output files:\n\n   ```bash\n   scfile file1.mcsa file2.mcsa -O 1.obj -O 2.obj\n   ```\n\n   _If count of `FILES` and `--output` is different, as many files as possible will be converted._\n\n5. Convert all `.mcsa` files in current directory:\n\n   ```bash\n   scfile *.mcsa\n   ```\n\n   _In this case, `--output` accepts only a directory. Subdirectories are not included._\n\n6. Convert all `.mcsa` files with subdirectories to a specified directory:\n\n   ```bash\n   scfile **/*.mcsa -O path/to/dir\n   ```\n\n   _In this case, `--output` accepts only a directory. With `--output` specified, directory structure is not duplicated._\n\n# 📚 Library\n\n## Install\n\n### Pip\n\n```bash\npip install sc-file -U\n```\n\n### Manual\n\n```bash\ngit clone git@github.com:onejeuu/sc-file.git\n```\n\n```bash\ncd sc-file\n```\n\n```bash\npoetry install\n```\n\n## Usage\n\n### Simple\n\n```python\nfrom scfile import convert\n\n# Output path is optional.\n# Defaults to source path with new suffix.\nconvert.mcsa_to_obj("path/to/model.mcsa", "path/to/model.obj")\nconvert.ol_to_dds("path/to/texture.ol", "path/to/texture.dds")\nconvert.mic_to_png("path/to/image.mic", "path/to/image.png")\n\n# Or determinate it automatically\nconvert.auto("path/to/model.mcsa")\n```\n\n### Advanced\n\nDefault\n\n```python\nfrom scfile.file.data import ModelData\nfrom scfile.file.mcsa.decoder import McsaDecoder\nfrom scfile.file.obj.encoder import ObjEncoder\n\nmcsa = McsaDecoder("model.mcsa")\ndata: ModelData = mcsa.decode()\nmcsa.close() # ? Necessary to close\n\nobj = ObjEncoder(data)\nobj.encode().save("model.obj") # ? Encoder closes after saving\n```\n\nUse encoded content bytes\n\n```python\nobj = ObjEncoder(data)\nobj.encode()\n\nwith open("model.obj", "wb") as fp:\n    fp.write(obj.content)\n\nobj.close() # ? Necessary to close\n```\n\nUse convert methods\n\n```python\nmcsa = McsaDecoder("model.mcsa")\nmcsa.convert_to(ObjEncoder).save("model.obj")\nmcsa.close() # ? Necessary to close\n```\n\n```python\nmcsa = McsaDecoder("model.mcsa")\nmcsa.to_obj().save("model.obj")\nmcsa.close() # ? Necessary to close\n```\n\nUse context manager\n\n```python\nwith McsaDecoder("model.mcsa") as mcsa:\n    data: ModelData = mcsa.decode()\n\nwith ObjEncoder(data) as obj:\n    obj.encode().save("model.obj")\n```\n\nUse context manager + convert methods\n\n```python\nwith McsaDecoder("model.mcsa") as mcsa:\n    mcsa.to_obj().save("model.obj")\n```\n\nSave multiple copies\n\n```python\nwith McsaDecoder("model.mcsa") as mcsa:\n    with mcsa.to_obj() as obj:\n        obj.save_as("model_1.obj")\n        obj.save_as("model_2.obj")\n```\n\n# 🛠️ Build\n\n> [!IMPORTANT]\n> You will need [poetry](https://python-poetry.org) to do compilation.\n\n> [!TIP]\n> Recommended to create virtual environment.\n>\n> ```bash\n> poetry shell\n> ```\n\nThen install dependencies:\n\n```bash\npoetry install\n```\n\nAnd run script to compile:\n\n```bash\npoetry run build\n```\n\nExecutable file will be created in `/dist` directory.\n',
     'author': 'onejeuu',
     'author_email': 'bloodtrail@beber1k.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/onejeuu/sc-file',
```

### Comparing `sc_file-3.1.1/PKG-INFO` & `sc_file-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sc-file
-Version: 3.1.1
+Version: 3.2.0
 Summary: Utility & Library for decoding stalcraft assets
 Home-page: https://github.com/onejeuu/sc-file
 License: MIT
 Author: onejeuu
 Author-email: bloodtrail@beber1k.ru
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
```

