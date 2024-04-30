# Comparing `tmp/flickr-photos-api-1.9.2.tar.gz` & `tmp/flickr_photos_api-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flickr-photos-api-1.9.2.tar", last modified: Tue Apr  2 13:08:20 2024, max compression
+gzip compressed data, was "flickr_photos_api-2.0.0.tar", last modified: Tue Apr 30 10:34:07 2024, max compression
```

## Comparing `flickr-photos-api-1.9.2.tar` & `flickr_photos_api-2.0.0.tar`

### file list

```diff
@@ -1,25 +1,32 @@
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-02 13:08:20.612800 flickr-photos-api-1.9.2/
--rw-r--r--   0 alexwlchan   (501) staff       (20)    11356 2023-11-05 12:32:45.000000 flickr-photos-api-1.9.2/LICENSE-APACHE
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1074 2023-11-05 12:32:47.000000 flickr-photos-api-1.9.2/LICENSE-MIT
--rw-r--r--   0 alexwlchan   (501) staff       (20)     3346 2024-04-02 13:08:20.612619 flickr-photos-api-1.9.2/PKG-INFO
--rw-r--r--   0 alexwlchan   (501) staff       (20)     2448 2023-12-27 10:54:19.000000 flickr-photos-api-1.9.2/README.md
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1810 2024-01-04 12:06:41.000000 flickr-photos-api-1.9.2/pyproject.toml
--rw-r--r--   0 alexwlchan   (501) staff       (20)       38 2024-04-02 13:08:20.612843 flickr-photos-api-1.9.2/setup.cfg
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-02 13:08:20.607174 flickr-photos-api-1.9.2/src/
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-02 13:08:20.609266 flickr-photos-api-1.9.2/src/flickr_photos_api/
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1002 2024-04-02 13:08:13.000000 flickr-photos-api-1.9.2/src/flickr_photos_api/__init__.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)    32718 2024-04-02 13:08:13.000000 flickr-photos-api-1.9.2/src/flickr_photos_api/api.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1632 2024-01-04 12:06:41.000000 flickr-photos-api-1.9.2/src/flickr_photos_api/exceptions.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)       93 2023-11-05 13:33:57.000000 flickr-photos-api-1.9.2/src/flickr_photos_api/py.typed
--rw-r--r--   0 alexwlchan   (501) staff       (20)     2063 2024-03-26 11:13:22.000000 flickr-photos-api-1.9.2/src/flickr_photos_api/types.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     5547 2024-03-21 12:08:35.000000 flickr-photos-api-1.9.2/src/flickr_photos_api/utils.py
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-02 13:08:20.612403 flickr-photos-api-1.9.2/src/flickr_photos_api.egg-info/
--rw-r--r--   0 alexwlchan   (501) staff       (20)     3346 2024-04-02 13:08:20.000000 flickr-photos-api-1.9.2/src/flickr_photos_api.egg-info/PKG-INFO
--rw-r--r--   0 alexwlchan   (501) staff       (20)      526 2024-04-02 13:08:20.000000 flickr-photos-api-1.9.2/src/flickr_photos_api.egg-info/SOURCES.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)        1 2024-04-02 13:08:20.000000 flickr-photos-api-1.9.2/src/flickr_photos_api.egg-info/dependency_links.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)       62 2024-04-02 13:08:20.000000 flickr-photos-api-1.9.2/src/flickr_photos_api.egg-info/requires.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)       18 2024-04-02 13:08:20.000000 flickr-photos-api-1.9.2/src/flickr_photos_api.egg-info/top_level.txt
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-02 13:08:20.612145 flickr-photos-api-1.9.2/tests/
--rw-r--r--   0 alexwlchan   (501) staff       (20)    21130 2024-03-26 11:13:22.000000 flickr-photos-api-1.9.2/tests/test_api.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     7091 2024-03-26 10:37:52.000000 flickr-photos-api-1.9.2/tests/test_errors.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)      472 2024-01-09 14:51:31.000000 flickr-photos-api-1.9.2/tests/test_utils.py
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 10:34:07.913467 flickr_photos_api-2.0.0/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)    11356 2023-11-05 12:32:45.000000 flickr_photos_api-2.0.0/LICENSE-APACHE
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1074 2023-11-05 12:32:47.000000 flickr_photos_api-2.0.0/LICENSE-MIT
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     4070 2024-04-30 10:34:07.913288 flickr_photos_api-2.0.0/PKG-INFO
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     3172 2024-04-30 10:34:01.000000 flickr_photos_api-2.0.0/README.md
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1856 2024-04-30 10:34:01.000000 flickr_photos_api-2.0.0/pyproject.toml
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       38 2024-04-30 10:34:07.913511 flickr_photos_api-2.0.0/setup.cfg
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 10:34:07.909504 flickr_photos_api-2.0.0/src/
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 10:34:07.911063 flickr_photos_api-2.0.0/src/flickr_photos_api/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1062 2024-04-30 10:34:01.000000 flickr_photos_api-2.0.0/src/flickr_photos_api/__init__.py
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 10:34:07.912623 flickr_photos_api-2.0.0/src/flickr_photos_api/api/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      564 2024-04-30 10:34:01.000000 flickr_photos_api-2.0.0/src/flickr_photos_api/api/__init__.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     5144 2024-04-30 10:34:01.000000 flickr_photos_api-2.0.0/src/flickr_photos_api/api/base.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)    10985 2024-04-30 10:34:01.000000 flickr_photos_api-2.0.0/src/flickr_photos_api/api/collection_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1994 2024-04-30 10:34:01.000000 flickr_photos_api-2.0.0/src/flickr_photos_api/api/comment_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     2797 2024-04-30 10:34:01.000000 flickr_photos_api-2.0.0/src/flickr_photos_api/api/from_url_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     3052 2024-04-30 10:34:01.000000 flickr_photos_api-2.0.0/src/flickr_photos_api/api/license_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     9409 2024-04-30 10:34:01.000000 flickr_photos_api-2.0.0/src/flickr_photos_api/api/single_photo_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     5834 2024-04-30 10:34:01.000000 flickr_photos_api-2.0.0/src/flickr_photos_api/api/user_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1632 2024-04-29 17:26:18.000000 flickr_photos_api-2.0.0/src/flickr_photos_api/exceptions.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       93 2023-11-05 13:33:57.000000 flickr_photos_api-2.0.0/src/flickr_photos_api/py.typed
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     3956 2024-04-30 10:34:01.000000 flickr_photos_api-2.0.0/src/flickr_photos_api/types.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     5547 2024-03-21 12:08:35.000000 flickr_photos_api-2.0.0/src/flickr_photos_api/utils.py
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 10:34:07.913119 flickr_photos_api-2.0.0/src/flickr_photos_api.egg-info/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     4070 2024-04-30 10:34:07.000000 flickr_photos_api-2.0.0/src/flickr_photos_api.egg-info/PKG-INFO
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      827 2024-04-30 10:34:07.000000 flickr_photos_api-2.0.0/src/flickr_photos_api.egg-info/SOURCES.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)        1 2024-04-30 10:34:07.000000 flickr_photos_api-2.0.0/src/flickr_photos_api.egg-info/dependency_links.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       62 2024-04-30 10:34:07.000000 flickr_photos_api-2.0.0/src/flickr_photos_api.egg-info/requires.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       18 2024-04-30 10:34:07.000000 flickr_photos_api-2.0.0/src/flickr_photos_api.egg-info/top_level.txt
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 10:34:07.912863 flickr_photos_api-2.0.0/tests/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     6662 2024-04-30 10:34:01.000000 flickr_photos_api-2.0.0/tests/test_errors.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      472 2024-01-09 14:51:31.000000 flickr_photos_api-2.0.0/tests/test_utils.py
```

### Comparing `flickr-photos-api-1.9.2/LICENSE-APACHE` & `flickr_photos_api-2.0.0/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `flickr-photos-api-1.9.2/LICENSE-MIT` & `flickr_photos_api-2.0.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `flickr-photos-api-1.9.2/PKG-INFO` & `flickr_photos_api-2.0.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flickr-photos-api
-Version: 1.9.2
+Version: 2.0.0
 Summary: Look up information about photos and collections of photos from Flickr
 Author-email: Flickr Foundation <hello@flickr.org>
 Maintainer-email: Alex Chan <alex@flickr.org>
 Project-URL: Homepage, https://github.com/Flickr-Foundation/flickr-photos-api
 Project-URL: Changelog, https://github.com/Flickr-Foundation/flickr-photos-api/blob/main/CHANGELOG.md
 Keywords: flickr
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,77 +18,93 @@
 Requires-Dist: flickr_url_parser>=1.8.0
 Requires-Dist: httpx
 Requires-Dist: silver-nitrate>=1.0.1
 Requires-Dist: tenacity
 
 # flickr-photos-api
 
