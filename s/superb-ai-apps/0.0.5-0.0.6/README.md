# Comparing `tmp/superb-ai-apps-0.0.5.tar.gz` & `tmp/superb-ai-apps-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superb-ai-apps-0.0.5.tar", last modified: Wed Apr 24 05:27:41 2024, max compression
+gzip compressed data, was "superb-ai-apps-0.0.6.tar", last modified: Tue Apr 30 08:01:43 2024, max compression
```

## Comparing `superb-ai-apps-0.0.5.tar` & `superb-ai-apps-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:27:41.199214 superb-ai-apps-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-24 05:27:41.199214 superb-ai-apps-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 05:27:26.000000 superb-ai-apps-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 05:27:41.199214 superb-ai-apps-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-24 05:27:26.000000 superb-ai-apps-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:27:41.199214 superb-ai-apps-0.0.5/spb_apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 05:27:26.000000 superb-ai-apps-0.0.5/spb_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-04-24 05:27:26.000000 superb-ai-apps-0.0.5/spb_apps/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:27:41.199214 superb-ai-apps-0.0.5/spb_apps/curate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 05:27:26.000000 superb-ai-apps-0.0.5/spb_apps/curate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 05:27:26.000000 superb-ai-apps-0.0.5/spb_apps/curate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:27:41.199214 superb-ai-apps-0.0.5/spb_apps/label/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 05:27:26.000000 superb-ai-apps-0.0.5/spb_apps/label/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13369 2024-04-24 05:27:26.000000 superb-ai-apps-0.0.5/spb_apps/superb_curate.py
--rw-r--r--   0 runner    (1001) docker     (127)    14887 2024-04-24 05:27:26.000000 superb-ai-apps-0.0.5/spb_apps/superb_label.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:27:41.199214 superb-ai-apps-0.0.5/spb_apps/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 05:27:26.000000 superb-ai-apps-0.0.5/spb_apps/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-24 05:27:26.000000 superb-ai-apps-0.0.5/spb_apps/utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-04-24 05:27:26.000000 superb-ai-apps-0.0.5/spb_apps/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:27:41.199214 superb-ai-apps-0.0.5/superb_ai_apps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-24 05:27:41.000000 superb-ai-apps-0.0.5/superb_ai_apps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-24 05:27:41.000000 superb-ai-apps-0.0.5/superb_ai_apps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 05:27:41.000000 superb-ai-apps-0.0.5/superb_ai_apps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-24 05:27:41.000000 superb-ai-apps-0.0.5/superb_ai_apps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 05:27:41.000000 superb-ai-apps-0.0.5/superb_ai_apps.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:01:43.627031 superb-ai-apps-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-30 08:01:43.627031 superb-ai-apps-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 08:01:25.000000 superb-ai-apps-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 08:01:43.627031 superb-ai-apps-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-30 08:01:25.000000 superb-ai-apps-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:01:43.623031 superb-ai-apps-0.0.6/spb_apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 08:01:25.000000 superb-ai-apps-0.0.6/spb_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-30 08:01:25.000000 superb-ai-apps-0.0.6/spb_apps/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:01:43.623031 superb-ai-apps-0.0.6/spb_apps/curate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 08:01:25.000000 superb-ai-apps-0.0.6/spb_apps/curate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 08:01:25.000000 superb-ai-apps-0.0.6/spb_apps/curate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:01:43.623031 superb-ai-apps-0.0.6/spb_apps/label/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 08:01:25.000000 superb-ai-apps-0.0.6/spb_apps/label/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11965 2024-04-30 08:01:25.000000 superb-ai-apps-0.0.6/spb_apps/superb_curate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13570 2024-04-30 08:01:25.000000 superb-ai-apps-0.0.6/spb_apps/superb_label.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:01:43.623031 superb-ai-apps-0.0.6/spb_apps/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 08:01:25.000000 superb-ai-apps-0.0.6/spb_apps/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-30 08:01:25.000000 superb-ai-apps-0.0.6/spb_apps/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-04-30 08:01:25.000000 superb-ai-apps-0.0.6/spb_apps/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:01:43.623031 superb-ai-apps-0.0.6/superb_ai_apps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-30 08:01:43.000000 superb-ai-apps-0.0.6/superb_ai_apps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-30 08:01:43.000000 superb-ai-apps-0.0.6/superb_ai_apps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 08:01:43.000000 superb-ai-apps-0.0.6/superb_ai_apps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-30 08:01:43.000000 superb-ai-apps-0.0.6/superb_ai_apps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 08:01:43.000000 superb-ai-apps-0.0.6/superb_ai_apps.egg-info/top_level.txt
```

### Comparing `superb-ai-apps-0.0.5/setup.py` & `superb-ai-apps-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="superb-ai-apps",
-    version="0.0.5",
+    version="0.0.6",
     description="Python Package for Superb-AI Apps",
     install_requires=[
         "asttokens==2.4.1",
         "attrs==23.2.0",
         "backcall==0.2.0",
         "beautifulsoup4==4.12.3",
         "bleach==6.1.0",
```

### Comparing `superb-ai-apps-0.0.5/spb_apps/apps.py` & `superb-ai-apps-0.0.6/spb_apps/apps.py`

 * *Files 12% similar despite different names*

```diff
@@ -76,22 +76,7 @@
             images_path (str): The path to the images to be uploaded.
             dataset_name (str, optional): The name of the dataset to upload the images to. Required for the 'label' platform.
 
         Returns:
             The result of the image upload operation, which varies by platform.
         """
         pass
-
-    @abstractmethod
-    def convert_yolo_bbox_to_platform(self):
-        """
-        Abstract method to convert YOLO format bounding box annotations to the platform-specific format.
-
-        Parameters:
-            data_key (str): The unique identifier for the image or dataset.
-            annotations (list): A list of YOLO format annotations to be converted.
-            classes (list, optional): The classes associated with the YOLO annotations. Required if format is 'yolo'.
-
-        Returns:
-            list: A list of platform-specific bounding box annotations converted from the YOLO format.
-        """
-        pass
```

### Comparing `superb-ai-apps-0.0.5/spb_apps/superb_curate.py` & `superb-ai-apps-0.0.6/spb_apps/superb_curate.py`

 * *Files 12% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         spb_curate.access_key = self.access_key
         if is_dev:
             spb_curate.api_base = "https://api.dev.superb-ai.com"
 
         if dataset_name:
             try:
                 self.dataset = spb_curate.fetch_dataset(name=dataset_name)
-            except ConflictError:
+            except:
                 print(
                     f"Dataset does not exist, Creating Dataset {dataset_name}"
                 )
                 self.dataset = spb_curate.create_dataset(
                     name=dataset_name, description="Demo dataset."
                 )
 
@@ -309,51 +309,14 @@
         """
         slice = self.dataset.fetch_images(
             slice=slice_name, include_image_url=True
         )
         for image in slice:
             self.download_image(data_key=image["key"], path=download_path)
 
-    def convert_yolo_bbox_to_platform(
-        self, data_key: str, annotations: list, classes: list = ""
-    ) -> list:
-        """
-        Converts YOLO format annotations to the platform's bounding box format and creates bounding box annotations.
-
-        Args:
-            data_key (str): The unique identifier for the image or dataset.
-            annotations (list): A list of YOLO format annotations to be converted.
-            classes (list, optional): The classes associated with the YOLO annotations. Required if format is 'yolo'.
-
-        Returns:
-            list: A list of bounding box annotations created from the converted YOLO annotations.
-        """
-
-        if classes == "":
-            print("To convert yolo annotations, you must provide classes.")
-            return []
-        bbox_annotation = []
-        try:
-            width, height = self.get_width_height(data_key=data_key)
-        except:
-            return []
-        converted_annotations = convert_yolo_bbox(
-            data_key, annotations, classes, width, height
-        )
-        if converted_annotations is not None:
-            for anno in converted_annotations:
-                bbox = self.make_bbox_annotation(
-                    data_key,
-                    anno[0],
-                    anno[1],
-                )
-                bbox_annotation.append(bbox)
-
-        return bbox_annotation
-
     def download_image_by_slice(self, slice_name: str, download_path: str):
         """
         Downloads an image by its slice name to a specified path. This method is exclusive to the Curate platform.
 
         Args:
             slice_name (str): The name of the slice from which to download the image.
             download_path (str): The local file path where the downloaded image will be saved.
```

### Comparing `superb-ai-apps-0.0.5/spb_apps/superb_label.py` & `superb-ai-apps-0.0.6/spb_apps/superb_label.py`

 * *Files 4% similar despite different names*

```diff
@@ -194,15 +194,15 @@
 
         Parameters:
         - label (spb_label.DataHandle, optional): The label data handle containing the image to download. If None, the label is retrieved using the data_key.
         - data_key (str, optional): The unique identifier for the image. Used if label is None.
         - path (str): The local file path where the image will be saved. Defaults to "/".
         """
         if label is None:
-            label = self.client.get_label(data_key=data_key)
+            label = self.get_label(data_key=data_key)
         label.download_image(download_to=path)
 
     def get_width_height(
         self, label: spb_label.DataHandle = None, data_key: str = None
     ) -> Tuple[int, int]:
         """
         Download an image associated with a label, return its width and height, and delete the image.
@@ -211,15 +211,15 @@
         - label (spb_label.DataHandle, optional): The label data handle containing the image to download. If None, the label is retrieved using the data_key.
         - data_key (str, optional): The unique identifier for the image. Used if label is None.
 
         Returns:
         Tuple[int, int]: A tuple containing the width and height of the downloaded image.
         """
         if label is None:
-            label = self.client.get_label(data_key=data_key)
+            label = self.get_label(data_key=data_key)
         image_url = label.get_image_url()
         response = requests.get(image_url)
         img = Image.open(BytesIO(response.content))
         width, height = img.size
 
         return width, height
 
@@ -244,47 +244,14 @@
                     "height": annotation[3],
                 }
             },
         }
 
         return bbox
 
