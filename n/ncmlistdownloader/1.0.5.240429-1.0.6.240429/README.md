# Comparing `tmp/ncmlistdownloader-1.0.5.240429.tar.gz` & `tmp/ncmlistdownloader-1.0.6.240429.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncmlistdownloader-1.0.5.240429.tar", last modified: Mon Apr 29 10:26:14 2024, max compression
+gzip compressed data, was "ncmlistdownloader-1.0.6.240429.tar", last modified: Mon Apr 29 14:58:32 2024, max compression
```

## Comparing `ncmlistdownloader-1.0.5.240429.tar` & `ncmlistdownloader-1.0.6.240429.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 10:26:14.502622 ncmlistdownloader-1.0.5.240429/
--rw-rw-rw-   0        0        0    35181 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.5.240429/LICENSE
--rw-rw-rw-   0        0        0     1409 2024-04-29 10:26:14.499626 ncmlistdownloader-1.0.5.240429/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-29 10:26:14.449251 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/
--rw-rw-rw-   0        0        0     1425 2024-04-29 10:18:45.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 10:26:14.471713 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/cmd/
--rw-rw-rw-   0        0        0     1789 2024-04-29 10:16:10.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/cmd/__init__.py
--rw-rw-rw-   0        0        0      651 2024-04-29 10:21:56.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/cmd/common.py
--rw-rw-rw-   0        0        0     1685 2024-04-29 10:22:02.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/cmd/download.py
--rw-rw-rw-   0        0        0     2689 2024-04-29 10:22:08.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/cmd/find_from_id.py
--rw-rw-rw-   0        0        0     1664 2024-04-29 10:23:33.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/cmd/json_io.py
-drwxrwxrwx   0        0        0        0 2024-04-29 10:26:14.484507 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/common/
--rw-rw-rw-   0        0        0     2862 2024-04-29 10:21:37.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/common/__init__.py
--rw-rw-rw-   0        0        0     2161 2024-04-29 10:21:11.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/common/encode_sec_key.py
--rw-rw-rw-   0        0        0     2376 2024-04-29 10:20:55.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/common/global_args.py
--rw-rw-rw-   0        0        0     1791 2024-04-29 10:20:35.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/common/thread_test.py
-drwxrwxrwx   0        0        0        0 2024-04-29 10:26:14.486106 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/downloader/
--rw-rw-rw-   0        0        0     6233 2024-04-29 10:20:23.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 10:26:14.488117 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/editer/
--rw-rw-rw-   0        0        0     3965 2024-04-29 10:20:17.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/editer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 10:26:14.490652 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/playlist/
--rw-rw-rw-   0        0        0     2296 2024-04-29 10:19:56.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/playlist/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 10:26:14.495640 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/song/
--rw-rw-rw-   0        0        0     8342 2024-04-29 10:16:56.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader/song/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 10:26:14.497632 ncmlistdownloader-1.0.5.240429/ncmlistdownloader.egg-info/
--rw-rw-rw-   0        0        0     1409 2024-04-29 10:26:14.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      777 2024-04-29 10:26:14.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 10:26:14.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-29 10:26:14.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2024-04-29 10:26:14.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-29 10:26:14.000000 ncmlistdownloader-1.0.5.240429/ncmlistdownloader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 10:26:14.502622 ncmlistdownloader-1.0.5.240429/setup.cfg
--rw-rw-rw-   0        0        0     1923 2024-04-29 10:24:20.000000 ncmlistdownloader-1.0.5.240429/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 14:58:32.879682 ncmlistdownloader-1.0.6.240429/
+-rw-rw-rw-   0        0        0    35181 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.6.240429/LICENSE
+-rw-rw-rw-   0        0        0     1409 2024-04-29 14:58:32.876685 ncmlistdownloader-1.0.6.240429/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-29 14:58:32.823840 ncmlistdownloader-1.0.6.240429/ncmlistdownloader/
+-rw-rw-rw-   0        0        0     1425 2024-04-29 10:18:45.000000 ncmlistdownloader-1.0.6.240429/ncmlistdownloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 14:58:32.849023 ncmlistdownloader-1.0.6.240429/ncmlistdownloader/cmd/
+-rw-rw-rw-   0        0        0     1789 2024-04-29 10:16:10.000000 ncmlistdownloader-1.0.6.240429/ncmlistdownloader/cmd/__init__.py
+-rw-rw-rw-   0        0        0      651 2024-04-29 10:21:56.000000 ncmlistdownloader-1.0.6.240429/ncmlistdownloader/cmd/common.py
+-rw-rw-rw-   0        0        0     1685 2024-04-29 10:22:02.000000 ncmlistdownloader-1.0.6.240429/ncmlistdownloader/cmd/download.py
+-rw-rw-rw-   0        0        0     2689 2024-04-29 10:22:08.000000 ncmlistdownloader-1.0.6.240429/ncmlistdownloader/cmd/find_from_id.py
+-rw-rw-rw-   0        0        0     1664 2024-04-29 10:23:33.000000 ncmlistdownloader-1.0.6.240429/ncmlistdownloader/cmd/json_io.py
+drwxrwxrwx   0        0        0        0 2024-04-29 14:58:32.858669 ncmlistdownloader-1.0.6.240429/ncmlistdownloader/common/
+-rw-rw-rw-   0        0        0     2862 2024-04-29 10:21:37.000000 ncmlistdownloader-1.0.6.240429/ncmlistdownloader/common/__init__.py
+-rw-rw-rw-   0        0        0     2161 2024-04-29 10:21:11.000000 ncmlistdownloader-1.0.6.240429/ncmlistdownloader/common/encode_sec_key.py
+-rw-rw-rw-   0        0        0     2376 2024-04-29 14:57:26.000000 ncmlistdownloader-1.0.6.240429/ncmlistdownloader/common/global_args.py
+-rw-rw-rw-   0        0        0     1791 2024-04-29 10:20:35.000000 ncmlistdownloader-1.0.6.240429/ncmlistdownloader/common/thread_test.py
+drwxrwxrwx   0        0        0        0 2024-04-29 14:58:32.863456 ncmlistdownloader-1.0.6.240429/ncmlistdownloader/downloader/
+-rw-rw-rw-   0        0        0     6233 2024-04-29 10:20:23.000000 ncmlistdownloader-1.0.6.240429/ncmlistdownloader/downloader/__init__.py
+-rw-rw-rw-   0        0        0     1038 2024-04-29 14:55:48.000000 ncmlistdownloader-1.0.6.240429/ncmlistdownloader/downloader/json_list_io.py
+drwxrwxrwx   0        0        0        0 2024-04-29 14:58:32.865475 ncmlistdownloader-1.0.6.240429/ncmlistdownloader/editer/
+-rw-rw-rw-   0        0        0     3965 2024-04-29 10:20:17.000000 ncmlistdownloader-1.0.6.240429/ncmlistdownloader/editer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 14:58:32.869076 ncmlistdownloader-1.0.6.240429/ncmlistdownloader/playlist/
+-rw-rw-rw-   0        0        0     2296 2024-04-29 10:19:56.000000 ncmlistdownloader-1.0.6.240429/ncmlistdownloader/playlist/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 14:58:32.871071 ncmlistdownloader-1.0.6.240429/ncmlistdownloader/song/
+-rw-rw-rw-   0        0        0     9302 2024-04-29 14:55:43.000000 ncmlistdownloader-1.0.6.240429/ncmlistdownloader/song/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 14:58:32.874763 ncmlistdownloader-1.0.6.240429/ncmlistdownloader.egg-info/
+-rw-rw-rw-   0        0        0     1409 2024-04-29 14:58:32.000000 ncmlistdownloader-1.0.6.240429/ncmlistdownloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      822 2024-04-29 14:58:32.000000 ncmlistdownloader-1.0.6.240429/ncmlistdownloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 14:58:32.000000 ncmlistdownloader-1.0.6.240429/ncmlistdownloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-29 14:58:32.000000 ncmlistdownloader-1.0.6.240429/ncmlistdownloader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2024-04-29 14:58:32.000000 ncmlistdownloader-1.0.6.240429/ncmlistdownloader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-29 14:58:32.000000 ncmlistdownloader-1.0.6.240429/ncmlistdownloader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 14:58:32.880674 ncmlistdownloader-1.0.6.240429/setup.cfg
+-rw-rw-rw-   0        0        0     1923 2024-04-29 14:56:39.000000 ncmlistdownloader-1.0.6.240429/setup.py
```

### Comparing `ncmlistdownloader-1.0.5.240429/LICENSE` & `ncmlistdownloader-1.0.6.240429/LICENSE`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.5.240429/PKG-INFO` & `ncmlistdownloader-1.0.6.240429/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.5.240429
+Version: 1.0.6.240429
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `ncmlistdownloader-1.0.5.240429/ncmlistdownloader/__init__.py` & `ncmlistdownloader-1.0.6.240429/ncmlistdownloader/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.5.240429/ncmlistdownloader/cmd/__init__.py` & `ncmlistdownloader-1.0.6.240429/ncmlistdownloader/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.5.240429/ncmlistdownloader/cmd/common.py` & `ncmlistdownloader-1.0.6.240429/ncmlistdownloader/cmd/common.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.5.240429/ncmlistdownloader/cmd/download.py` & `ncmlistdownloader-1.0.6.240429/ncmlistdownloader/cmd/download.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.5.240429/ncmlistdownloader/cmd/find_from_id.py` & `ncmlistdownloader-1.0.6.240429/ncmlistdownloader/cmd/find_from_id.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.5.240429/ncmlistdownloader/cmd/json_io.py` & `ncmlistdownloader-1.0.6.240429/ncmlistdownloader/cmd/json_io.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.5.240429/ncmlistdownloader/common/__init__.py` & `ncmlistdownloader-1.0.6.240429/ncmlistdownloader/common/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.5.240429/ncmlistdownloader/common/encode_sec_key.py` & `ncmlistdownloader-1.0.6.240429/ncmlistdownloader/common/encode_sec_key.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.5.240429/ncmlistdownloader/common/global_args.py` & `ncmlistdownloader-1.0.6.240429/ncmlistdownloader/common/global_args.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 PLAYLIST_API = json_file["PLAYLIST_API"]
 SONG_INFO_API = json_file["SONG_INFO_API"]
 SONG_FILE_API = json_file["SONG_FILE_API"]
 SONG_FILE_API_2 = json_file["SONG_FILE_API_2"]
 SEARCH_API = "https://music.163.com/weapi/cloudsearch/get/web?csrf_token="
 LYRIC_API = json_file["LYRIC_API"]
 CMD_VERSION = "Ver.1.0.4.240427"
