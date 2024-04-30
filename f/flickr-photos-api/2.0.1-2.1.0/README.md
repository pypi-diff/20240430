# Comparing `tmp/flickr_photos_api-2.0.1.tar.gz` & `tmp/flickr_photos_api-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flickr_photos_api-2.0.1.tar", last modified: Tue Apr 30 12:27:51 2024, max compression
+gzip compressed data, was "flickr_photos_api-2.1.0.tar", last modified: Tue Apr 30 14:50:59 2024, max compression
```

## Comparing `flickr_photos_api-2.0.1.tar` & `flickr_photos_api-2.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 12:27:51.247959 flickr_photos_api-2.0.1/
--rw-r--r--   0 alexwlchan   (501) staff       (20)    11356 2023-11-05 12:32:45.000000 flickr_photos_api-2.0.1/LICENSE-APACHE
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1074 2023-11-05 12:32:47.000000 flickr_photos_api-2.0.1/LICENSE-MIT
--rw-r--r--   0 alexwlchan   (501) staff       (20)     4070 2024-04-30 12:27:51.247782 flickr_photos_api-2.0.1/PKG-INFO
--rw-r--r--   0 alexwlchan   (501) staff       (20)     3172 2024-04-30 12:06:13.000000 flickr_photos_api-2.0.1/README.md
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1856 2024-04-30 12:06:13.000000 flickr_photos_api-2.0.1/pyproject.toml
--rw-r--r--   0 alexwlchan   (501) staff       (20)       38 2024-04-30 12:27:51.248004 flickr_photos_api-2.0.1/setup.cfg
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 12:27:51.243214 flickr_photos_api-2.0.1/src/
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 12:27:51.245073 flickr_photos_api-2.0.1/src/flickr_photos_api/
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1172 2024-04-30 12:27:45.000000 flickr_photos_api-2.0.1/src/flickr_photos_api/__init__.py
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 12:27:51.247013 flickr_photos_api-2.0.1/src/flickr_photos_api/api/
--rw-r--r--   0 alexwlchan   (501) staff       (20)      564 2024-04-30 12:06:13.000000 flickr_photos_api-2.0.1/src/flickr_photos_api/api/__init__.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     5267 2024-04-30 12:27:45.000000 flickr_photos_api-2.0.1/src/flickr_photos_api/api/base.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)    10985 2024-04-30 12:06:13.000000 flickr_photos_api-2.0.1/src/flickr_photos_api/api/collection_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1994 2024-04-30 12:06:13.000000 flickr_photos_api-2.0.1/src/flickr_photos_api/api/comment_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     2797 2024-04-30 12:06:13.000000 flickr_photos_api-2.0.1/src/flickr_photos_api/api/from_url_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     3052 2024-04-30 12:06:13.000000 flickr_photos_api-2.0.1/src/flickr_photos_api/api/license_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     9409 2024-04-30 12:06:13.000000 flickr_photos_api-2.0.1/src/flickr_photos_api/api/single_photo_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     6108 2024-04-30 12:27:45.000000 flickr_photos_api-2.0.1/src/flickr_photos_api/api/user_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1836 2024-04-30 12:27:45.000000 flickr_photos_api-2.0.1/src/flickr_photos_api/exceptions.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)       93 2023-11-05 13:33:57.000000 flickr_photos_api-2.0.1/src/flickr_photos_api/py.typed
--rw-r--r--   0 alexwlchan   (501) staff       (20)     3956 2024-04-30 12:06:13.000000 flickr_photos_api-2.0.1/src/flickr_photos_api/types.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     5547 2024-03-21 12:08:35.000000 flickr_photos_api-2.0.1/src/flickr_photos_api/utils.py
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 12:27:51.247569 flickr_photos_api-2.0.1/src/flickr_photos_api.egg-info/
--rw-r--r--   0 alexwlchan   (501) staff       (20)     4070 2024-04-30 12:27:51.000000 flickr_photos_api-2.0.1/src/flickr_photos_api.egg-info/PKG-INFO
--rw-r--r--   0 alexwlchan   (501) staff       (20)      827 2024-04-30 12:27:51.000000 flickr_photos_api-2.0.1/src/flickr_photos_api.egg-info/SOURCES.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)        1 2024-04-30 12:27:51.000000 flickr_photos_api-2.0.1/src/flickr_photos_api.egg-info/dependency_links.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)       62 2024-04-30 12:27:51.000000 flickr_photos_api-2.0.1/src/flickr_photos_api.egg-info/requires.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)       18 2024-04-30 12:27:51.000000 flickr_photos_api-2.0.1/src/flickr_photos_api.egg-info/top_level.txt
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 12:27:51.247289 flickr_photos_api-2.0.1/tests/
--rw-r--r--   0 alexwlchan   (501) staff       (20)     6662 2024-04-30 12:19:46.000000 flickr_photos_api-2.0.1/tests/test_errors.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)      472 2024-01-09 14:51:31.000000 flickr_photos_api-2.0.1/tests/test_utils.py
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 14:50:59.233897 flickr_photos_api-2.1.0/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)    11356 2023-11-05 12:32:45.000000 flickr_photos_api-2.1.0/LICENSE-APACHE
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1074 2023-11-05 12:32:47.000000 flickr_photos_api-2.1.0/LICENSE-MIT
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     4070 2024-04-30 14:50:59.233671 flickr_photos_api-2.1.0/PKG-INFO
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     3172 2024-04-30 12:06:13.000000 flickr_photos_api-2.1.0/README.md
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1856 2024-04-30 14:50:54.000000 flickr_photos_api-2.1.0/pyproject.toml
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       38 2024-04-30 14:50:59.233937 flickr_photos_api-2.1.0/setup.cfg
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 14:50:59.229161 flickr_photos_api-2.1.0/src/
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 14:50:59.231133 flickr_photos_api-2.1.0/src/flickr_photos_api/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1172 2024-04-30 14:50:54.000000 flickr_photos_api-2.1.0/src/flickr_photos_api/__init__.py
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 14:50:59.232958 flickr_photos_api-2.1.0/src/flickr_photos_api/api/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      564 2024-04-30 12:06:13.000000 flickr_photos_api-2.1.0/src/flickr_photos_api/api/__init__.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     5267 2024-04-30 12:27:45.000000 flickr_photos_api-2.1.0/src/flickr_photos_api/api/base.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)    12674 2024-04-30 14:50:54.000000 flickr_photos_api-2.1.0/src/flickr_photos_api/api/collection_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1994 2024-04-30 12:06:13.000000 flickr_photos_api-2.1.0/src/flickr_photos_api/api/comment_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     2234 2024-04-30 14:50:54.000000 flickr_photos_api-2.1.0/src/flickr_photos_api/api/from_url_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     3052 2024-04-30 12:06:13.000000 flickr_photos_api-2.1.0/src/flickr_photos_api/api/license_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     9409 2024-04-30 12:06:13.000000 flickr_photos_api-2.1.0/src/flickr_photos_api/api/single_photo_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     8414 2024-04-30 14:50:54.000000 flickr_photos_api-2.1.0/src/flickr_photos_api/api/user_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1836 2024-04-30 12:27:45.000000 flickr_photos_api-2.1.0/src/flickr_photos_api/exceptions.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       93 2023-11-05 13:33:57.000000 flickr_photos_api-2.1.0/src/flickr_photos_api/py.typed
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     3956 2024-04-30 12:06:13.000000 flickr_photos_api-2.1.0/src/flickr_photos_api/types.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     5547 2024-03-21 12:08:35.000000 flickr_photos_api-2.1.0/src/flickr_photos_api/utils.py
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 14:50:59.233451 flickr_photos_api-2.1.0/src/flickr_photos_api.egg-info/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     4070 2024-04-30 14:50:59.000000 flickr_photos_api-2.1.0/src/flickr_photos_api.egg-info/PKG-INFO
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      827 2024-04-30 14:50:59.000000 flickr_photos_api-2.1.0/src/flickr_photos_api.egg-info/SOURCES.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)        1 2024-04-30 14:50:59.000000 flickr_photos_api-2.1.0/src/flickr_photos_api.egg-info/dependency_links.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       62 2024-04-30 14:50:59.000000 flickr_photos_api-2.1.0/src/flickr_photos_api.egg-info/requires.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       18 2024-04-30 14:50:59.000000 flickr_photos_api-2.1.0/src/flickr_photos_api.egg-info/top_level.txt
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 14:50:59.233198 flickr_photos_api-2.1.0/tests/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     6546 2024-04-30 14:50:54.000000 flickr_photos_api-2.1.0/tests/test_errors.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      472 2024-01-09 14:51:31.000000 flickr_photos_api-2.1.0/tests/test_utils.py
```

### Comparing `flickr_photos_api-2.0.1/LICENSE-APACHE` & `flickr_photos_api-2.1.0/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.0.1/LICENSE-MIT` & `flickr_photos_api-2.1.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.0.1/PKG-INFO` & `flickr_photos_api-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: flickr-photos-api
-Version: 2.0.1
+Version: 2.1.0
 Summary: Look up information about photos and collections of photos from Flickr
 Author-email: Flickr Foundation <hello@flickr.org>
 Maintainer-email: Alex Chan <alex@flickr.org>
 Project-URL: Homepage, https://github.com/Flickr-Foundation/flickr-photos-api
 Project-URL: Changelog, https://github.com/Flickr-Foundation/flickr-photos-api/blob/main/CHANGELOG.md
 Keywords: flickr
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE-APACHE
 License-File: LICENSE-MIT