-This is a library for getting information about photos from the Flickr API.
+This is a library for using the Flickr API at the [Flickr Foundation].
 
-It's not a general-purpose Flickr API library.
-Instead, it focuses on providing information about photos and photo collections.
-It tries to abstract away some of the details of the Flickr API -- for example, licenses are returned as complete dictionaries, rather than as the numeric license IDs returned by Flickr API methods.
+It's *not* a general-purpose Flickr API library.
+It provides a subset of Flickr API methods with the following goals:
 
-Examples:
+*   Provide reusable code that can be called across all our projects.
+*   Abstract away some of the details of the Flickr API -- for example, licenses are returned as complete dictionaries, rather than as the numeric license IDs returned by Flickr API methods.
+*   Apply types to all results, so the Flickr API can be used safely in a typed context.
+
+[Flickr Foundation]: https://www.flickr.org/
+
+## Design
+
+Using the Flickr API is fairly simple: you make an HTTP GET to `https://api.flickr.com/services/rest/?api_key={api_key}` and pass one or more URL query parameters.
+One of those query parameters must be `method`, then you add other parameters depending on the API method.
+
+There's an abstract class that represents this interface:
+
+```python
+import abc
+from xml.etree import ElementTree as ET
+
+
+class FlickrApi(abc.ABC):
+    @abc.abstractmethod
+    def call(self, method: str, params: dict[str, str] | None = None) -> ET.Element:
+        return NotImplemented
+```
+
+The idea is that you can extend this class with "method" classes that wrap specific API methods, and make HTTP GET calls through this `call()` method:
+
+```python
+class GetSinglePhotoMethods(FlickrApi):
+    def get_single_photo(self, photo_id: str) -> ET.Element:
+        return self.call(method="flickr.photos.getInfo", params={"photo_id": photo_id})
+```
+
+This separates the code for making HTTP requests and separating the responses.
+
+The library includes a single implementation of `FlickrApi` for making HTTP requests, using `httpx`, but you could swap it out if you wanted to use e.g. `requests` or `urllib3`.
+This httpx implementation is the default implementation.
+
+## Examples
 
 ```console
->>> from flickr_photos_api import FlickrPhotosApi
->>> api = FlickrPhotosApi(api_key="…", user_agent="…")
+>>> from flickr_photos_api import FlickrApi
+>>> api = FlickrApi(api_key="…", user_agent="…")
 
 >>> photo = api.get_single_photo(photo_id="14898030836")
 
 >>> photo
 {'id': '14898030836', 'title': 'NASA Scientists Says', …}
 
 >>> photo["license"]
 {'id': 'cc-by-2.0', 'label': 'CC BY 2.0', 'url': 'https://creativecommons.org/licenses/by/2.0/'}
 
 >>> photo["url"]
 'https://www.flickr.com/photos/lassennps/14898030836/'
 ```
 