-CORE_VERSION_SETUP = "1.0.5.240429"
+CORE_VERSION_SETUP = "1.0.6.240429"
 CORE_VERSION = "Core.Ver." + CORE_VERSION_SETUP
 CMD_START_WORDS = [
     f"163ListDownloader CMD Ver - {CMD_VERSION}",
     "Made by CooooldWind_",
     "Here's the Gitee/GitHub Page, click a star if you like it~",
     "Gitee: https://gitee.com/CooooldWind/163ListDownloader_NexT/issues",
     "GitHub: https://github.com/CooooldWind/163ListDownloader_NexT/issues",
```

### Comparing `ncmlistdownloader-1.0.5.240429/ncmlistdownloader/common/thread_test.py` & `ncmlistdownloader-1.0.6.240429/ncmlistdownloader/common/thread_test.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.5.240429/ncmlistdownloader/downloader/__init__.py` & `ncmlistdownloader-1.0.6.240429/ncmlistdownloader/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.5.240429/ncmlistdownloader/editer/__init__.py` & `ncmlistdownloader-1.0.6.240429/ncmlistdownloader/editer/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.5.240429/ncmlistdownloader/playlist/__init__.py` & `ncmlistdownloader-1.0.6.240429/ncmlistdownloader/playlist/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.5.240429/ncmlistdownloader/song/__init__.py` & `ncmlistdownloader-1.0.6.240429/ncmlistdownloader/song/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ncmlistdownloader/song/__init__.py
-Core.Ver.1.0.5.240429
+Core.Ver.1.0.6.240429
 Author: CooooldWind_
 """
 
 from ncmlistdownloader.common import *
 from ncmlistdownloader.common.encode_sec_key import *
 from ncmlistdownloader.common.thread_test import best_thread
 from ncmlistdownloader.downloader import *
@@ -13,15 +13,15 @@
 from ncmlistdownloader.editer import *
 
 
 class Song:
     """
     Song类
     ----------
-    存储歌曲信息，以及各种函数。
+    存储歌曲信息, 以及各种函数。
     常用的有如下:
     1. `name` / `album` / `artist`
     2. `downloading_state` / `downloading_value`
     3. `raw_info` / `processed_info` / `url_info`
     参数:
     1. `id`: 歌曲id (其实传入url也行)
     """
@@ -33,15 +33,17 @@
         self.title = ""
         self.artist = []
         self.artist_str = ""
         self.album = ""
         self.downloading_state = 0
         self.downloading_value = 0.00
         self.encode_data = {
-            "c": str([{"id": str(self.id)}]),
+            "c": str([{
+                "id": str(self.id)
+            }]),
             "csrf_token": "",
         }
         self.lyric_encode_data = {
             "csrf_token": "",
             "id": str(str(self.id)),
             "lv": -1,
             "tv": -1,
@@ -68,48 +70,45 @@
             filename=self.filename_format,
             artist=self.artist_str,
             album=self.album,
             id=self.id,
             title=self.title,
         )
         if formated.rfind("/") != -1:
-            formated = formated[: formated.rfind("/") + 1] + clean(
-                formated[formated.rfind("/") + 1 :]
-            )
+            formated = formated[:formated.rfind("/") + 1] + clean(
+                formated[formated.rfind("/") + 1:])
         else:
             formated = clean(formated)
         formated += "." + suffix
         return formated
 
     def get_info(self):
         """
         获取歌曲信息
         ----------
         无参数。
         """
         self.raw_info = NeteaseParams(
-            url=SONG_INFO_API, encode_data=self.encode_data
-        ).get_resource()["songs"][0]
+            url=SONG_INFO_API,
+            encode_data=self.encode_data).get_resource()["songs"][0]
         self.title = self.raw_info["name"]
         self.album = self.raw_info["al"]["name"]
         for i in self.raw_info["ar"]:
             self.artist.append(i["name"])
         self.artist_str = artist_turn_str(self.artist)
         self.processed_info = {
             "album": self.album,
             "title": self.title,
             "artist": self.artist,
             "id": self.id,
         }
-        self.url_info.update(
-            {
-                "album_pic": self.raw_info["al"]["picUrl"],
-                "song_file": SONG_FILE_API + self.id,
-            }
-        )
+        self.url_info.update({
+            "album_pic": self.raw_info["al"]["picUrl"],
+            "song_file": SONG_FILE_API + self.id,
+        })
         self.filename_info = {
             "song": self.get_formated_filename("mp3"),
             "pic": self.get_formated_filename("jpg"),
             "lyric": self.get_formated_filename("lrc"),
         }
         self.is_get = True
         return self.raw_info
@@ -120,47 +119,50 @@
         ----------
         无参数。
         """
         with threading.Semaphore(8):
             self.get_info()
 
     def song_download_enhanced(self, level: str, cookies=None):
+        """
+        用另外一个API的下载函数, 需要导入 `cookies` 发挥最大功效。
+        """
         flag = True
         level_key = ["standard", "higher", "exhigh", "lossless"]
         for i in level_key:
             if i == level:
                 flag = False
         if flag:
             raise Exception("Error at inputing 'level'.")
         """
-        data的数据格式：
+        data的数据格式: 
         {
             “ids”:str([id]),
             “level”:“standard”,
             “encodeType”:“aac”,
             “csrf_token”: “”
         }
-        其中id表示歌曲的id号，
-        level是音乐品质，
-        标准为standard，
-        较高音质为higher，
-        极高音质exhigh，
+        其中id表示歌曲的id号, 
+        level是音乐品质, 
+        标准为standard, 
+        较高音质为higher, 
+        极高音质exhigh, 
         无损音质关键词为lossless。
         """
         enhance_encode_data = {
             "ids": str([self.id]),
             "level": level,
             "encodeType": "mp3",
             "csrf_token": "",
         }
         if level == "lossless":
             enhance_encode_data["encodeType"] = "aac"
         enhanced_info = NeteaseParams(
-            encode_data=enhance_encode_data, url=SONG_FILE_API_2
-        ).get_resource(cookies=cookies)
+            encode_data=enhance_encode_data,
+            url=SONG_FILE_API_2).get_resource(cookies=cookies)
         return enhanced_info
 
     def song_download(self):
         # filename = self.get_formated_filename('mp3')
         filename = self.filename_info["song"]
         file_origin = OriginFile(self.url_info["song_file"])
         if file_origin.total_size <= 0:
@@ -174,63 +176,80 @@
         file_origin = OriginFile(self.url_info["album_pic"])
         if file_origin.total_size == -1:
             return -1
         file_origin.auto_start(filename=filename)
         return filename
 
     def lyric_get(self):
-        self.lyric = (
-            NeteaseParams(url=LYRIC_API, encode_data=self.lyric_encode_data)
-            .get_resource()["lrc"]["lyric"]
-            .replace("\n", "\n")
-        )
+        self.lyric = (NeteaseParams(
+            url=LYRIC_API, encode_data=self.lyric_encode_data).get_resource()
+            ["lrc"]["lyric"].replace("\n", "\n"))
         # filename = self.get_formated_filename('lrc')
         filename = self.filename_info["lyric"]
         with open(file=filename, mode="w+", encoding="UTF-8") as file:
             file.write(self.lyric)
         return filename
 
     def attribute_write(self, filename="No filename"):
         """
         往文件里面写入歌曲信息
         ----------
         参数:
-        1. `filename`: 文件名，字符串，仅mp3/flac格式
+        1. `filename`: 文件名, 字符串, 仅 `mp3/flac` 格式
         """
         filename_ready = self.get_formated_filename("mp3")
         if filename == "No filename":
             if self.filename_info.get("song") == None:
                 filename = filename_ready
             else:
                 filename = self.filename_info["song"]
         attribute_write(filename=filename, info=self.processed_info)
 
