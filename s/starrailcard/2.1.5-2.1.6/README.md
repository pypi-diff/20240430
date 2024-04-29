# Comparing `tmp/starrailcard-2.1.5.tar.gz` & `tmp/starrailcard-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrailcard-2.1.5.tar", max compression
+gzip compressed data, was "starrailcard-2.1.6.tar", last modified: Mon Apr 29 22:39:02 2024, max compression
```

## Comparing `starrailcard-2.1.5.tar` & `starrailcard-2.1.6.tar`

### file list

```diff
@@ -1,51 +1,73 @@
--rw-r--r--   0        0        0     1721 2024-03-20 15:38:40.776791 starrailcard-2.1.5/LICENSE
--rw-r--r--   0        0        0     1106 2024-04-18 21:49:53.836647 starrailcard-2.1.5/pyproject.toml
--rw-r--r--   0        0        0     3642 2024-03-18 20:36:48.857949 starrailcard-2.1.5/README.md
--rw-r--r--   0        0        0       75 2024-03-15 20:07:42.107466 starrailcard-2.1.5/starrailcard/__init__.py
--rw-r--r--   0        0        0    11836 2024-04-17 16:12:22.105894 starrailcard-2.1.5/starrailcard/client.py
--rw-r--r--   0        0        0      106 2024-03-20 15:35:34.777763 starrailcard-2.1.5/starrailcard/requirements.txt
--rw-r--r--   0        0        0     2461 2024-04-14 21:56:24.992763 starrailcard-2.1.5/starrailcard/src/api/api.py
--rw-r--r--   0        0        0     3487 2024-04-14 22:43:00.884583 starrailcard-2.1.5/starrailcard/src/api/enka.py
--rw-r--r--   0        0        0    25187 2024-04-14 22:52:21.950058 starrailcard-2.1.5/starrailcard/src/api/enka_parsed.py
--rw-r--r--   0        0        0      487 2024-04-09 16:19:13.263140 starrailcard-2.1.5/starrailcard/src/api/error.py
--rw-r--r--   0        0        0   201292 2023-10-12 08:13:59.547042 starrailcard-2.1.5/starrailcard/src/assets/font/font_hsr.ttf
--rw-r--r--   0        0        0     1751 2024-03-28 18:26:38.347683 starrailcard-2.1.5/starrailcard/src/data/avatar.json
--rw-r--r--   0        0        0      252 2024-03-28 18:26:38.460098 starrailcard-2.1.5/starrailcard/src/data/element.json
--rw-r--r--   0        0        0       70 2024-03-28 18:26:38.462097 starrailcard-2.1.5/starrailcard/src/data/keys.json
--rw-r--r--   0        0        0      293 2024-03-28 18:26:38.423267 starrailcard-2.1.5/starrailcard/src/data/paths.json
--rw-r--r--   0        0        0     1915 2024-03-28 18:26:38.386139 starrailcard-2.1.5/starrailcard/src/data/relict_sets.json
--rw-r--r--   0        0        0     4947 2024-03-28 18:26:38.266305 starrailcard-2.1.5/starrailcard/src/data/stats.json
--rw-r--r--   0        0        0     4738 2024-03-28 18:26:38.308097 starrailcard-2.1.5/starrailcard/src/data/weapons.json
--rw-r--r--   0        0        0     6696 2024-04-06 18:31:53.629800 starrailcard-2.1.5/starrailcard/src/generator/style_profile_phone.py
--rw-r--r--   0        0        0    24567 2024-04-17 16:11:52.691388 starrailcard-2.1.5/starrailcard/src/generator/style_relict_score.py
--rw-r--r--   0        0        0    30356 2024-04-17 16:11:41.400283 starrailcard-2.1.5/starrailcard/src/generator/style_ticket.py
--rw-r--r--   0        0        0    11769 2024-04-14 20:59:53.695835 starrailcard-2.1.5/starrailcard/src/model/api_mihomo.py
--rw-r--r--   0        0        0     4759 2024-04-13 14:26:08.588002 starrailcard-2.1.5/starrailcard/src/model/StarRailCard.py
--rw-r--r--   0        0        0     4065 2024-03-13 13:47:58.864230 starrailcard-2.1.5/starrailcard/src/model/style.py
--rw-r--r--   0        0        0      493 2024-03-13 13:48:02.345029 starrailcard-2.1.5/starrailcard/src/model/ukrainization_model.py
--rw-r--r--   0        0        0      845 2024-03-13 13:48:07.469416 starrailcard-2.1.5/starrailcard/src/model/utils_model.py
--rw-r--r--   0        0        0      373 2024-04-06 18:51:59.632223 starrailcard-2.1.5/starrailcard/src/tools/calculator/src/assets/max.json
--rw-r--r--   0        0        0       49 2024-04-06 18:52:00.222443 starrailcard-2.1.5/starrailcard/src/tools/calculator/src/assets/relic_id.json
--rw-r--r--   0        0        0     3434 2024-04-06 18:52:00.479448 starrailcard-2.1.5/starrailcard/src/tools/calculator/src/assets/rolls.json
--rw-r--r--   0        0        0    92881 2024-04-06 18:52:01.246844 starrailcard-2.1.5/starrailcard/src/tools/calculator/src/assets/score.json
--rw-r--r--   0        0        0     1959 2024-03-13 13:47:21.923389 starrailcard-2.1.5/starrailcard/src/tools/calculator/src/utils.py
--rw-r--r--   0        0        0     5747 2024-04-01 14:16:17.689304 starrailcard-2.1.5/starrailcard/src/tools/calculator/stats.py
--rw-r--r--   0        0        0     2526 2024-02-22 12:56:12.220916 starrailcard-2.1.5/starrailcard/src/tools/cashe.py
--rw-r--r--   0        0        0      709 2024-04-09 17:29:46.754642 starrailcard-2.1.5/starrailcard/src/tools/enums.py
--rw-r--r--   0        0        0    10136 2024-02-23 21:20:24.125982 starrailcard-2.1.5/starrailcard/src/tools/git.py
--rw-r--r--   0        0        0    10025 2024-04-14 05:20:03.169865 starrailcard-2.1.5/starrailcard/src/tools/http.py
--rw-r--r--   0        0        0      938 2024-04-09 16:56:51.818599 starrailcard-2.1.5/starrailcard/src/tools/json_data.py
--rw-r--r--   0        0        0     6341 2024-04-14 04:42:09.584031 starrailcard-2.1.5/starrailcard/src/tools/options.py
--rw-r--r--   0        0        0      199 2024-02-18 13:46:16.566296 starrailcard-2.1.5/starrailcard/src/tools/pill/__init__.py
--rw-r--r--   0        0        0     3854 2024-02-22 12:55:07.451038 starrailcard-2.1.5/starrailcard/src/tools/pill/color.py
--rw-r--r--   0        0        0     2330 2024-02-22 13:03:49.291296 starrailcard-2.1.5/starrailcard/src/tools/pill/color_controle.py
--rw-r--r--   0        0        0     5518 2024-02-25 12:31:53.901150 starrailcard-2.1.5/starrailcard/src/tools/pill/grandiend_v2.py
--rw-r--r--   0        0        0     3284 2024-02-22 12:55:28.873148 starrailcard-2.1.5/starrailcard/src/tools/pill/grandient_v1.py
--rw-r--r--   0        0        0     3952 2024-04-14 22:23:43.804859 starrailcard-2.1.5/starrailcard/src/tools/pill/image_controle.py
--rw-r--r--   0        0        0     5106 2024-02-22 12:55:59.845148 starrailcard-2.1.5/starrailcard/src/tools/pill/style_editor.py
--rw-r--r--   0        0        0     2116 2024-02-22 13:01:14.697378 starrailcard-2.1.5/starrailcard/src/tools/pill/text_controle.py
--rw-r--r--   0        0        0     2360 2024-03-13 13:31:40.291343 starrailcard-2.1.5/starrailcard/src/tools/translator.py
--rw-r--r--   0        0        0     6585 2024-02-22 12:57:06.983609 starrailcard-2.1.5/starrailcard/src/tools/treePaths.py
--rw-r--r--   0        0        0     1748 2024-03-28 18:26:54.868269 starrailcard-2.1.5/starrailcard/src/tools/ukrainization.py
--rw-r--r--   0        0        0     6884 2024-03-18 20:19:11.991157 starrailcard-2.1.5/starrailcard/utils.py
--rw-r--r--   0        0        0     4845 1970-01-01 00:00:00.000000 starrailcard-2.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-29 22:39:02.966995 starrailcard-2.1.6/
+-rw-rw-rw-   0        0        0     1721 2024-03-20 15:38:40.000000 starrailcard-2.1.6/LICENSE
+-rw-rw-rw-   0        0        0       38 2024-04-29 22:20:14.000000 starrailcard-2.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     4744 2024-04-29 22:39:02.966995 starrailcard-2.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3642 2024-03-18 20:36:48.000000 starrailcard-2.1.6/README.md
+-rw-rw-rw-   0        0        0     1106 2024-04-18 21:49:53.000000 starrailcard-2.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-29 22:39:02.966995 starrailcard-2.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1544 2024-04-29 22:37:14.000000 starrailcard-2.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 22:39:02.927251 starrailcard-2.1.6/starrailcard/
+-rw-rw-rw-   0        0        0     1963 2024-04-29 22:38:56.000000 starrailcard-2.1.6/starrailcard/__init__.py
+-rw-rw-rw-   0        0        0    12335 2024-04-29 22:25:47.000000 starrailcard-2.1.6/starrailcard/client.py
+drwxrwxrwx   0        0        0        0 2024-04-29 22:39:02.920894 starrailcard-2.1.6/starrailcard/src/
+drwxrwxrwx   0        0        0        0 2024-04-29 22:39:02.942269 starrailcard-2.1.6/starrailcard/src/api/
+-rw-rw-rw-   0        0        0     2761 2024-04-29 21:42:26.000000 starrailcard-2.1.6/starrailcard/src/api/api.py
+-rw-rw-rw-   0        0        0     3487 2024-04-14 22:43:00.000000 starrailcard-2.1.6/starrailcard/src/api/enka.py
+-rw-rw-rw-   0        0        0    25187 2024-04-14 22:52:21.000000 starrailcard-2.1.6/starrailcard/src/api/enka_parsed.py
+-rw-rw-rw-   0        0        0      487 2024-04-09 16:19:13.000000 starrailcard-2.1.6/starrailcard/src/api/error.py
+drwxrwxrwx   0        0        0        0 2024-04-29 22:39:02.920894 starrailcard-2.1.6/starrailcard/src/assets/
+drwxrwxrwx   0        0        0        0 2024-04-29 22:39:02.942269 starrailcard-2.1.6/starrailcard/src/assets/font/
+-rw-rw-rw-   0        0        0   201292 2023-10-12 08:13:59.000000 starrailcard-2.1.6/starrailcard/src/assets/font/font_hsr.ttf
+drwxrwxrwx   0        0        0        0 2024-04-29 22:39:02.948270 starrailcard-2.1.6/starrailcard/src/data/
+-rw-rw-rw-   0        0        0     1751 2024-03-28 18:26:38.000000 starrailcard-2.1.6/starrailcard/src/data/avatar.json
+-rw-rw-rw-   0        0        0      252 2024-03-28 18:26:38.000000 starrailcard-2.1.6/starrailcard/src/data/element.json
+-rw-rw-rw-   0        0        0       70 2024-03-28 18:26:38.000000 starrailcard-2.1.6/starrailcard/src/data/keys.json
+-rw-rw-rw-   0        0        0      293 2024-03-28 18:26:38.000000 starrailcard-2.1.6/starrailcard/src/data/paths.json
+-rw-rw-rw-   0        0        0     1915 2024-03-28 18:26:38.000000 starrailcard-2.1.6/starrailcard/src/data/relict_sets.json
+-rw-rw-rw-   0        0        0     4947 2024-03-28 18:26:38.000000 starrailcard-2.1.6/starrailcard/src/data/stats.json
+-rw-rw-rw-   0        0        0     4738 2024-03-28 18:26:38.000000 starrailcard-2.1.6/starrailcard/src/data/weapons.json
+drwxrwxrwx   0        0        0        0 2024-04-29 22:39:02.949269 starrailcard-2.1.6/starrailcard/src/generator/
+-rw-rw-rw-   0        0        0     6662 2024-04-20 04:28:23.000000 starrailcard-2.1.6/starrailcard/src/generator/style_profile_phone.py
+-rw-rw-rw-   0        0        0    24567 2024-04-17 16:11:52.000000 starrailcard-2.1.6/starrailcard/src/generator/style_relict_score.py
+-rw-rw-rw-   0        0        0    30356 2024-04-17 16:11:41.000000 starrailcard-2.1.6/starrailcard/src/generator/style_ticket.py
+drwxrwxrwx   0        0        0        0 2024-04-29 22:39:02.952782 starrailcard-2.1.6/starrailcard/src/model/
+-rw-rw-rw-   0        0        0     4759 2024-04-13 14:26:08.000000 starrailcard-2.1.6/starrailcard/src/model/StarRailCard.py
+-rw-rw-rw-   0        0        0    11769 2024-04-14 20:59:53.000000 starrailcard-2.1.6/starrailcard/src/model/api_mihomo.py
+-rw-rw-rw-   0        0        0     4065 2024-03-13 13:47:58.000000 starrailcard-2.1.6/starrailcard/src/model/style.py
+-rw-rw-rw-   0        0        0      493 2024-03-13 13:48:02.000000 starrailcard-2.1.6/starrailcard/src/model/ukrainization_model.py
+-rw-rw-rw-   0        0        0      845 2024-03-13 13:48:07.000000 starrailcard-2.1.6/starrailcard/src/model/utils_model.py
+drwxrwxrwx   0        0        0        0 2024-04-29 22:39:02.957780 starrailcard-2.1.6/starrailcard/src/tools/
+drwxrwxrwx   0        0        0        0 2024-04-29 22:39:02.958779 starrailcard-2.1.6/starrailcard/src/tools/calculator/
+drwxrwxrwx   0        0        0        0 2024-04-29 22:39:02.958779 starrailcard-2.1.6/starrailcard/src/tools/calculator/src/
+drwxrwxrwx   0        0        0        0 2024-04-29 22:39:02.960779 starrailcard-2.1.6/starrailcard/src/tools/calculator/src/assets/
+-rw-rw-rw-   0        0        0      373 2024-04-06 18:51:59.000000 starrailcard-2.1.6/starrailcard/src/tools/calculator/src/assets/max.json
+-rw-rw-rw-   0        0        0       49 2024-04-06 18:52:00.000000 starrailcard-2.1.6/starrailcard/src/tools/calculator/src/assets/relic_id.json
+-rw-rw-rw-   0        0        0     3434 2024-04-06 18:52:00.000000 starrailcard-2.1.6/starrailcard/src/tools/calculator/src/assets/rolls.json
+-rw-rw-rw-   0        0        0    92881 2024-04-06 18:52:01.000000 starrailcard-2.1.6/starrailcard/src/tools/calculator/src/assets/score.json
+-rw-rw-rw-   0        0        0     1959 2024-03-13 13:47:21.000000 starrailcard-2.1.6/starrailcard/src/tools/calculator/src/utils.py
+-rw-rw-rw-   0        0        0     5747 2024-04-01 14:16:17.000000 starrailcard-2.1.6/starrailcard/src/tools/calculator/stats.py
+-rw-rw-rw-   0        0        0     2526 2024-02-22 12:56:12.000000 starrailcard-2.1.6/starrailcard/src/tools/cashe.py
+-rw-rw-rw-   0        0        0      709 2024-04-09 17:29:46.000000 starrailcard-2.1.6/starrailcard/src/tools/enums.py
+-rw-rw-rw-   0        0        0    10136 2024-02-23 21:20:24.000000 starrailcard-2.1.6/starrailcard/src/tools/git.py
+-rw-rw-rw-   0        0        0     9968 2024-04-29 22:09:02.000000 starrailcard-2.1.6/starrailcard/src/tools/http.py
+-rw-rw-rw-   0        0        0      938 2024-04-09 16:56:51.000000 starrailcard-2.1.6/starrailcard/src/tools/json_data.py
+-rw-rw-rw-   0        0        0     7017 2024-04-29 22:06:20.000000 starrailcard-2.1.6/starrailcard/src/tools/options.py
+drwxrwxrwx   0        0        0        0 2024-04-29 22:39:02.964995 starrailcard-2.1.6/starrailcard/src/tools/pill/
+-rw-rw-rw-   0        0        0      199 2024-04-29 21:26:56.000000 starrailcard-2.1.6/starrailcard/src/tools/pill/__init__.py
+-rw-rw-rw-   0        0        0     3854 2024-02-22 12:55:07.000000 starrailcard-2.1.6/starrailcard/src/tools/pill/color.py
+-rw-rw-rw-   0        0        0     2330 2024-02-22 13:03:49.000000 starrailcard-2.1.6/starrailcard/src/tools/pill/color_controle.py
+-rw-rw-rw-   0        0        0     5518 2024-02-25 12:31:53.000000 starrailcard-2.1.6/starrailcard/src/tools/pill/grandiend_v2.py
+-rw-rw-rw-   0        0        0     3284 2024-02-22 12:55:28.000000 starrailcard-2.1.6/starrailcard/src/tools/pill/grandient_v1.py
+-rw-rw-rw-   0        0        0     5534 2024-04-29 22:03:56.000000 starrailcard-2.1.6/starrailcard/src/tools/pill/image_controle.py
+-rw-rw-rw-   0        0        0     5106 2024-02-22 12:55:59.000000 starrailcard-2.1.6/starrailcard/src/tools/pill/style_editor.py
+-rw-rw-rw-   0        0        0     2116 2024-02-22 13:01:14.000000 starrailcard-2.1.6/starrailcard/src/tools/pill/text_controle.py
+-rw-rw-rw-   0        0        0     2360 2024-03-13 13:31:40.000000 starrailcard-2.1.6/starrailcard/src/tools/translator.py
+-rw-rw-rw-   0        0        0     6585 2024-02-22 12:57:06.000000 starrailcard-2.1.6/starrailcard/src/tools/treePaths.py
+-rw-rw-rw-   0        0        0     1748 2024-03-28 18:26:54.000000 starrailcard-2.1.6/starrailcard/src/tools/ukrainization.py
+-rw-rw-rw-   0        0        0     6884 2024-03-18 20:19:11.000000 starrailcard-2.1.6/starrailcard/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 22:39:02.965995 starrailcard-2.1.6/starrailcard.egg-info/
+-rw-rw-rw-   0        0        0     4744 2024-04-29 22:39:02.000000 starrailcard-2.1.6/starrailcard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2011 2024-04-29 22:39:02.000000 starrailcard-2.1.6/starrailcard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 22:39:02.000000 starrailcard-2.1.6/starrailcard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2024-04-29 22:39:02.000000 starrailcard-2.1.6/starrailcard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-29 22:39:02.000000 starrailcard-2.1.6/starrailcard.egg-info/top_level.txt
```

### Comparing `starrailcard-2.1.5/LICENSE` & `starrailcard-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/pyproject.toml` & `starrailcard-2.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/README.md` & `starrailcard-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/starrailcard/client.py` & `starrailcard-2.1.6/starrailcard/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,48 +3,60 @@
 
 import anyio
 #import asyncio
 
 from .src.tools import http, ukrainization, options, translator, cashe, git
 from .src.generator import style_relict_score, style_ticket, style_profile_phone
 from .src.api import api, enka
