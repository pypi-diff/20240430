# Comparing `tmp/gcp_pal-1.0.7.tar.gz` & `tmp/gcp_pal-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcp_pal-1.0.7.tar", max compression
+gzip compressed data, was "gcp_pal-1.0.8.tar", max compression
```

## Comparing `gcp_pal-1.0.7.tar` & `gcp_pal-1.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    28062 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/README.md
--rw-r--r--   0        0        0      865 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/gcp_pal/__init__.py
--rw-r--r--   0        0        0    31457 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/gcp_pal/bigquery.py
--rw-r--r--   0        0        0    13156 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/gcp_pal/cloudfunctions.py
--rw-r--r--   0        0        0    13920 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/gcp_pal/cloudrun.py
--rw-r--r--   0        0        0     7754 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/gcp_pal/cloudscheduler.py
--rw-r--r--   0        0        0       42 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/gcp_pal/config/__init__.py
--rw-r--r--   0        0        0     1094 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/gcp_pal/config/vars.py
--rw-r--r--   0        0        0    24859 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/gcp_pal/dataplex.py
--rw-r--r--   0        0        0    12490 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/gcp_pal/firestore.py
--rw-r--r--   0        0        0     3170 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/gcp_pal/project.py
--rw-r--r--   0        0        0     1674 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/gcp_pal/pubsub.py
--rw-r--r--   0        0        0     3873 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/gcp_pal/pydocker.py
--rw-r--r--   0        0        0     6975 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/gcp_pal/pylogging.py
--rw-r--r--   0        0        0     4737 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/gcp_pal/request.py
--rw-r--r--   0        0        0    23631 2024-04-30 08:29:13.014220 gcp_pal-1.0.7/gcp_pal/schema.py
--rw-r--r--   0        0        0     6332 2024-04-30 08:29:13.018220 gcp_pal-1.0.7/gcp_pal/secretmanager.py
--rw-r--r--   0        0        0       88 2024-04-30 08:29:13.018220 gcp_pal-1.0.7/gcp_pal/storage/__init__.py
--rw-r--r--   0        0        0     8735 2024-04-30 08:29:13.018220 gcp_pal-1.0.7/gcp_pal/storage/parquet.py
--rw-r--r--   0        0        0    17224 2024-04-30 08:29:13.018220 gcp_pal-1.0.7/gcp_pal/storage/storage.py
--rw-r--r--   0        0        0       82 2024-04-30 08:29:13.018220 gcp_pal-1.0.7/gcp_pal/utils/__init__.py
--rw-r--r--   0        0        0      935 2024-04-30 08:29:13.018220 gcp_pal-1.0.7/gcp_pal/utils/lazy_loader.py
--rw-r--r--   0        0        0    11431 2024-04-30 08:29:13.018220 gcp_pal-1.0.7/gcp_pal/utils/utils.py
--rw-r--r--   0        0        0     1051 2024-04-30 08:29:13.018220 gcp_pal-1.0.7/pyproject.toml
--rw-r--r--   0        0        0    28511 1970-01-01 00:00:00.000000 gcp_pal-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0    28062 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/README.md
+-rw-r--r--   0        0        0      865 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/__init__.py
+-rw-r--r--   0        0        0    31457 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/bigquery.py
+-rw-r--r--   0        0        0    13156 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/cloudfunctions.py
+-rw-r--r--   0        0        0    13920 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/cloudrun.py
+-rw-r--r--   0        0        0     7754 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/cloudscheduler.py
+-rw-r--r--   0        0        0       42 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/config/__init__.py
+-rw-r--r--   0        0        0     1094 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/config/vars.py
+-rw-r--r--   0        0        0    26783 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/dataplex.py
+-rw-r--r--   0        0        0    12490 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/firestore.py
+-rw-r--r--   0        0        0     3170 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/project.py
+-rw-r--r--   0        0        0     1674 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/pubsub.py
+-rw-r--r--   0        0        0     3873 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/pydocker.py
+-rw-r--r--   0        0        0     6975 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/pylogging.py
+-rw-r--r--   0        0        0     4737 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/request.py
+-rw-r--r--   0        0        0    23631 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/schema.py
+-rw-r--r--   0        0        0     6332 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/secretmanager.py
+-rw-r--r--   0        0        0       88 2024-04-30 10:30:09.063612 gcp_pal-1.0.8/gcp_pal/storage/__init__.py
+-rw-r--r--   0        0        0     8735 2024-04-30 10:30:09.063612 gcp_pal-1.0.8/gcp_pal/storage/parquet.py
+-rw-r--r--   0        0        0    17224 2024-04-30 10:30:09.063612 gcp_pal-1.0.8/gcp_pal/storage/storage.py
+-rw-r--r--   0        0        0       82 2024-04-30 10:30:09.063612 gcp_pal-1.0.8/gcp_pal/utils/__init__.py
+-rw-r--r--   0        0        0      935 2024-04-30 10:30:09.063612 gcp_pal-1.0.8/gcp_pal/utils/lazy_loader.py
+-rw-r--r--   0        0        0    11431 2024-04-30 10:30:09.063612 gcp_pal-1.0.8/gcp_pal/utils/utils.py
+-rw-r--r--   0        0        0     1051 2024-04-30 10:30:09.063612 gcp_pal-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0    28511 1970-01-01 00:00:00.000000 gcp_pal-1.0.8/PKG-INFO
```

### Comparing `gcp_pal-1.0.7/README.md` & `gcp_pal-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.7/gcp_pal/__init__.py` & `gcp_pal-1.0.8/gcp_pal/__init__.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.7/gcp_pal/bigquery.py` & `gcp_pal-1.0.8/gcp_pal/bigquery.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.7/gcp_pal/cloudfunctions.py` & `gcp_pal-1.0.8/gcp_pal/cloudfunctions.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.7/gcp_pal/cloudrun.py` & `gcp_pal-1.0.8/gcp_pal/cloudrun.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.7/gcp_pal/cloudscheduler.py` & `gcp_pal-1.0.8/gcp_pal/cloudscheduler.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.7/gcp_pal/config/vars.py` & `gcp_pal-1.0.8/gcp_pal/config/vars.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.7/gcp_pal/dataplex.py` & `gcp_pal-1.0.8/gcp_pal/dataplex.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,17 +38,18 @@
 
         self.project = project or os.environ.get("PROJECT") or get_auth_default()[1]
         self.location = location
 
         self.lake = lake
         self.zone = zone
         self.asset = asset
