# Comparing `tmp/valorant.py-1.0.6.tar.gz` & `tmp/valorant_py-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valorant.py-1.0.6.tar", last modified: Thu Aug 17 12:22:49 2023, max compression
+gzip compressed data, was "valorant_py-1.0.8.tar", last modified: Tue Apr 30 13:32:00 2024, max compression
```

## Comparing `valorant.py-1.0.6.tar` & `valorant_py-1.0.8.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 12:22:49.493676 valorant.py-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-17 12:22:36.000000 valorant.py-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-17 12:22:36.000000 valorant.py-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-08-17 12:22:49.493676 valorant.py-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-08-17 12:22:36.000000 valorant.py-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-08-17 12:22:36.000000 valorant.py-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-17 12:22:36.000000 valorant.py-1.0.6/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-17 12:22:36.000000 valorant.py-1.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-17 12:22:49.493676 valorant.py-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-08-17 12:22:36.000000 valorant.py-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 12:22:49.481675 valorant.py-1.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-17 12:22:36.000000 valorant.py-1.0.6/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25850 2023-08-17 12:22:36.000000 valorant.py-1.0.6/tests/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 12:22:49.481675 valorant.py-1.0.6/valorant/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    28199 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    14964 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    17931 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/localization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 12:22:49.489676 valorant.py-1.0.6/valorant/models/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/models/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/models/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/models/buddies.py
--rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/models/bundles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/models/ceremonies.py
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/models/competitive_tiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/models/content_tiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/models/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/models/currencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/models/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/models/gamemodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/models/gear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/models/level_borders.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/models/maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/models/missions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/models/player_cards.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/models/player_titles.py
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/models/seasons.py
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/models/sprays.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/models/themes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/models/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    20326 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/models/weapons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 12:22:49.493676 valorant.py-1.0.6/valorant/types/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/types/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/types/buddies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/types/bundles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/types/ceremonies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/types/competitive_tiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/types/content_tiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/types/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/types/currencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/types/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/types/gamemodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/types/gear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/types/level_borders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/types/maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/types/missions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/types/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/types/player_cards.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/types/player_titles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/types/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/types/seasons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/types/sprays.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/types/themes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/types/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/types/weapons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-08-17 12:22:36.000000 valorant.py-1.0.6/valorant/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-17 12:22:49.485676 valorant.py-1.0.6/valorant.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-08-17 12:22:49.000000 valorant.py-1.0.6/valorant.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-08-17 12:22:49.000000 valorant.py-1.0.6/valorant.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-17 12:22:49.000000 valorant.py-1.0.6/valorant.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-17 12:22:49.000000 valorant.py-1.0.6/valorant.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-17 12:22:49.000000 valorant.py-1.0.6/valorant.py.egg-info/top_level.txt
+drwxr-xr-x   0 deemc      (501) staff       (20)        0 2024-04-30 13:32:00.819507 valorant_py-1.0.8/
+-rw-r--r--   0 deemc      (501) staff       (20)     1063 2024-04-30 12:20:43.000000 valorant_py-1.0.8/LICENSE
+-rw-r--r--   0 deemc      (501) staff       (20)       87 2024-04-30 12:20:43.000000 valorant_py-1.0.8/MANIFEST.in
+-rw-r--r--   0 deemc      (501) staff       (20)     4090 2024-04-30 13:32:00.819030 valorant_py-1.0.8/PKG-INFO
+-rw-r--r--   0 deemc      (501) staff       (20)     1853 2024-04-30 12:20:43.000000 valorant_py-1.0.8/README.md
+-rw-r--r--   0 deemc      (501) staff       (20)     2656 2024-04-30 13:31:48.000000 valorant_py-1.0.8/pyproject.toml
+-rw-r--r--   0 deemc      (501) staff       (20)       67 2024-04-30 12:20:43.000000 valorant_py-1.0.8/requirements-dev.txt
+-rw-r--r--   0 deemc      (501) staff       (20)       17 2024-04-30 12:20:43.000000 valorant_py-1.0.8/requirements.txt
+-rw-r--r--   0 deemc      (501) staff       (20)       38 2024-04-30 13:32:00.819603 valorant_py-1.0.8/setup.cfg
+-rw-r--r--   0 deemc      (501) staff       (20)      234 2024-04-30 13:26:18.000000 valorant_py-1.0.8/setup.py
+drwxr-xr-x   0 deemc      (501) staff       (20)        0 2024-04-30 13:32:00.775683 valorant_py-1.0.8/tests/
+-rw-r--r--   0 deemc      (501) staff       (20)     1147 2024-04-30 12:20:43.000000 valorant_py-1.0.8/tests/test_client.py
+-rw-r--r--   0 deemc      (501) staff       (20)    25899 2024-04-30 12:20:43.000000 valorant_py-1.0.8/tests/test_models.py
+drwxr-xr-x   0 deemc      (501) staff       (20)        0 2024-04-30 13:32:00.781848 valorant_py-1.0.8/valorant/
+-rw-r--r--   0 deemc      (501) staff       (20)     2482 2024-04-30 13:01:34.000000 valorant_py-1.0.8/valorant/__init__.py
+-rw-r--r--   0 deemc      (501) staff       (20)     6432 2024-04-30 12:24:32.000000 valorant_py-1.0.8/valorant/asset.py
+-rw-r--r--   0 deemc      (501) staff       (20)    28199 2024-04-30 12:24:38.000000 valorant_py-1.0.8/valorant/cache.py
+-rw-r--r--   0 deemc      (501) staff       (20)    15050 2024-04-30 12:55:37.000000 valorant_py-1.0.8/valorant/client.py
+-rw-r--r--   0 deemc      (501) staff       (20)     8498 2024-04-30 12:20:43.000000 valorant_py-1.0.8/valorant/enums.py
+-rw-r--r--   0 deemc      (501) staff       (20)     3338 2024-04-30 12:55:39.000000 valorant_py-1.0.8/valorant/errors.py
+-rw-r--r--   0 deemc      (501) staff       (20)     4133 2024-04-30 12:24:34.000000 valorant_py-1.0.8/valorant/file.py
+-rw-r--r--   0 deemc      (501) staff       (20)    16422 2024-04-30 12:55:38.000000 valorant_py-1.0.8/valorant/http.py
+-rw-r--r--   0 deemc      (501) staff       (20)     7985 2024-04-30 12:20:43.000000 valorant_py-1.0.8/valorant/localization.py
+drwxr-xr-x   0 deemc      (501) staff       (20)        0 2024-04-30 13:32:00.799529 valorant_py-1.0.8/valorant/models/
+-rw-r--r--   0 deemc      (501) staff       (20)     2048 2024-04-30 12:57:09.000000 valorant_py-1.0.8/valorant/models/__init__.py
+-rw-r--r--   0 deemc      (501) staff       (20)    20303 2024-04-30 12:55:36.000000 valorant_py-1.0.8/valorant/models/agents.py
+-rw-r--r--   0 deemc      (501) staff       (20)     5071 2024-04-30 12:55:22.000000 valorant_py-1.0.8/valorant/models/base.py
+-rw-r--r--   0 deemc      (501) staff       (20)     4872 2024-04-30 12:55:35.000000 valorant_py-1.0.8/valorant/models/buddies.py
+-rw-r--r--   0 deemc      (501) staff       (20)     7845 2024-04-30 12:55:35.000000 valorant_py-1.0.8/valorant/models/bundles.py
+-rw-r--r--   0 deemc      (501) staff       (20)     2354 2024-04-30 12:55:34.000000 valorant_py-1.0.8/valorant/models/ceremonies.py
+-rw-r--r--   0 deemc      (501) staff       (20)     6050 2024-04-30 12:55:34.000000 valorant_py-1.0.8/valorant/models/competitive_tiers.py
+-rw-r--r--   0 deemc      (501) staff       (20)     3119 2024-04-30 12:55:32.000000 valorant_py-1.0.8/valorant/models/content_tiers.py
+-rw-r--r--   0 deemc      (501) staff       (20)     8447 2024-04-30 12:55:31.000000 valorant_py-1.0.8/valorant/models/contracts.py
+-rw-r--r--   0 deemc      (501) staff       (20)     3635 2024-04-30 12:55:31.000000 valorant_py-1.0.8/valorant/models/currencies.py
+-rw-r--r--   0 deemc      (501) staff       (20)     3442 2024-04-30 12:55:31.000000 valorant_py-1.0.8/valorant/models/events.py
+-rw-r--r--   0 deemc      (501) staff       (20)     7389 2024-04-30 12:55:30.000000 valorant_py-1.0.8/valorant/models/gamemodes.py
+-rw-r--r--   0 deemc      (501) staff       (20)     3170 2024-04-30 12:55:30.000000 valorant_py-1.0.8/valorant/models/gear.py
+-rw-r--r--   0 deemc      (501) staff       (20)     2995 2024-04-30 13:00:24.000000 valorant_py-1.0.8/valorant/models/level_borders.py
+-rw-r--r--   0 deemc      (501) staff       (20)     6141 2024-04-30 12:55:29.000000 valorant_py-1.0.8/valorant/models/maps.py
+-rw-r--r--   0 deemc      (501) staff       (20)     5291 2024-04-30 12:55:28.000000 valorant_py-1.0.8/valorant/models/missions.py
+-rw-r--r--   0 deemc      (501) staff       (20)     4185 2024-04-30 12:55:28.000000 valorant_py-1.0.8/valorant/models/player_cards.py
+-rw-r--r--   0 deemc      (501) staff       (20)     3147 2024-04-30 12:55:28.000000 valorant_py-1.0.8/valorant/models/player_titles.py
+-rw-r--r--   0 deemc      (501) staff       (20)     6776 2024-04-30 12:55:27.000000 valorant_py-1.0.8/valorant/models/seasons.py
+-rw-r--r--   0 deemc      (501) staff       (20)     6104 2024-04-30 12:55:27.000000 valorant_py-1.0.8/valorant/models/sprays.py
+-rw-r--r--   0 deemc      (501) staff       (20)     3045 2024-04-30 12:55:26.000000 valorant_py-1.0.8/valorant/models/themes.py
+-rw-r--r--   0 deemc      (501) staff       (20)     3001 2024-04-30 12:20:43.000000 valorant_py-1.0.8/valorant/models/version.py
+-rw-r--r--   0 deemc      (501) staff       (20)    20327 2024-04-30 12:55:25.000000 valorant_py-1.0.8/valorant/models/weapons.py
+drwxr-xr-x   0 deemc      (501) staff       (20)        0 2024-04-30 13:32:00.817819 valorant_py-1.0.8/valorant/types/
+-rw-r--r--   0 deemc      (501) staff       (20)      151 2024-04-30 12:20:43.000000 valorant_py-1.0.8/valorant/types/__init__.py
+-rw-r--r--   0 deemc      (501) staff       (20)     2402 2024-04-30 12:20:43.000000 valorant_py-1.0.8/valorant/types/agents.py
+-rw-r--r--   0 deemc      (501) staff       (20)     1662 2024-04-30 12:20:43.000000 valorant_py-1.0.8/valorant/types/buddies.py
+-rw-r--r--   0 deemc      (501) staff       (20)     1693 2024-04-30 12:20:43.000000 valorant_py-1.0.8/valorant/types/bundles.py
+-rw-r--r--   0 deemc      (501) staff       (20)     1349 2024-04-30 12:20:43.000000 valorant_py-1.0.8/valorant/types/ceremonies.py
+-rw-r--r--   0 deemc      (501) staff       (20)     1726 2024-04-30 12:20:43.000000 valorant_py-1.0.8/valorant/types/competitive_tiers.py
+-rw-r--r--   0 deemc      (501) staff       (20)     1478 2024-04-30 12:20:43.000000 valorant_py-1.0.8/valorant/types/content_tiers.py
+-rw-r--r--   0 deemc      (501) staff       (20)     2004 2024-04-30 12:20:43.000000 valorant_py-1.0.8/valorant/types/contracts.py
+-rw-r--r--   0 deemc      (501) staff       (20)     1441 2024-04-30 12:20:43.000000 valorant_py-1.0.8/valorant/types/currencies.py
+-rw-r--r--   0 deemc      (501) staff       (20)     1418 2024-04-30 12:20:43.000000 valorant_py-1.0.8/valorant/types/events.py
+-rw-r--r--   0 deemc      (501) staff       (20)     2138 2024-04-30 12:20:43.000000 valorant_py-1.0.8/valorant/types/gamemodes.py
+-rw-r--r--   0 deemc      (501) staff       (20)     1428 2024-04-30 12:20:43.000000 valorant_py-1.0.8/valorant/types/gear.py
+-rw-r--r--   0 deemc      (501) staff       (20)     1395 2024-04-30 12:20:43.000000 valorant_py-1.0.8/valorant/types/level_borders.py
+-rw-r--r--   0 deemc      (501) staff       (20)     1792 2024-04-30 12:20:43.000000 valorant_py-1.0.8/valorant/types/maps.py
+-rw-r--r--   0 deemc      (501) staff       (20)     1679 2024-04-30 12:20:43.000000 valorant_py-1.0.8/valorant/types/missions.py
+-rw-r--r--   0 deemc      (501) staff       (20)     1466 2024-04-30 12:20:43.000000 valorant_py-1.0.8/valorant/types/object.py
+-rw-r--r--   0 deemc      (501) staff       (20)     1500 2024-04-30 12:20:43.000000 valorant_py-1.0.8/valorant/types/player_cards.py
+-rw-r--r--   0 deemc      (501) staff       (20)     1434 2024-04-30 12:20:43.000000 valorant_py-1.0.8/valorant/types/player_titles.py
+-rw-r--r--   0 deemc      (501) staff       (20)     1224 2024-04-30 12:20:43.000000 valorant_py-1.0.8/valorant/types/response.py
+-rw-r--r--   0 deemc      (501) staff       (20)     1843 2024-04-30 12:20:43.000000 valorant_py-1.0.8/valorant/types/seasons.py
+-rw-r--r--   0 deemc      (501) staff       (20)     1823 2024-04-30 12:20:43.000000 valorant_py-1.0.8/valorant/types/sprays.py
+-rw-r--r--   0 deemc      (501) staff       (20)     1412 2024-04-30 12:20:43.000000 valorant_py-1.0.8/valorant/types/themes.py
+-rw-r--r--   0 deemc      (501) staff       (20)     1380 2024-04-30 12:20:43.000000 valorant_py-1.0.8/valorant/types/version.py
+-rw-r--r--   0 deemc      (501) staff       (20)     3339 2024-04-30 12:20:43.000000 valorant_py-1.0.8/valorant/types/weapons.py
+-rw-r--r--   0 deemc      (501) staff       (20)     2710 2024-04-30 12:55:38.000000 valorant_py-1.0.8/valorant/utils.py
+drwxr-xr-x   0 deemc      (501) staff       (20)        0 2024-04-30 13:32:00.818372 valorant_py-1.0.8/valorant.py.egg-info/
+-rw-r--r--   0 deemc      (501) staff       (20)     4090 2024-04-30 13:32:00.000000 valorant_py-1.0.8/valorant.py.egg-info/PKG-INFO
+-rw-r--r--   0 deemc      (501) staff       (20)     1809 2024-04-30 13:32:00.000000 valorant_py-1.0.8/valorant.py.egg-info/SOURCES.txt
+-rw-r--r--   0 deemc      (501) staff       (20)        1 2024-04-30 13:32:00.000000 valorant_py-1.0.8/valorant.py.egg-info/dependency_links.txt
+-rw-r--r--   0 deemc      (501) staff       (20)       18 2024-04-30 13:32:00.000000 valorant_py-1.0.8/valorant.py.egg-info/requires.txt
+-rw-r--r--   0 deemc      (501) staff       (20)        9 2024-04-30 13:32:00.000000 valorant_py-1.0.8/valorant.py.egg-info/top_level.txt
```

### Comparing `valorant.py-1.0.6/LICENSE` & `valorant_py-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.6/README.md` & `valorant_py-1.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -53,16 +53,16 @@
 asyncio.run(main())
 ```
 
 
 ## License
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
 
-## Project inspired by
-- [discord.py](https://github.com/Rapptz/discord.py) the Discord API wrapper for Python. 
+<!-- ## Project inspired by
+- [discord.py](https://github.com/Rapptz/discord.py) the Discord API wrapper for Python.  -->
 
 <!-- ## Support
 - [Discord Server](https://discord.com/invite/) -->
 
 ## Links
 - [Valorant API](https://valorant-api.com)
 - [Official Discord Server](https://discord.com/invite/9V5MWgD)
```

