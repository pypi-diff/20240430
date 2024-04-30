# Comparing `tmp/owimetadatabase_preprocessor-0.8.0.tar.gz` & `tmp/owimetadatabase_preprocessor-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owimetadatabase_preprocessor-0.8.0.tar", max compression
+gzip compressed data, was "owimetadatabase_preprocessor-0.8.1.tar", max compression
```

## Comparing `owimetadatabase_preprocessor-0.8.0.tar` & `owimetadatabase_preprocessor-0.8.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35148 2024-04-23 13:42:33.936551 owimetadatabase_preprocessor-0.8.0/LICENSE
--rw-r--r--   0        0        0     1471 2024-04-23 13:42:33.936551 owimetadatabase_preprocessor-0.8.0/README.md
--rw-r--r--   0        0        0     2535 2024-04-23 13:42:33.936551 owimetadatabase_preprocessor-0.8.0/pyproject.toml
--rw-r--r--   0        0        0       84 2024-04-23 13:42:33.940551 owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/__init__.py
--rw-r--r--   0        0        0       66 2024-04-23 13:42:33.940551 owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/fatigue/__init__.py
--rw-r--r--   0        0        0    34147 2024-04-23 13:42:33.940551 owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/fatigue/data_objects.py
--rw-r--r--   0        0        0    24890 2024-04-23 13:42:33.940551 owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/fatigue/io.py
--rw-r--r--   0        0        0       40 2024-04-23 13:42:33.940551 owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/geometry/__init__.py
--rw-r--r--   0        0        0    11835 2024-04-23 13:42:33.940551 owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/geometry/io.py
--rw-r--r--   0        0        0    38307 2024-04-23 13:42:33.940551 owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/geometry/processing.py
--rw-r--r--   0        0        0    24884 2024-04-23 13:42:33.940551 owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/geometry/structures.py
--rw-r--r--   0        0        0     7067 2024-04-23 13:42:33.940551 owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/io.py
--rw-r--r--   0        0        0       41 2024-04-23 13:42:33.940551 owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/locations/__init__.py
--rw-r--r--   0        0        0     8155 2024-04-23 13:42:33.940551 owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/locations/io.py
--rw-r--r--   0        0        0        0 2024-04-23 13:42:33.940551 owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/soil/__init__.py
--rw-r--r--   0        0        0    87680 2024-04-23 13:42:33.940551 owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/soil/io.py
--rw-r--r--   0        0        0     7268 2024-04-23 13:42:33.940551 owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/utils.py
--rw-r--r--   0        0        0     3748 1970-01-01 00:00:00.000000 owimetadatabase_preprocessor-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-04-30 08:33:48.953993 owimetadatabase_preprocessor-0.8.1/LICENSE
+-rw-r--r--   0        0        0     1471 2024-04-30 08:33:48.957993 owimetadatabase_preprocessor-0.8.1/README.md
+-rw-r--r--   0        0        0     2535 2024-04-30 08:33:48.957993 owimetadatabase_preprocessor-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0       84 2024-04-30 08:33:48.957993 owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/__init__.py
+-rw-r--r--   0        0        0       66 2024-04-30 08:33:48.957993 owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/fatigue/__init__.py
+-rw-r--r--   0        0        0    34147 2024-04-30 08:33:48.957993 owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/fatigue/data_objects.py
+-rw-r--r--   0        0        0    24890 2024-04-30 08:33:48.957993 owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/fatigue/io.py
+-rw-r--r--   0        0        0       40 2024-04-30 08:33:48.957993 owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/geometry/__init__.py
+-rw-r--r--   0        0        0    11835 2024-04-30 08:33:48.957993 owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/geometry/io.py
+-rw-r--r--   0        0        0    38484 2024-04-30 08:33:48.957993 owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/geometry/processing.py
+-rw-r--r--   0        0        0    24884 2024-04-30 08:33:48.957993 owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/geometry/structures.py
+-rw-r--r--   0        0        0     7067 2024-04-30 08:33:48.957993 owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/io.py
+-rw-r--r--   0        0        0       41 2024-04-30 08:33:48.961993 owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/locations/__init__.py
+-rw-r--r--   0        0        0     8155 2024-04-30 08:33:48.961993 owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/locations/io.py
+-rw-r--r--   0        0        0        0 2024-04-30 08:33:48.961993 owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/soil/__init__.py
+-rw-r--r--   0        0        0    87680 2024-04-30 08:33:48.961993 owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/soil/io.py
+-rw-r--r--   0        0        0     7268 2024-04-30 08:33:48.961993 owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/utils.py
+-rw-r--r--   0        0        0     3748 1970-01-01 00:00:00.000000 owimetadatabase_preprocessor-0.8.1/PKG-INFO
```

### Comparing `owimetadatabase_preprocessor-0.8.0/LICENSE` & `owimetadatabase_preprocessor-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `owimetadatabase_preprocessor-0.8.0/README.md` & `owimetadatabase_preprocessor-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `owimetadatabase_preprocessor-0.8.0/pyproject.toml` & `owimetadatabase_preprocessor-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "owimetadatabase-preprocessor"
-version = "0.8.0"
+version = "0.8.1"
 description = "Package for preprocessing data from owimetadatabase."
 authors = ["arsmlnkv <melnikov.arsene@gmail.com>"]
 readme = "README.md"
 homepage = "https://owi-lab.github.io/owimetadatabase-preprocessor/"
 repository = "https://github.com/OWI-Lab/owimetadatabase-preprocessor"
 license = "GNU General Public License v3.0"
 keywords = ["owimetadatabase"]
