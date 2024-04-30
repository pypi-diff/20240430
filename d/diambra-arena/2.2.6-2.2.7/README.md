# Comparing `tmp/diambra-arena-2.2.6.tar.gz` & `tmp/diambra_arena-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diambra-arena-2.2.6.tar", last modified: Sun Feb 18 16:53:06 2024, max compression
+gzip compressed data, was "diambra_arena-2.2.7.tar", last modified: Tue Apr 30 03:06:48 2024, max compression
```

## Comparing `diambra-arena-2.2.6.tar` & `diambra_arena-2.2.7.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 16:53:06.904366 diambra-arena-2.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    19105 2024-02-18 16:53:06.904366 diambra-arena-2.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16959 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 16:53:06.888366 diambra-arena-2.2.6/diambra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/diambra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 16:53:06.888366 diambra-arena-2.2.6/diambra/arena/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/diambra/arena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13774 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/diambra/arena/arena_gym.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 16:53:06.888366 diambra-arena-2.2.6/diambra/arena/engine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/diambra/arena/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/diambra/arena/engine/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    19894 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/diambra/arena/env_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/diambra/arena/make_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 16:53:06.892366 diambra-arena-2.2.6/diambra/arena/ray_rllib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/diambra/arena/ray_rllib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/diambra/arena/ray_rllib/make_ray_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 16:53:06.892366 diambra-arena-2.2.6/diambra/arena/sheeprl/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/diambra/arena/sheeprl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/diambra/arena/sheeprl/make_sheeprl_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 16:53:06.892366 diambra-arena-2.2.6/diambra/arena/stable_baselines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/diambra/arena/stable_baselines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/diambra/arena/stable_baselines/make_sb_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/diambra/arena/stable_baselines/sb_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 16:53:06.892366 diambra-arena-2.2.6/diambra/arena/stable_baselines3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/diambra/arena/stable_baselines3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/diambra/arena/stable_baselines3/make_sb3_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/diambra/arena/stable_baselines3/sb3_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 16:53:06.896366 diambra-arena-2.2.6/diambra/arena/utils/
--rw-r--r--   0 runner    (1001) docker     (127)   167633 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/diambra/arena/utils/.splash_screen.gif
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/diambra/arena/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40178 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/diambra/arena/utils/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/diambra/arena/utils/diambra_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    16265 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/diambra/arena/utils/engine_mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/diambra/arena/utils/gym_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14658 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/diambra/arena/utils/integratedGames.json
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/diambra/arena/utils/policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/diambra/arena/utils/splash_screen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 16:53:06.896366 diambra-arena-2.2.6/diambra/arena/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/diambra/arena/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9328 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/diambra/arena/wrappers/arena_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/diambra/arena/wrappers/episode_recording.py
--rw-r--r--   0 runner    (1001) docker     (127)    19861 2024-02-18 16:52:42.000000 diambra-arena-2.2.6/diambra/arena/wrappers/observation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 16:53:06.900366 diambra-arena-2.2.6/diambra_arena.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19105 2024-02-18 16:53:06.000000 diambra-arena-2.2.6/diambra_arena.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-02-18 16:53:06.000000 diambra-arena-2.2.6/diambra_arena.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-18 16:53:06.000000 diambra-arena-2.2.6/diambra_arena.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-02-18 16:53:06.000000 diambra-arena-2.2.6/diambra_arena.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-18 16:53:06.000000 diambra-arena-2.2.6/diambra_arena.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-18 16:53:06.904366 diambra-arena-2.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-02-18 16:52:43.000000 diambra-arena-2.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 16:53:06.900366 diambra-arena-2.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-02-18 16:52:43.000000 diambra-arena-2.2.6/tests/test_episode_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-02-18 16:52:43.000000 diambra-arena-2.2.6/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-02-18 16:52:43.000000 diambra-arena-2.2.6/tests/test_gym_settings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5861 2024-02-18 16:52:43.000000 diambra-arena-2.2.6/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-02-18 16:52:43.000000 diambra-arena-2.2.6/tests/test_recording_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-02-18 16:52:43.000000 diambra-arena-2.2.6/tests/test_speed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-02-18 16:52:43.000000 diambra-arena-2.2.6/tests/test_wrappers_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:06:48.701688 diambra_arena-2.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    19991 2024-04-30 03:06:48.701688 diambra_arena-2.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17967 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:06:48.693688 diambra_arena-2.2.7/diambra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/diambra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:06:48.693688 diambra_arena-2.2.7/diambra/arena/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/diambra/arena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14050 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/diambra/arena/arena_gym.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:06:48.693688 diambra_arena-2.2.7/diambra/arena/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/diambra/arena/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/diambra/arena/engine/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21138 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/diambra/arena/env_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/diambra/arena/make_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:06:48.693688 diambra_arena-2.2.7/diambra/arena/ray_rllib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/diambra/arena/ray_rllib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/diambra/arena/ray_rllib/make_ray_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:06:48.693688 diambra_arena-2.2.7/diambra/arena/sheeprl/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/diambra/arena/sheeprl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/diambra/arena/sheeprl/make_sheeprl_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:06:48.693688 diambra_arena-2.2.7/diambra/arena/stable_baselines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/diambra/arena/stable_baselines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/diambra/arena/stable_baselines/make_sb_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/diambra/arena/stable_baselines/sb_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:06:48.693688 diambra_arena-2.2.7/diambra/arena/stable_baselines3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/diambra/arena/stable_baselines3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/diambra/arena/stable_baselines3/make_sb3_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/diambra/arena/stable_baselines3/sb3_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:06:48.697688 diambra_arena-2.2.7/diambra/arena/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)   167633 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/diambra/arena/utils/.splash_screen.gif
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/diambra/arena/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40175 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/diambra/arena/utils/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/diambra/arena/utils/diambra_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16265 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/diambra/arena/utils/engine_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7155 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/diambra/arena/utils/gym_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22441 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/diambra/arena/utils/integratedGames.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/diambra/arena/utils/splash_screen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:06:48.697688 diambra_arena-2.2.7/diambra/arena/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/diambra/arena/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9338 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/diambra/arena/wrappers/arena_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/diambra/arena/wrappers/episode_recording.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19861 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/diambra/arena/wrappers/observation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:06:48.697688 diambra_arena-2.2.7/diambra_arena.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19991 2024-04-30 03:06:48.000000 diambra_arena-2.2.7/diambra_arena.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-30 03:06:48.000000 diambra_arena-2.2.7/diambra_arena.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 03:06:48.000000 diambra_arena-2.2.7/diambra_arena.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-30 03:06:48.000000 diambra_arena-2.2.7/diambra_arena.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 03:06:48.000000 diambra_arena-2.2.7/diambra_arena.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 03:06:48.701688 diambra_arena-2.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:06:48.697688 diambra_arena-2.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/tests/test_episode_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/tests/test_gym_settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5979 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/tests/test_recording_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/tests/test_speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-04-30 03:06:39.000000 diambra_arena-2.2.7/tests/test_wrappers_settings.py
```

### Comparing `diambra-arena-2.2.6/LICENSE.txt` & `diambra_arena-2.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.2.6/PKG-INFO` & `diambra_arena-2.2.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diambra-arena
-Version: 2.2.6
+Version: 2.2.7
 Summary: DIAMBRA™ Arena. Built with OpenAI Gym Python interface, easy to use, transforms popular video games into Reinforcement Learning environments
 Home-page: https://github.com/diambra/arena
 Author: DIAMBRA Team
 Author-email: info@diambra.ai
 License: Custom
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
@@ -13,25 +13,22 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Artificial Life
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Games/Entertainment :: Arcade
 Classifier: Topic :: Education
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: pip>=21
 Requires-Dist: importlib-metadata<=4.12.0; python_version <= "3.7"
-Requires-Dist: setuptools
-Requires-Dist: distro>=1
 Requires-Dist: gymnasium>=0.26.3
 Requires-Dist: inputs
 Requires-Dist: screeninfo
 Requires-Dist: tk
 Requires-Dist: opencv-python>=4.4.0.42
 Requires-Dist: grpcio
-Requires-Dist: diambra-engine~=2.2.0
+Requires-Dist: diambra-engine>=2.2.3
 Requires-Dist: dacite
 Provides-Extra: core
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-mock; extra == "tests"
 Requires-Dist: testresources; extra == "tests"
 Provides-Extra: stable-baselines
@@ -40,19 +37,18 @@
 Requires-Dist: protobuf==3.20.1; extra == "stable-baselines"
 Requires-Dist: pyyaml; extra == "stable-baselines"
 Provides-Extra: stable-baselines3
 Requires-Dist: stable-baselines3[extra]~=2.1.0; extra == "stable-baselines3"
 Requires-Dist: pyyaml; extra == "stable-baselines3"
 Provides-Extra: ray-rllib
 Requires-Dist: ray[rllib]~=2.7.0; extra == "ray-rllib"
-Requires-Dist: tensorflow; extra == "ray-rllib"
 Requires-Dist: torch; extra == "ray-rllib"
 Requires-Dist: pyyaml; extra == "ray-rllib"
 Provides-Extra: sheeprl
-Requires-Dist: sheeprl==0.5.1; extra == "sheeprl"
+Requires-Dist: sheeprl==0.5.5; extra == "sheeprl"
 Requires-Dist: importlib-resources==6.1.0; extra == "sheeprl"
 
 <img src="https://raw.githubusercontent.com/diambra/arena/main/img/github.jpg" alt="diambra" width="100%"/>
 
 <p align="center">
   <a href="https://docs.diambra.ai">Documentation</a> •
   <a href="https://diambra.ai/">Website</a>
