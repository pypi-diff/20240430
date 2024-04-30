# Comparing `tmp/myf_face_recognition-0.6.tar.gz` & `tmp/myf_face_recognition-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myf_face_recognition-0.6.tar", last modified: Mon Mar 25 09:29:26 2024, max compression
+gzip compressed data, was "myf_face_recognition-0.7.tar", last modified: Tue Apr 30 17:15:31 2024, max compression
```

## Comparing `myf_face_recognition-0.6.tar` & `myf_face_recognition-0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-25 09:29:25.326840 myf_face_recognition-0.6/
--rw-rw-rw-   0        0        0     1096 2024-03-24 20:45:15.000000 myf_face_recognition-0.6/LICENCE
--rw-rw-rw-   0        0        0      488 2024-03-25 09:29:25.319834 myf_face_recognition-0.6/PKG-INFO
--rw-rw-rw-   0        0        0     8351 2024-03-24 20:39:50.000000 myf_face_recognition-0.6/README.txt
-drwxrwxrwx   0        0        0        0 2024-03-25 09:29:24.906929 myf_face_recognition-0.6/myf_face_recognition/
--rw-rw-rw-   0        0        0        0 2024-03-25 05:22:33.000000 myf_face_recognition-0.6/myf_face_recognition/__init__.py
--rw-rw-rw-   0        0        0    11313 2024-03-25 09:28:30.000000 myf_face_recognition-0.6/myf_face_recognition/all.py
--rw-rw-rw-   0        0        0     3222 2024-03-25 09:28:35.000000 myf_face_recognition-0.6/myf_face_recognition/embeddings.py
--rw-rw-rw-   0        0        0     4107 2024-03-25 09:28:36.000000 myf_face_recognition-0.6/myf_face_recognition/images.py
--rw-rw-rw-   0        0        0     3841 2024-03-25 09:28:38.000000 myf_face_recognition-0.6/myf_face_recognition/simple_video.py
--rw-rw-rw-   0        0        0     4047 2024-03-25 09:28:42.000000 myf_face_recognition-0.6/myf_face_recognition/video.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:29:25.265830 myf_face_recognition-0.6/myf_face_recognition.egg-info/
--rw-rw-rw-   0        0        0      488 2024-03-25 09:29:21.000000 myf_face_recognition-0.6/myf_face_recognition.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      487 2024-03-25 09:29:22.000000 myf_face_recognition-0.6/myf_face_recognition.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-25 09:29:21.000000 myf_face_recognition-0.6/myf_face_recognition.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2024-03-25 09:29:21.000000 myf_face_recognition-0.6/myf_face_recognition.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       52 2024-03-25 09:29:21.000000 myf_face_recognition-0.6/myf_face_recognition.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-03-25 09:29:21.000000 myf_face_recognition-0.6/myf_face_recognition.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-25 09:29:25.331834 myf_face_recognition-0.6/setup.cfg
--rw-rw-rw-   0        0        0      728 2024-03-25 09:29:03.000000 myf_face_recognition-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 17:15:31.494316 myf_face_recognition-0.7/
+-rw-rw-rw-   0        0        0     1096 2024-03-24 20:45:15.000000 myf_face_recognition-0.7/LICENCE
+-rw-rw-rw-   0        0        0      488 2024-04-30 17:15:31.490315 myf_face_recognition-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     8669 2024-04-30 17:11:50.000000 myf_face_recognition-0.7/README.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 17:15:31.329913 myf_face_recognition-0.7/myf_face_recognition/
+-rw-rw-rw-   0        0        0        0 2024-03-25 05:22:33.000000 myf_face_recognition-0.7/myf_face_recognition/__init__.py
+-rw-rw-rw-   0        0        0    11503 2024-04-30 16:59:01.000000 myf_face_recognition-0.7/myf_face_recognition/all.py
+-rw-rw-rw-   0        0        0     3222 2024-03-25 09:28:35.000000 myf_face_recognition-0.7/myf_face_recognition/embeddings.py
+-rw-rw-rw-   0        0        0     4107 2024-03-25 09:28:36.000000 myf_face_recognition-0.7/myf_face_recognition/images.py
+-rw-rw-rw-   0        0        0     3841 2024-03-25 09:28:38.000000 myf_face_recognition-0.7/myf_face_recognition/simple_video.py
+-rw-rw-rw-   0        0        0     4392 2024-04-30 16:58:32.000000 myf_face_recognition-0.7/myf_face_recognition/video.py
+drwxrwxrwx   0        0        0        0 2024-04-30 17:15:31.485319 myf_face_recognition-0.7/myf_face_recognition.egg-info/
+-rw-rw-rw-   0        0        0      488 2024-04-30 17:15:25.000000 myf_face_recognition-0.7/myf_face_recognition.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      487 2024-04-30 17:15:26.000000 myf_face_recognition-0.7/myf_face_recognition.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 17:15:25.000000 myf_face_recognition-0.7/myf_face_recognition.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2024-04-30 17:15:25.000000 myf_face_recognition-0.7/myf_face_recognition.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       52 2024-04-30 17:15:25.000000 myf_face_recognition-0.7/myf_face_recognition.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-04-30 17:15:25.000000 myf_face_recognition-0.7/myf_face_recognition.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 17:15:31.495316 myf_face_recognition-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      728 2024-04-30 17:14:59.000000 myf_face_recognition-0.7/setup.py
```

### Comparing `myf_face_recognition-0.6/LICENCE` & `myf_face_recognition-0.7/LICENCE`

 * *Files identical despite different names*

### Comparing `myf_face_recognition-0.6/README.txt` & `myf_face_recognition-0.7/README.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,21 +22,23 @@
 -root
     -embeddings
         Tony_Stark_embeddings.npy
         .
         .
         .
     -myf_face_recognition