-from .src.model import StarRailCard
+from .src.model import StarRailCard,api_mihomo
+from .src.tools.pill import image_controle
+
 
 
 class Card:
-    def __init__(self, lang = "en", character_art = None, character_id = None, seeleland = False,
-                 user_font = None, save = False, asset_save = False, remove_logo = False,
-                 cashe = {"maxsize": 150, "ttl": 300}, enka = False):
+    def __init__(self, lang: str = "en", character_art = None, character_id = None, seeleland: bool = False,
+                 user_font = None, save: bool = False, asset_save: bool = False, boost_speed: bool = False, remove_logo: bool = False,
+                 cashe = {"maxsize": 150, "ttl": 300}, enka: bool = False, api_data: api_mihomo.MiHoMoApi = None, proxy: str =  None, 
+                 user_agent: str = None):
         """Main class for generating cards
 
         Args:
             lang (str, optional): Language in which generation will take place, supported languages: cht, cn, de, en, es, fr, id, jp, kr, pt, ru, th, vi, ua . Defaults to "en".
             character_art (dict, optional): A dictionary that contains a key - character id and link value (If you want to pass several images for 1 character, you can use list in the values). Defaults to None.
             character_id (str, optional): List character ids separated by commas. Defaults to None.
             seeleland (bool, optional): Enable Seeleland statistics. Defaults to False.
             user_font (srt, optional): Font path or font name. Defaults to None.
             save (bool, optional): Whether to save images or not (Does not work for animated cards). Defaults to False.
             asset_save (bool, optional): Save assets to the device so that in subsequent calls you do not have to download them, but open them from the device. Defaults to False.
+            boost_speed (bool, optional): Allows you to download generation resources to your device for further use without downloading. !!!Fills up the device memory!!!.
             remove_logo (bool, optional): Remove GItHub logo. Defaults to False.
             cashe (dict, optional): Set your cache settings. Defaults to {"maxsize": 150, "ttl": 300}.
+            api_data (MiHoMoApi, optional): Pass your data received via: api.ApiMiHoMo(uid,"en").get()
+            proxy (str, optional): Proxy as a string: http://111.111.111.111:8888
+            user_agent (str, optional): Custom User-Agent.
         """
         self.lang = lang
         self.character_art  = character_art
         self.character_id  = character_id
         self.seeleland = seeleland
         self.user_font = user_font
         self.save = save
         self.asset_save = asset_save
         self.remove_logo = remove_logo
         self.cashe = cashe
         self.enka = enka