```

### Comparing `owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/fatigue/data_objects.py` & `owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/fatigue/data_objects.py`

 * *Files identical despite different names*

### Comparing `owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/fatigue/io.py` & `owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/fatigue/io.py`

 * *Files identical despite different names*

### Comparing `owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/geometry/io.py` & `owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/geometry/io.py`

 * *Files identical despite different names*

### Comparing `owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/geometry/processing.py` & `owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/geometry/processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,18 +198,18 @@
             df = deepcopy(self.mp_sub_assemblies.loc[df_index, cols])
             toe = self.pile_head - df["height"].sum() * 1e-3
             self.pile_toe = round(toe, 3)
             depth_to = toe + df.z * 1e-3
             depth_from = depth_to + df.height * 1e-3
         else:
             raise ValueError("Unknown index.")
-        df["Depth from [mLAT]"] = depth_from
-        df["Depth to [mLAT]"] = depth_to
+        df["Elevation from [mLAT]"] = depth_from
+        df["Elevation to [mLAT]"] = depth_to
         # Round elevations to mm to avoid numerical inconsistencies later when setting altitude values to apply loads.
-        df = df.round({"Depth from [mLAT]": 3, "Depth to [mLAT]": 3})
+        df = df.round({"Elevation from [mLAT]": 3, "Elevation to [mLAT]": 3})
         return df
 
     def process_structure_geometry(self, idx: str) -> pd.DataFrame:
         """Calculate and/or converts geometrical data of subassemblies from the database to use as input for FE models.
 
         :param idx: Possible index to identify corresponding subassembly.
         :return: Dataframe consisting of the required data to build FE models.
@@ -228,16 +228,16 @@
         df["Diameter to [m]"] = np.array(d_to, dtype=float) * 1e-3
         df["rho [t/m]"] = df["mass"] / df["height"]
         df["Mass [t]"] = df["mass"] * 1e-3
         df["Height [m]"] = df["height"] * 1e-3
         df["Youngs modulus [GPa]"] = 210
         df["Poissons ratio [-]"] = 0.3
         cols = [
-            "Depth from [mLAT]",
-            "Depth to [mLAT]",
+            "Elevation from [mLAT]",
+            "Elevation to [mLAT]",
             "Height [m]",
             "Diameter from [m]",
             "Diameter to [m]",
             "Volume [m3]",
             "Wall thickness [mm]",
             "Youngs modulus [GPa]",
             "Poissons ratio [-]",
@@ -447,15 +447,15 @@
         """Recalculation of can properties based on section properties and can elevations: height [m],
         volume [m3], mass [t], rho [t/m].
 
         :param row: Original can properties.
         :return: Pandas series of recalculated can properties.
         """
         density = row["Mass [t]"] / row["Volume [m3]"]
-        height = row["Depth from [mLAT]"] - row["Depth to [mLAT]"]
+        height = row["Elevation from [mLAT]"] - row["Elevation to [mLAT]"]
         r1 = row["Diameter from [m]"] / 2
         r2 = row["Diameter to [m]"] / 2
         volume_out = 1 / 3 * np.pi * (r1**2 + r1 * r2 + r2**2) * height
         wall_thickness = row["Wall thickness [mm]"] * 1e-3
         r1 = r1 - wall_thickness
         r2 = r2 - wall_thickness
         volume_in = 1 / 3 * np.pi * (r1**2 + r1 * r2 + r2**2) * height
@@ -483,16 +483,19 @@
         """
         if position == "bottom":
             ind = -1
             _col = " to "
         else:
             ind = 0
             _col = " from "
-        df.loc[df.index[ind], "Depth" + _col + "[mLAT]"] = altitude  # type: ignore
-        elevation = [df.iloc[ind]["Depth from [mLAT]"], df.iloc[ind]["Depth to [mLAT]"]]
+        df.loc[df.index[ind], "Elevation" + _col + "[mLAT]"] = altitude  # type: ignore
+        elevation = [
+            df.iloc[ind]["Elevation from [mLAT]"],
+            df.iloc[ind]["Elevation to [mLAT]"],
+        ]
         diameters = [df.iloc[ind]["Diameter from [m]"], df.iloc[ind]["Diameter to [m]"]]
         df.loc[df.index[ind], "Diameter" + _col + "[m]"] = np.interp(
             [altitude], elevation, diameters  # type: ignore
         )[0]
         cols = ["Height [m]", "Volume [m3]", "Mass [t]", "rho [t/m]"]
         df.loc[df.index[ind], cols] = self.can_adjust_properties(df.iloc[ind])
         return df