+
         if isinstance(path, str) and path.startswith("projects/"):
-            paths = path.split("/")[1::2][2:]
-            path = "/".join(paths)
+            path = self._convert_full_id_to_path(path)
+
         try:
             # e.g. path = "lake" or "lake/zone" or "lake/zone/asset"
             self.lake = path.split("/")[0]
         except:
             pass
         try:
             # e.g. path = "lake/zone" or "lake/zone/asset"
@@ -149,14 +150,30 @@
             parent += ""
         elif self.type == "zone":
             parent += f"/lakes/{self.lake}"
         elif self.type == "asset":
             parent += f"/lakes/{self.lake}/zones/{self.zone}"
         return parent
 
+    def _convert_full_id_to_path(self, full_id):
+        """
+        Converts the full resource ID to the path of the form "lake/zone/asset" or "lake/zone" or "lake" or None.
+
+        Args:
+        - full_id (str): The full resource ID.
+
+        Returns:
+        - (str): The path of the resource.
+        """
+        if not full_id:
+            return None
+        paths = full_id.split("/")[1::2][2:]
+        path = "/".join(paths)
+        return path
+
     def get_lake(self):
         """
         Retrieves the lake resource.
 
         Returns:
         - (dict): The lake resource.
         """
@@ -480,72 +497,108 @@
         Returns:
         - (list): The list of lakes.
         """
         parent = name or self.parent
         lakes = self.client.list_lakes(parent=parent)
         output = [lake.name for lake in lakes]
         if not full_id:
-            output = [name.split("/")[-1] for name in output]
+            output = [self._convert_full_id_to_path(name) for name in output]
         return output
 
     def ls_zones(self, name=None, full_id=False):
         """
         Lists the zones in the lake.
 
         Args:
         - name (str): Optional path of the zone.
         - full_id (bool): If True, returns the full resource ID of the zones. Otherwise returns the path of form "lake/zone".
 
         Returns:
         - (list): The list of zones.
         """
-        parent = name or f"{self.parent}/lakes/{self.lake}"
-        zones = self.client.list_zones(parent=parent)
-        output = [zone.name for zone in zones]
+        output = []
+        if self.type == "project":
+            # Listing all zones in the project
+            zones = []
+            lakes = self.ls_lakes(full_id=True)
+            for lake in lakes:
+                lake = Dataplex(path=lake)
+                zones = lake.ls_zones(full_id=True)
+                output += zones
+        else:
+            parent = name or f"{self.parent}/lakes/{self.lake}"
+            zones = self.client.list_zones(parent=parent)
+            output = [zone.name for zone in zones]
         if not full_id:
-            zones = [name.split("/")[-1] for name in output]
-            output = [f"{self.lake}/{zone}" for zone in zones]
+            output = [self._convert_full_id_to_path(name) for name in output]
         return output
 
     def ls_assets(self, name=None, full_id=False):
         """
         Lists the assets in the zone.
 
         Args:
         - name (str): Optional path of the asset.
         - full_id (bool): If True, returns the full resource ID of the assets. Otherwise returns the path of form "lake/zone/asset".
 
         Returns:
         - (list): The list of assets.
         """
-        parent = name or f"{self.parent}/zones/{self.zone}"
-        assets = self.client.list_assets(parent=parent)
-        output = [asset.name for asset in assets]
+        output = []
+        if self.type == "project":
+            # Listing all assets in the project
+            assets = []
+            lakes = self.ls_lakes(full_id=True)
+            for lake in lakes:
+                lake = Dataplex(path=lake)
+                zones = lake.ls_zones(full_id=True)
+                for zone in zones:
+                    zone = Dataplex(path=zone)
+                    assets = zone.ls_assets(full_id=True)
+                    output += assets
+        elif self.type == "lake":
+            # Listing all assets in the lake
+            zones = self.ls_zones(full_id=True)
+            for zone in zones:
+                zone = Dataplex(path=zone)
+                assets = zone.ls_assets(full_id=True)
+                output += assets
+        else:
+            parent = name or f"{self.parent}/zones/{self.zone}"
+            assets = self.client.list_assets(parent=parent)
+            output = [asset.name for asset in assets]
         if not full_id:
-            assets = [name.split("/")[-1] for name in output]
-            output = [f"{self.lake}/{self.zone}/{asset}" for asset in assets]
+            output = [self._convert_full_id_to_path(name) for name in output]
         return output
 
-    def ls(self, full_id=False):
+    def ls(self, level=None, full_id=False):
         """
         Lists the resources.
 
         Args:
