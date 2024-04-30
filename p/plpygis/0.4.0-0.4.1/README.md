# Comparing `tmp/plpygis-0.4.0.tar.gz` & `tmp/plpygis-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plpygis-0.4.0.tar", last modified: Mon Apr 22 00:59:21 2024, max compression
+gzip compressed data, was "plpygis-0.4.1.tar", last modified: Tue Apr 30 06:21:01 2024, max compression
```

## Comparing `plpygis-0.4.0.tar` & `plpygis-0.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-04-22 00:59:21.690892 plpygis-0.4.0/
--rw-r--r--   0 ben       (1000) ben       (1000)     2492 2024-04-22 00:53:22.000000 plpygis-0.4.0/CHANGELOG.md
--rw-r--r--   0 ben       (1000) ben       (1000)    35142 2024-03-08 10:22:13.000000 plpygis-0.4.0/LICENSE
--rw-r--r--   0 ben       (1000) ben       (1000)      101 2024-04-22 00:53:22.000000 plpygis-0.4.0/MANIFEST.in
--rw-r--r--   0 ben       (1000) ben       (1000)     2472 2024-04-22 00:59:21.690892 plpygis-0.4.0/PKG-INFO
--rw-r--r--   0 ben       (1000) ben       (1000)     1671 2024-04-22 00:53:22.000000 plpygis-0.4.0/README.md
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-04-22 00:59:21.690892 plpygis-0.4.0/plpygis/
--rw-r--r--   0 ben       (1000) ben       (1000)      436 2024-04-22 00:53:22.000000 plpygis-0.4.0/plpygis/__init__.py
--rw-r--r--   0 ben       (1000) ben       (1000)       22 2024-04-22 00:53:22.000000 plpygis-0.4.0/plpygis/_version.py
--rw-r--r--   0 ben       (1000) ben       (1000)     1615 2024-04-22 00:53:22.000000 plpygis-0.4.0/plpygis/exceptions.py
--rw-r--r--   0 ben       (1000) ben       (1000)    32122 2024-04-22 00:53:22.000000 plpygis-0.4.0/plpygis/geometry.py
--rw-r--r--   0 ben       (1000) ben       (1000)     3085 2024-04-22 00:53:22.000000 plpygis-0.4.0/plpygis/hex.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-04-22 00:59:21.690892 plpygis-0.4.0/plpygis.egg-info/
--rw-r--r--   0 ben       (1000) ben       (1000)     2472 2024-04-22 00:59:21.000000 plpygis-0.4.0/plpygis.egg-info/PKG-INFO
--rw-r--r--   0 ben       (1000) ben       (1000)      330 2024-04-22 00:59:21.000000 plpygis-0.4.0/plpygis.egg-info/SOURCES.txt
--rw-r--r--   0 ben       (1000) ben       (1000)        1 2024-04-22 00:59:21.000000 plpygis-0.4.0/plpygis.egg-info/dependency_links.txt
--rw-r--r--   0 ben       (1000) ben       (1000)       70 2024-04-22 00:59:21.000000 plpygis-0.4.0/plpygis.egg-info/requires.txt
--rw-r--r--   0 ben       (1000) ben       (1000)        8 2024-04-22 00:59:21.000000 plpygis-0.4.0/plpygis.egg-info/top_level.txt
--rw-r--r--   0 ben       (1000) ben       (1000)      841 2024-04-22 00:53:22.000000 plpygis-0.4.0/pyproject.toml
--rw-r--r--   0 ben       (1000) ben       (1000)       38 2024-04-22 00:59:21.690892 plpygis-0.4.0/setup.cfg
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-04-22 00:59:21.690892 plpygis-0.4.0/test/
--rw-r--r--   0 ben       (1000) ben       (1000)    23345 2024-04-22 00:53:22.000000 plpygis-0.4.0/test/test_geometry.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-04-30 06:21:01.673656 plpygis-0.4.1/
+-rw-r--r--   0 ben       (1000) ben       (1000)     2563 2024-04-30 06:19:35.000000 plpygis-0.4.1/CHANGELOG.md
+-rw-r--r--   0 ben       (1000) ben       (1000)    35142 2024-03-08 10:22:13.000000 plpygis-0.4.1/LICENSE
+-rw-r--r--   0 ben       (1000) ben       (1000)      101 2024-04-22 00:53:22.000000 plpygis-0.4.1/MANIFEST.in
+-rw-r--r--   0 ben       (1000) ben       (1000)     3191 2024-04-30 06:21:01.673656 plpygis-0.4.1/PKG-INFO
+-rw-r--r--   0 ben       (1000) ben       (1000)     2390 2024-04-30 06:19:30.000000 plpygis-0.4.1/README.md
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-04-30 06:21:01.673656 plpygis-0.4.1/plpygis/
+-rw-r--r--   0 ben       (1000) ben       (1000)      435 2024-04-30 06:19:30.000000 plpygis-0.4.1/plpygis/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)       22 2024-04-30 06:19:35.000000 plpygis-0.4.1/plpygis/_version.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     1891 2024-04-30 06:19:30.000000 plpygis-0.4.1/plpygis/exceptions.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    31534 2024-04-30 06:19:30.000000 plpygis-0.4.1/plpygis/geometry.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     3208 2024-04-30 06:19:30.000000 plpygis-0.4.1/plpygis/hex.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-04-30 06:21:01.673656 plpygis-0.4.1/plpygis.egg-info/
+-rw-r--r--   0 ben       (1000) ben       (1000)     3191 2024-04-30 06:21:01.000000 plpygis-0.4.1/plpygis.egg-info/PKG-INFO
+-rw-r--r--   0 ben       (1000) ben       (1000)      330 2024-04-30 06:21:01.000000 plpygis-0.4.1/plpygis.egg-info/SOURCES.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)        1 2024-04-30 06:21:01.000000 plpygis-0.4.1/plpygis.egg-info/dependency_links.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)       70 2024-04-30 06:21:01.000000 plpygis-0.4.1/plpygis.egg-info/requires.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)        8 2024-04-30 06:21:01.000000 plpygis-0.4.1/plpygis.egg-info/top_level.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)      841 2024-04-22 00:53:22.000000 plpygis-0.4.1/pyproject.toml
+-rw-r--r--   0 ben       (1000) ben       (1000)       38 2024-04-30 06:21:01.673656 plpygis-0.4.1/setup.cfg
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-04-30 06:21:01.673656 plpygis-0.4.1/test/
+-rw-r--r--   0 ben       (1000) ben       (1000)    24322 2024-04-30 06:19:30.000000 plpygis-0.4.1/test/test_geometry.py
```

### Comparing `plpygis-0.4.0/CHANGELOG.md` & `plpygis-0.4.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Changelog
 
