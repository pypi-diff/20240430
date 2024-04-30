# Comparing `tmp/flickr-url-parser-1.8.2.tar.gz` & `tmp/flickr_url_parser-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flickr-url-parser-1.8.2.tar", last modified: Fri Feb  2 13:54:39 2024, max compression
+gzip compressed data, was "flickr_url_parser-1.8.3.tar", last modified: Tue Apr 30 14:43:35 2024, max compression
```

## Comparing `flickr-url-parser-1.8.2.tar` & `flickr_url_parser-1.8.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-02-02 13:54:39.222228 flickr-url-parser-1.8.2/
--rw-r--r--   0 alexwlchan   (501) staff       (20)    11356 2023-10-03 13:54:10.000000 flickr-url-parser-1.8.2/LICENSE-APACHE
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1074 2023-10-03 13:54:10.000000 flickr-url-parser-1.8.2/LICENSE-MIT
--rw-r--r--   0 alexwlchan   (501) staff       (20)     3835 2024-02-02 13:54:39.222046 flickr-url-parser-1.8.2/PKG-INFO
--rw-r--r--   0 alexwlchan   (501) staff       (20)     2991 2023-12-18 15:24:26.000000 flickr-url-parser-1.8.2/README.md
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1890 2023-12-18 15:19:07.000000 flickr-url-parser-1.8.2/pyproject.toml
--rw-r--r--   0 alexwlchan   (501) staff       (20)       38 2024-02-02 13:54:39.222265 flickr-url-parser-1.8.2/setup.cfg
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-02-02 13:54:39.217173 flickr-url-parser-1.8.2/src/
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-02-02 13:54:39.220066 flickr-url-parser-1.8.2/src/flickr_url_parser/
--rw-r--r--   0 alexwlchan   (501) staff       (20)      371 2024-02-02 13:42:13.000000 flickr-url-parser-1.8.2/src/flickr_url_parser/__init__.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)      878 2023-10-31 12:00:36.000000 flickr-url-parser-1.8.2/src/flickr_url_parser/base58.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)      649 2023-12-18 15:19:07.000000 flickr-url-parser-1.8.2/src/flickr_url_parser/cli.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)      309 2023-12-18 15:19:07.000000 flickr-url-parser-1.8.2/src/flickr_url_parser/exceptions.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)      481 2023-12-12 14:58:59.000000 flickr-url-parser-1.8.2/src/flickr_url_parser/matcher.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)    16782 2024-02-02 13:42:05.000000 flickr-url-parser-1.8.2/src/flickr_url_parser/parser.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)       93 2023-11-05 09:20:42.000000 flickr-url-parser-1.8.2/src/flickr_url_parser/py.typed
--rw-r--r--   0 alexwlchan   (501) staff       (20)      722 2023-12-27 13:29:56.000000 flickr-url-parser-1.8.2/src/flickr_url_parser/types.py
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-02-02 13:54:39.221847 flickr-url-parser-1.8.2/src/flickr_url_parser.egg-info/
--rw-r--r--   0 alexwlchan   (501) staff       (20)     3835 2024-02-02 13:54:39.000000 flickr-url-parser-1.8.2/src/flickr_url_parser.egg-info/PKG-INFO
--rw-r--r--   0 alexwlchan   (501) staff       (20)      653 2024-02-02 13:54:39.000000 flickr-url-parser-1.8.2/src/flickr_url_parser.egg-info/SOURCES.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)        1 2024-02-02 13:54:39.000000 flickr-url-parser-1.8.2/src/flickr_url_parser.egg-info/dependency_links.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)       65 2024-02-02 13:54:39.000000 flickr-url-parser-1.8.2/src/flickr_url_parser.egg-info/entry_points.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)       16 2024-02-02 13:54:39.000000 flickr-url-parser-1.8.2/src/flickr_url_parser.egg-info/requires.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)       18 2024-02-02 13:54:39.000000 flickr-url-parser-1.8.2/src/flickr_url_parser.egg-info/top_level.txt
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-02-02 13:54:39.221570 flickr-url-parser-1.8.2/tests/
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1323 2023-12-18 15:15:45.000000 flickr-url-parser-1.8.2/tests/test_cli.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)    16849 2024-02-02 13:41:54.000000 flickr-url-parser-1.8.2/tests/test_flickr_url_parser.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1786 2023-12-12 14:58:59.000000 flickr-url-parser-1.8.2/tests/test_matcher.py
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 14:43:35.813903 flickr_url_parser-1.8.3/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)    11356 2023-10-03 13:54:10.000000 flickr_url_parser-1.8.3/LICENSE-APACHE
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1074 2023-10-03 13:54:10.000000 flickr_url_parser-1.8.3/LICENSE-MIT
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     3835 2024-04-30 14:43:35.813669 flickr_url_parser-1.8.3/PKG-INFO
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     2991 2023-12-18 15:24:26.000000 flickr_url_parser-1.8.3/README.md
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1890 2023-12-18 15:19:07.000000 flickr_url_parser-1.8.3/pyproject.toml
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       38 2024-04-30 14:43:35.813953 flickr_url_parser-1.8.3/setup.cfg
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 14:43:35.808774 flickr_url_parser-1.8.3/src/
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 14:43:35.811503 flickr_url_parser-1.8.3/src/flickr_url_parser/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      371 2024-04-30 14:43:31.000000 flickr_url_parser-1.8.3/src/flickr_url_parser/__init__.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      878 2023-10-31 12:00:36.000000 flickr_url_parser-1.8.3/src/flickr_url_parser/base58.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      649 2023-12-18 15:19:07.000000 flickr_url_parser-1.8.3/src/flickr_url_parser/cli.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      309 2023-12-18 15:19:07.000000 flickr_url_parser-1.8.3/src/flickr_url_parser/exceptions.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      481 2023-12-12 14:58:59.000000 flickr_url_parser-1.8.3/src/flickr_url_parser/matcher.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)    16783 2024-04-30 14:43:31.000000 flickr_url_parser-1.8.3/src/flickr_url_parser/parser.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       93 2023-11-05 09:20:42.000000 flickr_url_parser-1.8.3/src/flickr_url_parser/py.typed
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      796 2024-04-30 09:55:09.000000 flickr_url_parser-1.8.3/src/flickr_url_parser/types.py
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 14:43:35.813381 flickr_url_parser-1.8.3/src/flickr_url_parser.egg-info/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     3835 2024-04-30 14:43:35.000000 flickr_url_parser-1.8.3/src/flickr_url_parser.egg-info/PKG-INFO
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      653 2024-04-30 14:43:35.000000 flickr_url_parser-1.8.3/src/flickr_url_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)        1 2024-04-30 14:43:35.000000 flickr_url_parser-1.8.3/src/flickr_url_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       65 2024-04-30 14:43:35.000000 flickr_url_parser-1.8.3/src/flickr_url_parser.egg-info/entry_points.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       16 2024-04-30 14:43:35.000000 flickr_url_parser-1.8.3/src/flickr_url_parser.egg-info/requires.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       18 2024-04-30 14:43:35.000000 flickr_url_parser-1.8.3/src/flickr_url_parser.egg-info/top_level.txt
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 14:43:35.813056 flickr_url_parser-1.8.3/tests/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1323 2023-12-18 15:15:45.000000 flickr_url_parser-1.8.3/tests/test_cli.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)    16854 2024-04-30 14:43:31.000000 flickr_url_parser-1.8.3/tests/test_flickr_url_parser.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1786 2023-12-12 14:58:59.000000 flickr_url_parser-1.8.3/tests/test_matcher.py
```

### Comparing `flickr-url-parser-1.8.2/LICENSE-APACHE` & `flickr_url_parser-1.8.3/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `flickr-url-parser-1.8.2/LICENSE-MIT` & `flickr_url_parser-1.8.3/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `flickr-url-parser-1.8.2/PKG-INFO` & `flickr_url_parser-1.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flickr-url-parser
-Version: 1.8.2
+Version: 1.8.3
 Summary: Enter a Flickr URL, and find out what sort of URL it is (single photo, album, gallery, etc.)
 Author-email: Flickr Foundation <hello@flickr.org>
 Maintainer-email: Alex Chan <alex@flickr.org>
 Project-URL: Homepage, https://github.com/Flickr-Foundation/flickr-url-parser
 Project-URL: Changelog, https://github.com/Flickr-Foundation/flickr-url-parser/blob/main/CHANGELOG.md
 Keywords: flickr
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `flickr-url-parser-1.8.2/README.md` & `flickr_url_parser-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `flickr-url-parser-1.8.2/pyproject.toml` & `flickr_url_parser-1.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flickr-url-parser-1.8.2/src/flickr_url_parser/base58.py` & `flickr_url_parser-1.8.3/src/flickr_url_parser/base58.py`

 * *Files identical despite different names*

### Comparing `flickr-url-parser-1.8.2/src/flickr_url_parser/cli.py` & `flickr_url_parser-1.8.3/src/flickr_url_parser/cli.py`

 * *Files identical despite different names*

### Comparing `flickr-url-parser-1.8.2/src/flickr_url_parser/parser.py` & `flickr_url_parser-1.8.3/src/flickr_url_parser/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -392,15 +392,15 @@
         and 4 <= len(u.path) <= 5
         and u.path[0] == "photos"
         and u.path[2] in {"albums", "sets"}
         and is_digits(u.path[3])
     ):
         return {
             "type": "album",
-            "user_url": f"https://www.flickr.com/photos/{u.path[1]}",
+            "user_url": f"https://www.flickr.com/photos/{u.path[1]}/",
             "album_id": u.path[3],
             "page": get_page(u),
         }
 
     # The URL for a user, e.g.
     #
     #     https://www.flickr.com/photos/blueminds/