@@ -121,14 +117,18 @@
 
 Additional details can be found in the <a href="https://docs.diambra.ai/envs/games/" target="_blank">dedicated section</a> of our Documentation.
 
 | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/doapp.jpg" alt="doapp" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/sfiii3n.jpg" alt="sfiii3n" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/tektagt.jpg" alt="tektagt" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/umk3.jpg" alt="umk3" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/samsh5sp.jpg" alt="samsh6sp" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/kof98umh.jpg" alt="kof98umh" width="125"/> |
 | :------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------: |
 |                                             Dead<br>Or<br>Alive ++                                             |                                        Street<br>Fighter III<br>3rd Strike                                         |                                              Tekken Tag<br>Tournament                                              |                                        Ultimate<br>Mortal<br>Kombat 3                                        |                                           Samurai<br>Showdown<br>5 Special                                           |                                 The King of<br>Fighers '98<br>Ultimate<br>Match Hero                                 |
 
+| <img src="https://raw.githubusercontent.com/diambra/arena/main/img/mvsc.jpg" alt="mvsc" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/xmvsf.jpg" alt="xmvsf" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/soulclbr.jpg" alt="soulclbr" width="125"/> |
+| :------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------: |
+|                                             Marvel<br>VS<br>Capcom                                             |                                        X-Men<br>VS<br>Street Fighter                                         |                                              Soul<br>Calibur                                              |
+
 **Many more are coming soon...**
 
 ## Competition Platform
 
 <img src="https://raw.githubusercontent.com/diambra/.github/master/img/platform.jpg" alt="DIAMBRA Competition Platform" width="100%"/>
 
 Our competition platform allows you to submit your agents and compete with other coders around the globe in epic video games tournaments!
```

#### html2text {}

```diff
@@ -1,36 +1,35 @@
-Metadata-Version: 2.1 Name: diambra-arena Version: 2.2.6 Summary: DIAMBRAâ¢
+Metadata-Version: 2.1 Name: diambra-arena Version: 2.2.7 Summary: DIAMBRAâ¢
 Arena. Built with OpenAI Gym Python interface, easy to use, transforms popular
 video games into Reinforcement Learning environments Home-page: https://
 github.com/diambra/arena Author: DIAMBRA Team Author-email: info@diambra.ai
 License: Custom Classifier: Development Status :: 3 - Alpha Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
 Scientific/Engineering :: Artificial Life Classifier: Topic :: Games/
 Entertainment Classifier: Topic :: Games/Entertainment :: Arcade Classifier:
 Topic :: Education Description-Content-Type: text/markdown License-File:
-LICENSE.txt Requires-Dist: pip>=21 Requires-Dist: importlib-metadata<=4.12.0;
-python_version <= "3.7" Requires-Dist: setuptools Requires-Dist: distro>=1
+LICENSE.txt Requires-Dist: importlib-metadata<=4.12.0; python_version <= "3.7"
 Requires-Dist: gymnasium>=0.26.3 Requires-Dist: inputs Requires-Dist:
 screeninfo Requires-Dist: tk Requires-Dist: opencv-python>=4.4.0.42 Requires-
-Dist: grpcio Requires-Dist: diambra-engine~=2.2.0 Requires-Dist: dacite
+Dist: grpcio Requires-Dist: diambra-engine>=2.2.3 Requires-Dist: dacite
 Provides-Extra: core Provides-Extra: tests Requires-Dist: pytest; extra ==
 "tests" Requires-Dist: pytest-mock; extra == "tests" Requires-Dist:
 testresources; extra == "tests" Provides-Extra: stable-baselines Requires-Dist:
 stable-baselines~=2.10.2; extra == "stable-baselines" Requires-Dist:
 gym<=0.21.0; extra == "stable-baselines" Requires-Dist: protobuf==3.20.1; extra
 == "stable-baselines" Requires-Dist: pyyaml; extra == "stable-baselines"
 Provides-Extra: stable-baselines3 Requires-Dist: stable-baselines3
 [extra]~=2.1.0; extra == "stable-baselines3" Requires-Dist: pyyaml; extra ==
 "stable-baselines3" Provides-Extra: ray-rllib Requires-Dist: ray[rllib]~=2.7.0;
-extra == "ray-rllib" Requires-Dist: tensorflow; extra == "ray-rllib" Requires-
-Dist: torch; extra == "ray-rllib" Requires-Dist: pyyaml; extra == "ray-rllib"
-Provides-Extra: sheeprl Requires-Dist: sheeprl==0.5.1; extra == "sheeprl"
-Requires-Dist: importlib-resources==6.1.0; extra == "sheeprl"[diambra]
+extra == "ray-rllib" Requires-Dist: torch; extra == "ray-rllib" Requires-Dist:
+pyyaml; extra == "ray-rllib" Provides-Extra: sheeprl Requires-Dist:
+sheeprl==0.5.5; extra == "sheeprl" Requires-Dist: importlib-resources==6.1.0;
+extra == "sheeprl"[diambra]
                            _D_o_c_u_m_e_n_t_a_t_i_o_n â¢ _W_e_b_s_i_t_e
             _L_i_n_k_e_d_i_n â¢ _D_i_s_c_o_r_d â¢ _T_w_i_t_c_h â¢ _Y_o_u_T_u_b_e â¢ _T_w_i_t_t_e_r
                                     _[_P_a_p_e_r_]
               _[_A_r_e_n_a_ _T_e_s_t_]_[_A_g_e_n_t_s_ _T_e_s_t_]_[_L_a_t_e_s_t_ _T_a_g_]_[_P_y_p_i_ _v_e_r_s_i_o_n_]
                        _[_S_u_p_p_o_r_t_e_d_ _O_S_]_[_L_a_s_t_ _D_o_c_s_ _U_p_d_a_t_e_]
 # DIAMBRA Arena ## Index - **[Overview](#overview)** - **[Competition Platform]
 (#competition-platform)** - **[Installation](#installation)** - **[Quickstart &
@@ -91,15 +90,25 @@
 Tournament | Ultimate
 Mortal
 Kombat 3 | Samurai
 Showdown
 5 Special | The King of
 Fighers '98
 Ultimate
-Match Hero | **Many more are coming soon...** ## Competition Platform [DIAMBRA
+Match Hero | | [mvsc]| [xmvsf]| [soulclbr]| | :--------------------------------
+----------------------------------------------------------------------------: |
+:------------------------------------------------------------------------------
+----------------------------------: | :----------------------------------------
+------------------------------------------------------------------------: | |
+Marvel
+VS
+Capcom | X-Men
+VS
+Street Fighter | Soul
+Calibur | **Many more are coming soon...** ## Competition Platform [DIAMBRA
 Competition Platform]Our competition platform allows you to submit your agents
 and compete with other coders around the globe in epic video games tournaments!
 It features a public global leaderboard where users are ranked by the best
 score achieved by their agents in our different environments. It also offers
 you the possibility to unlock cool achievements depending on the performances
 of your agent. Submitted agents are evaluated and their episodes are streamed
 on our Twitch channel. We aimed at making the submission process as smooth as
```

### Comparing `diambra-arena-2.2.6/README.md` & `diambra_arena-2.2.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,18 @@
 
 Additional details can be found in the <a href="https://docs.diambra.ai/envs/games/" target="_blank">dedicated section</a> of our Documentation.
 
 | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/doapp.jpg" alt="doapp" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/sfiii3n.jpg" alt="sfiii3n" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/tektagt.jpg" alt="tektagt" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/umk3.jpg" alt="umk3" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/samsh5sp.jpg" alt="samsh6sp" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/kof98umh.jpg" alt="kof98umh" width="125"/> |
 | :------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------: |
 |                                             Dead<br>Or<br>Alive ++                                             |                                        Street<br>Fighter III<br>3rd Strike                                         |                                              Tekken Tag<br>Tournament                                              |                                        Ultimate<br>Mortal<br>Kombat 3                                        |                                           Samurai<br>Showdown<br>5 Special                                           |                                 The King of<br>Fighers '98<br>Ultimate<br>Match Hero                                 |
 
+| <img src="https://raw.githubusercontent.com/diambra/arena/main/img/mvsc.jpg" alt="mvsc" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/xmvsf.jpg" alt="xmvsf" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/soulclbr.jpg" alt="soulclbr" width="125"/> |
+| :------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------: |
+|                                             Marvel<br>VS<br>Capcom                                             |                                        X-Men<br>VS<br>Street Fighter                                         |                                              Soul<br>Calibur                                              |
+
 **Many more are coming soon...**
 
 ## Competition Platform
 
 <img src="https://raw.githubusercontent.com/diambra/.github/master/img/platform.jpg" alt="DIAMBRA Competition Platform" width="100%"/>
 
 Our competition platform allows you to submit your agents and compete with other coders around the globe in epic video games tournaments!
```

#### html2text {}

```diff
@@ -63,15 +63,25 @@
 Tournament | Ultimate
 Mortal
 Kombat 3 | Samurai
 Showdown
 5 Special | The King of
 Fighers '98
 Ultimate
-Match Hero | **Many more are coming soon...** ## Competition Platform [DIAMBRA
+Match Hero | | [mvsc]| [xmvsf]| [soulclbr]| | :--------------------------------
+----------------------------------------------------------------------------: |
+:------------------------------------------------------------------------------
+----------------------------------: | :----------------------------------------
+------------------------------------------------------------------------: | |
+Marvel
+VS
+Capcom | X-Men
+VS
+Street Fighter | Soul
+Calibur | **Many more are coming soon...** ## Competition Platform [DIAMBRA
 Competition Platform]Our competition platform allows you to submit your agents
 and compete with other coders around the globe in epic video games tournaments!
 It features a public global leaderboard where users are ranked by the best
 score achieved by their agents in our different environments. It also offers
 you the possibility to unlock cool achievements depending on the performances
 of your agent. Submitted agents are evaluated and their episodes are streamed
 on our Twitch channel. We aimed at making the submission process as smooth as