+## [0.4.1] - DATE
+
+### Changed
+
+* Raise `WkbError` on malformed WKBs.
+
 ## [0.4.0] - 2024-04-22
 
 ### Added
 
-* All the `Geometry` classes now have a `coordinates()` method, and this is also used in the generation of GeoJSONs.
+* All the `Geometry` classes now have a `coordinates` property, and this is also used in the generation of GeoJSONs.
 * The `Geometry` classes also now have a `__copy__()` method.
 * Two new exceptions were added `CoordinateError` and `GeojsonError`.
 
 ### Chnaged
 
 * plpygis has been migrated to use `pyproject.toml` instead of `setup.py`.
 * The testing framework has been redone using `pytest`.
```

### Comparing `plpygis-0.4.0/LICENSE` & `plpygis-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `plpygis-0.4.0/plpygis/exceptions.py` & `plpygis-0.4.1/plpygis/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,66 +1,84 @@
 class PlpygisError(Exception):
     """
     Basic exception for ``plpygis``.
     """
+
     def __init__(self, msg):
         super().__init__(msg)
 
 
 class CoordinateError(PlpygisError):
     """
     Exception for problems in the coordinates of geometries.
     """
+
     def __init__(self, geom, msg=None):
         if msg is None:
             msg = f"Geometry has invalid coordinates: {geom}"
         super().__init__(msg)
 
 
+class CollectionError(PlpygisError):
+    """
+    Exception for problems with geometries in collection types.
+    """
+
+    def __init__(self, msg=None):
+        if msg is None:
+            msg = "Error in the geometries in a collection."
+        super().__init__(msg)
+
+
 class DependencyError(PlpygisError, ImportError):
     """
     Exception for a missing dependency.
     """
+
     def __init__(self, dep, msg=None):
         if msg is None:
             msg = f"Dependency '{dep}' is not available."
         super().__init__(msg)
 
 
 class WkbError(PlpygisError):
     """
     Exception for problems in parsing WKBs.
     """
+
     def __init__(self, msg=None):
         if msg is None:
             msg = "Unreadable WKB."
         super().__init__(msg)
 
 
 class DimensionalityError(PlpygisError):
     """
     Exception for problems in dimensionality of geometries.
     """
+
     def __init__(self, msg=None):
         if msg is None:
             msg = "Geometry has invalid dimensionality."
         super().__init__(msg)
 
 
 class SridError(PlpygisError):
     """
     Exception for problems in dimensionality of geometries.
     """
+
     def __init__(self, msg=None):
         if msg is None:
             msg = "Geometry has invalid SRID."
         super().__init__(msg)
 
 
 class GeojsonError(PlpygisError):
     """
     Exception for problems in GeoJSONs.
     """
+
     def __init__(self, msg=None):
         if msg is None:
             msg = "Invalid GeoJSON."
         super().__init__(msg)
```