-    def cover_write(self, filename="No filename", cover_filename="No cover_filename"):
+    def cover_write(self,
+                    filename="No filename",
+                    cover_filename="No cover_filename"):
         """
         专辑封面写入
         ----------
         参数:
-        1. `filename`: 文件名，字符串，仅mp3/flac格式
-        2. `cover_filename`: 封面的文件名, 字符串, 仅jpg格式
+        1. `filename`: 文件名, 字符串, 仅 `mp3/flac` 格式
+        2. `cover_filename`: 封面的文件名, 字符串, 仅 `jpg` 格式
         """
         if filename == "No filename":
             filename = self.filename_info["song"]
         if cover_filename == "No cover_filename":
             cover_filename = self.filename_info["pic"]
         cover_write(filename=filename, cover_filename=cover_filename)
 
-    def lyric_write(self, filename="No filename", lyric_filename="No lyric_filename"):
+    def lyric_write(self,
+                    filename="No filename",
+                    lyric_filename="No lyric_filename"):
+        """
+        歌词写入
+        ----------
+        参数:
+        1. `filename`: 文件名, 字符串, 仅 `mp3/flac` 格式
+        2. `lyric_filename`: 封面的文件名, 字符串, 仅jpg格式
+        提示: 如果留空不会怎么样的, 用 `filename_info` 的数据代替
+        """
         if filename == "No filename":
             filename = self.filename_info["song"]
         if lyric_filename == "No lyric_filename":
             lyric_filename = self.filename_info["lyric"]
         lyric_write(filename=filename, lyric_filename=lyric_filename)
 
     def auto_run(self, d=None):