### Comparing `valorant.py-1.0.6/tests/test_client.py` & `valorant_py-1.0.8/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.6/tests/test_models.py` & `valorant_py-1.0.8/tests/test_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,28 +44,28 @@
                 assert ability.slot is not None
                 assert isinstance(ability.slot, AbilitySlot)
                 assert ability.display_name is not None
                 assert ability.description is not None
                 if ability.display_icon:
                     assert ability.display_icon is not None
 
-            assert agent.voice_line_localization is not None
-            voice_line = agent.voice_line
-            if voice_line is not None:
-                assert agent.voice_line_localization.voice_locale == voice_line
-                for voice in agent.voice_line_localization.all():
-                    assert voice is not None
-                    assert voice.min_duration is not None
-                    assert voice.max_duration is not None
-                    assert voice.media_list is not None
-                    for media in voice.media_list:
-                        assert media is not None
-                        assert media.id is not None
-                        assert media.wwise is not None
-                        assert media.wave is not None
+            if agent.voice_line_localization is not None:
+                voice_line = agent.voice_line
+                if voice_line is not None:
+                    assert agent.voice_line_localization.voice_locale == voice_line
+                    for voice in agent.voice_line_localization.all():
+                        assert voice is not None
+                        assert voice.min_duration is not None
+                        assert voice.max_duration is not None
+                        assert voice.media_list is not None
+                        for media in voice.media_list:
+                            assert media is not None
+                            assert media.id is not None
+                            assert media.wwise is not None
+                            assert media.wave is not None
 
     @pytest.mark.asyncio
     async def test_buddies(self) -> None:
         assert len(self.client.buddies) > 0
         for buddy in self.client.buddies:
             assert buddy is not None
             # fbuddy = await self.client.fetch_buddy(buddy.uuid)
