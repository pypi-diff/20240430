# Comparing `tmp/flickr_photos_api-2.0.0.tar.gz` & `tmp/flickr_photos_api-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flickr_photos_api-2.0.0.tar", last modified: Tue Apr 30 10:34:07 2024, max compression
+gzip compressed data, was "flickr_photos_api-2.0.1.tar", last modified: Tue Apr 30 12:27:51 2024, max compression
```

## Comparing `flickr_photos_api-2.0.0.tar` & `flickr_photos_api-2.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 10:34:07.913467 flickr_photos_api-2.0.0/
--rw-r--r--   0 alexwlchan   (501) staff       (20)    11356 2023-11-05 12:32:45.000000 flickr_photos_api-2.0.0/LICENSE-APACHE
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1074 2023-11-05 12:32:47.000000 flickr_photos_api-2.0.0/LICENSE-MIT
--rw-r--r--   0 alexwlchan   (501) staff       (20)     4070 2024-04-30 10:34:07.913288 flickr_photos_api-2.0.0/PKG-INFO
--rw-r--r--   0 alexwlchan   (501) staff       (20)     3172 2024-04-30 10:34:01.000000 flickr_photos_api-2.0.0/README.md
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1856 2024-04-30 10:34:01.000000 flickr_photos_api-2.0.0/pyproject.toml
--rw-r--r--   0 alexwlchan   (501) staff       (20)       38 2024-04-30 10:34:07.913511 flickr_photos_api-2.0.0/setup.cfg
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 10:34:07.909504 flickr_photos_api-2.0.0/src/
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 10:34:07.911063 flickr_photos_api-2.0.0/src/flickr_photos_api/
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1062 2024-04-30 10:34:01.000000 flickr_photos_api-2.0.0/src/flickr_photos_api/__init__.py
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 10:34:07.912623 flickr_photos_api-2.0.0/src/flickr_photos_api/api/
--rw-r--r--   0 alexwlchan   (501) staff       (20)      564 2024-04-30 10:34:01.000000 flickr_photos_api-2.0.0/src/flickr_photos_api/api/__init__.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     5144 2024-04-30 10:34:01.000000 flickr_photos_api-2.0.0/src/flickr_photos_api/api/base.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)    10985 2024-04-30 10:34:01.000000 flickr_photos_api-2.0.0/src/flickr_photos_api/api/collection_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1994 2024-04-30 10:34:01.000000 flickr_photos_api-2.0.0/src/flickr_photos_api/api/comment_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     2797 2024-04-30 10:34:01.000000 flickr_photos_api-2.0.0/src/flickr_photos_api/api/from_url_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     3052 2024-04-30 10:34:01.000000 flickr_photos_api-2.0.0/src/flickr_photos_api/api/license_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     9409 2024-04-30 10:34:01.000000 flickr_photos_api-2.0.0/src/flickr_photos_api/api/single_photo_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     5834 2024-04-30 10:34:01.000000 flickr_photos_api-2.0.0/src/flickr_photos_api/api/user_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1632 2024-04-29 17:26:18.000000 flickr_photos_api-2.0.0/src/flickr_photos_api/exceptions.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)       93 2023-11-05 13:33:57.000000 flickr_photos_api-2.0.0/src/flickr_photos_api/py.typed
--rw-r--r--   0 alexwlchan   (501) staff       (20)     3956 2024-04-30 10:34:01.000000 flickr_photos_api-2.0.0/src/flickr_photos_api/types.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     5547 2024-03-21 12:08:35.000000 flickr_photos_api-2.0.0/src/flickr_photos_api/utils.py
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 10:34:07.913119 flickr_photos_api-2.0.0/src/flickr_photos_api.egg-info/
--rw-r--r--   0 alexwlchan   (501) staff       (20)     4070 2024-04-30 10:34:07.000000 flickr_photos_api-2.0.0/src/flickr_photos_api.egg-info/PKG-INFO
--rw-r--r--   0 alexwlchan   (501) staff       (20)      827 2024-04-30 10:34:07.000000 flickr_photos_api-2.0.0/src/flickr_photos_api.egg-info/SOURCES.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)        1 2024-04-30 10:34:07.000000 flickr_photos_api-2.0.0/src/flickr_photos_api.egg-info/dependency_links.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)       62 2024-04-30 10:34:07.000000 flickr_photos_api-2.0.0/src/flickr_photos_api.egg-info/requires.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)       18 2024-04-30 10:34:07.000000 flickr_photos_api-2.0.0/src/flickr_photos_api.egg-info/top_level.txt
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 10:34:07.912863 flickr_photos_api-2.0.0/tests/
--rw-r--r--   0 alexwlchan   (501) staff       (20)     6662 2024-04-30 10:34:01.000000 flickr_photos_api-2.0.0/tests/test_errors.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)      472 2024-01-09 14:51:31.000000 flickr_photos_api-2.0.0/tests/test_utils.py
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 12:27:51.247959 flickr_photos_api-2.0.1/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)    11356 2023-11-05 12:32:45.000000 flickr_photos_api-2.0.1/LICENSE-APACHE
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1074 2023-11-05 12:32:47.000000 flickr_photos_api-2.0.1/LICENSE-MIT
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     4070 2024-04-30 12:27:51.247782 flickr_photos_api-2.0.1/PKG-INFO
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     3172 2024-04-30 12:06:13.000000 flickr_photos_api-2.0.1/README.md
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1856 2024-04-30 12:06:13.000000 flickr_photos_api-2.0.1/pyproject.toml
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       38 2024-04-30 12:27:51.248004 flickr_photos_api-2.0.1/setup.cfg
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 12:27:51.243214 flickr_photos_api-2.0.1/src/
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 12:27:51.245073 flickr_photos_api-2.0.1/src/flickr_photos_api/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1172 2024-04-30 12:27:45.000000 flickr_photos_api-2.0.1/src/flickr_photos_api/__init__.py
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 12:27:51.247013 flickr_photos_api-2.0.1/src/flickr_photos_api/api/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      564 2024-04-30 12:06:13.000000 flickr_photos_api-2.0.1/src/flickr_photos_api/api/__init__.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     5267 2024-04-30 12:27:45.000000 flickr_photos_api-2.0.1/src/flickr_photos_api/api/base.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)    10985 2024-04-30 12:06:13.000000 flickr_photos_api-2.0.1/src/flickr_photos_api/api/collection_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1994 2024-04-30 12:06:13.000000 flickr_photos_api-2.0.1/src/flickr_photos_api/api/comment_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     2797 2024-04-30 12:06:13.000000 flickr_photos_api-2.0.1/src/flickr_photos_api/api/from_url_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     3052 2024-04-30 12:06:13.000000 flickr_photos_api-2.0.1/src/flickr_photos_api/api/license_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     9409 2024-04-30 12:06:13.000000 flickr_photos_api-2.0.1/src/flickr_photos_api/api/single_photo_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     6108 2024-04-30 12:27:45.000000 flickr_photos_api-2.0.1/src/flickr_photos_api/api/user_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1836 2024-04-30 12:27:45.000000 flickr_photos_api-2.0.1/src/flickr_photos_api/exceptions.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       93 2023-11-05 13:33:57.000000 flickr_photos_api-2.0.1/src/flickr_photos_api/py.typed
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     3956 2024-04-30 12:06:13.000000 flickr_photos_api-2.0.1/src/flickr_photos_api/types.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     5547 2024-03-21 12:08:35.000000 flickr_photos_api-2.0.1/src/flickr_photos_api/utils.py
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 12:27:51.247569 flickr_photos_api-2.0.1/src/flickr_photos_api.egg-info/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     4070 2024-04-30 12:27:51.000000 flickr_photos_api-2.0.1/src/flickr_photos_api.egg-info/PKG-INFO
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      827 2024-04-30 12:27:51.000000 flickr_photos_api-2.0.1/src/flickr_photos_api.egg-info/SOURCES.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)        1 2024-04-30 12:27:51.000000 flickr_photos_api-2.0.1/src/flickr_photos_api.egg-info/dependency_links.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       62 2024-04-30 12:27:51.000000 flickr_photos_api-2.0.1/src/flickr_photos_api.egg-info/requires.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       18 2024-04-30 12:27:51.000000 flickr_photos_api-2.0.1/src/flickr_photos_api.egg-info/top_level.txt
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 12:27:51.247289 flickr_photos_api-2.0.1/tests/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     6662 2024-04-30 12:19:46.000000 flickr_photos_api-2.0.1/tests/test_errors.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      472 2024-01-09 14:51:31.000000 flickr_photos_api-2.0.1/tests/test_utils.py
```

### Comparing `flickr_photos_api-2.0.0/LICENSE-APACHE` & `flickr_photos_api-2.0.1/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.0.0/LICENSE-MIT` & `flickr_photos_api-2.0.1/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.0.0/PKG-INFO` & `flickr_photos_api-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flickr-photos-api
-Version: 2.0.0
+Version: 2.0.1
 Summary: Look up information about photos and collections of photos from Flickr
 Author-email: Flickr Foundation <hello@flickr.org>
 Maintainer-email: Alex Chan <alex@flickr.org>
 Project-URL: Homepage, https://github.com/Flickr-Foundation/flickr-photos-api
 Project-URL: Changelog, https://github.com/Flickr-Foundation/flickr-photos-api/blob/main/CHANGELOG.md
 Keywords: flickr
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `flickr_photos_api-2.0.0/README.md` & `flickr_photos_api-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.0.0/pyproject.toml` & `flickr_photos_api-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.0.0/src/flickr_photos_api/__init__.py` & `flickr_photos_api-2.0.1/src/flickr_photos_api/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from .api import FlickrApi
 from .exceptions import (
     FlickrApiException,
     InvalidApiKey,
     InvalidXmlException,
     ResourceNotFound,
     LicenseNotFound,
+    UnrecognisedFlickrApiException,
+    UserDeleted,
 )
 from .types import (
     Comment,
     License,
     User,
     UserInfo,
     TakenGranularity,
@@ -25,15 +27,15 @@
     AlbumInfo,
     GalleryInfo,
     GroupInfo,
     SinglePhotoInfo,
 )
 
 
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 
 
 __all__ = [
     "FlickrApi",
     "FlickrApiException",
     "ResourceNotFound",
     "InvalidApiKey",
@@ -54,9 +56,11 @@
     "PhotosFromUrl",
     "PhotosInAlbum",
     "PhotosInGallery",
     "PhotosInGroup",
     "AlbumInfo",
     "GalleryInfo",
     "GroupInfo",
+    "UnrecognisedFlickrApiException",
+    "UserDeleted",
     "__version__",
 ]
```