### Comparing `plpygis-0.4.0/plpygis/geometry.py` & `plpygis-0.4.1/plpygis/geometry.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 import numbers
 from copy import copy
-from .exceptions import DependencyError, WkbError, SridError, DimensionalityError, CoordinateError, GeojsonError
+from .exceptions import (
+    DependencyError,
+    WkbError,
+    SridError,
+    DimensionalityError,
+    CoordinateError,
+    GeojsonError,
+    CollectionError,
+)
 from .hex import HexReader, HexWriter, HexBytes
 
 try:
     import shapely
     import shapely.wkb
+
     SHAPELY = True
 except ImportError:
     SHAPELY = False
 
 
-class Geometry():
+class Geometry:
     r"""A representation of a PostGIS geometry.
 
     PostGIS geometries are either an OpenGIS Consortium Simple Features for SQL
     specification type or a PostGIS extended type. The object's canonical form
     is stored in WKB or EWKB format along with an SRID and flags indicating
     whether the coordinates are 3DZ, 3DM or 4D.
 
@@ -55,15 +64,15 @@
         <MultiPoint: 'geometry(MultiPoint)'>
 
     A ``Geometry`` can be read as long as it is one of the following
     types: ``Point``, ``LineString``, ``Polygon``, ``MultiPoint``, ``MultiLineString``,
     ``MultiPolygon`` or ``GeometryCollection``. The M dimension will be preserved.
     """
 
-    _WKBTYPE = 0x1fffffff
+    _WKBTYPE = 0x1FFFFFFF
     _WKBZFLAG = 0x80000000
     _WKBMFLAG = 0x40000000
     _WKBSRIDFLAG = 0x20000000
     __slots__ = ["_wkb", "_reader", "_srid", "_dimz", "_dimm"]
 
     def __new__(cls, wkb, srid=None, dimz=False, dimm=False):
         if cls == Geometry:
@@ -239,18 +248,15 @@
             if (srid or self.srid) and srid != self.srid:
                 raise SridError(f"SRID mismatch: {srid} {self.srid}")
             return sgeom
         raise DependencyError("Shapely")
 
     def _to_geojson(self):
         coordinates = self._to_geojson_coordinates()
-        geojson = {
-                "type": self.type,
-                "coordinates": coordinates
-        }
+        geojson = {"type": self.type, "coordinates": coordinates}
         return geojson
 
     def __repr__(self):
         return f"<{self.type}: '{self.postgis_type}'>"
 
     def __str__(self):
         return self.wkb.__str__()
@@ -307,31 +313,55 @@
                 srid = None
         except TypeError as e:
             raise WkbError() from e
         return lwgeomtype, dimz, dimm, srid
 
     def _write_wkb_header(self, writer, use_srid, dimz, dimm):
         writer.add_order()
-        header = (self._LWGEOMTYPE |
-                  (Geometry._WKBZFLAG if dimz else 0) |
-                  (Geometry._WKBMFLAG if dimm else 0) |
-                  (Geometry._WKBSRIDFLAG if self.srid else 0))
+        header = (
+            self._LWGEOMTYPE
+            | (Geometry._WKBZFLAG if dimz else 0)
+            | (Geometry._WKBMFLAG if dimm else 0)
+            | (Geometry._WKBSRIDFLAG if self.srid else 0)
+        )
         writer.add_int(header)
         if use_srid and self.srid:
             writer.add_int(self.srid)
         return writer
 
 
 class _MultiGeometry(Geometry):