-This library was created for use in [Flinumeratr], [Flickypedia], and other [Flickr Foundation] projects.
-
-[Flinumeratr]: https://github.com/Flickr-Foundation/flinumeratr
-[Flickypedia]: https://commons.wikimedia.org/wiki/Commons:Flickypedia
-[Flickr Foundation]: https://www.flickr.org/
-
 ## Usage
 
 1.  Install flickr-photos-api from PyPI:
 
     ```console
     $ pip install flickr-photos-api
     ```
 
-2.  Construct an instance of `FlickrPhotosApi`.
+2.  Construct an instance of `FlickrApi`.
     You need to pass a user-agent that identifies you, and a [Flickr API key][key].
 
     ```python
-    from flickr_photos_api import FlickrPhotosApi
+    from flickr_photos_api import FlickrApi
 
-    api = FlickrPhotosApi(api_key="…", user_agent="…")
+    api = FlickrApi(api_key="…", user_agent="…")
     ```
 
-3.  Call methods on FlickrPhotosApi.
-    The methods meant for public use are:
-
-    ```python
-    def get_single_photo(photo_id: str) -> SinglePhoto: ...
-
-    def get_photos_in_album(user_url: str, album_id: str) -> PhotosInAlbum: ...
-
-    def get_photos_in_gallery(gallery_id: str) -> PhotosInGallery: ...
-
-    def get_public_photos_by_user(user_url: str) -> CollectionOfPhotos: ...
-
-    def get_photos_in_group_pool(group_url: str) -> PhotosInGroup: ...
-
-    def get_photos_with_tag(tag: str) -> CollectionOfPhotos: ...
-    ```
+3.  Call methods on FlickrApi.
+    There's no complete list of methods right now; look at the files `X_methods.py` in the `api` directory.
 
     Methods that return collections of photos also support `page` and `per_page` parameters to control pagination.
 
 [key]: https://www.flickr.com/services/api/misc.api_keys.html
 
 ## Development