```

### Comparing `valorant.py-1.0.6/valorant/asset.py` & `valorant_py-1.0.8/valorant/asset.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,34 +18,34 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
-
 # source : https://github.com/Rapptz/discord.py/blob/master/discord/asset.py
 from __future__ import annotations
 
 import io
-import os
 from typing import TYPE_CHECKING, Any, Optional, Tuple, Union
 
 import yarl
 
 from . import utils
 from .file import File
 
 # fmt: off
 __all__ = (
     'Asset',
 )
 # fmt: on
 
 if TYPE_CHECKING:
+    import os
+
     from typing_extensions import Self
 
     from .cache import CacheState
 
 MISSING = utils.MISSING
 
 
@@ -137,15 +137,14 @@
         """
         data = await self.read()
         file_filename = filename if filename is not MISSING else yarl.URL(self.url).name
         return File(io.BytesIO(data), filename=file_filename)
 
 
 class Asset(AssetMixin):
-
     """Represents a CDN asset on Valorant.
     .. container:: operations
         .. describe:: str(x)
             Returns the URL of the CDN asset.
         .. describe:: len(x)
             Returns the length of the CDN asset's URL.
         .. describe:: x == y
```

### Comparing `valorant.py-1.0.6/valorant/cache.py` & `valorant_py-1.0.8/valorant/cache.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.6/valorant/client.py` & `valorant_py-1.0.8/valorant/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,55 +27,56 @@
 import asyncio
 import logging
 from typing import TYPE_CHECKING, List, Optional, Type
 
 from .cache import CacheState
 from .enums import Locale
 from .http import HTTPClient
-from .models.agents import Agent
-from .models.buddies import Buddy, BuddyLevel
-from .models.bundles import Bundle
-from .models.ceremonies import Ceremony
-from .models.competitive_tiers import CompetitiveTier
-from .models.content_tiers import ContentTier
-from .models.contracts import Contract
-from .models.currencies import Currency
-from .models.events import Event
-from .models.gamemodes import GameMode, GameModeEquippable
-from .models.gear import Gear
-from .models.level_borders import LevelBorder
-from .models.maps import Map
-from .models.missions import Mission
-from .models.player_cards import PlayerCard
-from .models.player_titles import PlayerTitle
-from .models.seasons import CompetitiveSeason, Season
-from .models.sprays import Spray, SprayLevel
-from .models.themes import Theme
-from .models.version import Version
-from .models.weapons import Skin, SkinChroma, SkinLevel, Weapon
 from .utils import MISSING
 
 if TYPE_CHECKING:
     from types import TracebackType
 
     from typing_extensions import Self
 
+    from .models.agents import Agent
+    from .models.buddies import Buddy, BuddyLevel
+    from .models.bundles import Bundle
+    from .models.ceremonies import Ceremony
+    from .models.competitive_tiers import CompetitiveTier
+    from .models.content_tiers import ContentTier
+    from .models.contracts import Contract
+    from .models.currencies import Currency
+    from .models.events import Event
+    from .models.gamemodes import GameMode, GameModeEquippable
+    from .models.gear import Gear
+    from .models.level_borders import LevelBorder
+    from .models.maps import Map
+    from .models.missions import Mission
+    from .models.player_cards import PlayerCard
+    from .models.player_titles import PlayerTitle
+    from .models.seasons import CompetitiveSeason, Season
+    from .models.sprays import Spray, SprayLevel
+    from .models.themes import Theme
+    from .models.version import Version
+    from .models.weapons import Skin, SkinChroma, SkinLevel, Weapon
+
 _log = logging.getLogger(__name__)
 
 # fmt: off
 __all__ = (
     'Client',
 )
 # fmt: on
 
 
 class Client:
     def __init__(
         self,
-        locale: Locale = Locale.american_english
+        locale: Locale = Locale.american_english,
         # *,
         # enable_cache: bool = True,
     ) -> None:
         self.locale: Locale = locale
         # self.enable_cache: bool = enable_cache
         self.http: HTTPClient = HTTPClient()
         self.cache: CacheState = CacheState(locale=locale, http=self.http)