@@ -503,23 +506,23 @@
 
         :return: None
         """
         self._init_spec_part = True
         if (self.transition_piece is not None) and (self.monopile is not None):
             mp_head = self.pile_head
             tp = self.transition_piece
-            df = deepcopy(tp[tp["Depth from [mLAT]"] > mp_head])
-            if df.loc[df.index[0], "Depth to [mLAT]"] != mp_head:
+            df = deepcopy(tp[tp["Elevation from [mLAT]"] > mp_head])
+            if df.loc[df.index[0], "Elevation to [mLAT]"] != mp_head:
                 # Not bolted connection (i.e. Rentel) preprocessing needed
                 tp1 = self.can_modification(df, mp_head, position="bottom")
                 self.substructure = pd.concat([tp1, deepcopy(self.monopile)])
             else:
                 # Bolted connection, nothing to do
                 self.substructure = pd.concat([df, deepcopy(self.monopile)])
-            df = deepcopy(tp[tp["Depth to [mLAT]"] < mp_head])
+            df = deepcopy(tp[tp["Elevation to [mLAT]"] < mp_head])
             self.tp_skirt = self.can_modification(df, mp_head, position="top")
         else:
             raise TypeError("TP or MP items need to be processed before!")
 
     def assembly_full_structure(self) -> None:
         """Process the full structure of the OWT: tower + tp combiantion with monopile.
 
@@ -570,16 +573,18 @@
         if self.mp_sub_assemblies is not None:
             df = self.mp_sub_assemblies.copy()
         else:
             raise ValueError("Monopile subassembly data not found.")
         df.reset_index(inplace=True)
         for i, row in df.iterrows():
             if i != 0:
-                pile.loc[i, "Depth from [m]"] = penetration - 1e-3 * df["z"].iloc[i - 1]
-                pile.loc[i, "Depth to [m]"] = penetration - 1e-3 * row["z"]
+                pile.loc[i, "Elevation from [m]"] = (
+                    penetration - 1e-3 * df["z"].iloc[i - 1]
+                )
+                pile.loc[i, "Elevation to [m]"] = penetration - 1e-3 * row["z"]
                 pile.loc[i, "Pile material"] = (
                     self.sub_assemblies["MP"].bb[0].material.title
                 )
                 pile.loc[i, "Pile material submerged unit weight [kN/m3]"] = (
                     1e-2 * self.sub_assemblies["MP"].bb[0].material.density - 10
                 )
                 pile.loc[i, "Wall thickness [mm]"] = row["wall_thickness"]
@@ -591,16 +596,18 @@
                 pile.loc[i, "Youngs modulus [GPa]"] = (
                     self.sub_assemblies["MP"].bb[0].material.young_modulus
                 )
                 pile.loc[i, "Poissons ratio [-]"] = (
                     self.sub_assemblies["MP"].bb[0].material.poisson_ratio
                 )
         if not np.math.isnan(cutoff_point):
-            pile = pile.loc[pile["Depth to [m]"] > cutoff_point].reset_index(drop=True)
-            pile.loc[0, "Depth from [m]"] = cutoff_point
+            pile = pile.loc[pile["Elevation to [m]"] > cutoff_point].reset_index(
+                drop=True
+            )
+            pile.loc[0, "Elevation from [m]"] = cutoff_point
         return pile
 
     def __eq__(self, other) -> bool:
         if isinstance(other, type(self)):
             comp = deepcompare(self, other)
             assert comp[0], comp[1]
         elif isinstance(other, dict):
```

### Comparing `owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/geometry/structures.py` & `owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/geometry/structures.py`

 * *Files identical despite different names*

### Comparing `owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/io.py` & `owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/io.py`

 * *Files identical despite different names*

### Comparing `owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/locations/io.py` & `owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/locations/io.py`

 * *Files identical despite different names*

### Comparing `owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/soil/io.py` & `owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/soil/io.py`

 * *Files identical despite different names*

### Comparing `owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/utils.py` & `owimetadatabase_preprocessor-0.8.1/src/owimetadatabase_preprocessor/utils.py`

 * *Files identical despite different names*

### Comparing `owimetadatabase_preprocessor-0.8.0/PKG-INFO` & `owimetadatabase_preprocessor-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owimetadatabase-preprocessor
-Version: 0.8.0
+Version: 0.8.1
 Summary: Package for preprocessing data from owimetadatabase.
 Home-page: https://owi-lab.github.io/owimetadatabase-preprocessor/
 License: GNU General Public License v3.0
 Keywords: owimetadatabase
 Author: arsmlnkv
 Author-email: melnikov.arsene@gmail.com
 Requires-Python: >=3.9,<3.13
```