```

### Comparing `flickr-photos-api-1.9.2/README.md` & `flickr_photos_api-2.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,72 +1,88 @@
 # flickr-photos-api
 
-This is a library for getting information about photos from the Flickr API.
+This is a library for using the Flickr API at the [Flickr Foundation].
 
-It's not a general-purpose Flickr API library.
-Instead, it focuses on providing information about photos and photo collections.
-It tries to abstract away some of the details of the Flickr API -- for example, licenses are returned as complete dictionaries, rather than as the numeric license IDs returned by Flickr API methods.
+It's *not* a general-purpose Flickr API library.
+It provides a subset of Flickr API methods with the following goals:
 
-Examples:
+*   Provide reusable code that can be called across all our projects.
+*   Abstract away some of the details of the Flickr API -- for example, licenses are returned as complete dictionaries, rather than as the numeric license IDs returned by Flickr API methods.
+*   Apply types to all results, so the Flickr API can be used safely in a typed context.
+
+[Flickr Foundation]: https://www.flickr.org/
+
+## Design
+
+Using the Flickr API is fairly simple: you make an HTTP GET to `https://api.flickr.com/services/rest/?api_key={api_key}` and pass one or more URL query parameters.
+One of those query parameters must be `method`, then you add other parameters depending on the API method.
+
+There's an abstract class that represents this interface:
+
+```python
+import abc
+from xml.etree import ElementTree as ET
+
+
+class FlickrApi(abc.ABC):
+    @abc.abstractmethod
+    def call(self, method: str, params: dict[str, str] | None = None) -> ET.Element:
+        return NotImplemented
+```
+
+The idea is that you can extend this class with "method" classes that wrap specific API methods, and make HTTP GET calls through this `call()` method:
+
+```python
+class GetSinglePhotoMethods(FlickrApi):
+    def get_single_photo(self, photo_id: str) -> ET.Element:
+        return self.call(method="flickr.photos.getInfo", params={"photo_id": photo_id})
+```
+
+This separates the code for making HTTP requests and separating the responses.
+
+The library includes a single implementation of `FlickrApi` for making HTTP requests, using `httpx`, but you could swap it out if you wanted to use e.g. `requests` or `urllib3`.
+This httpx implementation is the default implementation.
+
+## Examples
 
 ```console
->>> from flickr_photos_api import FlickrPhotosApi
->>> api = FlickrPhotosApi(api_key="…", user_agent="…")
+>>> from flickr_photos_api import FlickrApi
+>>> api = FlickrApi(api_key="…", user_agent="…")
 
 >>> photo = api.get_single_photo(photo_id="14898030836")
 
 >>> photo
 {'id': '14898030836', 'title': 'NASA Scientists Says', …}
 
 >>> photo["license"]
 {'id': 'cc-by-2.0', 'label': 'CC BY 2.0', 'url': 'https://creativecommons.org/licenses/by/2.0/'}
 
 >>> photo["url"]
 'https://www.flickr.com/photos/lassennps/14898030836/'
 ```
 