### Comparing `flickr_photos_api-2.0.0/src/flickr_photos_api/api/__init__.py` & `flickr_photos_api-2.0.1/src/flickr_photos_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.0.0/src/flickr_photos_api/api/base.py` & `flickr_photos_api-2.0.1/src/flickr_photos_api/api/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,18 +8,18 @@
     retry_if_exception,
     RetryError,
     stop_after_attempt,
     wait_random_exponential,
 )
 
 from ..exceptions import (
-    FlickrApiException,
     InvalidApiKey,
     InvalidXmlException,
     ResourceNotFound,
+    UnrecognisedFlickrApiException,
 )
 
 
 class FlickrApi(abc.ABC):
     """
     This is a basic model for Flickr API implementations: they have to provide
     a ``call()`` method that takes a Flickr API method and parameters, and returns
@@ -55,15 +55,15 @@
     #     <err
     #       code="201"
     #       msg="Sorry, the Flickr API service is not currently available."
     #     />
     #
     # but this indicates a flaky connection rather than a genuine failure.
     if (
-        isinstance(exc, FlickrApiException)
+        isinstance(exc, UnrecognisedFlickrApiException)
         and isinstance(exc.args[0], dict)
         and exc.args[0].get("code") == "201"
     ):
         return True
 
     return False
 
@@ -141,14 +141,16 @@
             # Although I haven't found any explicit documentation of this,
             # it seems like a pretty common convention that:
             #
             #   - error code "1" means "not found"
             #   - error code "2" means "user not found"
             #
             if errors["code"] == "1" or errors["code"] == "2":
-                raise ResourceNotFound(method, params)
+                raise ResourceNotFound(
+                    f"Unable to find resource at {method} with properties {params}"
+                )
             elif errors["code"] == "100":
                 raise InvalidApiKey(message=errors["msg"])
             else:
-                raise FlickrApiException(errors)
+                raise UnrecognisedFlickrApiException(errors)
 
         return xml
```

### Comparing `flickr_photos_api-2.0.0/src/flickr_photos_api/api/collection_methods.py` & `flickr_photos_api-2.0.1/src/flickr_photos_api/api/collection_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.0.0/src/flickr_photos_api/api/comment_methods.py` & `flickr_photos_api-2.0.1/src/flickr_photos_api/api/comment_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.0.0/src/flickr_photos_api/api/from_url_methods.py` & `flickr_photos_api-2.0.1/src/flickr_photos_api/api/from_url_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.0.0/src/flickr_photos_api/api/license_methods.py` & `flickr_photos_api-2.0.1/src/flickr_photos_api/api/license_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.0.0/src/flickr_photos_api/api/single_photo_methods.py` & `flickr_photos_api-2.0.1/src/flickr_photos_api/api/single_photo_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.0.0/src/flickr_photos_api/api/user_methods.py` & `flickr_photos_api-2.0.1/src/flickr_photos_api/api/user_methods.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import functools
 
 from flickr_url_parser import parse_flickr_url
 from nitrate.xml import find_optional_text, find_required_elem, find_required_text
 
 from .base import FlickrApi
+from ..exceptions import UnrecognisedFlickrApiException, UserDeleted
 from ..types import UserInfo
 
 
 class UserMethods(FlickrApi):
     def lookup_user_by_id(self, *, user_id: str) -> UserInfo:
         """
         Given the link to a user's photos or profile, return their info.