```

### Comparing `valorant.py-1.0.6/valorant/enums.py` & `valorant_py-1.0.8/valorant/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,16 +118,16 @@
     @property
     def __members__(cls) -> Mapping[str, Any]:
         return types.MappingProxyType(cls._enum_member_map_)
 
     def __call__(cls, value: str) -> Any:
         try:
             return cls._enum_value_map_[value]
-        except (KeyError, TypeError):
-            raise ValueError(f"{value!r} is not a valid {cls.__name__}")
+        except (KeyError, TypeError) as e:
+            raise ValueError(f'{value!r} is not a valid {cls.__name__}') from e
 
     def __getitem__(cls, key: str) -> Any:
         return cls._enum_member_map_[key]
 
     def __setattr__(cls, name: str, value: Any) -> None:
         raise TypeError('Enums are immutable.')
```

### Comparing `valorant.py-1.0.6/valorant/errors.py` & `valorant_py-1.0.8/valorant/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,18 +58,18 @@
         The text of the error. Could be an empty string.
     status: :class:`int`
         The status code of the HTTP request.
     """
 
     def __init__(self, response: ClientResponse, message: Optional[Union[str, Dict[str, Any]]]):
         self.response: ClientResponse = response
-        self.status: int = response.status  # This attribute is filled by the library even if using requests # noqa: E501
+        self.status: int = response.status
         self.text: str
         if isinstance(message, dict):
-            self.text = message.get('message') or message.get('error', '')
+            self.text = message.get('error', '')
         else:
             self.text = message or ''
 
         fmt = '{0.status} {0.reason}'
         if len(self.text):
             fmt += ': {1}'
```

### Comparing `valorant.py-1.0.6/valorant/file.py` & `valorant_py-1.0.8/valorant/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 # source: https://github.com/Rapptz/discord.py/blob/master/discord/file.py
 
 
 class File:
     r"""A class that represents a file to be sent.
 
     Attributes
-    -----------
+    ----------
     fp: Union[:class:`os.PathLike`, :class:`io.BufferedIOBase`]
         A file-like object opened in binary mode and read mode
         or a filename representing a file in the hard drive to
         open.
 
         .. note::
```

### Comparing `valorant.py-1.0.6/valorant/http.py` & `valorant_py-1.0.8/valorant/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 
-import asyncio
 import logging
 import sys
 from typing import TYPE_CHECKING, Any, ClassVar, Coroutine, Dict, Optional, TypeVar, Union
 from urllib.parse import quote as _uriquote
 
 import aiohttp
 
@@ -111,56 +110,32 @@
         method = route.method
         url = route.url
         kwargs['headers'] = {'User-Agent': self.user_agent}
 
         response: Optional[aiohttp.ClientResponse] = None
         data: Optional[Union[Dict[str, Any], str]] = None
 
-        for tries in range(5):
-            try:
-                async with self.__session.request(method, url, **kwargs) as response:
-                    _log.debug('%s %s with %s has returned %s', method, url, kwargs.get('data'), response.status)
-                    data = await to_json(response)
-                    if 300 > response.status >= 200:
-                        _log.debug('%s %s has received %s', method, url, data)
-                        return data
-
-                    if response.status == 400:
-                        raise BadRequest(response, data)
-
-                    # we are being rate limited
-                    if response.status == 429:
-                        if not response.headers.get('Via') or isinstance(data, str):
-                            # Banned by Cloudflare more than likely.
-                            raise HTTPException(response, data)
-                        raise RateLimited(response, data)
-                    elif response.status == 403:
-                        raise Forbidden(response, data)
-                    elif response.status == 404:
-                        raise NotFound(response, data)
-                    elif response.status >= 500:
-                        raise InternalServerError(response, data)
-                    else:
-                        raise HTTPException(response, data)
-
-            except OSError as e:
-                # Connection reset by peer
-                if tries < 4 and e.errno in (54, 10054):
-                    await asyncio.sleep(1 + tries * 2)
-                    continue
-                raise
-
-        if response is not None:
-            # We've run out of retries, raise.
-            if response.status >= 500:
+        async with self.__session.request(method, url, **kwargs) as response:
+            _log.debug('%s %s with %s has returned %s', method, url, kwargs.get('data'), response.status)
+            data = await to_json(response)
+            if 300 > response.status >= 200:
+                _log.debug('%s %s has received %s', method, url, data)
+                return data
+
+            if response.status == 400:
+                raise BadRequest(response, data)
+
+            if response.status == 429:
+                raise RateLimited(response, data)
+            elif response.status == 404:
+                raise NotFound(response, data)
+            elif response.status >= 500:
                 raise InternalServerError(response, data)
-
-            raise HTTPException(response, data)
-
-        raise RuntimeError('Unreachable code in HTTP handling')
+            else:
+                raise HTTPException(response, data)
 
     async def close(self) -> None:
         if self.__session is not MISSING:
             await self.__session.close()
 
     def clear(self) -> None:
         if self.__session and self.__session.closed:
@@ -173,28 +148,19 @@
             elif resp.status == 403:
                 raise Forbidden(resp, 'cannot retrieve asset')
             elif resp.status == 404:
                 raise NotFound(resp, 'asset not found')
             else:
                 raise HTTPException(resp, 'failed to get asset')
 
-    async def text_from_url(self, url: str) -> str:
-        async with self.__session.get(url) as resp:
-            if resp.status == 200:
-                return await resp.text()
-            elif resp.status == 404:
-                raise NotFound(resp, 'asset not found')
-            elif resp.status == 403:
-                raise Forbidden(resp, 'cannot retrieve asset')
-            else:
-                raise HTTPException(resp, 'failed to get asset')
-
     # valorant-api.com
 
-    def get_agents(self, *, language: Optional[str] = 'all', is_playable_character: bool = True) -> Response[agents.Agents]:
+    def get_agents(
+        self, *, language: Optional[str] = 'all', is_playable_character: bool = True
+    ) -> Response[agents.Agents]:
         params = {'isPlayableCharacter': str(is_playable_character), 'language': language}
         return self.request(Route('GET', '/agents'), params=params)
 
     def get_agent(self, uuid: str, *, language: Optional[str] = 'all') -> Response[agents.AgentUUID]:
         params = {'language': language}
         return self.request(Route('GET', '/agents/{uuid}', uuid=uuid), params=params)
 
@@ -239,15 +205,17 @@
         return self.request(Route('GET', '/competitivetiers/{uuid}', uuid=uuid), params={'language': language})
 
     # -
 
     def get_content_tiers(self, *, language: Optional[str] = 'all') -> Response[content_tiers.ContentTiers]:
         return self.request(Route('GET', '/contenttiers'), params={'language': language})
 
-    def get_content_tier(self, uuid: str, *, language: Optional[str] = 'all') -> Response[content_tiers.ContentTierUUID]:
+    def get_content_tier(
+        self, uuid: str, *, language: Optional[str] = 'all'
+    ) -> Response[content_tiers.ContentTierUUID]:
         return self.request(Route('GET', '/contenttiers/{uuid}', uuid=uuid), params={'language': language})
 
     # -
 
     def get_contracts(self, *, language: Optional[str] = 'all') -> Response[contracts.Contracts]:
         return self.request(Route('GET', '/contracts'), params={'language': language})
 