+        models
+            yolov8n-face.pt (Pre-trained YOLO face Detection Model)
         all.py
         embeddings.py
         images.py
         simple_video.py
         video.py
-        yolov8n-face.pt (YOLO Fface Detection Model)
-    readme.txt
+
+    README.txt
     test_script.py (Create your python scripts here to use this library)
 
 Don't change the myf_face_recognition folder Structure,
 and create your scripts in the root directory directly and not in some folders.
 
 
 
@@ -49,15 +51,15 @@
 Identify Faces in Videos
 
 
 
 1. Generate Face Embeddings
 
 What are Face Embeddings?
-Face embeddings are vector representations of facial features extracted from images. These vectors encode unique characteristics of faces in a high-dimensional space, enabling efficient comparison and recognition of faces.
+Face embeddings are vector representations of facial features extracted from images. These vectors encode unique characteristics of faces in a high-dimensional space, enabling efficient comparison and recognition of faces. In simple words, face embeddings are mathematical representation of a face, it is unique for each faces.
 
 Usage-
 
 generate_face_embeddings(name, folder_path, output_folder_path, show_training=False)
 
 Args-
 name: Name of the person.
@@ -128,20 +130,21 @@
 
 3. Identify Faces in Videos
 
 This is very similar to that of the face recognition in image, essentially this is the same thing but in a loop, we pass each frame of the video to the function and it gives us the results.
 
 Usage-
 
-identify_faces_in_video(test_image, embedding_files, threshold=0.65, show_frame=True)
+identify_faces_in_video(test_image, embedding_files, threshold=0.65, model_path=default_model_path, show_frame=True)
 
 Args-
 test_image: Pass each frame of the video in which you want to search the person, this can be done using cv2 library using a loop or some other libraries.
 embedding_files: This is a list of person's embeddings for whome you want to search in the image.
 threshold: This is the trigger knob, adjust this to fine tune the results (default: 0.65).
+model_path: If you have a different pre-trained face detection model, pass its path here, the default model is yolov8n-face.pt.
 show_frame: Whether to show the frames and highlight his/her location (default: True).
 
 Return-
 recognized_faces: This function returns a dictionary containing the name of the persons as the keys and the accuracy as their values.
 
 Here is a dummy script for face recognition in a video.
 {
@@ -168,14 +171,15 @@
         results = identify_faces_in_video(frame, embedding_files)
         print(results)
 
         if cv2.waitKey(1) & 0xFF == ord('q'):
             print("Exiting...")
             break
 
+    cap.release() 
     cv2.destroyAllWindows()
 
 }
 
 
 
 This function uses YOLO for face detection and then FaceNet for face recognition, due to YOLO it becomes a little slower, so instead another option can be considered but the accuracy drops significantly.