```

### Comparing `flickr-url-parser-1.8.2/src/flickr_url_parser/types.py` & `flickr_url_parser-1.8.3/src/flickr_url_parser/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from typing import Literal, TypedDict
+import typing
 
 
-class Homepage(TypedDict):
-    type: Literal["homepage"]
+class Homepage(typing.TypedDict):
+    type: typing.Literal["homepage"]
 
 
-class SinglePhoto(TypedDict):
-    type: Literal["single_photo"]
+class SinglePhoto(typing.TypedDict):
+    type: typing.Literal["single_photo"]
     photo_id: str
 
 
-class Album(TypedDict):
-    type: Literal["album"]
+class Album(typing.TypedDict):
+    type: typing.Literal["album"]
     user_url: str
     album_id: str
     page: int
 
 
-class User(TypedDict):
-    type: Literal["user"]
+class User(typing.TypedDict):
+    type: typing.Literal["user"]
     page: int
     user_url: str
     user_id: str | None
 
 
-class Group(TypedDict):
-    type: Literal["group"]
+class Group(typing.TypedDict):
+    type: typing.Literal["group"]
     group_url: str
     page: int
 
 
-class Gallery(TypedDict):
-    type: Literal["gallery"]
+class Gallery(typing.TypedDict):
+    type: typing.Literal["gallery"]
     gallery_id: str
     page: int
 
 