@@ -330,15 +298,17 @@
         return self.request(Route('GET', '/playercards/{uuid}', uuid=uuid), params={'language': language})
 
     # -
 
     def get_player_titles(self, *, language: Optional[str] = 'all') -> Response[player_titles.PlayerTitles]:
         return self.request(Route('GET', '/playertitles'), params={'language': language})
 
-    def get_player_title(self, uuid: str, *, language: Optional[str] = 'all') -> Response[player_titles.PlayerTitleUUID]:
+    def get_player_title(
+        self, uuid: str, *, language: Optional[str] = 'all'
+    ) -> Response[player_titles.PlayerTitleUUID]:
         return self.request(Route('GET', '/playertitles/{uuid}', uuid=uuid), params={'language': language})
 
     # -
 
     def get_seasons(self, *, language: Optional[str] = 'all') -> Response[seasons.Seasons]:
         return self.request(Route('GET', '/seasons'), params={'language': language})
```

### Comparing `valorant.py-1.0.6/valorant/localization.py` & `valorant_py-1.0.8/valorant/localization.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         self.th_TH: str = self.untranslated.get('th-TH', default)
         self.tr_TR: str = self.untranslated.get('tr-TR', default)
         self.vi_VN: str = self.untranslated.get('vi-VN', default)
         self.zh_CN: str = self.untranslated.get('zh-CN', default)
         self.zh_TW: str = self.untranslated.get('zh-TW', default)
 
     def __str__(self) -> str:
-        """Returns the default locale."""
+        """Return the default locale."""
         return self.locale
 
     def __repr__(self) -> str:
         return self.__str__()
 
     def __eq__(self, other: object) -> bool:
         return isinstance(other, Localization) and self.untranslated == other.untranslated
```

### Comparing `valorant.py-1.0.6/valorant/models/abc.py` & `valorant_py-1.0.8/valorant/models/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,38 +20,36 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 
-import abc
 import uuid
 from typing import TYPE_CHECKING, Dict, Optional, Union
 
 from ..asset import Asset
-from ..enums import Locale
 from ..localization import Localization
 
 if TYPE_CHECKING:
     from ..cache import CacheState
+    from ..enums import Locale
     from ..types.object import GridPosition as GridPositionPayload, ShopData as ShopDataPayload
     from .gear import Gear
     from .weapons import Weapon
 
 
 __all__ = (
     'BaseModel',
     'GridPosition',
     'ShopData',
 )
 
 
-class BaseModel(abc.ABC):
-    __slots__ = ('_uuid',)
+class BaseModel:
 
     def __init__(self, uuid: str) -> None:
         self._uuid = uuid
 
     @property
     def uuid(self) -> uuid.UUID:
         return uuid.UUID(self._uuid)
```

### Comparing `valorant.py-1.0.6/valorant/models/agents.py` & `valorant_py-1.0.8/valorant/models/agents.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 from ..asset import Asset
 from ..enums import AbilitySlot, Locale, try_enum
 from ..localization import Localization
-from .abc import BaseModel
+from .base import BaseModel
 
 if TYPE_CHECKING:
     from ..cache import CacheState
     from ..types.agents import (
         Ability as AbilityPayload,
         Agent as AgentPayload,
         Media as MediaPayload,
@@ -225,15 +225,15 @@
             ('ru_RU', self.ru_RU),
             ('th_TH', self.th_TH),
             ('tr_TR', self.tr_TR),
             ('vi_VN', self.vi_VN),
             ('zh_CN', self.zh_CN),
             ('zh_TW', self.zh_TW),
         ]
-        joined = ' '.join('%s=%r' % t for t in attrs)
+        joined = ' '.join('%s=%r' % t for t in attrs)  # noqa: UP031
         return f'<{self.__class__.__name__} {joined}>'
 
     def __eq__(self, other: object) -> bool:
         return isinstance(other, Localization) and self.ut == other.untranslated
 
     def __ne__(self, other: object) -> bool:
         return not self.__eq__(other)
@@ -265,15 +265,15 @@
             Locale.chinese: self.zh_CN,
             Locale.taiwan_chinese: self.zh_TW,
         }
         return voices
 
     def all(self) -> List[VoiceLine]:
         """:class:`List[VoiceLine]`: Returns all locales as a list."""
-        return list([v for v in self._dict().values() if v is not None])
+        return [v for v in self._dict().values() if v is not None]
 
     @property
     def voice_locale(self) -> Optional[VoiceLine]:
         """:class:`Optional[VoiceLine]`: Returns the voice locale of the current locale."""
         return self._dict().get(self._locale)
 
     @property
@@ -397,17 +397,18 @@
         self.asset_path: str = data['assetPath']
         self._is_full_portrait_right_facing: bool = data['isFullPortraitRightFacing']
         self._is_playable_character: bool = data['isPlayableCharacter']
         self._is_available_for_test: bool = data['isAvailableForTest']
         self._is_base_content: bool = data['isBaseContent']
         self.role: Role = Role(state=self._state, data=data['role'])
         self._abilities: Dict[AbilitySlot, Ability] = {
-            try_enum(AbilitySlot, ability['slot']): Ability(state=self._state, data=ability) for ability in data['abilities']
+            try_enum(AbilitySlot, ability['slot']): Ability(state=self._state, data=ability)
+            for ability in data['abilities']
         }
-        self._voice_line: Union[VoiceLinePayload, Dict[str, Optional[VoiceLinePayload]]] = data['voiceLine']
+        self._voice_line: Optional[Union[VoiceLinePayload, Dict[str, Optional[VoiceLinePayload]]]] = data['voiceLine']
         self._display_name_localized: Localization = Localization(self._display_name, locale=self._state.locale)
         self._description_localized: Localization = Localization(self._description, locale=self._state.locale)
 
     def __str__(self) -> str:
         return self.display_name.locale
 
     def __repr__(self) -> str:
@@ -468,19 +469,23 @@
     def abilities(self) -> List[Ability]:
         """:class: `List[AgentAbility]` Returns the agent's abilities."""
         return list(self._abilities.values())
 
     @property
     def voice_line(self) -> Optional[VoiceLine]:
         """:class: `AgentVoiceLineLocalization` Returns the agent's voice line."""
+        if self.voice_line_localization is None:
+            return None
         return self.voice_line_localization.voice_locale
 
     @property
-    def voice_line_localization(self) -> VoiceLineLocalization:
+    def voice_line_localization(self) -> Optional[VoiceLineLocalization]:
         """:class: `AgentVoiceLineLocalization` Returns the agent's voice line."""
+        if self._voice_line is None:
+            return None
         return VoiceLineLocalization(self._voice_line)
 
     def is_full_portrait_right_facing(self) -> bool:
         """:class: `bool` Returns whether the agent's full portrait is right facing."""
         return self._is_full_portrait_right_facing
 
     def is_playable_character(self) -> bool:
```

### Comparing `valorant.py-1.0.6/valorant/models/buddies.py` & `valorant_py-1.0.8/valorant/models/buddies.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Dict, List, Optional, Union
 
 from ..asset import Asset
-from ..enums import Locale
 from ..localization import Localization
-from .abc import BaseModel
+from .base import BaseModel
 
 if TYPE_CHECKING:
     from ..cache import CacheState