```

### Comparing `myf_face_recognition-0.6/myf_face_recognition/all.py` & `myf_face_recognition-0.7/myf_face_recognition/all.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 import numpy as np
 from keras_facenet import FaceNet
 import cv2
 import os
 from mtcnn import MTCNN
+from ultralytics import YOLO
+
 
 # Initialize FaceNet model
 print("Loading FaceNet Model...")
 facenet_model = FaceNet()
 print("FaceNet model loaded successfully.")
 
 # Initialize MTCNN detector
 detector = None
 
 face_cascade = cv2.CascadeClassifier(cv2.data.haarcascades + 'haarcascade_frontalface_default.xml')
 
-def load_mtcnn_model():
-    """
-    Load MTCNN model if not loaded already.
-    """
-    global detector
-    if detector is None:
-        print("Loading MTCNN model...")
-        detector = MTCNN()
-        print("MTCNN model loaded successfully.")
+default_model_path = os.path.join(os.path.dirname(__file__), "models", "yolov8n-face.pt")
+
+# Initialize Yolo model
+yolo_model = None
+
+def load_yolo_model(model_path):
+    print("Loading YOLO Model...")
+    yolo_model = YOLO(model_path)
+    print("YOLO model loaded successfully.")
+    return yolo_model
 
 def face_recognition(cropped_image, embedding_files, threshold=0.65):
     """
     Recognize faces in the cropped image and return the recognized person along with the similarity score.
 
     Args:
         cropped_image (numpy.ndarray): Cropped face region from the input image.
@@ -173,32 +176,36 @@
             print("Press any key to continue.")
             cv2.waitKey(0)
     else:
         print("No faces found")
 
     return recognized_faces
 
-def identify_faces_in_video(test_image, embedding_files, yolo_model, threshold=0.65, show_frame=True):
+def identify_faces_in_video(test_image, embedding_files, threshold=0.65, model_path=default_model_path, show_frame=True):
     """
     Identify faces in a video stream using YOLO model and recognize them using FaceNet.
 
     Args:
         test_image (numpy.ndarray): Input video frame.
         embedding_files (list): List of paths to the embedding files.
         threshold (float, optional): Threshold value for similarity score. Default is 0.65.
         show_frame (bool, optional): Flag to display the processed frame with recognized faces. Default is True.
 
     Returns:
         dict: Dictionary containing recognized faces and their similarity scores.
     """
-    global facenet_model
+
+    global yolo_model
 
     test_image = cv2.cvtColor(test_image, cv2.COLOR_BGR2RGB)
     image_np_original = np.array(test_image)
 
+    if yolo_model is None:
+        yolo_model = load_yolo_model(model_path)
+
     results = yolo_model.predict(test_image, show=False, stream=False)
     recognized_faces = {}  # Dictionary to store recognized faces and their similarity scores
 
     if results:
         for r in results:
             for box, score, class_id in zip(r.boxes.xyxy, r.boxes.conf, r.boxes.cls):
                 xmin, ymin, xmax, ymax = map(int, box.tolist())
@@ -224,14 +231,15 @@
         if show_frame:
             cv2.imshow("Frame", image_np_original)
     else:
         print("No faces found")
 
     return recognized_faces
 
+
 def simple_identify_faces_in_video(test_image, embedding_files, threshold=0.65, show_frame=True):
     """
     Identify faces in the input image using a simple method and return recognized faces along with their similarity scores.
 
     Args:
         test_image (numpy.ndarray): Input image.
         embedding_files (list): List of paths to the embedding files.
```

### Comparing `myf_face_recognition-0.6/myf_face_recognition/embeddings.py` & `myf_face_recognition-0.7/myf_face_recognition/embeddings.py`

 * *Files identical despite different names*

### Comparing `myf_face_recognition-0.6/myf_face_recognition/images.py` & `myf_face_recognition-0.7/myf_face_recognition/images.py`

 * *Files identical despite different names*

### Comparing `myf_face_recognition-0.6/myf_face_recognition/simple_video.py` & `myf_face_recognition-0.7/myf_face_recognition/simple_video.py`

 * *Files identical despite different names*

### Comparing `myf_face_recognition-0.6/myf_face_recognition/video.py` & `myf_face_recognition-0.7/myf_face_recognition/video.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 import numpy as np
 from keras_facenet import FaceNet
 import cv2
 import os