+    __slots__ = ["_geometries"]
+
+    def __init__(self, multitype, geometries=None, srid=None):
+        if self._wkb:
+            self._geometries = None
+        else:
+            if not all(isinstance(geometry, multitype) for geometry in geometries):
+                raise CollectionError(
+                    f"Found non-{multitype} when creating a Multi{multitype}"
+                )
+            self._geometries = geometries
+            self._srid = srid
+            self._set_multi_metadata()
+
     def __copy__(self):
         cls = self.__class__
-        geometries = [copy(geometry) for geometry in self.geometries]
+        geometries = [copy(geometry) for geometry in self._geometries]
         return cls(geometries, self.srid)
 
     @property
+    def geometries(self):
+        """
+        List of all component geometries.
+        """
+        self._check_cache()
+        return self._geometries
+
+    @property
     def dimz(self):
         """
         Whether the geometry has a Z dimension.
 
         :getter: ``True`` if the geometry has a Z dimension.
         :setter: Add or remove the Z dimension from this and all geometries in the collection.
         :rtype: bool
@@ -350,15 +380,15 @@
     def dimm(self):
         """
         Whether the geometry has an M dimension.
 
         :getter: ``True`` if the geometry has an M dimension.
         :setter: Add or remove the M dimension from this and all geometries in the collection.
         :rtype: bool
-       """
+        """
         return self._dimm
 
     @dimm.setter
     def dimm(self, value):
         if self._dimm == value:
             return
         for geometry in self.geometries:
@@ -378,15 +408,17 @@
         geometries = []
         for coordinates in geojson["coordinates"]:
             geometry = cls(coordinates, srid=None)
             geometries.append(geometry)
         return geometries
 
     def _load_geometry(self):
-        self._geometries = self.__class__._read_wkb(self._reader, self._dimz, self._dimm)
+        self._geometries = self.__class__._read_wkb(
+            self._reader, self._dimz, self._dimm
+        )
 
     def _set_multi_metadata(self):
         self._dimz = None
         self._dimm = None
         for geometry in self.geometries:
             if self._dimz is None:
                 self._dimz = geometry.dimz
@@ -394,23 +426,30 @@
                 raise DimensionalityError("Mixed dimensionality in MultiGeometry")
             if self._dimm is None:
                 self._dimm = geometry.dimm
             elif self._dimm != geometry.dimm:
                 raise DimensionalityError("Mixed dimensionality in MultiGeometry")
             if geometry._srid is not None:
                 if self._srid != geometry._srid:
-                    raise SridError("Geometry can not be different from SRID in MultiGeometry")
+                    raise SridError(
+                        "Geometry can not be different from SRID in MultiGeometry"
+                    )
                 geometry._srid = None
 
     def _coordinates(self, dimz=True, dimm=True, tpl=True):
         return [g._coordinates(dimz, dimm, tpl) for g in self.geometries]
 
     def _to_geojson_coordinates(self):
         return self._coordinates(dimm=False, tpl=False)
 
+    def _load_geometry(self):
+        self._geometries = _MultiGeometry._read_wkb(
+            self._reader, self._dimz, self._dimm
+        )
+
     @staticmethod
     def _read_wkb(reader, dimz, dimm):
         geometries = []
         try:
             for _ in range(reader.get_int()):
                 cls, dimz, dimm, srid = Geometry._get_wkb_type(reader)
                 coordinates = cls._read_wkb(reader, dimz, dimm)
@@ -418,15 +457,15 @@
                 geometries.append(geometry)
         except TypeError as e:
             raise WkbError() from e
         return geometries
 
     def _write_wkb(self, writer, dimz, dimm):
         writer.add_int(len(self.geometries))