+    from ..enums import Locale
     from ..types.buddies import Buddy as BuddyPayload, BuddyLevel as BuddyLevelPayload
     from .themes import Theme
 
 __all__ = (
     'Buddy',
     'BuddyLevel',
 )
```

### Comparing `valorant.py-1.0.6/valorant/models/bundles.py` & `valorant_py-1.0.8/valorant/models/bundles.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Dict, List, Optional, Union
 
 from ..asset import Asset
-from ..enums import Locale
 from ..localization import Localization
-from .abc import BaseModel
+from .base import BaseModel
 
 if TYPE_CHECKING:
     from ..cache import CacheState
+    from ..enums import Locale
     from ..types.bundles import Bundle as BundlePayload
     from .buddies import Buddy
     from .player_cards import PlayerCard
     from .player_titles import PlayerTitle
     from .sprays import Spray
     from .weapons import Skin
 
@@ -64,16 +64,20 @@
         self._vertical_promo_image: str = data['verticalPromoImage']
         self.asset_path: str = data['assetPath']
         self._display_name_localized: Localization = Localization(self._display_name, locale=self._state.locale)
         self._display_name_sub_text_localized: Localization = Localization(
             self._display_name_sub_text, locale=self._state.locale
         )
         self._description_localized: Localization = Localization(self._description, locale=self._state.locale)
-        self._extra_description_localized: Localization = Localization(self._extra_description, locale=self._state.locale)
-        self._promo_description_localized: Localization = Localization(self._promo_description, locale=self._state.locale)
+        self._extra_description_localized: Localization = Localization(
+            self._extra_description, locale=self._state.locale
+        )
+        self._promo_description_localized: Localization = Localization(
+            self._promo_description, locale=self._state.locale
+        )
         self._items: List[BundleItem] = []
 
     def __str__(self) -> str:
         return self.display_name.locale
 
     def __repr__(self) -> str:
         return f'<Bundle display_name={self.display_name!r}>'
```

### Comparing `valorant.py-1.0.6/valorant/models/ceremonies.py` & `valorant_py-1.0.8/valorant/models/ceremonies.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,20 +22,20 @@
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Dict, Optional, Union
 
-from ..enums import Locale
 from ..localization import Localization
-from .abc import BaseModel
+from .base import BaseModel
 
 if TYPE_CHECKING:
     from ..cache import CacheState
+    from ..enums import Locale
     from ..types.ceremonies import Ceremony as CeremonyPayload
 
 # fmt: off
 __all__ = (
     'Ceremony',
 )
 # fmt: on
```

### Comparing `valorant.py-1.0.6/valorant/models/competitive_tiers.py` & `valorant_py-1.0.8/valorant/models/competitive_tiers.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Dict, List, Optional, Union
 
 from ..asset import Asset
-from ..enums import Locale
 from ..localization import Localization
-from .abc import BaseModel
+from .base import BaseModel
 
 if TYPE_CHECKING:
     from ..cache import CacheState
+    from ..enums import Locale
     from ..types.competitive_tiers import CompetitiveTier as CompetitiveTierPayload, Tier as TierPayload
 
 
 __all__ = (
     'CompetitiveTier',
     'Tier',
 )
```

### Comparing `valorant.py-1.0.6/valorant/models/content_tiers.py` & `valorant_py-1.0.8/valorant/models/content_tiers.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Dict, Optional, Union
 
 from ..asset import Asset
-from ..enums import Locale
 from ..localization import Localization
-from .abc import BaseModel
+from .base import BaseModel
 
 if TYPE_CHECKING:
     from ..cache import CacheState
+    from ..enums import Locale
     from ..types.content_tiers import ContentTier as ContentTierPayload
 
 # fmt: off
 __all__ = (
     'ContentTier',
 )
 # fmt: on
```

### Comparing `valorant.py-1.0.6/valorant/models/contracts.py` & `valorant_py-1.0.8/valorant/models/contracts.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 import logging
 from typing import TYPE_CHECKING, Dict, List, Optional, Union
 
 from ..asset import Asset
 from ..enums import Locale, RelationType, RewardType, try_enum
 from ..localization import Localization