-class Tag(TypedDict):
-    type: Literal["tag"]
+class Tag(typing.TypedDict):
+    type: typing.Literal["tag"]
     tag: str
     page: int
 
 
 ParseResult = Homepage | SinglePhoto | Album | User | Group | Gallery | Tag
```

### Comparing `flickr-url-parser-1.8.2/src/flickr_url_parser.egg-info/PKG-INFO` & `flickr_url_parser-1.8.3/src/flickr_url_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flickr-url-parser
-Version: 1.8.2
+Version: 1.8.3
 Summary: Enter a Flickr URL, and find out what sort of URL it is (single photo, album, gallery, etc.)
 Author-email: Flickr Foundation <hello@flickr.org>
 Maintainer-email: Alex Chan <alex@flickr.org>
 Project-URL: Homepage, https://github.com/Flickr-Foundation/flickr-url-parser
 Project-URL: Changelog, https://github.com/Flickr-Foundation/flickr-url-parser/blob/main/CHANGELOG.md
 Keywords: flickr
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `flickr-url-parser-1.8.2/src/flickr_url_parser.egg-info/SOURCES.txt` & `flickr_url_parser-1.8.3/src/flickr_url_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flickr-url-parser-1.8.2/tests/test_cli.py` & `flickr_url_parser-1.8.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `flickr-url-parser-1.8.2/tests/test_flickr_url_parser.py` & `flickr_url_parser-1.8.3/tests/test_flickr_url_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,33 +201,33 @@
 @pytest.mark.parametrize(
     ["url", "album"],
     [
         (
             "https://www.flickr.com/photos/cat_tac/albums/72157666833379009",
             {
                 "type": "album",
-                "user_url": "https://www.flickr.com/photos/cat_tac",
+                "user_url": "https://www.flickr.com/photos/cat_tac/",
                 "album_id": "72157666833379009",
                 "page": 1,
             },
         ),
         (
             "https://www.flickr.com/photos/cat_tac/sets/72157666833379009",
             {
                 "type": "album",
-                "user_url": "https://www.flickr.com/photos/cat_tac",
+                "user_url": "https://www.flickr.com/photos/cat_tac/",
                 "album_id": "72157666833379009",
                 "page": 1,
             },
         ),
         (
             "https://www.flickr.com/photos/andygocher/albums/72157648252420622/page3",
             {
                 "type": "album",
-                "user_url": "https://www.flickr.com/photos/andygocher",
+                "user_url": "https://www.flickr.com/photos/andygocher/",
                 "album_id": "72157648252420622",
                 "page": 3,
             },
         ),
     ],
 )
 def test_it_parses_an_album(url: str, album: Album) -> None:
@@ -240,15 +240,15 @@
         pytest.param("http://flic.kr/s/aHsjybZ5ZD", id="http-aHsjybZ5ZD"),
         pytest.param("https://flic.kr/s/aHsjybZ5ZD", id="https-aHsjybZ5ZD"),
     ],
 )
 def test_it_parses_a_short_album_url(vcr_cassette: str, url: str) -> None:
     assert parse_flickr_url(url) == {
         "type": "album",
-        "user_url": "https://www.flickr.com/photos/64527945@N07",
+        "user_url": "https://www.flickr.com/photos/64527945@N07/",
         "album_id": "72157628959784871",
         "page": 1,
     }
 
 
 @pytest.mark.parametrize(
     "url",
@@ -451,15 +451,15 @@
     ["url", "expected"],
     [
         # from https://twitter.com/PAPhotoMatt/status/1715111983974940683
         pytest.param(
             "https://www.flickr.com/gp/realphotomatt/M195SLkj98",
             {
                 "type": "album",
-                "user_url": "https://www.flickr.com/photos/realphotomatt",
+                "user_url": "https://www.flickr.com/photos/realphotomatt/",
                 "album_id": "72177720312002426",
                 "page": 1,
             },
             id="M195SLkj98",
         ),
         # one of mine (Alex's)
         pytest.param(
```

### Comparing `flickr-url-parser-1.8.2/tests/test_matcher.py` & `flickr_url_parser-1.8.3/tests/test_matcher.py`

 * *Files identical despite different names*

