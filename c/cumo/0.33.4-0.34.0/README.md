# Comparing `tmp/cumo-0.33.4.tar.gz` & `tmp/cumo-0.34.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cumo-0.33.4.tar", max compression
+gzip compressed data, was "cumo-0.34.0.tar", max compression
```

## Comparing `cumo-0.33.4.tar` & `cumo-0.34.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1275 2024-04-17 11:54:20.796681 cumo-0.33.4/README.md
--rw-r--r--   0        0        0        7 2022-05-27 04:27:01.699189 cumo-0.33.4/cumo/.gitignore
--rw-r--r--   0        0        0      117 2022-05-27 04:27:01.699189 cumo-0.33.4/cumo/__init__.py
--rw-r--r--   0        0        0     3683 2024-04-12 05:59:32.220796 cumo-0.33.4/cumo/__main__.py
--rw-r--r--   0        0        0        9 2022-05-27 04:27:01.699189 cumo-0.33.4/cumo/_internal/.gitignore
--rw-r--r--   0        0        0        0 2022-05-27 04:27:01.699189 cumo-0.33.4/cumo/_internal/__init__.py
--rw-r--r--   0        0        0     1675 2023-09-13 10:26:38.801824 cumo-0.33.4/cumo/_internal/down_sample.py
--rw-r--r--   0        0        0        0 2022-05-27 04:27:01.699189 cumo-0.33.4/cumo/_internal/members/__init__.py
--rw-r--r--   0        0        0     8722 2023-09-13 10:26:38.801824 cumo-0.33.4/cumo/_internal/members/camera.py
--rw-r--r--   0        0        0     1177 2022-05-27 04:27:01.699189 cumo-0.33.4/cumo/_internal/members/capture_screen.py
--rw-r--r--   0        0        0    12413 2022-05-27 04:27:01.699189 cumo-0.33.4/cumo/_internal/members/custom_control.py
--rw-r--r--   0        0        0     5927 2023-09-13 10:26:38.801824 cumo-0.33.4/cumo/_internal/members/event_handler.py
--rw-r--r--   0        0        0      974 2022-05-27 04:27:01.699189 cumo-0.33.4/cumo/_internal/members/internal_utils.py
--rw-r--r--   0        0        0     6396 2023-09-11 09:15:41.832883 cumo-0.33.4/cumo/_internal/members/keyboard_event_handler.py
--rw-r--r--   0        0        0     1360 2022-05-27 04:27:01.699189 cumo-0.33.4/cumo/_internal/members/remove_object.py
--rw-r--r--   0        0        0    20526 2023-07-27 11:30:24.682816 cumo-0.33.4/cumo/_internal/members/send_object.py
--rw-r--r--   0        0        0    10336 2023-09-13 10:26:38.801824 cumo-0.33.4/cumo/_internal/members/set_custom_control.py
--rw-r--r--   0        0        0     1045 2022-12-22 06:09:32.016687 cumo-0.33.4/cumo/_internal/members/set_enable.py
--rw-r--r--   0        0        0     1256 2023-09-13 10:26:38.801824 cumo-0.33.4/cumo/_internal/members/utils.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:41.386831 cumo-0.33.4/cumo/_internal/protobuf/__init__.py
--rw-r--r--   0        0        0     3923 2024-04-17 11:53:41.386831 cumo-0.33.4/cumo/_internal/protobuf/client_pb2.py
--rw-r--r--   0        0        0    10387 2024-04-17 11:53:41.386831 cumo-0.33.4/cumo/_internal/protobuf/client_pb2.pyi
--rw-r--r--   0        0        0    12303 2024-04-17 11:53:40.646801 cumo-0.33.4/cumo/_internal/protobuf/server_pb2.py
--rw-r--r--   0        0        0    40121 2024-04-17 11:53:40.646801 cumo-0.33.4/cumo/_internal/protobuf/server_pb2.pyi
--rw-r--r--   0        0        0     4200 2024-03-21 11:15:04.876331 cumo-0.33.4/cumo/_internal/server.py
--rw-r--r--   0        0        0     1509 2022-05-27 04:27:01.699189 cumo-0.33.4/cumo/_vendor/pypcd/LICENSE
--rw-r--r--   0        0        0    28920 2022-05-27 04:27:01.699189 cumo-0.33.4/cumo/_vendor/pypcd/pypcd.py
--rw-r--r--   0        0        0     1119 2023-09-13 10:26:38.801824 cumo-0.33.4/cumo/camera_state.py
--rw-r--r--   0        0        0      924 2022-05-27 04:27:01.699189 cumo-0.33.4/cumo/keyboard_event.py
--rw-r--r--   0        0        0     3554 2023-09-13 10:26:38.801824 cumo-0.33.4/cumo/pointcloudviewer.py
--rw-r--r--   0        0        0  5077319 2024-04-17 11:54:20.796681 cumo-0.33.4/cumo/public/bundle-a501c275.js
--rw-r--r--   0        0        0   243028 2024-04-17 11:54:20.796681 cumo-0.33.4/cumo/public/bundle.js.LICENSE.txt
--rw-r--r--   0        0        0      515 2024-04-17 11:54:20.786681 cumo-0.33.4/cumo/public/index-31f52342.css
--rw-r--r--   0        0        0      281 2024-04-17 11:54:20.796681 cumo-0.33.4/cumo/public/index.html
--rw-r--r--   0        0        0     1219 2024-04-17 11:51:59.710239 cumo-0.33.4/pyproject.toml
--rw-r--r--   0        0        0     2602 1970-01-01 00:00:00.000000 cumo-0.33.4/PKG-INFO
+-rw-r--r--   0        0        0     1275 2024-04-30 05:10:40.871452 cumo-0.34.0/README.md
+-rw-r--r--   0        0        0        7 2024-04-18 06:06:53.389837 cumo-0.34.0/cumo/.gitignore
+-rw-r--r--   0        0        0      117 2024-04-18 06:06:53.389837 cumo-0.34.0/cumo/__init__.py
+-rw-r--r--   0        0        0     3683 2024-04-18 06:06:53.389837 cumo-0.34.0/cumo/__main__.py
+-rw-r--r--   0        0        0        9 2024-04-18 06:06:53.389837 cumo-0.34.0/cumo/_internal/.gitignore
+-rw-r--r--   0        0        0        0 2024-04-18 06:06:53.389837 cumo-0.34.0/cumo/_internal/__init__.py
+-rw-r--r--   0        0        0     1675 2024-04-18 06:06:53.389837 cumo-0.34.0/cumo/_internal/down_sample.py
+-rw-r--r--   0        0        0        0 2024-04-18 06:06:53.389837 cumo-0.34.0/cumo/_internal/members/__init__.py
+-rw-r--r--   0        0        0     8722 2024-04-18 06:06:53.389837 cumo-0.34.0/cumo/_internal/members/camera.py
+-rw-r--r--   0        0        0     1177 2024-04-18 06:06:53.389837 cumo-0.34.0/cumo/_internal/members/capture_screen.py
+-rw-r--r--   0        0        0    12413 2024-04-18 06:06:53.389837 cumo-0.34.0/cumo/_internal/members/custom_control.py
+-rw-r--r--   0        0        0     5927 2024-04-18 06:06:53.389837 cumo-0.34.0/cumo/_internal/members/event_handler.py
+-rw-r--r--   0        0        0      974 2024-04-18 06:06:53.389837 cumo-0.34.0/cumo/_internal/members/internal_utils.py
+-rw-r--r--   0        0        0     6396 2024-04-18 06:06:53.389837 cumo-0.34.0/cumo/_internal/members/keyboard_event_handler.py
+-rw-r--r--   0        0        0     1360 2024-04-18 06:06:53.389837 cumo-0.34.0/cumo/_internal/members/remove_object.py
+-rw-r--r--   0        0        0    20526 2024-04-18 06:06:53.389837 cumo-0.34.0/cumo/_internal/members/send_object.py
+-rw-r--r--   0        0        0    10336 2024-04-18 06:06:53.389837 cumo-0.34.0/cumo/_internal/members/set_custom_control.py
+-rw-r--r--   0        0        0     1045 2024-04-18 06:06:53.389837 cumo-0.34.0/cumo/_internal/members/set_enable.py
+-rw-r--r--   0        0        0     1256 2024-04-18 06:06:53.389837 cumo-0.34.0/cumo/_internal/members/utils.py
+-rw-r--r--   0        0        0        0 2024-04-30 05:10:32.699489 cumo-0.34.0/cumo/_internal/protobuf/__init__.py
+-rw-r--r--   0        0        0     3923 2024-04-30 05:10:32.695490 cumo-0.34.0/cumo/_internal/protobuf/client_pb2.py
+-rw-r--r--   0        0        0    10387 2024-04-30 05:10:32.695490 cumo-0.34.0/cumo/_internal/protobuf/client_pb2.pyi
+-rw-r--r--   0        0        0    12303 2024-04-30 05:10:32.511490 cumo-0.34.0/cumo/_internal/protobuf/server_pb2.py
+-rw-r--r--   0        0        0    40121 2024-04-30 05:10:32.511490 cumo-0.34.0/cumo/_internal/protobuf/server_pb2.pyi
+-rw-r--r--   0        0        0     4200 2024-04-18 06:06:53.393837 cumo-0.34.0/cumo/_internal/server.py
+-rw-r--r--   0        0        0     1509 2024-04-18 06:06:53.393837 cumo-0.34.0/cumo/_vendor/pypcd/LICENSE
+-rw-r--r--   0        0        0    28920 2024-04-18 06:06:53.393837 cumo-0.34.0/cumo/_vendor/pypcd/pypcd.py
+-rw-r--r--   0        0        0     1119 2024-04-18 06:06:53.393837 cumo-0.34.0/cumo/camera_state.py
+-rw-r--r--   0        0        0      924 2024-04-18 06:06:53.393837 cumo-0.34.0/cumo/keyboard_event.py
+-rw-r--r--   0        0        0     3554 2024-04-18 06:06:53.393837 cumo-0.34.0/cumo/pointcloudviewer.py
+-rw-r--r--   0        0        0  5077405 2024-04-30 05:10:40.867452 cumo-0.34.0/cumo/public/bundle-e4641802.js
+-rw-r--r--   0        0        0   243028 2024-04-30 05:10:40.867452 cumo-0.34.0/cumo/public/bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0      515 2024-04-30 05:10:40.867452 cumo-0.34.0/cumo/public/index-31f52342.css
+-rw-r--r--   0        0        0      281 2024-04-30 05:10:40.867452 cumo-0.34.0/cumo/public/index.html
+-rw-r--r--   0        0        0     1219 2024-04-30 05:09:06.284783 cumo-0.34.0/pyproject.toml
+-rw-r--r--   0        0        0     2602 1970-01-01 00:00:00.000000 cumo-0.34.0/PKG-INFO
```

### Comparing `cumo-0.33.4/README.md` & `cumo-0.34.0/README.md`

 * *Files identical despite different names*

### Comparing `cumo-0.33.4/cumo/__main__.py` & `cumo-0.34.0/cumo/__main__.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.4/cumo/_internal/down_sample.py` & `cumo-0.34.0/cumo/_internal/down_sample.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.4/cumo/_internal/members/camera.py` & `cumo-0.34.0/cumo/_internal/members/camera.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.4/cumo/_internal/members/capture_screen.py` & `cumo-0.34.0/cumo/_internal/members/capture_screen.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.4/cumo/_internal/members/custom_control.py` & `cumo-0.34.0/cumo/_internal/members/custom_control.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.4/cumo/_internal/members/event_handler.py` & `cumo-0.34.0/cumo/_internal/members/event_handler.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.4/cumo/_internal/members/internal_utils.py` & `cumo-0.34.0/cumo/_internal/members/internal_utils.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.4/cumo/_internal/members/keyboard_event_handler.py` & `cumo-0.34.0/cumo/_internal/members/keyboard_event_handler.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.4/cumo/_internal/members/remove_object.py` & `cumo-0.34.0/cumo/_internal/members/remove_object.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.4/cumo/_internal/members/send_object.py` & `cumo-0.34.0/cumo/_internal/members/send_object.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.4/cumo/_internal/members/set_custom_control.py` & `cumo-0.34.0/cumo/_internal/members/set_custom_control.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.4/cumo/_internal/members/set_enable.py` & `cumo-0.34.0/cumo/_internal/members/set_enable.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.4/cumo/_internal/members/utils.py` & `cumo-0.34.0/cumo/_internal/members/utils.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.4/cumo/_internal/protobuf/client_pb2.py` & `cumo-0.34.0/cumo/_internal/protobuf/client_pb2.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.4/cumo/_internal/protobuf/client_pb2.pyi` & `cumo-0.34.0/cumo/_internal/protobuf/client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cumo-0.33.4/cumo/_internal/protobuf/server_pb2.py` & `cumo-0.34.0/cumo/_internal/protobuf/server_pb2.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.4/cumo/_internal/protobuf/server_pb2.pyi` & `cumo-0.34.0/cumo/_internal/protobuf/server_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cumo-0.33.4/cumo/_internal/server.py` & `cumo-0.34.0/cumo/_internal/server.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.4/cumo/_vendor/pypcd/LICENSE` & `cumo-0.34.0/cumo/_vendor/pypcd/LICENSE`

 * *Files identical despite different names*

### Comparing `cumo-0.33.4/cumo/_vendor/pypcd/pypcd.py` & `cumo-0.34.0/cumo/_vendor/pypcd/pypcd.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.4/cumo/camera_state.py` & `cumo-0.34.0/cumo/camera_state.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.4/cumo/keyboard_event.py` & `cumo-0.34.0/cumo/keyboard_event.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.4/cumo/pointcloudviewer.py` & `cumo-0.34.0/cumo/pointcloudviewer.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.4/cumo/public/bundle-a501c275.js` & `cumo-0.34.0/cumo/public/bundle-e4641802.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -123682,16 +123682,20 @@
         this.zoomStart.copyFrom(this.zoomEnd)
     }
     panCamera() {
         if (this.camera === null) return;
         const t = this.panEnd.subtract(this.panStart);
         if (t.lengthSquared()) {
             t.scaleInPlace(this.eye.length() * this.panSpeed);
-            const r = this.eye.cross(this.camera.upVector).normalize().scaleInPlace(-t.x);
-            r.addInPlace(this.camera.upVector.scale(t.y)), this.target.addInPlace(r), this.panStart.copyFrom(this.panEnd)
+            const r = this.eye.clone(),
+                s = this.camera.upVector.clone(),
+                n = r.scale(Vector3.Dot(r, s) / r.lengthSquared()),
+                o = s.subtract(n).normalize(),
+                c = this.eye.cross(o).normalize().scaleInPlace(-t.x);
+            c.addInPlace(o.scale(t.y)), this.target.addInPlace(c), this.panStart.copyFrom(this.panEnd)
         }
     }
     rollCamera() {
         if (this.camera === null) return;
         const t = Math.atan2(this.rollStart.y, this.rollStart.x),
             r = Math.atan2(this.rollEnd.y, this.rollEnd.x),
             s = t - r;
```

### Comparing `cumo-0.33.4/cumo/public/bundle.js.LICENSE.txt` & `cumo-0.34.0/cumo/public/bundle.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cumo-0.33.4/cumo/public/index-31f52342.css` & `cumo-0.34.0/cumo/public/index-31f52342.css`

 * *Files identical despite different names*

### Comparing `cumo-0.33.4/pyproject.toml` & `cumo-0.34.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 readme = "README.md"
 name = "cumo"
-version = "0.33.4"
+version = "0.34.0"
 description = "Webブラウザ上に点群を描画する python ライブラリ"
 authors = ["Kurusugawa Computer"]
 license = "BSD"
 keywords = ["point-cloud", "pcd"]
 repository = "https://github.com/kurusugawa-computer/cumo"
 classifiers = [
 	"Development Status :: 3 - Alpha",
```

### Comparing `cumo-0.33.4/PKG-INFO` & `cumo-0.34.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cumo
-Version: 0.33.4
+Version: 0.34.0
 Summary: Webブラウザ上に点群を描画する python ライブラリ
 Home-page: https://github.com/kurusugawa-computer/cumo
 License: BSD
 Keywords: point-cloud,pcd
 Author: Kurusugawa Computer
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
```