-This library was created for use in [Flinumeratr], [Flickypedia], and other [Flickr Foundation] projects.
-
-[Flinumeratr]: https://github.com/Flickr-Foundation/flinumeratr
-[Flickypedia]: https://commons.wikimedia.org/wiki/Commons:Flickypedia
-[Flickr Foundation]: https://www.flickr.org/
-
 ## Usage
 
 1.  Install flickr-photos-api from PyPI:
 
     ```console
     $ pip install flickr-photos-api
     ```
 
-2.  Construct an instance of `FlickrPhotosApi`.
+2.  Construct an instance of `FlickrApi`.
     You need to pass a user-agent that identifies you, and a [Flickr API key][key].
 
     ```python
-    from flickr_photos_api import FlickrPhotosApi
+    from flickr_photos_api import FlickrApi
 
-    api = FlickrPhotosApi(api_key="…", user_agent="…")
+    api = FlickrApi(api_key="…", user_agent="…")
     ```
 
-3.  Call methods on FlickrPhotosApi.
-    The methods meant for public use are:
-
-    ```python
-    def get_single_photo(photo_id: str) -> SinglePhoto: ...
-
-    def get_photos_in_album(user_url: str, album_id: str) -> PhotosInAlbum: ...
-
-    def get_photos_in_gallery(gallery_id: str) -> PhotosInGallery: ...
-
-    def get_public_photos_by_user(user_url: str) -> CollectionOfPhotos: ...
-
-    def get_photos_in_group_pool(group_url: str) -> PhotosInGroup: ...
-
-    def get_photos_with_tag(tag: str) -> CollectionOfPhotos: ...
-    ```
+3.  Call methods on FlickrApi.
+    There's no complete list of methods right now; look at the files `X_methods.py` in the `api` directory.
 
     Methods that return collections of photos also support `page` and `per_page` parameters to control pagination.
 
 [key]: https://www.flickr.com/services/api/misc.api_keys.html
 
 ## Development
```

### Comparing `flickr-photos-api-1.9.2/pyproject.toml` & `flickr_photos_api-2.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -50,14 +50,17 @@
   "tests",
 ]
 
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 fail_under = 100
+exclude_also = [
+  "return NotImplemented",
+]
 
 [tool.pytest.ini_options]
 filterwarnings = [
   "error",
 ]
 
 [tool.mypy]
```

### Comparing `flickr-photos-api-1.9.2/src/flickr_photos_api/__init__.py` & `flickr_photos_api-2.0.0/src/flickr_photos_api/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from .api import FlickrPhotosApi
+from .api import FlickrApi
 from .exceptions import (
     FlickrApiException,
     InvalidApiKey,
     InvalidXmlException,
     ResourceNotFound,
     LicenseNotFound,
 )
 from .types import (
+    Comment,
     License,
     User,
     UserInfo,
     TakenGranularity,
     DateTaken,
     LocationInfo,
     Size,
@@ -20,36 +21,39 @@
     PhotosFromUrl,
     PhotosInAlbum,
     PhotosInGallery,
     PhotosInGroup,
     AlbumInfo,
     GalleryInfo,
     GroupInfo,
+    SinglePhotoInfo,
 )
 
 