```

### Comparing `diambra-arena-2.2.6/diambra/arena/arena_gym.py` & `diambra_arena-2.2.7/diambra/arena/arena_gym.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,17 @@
             for k, v in sorted(observation.items()):
                 self.show_obs(v, wait_key=wait_key, viz=viz, string=string + "[\"{}\"]".format(k), key=k, outermost=False)
         else:
             if key != "frame":
                 if key.startswith("character"):
                     char_idx = observation if type(observation) == int else np.where(observation == 1)[0][0]
                     print(string + ": {} / {}".format(observation, self.env_info.characters_info.char_list[char_idx]))
+                elif key == "partner":
+                    partner_idx = observation if type(observation) == int else np.where(observation == 1)[0][0]
+                    print(string + ": {} / {}".format(observation, self.env_info.characters_info.partner_list[partner_idx]))
                 else:
                     print(string + ": {}".format(observation))
             else:
                 print(string + ": shape {} - min {} - max {}".format(observation.shape, np.amin(observation), np.amax(observation)))
 
                 if viz is True and (sys.platform.startswith('linux') is False or 'DISPLAY' in os.environ):
                     try:
```

### Comparing `diambra-arena-2.2.6/diambra/arena/engine/interface.py` & `diambra_arena-2.2.7/diambra/arena/engine/interface.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.2.6/diambra/arena/env_settings.py` & `diambra_arena-2.2.7/diambra/arena/env_settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     tower: Union[None, int] = 3  # UMK3 Specific
 
     # Bookkeeping variables
     _last_seed: Union[None, int] = None
     pb_model: model = None
 
     episode_settings = ["seed", "difficulty", "continue_game", "show_final", "tower", "role",
-                        "characters", "outfits", "super_art", "fighting_style", "ultimate_style"]
+                        "characters", "outfits", "super_art", "fighting_style", "ultimate_style", "speed_mode"]
 
     # Transforming env settings dict to pb request
     def get_pb_request(self, init=False):
         frame_shape = {
             "h": self.frame_shape[0],
             "w": self.frame_shape[1],
             "c": self.frame_shape[2]
@@ -213,16 +213,17 @@
     action_space: int = SpaceTypes.MULTI_DISCRETE
 
     # Episode settings
     role: Union[None, int] = None
     characters: Union[None, str, Tuple[str], Tuple[str, str], Tuple[str, str, str]] = None
     outfits: int = 1
     super_art: Union[None, int] = None  # SFIII Specific
-    fighting_style: Union[None, int] = None # KOF Specific
+    fighting_style: Union[None, int] = None # KOF, MVSC Specific
     ultimate_style: Union[None, Tuple[int, int, int]] = None # KOF Specific
+    speed_mode: Union[None, int] = None # MVSC, XMVSF Specific
 
     def _sanity_check(self):
         super()._sanity_check()
 
         # Env settings
         check_num_in_range("n_players", self.n_players, [1, 1])
         check_space_type("action_space", self.action_space, [SpaceTypes.DISCRETE, SpaceTypes.MULTI_DISCRETE])
@@ -237,18 +238,23 @@
                 self.characters += (None, )
         char_list = list(self.env_info.characters_info.char_list)
         char_list.append(None)
         for idx in range(3):
             check_val_in_list("characters[{}]".format(idx), self.characters[idx], char_list)
         check_num_in_range("outfits", self.outfits, self.games_dict[self.game_id]["outfits"])
         check_val_in_list("super_art", self.super_art, [None, 1, 2, 3])
-        check_val_in_list("fighting_style", self.fighting_style, [None, 1, 2, 3])
+        if self.game_id == "kof98umh":
+            check_val_in_list("fighting_style", self.fighting_style, [None, 1, 2, 3])
+        else:
+            check_val_in_list("fighting_style", self.fighting_style, [None, 1, 2])
+
         if self.ultimate_style is not None:
             for idx in range(3):
                 check_val_in_list("ultimate_style[{}]".format(idx), self.ultimate_style[idx], [1, 2])
+        check_val_in_list("speed_mode", self.speed_mode, [None, 1, 2])
 
     def _get_action_spaces(self):
         return [self.action_space]
 
     def _process_random_values(self):
         super()._process_random_values()
 
@@ -262,26 +268,32 @@
         self.characters = tuple(characters_tmp)
 
         if self.role is None:
             self.role = random.choice([Roles.P1, Roles.P2])
         if self.super_art is None:
             self.super_art = random.choice(list(range(1, 4)))
         if self.fighting_style is None:
-            self.fighting_style = random.choice(list(range(1, 4)))
+            maxFightingStyle = 3
+            if self.game_id == "kof98umh":
+                maxFightingStyle = 4
+            self.fighting_style = random.choice(list(range(1, maxFightingStyle)))
         if self.ultimate_style is None:
             self.ultimate_style = tuple([random.choice(list(range(1, 3))) for _ in range(3)])
+        if self.speed_mode is None:
+            self.speed_mode = random.choice(list(range(1, 3)))
 
     def _get_player_specific_values(self):
         player_settings = model.EnvSettings.EpisodeSettings.PlayerSettings(
             role=self.role,
             characters=[self.characters[idx] for idx in range(self.env_info.characters_info.chars_to_select)],
             outfits=self.outfits,
             super_art=self.super_art,
             fighting_style=self.fighting_style,
-            ultimate_style={"dash": self.ultimate_style[0], "evade": self.ultimate_style[1], "bar": self.ultimate_style[2]}
+            ultimate_style={"dash": self.ultimate_style[0], "evade": self.ultimate_style[1], "bar": self.ultimate_style[2]},
+            speed_mode=self.speed_mode,
         )
 
         return [player_settings]
 
 @dataclass
 class EnvironmentSettingsMultiAgent(EnvironmentSettingsBase):
     """Multi Agent Environment Settings Class"""
@@ -292,16 +304,17 @@
     # Episode Settings
     role: Union[Tuple[None, None], Tuple[int, int]] = (None, None)
     characters: Union[Tuple[None, None], Tuple[str, None], Tuple[None, str], Tuple[str, str],
                       Tuple[Tuple[str], Tuple[str]], Tuple[Tuple[str, str], Tuple[str, str]],
                       Tuple[Tuple[str, str, str], Tuple[str, str, str]]] = (None, None)
     outfits: Tuple[int, int] = (1, 1)
     super_art: Union[Tuple[None, None], Tuple[int, int]] = (None, None)  # SFIII Specific
-    fighting_style: Union[Tuple[None, None], Tuple[int, int]] = (None, None)  # KOF Specific
+    fighting_style: Union[Tuple[None, None], Tuple[int, int]] = (None, None)  # KOF, MVSC Specific
     ultimate_style: Union[Tuple[None, None], Tuple[Tuple[int, int, int], Tuple[int, int, int]]] = (None, None)  # KOF Specific
+    speed_mode: Union[Tuple[None, None], Tuple[int, int]] = (None, None)  # MVSC, XMVSF Specific
 
     def _sanity_check(self):
         super()._sanity_check()
 
         # Env Settings
         check_num_in_range("n_players", self.n_players, [2, 2])
         for idx in range(2):
@@ -321,18 +334,22 @@
         for idx in range(2):
             if self.role[idx] is not None:
                 check_roles("role[{}]".format(idx), self.role[idx], [Roles.P1, Roles.P2])
             for jdx in range(3):
                 check_val_in_list("characters[{}][{}]".format(idx, jdx), self.characters[idx][jdx], char_list)
             check_num_in_range("outfits[{}]".format(idx), self.outfits[idx], self.games_dict[self.game_id]["outfits"])
             check_val_in_list("super_art[{}]".format(idx), self.super_art[idx], [None, 1, 2, 3])
-            check_val_in_list("fighting_style[{}]".format(idx), self.fighting_style[idx], [None, 1, 2, 3])
+            if self.game_id == "kof98umh":
+                check_val_in_list("fighting_style[{}]".format(idx), self.fighting_style[idx], [None, 1, 2, 3])
+            else:
+                check_val_in_list("fighting_style[{}]".format(idx), self.fighting_style[idx], [None, 1, 2])
             if self.ultimate_style[idx] is not None:
                 for jdx in range(3):
                     check_val_in_list("ultimate_style[{}][{}]".format(idx, jdx), self.ultimate_style[idx][jdx], [1, 2])
+            check_val_in_list("speed_mode[{}]".format(idx), self.speed_mode[idx], [None, 1, 2])
 
     def _process_random_values(self):
         super()._process_random_values()
 
         characters_tmp = [[],[]]
 
         for idx, characters in enumerate(self.characters):
@@ -352,31 +369,36 @@
             else:
                 self.role = (Roles.P1 if self.role[1] == Roles.P2 else Roles.P2, self.role[1])
         else:
             if self.role[1] is None:
                 self.role = (self.role[0], Roles.P1 if self.role[0] == Roles.P2 else Roles.P2)
 
         self.super_art = tuple([random.choice(list(range(1, 4))) if self.super_art[idx] is None else self.super_art[idx] for idx in range(2)])
-        self.fighting_style = tuple([random.choice(list(range(1, 4))) if self.fighting_style[idx] is None else self.fighting_style[idx] for idx in range(2)])
+        maxFightingStyle = 3
+        if self.game_id == "kof98umh":
+            maxFightingStyle = 4
+        self.fighting_style = tuple([random.choice(list(range(1, maxFightingStyle))) if self.fighting_style[idx] is None else self.fighting_style[idx] for idx in range(2)])
         self.ultimate_style = tuple([[random.choice(list(range(1, 3))) for _ in range(3)] if self.ultimate_style[idx] is None else self.ultimate_style[idx] for idx in range(2)])
+        self.speed_mode = tuple([random.choice(list(range(1, 3))) if self.speed_mode[idx] is None else self.speed_mode[idx] for idx in range(2)])
 
     def _get_action_spaces(self):
         return [action_space for action_space in self.action_space]
 
     def _get_player_specific_values(self):
         players_env_settings = []
 
         for idx in range(2):
             player_settings = model.EnvSettings.EpisodeSettings.PlayerSettings(
                 role=self.role[idx],
                 characters=[self.characters[idx][jdx] for jdx in range(self.env_info.characters_info.chars_to_select)],
                 outfits=self.outfits[idx],
                 super_art=self.super_art[idx],
                 fighting_style=self.fighting_style[idx],
-                ultimate_style={"dash": self.ultimate_style[idx][0], "evade": self.ultimate_style[idx][1], "bar": self.ultimate_style[idx][2]}
+                ultimate_style={"dash": self.ultimate_style[idx][0], "evade": self.ultimate_style[idx][1], "bar": self.ultimate_style[idx][2]},
+                speed_mode=self.speed_mode[idx],
             )
 
             players_env_settings.append(player_settings)
 
         return players_env_settings
 
 @dataclass
@@ -403,15 +425,15 @@
     def sanity_check(self):
         check_num_in_range("no_op_max", self.no_op_max, [0, 12])
         check_num_in_range("repeat_action", self.repeat_action, [1, 12])
         check_type("normalize_reward", self.normalize_reward, bool, admit_none=False)
         check_num_in_range("normalization_factor", self.normalization_factor, [0.0, 1000000])
         check_type("clip_reward", self.clip_reward, bool, admit_none=False)
         check_type("no_attack_buttons_combinations", self.no_attack_buttons_combinations, bool, admit_none=False)
-        check_val_in_list("frame_shape[2]", self.frame_shape[2], [0, 1, 3])
+        check_val_in_list("frame_shape[2]", self.frame_shape[2], [0, 1])
         check_num_in_range("frame_shape[0]", self.frame_shape[0], [0, MAX_FRAME_RES])
         check_num_in_range("frame_shape[1]", self.frame_shape[1], [0, MAX_FRAME_RES])
         if (min(self.frame_shape[0], self.frame_shape[1]) == 0 and
             max(self.frame_shape[0], self.frame_shape[1]) != 0):
             raise Exception("\"frame_shape[0] and frame_shape[1]\" must be both different from 0")
         check_num_in_range("stack_frames", self.stack_frames, [1, MAX_STACK_VALUE])
         check_num_in_range("dilation", self.dilation, [1, MAX_STACK_VALUE])
```

### Comparing `diambra-arena-2.2.6/diambra/arena/make_env.py` & `diambra_arena-2.2.7/diambra/arena/make_env.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.2.6/diambra/arena/ray_rllib/make_ray_env.py` & `diambra_arena-2.2.7/diambra/arena/ray_rllib/make_ray_env.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.2.6/diambra/arena/sheeprl/make_sheeprl_env.py` & `diambra_arena-2.2.7/diambra/arena/sheeprl/make_sheeprl_env.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.2.6/diambra/arena/stable_baselines/make_sb_env.py` & `diambra_arena-2.2.7/diambra/arena/stable_baselines/make_sb_env.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.2.6/diambra/arena/stable_baselines/sb_utils.py` & `diambra_arena-2.2.7/diambra/arena/stable_baselines/sb_utils.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.2.6/diambra/arena/stable_baselines3/make_sb3_env.py` & `diambra_arena-2.2.7/diambra/arena/stable_baselines3/make_sb3_env.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.2.6/diambra/arena/stable_baselines3/sb3_utils.py` & `diambra_arena-2.2.7/diambra/arena/stable_baselines3/sb3_utils.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.2.6/diambra/arena/utils/.splash_screen.gif` & `diambra_arena-2.2.7/diambra/arena/utils/.splash_screen.gif`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.2.6/diambra/arena/utils/controller.py` & `diambra_arena-2.2.7/diambra/arena/utils/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     def __init__(self, device, action_list=(("NoMove", "Left", "UpLeft", "Up", "UpRight", "Right", "DownRight", "Down", "DownLeft"),
                                             ("But0", "But1", "But2", "But3", "But4", "But5", "But6", "But7", "But8")),
                  cfg=["But1", "But2", "But3", "But4", "But5", "But6", "But7", "But8"],
                  force_configure=False, skip_configure=False, logging_level=logging.INFO):
         # thread init class (don't forget this)
         Thread.__init__(self, daemon=True)
         self.logger = logging.getLogger(__name__)
-        self.logger.basicConfig(logging_level)
+        self.logger.setLevel(logging_level)
 
         self.stop_event = Event()
 
         self.start_code = ""
         self.select_code = ""
         self.start_but = 0
         self.select_but = 0
```

### Comparing `diambra-arena-2.2.6/diambra/arena/utils/diambra_data_loader.py` & `diambra_arena-2.2.7/diambra/arena/utils/diambra_data_loader.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.2.6/diambra/arena/utils/engine_mock.py` & `diambra_arena-2.2.7/diambra/arena/utils/engine_mock.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.2.6/diambra/arena/utils/gym_utils.py` & `diambra_arena-2.2.7/diambra/arena/utils/gym_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,26 +93,14 @@
         if isinstance(v, gym.spaces.dict.Dict):
             standard_dict[k] = gym_obs_dict_space_to_standard_dict(v)
         else:
             standard_dict[k] = v
 
     return standard_dict
 
-# Utility to create a Gym compliant Dict Space from the InternalObsDict
-def standard_dict_to_gym_obs_dict(obsstandard_dict):
-
-    for k, v in obsstandard_dict.items():
-        if isinstance(v, dict):
-            obsstandard_dict[k] = standard_dict_to_gym_obs_dict(v)
-        else:
-            obsstandard_dict[k] = v
-
-    return spaces.Dict(obsstandard_dict)
-
-
 # Discrete to multidiscrete action conversion
 def discrete_to_multi_discrete_action(action, n_move_actions):
 
     mov_act = 0
     att_act = 0
 
     if action <= n_move_actions - 1:
```

### Comparing `diambra-arena-2.2.6/diambra/arena/utils/integratedGames.json` & `diambra_arena-2.2.7/diambra/arena/utils/integratedGames.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'mvsc'": "OrderedDict([('name', 'Marvel VS Capcom'), ('id', 'mvsc'), ('original_rom_name', "*

 * *           "'mvsc.zip'), ('search_keywords', ['marvel vs capcom clash of super heroes', "*

 * *           "'marvel-vs.-capcom-clash-of-super-heroes-euro-980123', '5511', 'wowroms']), ('notes', "*

 * *           "'Requires the QSound_HLE sound driver to be placed in the roms folder. Search "*

 * *           'keywords: "qsound_hle.zip", "dl-1425.bin"\'), (\'nvram_save\', \'\'), (\'sha256\', '*

 * *           "'6f63627cc37c554f74e8bf07b […]*

```diff
@@ -282,14 +282,212 @@
             "The King Of Fighters '98: Ultimate Match HERO",
             "kof98umh",
             "allmyroms"
         ],
         "sha256": "beb7bdea87137832f5f6d731fd1abd0350c0cd6b6b2d57cab2bedbac24fe8d0a",
         "stages_per_game": 7
     },
+    "mvsc": {
+        "cfg": {
+            "MK": "But5",
+            "MP": "But2",
+            "SK": "But6",
+            "SP": "But3",
+            "WK": "But4",
+            "WP": "But1"
+        },
+        "char_forbidden_list": [
+            "Roll",
+            "Onslaught",
+            "Alt-Venom",
+            "Alt-Hulk",
+            "Alt-War Machine",
+            "Shadow Lady",
+            "Alt-Morrigan"
+        ],
+        "char_homonymy_map": {},
+        "char_list": [
+            "Chun-Li",
+            "Ryu",
+            "Zangief",
+            "Morrigan",
+            "Captain Commando",
+            "Megaman",
+            "Strider Hiryu",
+            "Spider Man",
+            "Jin",
+            "Captain America",
+            "Venom",
+            "Hulk",
+            "Gambit",
+            "War Machine",
+            "Wolverine",
+            "Roll",
+            "Onslaught",
+            "Alt-Venom",
+            "Alt-Hulk",
+            "Alt-War Machine",
+            "Shadow Lady",
+            "Alt-Morrigan"
+        ],
+        "cluster_to_difficulty_map": {
+            "Easy": 4,
+            "Hard": 8,
+            "Medium": 6
+        },
+        "difficulty": [
+            1,
+            8,
+            2
+        ],
+        "difficulty_to_cluster_map": {
+            "1": "Easy",
+            "2": "Easy",
+            "3": "Easy",
+            "4": "Easy",
+            "5": "Medium",
+            "6": "Medium",
+            "7": "Hard",
+            "8": "Hard"
+        },
+        "frame_shape": [
+            224,
+            384,
+            3
+        ],
+        "health": [
+            0,
+            144
+        ],
+        "id": "mvsc",
+        "n_actions": [
+            9,
+            19,
+            7
+        ],
+        "name": "Marvel VS Capcom",
+        "notes": "Requires the QSound_HLE sound driver to be placed in the roms folder. Search keywords: \"qsound_hle.zip\", \"dl-1425.bin\"",
+        "number_of_chars_per_round": 2,
+        "number_of_chars_to_select": 2,
+        "nvram_save": "",
+        "original_rom_name": "mvsc.zip",
+        "outfits": [
+            1,
+            2
+        ],
+        "partner_list": [
+            "Lou",
+            "Juggernaut",
+            "Magneto",
+            "Psylocke",
+            "Cyclops",
+            "Colossus",
+            "Unknown Soldier",
+            "Ton Pooh",
+            "Arthur",
+            "Saki",
+            "Miechele Heart",
+            "Thor",
+            "Storm",
+            "Rogue",
+            "Iceman",
+            "Pure&Fur",
+            "US Agent",
+            "Anita",
+            "Devilot",
+            "Jubilee",
+            "Shadow",
+            "Sentinel"
+        ],
+        "ram_states": {
+            "Px": {
+                "active_character": [
+                    "BINARY",
+                    0,
+                    1
+                ],
+                "character": [
+                    "DISCRETE",
+                    0,
+                    21
+                ],
+                "character_1": [
+                    "DISCRETE",
+                    0,
+                    21
+                ],
+                "character_2": [
+                    "DISCRETE",
+                    0,
+                    21
+                ],
+                "health_1": [
+                    "BOX",
+                    0,
+                    144
+                ],
+                "health_2": [
+                    "BOX",
+                    0,
+                    144
+                ],
+                "partner": [
+                    "DISCRETE",
+                    0,
+                    21
+                ],
+                "partner_attacks": [
+                    "BOX",
+                    0,
+                    9
+                ],
+                "side": [
+                    "BINARY",
+                    0,
+                    1
+                ],
+                "super_bar": [
+                    "BOX",
+                    0,
+                    144
+                ],
+                "super_count": [
+                    "BOX",
+                    0,
+                    3
+                ],
+                "wins": [
+                    "BOX",
+                    0,
+                    1
+                ]
+            },
+            "common": {
+                "stage": [
+                    "BOX",
+                    1,
+                    8
+                ],
+                "timer": [
+                    "BOX",
+                    0,
+                    99
+                ]
+            }
+        },
+        "rounds_per_stage": 1,
+        "search_keywords": [
+            "marvel vs capcom clash of super heroes",
+            "marvel-vs.-capcom-clash-of-super-heroes-euro-980123",
+            "5511",
+            "wowroms"
+        ],
+        "sha256": "6f63627cc37c554f74e8bf07b21730fa7f85511c7d5d07449850be98dde91da8",
+        "stages_per_game": 8
+    },
     "samsh5sp": {
         "cfg": {
             "K": "But3",
             "M": "But4",
             "MS": "But2",
             "WS": "But1"
         },
@@ -603,14 +801,133 @@
             "street-fighter-iii-3rd-strike-fight-for-the-futur-japan-clone",
             "106255",
             "wowroms"
         ],
         "sha256": "7239b5eb005488db22ace477501c574e9420c0ab70aeeb0795dfeb474284d416",
         "stages_per_game": 10
     },
+    "soulclbr": {
+        "cfg": {
+            "G": "But4",
+            "HA": "But1",
+            "K": "But3",
+            "VA": "But2"
+        },
+        "char_forbidden_list": [
+            "Inferno"
+        ],
+        "char_homonymy_map": {},
+        "char_list": [
+            "Xianghua",
+            "Yoshimitsu",
+            "Lizard Man",
+            "Siegfried",
+            "Rock",
+            "Seung Mina",
+            "Edge Master",
+            "Voldo",
+            "Ivy",
+            "Sophitia",
+            "Arthur",
+            "Kilik",
+            "Hwang",
+            "Maxi",
+            "Nightmare",
+            "Taki",
+            "Astaroth",
+            "Inferno"
+        ],
+        "cluster_to_difficulty_map": {
+            "Easy": 3,
+            "Hard": 5,
+            "Medium": 4
+        },
+        "difficulty": [
+            1,
+            5,
+            3
+        ],
+        "difficulty_to_cluster_map": {
+            "1": "Easy",
+            "2": "Easy",
+            "3": "Easy",
+            "4": "Medium",
+            "5": "Hard"
+        },
+        "frame_shape": [
+            240,
+            512,
+            3
+        ],
+        "health": [
+            0,
+            240
+        ],
+        "id": "soulclbr",
+        "n_actions": [
+            9,
+            13,
+            5
+        ],
+        "name": "Soul Calibur",
+        "notes": "",
+        "number_of_chars_per_round": 1,
+        "number_of_chars_to_select": 1,
+        "nvram_save": "at28c16",
+        "original_rom_name": "soulclbr.zip",
+        "outfits": [
+            1,
+            2
+        ],
+        "ram_states": {
+            "Px": {
+                "character": [
+                    "DISCRETE",
+                    0,
+                    17
+                ],
+                "health": [
+                    "BOX",
+                    0,
+                    240
+                ],
+                "side": [
+                    "BINARY",
+                    0,
+                    1
+                ],
+                "wins": [
+                    "BOX",
+                    0,
+                    2
+                ]
+            },
+            "common": {
+                "stage": [
+                    "BOX",
+                    1,
+                    8
+                ],
+                "timer": [
+                    "BOX",
+                    0,
+                    40
+                ]
+            }
+        },
+        "rounds_per_stage": 2,
+        "search_keywords": [
+            "soul calibur",
+            "soul-calibur",
+            "106959",
+            "wowroms"
+        ],
+        "sha256": "a07a1a19995d582b56f2865783c5d7adb7acb9a6ad995a26fc7c4cfecd821817",
+        "stages_per_game": 8
+    },
     "tektagt": {
         "cfg": {
             "LK": "But3",
             "LP": "But4",
             "RK": "But2",
             "RP": "But1",
             "TAG": "But6"
@@ -920,9 +1237,165 @@
             "ULTIMATE MORTAL KOMBAT 3 (CLONE)",
             "ultimate-mortal-kombat-3-clone",
             "109574",
             "wowroms"
         ],
         "sha256": "f48216ad82f78cb86e9c07d2507be347f904f4b5ae354a85ae7c34d969d265af",
         "stages_per_game": 11
+    },
+    "xmvsf": {
+        "cfg": {
+            "MK": "But5",
+            "MP": "But2",
+            "SK": "But6",
+            "SP": "But3",
+            "WK": "But4",
+            "WP": "But1"
+        },
+        "char_forbidden_list": [
+            "Apocalypse",
+            "Alpha Chun-Li"
+        ],
+        "char_homonymy_map": {},
+        "char_list": [
+            "Akuma",
+            "Magneto",
+            "Juggernaut",
+            "Dhalsim",
+            "Mr. Bison",
+            "Sabretooth",
+            "Storm",
+            "Chun-Li",
+            "Zangief",
+            "Gambit",
+            "Rogue",
+            "Cammy",
+            "Charlie",
+            "Wolverine",
+            "Cyclops",
+            "Ryu",
+            "Ken",
+            "Apocalypse",
+            "Alpha Chun-Li"
+        ],
+        "cluster_to_difficulty_map": {
+            "Easy": 4,
+            "Hard": 8,
+            "Medium": 6
+        },
+        "difficulty": [
+            1,
+            8,
+            2
+        ],
+        "difficulty_to_cluster_map": {
+            "1": "Easy",
+            "2": "Easy",
+            "3": "Easy",
+            "4": "Easy",
+            "5": "Medium",
+            "6": "Medium",
+            "7": "Hard",
+            "8": "Hard"
+        },
+        "frame_shape": [
+            224,
+            384,
+            3
+        ],
+        "health": [
+            0,
+            144
+        ],
+        "id": "xmvsf",
+        "n_actions": [
+            9,
+            18,
+            7
+        ],
+        "name": "X-Men VS Street Fighter",
+        "notes": "Requires the QSound_HLE sound driver to be placed in the roms folder. Search keywords: \"qsound_hle.zip\", \"dl-1425.bin\"",
+        "number_of_chars_per_round": 2,
+        "number_of_chars_to_select": 2,
+        "nvram_save": "",
+        "original_rom_name": "xmvsf.zip",
+        "outfits": [
+            1,
+            2
+        ],
+        "ram_states": {
+            "Px": {
+                "active_character": [
+                    "BINARY",
+                    0,
+                    1
+                ],
+                "character": [
+                    "DISCRETE",
+                    0,
+                    18
+                ],
+                "character_1": [
+                    "DISCRETE",
+                    0,
+                    18
+                ],
+                "character_2": [
+                    "DISCRETE",
+                    0,
+                    18
+                ],
+                "health_1": [
+                    "BOX",
+                    0,
+                    144
+                ],
+                "health_2": [
+                    "BOX",
+                    0,
+                    144
+                ],
+                "side": [
+                    "BINARY",
+                    0,
+                    1
+                ],
+                "super_bar": [
+                    "BOX",
+                    0,
+                    144
+                ],
+                "super_count": [
+                    "BOX",
+                    0,
+                    3
+                ],
+                "wins": [
+                    "BOX",
+                    0,
+                    1
+                ]
+            },
+            "common": {
+                "stage": [
+                    "BOX",
+                    1,
+                    8
+                ],
+                "timer": [
+                    "BOX",
+                    0,
+                    99
+                ]
+            }
+        },
+        "rounds_per_stage": 1,
+        "search_keywords": [
+            "x-men vs street fighter",
+            "x-men-vs.-street-fighter-usa-961004",
+            "8769",
+            "wowroms"
+        ],
+        "sha256": "833aa46af63a3ad87f69ce2bacd85a4445f35a50e3aff4f793f069b205b51c60",
+        "stages_per_game": 8
     }
 }
```

### Comparing `diambra-arena-2.2.6/diambra/arena/utils/splash_screen.py` & `diambra_arena-2.2.7/diambra/arena/utils/splash_screen.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.2.6/diambra/arena/wrappers/arena_wrappers.py` & `diambra_arena-2.2.7/diambra/arena/wrappers/arena_wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
         native_frame_size = env.observation_space["frame"].shape
         if wrappers_settings.frame_shape[0] > native_frame_size[0] or wrappers_settings.frame_shape[1] > native_frame_size[1]:
             warning_message  = "Warning: \"frame_shape\" greater than game native frame shape.\n"
             warning_message += "   \"native frame shape\" = [" + str(native_frame_size[0])
             warning_message += " X " + str(native_frame_size[1]) + "]\n"
             warning_message += "   \"frame_shape\" = [" + str(wrappers_settings.frame_shape[0])
             warning_message += " X " + str(wrappers_settings.frame_shape[1]) + "]"
-            env.logger.warning(warning_message)
+            env.unwrapped.logger.warning(warning_message)
 
         env = WarpFrame(env, wrappers_settings.frame_shape[:2])
 
     # Stack #frameStack frames together
     if wrappers_settings.stack_frames > 1:
         env = FrameStack(env, wrappers_settings.stack_frames, wrappers_settings.dilation)
```

### Comparing `diambra-arena-2.2.6/diambra/arena/wrappers/episode_recording.py` & `diambra_arena-2.2.7/diambra/arena/wrappers/episode_recording.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         """
         gym.Wrapper.__init__(self, env)
         self.dataset_path = recording_settings.dataset_path
         self.username = recording_settings.username
 
         self.compression_parameters = [int(cv2.IMWRITE_JPEG_QUALITY), 80]
 
-        self.env.logger.info("Recording trajectories in \"{}\"".format(self.dataset_path))
+        self.unwrapped.logger.info("Recording trajectories in \"{}\"".format(self.dataset_path))
         os.makedirs(self.dataset_path, exist_ok=True)
 
     def reset(self, **kwargs):
         """
         Reset the environment and add requested info to the observation
         :return: observation
         """
```

### Comparing `diambra-arena-2.2.6/diambra/arena/wrappers/observation.py` & `diambra_arena-2.2.7/diambra/arena/wrappers/observation.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.2.6/diambra_arena.egg-info/PKG-INFO` & `diambra_arena-2.2.7/diambra_arena.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diambra-arena
-Version: 2.2.6
+Version: 2.2.7
 Summary: DIAMBRA™ Arena. Built with OpenAI Gym Python interface, easy to use, transforms popular video games into Reinforcement Learning environments
 Home-page: https://github.com/diambra/arena
 Author: DIAMBRA Team
 Author-email: info@diambra.ai
 License: Custom
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
@@ -13,25 +13,22 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Artificial Life
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Games/Entertainment :: Arcade
 Classifier: Topic :: Education
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: pip>=21
 Requires-Dist: importlib-metadata<=4.12.0; python_version <= "3.7"
-Requires-Dist: setuptools
-Requires-Dist: distro>=1
 Requires-Dist: gymnasium>=0.26.3
 Requires-Dist: inputs
 Requires-Dist: screeninfo
 Requires-Dist: tk
 Requires-Dist: opencv-python>=4.4.0.42
 Requires-Dist: grpcio
-Requires-Dist: diambra-engine~=2.2.0
+Requires-Dist: diambra-engine>=2.2.3
 Requires-Dist: dacite
 Provides-Extra: core
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-mock; extra == "tests"
 Requires-Dist: testresources; extra == "tests"
 Provides-Extra: stable-baselines
@@ -40,19 +37,18 @@
 Requires-Dist: protobuf==3.20.1; extra == "stable-baselines"
 Requires-Dist: pyyaml; extra == "stable-baselines"
 Provides-Extra: stable-baselines3
 Requires-Dist: stable-baselines3[extra]~=2.1.0; extra == "stable-baselines3"
 Requires-Dist: pyyaml; extra == "stable-baselines3"
 Provides-Extra: ray-rllib
 Requires-Dist: ray[rllib]~=2.7.0; extra == "ray-rllib"
-Requires-Dist: tensorflow; extra == "ray-rllib"
 Requires-Dist: torch; extra == "ray-rllib"
 Requires-Dist: pyyaml; extra == "ray-rllib"
 Provides-Extra: sheeprl
-Requires-Dist: sheeprl==0.5.1; extra == "sheeprl"
+Requires-Dist: sheeprl==0.5.5; extra == "sheeprl"
 Requires-Dist: importlib-resources==6.1.0; extra == "sheeprl"
 
 <img src="https://raw.githubusercontent.com/diambra/arena/main/img/github.jpg" alt="diambra" width="100%"/>
 
 <p align="center">
   <a href="https://docs.diambra.ai">Documentation</a> •
   <a href="https://diambra.ai/">Website</a>
@@ -121,14 +117,18 @@
 
 Additional details can be found in the <a href="https://docs.diambra.ai/envs/games/" target="_blank">dedicated section</a> of our Documentation.
 
 | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/doapp.jpg" alt="doapp" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/sfiii3n.jpg" alt="sfiii3n" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/tektagt.jpg" alt="tektagt" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/umk3.jpg" alt="umk3" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/samsh5sp.jpg" alt="samsh6sp" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/kof98umh.jpg" alt="kof98umh" width="125"/> |
 | :------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------: |
 |                                             Dead<br>Or<br>Alive ++                                             |                                        Street<br>Fighter III<br>3rd Strike                                         |                                              Tekken Tag<br>Tournament                                              |                                        Ultimate<br>Mortal<br>Kombat 3                                        |                                           Samurai<br>Showdown<br>5 Special                                           |                                 The King of<br>Fighers '98<br>Ultimate<br>Match Hero                                 |
 
+| <img src="https://raw.githubusercontent.com/diambra/arena/main/img/mvsc.jpg" alt="mvsc" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/xmvsf.jpg" alt="xmvsf" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/soulclbr.jpg" alt="soulclbr" width="125"/> |
+| :------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------: |
+|                                             Marvel<br>VS<br>Capcom                                             |                                        X-Men<br>VS<br>Street Fighter                                         |                                              Soul<br>Calibur                                              |
+
 **Many more are coming soon...**
 
 ## Competition Platform
 
 <img src="https://raw.githubusercontent.com/diambra/.github/master/img/platform.jpg" alt="DIAMBRA Competition Platform" width="100%"/>
 
 Our competition platform allows you to submit your agents and compete with other coders around the globe in epic video games tournaments!
```

#### html2text {}

```diff
@@ -1,36 +1,35 @@
-Metadata-Version: 2.1 Name: diambra-arena Version: 2.2.6 Summary: DIAMBRAâ¢
+Metadata-Version: 2.1 Name: diambra-arena Version: 2.2.7 Summary: DIAMBRAâ¢
 Arena. Built with OpenAI Gym Python interface, easy to use, transforms popular
 video games into Reinforcement Learning environments Home-page: https://
 github.com/diambra/arena Author: DIAMBRA Team Author-email: info@diambra.ai
 License: Custom Classifier: Development Status :: 3 - Alpha Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
 Scientific/Engineering :: Artificial Life Classifier: Topic :: Games/
 Entertainment Classifier: Topic :: Games/Entertainment :: Arcade Classifier:
 Topic :: Education Description-Content-Type: text/markdown License-File:
-LICENSE.txt Requires-Dist: pip>=21 Requires-Dist: importlib-metadata<=4.12.0;
-python_version <= "3.7" Requires-Dist: setuptools Requires-Dist: distro>=1
+LICENSE.txt Requires-Dist: importlib-metadata<=4.12.0; python_version <= "3.7"
 Requires-Dist: gymnasium>=0.26.3 Requires-Dist: inputs Requires-Dist:
 screeninfo Requires-Dist: tk Requires-Dist: opencv-python>=4.4.0.42 Requires-
-Dist: grpcio Requires-Dist: diambra-engine~=2.2.0 Requires-Dist: dacite
+Dist: grpcio Requires-Dist: diambra-engine>=2.2.3 Requires-Dist: dacite
 Provides-Extra: core Provides-Extra: tests Requires-Dist: pytest; extra ==
 "tests" Requires-Dist: pytest-mock; extra == "tests" Requires-Dist:
 testresources; extra == "tests" Provides-Extra: stable-baselines Requires-Dist:
 stable-baselines~=2.10.2; extra == "stable-baselines" Requires-Dist:
 gym<=0.21.0; extra == "stable-baselines" Requires-Dist: protobuf==3.20.1; extra
 == "stable-baselines" Requires-Dist: pyyaml; extra == "stable-baselines"
 Provides-Extra: stable-baselines3 Requires-Dist: stable-baselines3
 [extra]~=2.1.0; extra == "stable-baselines3" Requires-Dist: pyyaml; extra ==
 "stable-baselines3" Provides-Extra: ray-rllib Requires-Dist: ray[rllib]~=2.7.0;
-extra == "ray-rllib" Requires-Dist: tensorflow; extra == "ray-rllib" Requires-
-Dist: torch; extra == "ray-rllib" Requires-Dist: pyyaml; extra == "ray-rllib"
-Provides-Extra: sheeprl Requires-Dist: sheeprl==0.5.1; extra == "sheeprl"
-Requires-Dist: importlib-resources==6.1.0; extra == "sheeprl"[diambra]
+extra == "ray-rllib" Requires-Dist: torch; extra == "ray-rllib" Requires-Dist:
+pyyaml; extra == "ray-rllib" Provides-Extra: sheeprl Requires-Dist:
+sheeprl==0.5.5; extra == "sheeprl" Requires-Dist: importlib-resources==6.1.0;
+extra == "sheeprl"[diambra]
                            _D_o_c_u_m_e_n_t_a_t_i_o_n â¢ _W_e_b_s_i_t_e
             _L_i_n_k_e_d_i_n â¢ _D_i_s_c_o_r_d â¢ _T_w_i_t_c_h â¢ _Y_o_u_T_u_b_e â¢ _T_w_i_t_t_e_r
                                     _[_P_a_p_e_r_]
               _[_A_r_e_n_a_ _T_e_s_t_]_[_A_g_e_n_t_s_ _T_e_s_t_]_[_L_a_t_e_s_t_ _T_a_g_]_[_P_y_p_i_ _v_e_r_s_i_o_n_]
                        _[_S_u_p_p_o_r_t_e_d_ _O_S_]_[_L_a_s_t_ _D_o_c_s_ _U_p_d_a_t_e_]
 # DIAMBRA Arena ## Index - **[Overview](#overview)** - **[Competition Platform]
 (#competition-platform)** - **[Installation](#installation)** - **[Quickstart &
@@ -91,15 +90,25 @@
 Tournament | Ultimate
 Mortal
 Kombat 3 | Samurai
 Showdown
 5 Special | The King of
 Fighers '98
 Ultimate
-Match Hero | **Many more are coming soon...** ## Competition Platform [DIAMBRA
+Match Hero | | [mvsc]| [xmvsf]| [soulclbr]| | :--------------------------------
+----------------------------------------------------------------------------: |
+:------------------------------------------------------------------------------
+----------------------------------: | :----------------------------------------
+------------------------------------------------------------------------: | |
+Marvel
+VS
+Capcom | X-Men
+VS
+Street Fighter | Soul
+Calibur | **Many more are coming soon...** ## Competition Platform [DIAMBRA
 Competition Platform]Our competition platform allows you to submit your agents
 and compete with other coders around the globe in epic video games tournaments!
 It features a public global leaderboard where users are ranked by the best
 score achieved by their agents in our different environments. It also offers
 you the possibility to unlock cool achievements depending on the performances
 of your agent. Submitted agents are evaluated and their episodes are streamed
 on our Twitch channel. We aimed at making the submission process as smooth as
```

### Comparing `diambra-arena-2.2.6/diambra_arena.egg-info/SOURCES.txt` & `diambra_arena-2.2.7/diambra_arena.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE.txt
 MANIFEST.in
 README.md
+pyproject.toml
 setup.py
 diambra/__init__.py
 diambra/arena/__init__.py
 diambra/arena/arena_gym.py
 diambra/arena/env_settings.py
 diambra/arena/make_env.py
 diambra/arena/engine/__init__.py
@@ -22,15 +23,14 @@
 diambra/arena/utils/.splash_screen.gif
 diambra/arena/utils/__init__.py
 diambra/arena/utils/controller.py
 diambra/arena/utils/diambra_data_loader.py
 diambra/arena/utils/engine_mock.py
 diambra/arena/utils/gym_utils.py
 diambra/arena/utils/integratedGames.json
-diambra/arena/utils/policies.py
 diambra/arena/utils/splash_screen.py
 diambra/arena/wrappers/__init__.py
 diambra/arena/wrappers/arena_wrappers.py
 diambra/arena/wrappers/episode_recording.py
 diambra/arena/wrappers/observation.py
 diambra_arena.egg-info/PKG-INFO
 diambra_arena.egg-info/SOURCES.txt
```

### Comparing `diambra-arena-2.2.6/setup.py` & `diambra_arena-2.2.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,25 @@
 import os
 from pathlib import Path
 
 import setuptools
 
-try:
-    from pip import main as pipmain
-except ImportError:
-    from pip._internal import main as pipmain
-
-pipmain(["install", "setuptools"])
-pipmain(["install", "distro"])
-
 extras = {
     "core": [],
     "tests": ["pytest", "pytest-mock", "testresources"],
     "stable-baselines": [
         "stable-baselines~=2.10.2",
         "gym<=0.21.0",
         "protobuf==3.20.1",
         "pyyaml",
     ],
     "stable-baselines3": ["stable-baselines3[extra]~=2.1.0", "pyyaml"],
-    "ray-rllib": ["ray[rllib]~=2.7.0", "tensorflow", "torch", "pyyaml"],
+    "ray-rllib": ["ray[rllib]~=2.7.0", "torch", "pyyaml"],
     "sheeprl": [
-        "sheeprl==0.5.1",
+        "sheeprl==0.5.5",
         "importlib-resources==6.1.0",
     ],
 }
 
 # NOTE Package data is inside MANIFEST.In
 
 setuptools.setup(
@@ -37,25 +29,22 @@
     author="DIAMBRA Team",
     author_email="info@diambra.ai",
     description="DIAMBRA™ Arena. Built with OpenAI Gym Python interface, easy to use, transforms popular video games into Reinforcement Learning environments",
     long_description=(Path(__file__).parent / "README.md").read_text(),
     long_description_content_type="text/markdown",
     license="Custom",
     install_requires=[
-        "pip>=21",
         'importlib-metadata<=4.12.0; python_version <= "3.7"',  # problem with gym for importlib-metadata==5.0.0 and python <=3.7
-        "setuptools",
-        "distro>=1",
         "gymnasium>=0.26.3",
         "inputs",
         "screeninfo",
         "tk",
         "opencv-python>=4.4.0.42",
         "grpcio",
-        "diambra-engine~=2.2.0",
+        "diambra-engine>=2.2.3",
         "dacite",
     ],
     packages=[
         package
         for package in setuptools.find_packages()
         if package.startswith("diambra")
     ],
```

### Comparing `diambra-arena-2.2.6/tests/test_episode_data_loader.py` & `diambra_arena-2.2.7/tests/test_episode_data_loader.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.2.6/tests/test_examples.py` & `diambra_arena-2.2.7/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.2.6/tests/test_gym_settings.py` & `diambra_arena-2.2.7/tests/test_gym_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,53 +25,55 @@
     except Exception as e:
         print(e)
         print("ERROR, ABORTED.")
         return 1
 
 games_dict = available_games(False)
 gym_settings_var_order = ["frame_shape", "step_ratio", "action_space", "difficulty", "continue_game",
-                          "tower", "role", "characters", "super_art", "fighting_style", "ultimate_style"]
+                          "tower", "role", "characters", "super_art", "fighting_style", "ultimate_style", "speed_mode"]
 
 ok_test_parameters = {
     "frame_shape": [(0, 0, 0), (0, 0, 1), (82, 82, 0), (82, 82, 1)],
     "step_ratio": [1, 3, 6],
     "action_space": [SpaceTypes.DISCRETE, SpaceTypes.MULTI_DISCRETE],
     "difficulty": [None, 1, 3],
     "continue_game": [-1.0, 0.0, 0.3],
     "tower": [1, 3, 4],
     "role": [[Roles.P1, Roles.P2], [Roles.P2, Roles.P1], [None, None]],
     "characters": [[None, None], [None, "TBD"], ["TBD", "TBD"]],
     "super_art": [None, 1, 3],
-    "fighting_style": [None, 1, 3],
+    "fighting_style": [None, 1, 2, 3],
     "ultimate_style": [None, (2, 2, 2)],
+    "speed_mode": [None, 1, 2],
 }
 
 ko_test_parameters = {
     "frame_shape": [(0, 82, 0), (0, 0, 4), (-100, -100, 3)],
     "step_ratio": [8],
     "difficulty": [True, 0, "Random"],
     "action_space": ["Random", 12, "discrete", SpaceTypes.BOX],
     "continue_game": [1.3, "string"],
     "tower": [5],
     "role": [["P1", "P2"], [5, 4], ["P1P2", "Random"], ["Random", "Random"]],
     "characters": [["Random", "TBD"], ["NoName", None]],
     "super_art": ["Random", 4, 0],
     "fighting_style": [False, 6, 0, "Random"],
     "ultimate_style": [(10, 0, 0), "string", (None, None, None), ("Random", "Random", "Random")],
+    "speed_mode": [False, 6, 0, "Random"],
 }
 
 def pytest_generate_tests(metafunc):
     test_vars, values_list = generate_pytest_decorator_input(gym_settings_var_order, ok_test_parameters, ko_test_parameters)
     metafunc.parametrize(test_vars, values_list)
 
 # Gym
 @pytest.mark.parametrize("game_id", list(games_dict.keys()))
 @pytest.mark.parametrize("n_players", [1, 2])
 def test_gym_settings(game_id, n_players, frame_shape, step_ratio, action_space, difficulty, continue_game,
-                      tower, role, characters, super_art, fighting_style, ultimate_style, expected, mocker):
+                      tower, role, characters, super_art, fighting_style, ultimate_style, speed_mode, expected, mocker):
 
     game_data = games_dict[game_id]
 
     outfits_range = range(game_data["outfits"][0], game_data["outfits"][1] + 1)
     characters = [random.choice(game_data["char_list"]) if characters[idx] == "TBD" else characters[idx] for idx in range(2)]
     outfits = random.choice(outfits_range)
 
@@ -80,25 +82,29 @@
         settings = EnvironmentSettings()
     else:
         settings = EnvironmentSettingsMultiAgent()
     settings.game_id = game_id
     settings.frame_shape = frame_shape
     settings.step_ratio = step_ratio
     settings.action_space = (action_space, action_space)
+    settings.splash_screen = False
 
     settings.difficulty = difficulty
     settings.continue_game = continue_game
     settings.tower = tower
 
     settings.role = (role[0], role[1])
     settings.characters = (characters[0], characters[1])
     settings.outfits = (outfits, outfits)
     settings.super_art = (super_art, super_art)
+    if game_id != "kof98umh" and fighting_style == 3:
+        fighting_style = 2
     settings.fighting_style = (fighting_style, fighting_style)
     settings.ultimate_style = (ultimate_style, ultimate_style)
+    settings.speed_mode = (speed_mode, speed_mode)
 
     if n_players != 2:
         for key in ["action_space", "role", "characters" , "outfits",
-                    "super_art", "fighting_style", "ultimate_style"]:
+                    "super_art", "fighting_style", "ultimate_style", "speed_mode"]:
             setattr(settings, key, getattr(settings, key)[0])
 
     assert func(settings, mocker) == expected
```

### Comparing `diambra-arena-2.2.6/tests/test_random.py` & `diambra_arena-2.2.7/tests/test_random.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 import pytest
 from env_exec_interface import env_exec
 import random
 from diambra.arena.utils.engine_mock import load_mocker
 from diambra.arena import SpaceTypes, Roles, EnvironmentSettings, EnvironmentSettingsMultiAgent, WrappersSettings, RecordingSettings
+from diambra.arena.utils.gym_utils import available_games
 
 # Example Usage:
 # pytest
 # (optional)
 #    module.py (Run specific module)
 #    -s (show output)
 #    -k "expression" (filter tests using case-insensitive with parts of the test name and/or parameters values combined with boolean operators, e.g. "wrappers and doapp")
@@ -34,14 +35,15 @@
         if (n_players == 1):
             settings = EnvironmentSettings()
         else:
             settings = EnvironmentSettingsMultiAgent()
         settings.game_id = game_id
         settings.frame_shape = frame_shape
         settings.action_space = (action_space, action_space)
+        settings.splash_screen = False
         if settings.n_players == 1:
             settings.action_space = settings.action_space[0]
 
         # Options (settings to change at reset)
         options_list = []
         roles = [[Roles.P1, Roles.P2], [Roles.P2, Roles.P1]]
         for role in roles:
@@ -54,31 +56,31 @@
                 options_list.append({"role": role_value})
 
         return env_exec(settings, options_list, wrappers_settings, RecordingSettings(), args)
     except Exception as e:
         print(e)
         return 1
 
-game_ids = ["doapp", "sfiii3n", "tektagt", "umk3", "samsh5sp", "kof98umh"]
+games_dict = available_games(False)
 n_players = [1, 2]
 action_spaces = [SpaceTypes.DISCRETE, SpaceTypes.MULTI_DISCRETE]
 no_action_probabilities = [0.0, 1.0]
 
-@pytest.mark.parametrize("game_id", game_ids)
+@pytest.mark.parametrize("game_id", list(games_dict.keys()))
 @pytest.mark.parametrize("n_players", n_players)
 @pytest.mark.parametrize("action_space", action_spaces)
 @pytest.mark.parametrize("no_action_probability", no_action_probabilities)
 def test_random_gym_mock(game_id, n_players, action_space, no_action_probability, mocker):
-    frame_shape = random.choice([(128, 128, 1), (256, 256, 0)])
+    frame_shape = random.choice([(128, 128, 1), (128, 256, 1), (256, 256, 0)])
     continue_games = [0.0]
     use_mock_env = True
     assert func(game_id, n_players, action_space, frame_shape, WrappersSettings(),
                 no_action_probability, continue_games, use_mock_env, mocker) == 0
 
-@pytest.mark.parametrize("game_id", game_ids)
+@pytest.mark.parametrize("game_id", list(games_dict.keys()))
 @pytest.mark.parametrize("n_players", n_players)
 @pytest.mark.parametrize("action_space", action_spaces)
 @pytest.mark.parametrize("no_action_probability", no_action_probabilities)
 def test_random_wrappers_mock(game_id, n_players, action_space, no_action_probability, mocker):
     frame_shape = random.choice([(128, 128, 1), (256, 256, 0)])
     continue_games = [0.0]
     use_mock_env = True
@@ -102,15 +104,15 @@
         suffix = "agent_0_"
     wrappers_settings.filter_keys = ["stage", "timer", suffix + "own_side", suffix + "opp_side",
                                      suffix + "opp_character", suffix + "action"]
 
     assert func(game_id, n_players, action_space, frame_shape, wrappers_settings,
                 no_action_probability, continue_games, use_mock_env, mocker) == 0
 
-@pytest.mark.parametrize("game_id", game_ids)
+@pytest.mark.parametrize("game_id", list(games_dict.keys()))
 @pytest.mark.parametrize("n_players", n_players)
 @pytest.mark.parametrize("action_space", action_spaces)
 @pytest.mark.parametrize("no_action_probability", [0.0])
 def test_random_integration(game_id, n_players, action_space, no_action_probability, mocker):
     frame_shape = random.choice([(128, 128, 1), (256, 256, 0)])
     continue_games = [-1.0, 0.0, 0.3]
     use_mock_env = False
```

### Comparing `diambra-arena-2.2.6/tests/test_recording_settings.py` & `diambra_arena-2.2.7/tests/test_recording_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     # Env settings
     if (n_players == 1):
         settings = EnvironmentSettings()
     else:
         settings = EnvironmentSettingsMultiAgent()
     settings.game_id = game_id
     settings.action_space = action_space
+    settings.splash_screen = False
     if n_players == 2:
         settings.action_space = (action_space, action_space)
 
     # Env wrappers settings
     wrappers_settings = WrappersSettings()
     wrappers_settings.frame_shape = (128, 128, 1)
     wrappers_settings.normalize_reward = True
```

### Comparing `diambra-arena-2.2.6/tests/test_speed.py` & `diambra_arena-2.2.7/tests/test_speed.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 import pytest
 import time
 import diambra.arena
 from diambra.arena import EnvironmentSettings, EnvironmentSettingsMultiAgent, WrappersSettings
 from diambra.arena.utils.engine_mock import load_mocker
+from diambra.arena.utils.gym_utils import available_games
 import numpy as np
 import warnings
 
 def reject_outliers(data):
     u = np.mean(data)
     s = np.std(data)
     filtered = [e for e in data if (u - 2 * s < e < u + 2 * s)]
@@ -21,14 +22,15 @@
         if (n_players == 1):
             settings = EnvironmentSettings()
         else:
             settings = EnvironmentSettingsMultiAgent()
 
         settings.step_ratio = 1
         settings.frame_shape = (128, 128, 1)
+        settings.splash_screen = False
 
         env = diambra.arena.make(game_id, settings, wrappers_settings)
         observation, info = env.reset()
 
         n_step = 0
         fps_val = []
         while n_step < 1000:
@@ -53,15 +55,15 @@
 
         return 0
     except Exception as e:
         print(e)
         return 1
 
 n_players = [1, 2]
-game_ids = ["doapp", "sfiii3n", "tektagt", "umk3", "samsh5sp", "kof98umh"]
+games_dict = available_games(False)
 
 @pytest.mark.parametrize("n_players", n_players)
 def test_speed_gym_mock(n_players, mocker):
     use_mocker = True
     game_id = "doapp"
     assert func(game_id, n_players, WrappersSettings(), use_mocker, mocker) == 0
 
@@ -88,12 +90,39 @@
     if n_players == 2:
         suffix = "agent_0_"
     wrappers_settings.filter_keys = ["stage", "timer", suffix + "own_side", suffix + "opp_side",
                                      suffix + "opp_character", suffix + "action"]
 
     assert func(game_id, n_players, wrappers_settings, use_mocker, mocker) == 0
 
-@pytest.mark.parametrize("game_id", game_ids)
+@pytest.mark.parametrize("game_id", list(games_dict.keys()))
 @pytest.mark.parametrize("n_players", n_players)
 def test_speed_gym_integration(game_id, n_players, mocker):
     use_mocker = False
-    assert func(game_id, n_players, WrappersSettings(), use_mocker, mocker) == 0
+    assert func(game_id, n_players, WrappersSettings(), use_mocker, mocker) == 0
+
+@pytest.mark.parametrize("game_id", list(games_dict.keys()))
+@pytest.mark.parametrize("n_players", n_players)
+def test_speed_wrappers_integration(game_id, n_players, mocker):
+    use_mocker = False
+
+    # Env wrappers settings
+    wrappers_settings = WrappersSettings()
+    wrappers_settings.no_op_max = 0
+    wrappers_settings.repeat_action = 1
+    wrappers_settings.normalize_reward = True
+    wrappers_settings.clip_reward = False
+    wrappers_settings.stack_frames = 4
+    wrappers_settings.dilation = 1
+    wrappers_settings.add_last_action = True
+    wrappers_settings.stack_actions = 12
+    wrappers_settings.scale = True
+    wrappers_settings.role_relative = True
+    wrappers_settings.flatten = True
+
+    suffix = ""
+    if n_players == 2:
+        suffix = "agent_0_"
+    wrappers_settings.filter_keys = ["stage", "timer", suffix + "own_side", suffix + "opp_side",
+                                     suffix + "opp_character", suffix + "action"]
+
+    assert func(game_id, n_players, wrappers_settings, use_mocker, mocker) == 0
```

### Comparing `diambra-arena-2.2.6/tests/test_wrappers_settings.py` & `diambra_arena-2.2.7/tests/test_wrappers_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 ok_test_parameters = {
     "no_op_max": [0, 2],
     "repeat_action": [1, 4],
     "normalize_reward": [True, False],
     "normalization_factor": [0.2, 0.5],
     "clip_reward": [True, False],
     "no_attack_buttons_combinations": [True, False],
-    "frame_shape": [(0, 0, 0), (84, 84, 1), (84, 84, 3), (84, 84, 0)],
+    "frame_shape": [(0, 0, 0), (84, 84, 1), (84, 84, 0)],
     "stack_frames": [1, 5],
     "dilation": [1, 3],
     "add_last_action": [True, False],
     "stack_actions": [1, 6],
     "scale": [True, False],
     "role_relative": [True, False],
     "flatten": [True, False],
@@ -90,14 +90,15 @@
     if (n_players == 1):
         settings = EnvironmentSettings()
     else:
         settings = EnvironmentSettingsMultiAgent()
     settings.game_id = game_id
     settings.step_ratio = step_ratio
     settings.action_space = action_space
+    settings.splash_screen = False
     if n_players == 2:
         settings.action_space = (action_space, action_space)
 
     # Env wrappers settings
     wrappers_settings = WrappersSettings()
     wrappers_settings.no_op_max = no_op_max
     wrappers_settings.repeat_action = repeat_action
```

