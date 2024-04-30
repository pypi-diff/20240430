# Comparing `tmp/scdl-2.7.6.tar.gz` & `tmp/scdl-2.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/scdl/scdl/dist/.tmp-x78ywq8_/scdl-2.7.6.tar", last modified: Sun Apr 28 02:16:28 2024, max compression
+gzip compressed data, was "/home/runner/work/scdl/scdl/dist/.tmp-tjy4zj9j/scdl-2.7.7.tar", last modified: Tue Apr 30 17:05:25 2024, max compression
```

## Comparing `scdl-2.7.6.tar` & `scdl-2.7.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:28.000000 scdl-2.7.6/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-28 02:16:08.000000 scdl-2.7.6/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    18027 2024-04-28 02:16:08.000000 scdl-2.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-28 02:16:08.000000 scdl-2.7.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-28 02:16:28.000000 scdl-2.7.6/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     4954 2024-04-28 02:16:08.000000 scdl-2.7.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:28.000000 scdl-2.7.6/scdl/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-28 02:16:08.000000 scdl-2.7.6/scdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-28 02:16:08.000000 scdl-2.7.6/scdl/scdl.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)    38878 2024-04-28 02:16:08.000000 scdl-2.7.6/scdl/scdl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-28 02:16:08.000000 scdl-2.7.6/scdl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:16:28.000000 scdl-2.7.6/scdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-28 02:16:28.000000 scdl-2.7.6/scdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-28 02:16:28.000000 scdl-2.7.6/scdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 02:16:28.000000 scdl-2.7.6/scdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-28 02:16:28.000000 scdl-2.7.6/scdl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-28 02:16:28.000000 scdl-2.7.6/scdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-28 02:16:28.000000 scdl-2.7.6/scdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 02:16:28.000000 scdl-2.7.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1594 2024-04-28 02:16:08.000000 scdl-2.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:05:25.000000 scdl-2.7.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-30 17:05:08.000000 scdl-2.7.7/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    18027 2024-04-30 17:05:08.000000 scdl-2.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-30 17:05:08.000000 scdl-2.7.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-30 17:05:25.000000 scdl-2.7.7/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4954 2024-04-30 17:05:08.000000 scdl-2.7.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:05:25.000000 scdl-2.7.7/scdl/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-30 17:05:08.000000 scdl-2.7.7/scdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-30 17:05:08.000000 scdl-2.7.7/scdl/scdl.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    38567 2024-04-30 17:05:08.000000 scdl-2.7.7/scdl/scdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-30 17:05:08.000000 scdl-2.7.7/scdl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:05:25.000000 scdl-2.7.7/scdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-30 17:05:25.000000 scdl-2.7.7/scdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-30 17:05:25.000000 scdl-2.7.7/scdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 17:05:25.000000 scdl-2.7.7/scdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-30 17:05:25.000000 scdl-2.7.7/scdl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-30 17:05:25.000000 scdl-2.7.7/scdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-30 17:05:25.000000 scdl-2.7.7/scdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 17:05:25.000000 scdl-2.7.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1594 2024-04-30 17:05:08.000000 scdl-2.7.7/setup.py
```

### Comparing `scdl-2.7.6/LICENSE` & `scdl-2.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `scdl-2.7.6/PKG-INFO` & `scdl-2.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scdl
-Version: 2.7.6
+Version: 2.7.7
 Summary: Download Music from Souncloud
 Home-page: https://github.com/flyingrub/scdl
 Author: FlyinGrub
 Author-email: flyinggrub@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `scdl-2.7.6/README.md` & `scdl-2.7.7/README.md`

 * *Files identical despite different names*

### Comparing `scdl-2.7.6/scdl/scdl.cfg` & `scdl-2.7.7/scdl/scdl.cfg`

 * *Files identical despite different names*

### Comparing `scdl-2.7.6/scdl/scdl.py` & `scdl-2.7.7/scdl/scdl.py`

 * *Files 1% similar despite different names*

```diff
@@ -385,20 +385,19 @@
         logger.error(f"Unknown item type {item.kind}")
         sys.exit(1)
 
 def remove_files():
     """
     Removes any pre-existing tracks that were not just downloaded
     """