-__version__ = "1.9.2"
+__version__ = "2.0.0"
 
 
 __all__ = [
-    "FlickrPhotosApi",
+    "FlickrApi",
     "FlickrApiException",
     "ResourceNotFound",
     "InvalidApiKey",
     "InvalidXmlException",
     "LicenseNotFound",
     "License",
     "LocationInfo",
     "User",
     "UserInfo",
     "TakenGranularity",
+    "Comment",
     "DateTaken",
     "Size",
     "SafetyLevel",
     "SinglePhoto",
+    "SinglePhotoInfo",
     "CollectionOfPhotos",
     "PhotosFromUrl",
     "PhotosInAlbum",
     "PhotosInGallery",
     "PhotosInGroup",
     "AlbumInfo",
     "GalleryInfo",
```

### Comparing `flickr-photos-api-1.9.2/src/flickr_photos_api/exceptions.py` & `flickr_photos_api-2.0.0/src/flickr_photos_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `flickr-photos-api-1.9.2/src/flickr_photos_api/utils.py` & `flickr_photos_api-2.0.0/src/flickr_photos_api/utils.py`

 * *Files identical despite different names*

### Comparing `flickr-photos-api-1.9.2/src/flickr_photos_api.egg-info/PKG-INFO` & `flickr_photos_api-2.0.0/src/flickr_photos_api.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flickr-photos-api
-Version: 1.9.2
+Version: 2.0.0
 Summary: Look up information about photos and collections of photos from Flickr
 Author-email: Flickr Foundation <hello@flickr.org>
 Maintainer-email: Alex Chan <alex@flickr.org>
 Project-URL: Homepage, https://github.com/Flickr-Foundation/flickr-photos-api
 Project-URL: Changelog, https://github.com/Flickr-Foundation/flickr-photos-api/blob/main/CHANGELOG.md
 Keywords: flickr
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,77 +18,93 @@
 Requires-Dist: flickr_url_parser>=1.8.0
 Requires-Dist: httpx
 Requires-Dist: silver-nitrate>=1.0.1
 Requires-Dist: tenacity
 
 # flickr-photos-api
 
-This is a library for getting information about photos from the Flickr API.
+This is a library for using the Flickr API at the [Flickr Foundation].
 
-It's not a general-purpose Flickr API library.
-Instead, it focuses on providing information about photos and photo collections.
-It tries to abstract away some of the details of the Flickr API -- for example, licenses are returned as complete dictionaries, rather than as the numeric license IDs returned by Flickr API methods.
+It's *not* a general-purpose Flickr API library.
+It provides a subset of Flickr API methods with the following goals:
 
-Examples:
+*   Provide reusable code that can be called across all our projects.
+*   Abstract away some of the details of the Flickr API -- for example, licenses are returned as complete dictionaries, rather than as the numeric license IDs returned by Flickr API methods.
+*   Apply types to all results, so the Flickr API can be used safely in a typed context.
+
+[Flickr Foundation]: https://www.flickr.org/
+
+## Design
+
+Using the Flickr API is fairly simple: you make an HTTP GET to `https://api.flickr.com/services/rest/?api_key={api_key}` and pass one or more URL query parameters.
+One of those query parameters must be `method`, then you add other parameters depending on the API method.
+
+There's an abstract class that represents this interface:
+
+```python
+import abc
+from xml.etree import ElementTree as ET
+
+
+class FlickrApi(abc.ABC):
+    @abc.abstractmethod
+    def call(self, method: str, params: dict[str, str] | None = None) -> ET.Element:
+        return NotImplemented
+```
+
+The idea is that you can extend this class with "method" classes that wrap specific API methods, and make HTTP GET calls through this `call()` method:
+
+```python
+class GetSinglePhotoMethods(FlickrApi):
+    def get_single_photo(self, photo_id: str) -> ET.Element:
+        return self.call(method="flickr.photos.getInfo", params={"photo_id": photo_id})
+```
+
+This separates the code for making HTTP requests and separating the responses.
+
+The library includes a single implementation of `FlickrApi` for making HTTP requests, using `httpx`, but you could swap it out if you wanted to use e.g. `requests` or `urllib3`.
+This httpx implementation is the default implementation.
+
+## Examples
 
 ```console
->>> from flickr_photos_api import FlickrPhotosApi
->>> api = FlickrPhotosApi(api_key="…", user_agent="…")
+>>> from flickr_photos_api import FlickrApi
+>>> api = FlickrApi(api_key="…", user_agent="…")
 
 >>> photo = api.get_single_photo(photo_id="14898030836")
 
 >>> photo
 {'id': '14898030836', 'title': 'NASA Scientists Says', …}
 
 >>> photo["license"]
 {'id': 'cc-by-2.0', 'label': 'CC BY 2.0', 'url': 'https://creativecommons.org/licenses/by/2.0/'}
 
 >>> photo["url"]
 'https://www.flickr.com/photos/lassennps/14898030836/'
 ```
 
-This library was created for use in [Flinumeratr], [Flickypedia], and other [Flickr Foundation] projects.
-
-[Flinumeratr]: https://github.com/Flickr-Foundation/flinumeratr
-[Flickypedia]: https://commons.wikimedia.org/wiki/Commons:Flickypedia
-[Flickr Foundation]: https://www.flickr.org/
-
 ## Usage
 
 1.  Install flickr-photos-api from PyPI:
 
     ```console
     $ pip install flickr-photos-api
     ```
 
-2.  Construct an instance of `FlickrPhotosApi`.
+2.  Construct an instance of `FlickrApi`.
     You need to pass a user-agent that identifies you, and a [Flickr API key][key].
 
     ```python
-    from flickr_photos_api import FlickrPhotosApi
+    from flickr_photos_api import FlickrApi
 
-    api = FlickrPhotosApi(api_key="…", user_agent="…")
+    api = FlickrApi(api_key="…", user_agent="…")
     ```
 
-3.  Call methods on FlickrPhotosApi.
-    The methods meant for public use are:
-
-    ```python
-    def get_single_photo(photo_id: str) -> SinglePhoto: ...
-
-    def get_photos_in_album(user_url: str, album_id: str) -> PhotosInAlbum: ...
-
-    def get_photos_in_gallery(gallery_id: str) -> PhotosInGallery: ...
-
-    def get_public_photos_by_user(user_url: str) -> CollectionOfPhotos: ...
-
-    def get_photos_in_group_pool(group_url: str) -> PhotosInGroup: ...
-
-    def get_photos_with_tag(tag: str) -> CollectionOfPhotos: ...
-    ```
+3.  Call methods on FlickrApi.
+    There's no complete list of methods right now; look at the files `X_methods.py` in the `api` directory.
 
     Methods that return collections of photos also support `page` and `per_page` parameters to control pagination.
 
 [key]: https://www.flickr.com/services/api/misc.api_keys.html
 
 ## Development
```

### Comparing `flickr-photos-api-1.9.2/src/flickr_photos_api.egg-info/SOURCES.txt` & `flickr_photos_api-2.0.0/src/flickr_photos_api.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 LICENSE-APACHE
 LICENSE-MIT
 README.md
 pyproject.toml
 src/flickr_photos_api/__init__.py
-src/flickr_photos_api/api.py
 src/flickr_photos_api/exceptions.py
 src/flickr_photos_api/py.typed
 src/flickr_photos_api/types.py
 src/flickr_photos_api/utils.py
 src/flickr_photos_api.egg-info/PKG-INFO
 src/flickr_photos_api.egg-info/SOURCES.txt
 src/flickr_photos_api.egg-info/dependency_links.txt
 src/flickr_photos_api.egg-info/requires.txt
 src/flickr_photos_api.egg-info/top_level.txt
-tests/test_api.py
+src/flickr_photos_api/api/__init__.py
+src/flickr_photos_api/api/base.py
+src/flickr_photos_api/api/collection_methods.py
+src/flickr_photos_api/api/comment_methods.py
+src/flickr_photos_api/api/from_url_methods.py
+src/flickr_photos_api/api/license_methods.py
+src/flickr_photos_api/api/single_photo_methods.py
+src/flickr_photos_api/api/user_methods.py
 tests/test_errors.py
 tests/test_utils.py
```

### Comparing `flickr-photos-api-1.9.2/tests/test_errors.py` & `flickr_photos_api-2.0.0/tests/test_errors.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import httpx
 import pytest
 
 from flickr_photos_api import (
-    FlickrPhotosApi,
+    FlickrApi as FlickrPhotosApi,
     FlickrApiException,
     InvalidApiKey,
     InvalidXmlException,
     ResourceNotFound,
 )
 
 
@@ -27,35 +27,35 @@
             "get_single_photo",
             {"photo_id": "12345678901234567890"},
             id="get_single_photo",
         ),
         pytest.param(
             "get_photos_in_album",
             {
-                "user_url": "https://www.flickr.com/photos/DefinitelyDoesNotExist",
+                "user_id": "-1",
                 "album_id": "1234",
             },
             id="get_photos_in_album_with_missing_user",
         ),
         pytest.param(
             "get_photos_in_album",
             {
-                "user_url": "https://www.flickr.com/photos/britishlibrary/",
+                "user_id": "12403504@N02",
                 "album_id": "12345678901234567890",
             },
             id="get_photos_in_album_with_missing_album",
         ),
         pytest.param(
             "get_photos_in_gallery",
             {"gallery_id": "12345678901234567890"},
             id="get_photos_in_gallery",
         ),
         pytest.param(
-            "get_public_photos_by_user",
-            {"user_url": "https://www.flickr.com/photos/DefinitelyDoesNotExist"},
+            "get_photos_in_user_photostream",
+            {"user_id": "-1"},
             id="get_public_photos_by_non_existent_user",
         ),
         pytest.param(
             "get_photos_in_group_pool",
             {"group_url": "https://www.flickr.com/groups/doesnotexist/pool/"},
             id="get_photos_in_non_existent_group_pool",
         ),