-        for geometry in self.geometries:
+        for geometry in self._geometries:
             geometry._write_wkb_header(writer, False, dimz, dimm)
             geometry._write_wkb(writer, dimz, dimm)
 
 
 class Point(Geometry):
     """
     A representation of a PostGIS Point.
@@ -451,21 +490,25 @@
             self._z = None
             self._m = None
         else:
             for c in coordinates:
                 if c is None:
                     continue
                 if not isinstance(c, numbers.Number):
-                    raise CoordinateError(f"Coordinates must be numeric: {coordinates}", coordinates)
+                    raise CoordinateError(
+                        f"Coordinates must be numeric: {coordinates}", coordinates
+                    )
             self._srid = srid
             self._x = coordinates[0]
             self._y = coordinates[1]
             num = len(coordinates)
             if num > 4:
-                raise DimensionalityError(f"Maximum dimensionality supported for coordinates is 4: {coordinates}")
+                raise DimensionalityError(
+                    f"Maximum dimensionality supported for coordinates is 4: {coordinates}"
+                )
             if num == 2:  # fill in Z and M if we are supposed to have them, else None
                 if dimz and dimm:
                     self._z = 0
                     self._m = 0
                 elif dimz:
                     self._z = 0
                     self._m = None
@@ -620,15 +663,17 @@
     def _to_geojson_coordinates(self):
         return self._coordinates(dimm=False, tpl=False)
 
     def _bounds(self):
         return (self.x, self.y, self.x, self.y)
 
     def _load_geometry(self):
-        self._x, self._y, self._z, self._m = Point._read_wkb(self._reader, self._dimz, self._dimm)
+        self._x, self._y, self._z, self._m = Point._read_wkb(
+            self._reader, self._dimz, self._dimm
+        )
 
     @staticmethod
     def _read_wkb(reader, dimz, dimm):
         try:
             x = reader.get_double()
             y = reader.get_double()
             if dimz and dimm:
@@ -679,15 +724,17 @@
     def __init__(self, vertices=None, srid=None, dimz=False, dimm=False):
         if self._wkb:
             self._vertices = None
         else:
             self._srid = srid
             self._dimz = dimz
             self._dimm = dimm
-            self._vertices = LineString._from_coordinates(vertices, dimz=dimz, dimm=dimm)
+            self._vertices = LineString._from_coordinates(
+                vertices, dimz=dimz, dimm=dimm
+            )
             self._set_dimensionality(self._vertices)
 
     @property
     def vertices(self):
         """
         List of vertices that comprise the line.
         """
@@ -905,41 +952,24 @@
         <MultiPoint: 'geometry(MultiPointZ)'>
 
     The SRID and dimensionality of all geometries in the collection must be
     identical.
     """
 
     _LWGEOMTYPE = 4
-    __slots__ = ["_points"]
 
     def __init__(self, points=None, srid=None):
-        if self._wkb:
-            self._points = None
-        else:
-            self._points = points
-            self._srid = srid
-            self._set_multi_metadata()
+        super().__init__(Point, geometries=points, srid=srid)
 
     @property
     def points(self):
         """
         List of all component points.
         """
-        self._check_cache()
-        return self._points
-
-    @property
-    def geometries(self):
-        """
-        List of all component points.
-        """
-        return self.points
-
-    def _load_geometry(self):
-        self._points = MultiPoint._read_wkb(self._reader, self._dimz, self._dimm)
+        return self.geometries
 
 
 class MultiLineString(_MultiGeometry):
     """
     A representation of a PostGIS MultiLineString
 
     ``MultiLineString`` objects can be created directly from a list of
@@ -951,41 +981,24 @@
         <MultiLineString: 'geometry(MultiLineStringM)'>
 
     The SRID and dimensionality of all geometries in the collection must be
     identical.
     """
 
     _LWGEOMTYPE = 5
-    __slots__ = ["_linestrings"]
 
     def __init__(self, linestrings=None, srid=None):
-        if self._wkb:
-            self._linestrings = None
-        else:
-            self._linestrings = linestrings
-            self._srid = srid
-            self._set_multi_metadata()
+        super().__init__(LineString, geometries=linestrings, srid=srid)
 
     @property
     def linestrings(self):
         """
         List of all component lines.
         """
