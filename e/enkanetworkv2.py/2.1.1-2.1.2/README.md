# Comparing `tmp/enkanetworkv2.py-2.1.1.tar.gz` & `tmp/enkanetworkv2.py-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enkanetworkv2.py-2.1.1.tar", last modified: Tue Apr 30 13:35:40 2024, max compression
+gzip compressed data, was "enkanetworkv2.py-2.1.2.tar", last modified: Tue Apr 30 13:44:48 2024, max compression
```

## Comparing `enkanetworkv2.py-2.1.1.tar` & `enkanetworkv2.py-2.1.2.tar`

### file list

```diff
@@ -1,59 +1,62 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 13:35:40.246979 enkanetworkv2.py-2.1.1/
--rw-rw-rw-   0        0        0     1070 2024-02-24 18:53:52.000000 enkanetworkv2.py-2.1.1/LICENSE
--rw-rw-rw-   0        0        0       36 2024-02-24 18:58:13.000000 enkanetworkv2.py-2.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0    19316 2024-04-30 13:35:40.245476 enkanetworkv2.py-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    18242 2024-02-24 19:02:02.000000 enkanetworkv2.py-2.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 13:35:40.101350 enkanetworkv2.py-2.1.1/enkanetwork/
--rw-rw-rw-   0        0        0     1496 2024-04-30 13:35:14.000000 enkanetworkv2.py-2.1.1/enkanetwork/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 13:35:40.054304 enkanetworkv2.py-2.1.1/enkanetwork/assets/
-drwxrwxrwx   0        0        0        0 2024-04-30 13:35:40.144382 enkanetworkv2.py-2.1.1/enkanetwork/assets/data/
--rw-rw-rw-   0        0        0    54223 2024-04-29 13:06:38.000000 enkanetworkv2.py-2.1.1/enkanetwork/assets/data/artifact_props.json
--rw-rw-rw-   0        0        0  1095132 2024-04-29 13:06:37.000000 enkanetworkv2.py-2.1.1/enkanetwork/assets/data/artifacts.json
--rw-rw-rw-   0        0        0    43649 2024-04-29 13:06:38.000000 enkanetworkv2.py-2.1.1/enkanetwork/assets/data/characters.json
--rw-rw-rw-   0        0        0    52516 2024-04-29 13:06:38.000000 enkanetworkv2.py-2.1.1/enkanetwork/assets/data/constellations.json
--rw-rw-rw-   0        0        0    12831 2024-04-29 13:06:37.000000 enkanetworkv2.py-2.1.1/enkanetwork/assets/data/costumes.json
--rw-rw-rw-   0        0        0  1316924 2024-04-29 13:06:38.000000 enkanetworkv2.py-2.1.1/enkanetwork/assets/data/fight_props.json
--rw-rw-rw-   0        0        0    57396 2024-04-29 13:06:36.000000 enkanetworkv2.py-2.1.1/enkanetwork/assets/data/namecards.json
--rw-rw-rw-   0        0        0     8862 2024-04-29 13:07:47.000000 enkanetworkv2.py-2.1.1/enkanetwork/assets/data/pfps.json
--rw-rw-rw-   0        0        0    87635 2024-04-29 13:06:38.000000 enkanetworkv2.py-2.1.1/enkanetwork/assets/data/skills.json
--rw-rw-rw-   0        0        0    41728 2024-04-29 13:06:36.000000 enkanetworkv2.py-2.1.1/enkanetwork/assets/data/weapons.json
-drwxrwxrwx   0        0        0        0 2024-04-30 13:35:40.180419 enkanetworkv2.py-2.1.1/enkanetwork/assets/langs/
--rw-rw-rw-   0        0        0   588222 2024-04-29 13:07:45.000000 enkanetworkv2.py-2.1.1/enkanetwork/assets/langs/artifact_sets.json
--rw-rw-rw-   0        0        0  2571922 2024-04-29 13:07:46.000000 enkanetworkv2.py-2.1.1/enkanetwork/assets/langs/artifacts.json
--rw-rw-rw-   0        0        0    35634 2024-04-29 13:07:46.000000 enkanetworkv2.py-2.1.1/enkanetwork/assets/langs/characters.json
--rw-rw-rw-   0        0        0   329271 2024-04-29 13:07:46.000000 enkanetworkv2.py-2.1.1/enkanetwork/assets/langs/constellations.json
--rw-rw-rw-   0        0        0    30562 2024-04-26 18:46:57.000000 enkanetworkv2.py-2.1.1/enkanetwork/assets/langs/fight_props.json
--rw-rw-rw-   0        0        0   129254 2024-04-29 13:07:46.000000 enkanetworkv2.py-2.1.1/enkanetwork/assets/langs/namecards.json
--rw-rw-rw-   0        0        0   328482 2024-04-29 13:07:47.000000 enkanetworkv2.py-2.1.1/enkanetwork/assets/langs/skills.json
--rw-rw-rw-   0        0        0   119987 2024-04-29 13:07:47.000000 enkanetworkv2.py-2.1.1/enkanetwork/assets/langs/weapons.json
--rw-rw-rw-   0        0        0     8268 2024-04-29 12:09:14.000000 enkanetworkv2.py-2.1.1/enkanetwork/assets.py
--rw-rw-rw-   0        0        0      645 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.1.1/enkanetwork/cache.py
--rw-rw-rw-   0        0        0    12905 2024-04-29 12:21:07.000000 enkanetworkv2.py-2.1.1/enkanetwork/client.py
--rw-rw-rw-   0        0        0      798 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.1.1/enkanetwork/config.py
--rw-rw-rw-   0        0        0     1099 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.1.1/enkanetwork/enum.py
--rw-rw-rw-   0        0        0     1925 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.1.1/enkanetwork/exception.py
--rw-rw-rw-   0        0        0     7345 2024-02-24 18:56:30.000000 enkanetworkv2.py-2.1.1/enkanetwork/http.py
-drwxrwxrwx   0        0        0        0 2024-04-30 13:35:40.223456 enkanetworkv2.py-2.1.1/enkanetwork/model/
--rw-rw-rw-   0        0        0      137 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.1.1/enkanetwork/model/__init__.py
--rw-rw-rw-   0        0        0     5029 2024-04-06 17:00:40.000000 enkanetworkv2.py-2.1.1/enkanetwork/model/assets.py
--rw-rw-rw-   0        0        0     1935 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.1.1/enkanetwork/model/base.py
--rw-rw-rw-   0        0        0     1403 2024-02-24 18:46:53.000000 enkanetworkv2.py-2.1.1/enkanetwork/model/build.py
--rw-rw-rw-   0        0        0     5183 2024-02-24 18:47:25.000000 enkanetworkv2.py-2.1.1/enkanetwork/model/character.py
--rw-rw-rw-   0        0        0     5634 2024-02-24 18:35:48.000000 enkanetworkv2.py-2.1.1/enkanetwork/model/equipments.py
--rw-rw-rw-   0        0        0      307 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.1.1/enkanetwork/model/hoyos.py
--rw-rw-rw-   0        0        0     4063 2024-04-29 12:09:18.000000 enkanetworkv2.py-2.1.1/enkanetwork/model/players.py
--rw-rw-rw-   0        0        0      346 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.1.1/enkanetwork/model/profile.py
--rw-rw-rw-   0        0        0     7763 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.1.1/enkanetwork/model/stats.py
--rw-rw-rw-   0        0        0      293 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.1.1/enkanetwork/model/utils.py
--rw-rw-rw-   0        0        0     1313 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.1.1/enkanetwork/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-30 13:35:40.228968 enkanetworkv2.py-2.1.1/enkanetwork/types/
--rw-rw-rw-   0        0        0     1157 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.1.1/enkanetwork/types/enkanetwork.py
--rw-rw-rw-   0        0        0     3617 2024-04-26 17:01:35.000000 enkanetworkv2.py-2.1.1/enkanetwork/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-30 13:35:40.245476 enkanetworkv2.py-2.1.1/enkanetworkv2.py.egg-info/
--rw-rw-rw-   0        0        0    19316 2024-04-30 13:35:39.000000 enkanetworkv2.py-2.1.1/enkanetworkv2.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1520 2024-04-30 13:35:40.000000 enkanetworkv2.py-2.1.1/enkanetworkv2.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 13:35:39.000000 enkanetworkv2.py-2.1.1/enkanetworkv2.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-04-30 13:35:39.000000 enkanetworkv2.py-2.1.1/enkanetworkv2.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-30 13:35:39.000000 enkanetworkv2.py-2.1.1/enkanetworkv2.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 13:35:40.246979 enkanetworkv2.py-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1090 2024-04-29 13:13:06.000000 enkanetworkv2.py-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 13:44:48.369234 enkanetworkv2.py-2.1.2/
+-rw-rw-rw-   0        0        0     1070 2024-02-24 18:53:52.000000 enkanetworkv2.py-2.1.2/LICENSE
+-rw-rw-rw-   0        0        0       88 2024-04-30 13:42:24.000000 enkanetworkv2.py-2.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    19316 2024-04-30 13:44:48.368175 enkanetworkv2.py-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    18242 2024-02-24 19:02:02.000000 enkanetworkv2.py-2.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 13:44:48.327363 enkanetworkv2.py-2.1.2/enkanetwork/
+-rw-rw-rw-   0        0        0     1496 2024-04-30 13:44:29.000000 enkanetworkv2.py-2.1.2/enkanetwork/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 13:44:48.316268 enkanetworkv2.py-2.1.2/enkanetwork/assets/
+drwxrwxrwx   0        0        0        0 2024-04-30 13:44:48.335504 enkanetworkv2.py-2.1.2/enkanetwork/assets/data/
+-rw-rw-rw-   0        0        0    54223 2024-04-29 13:06:38.000000 enkanetworkv2.py-2.1.2/enkanetwork/assets/data/artifact_props.json
+-rw-rw-rw-   0        0        0  1095132 2024-04-29 13:06:37.000000 enkanetworkv2.py-2.1.2/enkanetwork/assets/data/artifacts.json
+-rw-rw-rw-   0        0        0    43649 2024-04-29 13:06:38.000000 enkanetworkv2.py-2.1.2/enkanetwork/assets/data/characters.json
+-rw-rw-rw-   0        0        0    52516 2024-04-29 13:06:38.000000 enkanetworkv2.py-2.1.2/enkanetwork/assets/data/constellations.json
+-rw-rw-rw-   0        0        0    12831 2024-04-29 13:06:37.000000 enkanetworkv2.py-2.1.2/enkanetwork/assets/data/costumes.json
+-rw-rw-rw-   0        0        0  1316924 2024-04-29 13:06:38.000000 enkanetworkv2.py-2.1.2/enkanetwork/assets/data/fight_props.json
+-rw-rw-rw-   0        0        0    57396 2024-04-29 13:06:36.000000 enkanetworkv2.py-2.1.2/enkanetwork/assets/data/namecards.json
+-rw-rw-rw-   0        0        0     8862 2024-04-29 13:07:47.000000 enkanetworkv2.py-2.1.2/enkanetwork/assets/data/pfps.json
+-rw-rw-rw-   0        0        0    87635 2024-04-29 13:06:38.000000 enkanetworkv2.py-2.1.2/enkanetwork/assets/data/skills.json
+-rw-rw-rw-   0        0        0    41728 2024-04-29 13:06:36.000000 enkanetworkv2.py-2.1.2/enkanetwork/assets/data/weapons.json
+drwxrwxrwx   0        0        0        0 2024-04-30 13:44:48.343012 enkanetworkv2.py-2.1.2/enkanetwork/assets/langs/
+-rw-rw-rw-   0        0        0   588222 2024-04-29 13:07:45.000000 enkanetworkv2.py-2.1.2/enkanetwork/assets/langs/artifact_sets.json
+-rw-rw-rw-   0        0        0  2571922 2024-04-29 13:07:46.000000 enkanetworkv2.py-2.1.2/enkanetwork/assets/langs/artifacts.json
+-rw-rw-rw-   0        0        0    35634 2024-04-29 13:07:46.000000 enkanetworkv2.py-2.1.2/enkanetwork/assets/langs/characters.json
+-rw-rw-rw-   0        0        0   329271 2024-04-29 13:07:46.000000 enkanetworkv2.py-2.1.2/enkanetwork/assets/langs/constellations.json
+-rw-rw-rw-   0        0        0    30562 2024-04-26 18:46:57.000000 enkanetworkv2.py-2.1.2/enkanetwork/assets/langs/fight_props.json
+-rw-rw-rw-   0        0        0   129254 2024-04-29 13:07:46.000000 enkanetworkv2.py-2.1.2/enkanetwork/assets/langs/namecards.json
+-rw-rw-rw-   0        0        0   328482 2024-04-29 13:07:47.000000 enkanetworkv2.py-2.1.2/enkanetwork/assets/langs/skills.json
+-rw-rw-rw-   0        0        0   119987 2024-04-29 13:07:47.000000 enkanetworkv2.py-2.1.2/enkanetwork/assets/langs/weapons.json
+-rw-rw-rw-   0        0        0     8268 2024-04-29 12:09:14.000000 enkanetworkv2.py-2.1.2/enkanetwork/assets.py
+-rw-rw-rw-   0        0        0      645 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.1.2/enkanetwork/cache.py
+-rw-rw-rw-   0        0        0    12905 2024-04-29 12:21:07.000000 enkanetworkv2.py-2.1.2/enkanetwork/client.py
+-rw-rw-rw-   0        0        0      798 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.1.2/enkanetwork/config.py
+drwxrwxrwx   0        0        0        0 2024-04-30 13:44:48.347011 enkanetworkv2.py-2.1.2/enkanetwork/enkanetwork_update/
+-rw-rw-rw-   0        0        0       77 2024-04-30 13:41:41.000000 enkanetworkv2.py-2.1.2/enkanetwork/enkanetwork_update/__init__.py
+-rw-rw-rw-   0        0        0     1510 2024-04-25 09:25:17.000000 enkanetworkv2.py-2.1.2/enkanetwork/enkanetwork_update/config.py
+-rw-rw-rw-   0        0        0    11832 2024-04-29 12:16:42.000000 enkanetworkv2.py-2.1.2/enkanetwork/enkanetwork_update/enka_update.py
+-rw-rw-rw-   0        0        0      549 2024-04-26 18:31:03.000000 enkanetworkv2.py-2.1.2/enkanetwork/enkanetwork_update/pathfinding.py
+-rw-rw-rw-   0        0        0     1099 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.1.2/enkanetwork/enum.py
+-rw-rw-rw-   0        0        0     1925 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.1.2/enkanetwork/exception.py
+-rw-rw-rw-   0        0        0     7345 2024-02-24 18:56:30.000000 enkanetworkv2.py-2.1.2/enkanetwork/http.py
+drwxrwxrwx   0        0        0        0 2024-04-30 13:44:48.352160 enkanetworkv2.py-2.1.2/enkanetwork/model/
+-rw-rw-rw-   0        0        0      137 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.1.2/enkanetwork/model/__init__.py
+-rw-rw-rw-   0        0        0     5029 2024-04-06 17:00:40.000000 enkanetworkv2.py-2.1.2/enkanetwork/model/assets.py
+-rw-rw-rw-   0        0        0     1935 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.1.2/enkanetwork/model/base.py
+-rw-rw-rw-   0        0        0     1403 2024-02-24 18:46:53.000000 enkanetworkv2.py-2.1.2/enkanetwork/model/build.py
+-rw-rw-rw-   0        0        0     5183 2024-02-24 18:47:25.000000 enkanetworkv2.py-2.1.2/enkanetwork/model/character.py
+-rw-rw-rw-   0        0        0     5634 2024-02-24 18:35:48.000000 enkanetworkv2.py-2.1.2/enkanetwork/model/equipments.py
+-rw-rw-rw-   0        0        0      307 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.1.2/enkanetwork/model/hoyos.py
+-rw-rw-rw-   0        0        0     4063 2024-04-29 12:09:18.000000 enkanetworkv2.py-2.1.2/enkanetwork/model/players.py
+-rw-rw-rw-   0        0        0      346 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.1.2/enkanetwork/model/profile.py
+-rw-rw-rw-   0        0        0     7763 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.1.2/enkanetwork/model/stats.py
+-rw-rw-rw-   0        0        0      293 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.1.2/enkanetwork/model/utils.py
+-rw-rw-rw-   0        0        0     1313 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.1.2/enkanetwork/tools.py
+-rw-rw-rw-   0        0        0     3617 2024-04-26 17:01:35.000000 enkanetworkv2.py-2.1.2/enkanetwork/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-30 13:44:48.367175 enkanetworkv2.py-2.1.2/enkanetworkv2.py.egg-info/
+-rw-rw-rw-   0        0        0    19316 2024-04-30 13:44:48.000000 enkanetworkv2.py-2.1.2/enkanetworkv2.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1663 2024-04-30 13:44:48.000000 enkanetworkv2.py-2.1.2/enkanetworkv2.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 13:44:48.000000 enkanetworkv2.py-2.1.2/enkanetworkv2.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-04-30 13:44:48.000000 enkanetworkv2.py-2.1.2/enkanetworkv2.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-30 13:44:48.000000 enkanetworkv2.py-2.1.2/enkanetworkv2.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 13:44:48.369234 enkanetworkv2.py-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1090 2024-04-29 13:13:06.000000 enkanetworkv2.py-2.1.2/setup.py
```

### Comparing `enkanetworkv2.py-2.1.1/LICENSE` & `enkanetworkv2.py-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/PKG-INFO` & `enkanetworkv2.py-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enkanetworkv2.py
-Version: 2.1.1
+Version: 2.1.2
 Summary: Library for fetching JSON data from site https://enka.network/
 Home-page: https://github.com/DEViantUA/EnkaNetworkV2.py
 Author: DeviantUa
 Author-email: deviantapi@gmail.com
 Keywords: enkanetwork.py,enkanetwork,enka.network,genshinapi,enkanetworkV2,enkanetworkV2.py
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enkanetworkv2.py-2.1.1/README.md` & `enkanetworkv2.py-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/__init__.py` & `enkanetworkv2.py-2.1.2/enkanetwork/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE."""
 
 __title__ = 'enkanetworkV2.py'
 __author__ = 'DeviantUa'
-__version__ = '2.1.1'
+__version__ = '2.1.2'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2024-present DeviantUa'
 
 
 from .client import *
 from .exception import *
 from .model import *
```

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/assets/data/artifact_props.json` & `enkanetworkv2.py-2.1.2/enkanetwork/assets/data/artifact_props.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/assets/data/artifacts.json` & `enkanetworkv2.py-2.1.2/enkanetwork/assets/data/artifacts.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/assets/data/characters.json` & `enkanetworkv2.py-2.1.2/enkanetwork/assets/data/characters.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/assets/data/constellations.json` & `enkanetworkv2.py-2.1.2/enkanetwork/assets/data/constellations.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/assets/data/costumes.json` & `enkanetworkv2.py-2.1.2/enkanetwork/assets/data/costumes.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/assets/data/fight_props.json` & `enkanetworkv2.py-2.1.2/enkanetwork/assets/data/fight_props.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/assets/data/namecards.json` & `enkanetworkv2.py-2.1.2/enkanetwork/assets/data/namecards.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/assets/data/pfps.json` & `enkanetworkv2.py-2.1.2/enkanetwork/assets/data/pfps.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/assets/data/skills.json` & `enkanetworkv2.py-2.1.2/enkanetwork/assets/data/skills.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/assets/data/weapons.json` & `enkanetworkv2.py-2.1.2/enkanetwork/assets/data/weapons.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/assets/langs/artifact_sets.json` & `enkanetworkv2.py-2.1.2/enkanetwork/assets/langs/artifact_sets.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/assets/langs/artifacts.json` & `enkanetworkv2.py-2.1.2/enkanetwork/assets/langs/artifacts.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/assets/langs/characters.json` & `enkanetworkv2.py-2.1.2/enkanetwork/assets/langs/characters.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/assets/langs/constellations.json` & `enkanetworkv2.py-2.1.2/enkanetwork/assets/langs/constellations.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/assets/langs/fight_props.json` & `enkanetworkv2.py-2.1.2/enkanetwork/assets/langs/fight_props.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/assets/langs/namecards.json` & `enkanetworkv2.py-2.1.2/enkanetwork/assets/langs/namecards.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/assets/langs/skills.json` & `enkanetworkv2.py-2.1.2/enkanetwork/assets/langs/skills.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/assets/langs/weapons.json` & `enkanetworkv2.py-2.1.2/enkanetwork/assets/langs/weapons.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/assets.py` & `enkanetworkv2.py-2.1.2/enkanetwork/assets.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/cache.py` & `enkanetworkv2.py-2.1.2/enkanetwork/cache.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/client.py` & `enkanetworkv2.py-2.1.2/enkanetwork/client.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/config.py` & `enkanetworkv2.py-2.1.2/enkanetwork/config.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/enum.py` & `enkanetworkv2.py-2.1.2/enkanetwork/enum.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/exception.py` & `enkanetworkv2.py-2.1.2/enkanetwork/exception.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/http.py` & `enkanetworkv2.py-2.1.2/enkanetwork/http.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/model/assets.py` & `enkanetworkv2.py-2.1.2/enkanetwork/model/assets.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/model/base.py` & `enkanetworkv2.py-2.1.2/enkanetwork/model/base.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/model/build.py` & `enkanetworkv2.py-2.1.2/enkanetwork/model/build.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/model/character.py` & `enkanetworkv2.py-2.1.2/enkanetwork/model/character.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/model/equipments.py` & `enkanetworkv2.py-2.1.2/enkanetwork/model/equipments.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/model/players.py` & `enkanetworkv2.py-2.1.2/enkanetwork/model/players.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/model/stats.py` & `enkanetworkv2.py-2.1.2/enkanetwork/model/stats.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/tools.py` & `enkanetworkv2.py-2.1.2/enkanetwork/tools.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetwork/utils.py` & `enkanetworkv2.py-2.1.2/enkanetwork/utils.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.1.1/enkanetworkv2.py.egg-info/PKG-INFO` & `enkanetworkv2.py-2.1.2/enkanetworkv2.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enkanetworkv2.py
-Version: 2.1.1
+Version: 2.1.2
 Summary: Library for fetching JSON data from site https://enka.network/
 Home-page: https://github.com/DEViantUA/EnkaNetworkV2.py
 Author: DeviantUa
 Author-email: deviantapi@gmail.com
 Keywords: enkanetwork.py,enkanetwork,enka.network,genshinapi,enkanetworkV2,enkanetworkV2.py
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enkanetworkv2.py-2.1.1/enkanetworkv2.py.egg-info/SOURCES.txt` & `enkanetworkv2.py-2.1.2/enkanetworkv2.py.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -26,24 +26,27 @@
 enkanetwork/assets/langs/artifacts.json
 enkanetwork/assets/langs/characters.json
 enkanetwork/assets/langs/constellations.json
 enkanetwork/assets/langs/fight_props.json
 enkanetwork/assets/langs/namecards.json
 enkanetwork/assets/langs/skills.json
 enkanetwork/assets/langs/weapons.json
+enkanetwork/enkanetwork_update/__init__.py
+enkanetwork/enkanetwork_update/config.py
+enkanetwork/enkanetwork_update/enka_update.py
+enkanetwork/enkanetwork_update/pathfinding.py
 enkanetwork/model/__init__.py
 enkanetwork/model/assets.py
 enkanetwork/model/base.py
 enkanetwork/model/build.py
 enkanetwork/model/character.py
 enkanetwork/model/equipments.py
 enkanetwork/model/hoyos.py
 enkanetwork/model/players.py
 enkanetwork/model/profile.py
 enkanetwork/model/stats.py
 enkanetwork/model/utils.py
-enkanetwork/types/enkanetwork.py
 enkanetworkv2.py.egg-info/PKG-INFO
 enkanetworkv2.py.egg-info/SOURCES.txt
 enkanetworkv2.py.egg-info/dependency_links.txt
 enkanetworkv2.py.egg-info/requires.txt
 enkanetworkv2.py.egg-info/top_level.txt
```

### Comparing `enkanetworkv2.py-2.1.1/setup.py` & `enkanetworkv2.py-2.1.2/setup.py`

 * *Files identical despite different names*