-        self.get_info()
+        """
+        自动获取信息&下载。
+        ----------
+        参数: 
+        1. `d`: 包含6个键: `song_download`, `cover_download`, `lyric_download`, `attribute_write`, `cover_write`, `lyric_write` 的字典。这几个键的值都是 `bool` 类型的。
+        """
+        if self.is_get == False:
+            self.get_info()
         if d["song_download"] == True:
             c = self.song_download()
             if c == -1:
                 self.is_dl = True
                 return -1
         if d["cover_download"] == True:
             self.cover_download()
@@ -241,8 +260,14 @@
         if d["cover_write"] == True:
             self.cover_write()
         if d["lyric_write"] == True:
             self.lyric_write()
         self.is_dl = True
 
     def multi_run(self, d=None):
-        threading.Thread(target=self.auto_run, args=(d,)).start()
+        """
+        多开线程的时候用的函数。
+        ----------
+        参数: 
+        1. `d`: 同 `auto_run` 的定义。
+        """
+        threading.Thread(target=self.auto_run, args=(d, )).start()
```

### Comparing `ncmlistdownloader-1.0.5.240429/ncmlistdownloader.egg-info/PKG-INFO` & `ncmlistdownloader-1.0.6.240429/ncmlistdownloader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.5.240429
+Version: 1.0.6.240429
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `ncmlistdownloader-1.0.5.240429/ncmlistdownloader.egg-info/SOURCES.txt` & `ncmlistdownloader-1.0.6.240429/ncmlistdownloader.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,10 +13,11 @@
 ncmlistdownloader/cmd/find_from_id.py
 ncmlistdownloader/cmd/json_io.py
 ncmlistdownloader/common/__init__.py
 ncmlistdownloader/common/encode_sec_key.py
 ncmlistdownloader/common/global_args.py
 ncmlistdownloader/common/thread_test.py
 ncmlistdownloader/downloader/__init__.py
+ncmlistdownloader/downloader/json_list_io.py
 ncmlistdownloader/editer/__init__.py
 ncmlistdownloader/playlist/__init__.py
 ncmlistdownloader/song/__init__.py
```

### Comparing `ncmlistdownloader-1.0.5.240429/setup.py` & `ncmlistdownloader-1.0.6.240429/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
     ],
     name="ncmlistdownloader",
-    version="1.0.5.240429",
+    version="1.0.6.240429",
     description="获取网易云音乐歌单数据，下载音乐，主动添加元信息。",
     author="CooooldWind_",
     url="https://gitee.com/Cooooldwind/163ListDownloader_NexT",
     packages=find_packages(),
     install_requires=[
         "pycryptodome",
         "pillow",
```