+        - level (str): The level of the resources to list. Either "lakes", "zones" or "assets".
         - full_id (bool): If True, returns the full resource ID of the resources.
 
         Returns:
         - (list): The list of resources.
         """
         if self.type == "asset":
             raise ValueError("The method 'Dataplex.ls' is not supported for assets.")
-        list_method = {
-            "project": self.ls_lakes,
-            "lake": self.ls_zones,
-            "zone": self.ls_assets,
-        }.get(self.type)
+        if level:
+            list_method = {
+                "lakes": self.ls_lakes,
+                "zones": self.ls_zones,
+                "assets": self.ls_assets,
+            }.get(level)
+        else:
+            list_method = {
+                "project": self.ls_lakes,
+                "lake": self.ls_zones,
+                "zone": self.ls_assets,
+            }.get(self.type)
         output = list_method(full_id=full_id)
         return output
 
     def exists(self):
         """
         Checks if the resource exists.
 
@@ -675,29 +728,31 @@
         return output
 
 
 if __name__ == "__main__":
     # Example: Create a Dataplex object
     from gcp_pal import BigQuery
 
-    lake_name = "test-lake1"
-    zone_name = "test-zone1"
-    Dataplex(path="artem-lake2").create_lake()
-    Dataplex(path=f"{lake_name}/{zone_name}").create_zone(
-        zone_type="raw", location_type="single-region"
-    )
-    BigQuery(dataset="dataplex_dataset1").create()
-    BigQuery(dataset="dataplex_dataset2").create()
-    Dataplex(
-        path=f"{lake_name}/{zone_name}/test-asset1",
-    ).create_asset(
-        asset_source="dataplex_dataset1",
-        asset_type="bigquery",
-    )
-    Dataplex(
-        path=f"{lake_name}/{zone_name}/test-asset2",
-    ).create_asset(
-        asset_source="dataplex_dataset2",
-        asset_type="bigquery",
-    )
+    print(Dataplex().ls(level="assets", full_id=False))
+
+    # lake_name = "artem-lake3"
+    # zone_name = "artem-zone3"
+    # Dataplex(path=lake_name).create_lake()
+    # Dataplex(path=f"{lake_name}/{zone_name}").create_zone(
+    #     zone_type="raw", location_type="single-region"
+    # )
+    # # BigQuery(dataset="dataplex_dataset1").create()
+    # # BigQuery(dataset="dataplex_dataset2").create()
+    # Dataplex(
+    #     path=f"{lake_name}/{zone_name}/test-asset1",
+    # ).create_asset(
+    #     asset_source="dataplex_dataset1",
+    #     asset_type="bigquery",
+    # )
+    # Dataplex(
+    #     path=f"{lake_name}/{zone_name}/test-asset2",
+    # ).create_asset(
+    #     asset_source="dataplex_dataset2",
+    #     asset_type="bigquery",
+    # )
 