@@ -42,17 +43,23 @@
         #       <profileurl>flickr.com/people/britishlibrary/</profileurl>
         #       <photos>
         #         <count>1234</count>
         #       </photos>
         #       …
         #     </person>
         #
-        info_resp = self.call(
-            method="flickr.people.getInfo", params={"user_id": user_id}
-        )
+        try:
+            info_resp = self.call(
+                method="flickr.people.getInfo", params={"user_id": user_id}
+            )
+        except UnrecognisedFlickrApiException as exc:
+            if exc.args[0]["code"] == "5":
+                raise UserDeleted(user_id)
+            else:
+                raise
 
         person_elem = find_required_elem(info_resp, path="person")
 
         username = find_required_text(person_elem, path="username")
         photos_url = find_required_text(person_elem, path="photosurl")
         profile_url = find_required_text(person_elem, path="profileurl")
         description = find_optional_text(person_elem, path="description")
```

### Comparing `flickr_photos_api-2.0.0/src/flickr_photos_api/types.py` & `flickr_photos_api-2.0.1/src/flickr_photos_api/types.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.0.0/src/flickr_photos_api/utils.py` & `flickr_photos_api-2.0.1/src/flickr_photos_api/utils.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.0.0/src/flickr_photos_api.egg-info/PKG-INFO` & `flickr_photos_api-2.0.1/src/flickr_photos_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flickr-photos-api
-Version: 2.0.0
+Version: 2.0.1
 Summary: Look up information about photos and collections of photos from Flickr
 Author-email: Flickr Foundation <hello@flickr.org>
 Maintainer-email: Alex Chan <alex@flickr.org>
 Project-URL: Homepage, https://github.com/Flickr-Foundation/flickr-photos-api
 Project-URL: Changelog, https://github.com/Flickr-Foundation/flickr-photos-api/blob/main/CHANGELOG.md
 Keywords: flickr
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `flickr_photos_api-2.0.0/src/flickr_photos_api.egg-info/SOURCES.txt` & `flickr_photos_api-2.0.1/src/flickr_photos_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.0.0/tests/test_errors.py` & `flickr_photos_api-2.0.1/tests/test_errors.py`

 * *Files identical despite different names*