-    logger.info("Removing local track files...")
+    logger.info("Removing local track files that were not downloaded...")
     files = [f for f in os.listdir(".") if os.path.isfile(f)]
     for f in files:
         if f not in fileToKeep:
             os.remove(f)
-            logger.info(f'Removed {f}')
 
 def sync(client: SoundCloud, playlist: BasicAlbumPlaylist, playlist_info, **kwargs):
     """
     Downloads/Removes tracks that have been changed on playlist since last archive file
     """
     logger.info("Comparing tracks...")
     archive = kwargs.get("sync")
@@ -413,30 +412,27 @@
             logger.error(f'Error trying to convert track ids. Verify archive file is not empty.')
             logger.debug(verr)
             sys.exit(1)
 
     new = [track.id for track in playlist.tracks]
     add = set(new).difference(old) # find tracks to download
     rem = set(old).difference(new) # find tracks to remove
-    for track_id in new:
-        if (
-            client.get_track(track_id).downloadable
-            and not kwargs["onlymp3"]
-            and not kwargs.get("no_original")
-        ):
-            fileToKeep.append(get_original_filename(client, client.get_track(track_id), playlist_info, **kwargs))
-        else:
-            fileToKeep.append(get_filename(client.get_track(track_id), playlist_info=playlist_info, **kwargs))
 
     if not (add or rem):
         logger.info("No changes found. Exiting...")
         sys.exit(0)
 
     if rem:
-        remove_files()
+        for track_id in rem:
+            filename = get_filename(client.get_track(track_id),playlist_info=playlist_info,**kwargs)
+            if filename in os.listdir('.'):
+                os.remove(filename)
+                logger.info(f'Removed {filename}')
+            else:
+                logger.info(f'Could not find {filename} to remove')
         with open(archive,'w') as f:
           for track_id in old:
             if track_id not in rem:
               f.write(str(track_id)+'\n')
     else:
         logger.info('No tracks to remove.')
               
@@ -527,15 +523,18 @@
     if original_filename is not None:
         original_filename = original_filename.encode("utf-8", "ignore").decode("utf-8")
         ext = os.path.splitext(original_filename)[1]
     filename = limit_filename_length(title, ext)
     filename = sanitize_filename(filename)
     return filename
 
-def get_original_filename(client: SoundCloud, track: BasicTrack, playlist_info=None, **kwargs):
+
+def download_original_file(client: SoundCloud, track: BasicTrack, title: str, playlist_info=None, **kwargs):
+    logger.info("Downloading the original file.")
+
     # Get the requests stream
     url = client.get_track_original_download(track.id, track.secret_token)
     
     if not url:
         logger.info("Could not get original download link")
         return (None, False)
     
@@ -564,20 +563,15 @@
 
         # Find file extension
         mime = r.headers.get("content-type")
         ext = ext or mimetypes.guess_extension(mime)
         filename += ext
 
         filename = get_filename(track, filename, playlist_info=playlist_info, **kwargs)
-        return filename
-
-def download_original_file(client: SoundCloud, track: BasicTrack, title: str, playlist_info=None, **kwargs):
-    logger.info("Downloading the original file.")
 
-    filename = get_original_filename(client, track, playlist_info, **kwargs)
     logger.debug(f"filename : {filename}")
 
     # Skip if file ID or filename already exists
     if already_downloaded(track, title, filename, **kwargs):
         if kwargs.get("flac") and can_convert(filename):
             filename = filename[:-4] + ".flac"
         return (filename, True)
```

### Comparing `scdl-2.7.6/scdl/utils.py` & `scdl-2.7.7/scdl/utils.py`

 * *Files identical despite different names*

### Comparing `scdl-2.7.6/scdl.egg-info/PKG-INFO` & `scdl-2.7.7/scdl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scdl
-Version: 2.7.6
+Version: 2.7.7
 Summary: Download Music from Souncloud
 Home-page: https://github.com/flyingrub/scdl
 Author: FlyinGrub
 Author-email: flyinggrub@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `scdl-2.7.6/setup.py` & `scdl-2.7.7/setup.py`

 * *Files identical despite different names*