-    Dataplex(lake_name, location="europe-west2").delete()
+    # Dataplex(lake_name, location="europe-west2").delete()
```

### Comparing `gcp_pal-1.0.7/gcp_pal/firestore.py` & `gcp_pal-1.0.8/gcp_pal/firestore.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.7/gcp_pal/project.py` & `gcp_pal-1.0.8/gcp_pal/project.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.7/gcp_pal/pubsub.py` & `gcp_pal-1.0.8/gcp_pal/pubsub.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.7/gcp_pal/pydocker.py` & `gcp_pal-1.0.8/gcp_pal/pydocker.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.7/gcp_pal/pylogging.py` & `gcp_pal-1.0.8/gcp_pal/pylogging.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.7/gcp_pal/request.py` & `gcp_pal-1.0.8/gcp_pal/request.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.7/gcp_pal/schema.py` & `gcp_pal-1.0.8/gcp_pal/schema.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.7/gcp_pal/secretmanager.py` & `gcp_pal-1.0.8/gcp_pal/secretmanager.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.7/gcp_pal/storage/parquet.py` & `gcp_pal-1.0.8/gcp_pal/storage/parquet.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.7/gcp_pal/storage/storage.py` & `gcp_pal-1.0.8/gcp_pal/storage/storage.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.7/gcp_pal/utils/lazy_loader.py` & `gcp_pal-1.0.8/gcp_pal/utils/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.7/gcp_pal/utils/utils.py` & `gcp_pal-1.0.8/gcp_pal/utils/utils.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.7/pyproject.toml` & `gcp_pal-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gcp-pal"
-version = "1.0.7"
+version = "1.0.8"
 description = "Set of utilities for interacting with Google Cloud Platform"
 authors = ["VitaminB16 <artemiy.nosov@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `gcp_pal-1.0.7/PKG-INFO` & `gcp_pal-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcp-pal
-Version: 1.0.7
+Version: 1.0.8
 Summary: Set of utilities for interacting with Google Cloud Platform
 Author: VitaminB16
 Author-email: artemiy.nosov@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