-Requires-Dist: flickr_url_parser>=1.8.0
+Requires-Dist: flickr_url_parser>=1.8.3
 Requires-Dist: httpx
 Requires-Dist: silver-nitrate>=1.0.1
 Requires-Dist: tenacity
 
 # flickr-photos-api
 
 This is a library for using the Flickr API at the [Flickr Foundation].
```

### Comparing `flickr_photos_api-2.0.1/README.md` & `flickr_photos_api-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.0.1/pyproject.toml` & `flickr_photos_api-2.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: Apache Software License",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3.12",
 ]
 requires-python = ">=3.12"
 dependencies = [
-  "flickr_url_parser>=1.8.0",
+  "flickr_url_parser>=1.8.3",
   "httpx",
   "silver-nitrate>=1.0.1",
   "tenacity",
 ]
 dynamic = ["version"]
 
 [project.urls]
```

### Comparing `flickr_photos_api-2.0.1/src/flickr_photos_api/__init__.py` & `flickr_photos_api-2.1.0/src/flickr_photos_api/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     AlbumInfo,
     GalleryInfo,
     GroupInfo,
     SinglePhotoInfo,
 )
 
 
-__version__ = "2.0.1"
+__version__ = "2.1.0"
 
 
 __all__ = [
     "FlickrApi",
     "FlickrApiException",
     "ResourceNotFound",
     "InvalidApiKey",
```

### Comparing `flickr_photos_api-2.0.1/src/flickr_photos_api/api/__init__.py` & `flickr_photos_api-2.1.0/src/flickr_photos_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.0.1/src/flickr_photos_api/api/base.py` & `flickr_photos_api-2.1.0/src/flickr_photos_api/api/base.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.0.1/src/flickr_photos_api/api/collection_methods.py` & `flickr_photos_api-2.1.0/src/flickr_photos_api/api/collection_methods.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 
 from xml.etree import ElementTree as ET
 
 from nitrate.xml import find_optional_text, find_required_elem, find_required_text
 
 from .license_methods import LicenseMethods
+from .user_methods import UserMethods
 from ..types import (
     CollectionOfPhotos,
     GroupInfo,
     PhotosInAlbum,
     PhotosInGallery,
     PhotosInGroup,
     SinglePhotoInfoWithSizes,
@@ -23,15 +24,15 @@
     parse_date_taken,
     parse_location,
     parse_safety_level,
     parse_sizes,
 )
 
 
-class CollectionMethods(LicenseMethods):
+class CollectionMethods(LicenseMethods, UserMethods):
     def _from_collection_photo(
         self, photo_elem: ET.Element, owner: User | None
     ) -> SinglePhotoInfoWithSizes:
         """
         Given a <photo> element from a collection response, extract all the photo info.
         """
         photo_id = photo_elem.attrib["id"]
@@ -157,15 +158,44 @@
         return {
             "photos": photos,
             "count_pages": count_pages,
             "count_photos": count_photos,
         }
 
     def get_photos_in_album(
-        self, *, user_id: str, album_id: str, page: int = 1, per_page: int = 10
+        self,
+        album_id: str,
+        user_id: str | None = None,
+        user_url: str | None = None,
+        page: int = 1,
+        per_page: int = 10,
+    ) -> PhotosInAlbum:
+        """
+        Get a page of photos from an album.
+
+        You need to pass a numeric album ID and one of the ``user_id`` or ``user_url``.
+
+        For example, if the album URL is
+
+            https://www.flickr.com/photos/158685238@N03/albums/72177720313849533/
+
+        then you need to pass one of:
+
+            {"album_id": "72177720313849533", "user_id": "158685238@N03"}
+            {"album_id": "72177720313849533", "user_url": "https://www.flickr.com/photos/158685238@N03/"}
+
+        """
+        user_id = self._ensure_user_id(user_id=user_id, user_url=user_url)
+
+        return self._get_photos_in_album(
+            user_id=user_id, album_id=album_id, page=page, per_page=per_page
+        )
+
+    def _get_photos_in_album(
+        self, *, user_id: str, album_id: str, page: int, per_page: int
     ) -> PhotosInAlbum:
         """
         Get a page of photos from an album.
         """
         # https://www.flickr.com/services/api/flickr.photosets.getPhotos.html
         resp = self.call(
             method="flickr.photosets.getPhotos",
@@ -226,19 +256,44 @@
 
         return {
             **self._create_collection(photos_elem),
             "gallery": {"owner_name": gallery_owner_name, "title": gallery_title},
         }
 
     def get_photos_in_user_photostream(
-        self, *, user_id: str, page: int = 1, per_page: int = 10
+        self,
+        user_id: str | None = None,
+        user_url: str | None = None,
+        page: int = 1,
+        per_page: int = 10,
     ) -> CollectionOfPhotos:
         """
-        Get a page of photos in a user's photostream.
+        Get a page of photos from a user's photostream.
+
+        You need to pass either the ``user_id`` or ``user_url``.
+
+        For example, if the person's URL is
+
+            https://www.flickr.com/photos/158685238@N03/
+
+        then you need to pass one of:
+
+            {"user_id": "158685238@N03"}
+            {"user_url": "https://www.flickr.com/photos/158685238@N03/"}
+
         """
+        user_id = self._ensure_user_id(user_id=user_id, user_url=user_url)
+
+        return self._get_photos_in_user_photostream(
+            user_id=user_id, page=page, per_page=per_page
+        )
+
+    def _get_photos_in_user_photostream(
+        self, *, user_id: str, page: int, per_page: int
+    ) -> CollectionOfPhotos:
         resp = self.call(
             method="flickr.people.getPublicPhotos",
             params={
                 "user_id": user_id,
                 "extras": ",".join(self.extras),
                 "page": str(page),
                 "per_page": str(per_page),
```

### Comparing `flickr_photos_api-2.0.1/src/flickr_photos_api/api/comment_methods.py` & `flickr_photos_api-2.1.0/src/flickr_photos_api/api/comment_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.0.1/src/flickr_photos_api/api/from_url_methods.py` & `flickr_photos_api-2.1.0/src/flickr_photos_api/api/from_url_methods.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,42 +24,23 @@
         """
         Given a URL on Flickr.com that's been parsed with flickr-url-parser,
         return the photos at that URL (if possible).
         """
         if parsed_url["type"] == "single_photo":
             return self.get_single_photo(photo_id=parsed_url["photo_id"])
         elif parsed_url["type"] == "album":
-            parsed_user_url = parse_flickr_url(parsed_url["user_url"])
-            assert parsed_user_url["type"] == "user"
-
-            user_id = parsed_user_url["user_id"]
-
-            if user_id is None:
-                user = self.lookup_user_by_url(url=parsed_user_url["user_url"])
-                user_id = user["id"]
-
-            assert user_id is not None
-
             return self.get_photos_in_album(
-                user_id=user_id,
+                user_url=parsed_url["user_url"],
                 album_id=parsed_url["album_id"],
                 page=parsed_url["page"],
                 per_page=100,
             )
         elif parsed_url["type"] == "user":
-            user_id = parsed_url["user_id"]
-
-            if user_id is None:
-                user = self.lookup_user_by_url(url=parsed_url["user_url"])
-                user_id = user["id"]
-
-            assert user_id is not None
-
             return self.get_photos_in_user_photostream(
-                user_id=user_id, page=parsed_url["page"], per_page=100
+                user_url=parsed_url["user_url"], page=parsed_url["page"], per_page=100
             )
         elif parsed_url["type"] == "gallery":
             return self.get_photos_in_gallery(
                 gallery_id=parsed_url["gallery_id"],
                 page=parsed_url["page"],
                 per_page=100,
             )
```

### Comparing `flickr_photos_api-2.0.1/src/flickr_photos_api/api/license_methods.py` & `flickr_photos_api-2.1.0/src/flickr_photos_api/api/license_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.0.1/src/flickr_photos_api/api/single_photo_methods.py` & `flickr_photos_api-2.1.0/src/flickr_photos_api/api/single_photo_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.0.1/src/flickr_photos_api/exceptions.py` & `flickr_photos_api-2.1.0/src/flickr_photos_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.0.1/src/flickr_photos_api/types.py` & `flickr_photos_api-2.1.0/src/flickr_photos_api/types.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.0.1/src/flickr_photos_api/utils.py` & `flickr_photos_api-2.1.0/src/flickr_photos_api/utils.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.0.1/src/flickr_photos_api.egg-info/PKG-INFO` & `flickr_photos_api-2.1.0/src/flickr_photos_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: flickr-photos-api
-Version: 2.0.1
+Version: 2.1.0
 Summary: Look up information about photos and collections of photos from Flickr
 Author-email: Flickr Foundation <hello@flickr.org>
 Maintainer-email: Alex Chan <alex@flickr.org>
 Project-URL: Homepage, https://github.com/Flickr-Foundation/flickr-photos-api
 Project-URL: Changelog, https://github.com/Flickr-Foundation/flickr-photos-api/blob/main/CHANGELOG.md
 Keywords: flickr
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE-APACHE
 License-File: LICENSE-MIT
-Requires-Dist: flickr_url_parser>=1.8.0
+Requires-Dist: flickr_url_parser>=1.8.3
 Requires-Dist: httpx
 Requires-Dist: silver-nitrate>=1.0.1
 Requires-Dist: tenacity
 
 # flickr-photos-api
 
 This is a library for using the Flickr API at the [Flickr Foundation].
```

### Comparing `flickr_photos_api-2.0.1/src/flickr_photos_api.egg-info/SOURCES.txt` & `flickr_photos_api-2.1.0/src/flickr_photos_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.0.1/tests/test_errors.py` & `flickr_photos_api-2.1.0/tests/test_errors.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import httpx
 import pytest
 
 from flickr_photos_api import (
-    FlickrApi as FlickrPhotosApi,
+    FlickrApi,
     FlickrApiException,
     InvalidApiKey,
     InvalidXmlException,
     ResourceNotFound,
 )
 
 
 @pytest.mark.parametrize(
     ["method", "params"],
     [
         pytest.param(
-            "lookup_user_by_url",
-            {"url": "https://www.flickr.com/photos/DefinitelyDoesNotExist"},
-            id="lookup_user_by_url",
+            "get_user",
+            {"user_url": "https://www.flickr.com/photos/DefinitelyDoesNotExist"},
+            id="get_user_by_url",
         ),
         pytest.param(
-            "lookup_user_by_id",
+            "get_user",
             {"user_id": "1234567@N00"},
-            id="lookup_user_by_id",
+            id="get_user_by_id",
         ),
         pytest.param(
             "get_single_photo",
             {"photo_id": "12345678901234567890"},
             id="get_single_photo",
         ),
         pytest.param(
@@ -58,38 +58,38 @@
             "get_photos_in_group_pool",
             {"group_url": "https://www.flickr.com/groups/doesnotexist/pool/"},
             id="get_photos_in_non_existent_group_pool",
         ),
     ],
 )
 def test_methods_fail_if_not_found(
-    api: FlickrPhotosApi, method: str, params: dict[str, str]
+    api: FlickrApi, method: str, params: dict[str, str]
 ) -> None:
     api_method = getattr(api, method)
 
     with pytest.raises(ResourceNotFound):
         api_method(**params)
 
 
 def test_it_throws_if_bad_auth(vcr_cassette: str, user_agent: str) -> None:
-    api = FlickrPhotosApi(api_key="doesnotexist", user_agent=user_agent)
+    api = FlickrApi(api_key="doesnotexist", user_agent=user_agent)
 
     with pytest.raises(FlickrApiException):
-        api.lookup_user_by_url(url="https://www.flickr.com/photos/flickr/")
+        api.get_user(user_url="https://www.flickr.com/photos/flickr/")
 
 
 def test_empty_api_key_is_error(user_agent: str) -> None:
     with pytest.raises(
         ValueError, match="Cannot create a client with an empty string as the API key"
     ):
-        FlickrPhotosApi(api_key="", user_agent=user_agent)
+        FlickrApi(api_key="", user_agent=user_agent)
 
 
 def test_invalid_api_key_is_error(user_agent: str) -> None:
-    api = FlickrPhotosApi(api_key="<bad key>", user_agent=user_agent)
+    api = FlickrApi(api_key="<bad key>", user_agent=user_agent)
 
     with pytest.raises(InvalidApiKey) as err:
         api.get_single_photo(photo_id="52578982111")
 
     assert (
         err.value.args[0]
         == "Flickr API rejected the API key as invalid (Key has invalid format)"
@@ -100,15 +100,15 @@
     #
     #     ResourceWarning: unclosed <ssl.SSLSocket fd=13, family=2,
     #     type=1, proto=0, laddr=('…', 58686), raddr=('…', 443)>
     #
     api.client.close()
 
 
-def test_a_timeout_is_retried(api: FlickrPhotosApi) -> None:
+def test_a_timeout_is_retried(api: FlickrApi) -> None:
     # This client throws a timeout error on the first GET request,
     # and then makes regular HTTP requests after that.
     class FlakyClient:
         def __init__(self, underlying: httpx.Client):
             self.underlying = underlying
             self.get_request_count = 0
 
@@ -123,70 +123,70 @@
     api.client = FlakyClient(underlying=api.client)  # type: ignore
 
     resp = api.get_photos_in_user_photostream(user_id="61270229@N05")
 
     assert len(resp["photos"]) == 10
 
 
-def test_retries_5xx_error(api: FlickrPhotosApi) -> None:
+def test_retries_5xx_error(api: FlickrApi) -> None:
     # The cassette for this test was constructed manually: I edited
     # an existing cassette to add a 500 response as the first response,
     # then we want to see it make a second request to retry it.
     resp = api.get_photos_in_user_photostream(user_id="61270229@N05")
 
     assert len(resp["photos"]) == 10
 
 
-def test_a_persistent_5xx_error_is_raised(api: FlickrPhotosApi) -> None:
+def test_a_persistent_5xx_error_is_raised(api: FlickrApi) -> None:
     # The cassette for this test was constructed manually: I copy/pasted
     # the 500 response from the previous test so that there were more
     # than it would retry.
     with pytest.raises(httpx.HTTPStatusError) as err:
         api.get_photos_in_user_photostream(user_id="61270229@N05")
 
     assert err.value.response.status_code == 500
 
 
-def test_retries_invalid_xml_error(api: FlickrPhotosApi) -> None:
+def test_retries_invalid_xml_error(api: FlickrApi) -> None:
     # The cassette for this test was constructed manually: I edited
     # an existing cassette to add the invalid XML as the first response,
     # then we want to see it make a second request to retry it.
     resp = api.get_photos_in_user_photostream(user_id="61270229@N05")
 
     assert len(resp["photos"]) == 10
 
 
-def test_a_persistent_invalid_xml_error_is_raised(api: FlickrPhotosApi) -> None:
+def test_a_persistent_invalid_xml_error_is_raised(api: FlickrApi) -> None:
     # The cassette for this test was constructed manually: I copy/pasted
     # the invalid XML from the previous test so that there were more
     # than it would retry.
     with pytest.raises(InvalidXmlException):
         api.get_photos_in_user_photostream(user_id="61270229@N05")
 
 
-def test_retries_error_code_201(api: FlickrPhotosApi) -> None:
+def test_retries_error_code_201(api: FlickrApi) -> None:
     # The cassette for this test was constructed manually: I edited
     # an existing cassette to add the invalid XML as the first response,
     # then we want to see it make a second request to retry it.
     resp = api.get_photos_in_user_photostream(user_id="61270229@N05")
 
     assert len(resp["photos"]) == 10
 
 
-def test_a_persistent_error_201_is_raised(api: FlickrPhotosApi) -> None:
+def test_a_persistent_error_201_is_raised(api: FlickrApi) -> None:
     # The cassette for this test was constructed manually: I edited
     # an existing cassette to add the invalid XML as the first response,
     # then we want to see it make a second request to retry it.
     with pytest.raises(FlickrApiException) as exc:
         api.get_photos_in_user_photostream(user_id="61270229@N05")
 
     assert exc.value.args[0] == {
         "code": "201",
         "msg": "Sorry, the Flickr API service is not currently available.",
     }
 
 
-def test_an_unrecognised_error_is_generic_exception(api: FlickrPhotosApi) -> None:
+def test_an_unrecognised_error_is_generic_exception(api: FlickrApi) -> None:
     with pytest.raises(FlickrApiException) as exc:
         api.call(method="flickr.test.null")
 
     assert exc.value.args[0]["code"] == "99"
```