-        self._check_cache()
-        return self._linestrings
-
-    @property
-    def geometries(self):
-        """
-        List of all component lines.
-        """
-        return self.linestrings
-
-    def _load_geometry(self):
-        self._linestrings = MultiLineString._read_wkb(self._reader, self._dimz, self._dimm)
+        return self.geometries
 
 
 class MultiPolygon(_MultiGeometry):
     """
     A representation of a PostGIS MultiPolygon.
 
     ``MultiPolygon`` objects can be created directly from a list of ``Polygon``
@@ -997,41 +1010,24 @@
         <MultiPolygon: 'geometry(MultiPolygon,4326)'>
 
     The SRID and dimensionality of all geometries in the collection must be
     identical.
     """
 
     _LWGEOMTYPE = 6
-    __slots__ = ["__polygons__"]
 
     def __init__(self, polygons=None, srid=None):
-        if self._wkb:
-            self._polygons = None
-        else:
-            self._polygons = polygons
-            self._srid = srid
-            self._set_multi_metadata()
+        super().__init__(Polygon, geometries=polygons, srid=srid)
 
     @property
     def polygons(self):
         """
         List of all component polygons.
         """
-        self._check_cache()
-        return self._polygons
-
-    @property
-    def geometries(self):
-        """
-        List of all component polygons.
-        """
-        return self.polygons
-
-    def _load_geometry(self):
-        self._polygons = MultiPolygon._read_wkb(self._reader, self._dimz, self._dimm)
+        return self.geometries
 
 
 class GeometryCollection(_MultiGeometry):
     """
     A representation of a PostGIS GeometryCollection.
 
     ``GeometryCollection`` objects can be created directly from a list of
@@ -1043,32 +1039,15 @@
         <GeometryCollection: 'geometry(GeometryCollectionZ)'>
 
     The SRID and dimensionality of all geometries in the collection must be
     identical.
     """
 
     _LWGEOMTYPE = 7
-    __slots__ = ["_geometries"]
 
     def __init__(self, geometries=None, srid=None):
-        if self._wkb:
-            self._geometries = None
-        else:
-            self._geometries = geometries
-            self._srid = srid
-            self._set_multi_metadata()
-
-    @property
-    def geometries(self):
-        """
-        List of all component geometries.
-        """
-        self._check_cache()
-        return self._geometries
+        super().__init__(Geometry, geometries=geometries, srid=srid)
 
     def _to_geojson(self):
-        geometries = [g._to_geojson() for g in self.geometries]
-        geojson = {
-                "type": self.__class__.__name__,
-                "geometries": geometries
-        }
+        geometries = [g._to_geojson() for g in self._geometries]
+        geojson = {"type": self.__class__.__name__, "geometries": geometries}
         return geojson
```

### Comparing `plpygis-0.4.0/plpygis/hex.py` & `plpygis-0.4.1/plpygis/hex.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 from binascii import hexlify, unhexlify
-from struct import calcsize, unpack_from, pack
+from struct import calcsize, unpack_from, pack, error
+from .exceptions import WkbError
 
 
 class HexReader:
     """
     A reader for generic hex data. The current position in the stream of bytes
     will be retained as data is read.
     """
+
     def __init__(self, hexdata, order, offset=0):
         self._data = hexdata
         self._order = order
         self._ini_offset = offset
         self._cur_offset = offset
 
     def reset(self):
         """
         Start reading from the initial position again.
         """
         self._cur_offset = self._ini_offset
 
     def _get_value(self, fmt):
-        value = unpack_from(f"{self._order}{fmt}", self._data, self._cur_offset)[0]
+        try:
+            value = unpack_from(f"{self._order}{fmt}", self._data, self._cur_offset)[0]
+        except error as e:
+            raise WkbError(e) from e
         self._cur_offset += calcsize(fmt)
         return value
 
     def get_char(self):
         """
         Get the next character from the stream of bytes.
         """
@@ -43,14 +48,15 @@
         return self._get_value("d")
 
 
 class HexWriter:
     """
     A writer for generic hex data.
     """
+
     def __init__(self, order):
         self._fmts = []
         self._values = []
         self._order = order
 
     def _add_value(self, fmt, value):
         self._fmts.append(fmt)
@@ -97,18 +103,18 @@
     """A subclass of bytearray that represents binary WKB data.
     It can be converted to a hexadecimal representation of the data using str()
     and compared to a hexadecimal representation with the normal equality operator."""
 
     def __new__(cls, data):
         if not isinstance(data, (bytes, bytearray)):
             data = unhexlify(str(data))