-from .abc import BaseModel
+from .base import BaseModel
 
 if TYPE_CHECKING:
     from uuid import UUID
 
     from ..cache import CacheState
     from ..types.contracts import (
         Chapter as ChapterPayload,
```

### Comparing `valorant.py-1.0.6/valorant/models/currencies.py` & `valorant_py-1.0.8/valorant/models/currencies.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Dict, Optional, Union
 
 from ..asset import Asset
-from ..enums import Locale
 from ..localization import Localization
-from .abc import BaseModel
+from .base import BaseModel
 
 if TYPE_CHECKING:
     from ..cache import CacheState
+    from ..enums import Locale
     from ..types.currencies import Currency as CurrencyPayload
 
 # fmt: off
 __all__ = (
     'Currency',
 )
 # fmt: on
```

### Comparing `valorant.py-1.0.6/valorant/models/events.py` & `valorant_py-1.0.8/valorant/models/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,22 +23,22 @@
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Dict, Optional, Union
 
 from .. import utils
-from ..enums import Locale
 from ..localization import Localization
-from .abc import BaseModel
+from .base import BaseModel
 
 if TYPE_CHECKING:
     import datetime
 
     from ..cache import CacheState
+    from ..enums import Locale
     from ..types.events import Event as EventPayload
 
 # fmt: off
 __all__ = (
     'Event',
 )
 # fmt: on
@@ -50,15 +50,17 @@
         self._state: CacheState = state
         self._display_name: Union[str, Dict[str, str]] = data['displayName']
         self._short_display_name: Union[str, Dict[str, str]] = data['shortDisplayName']
         self._start_time_iso: str = data['startTime']
         self._end_time_iso: str = data['endTime']
         self.asset_path: str = data['assetPath']
         self._display_name_localized: Localization = Localization(self._display_name, locale=self._state.locale)
-        self._short_display_name_localized: Localization = Localization(self._short_display_name, locale=self._state.locale)
+        self._short_display_name_localized: Localization = Localization(
+            self._short_display_name, locale=self._state.locale
+        )
 
     def __str__(self) -> str:
         return self.display_name.locale
 
     def __repr__(self) -> str:
         return f'<Event display_name={self.display_name!r}>'
```

### Comparing `valorant.py-1.0.6/valorant/models/gamemodes.py` & `valorant_py-1.0.8/valorant/models/gamemodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Dict, List, Optional, Union
 
 from ..asset import Asset
-from ..enums import Locale
 from ..localization import Localization
-from .abc import BaseModel
+from .base import BaseModel
 
 if TYPE_CHECKING:
     from ..cache import CacheState
+    from ..enums import Locale
     from ..types.gamemodes import (
         GameFeatureOverride as GameFeatureOverridePayload,
         GameMode as GameModePayload,
         GameModeEquippable as GameModeEquippablePayload,
         GameRuleBoolOverride as GameRuleBoolOverridePayload,
     )
     from .weapons import Weapon
```

### Comparing `valorant.py-1.0.6/valorant/models/gear.py` & `valorant_py-1.0.8/valorant/models/gear.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Dict, Optional, Union
 
 from ..asset import Asset
-from ..enums import Locale
 from ..localization import Localization
-from .abc import BaseModel, ShopData
+from .base import BaseModel, ShopData
 
 if TYPE_CHECKING:
     from ..cache import CacheState
+    from ..enums import Locale
     from ..types.gear import Gear_ as GearPayload
 
 # fmt: off
 __all__ = (
     'Gear',
 )
 # fmt: on
```

### Comparing `valorant.py-1.0.6/valorant/models/level_borders.py` & `valorant_py-1.0.8/valorant/models/level_borders.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import annotations
+
 
 """
 The MIT License (MIT)
 
 Copyright (c) 2023-present STACiA
 
 Permission is hereby granted, free of charge, to any person obtaining a
@@ -19,30 +19,31 @@
 OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
+from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from ..asset import Asset
-from .abc import BaseModel
-
-if TYPE_CHECKING:
-    from ..cache import CacheState
-    from ..types.level_borders import LevelBorder as LevelBorderPayload
+from .base import BaseModel
 
 # fmt: off
 __all__ = (
     'LevelBorder',
 )
 # fmt: on
 
+if TYPE_CHECKING:
+    from ..cache import CacheState
+    from ..types.level_borders import LevelBorder as LevelBorderPayload
+
 
 class LevelBorder(BaseModel):
     def __init__(self, state: CacheState, data: LevelBorderPayload) -> None:
         super().__init__(data['uuid'])
         self._state: CacheState = state
         self.starting_level: int = data['startingLevel']
         self._level_number_appearance: str = data['levelNumberAppearance']
```

### Comparing `valorant.py-1.0.6/valorant/models/maps.py` & `valorant_py-1.0.8/valorant/models/maps.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Dict, List, Optional, Union
 
 from ..asset import Asset
-from ..enums import Locale
 from ..localization import Localization
-from .abc import BaseModel
+from .base import BaseModel
 
 if TYPE_CHECKING:
     from ..cache import CacheState
+    from ..enums import Locale
     from ..types.maps import Callout as CalloutPayload, Location as LocationPayload, Map as MapPayload
 
 
 __all__ = (
     'Map',
     'Callout',
     'Location',
@@ -61,15 +61,17 @@
 class Callout:
     def __init__(self, state: CacheState, data: CalloutPayload) -> None:
         self._state: CacheState = state
         self._region_name: Union[str, Dict[str, str]] = data['regionName']
         self._super_region_name: Union[str, Dict[str, str]] = data['superRegionName']
         self.location: Location = Location(data['location'])
         self._region_name_localized: Localization = Localization(self._region_name, locale=self._state.locale)
-        self._super_region_name_localized: Localization = Localization(self._super_region_name, locale=self._state.locale)
+        self._super_region_name_localized: Localization = Localization(
+            self._super_region_name, locale=self._state.locale
+        )
 
     def __str__(self) -> str:
         return self.region_name.locale
 
     def __repr__(self) -> str:
         attrs = [
             ('region_name', self.region_name),
```

### Comparing `valorant.py-1.0.6/valorant/models/missions.py` & `valorant_py-1.0.8/valorant/models/missions.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,23 +20,24 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 
-import datetime
 from typing import TYPE_CHECKING, Dict, List, Optional, Union
 
 from .. import utils
 from ..enums import Locale, MissionType, try_enum
 from ..localization import Localization
-from .abc import BaseModel
+from .base import BaseModel
 
 if TYPE_CHECKING:
+    import datetime
+
     from ..cache import CacheState
     from ..types.missions import Mission as MissionPayload, Objective as ObjectivePayload
 
 # fmt: off
 __all__ = (
     'Mission',
 )
```

### Comparing `valorant.py-1.0.6/valorant/models/player_cards.py` & `valorant_py-1.0.8/valorant/models/player_cards.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Dict, Optional, Union
 
 from ..asset import Asset
-from ..enums import Locale
 from ..localization import Localization
-from .abc import BaseModel
+from .base import BaseModel
 
 if TYPE_CHECKING:
     from ..cache import CacheState
+    from ..enums import Locale
     from ..types.player_cards import PlayerCard as PlayerCardPayload
     from .themes import Theme
 
 # fmt: off
 __all__ = (
     'PlayerCard',
 )
```

### Comparing `valorant.py-1.0.6/valorant/models/player_titles.py` & `valorant_py-1.0.8/valorant/models/player_titles.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,20 +22,20 @@
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Dict, Optional, Union
 
-from ..enums import Locale
 from ..localization import Localization
-from .abc import BaseModel
+from .base import BaseModel
 
 if TYPE_CHECKING:
     from ..cache import CacheState
+    from ..enums import Locale
     from ..types.player_titles import PlayerTitle as PlayerTitlePayload
 
 
 # fmt: off
 __all__ = (
     'PlayerTitle',
 )
```

### Comparing `valorant.py-1.0.6/valorant/models/seasons.py` & `valorant_py-1.0.8/valorant/models/seasons.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,23 +24,23 @@
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Dict, List, Optional, Union
 
 from .. import utils
 from ..asset import Asset
-from ..enums import Locale
 from ..localization import Localization
-from .abc import BaseModel
+from .base import BaseModel
 
 if TYPE_CHECKING:
     import datetime
     from uuid import UUID
 
     from ..cache import CacheState
+    from ..enums import Locale
     from ..types.seasons import (
         Border as BorderPayload,
         CompetitiveSeason as CompetitiveSeasonPayload,
         Season as SeasonPayload,
     )
     from .competitive_tiers import CompetitiveTier
```

### Comparing `valorant.py-1.0.6/valorant/models/sprays.py` & `valorant_py-1.0.8/valorant/models/sprays.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Dict, List, Optional, Union
 
 from ..asset import Asset
-from ..enums import Locale
 from ..localization import Localization
-from .abc import BaseModel
+from .base import BaseModel
 
 if TYPE_CHECKING:
     from ..cache import CacheState
+    from ..enums import Locale
     from ..types.sprays import Spray as SprayPayload, SprayLevel as SprayLevelPayload
     from .themes import Theme
 
 __all__ = (
     'Spray',
     'SprayLevel',
 )
```

### Comparing `valorant.py-1.0.6/valorant/models/themes.py` & `valorant_py-1.0.8/valorant/models/themes.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Dict, Optional, Union
 
 from ..asset import Asset
-from ..enums import Locale
 from ..localization import Localization
-from .abc import BaseModel
+from .base import BaseModel
 
 if TYPE_CHECKING:
     from ..cache import CacheState
+    from ..enums import Locale
     from ..types.themes import Theme as ThemePayload
 
 # fmt: off
 __all__ = (
     'Theme',
 )
 # fmt: on
```

### Comparing `valorant.py-1.0.6/valorant/models/version.py` & `valorant_py-1.0.8/valorant/models/version.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.6/valorant/models/weapons.py` & `valorant_py-1.0.8/valorant/models/weapons.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 from typing import TYPE_CHECKING, Dict, List, Optional, Union
 
 from .. import utils
 from ..asset import Asset
 from ..enums import MELEE_WEAPON_ID, Locale
 from ..localization import Localization
-from .abc import BaseModel, ShopData
+from .base import BaseModel, ShopData
 
 if TYPE_CHECKING:
     from ..cache import CacheState
     from ..types.weapons import (
         AdsStats as AdsStatsPayload,
         AirBurstStats as AirBurstStatsPayload,
         AltShotgunStats as AltShotgunStatsPayload,
@@ -83,24 +83,24 @@
 
 class AltShotgunStats:
     def __init__(self, data: AltShotgunStatsPayload) -> None:
         self.shotgun_pellet_count: float = data['shotgunPelletCount']
         self.burst_rate: float = data['burstRate']
 
     def __repr__(self) -> str:
-        return f"<AltShotgunStats shotgun_pellet_count={self.shotgun_pellet_count} burst_rate={self.burst_rate}>"
+        return f'<AltShotgunStats shotgun_pellet_count={self.shotgun_pellet_count} burst_rate={self.burst_rate}>'
 
 
 class AirBurstStats:
     def __init__(self, data: AirBurstStatsPayload) -> None:
         self.shotgun_pellet_count: float = data['shotgunPelletCount']
         self.burst_distance: float = data['burstDistance']
 
     def __repr__(self) -> str:
-        return f"<AirBurstStats shotgun_pellet_count={self.shotgun_pellet_count} burst_distance={self.burst_distance}>"
+        return f'<AirBurstStats shotgun_pellet_count={self.shotgun_pellet_count} burst_distance={self.burst_distance}>'
 
 
 class DamageRange:
     def __init__(self, data: DamageRangePayload) -> None:
         self.range_start_meters: float = data['rangeStartMeters']
         self.range_end_meters: float = data['rangeEndMeters']
         self.head_damage: float = data['headDamage']
@@ -185,15 +185,15 @@
         self._is_melee: bool = True if self.uuid == MELEE_WEAPON_ID else False
         self._display_name_localized: Localization = Localization(self._display_name, locale=self._state.locale)
 
     def __str__(self) -> str:
         return self.display_name.locale
 
     def __repr__(self) -> str:
-        return f"<Weapon display_name={self.display_name!r}>"
+        return f'<Weapon display_name={self.display_name!r}>'
 
     def display_name_localized(self, locale: Optional[Union[Locale, str]] = None) -> str:
         return self._display_name_localized.from_locale(locale)
 
     @property
     def display_name(self) -> Localization:
         """:class: `str` Returns the weapon's name."""
@@ -242,15 +242,15 @@
         self.parent: Weapon = parent
         self._display_name_localized: Localization = Localization(self._display_name, locale=self._state.locale)
 
     def __str__(self) -> str:
         return self.display_name.locale
 
     def __repr__(self) -> str:
-        return f"<Skin display_name={self.display_name!r}>"
+        return f'<Skin display_name={self.display_name!r}>'
 
     def display_name_localized(self, locale: Optional[Union[Locale, str]] = None) -> str:
         return self._display_name_localized.from_locale(locale)
 
     @property
     def display_name(self) -> Localization:
         """:class: `str` Returns the skin's name."""
@@ -443,15 +443,15 @@
         self.parent: Skin = parent
         self._display_name_localized: Localization = Localization(self._display_name, locale=self._state.locale)
 
     def __str__(self) -> str:
         return str(self.display_name)
 
     def __repr__(self) -> str:
-        return f"<SkinLevel display_name={self.display_name!r} level={self.level!r}>"
+        return f'<SkinLevel display_name={self.display_name!r} level={self.level!r}>'
 
     def display_name_localized(self, locale: Optional[Union[Locale, str]] = None) -> str:
         return self._display_name_localized.from_locale(locale=locale)
 
     @property
     def display_name(self) -> Localization:
         """:class: `str` Returns the skin's name."""
```

### Comparing `valorant.py-1.0.6/valorant/types/agents.py` & `valorant_py-1.0.8/valorant/types/agents.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,12 +70,12 @@
     assetPath: str
     isFullPortraitRightFacing: bool
     isPlayableCharacter: bool
     isAvailableForTest: bool
     isBaseContent: bool
     role: Role
     abilities: List[Ability]
-    voiceLine: Union[VoiceLine, Dict[str, Optional[VoiceLine]]]
+    voiceLine: Optional[Union[VoiceLine, Dict[str, Optional[VoiceLine]]]]
 
 
 Agents = Response[List[Agent]]
 AgentUUID = Response[Agent]
```

### Comparing `valorant.py-1.0.6/valorant/types/buddies.py` & `valorant_py-1.0.8/valorant/types/buddies.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.6/valorant/types/bundles.py` & `valorant_py-1.0.8/valorant/types/bundles.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.6/valorant/types/ceremonies.py` & `valorant_py-1.0.8/valorant/types/ceremonies.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.6/valorant/types/competitive_tiers.py` & `valorant_py-1.0.8/valorant/types/competitive_tiers.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.6/valorant/types/content_tiers.py` & `valorant_py-1.0.8/valorant/types/content_tiers.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.6/valorant/types/contracts.py` & `valorant_py-1.0.8/valorant/types/contracts.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.6/valorant/types/currencies.py` & `valorant_py-1.0.8/valorant/types/currencies.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.6/valorant/types/events.py` & `valorant_py-1.0.8/valorant/types/events.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.6/valorant/types/gamemodes.py` & `valorant_py-1.0.8/valorant/types/gamemodes.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.6/valorant/types/gear.py` & `valorant_py-1.0.8/valorant/types/gear.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.6/valorant/types/level_borders.py` & `valorant_py-1.0.8/valorant/types/level_borders.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.6/valorant/types/maps.py` & `valorant_py-1.0.8/valorant/types/maps.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.6/valorant/types/missions.py` & `valorant_py-1.0.8/valorant/types/missions.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.6/valorant/types/object.py` & `valorant_py-1.0.8/valorant/types/object.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.6/valorant/types/player_cards.py` & `valorant_py-1.0.8/valorant/types/player_cards.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.6/valorant/types/player_titles.py` & `valorant_py-1.0.8/valorant/types/player_titles.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.6/valorant/types/response.py` & `valorant_py-1.0.8/valorant/types/response.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.6/valorant/types/seasons.py` & `valorant_py-1.0.8/valorant/types/seasons.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.6/valorant/types/sprays.py` & `valorant_py-1.0.8/valorant/types/sprays.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.6/valorant/types/themes.py` & `valorant_py-1.0.8/valorant/types/themes.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.6/valorant/types/version.py` & `valorant_py-1.0.8/valorant/types/version.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.6/valorant/types/weapons.py` & `valorant_py-1.0.8/valorant/types/weapons.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.6/valorant/utils.py` & `valorant_py-1.0.8/valorant/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,35 +31,35 @@
 from typing import Any
 
 try:
     import orjson  # type: ignore
 except ImportError:
     HAS_ORJSON = False
 else:
-    HAS_ORJSON = True
+    HAS_ORJSON = True  # pragma: no cover
 
 if HAS_ORJSON:
     _from_json = orjson.loads  # type: ignore
 else:
     _from_json = json.loads
 
 
 class _MissingSentinel:
     __slots__ = ()
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any) -> bool:
         return False
 
-    def __bool__(self):
+    def __bool__(self) -> bool:
         return False
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         return 0
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return '...'
 
 
 MISSING: Any = _MissingSentinel()
 
 # - end
```

### Comparing `valorant.py-1.0.6/valorant.py.egg-info/SOURCES.txt` & `valorant_py-1.0.8/valorant.py.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 valorant/utils.py
 valorant.py.egg-info/PKG-INFO
 valorant.py.egg-info/SOURCES.txt
 valorant.py.egg-info/dependency_links.txt
 valorant.py.egg-info/requires.txt
 valorant.py.egg-info/top_level.txt
 valorant/models/__init__.py
-valorant/models/abc.py
 valorant/models/agents.py
+valorant/models/base.py
 valorant/models/buddies.py
 valorant/models/bundles.py
 valorant/models/ceremonies.py
 valorant/models/competitive_tiers.py
 valorant/models/content_tiers.py
 valorant/models/contracts.py
 valorant/models/currencies.py
```