+from ultralytics import YOLO
+
+default_model_path = os.path.join(os.path.dirname(__file__), "models", "yolov8n-face.pt")
+
+# Initialize Yolo model
+yolo_model = None
+
+def load_yolo_model(model_path):
+    print("Loading YOLO Model...")
+    yolo_model = YOLO(model_path)
+    print("YOLO model loaded successfully.")
+    return yolo_model
 
 # Initialize FaceNet model
 print("Loading FaceNet model...")
 facenet_model = FaceNet()
 print("FaceNet model loaded successfully.")
 
-
 def face_recognition(cropped_image, embedding_files, threshold=0.65):
     """
     Recognize faces in the cropped image and return the recognized person along with the similarity score.
 
+
     Args:
         cropped_image (numpy.ndarray): Cropped face region from the input image.
         embedding_files (list): List of paths to the embedding files.
         threshold (float, optional): Threshold value for similarity score. Default is 0.65.
 
     Returns:
         tuple: Recognized person name and the maximum similarity score.
@@ -37,32 +49,36 @@
         name_without_suffix = base_name.replace("_embeddings.npy", "")
         recognized_person = name_without_suffix.replace("_", " ").title()
     else:
         recognized_person = "Unknown"
 
     return recognized_person, max_score
 
-def identify_faces_in_video(test_image, embedding_files, yolo_model, threshold=0.65, show_frame=True):
+def identify_faces_in_video(test_image, embedding_files, threshold=0.65, model_path=default_model_path, show_frame=True):
     """
-    Identify faces in the input image using YOLO model and return recognized faces along with their similarity scores.
+    Identify faces in a video stream using YOLO model and recognize them using FaceNet.
 
     Args:
-        test_image (numpy.ndarray): Input image.
+        test_image (numpy.ndarray): Input video frame.
         embedding_files (list): List of paths to the embedding files.
         threshold (float, optional): Threshold value for similarity score. Default is 0.65.
-        show_frame (bool, optional): Flag to display the processed image with recognized faces. Default is True.
+        show_frame (bool, optional): Flag to display the processed frame with recognized faces. Default is True.
 
     Returns:
         dict: Dictionary containing recognized faces and their similarity scores.
     """
-    global facenet_model
+
+    global yolo_model
 
     test_image = cv2.cvtColor(test_image, cv2.COLOR_BGR2RGB)
     image_np_original = np.array(test_image)
 
+    if yolo_model is None:
+        yolo_model = load_yolo_model(model_path)
+
     results = yolo_model.predict(test_image, show=False, stream=False)
     recognized_faces = {}  # Dictionary to store recognized faces and their similarity scores
 
     if results:
         for r in results:
             for box, score, class_id in zip(r.boxes.xyxy, r.boxes.conf, r.boxes.cls):
                 xmin, ymin, xmax, ymax = map(int, box.tolist())
@@ -78,16 +94,16 @@
                 if recognized_person == "Unknown":
                     continue
                 else:
                     recognized_faces[recognized_person] = max_score  # Add to recognized_faces dictionary
 
                 if show_frame:
                     cv2.putText(image_np_original, f"{recognized_person} ({max_score:.2f})", (xmin, ymin - 10),
-                            cv2.FONT_HERSHEY_SIMPLEX, 1, (0, 255, 0), 3)
+                                cv2.FONT_HERSHEY_SIMPLEX, 1, (0, 255, 0), 3)
 
         image_np_original = cv2.cvtColor(image_np_original, cv2.COLOR_BGR2RGB)
         if show_frame:
             cv2.imshow("Frame", image_np_original)
     else:
         print("No faces found")
 
-    return recognized_faces  # Return dictionary containing recognized faces and their similarity scores
+    return recognized_faces
```

### Comparing `myf_face_recognition-0.6/setup.py` & `myf_face_recognition-0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myf_face_recognition',
-    version='0.6',
+    version='0.7',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'keras-facenet',
         'opencv-python',
         'mtcnn',
         'ultralytics'
```