-        elif data[:2] in (b'00', b'01'):  # hex-encoded string as bytes
-            data = unhexlify(data.decode('ascii'))
+        elif data[:2] in (b"00", b"01"):  # hex-encoded string as bytes
+            data = unhexlify(data.decode("ascii"))
         return bytes.__new__(cls, data)
 
     def __str__(self):
-        return hexlify(self).decode('ascii')
+        return hexlify(self).decode("ascii")
 
     def __eq__(self, other):
-        if isinstance(other, str) and other[:2] in ('00', '01'):
+        if isinstance(other, str) and other[:2] in ("00", "01"):
             other = unhexlify(other)
         return super().__eq__(other)
```

### Comparing `plpygis-0.4.0/pyproject.toml` & `plpygis-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plpygis-0.4.0/test/test_geometry.py` & `plpygis-0.4.1/test/test_geometry.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 Test Geometry
 """
 
 import pytest
 from shapely import geometry
 from plpygis import Geometry, Point, LineString, Polygon
 from plpygis import MultiPoint, MultiLineString, MultiPolygon, GeometryCollection
-from plpygis.exceptions import WkbError, SridError, DimensionalityError, CoordinateError, GeojsonError
+from plpygis.exceptions import WkbError, SridError, DimensionalityError, CoordinateError, GeojsonError, CollectionError
+from copy import copy
 
 geojson_pt = {"type":"Point","coordinates":[0.0,0.0]}
 geojson_ln = {"type":"LineString","coordinates":[[107,60],[102,59]]}
 geojson_pg = {"type":"Polygon","coordinates":[[[100,0],[101.0,0.0],[101.0,1.0],[100.0,1.0],[100.0,0.0]]]}
 geojson_mpt = {"type":"MultiPoint","coordinates":[[0,0],[1,1]]}
 geojson_mln = {"type":"MultiLineString","coordinates":[[[0,0],[1,1]],[[2,2],[3,3]]]}
 geojson_mpg = {"type":"MultiPolygon","coordinates":[[[[1,0],[111,0.0],[101.0,1.0],[100.0,1.0],[1,0]]],[[[100,0],[101.0,0.0],[101.0,1.0],[100.0,1.0],[100.0,0.0]]]]}
@@ -140,14 +141,24 @@
     geom.srid = geom.srid # clear cached WKB
     postgis_type = "geometry(PointZM,4326)"
     assert geom.postgis_type == postgis_type
     assert geom.__repr__() == "<Point: 'geometry(PointZM,4326)'>"
     geom.srid = geom.srid # clear cached WKB
     assert geom.__str__().lower() == wkb.lower()
 
+def test_read_wkb_data_error():
+    """
+    read WKB with good header but malformed data
+    """
+    wkb = "0000000001000000000000"
+    geom = Geometry(wkb)
+    assert geom.type == "Point"
+    with pytest.raises(WkbError):
+        geom.x
+
 def test_read_wkb_linestring():
     """
     read WKB LineString
     """
     wkb = wkb_ln
     geom = Geometry(wkb)
     assert geom.type == "LineString"
@@ -191,14 +202,17 @@
     postgis_type = "geometry(MultiPointZ)"
     assert geom.postgis_type == postgis_type
     assert geom.__repr__() == "<MultiPoint: 'geometry(MultiPointZ)'>"
     geom.srid = geom.srid # clear cached WKB
     assert geom.__str__().lower() == wkb.lower()
     for g in geom.geometries:
         assert g.type == "Point"
+    for g in geom.points:
+        assert g.type == "Point"
+    assert wkb == geom.wkb
 
 def test_read_wkb_multilinestring():
     """
     read WKB MultiLineString
     """
     wkb = wkb_mln
     geom = Geometry(wkb)
@@ -209,14 +223,17 @@
     postgis_type = "geometry(MultiLineStringM)"
     assert geom.postgis_type == postgis_type
     assert geom.__repr__() == "<MultiLineString: 'geometry(MultiLineStringM)'>"
     geom.srid = geom.srid # clear cached WKB
     assert geom.__str__().lower() == wkb.lower()
     for g in geom.geometries:
         assert g.type == "LineString"
+    for g in geom.linestrings:
+        assert g.type == "LineString"
+    assert wkb == geom.wkb
 
 def test_read_wkb_multipolygon():
     """
     read WKB MultiPolygon
     """
     wkb = wkb_mpg
     geom = Geometry(wkb)
@@ -227,14 +244,17 @@
     postgis_type = "geometry(MultiPolygon)"
     assert geom.postgis_type == postgis_type
     assert geom.__repr__() == "<MultiPolygon: 'geometry(MultiPolygon)'>"
     geom.srid = geom.srid # clear cached WKB
     assert geom.__str__().lower() == wkb.lower()
     for g in geom.geometries:
         assert g.type == "Polygon"
+    for g in geom.polygons:
+        assert g.type == "Polygon"
+    assert wkb == geom.wkb
 
 def test_read_wkb_geometrycollection():
     """
     read WKB GeometryCollection
     """
     wkb = wkb_gc
     geom = Geometry(wkb)
@@ -245,14 +265,36 @@
     postgis_type = "geometry(GeometryCollection)"
     assert geom.postgis_type == postgis_type
     assert geom.__repr__() == "<GeometryCollection: 'geometry(GeometryCollection)'>"
     geom.srid = geom.srid # clear cached WKB
     assert geom.__str__().lower() == wkb.lower()
     assert geom.geometries[0].type == "Point"
     assert geom.geometries[1].type == "LineString"
+    assert wkb == geom.wkb
+
+def test_multigeometry_raise_error():
+    """
+    raise error when adding wrong type to a multigeometry
+    """
+    pt = Point((0,1))
+    ls = LineString([(0,1), (2,3)])
+
+    MultiPoint([pt, copy(pt)])
+
+    with pytest.raises(CollectionError):
+        MultiPoint([pt, ls])
+
+    with pytest.raises(CollectionError):
+        MultiLineString([pt, ls])
+
+    with pytest.raises(CollectionError):
+        MultiPolygon([pt, ls])
+
+    with pytest.raises(CollectionError):
+        GeometryCollection([pt, ls, True])
 
 def test_multigeometry_changedimensionality():
     """
     change dimensionality of a MultiGeometry
     """
     wkb = wkb_gc
     geom = Geometry(wkb)
@@ -669,16 +711,14 @@
     assert mp.coordinates == coordinates
 
 def test_point_copy():
     """
     copy a Point object
     """
     p1 = Point((0, 1, 2), srid=4326, dimm=True)
-
-    from copy import copy
     p2 = copy(p1)
     p3 = copy(p1)
 
     assert p1.coordinates == p2.coordinates
     assert p1.srid == p2.srid
     assert p1.wkb == p2.wkb
     assert p1 != p2
@@ -705,30 +745,26 @@
     """
     copy a MultiPoint object
     """
     p1 = Point((0, 1, 2))
     p2 = Point((3, 4, 5))
     p3 = Point((6, 7, 8))
     mp1 = MultiPoint([p1, p2, p3], srid=4326)
-
-    from copy import copy
     mp2 = copy(mp1)
 
     assert mp1.coordinates == mp2.coordinates
 
 def test_geometrycollection_create():
     """
     create a GeometryCollection object
     """
     pt = Point((0, 1, 2))
     ls = LineString([(3, 4, 5), (9, 10, 11)])
     pl = Polygon([[(1, 2, 3), (6, 7, 8), (10, 11, 12), (1, 2, 3)]])
     gc1 = GeometryCollection([pt, ls, pl])
-
-    from copy import copy
     gc2 = copy(gc1)
     assert gc1.coordinates == gc2.coordinates
 
     pt.x = 100
     assert gc1.coordinates != gc2.coordinates
 
     gc1.geometries[0].x = 200
@@ -739,16 +775,14 @@
     modify a GeometryCollection object
     """
     pt = Point((0, 1, 2))
     ls = LineString([(3, 4, 5), (9, 10, 11)])
     pl = Polygon([[(1, 2, 3), (6, 7, 8), (10, 11, 12), (1, 2, 3)]])
     gc1 = GeometryCollection([pt, ls, pl])
     gc1.wkb
-
-    from copy import copy
     gc2 = copy(gc1)
     assert gc1.wkb == gc2.wkb
 
     pt = Point((-1, -5, -1))
     gc2.geometries[1] = pt
 
     assert gc1.coordinates != gc2.coordinates
```