+        self.boost_speed = boost_speed
+        self.api_data = api_data
+        self.proxy = proxy
+        self.user_agent = options.get_user_agent(user_agent)
+
         
     async def __aenter__(self):
         cashe.Cache.get_cache(maxsize = self.cashe.get("maxsize", 150), ttl = self.cashe.get("ttl", 300))
-        await http.AioSession.enter()
+        await http.AioSession.enter(self.proxy)
         
         await git.ImageCache.set_assets_dowload(self.asset_save)
         
         if self.character_id:
             self.character_id = await options.get_charter_id(self.character_id)
         
         if self.character_art:
@@ -61,14 +73,17 @@
             await ukrainization.TranslateDataManager().check_update()
         
         self.translateLang = translator.Translator(self.lang)
 
         if self.user_font:
             await git.change_font(font_path = self.user_font)
         
+        image_controle._boost_speed = self.boost_speed
+
+        
         if self.remove_logo:
             print("""
                 Thank you for using our StarRailCard!
                 By removing the GitHub logo from the generated results, you acknowledge supporting the author through one of the following links:
                 - Patreon: https://www.patreon.com/deviantapi/membership
                 - Ko-fi: https://ko-fi.com/dezzso
 
@@ -113,19 +128,26 @@
             hide_uid (bool, optional): Hide UID. Defaults to False.
             background (str, optional): Link to custom card background. Defaults to None.
             force_update (bool, optional): Forced update of user data. Defaults to False.
 
         Returns:
             StarRail: A class object containing profile information and a profile card
         """
-        if self.enka:
-            data = await enka.ApiEnkaNetwork(uid, lang= self.lang).get()
+        if self.api_data is None:
+            if self.enka:
+                try:
+                    data = await enka.ApiEnkaNetwork(uid, lang= self.lang).get()
+                except Exception as e:
+                    print("To use the EnkaNetwork API you need to download/update the asset\nExample: await enka.ApiEnkaNetwork().update_assets()")
+                    data = await api.ApiMiHoMo(uid, lang= self.lang, force_update = force_update, user_agent= self.user_agent).get()
+            else:
+                data = await api.ApiMiHoMo(uid, lang= self.lang, force_update = force_update, user_agent= self.user_agent).get()
         else:
-            data = await api.ApiMiHoMo(uid, lang= self.lang, force_update = force_update).get()
-        
+            data = self.api_data
+            
         try:
             player = data.player.model_dump()
         except:
             player = data.player
             
         response = {
             "settings": {
@@ -167,24 +189,26 @@
             force_update (bool, optional): forced update of user data. Defaults to False.
             style_settings (dict, optional): not implemented yet. Defaults to None.
 
         Returns:
             StarRail: A class object containing profile information and a character cards
         """
         
-        if self.enka:
-            try:
-                data = await enka.ApiEnkaNetwork(uid, lang= self.lang).get()
-            except Exception as e:
-                print("To use the EnkaNetwork API you need to download/update the asset\nExample: await enka.ApiEnkaNetwork().update_assets()")
-                data = await api.ApiMiHoMo(uid, lang= self.lang, force_update = force_update).get()
+        if self.api_data is None:
+            if self.enka:
+                try:
+                    data = await enka.ApiEnkaNetwork(uid, lang= self.lang).get()
+                except Exception as e:
+                    print("To use the EnkaNetwork API you need to download/update the asset")
+                    data = await api.ApiMiHoMo(uid, lang= self.lang, force_update = force_update, user_agent= self.user_agent).get()
+            else:
+                data = await api.ApiMiHoMo(uid, lang= self.lang, force_update = force_update, user_agent= self.user_agent).get()
         else:
-            data = await api.ApiMiHoMo(uid, lang= self.lang, force_update = force_update).get()
-            
-        #data = await api.ApiMiHoMo(uid, lang= self.lang, force_update = force_update).get()
+            data = self.api_data
+
         result = []
         
         style, style_settings = await options.style_setting(style, style_settings)
         
         try:
             player = data.player.model_dump()
         except:
@@ -225,36 +249,15 @@
                             result.append(await style_relict_score.Creat(key,self.translateLang,art,hide_uid,uid, self.seeleland,self.remove_logo).start())
                         elif style == 2:
                             result.append(await style_ticket.Creat(key,self.translateLang,art,hide_uid,uid, self.seeleland,self.remove_logo).start())
                     except Exception as e:
                         print(f"Error in get_result for character {key.id}: {e}")
                         
                 tasks.start_soon(get_result, key)
-        
-        '''for key in data.characters:
-            response["character_id"].append(key.id)
-            response["character_name"].append(key.name)
-            
-            if self.character_id:
-                if not str(key.id) in self.character_id:
-                    continue  
-            
-            art = None
-            if self.character_art:
-                if str(key.id) in self.character_art:
-                    art = self.character_art[str(key.id)]
-            if style == 1:
-                result.append(style_relict_score.Creat(key,self.translateLang,art,hide_uid,uid, self.seeleland,self.remove_logo).start())
-            elif style == 2:
-                result.append(style_ticket.Creat(key,self.translateLang,art,hide_uid,uid, self.seeleland,self.remove_logo).start())
-
-        
-        result = await asyncio.gather(*result)'''
-            
-        
+                    
         response["card"] = result
         
         if self.lang == "ua":
             StarRailCard.UA_LANG = True
         else:
             StarRailCard.UA_LANG = False
```

### Comparing `starrailcard-2.1.5/starrailcard/src/api/api.py` & `starrailcard-2.1.6/starrailcard/src/api/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import aiohttp
 from typing import Optional
 
-from ..tools import http, translator, ukrainization
+from ..tools import http, translator, ukrainization, options
 from ..model import api_mihomo
 from .error import StarRailCardError
 from ..tools.json_data import JsonManager
 from ..tools.enums import PathData
 
 _API_MIHOMO: str = "https://api.mihomo.me/sr_info_parsed/{uid}"
 
 
 
 class ApiMiHoMo:
     """Class for interacting with the MiHoMo API."""
 
-    def __init__(self, uid: str, lang: str = "en", v: int = 2, force_update: bool = False) -> None:
+    def __init__(self, uid: str, lang: str = "en", v: int = 2, force_update: bool = False, user_agent: str = None, proxy = None) -> None:
         """Initialize the ApiMiHoMo object."""
         self.force_update: bool = force_update
         self.uid: str = uid
         self.lang: str = translator.SUPPORTED_LANGUAGES.get(lang, "en")
         self.ua_lang: str = lang == "en"
+        self.user_agent: str = options.get_user_agent(user_agent)
+        self.proxy: str = proxy
         api_mihomo.UA_LANG = False
         if lang == "ua":
             self.ua_lang = True
             api_mihomo.UA_LANG = True
             
         self.v = v
 
@@ -31,15 +33,20 @@
         """Get data from the MiHoMo API."""
         try:
             params = {
                 'lang': self.lang,
                 'is_force_update': str(self.force_update),
                 'version': f"v{self.v}"
             }
-            data = await http.AioSession.get(_API_MIHOMO.format(uid=self.uid), params=params)
+            
+            headers = {
+                "User-Agent": self.user_agent
+            }
+            
+            data = await http.AioSession.get(_API_MIHOMO.format(uid=self.uid), headers = headers, params=params, proxy= self.proxy)
             
             if data is None:
                 raise StarRailCardError(4, "Failed to get data from API, please try again")
             
             if 'detail' in data:
                 detail = data['detail']
                 if detail == 'User not found':
```

### Comparing `starrailcard-2.1.5/starrailcard/src/api/enka.py` & `starrailcard-2.1.6/starrailcard/src/api/enka.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/starrailcard/src/api/enka_parsed.py` & `starrailcard-2.1.6/starrailcard/src/api/enka_parsed.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/starrailcard/src/assets/font/font_hsr.ttf` & `starrailcard-2.1.6/starrailcard/src/assets/font/font_hsr.ttf`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/starrailcard/src/data/avatar.json` & `starrailcard-2.1.6/starrailcard/src/data/avatar.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/starrailcard/src/data/relict_sets.json` & `starrailcard-2.1.6/starrailcard/src/data/relict_sets.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/starrailcard/src/data/stats.json` & `starrailcard-2.1.6/starrailcard/src/data/stats.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/starrailcard/src/data/weapons.json` & `starrailcard-2.1.6/starrailcard/src/data/weapons.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/starrailcard/src/generator/style_profile_phone.py` & `starrailcard-2.1.6/starrailcard/src/generator/style_profile_phone.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,17 +30,17 @@
             background_image = await pill.get_dowload_img(self.background)
             background_image = await pill.get_centr_size((828,1078),background_image)
             background_shadow = Image.new("RGBA", (828, 1078), (0,0,0,150))
         background_image = background_image.convert("RGBA")
         background_image.alpha_composite(background_shadow)
         self.background_profile.paste(background_image,(0,0),maska.convert("L"))
         self.background_profile.alpha_composite(frame)
+        
 
     async def creat_charter(self,key):
-        
         if key.rarity == 5:
             charter_profile = await _of.avatar_five
         else:
             charter_profile = await _of.avatar_four
         
         charter_profile = charter_profile.copy()
         
@@ -51,30 +51,28 @@
                 url_id = f'https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/icon/avatar/{key.id}.png'
         else:
             url_id = f'https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/icon/avatar/{key.id}.png'
             
         splash,mask = await asyncio.gather(pill.get_dowload_img(url_id),_of.maska_character)
         splash = await pill.get_centr_size((109,109),splash)
         charter_profile.paste(splash,(16,28),mask.convert("L"))
-        
         name = await pill.create_image_with_text(key.name,16, max_width=123, color=(255, 255, 255, 255)) 
         
         charter_profile.alpha_composite(name,(136,int(49-name.size[1]/2)))       
 
         max_level = options.max_lvl(key.promotion)
         level = f"{self.lang.lvl}: {key.level}/{max_level}"
         
         element_icon = await pill.get_dowload_img(key.element.icon, size=(28,28))
         path_icon = await pill.get_dowload_img(key.path.icon, size=(28,28))
         
         charter_profile.alpha_composite(path_icon,(263,28))
         charter_profile.alpha_composite(element_icon,(293,28))
         
         
-        
         d = ImageDraw.Draw(charter_profile)
         d.text((19,7), level, font= self.font_charter, fill=(255,255,255,255))
         
         
         if not key.light_cone is None:
             icon = await pill.get_dowload_img(key.light_cone.icon, size = (66,66))
             charter_profile.alpha_composite(icon,(136,70))
@@ -88,22 +86,22 @@
             d = ImageDraw.Draw(background)
             font_12 = await pill.get_font(12)
             up = options.ups(key.light_cone.rank)
             x = int(font_12.getlength(str(up))/2)
             d.text((10-x, 4), up, font= font_12, fill=(255, 217, 144, 255))
             
             charter_profile.alpha_composite(background.resize((17,17)), (202,114))
-        
+            
         return charter_profile
     
     async def get_charter(self):
         task = []
         for key in self.profile.characters:
             task.append(self.creat_charter(key))
-        
+            
         self.charter = await asyncio.gather(*task)
     
     async def creat_avatar(self):
         self.background_profile_avatar = Image.new("RGBA", (625, 254), (0,0,0,0))
         avatar = self.profile.player.avatar.icon
             
         avatar,font_20,desc_frame = await asyncio.gather(pill.get_dowload_img(avatar, size= (134,134)),pill.get_font(18),_of.desc_frame)
@@ -126,33 +124,30 @@
                 
         signature = await pill.create_image_with_text(self.profile.player.signature, 18, max_width=606, color=(255, 255, 255, 255))
         self.background_profile_avatar.alpha_composite(desc_frame,(0,163))
         self.background_profile_avatar.alpha_composite(signature,(int(320-signature.size[0]/2),int(199-signature.size[1]/2)))
         
     
     async def build(self):
-        
         self.background_profile.alpha_composite(self.background_profile_avatar,(29,53))
 
         x,y = 0,407  
         for i, key in enumerate(self.charter):
             self.background_profile.alpha_composite(key,(x,y))
             y += 155
             if i == 3:
                 x = 338
                 y = 407
                 
         if not self.remove_logo:
             logo = await _of.LOGO_GIT_INV
             self.background_profile.alpha_composite(logo,(752,0))
-
                 
     async def start(self):
         
         _of.set_mapping(3)
-        
         self.font_charter = await pill.get_font(13)
         
         await asyncio.gather(self.creat_background(), self.get_charter(), self.creat_avatar())
         await self.build()        
         
         return self.background_profile
```

### Comparing `starrailcard-2.1.5/starrailcard/src/generator/style_relict_score.py` & `starrailcard-2.1.6/starrailcard/src/generator/style_relict_score.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/starrailcard/src/generator/style_ticket.py` & `starrailcard-2.1.6/starrailcard/src/generator/style_ticket.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/starrailcard/src/model/api_mihomo.py` & `starrailcard-2.1.6/starrailcard/src/model/api_mihomo.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/starrailcard/src/model/StarRailCard.py` & `starrailcard-2.1.6/starrailcard/src/model/StarRailCard.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/starrailcard/src/model/style.py` & `starrailcard-2.1.6/starrailcard/src/model/style.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/starrailcard/src/model/utils_model.py` & `starrailcard-2.1.6/starrailcard/src/model/utils_model.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/starrailcard/src/tools/calculator/src/assets/rolls.json` & `starrailcard-2.1.6/starrailcard/src/tools/calculator/src/assets/rolls.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/starrailcard/src/tools/calculator/src/assets/score.json` & `starrailcard-2.1.6/starrailcard/src/tools/calculator/src/assets/score.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/starrailcard/src/tools/calculator/src/utils.py` & `starrailcard-2.1.6/starrailcard/src/tools/calculator/src/utils.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/starrailcard/src/tools/calculator/stats.py` & `starrailcard-2.1.6/starrailcard/src/tools/calculator/stats.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/starrailcard/src/tools/cashe.py` & `starrailcard-2.1.6/starrailcard/src/tools/cashe.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/starrailcard/src/tools/enums.py` & `starrailcard-2.1.6/starrailcard/src/tools/enums.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/starrailcard/src/tools/git.py` & `starrailcard-2.1.6/starrailcard/src/tools/git.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/starrailcard/src/tools/http.py` & `starrailcard-2.1.6/starrailcard/src/tools/http.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,17 +121,20 @@
         
         return result
 
 
 
 class AioSession:
     session = SharedObject(aiohttp.ClientSession)
-
+    proxy = None
+    
     @classmethod
-    async def enter(cls, /):
+    async def enter(cls, proxy = None, /):
+        cls.proxy = proxy
+        
         return await cls.session.__aenter__()
     
     @classmethod
     async def exit(cls, /, *exc_info):
         if not exc_info:
             exc_info = (None, None, None)
         
@@ -175,15 +178,15 @@
 
         Returns:
             aiohttp.ClientSession: The current session instance, or None if the session is not created.
         """
         return cls.session'''
 
     @classmethod
-    async def get(cls, url, headers=None, response_format='json', **kwargs):
+    async def get(cls, url, headers=None, response_format='json', proxy=None, **kwargs):
         """
         Sends a GET request using the current session instance.
 
         Args:
             url (str): The URL to send the request to.
             headers (dict): Optional headers to include in the request.
             response_format (str): The format of the response data to return.
@@ -192,28 +195,27 @@
         Returns:
             Depends on the specified response format:
             - dict: for 'json' format;
             - str: for 'text' format;
             - bytes: for 'bytes' format.
         """
         async with cls.session as session:
+            if not cls.proxy is None:
+                proxy = cls.proxy
+                
             try:
-                async with cls.session as session:
-                    response = await session.get(url, headers=headers, **kwargs)   
-                                                            
+                async with session.get(url, headers=headers, proxy=proxy, **kwargs) as response:
                     data = await cls.process_response(response, response_format)
-                    
                     return data
-                
             except Exception as e:
                 print(f"Error during GET request: {e}")
 
 
     @classmethod
-    async def post(cls, url, data=None, headers=None, response_format='json', **kwargs):
+    async def post(cls, url, data=None, headers=None, response_format='json', proxy=None, **kwargs):
         """
         Sends a POST request using the current session instance.
 
         Args:
             url (str): The URL to send the request to.
             data: The data to send in the request body.
             headers (dict): Optional headers to include in the request.
@@ -222,28 +224,27 @@
 
         Returns:
             Depends on the specified response format:
             - dict: for 'json' format;
             - str: for 'text' format;
             - bytes: for 'bytes' format.
         """
+        if not cls.proxy is None:
+            proxy = cls.proxy
+                
         async with cls.session as session:
             try:
-                async with cls.session as session:
-                    response = await session.post(url, headers=headers, **kwargs)   
-                                                            
+                async with session.post(url, data=data, headers=headers, proxy=proxy, **kwargs) as response:
                     data = await cls.process_response(response, response_format)
-                    
                     return data
-                
             except Exception as e:
                 print(f"Error during POST request: {e}")
 
     @classmethod
-    async def request(cls, method, url, headers=None, response_format='json', **kwargs):
+    async def request(cls, method, url, headers=None, response_format='json', proxy=None, **kwargs):
         """
         Sends a custom HTTP request using the current session instance.
 
         Args:
             method (str): The HTTP method to use (e.g., 'GET', 'POST').
             url (str): The URL to send the request to.
             headers (dict): Optional headers to include in the request.
@@ -252,24 +253,22 @@
 
         Returns:
             Depends on the specified response format:
             - dict: for 'json' format;
             - str: for 'text' format;
             - bytes: for 'bytes' format.
         """
-        
+        if not cls.proxy is None:
+            proxy = cls.proxy
+            
         async with cls.session as session:
             try:
-                async with cls.session as session:
-                    response = await session.request(method, url, headers=headers, **kwargs)   
-                                                            
+                async with session.request(method, url, headers=headers, proxy=proxy, **kwargs) as response:
                     data = await cls.process_response(response, response_format)
-                    
                     return data
-                
             except Exception as e:
                 print(f"Error during custom request: {e}")
    
     
     @classmethod
     async def process_response(cls, response, response_format):
         """
```

### Comparing `starrailcard-2.1.5/starrailcard/src/tools/json_data.py` & `starrailcard-2.1.6/starrailcard/src/tools/json_data.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/starrailcard/src/tools/options.py` & `starrailcard-2.1.6/starrailcard/src/tools/options.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,39 @@
 # Copyright 2024 DEViantUa <t.me/deviant_ua>
 # All rights reserved.
-
 import random
 import aiofiles
 import io
 from PIL import Image
 import os
+import sys
 import datetime
 
 from .git import ImageCache
 from .http import AioSession
+from ... import __version__
 
 _git = ImageCache()
 
+def get_user_agent(user_agent):
+    python_version = sys.version_info
+    
+    if not user_agent is None:
+        if user_agent == "StarRailCard/{version} (Python {major}.{minor}.{micro})".format(version=__version__,major=python_version.major,minor=python_version.minor,micro=python_version.micro):
+            return user_agent
+        
+        return f"StarRailCad/{__version__}: {user_agent}"
+    
+    return "StarRailCard/{version} (Python {major}.{minor}.{micro})".format(
+        version=__version__,
+        major=python_version.major,
+        minor=python_version.minor,
+        micro=python_version.micro
+    )
+
 _DEFAULT_SCORE = {'count': 0, 
                   'rolls': {}, 
                   'rank': {'name': 'N/A', 
                            'color': (255, 255, 255, 255)
                     }
 }
```

### Comparing `starrailcard-2.1.5/starrailcard/src/tools/pill/color.py` & `starrailcard-2.1.6/starrailcard/src/tools/pill/color.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/starrailcard/src/tools/pill/color_controle.py` & `starrailcard-2.1.6/starrailcard/src/tools/pill/color_controle.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/starrailcard/src/tools/pill/grandiend_v2.py` & `starrailcard-2.1.6/starrailcard/src/tools/pill/grandiend_v2.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/starrailcard/src/tools/pill/grandient_v1.py` & `starrailcard-2.1.6/starrailcard/src/tools/pill/grandient_v1.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/starrailcard/src/tools/pill/style_editor.py` & `starrailcard-2.1.6/starrailcard/src/tools/pill/style_editor.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/starrailcard/src/tools/pill/text_controle.py` & `starrailcard-2.1.6/starrailcard/src/tools/pill/text_controle.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/starrailcard/src/tools/translator.py` & `starrailcard-2.1.6/starrailcard/src/tools/translator.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/starrailcard/src/tools/treePaths.py` & `starrailcard-2.1.6/starrailcard/src/tools/treePaths.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/starrailcard/src/tools/ukrainization.py` & `starrailcard-2.1.6/starrailcard/src/tools/ukrainization.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/starrailcard/utils.py` & `starrailcard-2.1.6/starrailcard/utils.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.5/PKG-INFO` & `starrailcard-2.1.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,107 +1,103 @@
-Metadata-Version: 2.1
-Name: starrailcard
-Version: 2.1.5
-Summary: This Python module provides the ability to create captivating character cards based on player data from Honkai Star Rail, obtained through their unique user identifiers (UIDs). StarRailCard streamlines the process of generating personalized character assembly cards, relying on the information provided by players.
-Home-page: https://github.com/DEViantUA/StarRailCard
-License: MIT License with Additional Restrictions
-Keywords: honkai,cards,generation,honkaistarraill,raill,starraill,builds,honkairail,honkai
-Author: DEViantUA
-Author-email: deviantapi@gmail.com
-Requires-Python: >=3.9,<4.0
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Pillow
-Requires-Dist: aiofiles
-Requires-Dist: aiohttp
-Requires-Dist: anyio
-Requires-Dist: beautifulsoup4
-Requires-Dist: cachetools
-Requires-Dist: imageio
-Requires-Dist: more-itertools
-Requires-Dist: moviepy
-Requires-Dist: numpy
-Requires-Dist: pydantic
-Project-URL: Repository, https://github.com/DEViantUA/StarRailCard
-Description-Content-Type: text/markdown
-
-<p align="center">
- <img src="https://raw.githubusercontent.com/DEViantUA/StarRailCard/main/Examples/image/starRailCardBanner.png" alt="Баннер"/>
-</p>
-
-## StarRailCard
-<details>
-  <summary>
-   Description:
-  </summary>
-<br>
-Welcome to the world of StarRailCard – your magical guide to the universe of Honkai Star Rail! This Python module provides the ability to create captivating character cards based on player data from Honkai Star Rail, obtained through their unique user identifiers (UIDs). StarRailCard streamlines the process of generating personalized character assembly cards, relying on the information provided by players.
- 
----
- 
-* **Easy Installation:** Set up StarRailCard in just a few simple steps to start using it without any hassle.
-* **Support for Other Programming Languages:** StarRailCard provides support for multiple programming languages, making it accessible to a wide range of developers.
-* **Color Adaptation:** StarRailCard seamlessly adapts its color scheme to match the user's custom images, ensuring a harmonious blend between character cards and background images.
-* **Flexible Configuration:** Customize StarRailCard according to your preferences with flexible configuration options, allowing you to tailor the generation process to your liking.
-* **Multi-Language Support:** With support for all languages available in the game, including Ukrainian, StarRailCard can generate character cards in any language.
-* **Personalized Character Cards:** Create character assembly cards based on specific player data to highlight their uniqueness and individuality.
-* **Animation Support:** StarRailCard supports animated elements, adding extra vitality and dynamism to character cards.
-* **Custom Fonts and Images:** Use custom fonts and character images to create character cards with a unique style.
-* **Instant Data Update and Retrieval:** Get updated character and player profile data instantly, ensuring the information on cards is always up-to-date.
-* **Integration with MiHoMo API Wrapper:** Seamlessly integrate StarRailCard with the MiHoMo API wrapper for quick access to game and character data.
-</details>
-
-* [Documentation](https://github.com/DEViantUA/StarRailCard/wiki/Documentation)
-* [View cards](https://github.com/DEViantUA/StarRailCard/wiki/View-cards)
-* [API](https://github.com/DEViantUA/StarRailCard/wiki/StarRailCard-API)
-* [Languages-Supported](https://github.com/DEViantUA/StarRailCard/wiki/Languages-Supported)
-* [F.A.Q.](https://github.com/DEViantUA/StarRailCard/wiki/F.A.Q.)
-* [PyPi](https://pypi.org/project/starrailcard/)
-* [Telegram](https://t.me/enkacardchat)
-* [Patreon](https://www.patreon.com/deviantapi)
-* [GitHub](https://github.com/DEViantUA/StarRailCard)
-
-### Api:
-> You can use the API to generate cards if you are using a different programming language.
-[Documentation](https://github.com/DEViantUA/StarRailCard/wiki/StarRailCard-API)
-
-## Installation:
-```
-pip install starrailcard
-```
-
-## Launch:
-``` python
-import asyncio
-import starrailcard
-
-async def main():
-    async with starrailcard.Card() as card:
-        data = await card.creat(700649319, style=2)
-    print(data)
-
-asyncio.run(main())
-```
-
-<details>
-<summary>Create a profile card.</summary>
-
-``` python
-import asyncio
-import starrailcard
-
-async def main():
-    async with starrailcard.Card() as card:
-        data = await card.creat_profile(700649319)
-    print(data)
-
-asyncio.run(main())
-```
-</details>
-
-# Thank the author for the code: 
-* **Patreon**: https://www.patreon.com/deviantapi
-* **Ko-Fi**: https://ko-fi.com/dezzso
-
+Metadata-Version: 2.1
+Name: starrailcard
+Version: 2.1.6
+Summary: This Python module provides the ability to create captivating character cards based on player data from Honkai Star Rail, obtained through their unique user identifiers (UIDs). StarRailCard streamlines the process of generating personalized character assembly cards, relying on the information provided by players.
+Home-page: https://github.com/DEViantUA/StarRailCard
+Author: DeviantUa
+Author-email: deviantapi@gmail.com
+Keywords: honkai,cards,generation,honkaistarraill,raill,starraill,builds,honkairail,honkai
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pydantic
+Requires-Dist: aiohttp
+Requires-Dist: cachetools
+Requires-Dist: Pillow
+Requires-Dist: aiofiles
+Requires-Dist: imageio
+Requires-Dist: moviepy
+Requires-Dist: more-itertools
+Requires-Dist: numpy
+Requires-Dist: beautifulsoup4
+Requires-Dist: anyio
+
+<p align="center">
+ <img src="https://raw.githubusercontent.com/DEViantUA/StarRailCard/main/Examples/image/starRailCardBanner.png" alt="Баннер"/>
+</p>
+
+## StarRailCard
+<details>
+  <summary>
+   Description:
+  </summary>
+<br>
+Welcome to the world of StarRailCard – your magical guide to the universe of Honkai Star Rail! This Python module provides the ability to create captivating character cards based on player data from Honkai Star Rail, obtained through their unique user identifiers (UIDs). StarRailCard streamlines the process of generating personalized character assembly cards, relying on the information provided by players.
+ 
+---
+ 
+* **Easy Installation:** Set up StarRailCard in just a few simple steps to start using it without any hassle.
+* **Support for Other Programming Languages:** StarRailCard provides support for multiple programming languages, making it accessible to a wide range of developers.
+* **Color Adaptation:** StarRailCard seamlessly adapts its color scheme to match the user's custom images, ensuring a harmonious blend between character cards and background images.
+* **Flexible Configuration:** Customize StarRailCard according to your preferences with flexible configuration options, allowing you to tailor the generation process to your liking.
+* **Multi-Language Support:** With support for all languages available in the game, including Ukrainian, StarRailCard can generate character cards in any language.
+* **Personalized Character Cards:** Create character assembly cards based on specific player data to highlight their uniqueness and individuality.
+* **Animation Support:** StarRailCard supports animated elements, adding extra vitality and dynamism to character cards.
+* **Custom Fonts and Images:** Use custom fonts and character images to create character cards with a unique style.
+* **Instant Data Update and Retrieval:** Get updated character and player profile data instantly, ensuring the information on cards is always up-to-date.
+* **Integration with MiHoMo API Wrapper:** Seamlessly integrate StarRailCard with the MiHoMo API wrapper for quick access to game and character data.
+</details>
+
+* [Documentation](https://github.com/DEViantUA/StarRailCard/wiki/Documentation)
+* [View cards](https://github.com/DEViantUA/StarRailCard/wiki/View-cards)
+* [API](https://github.com/DEViantUA/StarRailCard/wiki/StarRailCard-API)
+* [Languages-Supported](https://github.com/DEViantUA/StarRailCard/wiki/Languages-Supported)
+* [F.A.Q.](https://github.com/DEViantUA/StarRailCard/wiki/F.A.Q.)
+* [PyPi](https://pypi.org/project/starrailcard/)
+* [Telegram](https://t.me/enkacardchat)
+* [Patreon](https://www.patreon.com/deviantapi)
+* [GitHub](https://github.com/DEViantUA/StarRailCard)
+
+### Api:
+> You can use the API to generate cards if you are using a different programming language.
+[Documentation](https://github.com/DEViantUA/StarRailCard/wiki/StarRailCard-API)
+
+## Installation:
+```
+pip install starrailcard
+```
+
+## Launch:
+``` python
+import asyncio
+import starrailcard
+
+async def main():
+    async with starrailcard.Card() as card:
+        data = await card.creat(700649319, style=2)
+    print(data)
+
+asyncio.run(main())
+```
+
+<details>
+<summary>Create a profile card.</summary>
+
+``` python
+import asyncio
+import starrailcard
+
+async def main():
+    async with starrailcard.Card() as card:
+        data = await card.creat_profile(700649319)
+    print(data)
+
+asyncio.run(main())
+```
+</details>
+
+# Thank the author for the code: 
+* **Patreon**: https://www.patreon.com/deviantapi
+* **Ko-Fi**: https://ko-fi.com/dezzso
```