-    def convert_yolo_bbox_to_platform(
-        self,
-        data_key: str,
-        annotations: list,
-        classes: list,
-    ) -> Tuple[Optional[str], Optional[list]]:
-        """
-        Convert YOLO bounding box annotations to the format expected by the platform.
-
-        Returns:
-            Tuple[Optional[str], Optional[list]]: A tuple containing the data handler and the converted annotations if successful, otherwise None for each.
-        """
-        _, label = self.client.get_labels(data_key=data_key)
-        if len(label) == 0:
-            print(
-                f"[SKIPPED] Data key: {data_key}, does not exist in project {self.client.get_project_name()}"
-            )
-            return None, None
-        data_handler = label[0]
-        if classes == "":
-            print("To upload yolo annotations, you must provide classes.")
-            return None, None
-        width, height = self.get_width_height(data_handler=data_handler)
-        converted_annotations = convert_yolo_bbox(
-            data_key, annotations, classes, width, height
-        )
-        label_annotations = []
-        for anno in converted_annotations:
-            bbox = self.make_bbox_annotation(anno[0], anno[1])
-            label_annotations.append(bbox)
-
-        return data_handler, label_annotations
-
     def upload_images(self, image_paths: list, dataset_name: str):
         """
         Upload images to a specified dataset.
 
         Parameters:
         - image_paths (list): A list of paths to the images to be uploaded.
         - dataset_name (str): The name of the dataset to upload the images to.
```

### Comparing `superb-ai-apps-0.0.5/spb_apps/utils/converter.py` & `superb-ai-apps-0.0.6/spb_apps/utils/converter.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         class_number, x_norm, y_norm, w_norm, h_norm = (
             anno[0],
             anno[1],
             anno[2],
             anno[3],
             anno[4],
         )
-        class_name = classes[class_number]
+        class_name = classes[int(class_number)]
         # Check normalization
         if any(value > 1 for value in (x_norm, y_norm, w_norm, h_norm)):
             print(
                 f"[WARNING] [Invalid zip file] {data_key}.txt\n"
                 + f"[[Class index] [x_center] [y_center] [width] [height]]: [{int(class_number)} {x_norm} {y_norm} {w_norm} {h_norm}]\n"
                 + f" YOLO format coordinates, width, and height must be normalized (0 - 1)."
             )
```

### Comparing `superb-ai-apps-0.0.5/spb_apps/utils/utils.py` & `superb-ai-apps-0.0.6/spb_apps/utils/utils.py`

 * *Files identical despite different names*

### Comparing `superb-ai-apps-0.0.5/superb_ai_apps.egg-info/requires.txt` & `superb-ai-apps-0.0.6/superb_ai_apps.egg-info/requires.txt`

 * *Files identical despite different names*