@@ -118,84 +118,70 @@
             if self.get_request_count == 1:
                 raise httpx.ReadTimeout("The read operation timed out")
             else:
                 return self.underlying.get(url=url, params=params, timeout=timeout)
 
     api.client = FlakyClient(underlying=api.client)  # type: ignore
 
-    resp = api.get_public_photos_by_user(
-        user_url="https://www.flickr.com/photos/navymedicine/"
-    )
+    resp = api.get_photos_in_user_photostream(user_id="61270229@N05")
 
     assert len(resp["photos"]) == 10
 
 
 def test_retries_5xx_error(api: FlickrPhotosApi) -> None:
     # The cassette for this test was constructed manually: I edited
     # an existing cassette to add a 500 response as the first response,
     # then we want to see it make a second request to retry it.
-    resp = api.get_public_photos_by_user(
-        user_url="https://www.flickr.com/photos/navymedicine/"
-    )
+    resp = api.get_photos_in_user_photostream(user_id="61270229@N05")
 
     assert len(resp["photos"]) == 10
 
 
 def test_a_persistent_5xx_error_is_raised(api: FlickrPhotosApi) -> None:
     # The cassette for this test was constructed manually: I copy/pasted
     # the 500 response from the previous test so that there were more
     # than it would retry.
     with pytest.raises(httpx.HTTPStatusError) as err:
-        api.get_public_photos_by_user(
-            user_url="https://www.flickr.com/photos/navymedicine/"
-        )
+        api.get_photos_in_user_photostream(user_id="61270229@N05")
 
     assert err.value.response.status_code == 500
 
 
 def test_retries_invalid_xml_error(api: FlickrPhotosApi) -> None:
     # The cassette for this test was constructed manually: I edited
     # an existing cassette to add the invalid XML as the first response,
     # then we want to see it make a second request to retry it.
-    resp = api.get_public_photos_by_user(
-        user_url="https://www.flickr.com/photos/navymedicine/"
-    )
+    resp = api.get_photos_in_user_photostream(user_id="61270229@N05")
 
     assert len(resp["photos"]) == 10
 
 
 def test_a_persistent_invalid_xml_error_is_raised(api: FlickrPhotosApi) -> None:
     # The cassette for this test was constructed manually: I copy/pasted
     # the invalid XML from the previous test so that there were more
     # than it would retry.
     with pytest.raises(InvalidXmlException):
-        api.get_public_photos_by_user(
-            user_url="https://www.flickr.com/photos/navymedicine/"
-        )
+        api.get_photos_in_user_photostream(user_id="61270229@N05")
 
 
 def test_retries_error_code_201(api: FlickrPhotosApi) -> None:
     # The cassette for this test was constructed manually: I edited
     # an existing cassette to add the invalid XML as the first response,
     # then we want to see it make a second request to retry it.
-    resp = api.get_public_photos_by_user(
-        user_url="https://www.flickr.com/photos/navymedicine/"
-    )
+    resp = api.get_photos_in_user_photostream(user_id="61270229@N05")
 
     assert len(resp["photos"]) == 10
 
 
 def test_a_persistent_error_201_is_raised(api: FlickrPhotosApi) -> None:
     # The cassette for this test was constructed manually: I edited
     # an existing cassette to add the invalid XML as the first response,
     # then we want to see it make a second request to retry it.
     with pytest.raises(FlickrApiException) as exc:
-        api.get_public_photos_by_user(
-            user_url="https://www.flickr.com/photos/navymedicine/"
-        )
+        api.get_photos_in_user_photostream(user_id="61270229@N05")
 
     assert exc.value.args[0] == {
         "code": "201",
         "msg": "Sorry, the Flickr API service is not currently available.",
     }
```

