# Comparing `tmp/cellworld_game-0.0.60.tar.gz` & `tmp/cellworld_game-0.0.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellworld_game-0.0.60.tar", last modified: Fri Apr 26 19:48:36 2024, max compression
+gzip compressed data, was "cellworld_game-0.0.61.tar", last modified: Mon Apr 29 16:23:50 2024, max compression
```

## Comparing `cellworld_game-0.0.60.tar` & `cellworld_game-0.0.61.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 19:48:36.814063 cellworld_game-0.0.60/
--rw-rw-rw-   0        0        0       36 2024-04-26 19:48:36.000000 cellworld_game-0.0.60/MANIFEST.in
--rw-rw-rw-   0        0        0      474 2024-04-26 19:48:36.813063 cellworld_game-0.0.60/PKG-INFO
--rw-rw-rw-   0        0        0       33 2024-04-26 19:48:36.000000 cellworld_game-0.0.60/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 19:48:36.774062 cellworld_game-0.0.60/cellworld_game/
--rw-rw-rw-   0        0        0       33 2024-04-26 19:48:36.000000 cellworld_game-0.0.60/cellworld_game/README.md
--rw-rw-rw-   0        0        0      447 2024-04-26 16:52:38.000000 cellworld_game-0.0.60/cellworld_game/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 19:48:36.797062 cellworld_game-0.0.60/cellworld_game/__pycache__/
--rw-rw-rw-   0        0        0      782 2024-04-26 16:52:40.000000 cellworld_game-0.0.60/cellworld_game/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0    10222 2024-04-26 17:03:42.000000 cellworld_game-0.0.60/cellworld_game/__pycache__/agent.cpython-312.pyc
--rw-rw-rw-   0        0        0     5043 2024-04-26 16:48:26.000000 cellworld_game-0.0.60/cellworld_game/__pycache__/cellworld_loader.cpython-312.pyc
--rw-rw-rw-   0        0        0     1424 2024-04-10 15:31:18.000000 cellworld_game-0.0.60/cellworld_game/__pycache__/geometry.cpython-312.pyc
--rw-rw-rw-   0        0        0     9662 2024-04-25 18:38:43.000000 cellworld_game-0.0.60/cellworld_game/__pycache__/model.cpython-312.pyc
--rw-rw-rw-   0        0        0     2208 2024-04-23 16:26:46.000000 cellworld_game-0.0.60/cellworld_game/__pycache__/mouse.cpython-312.pyc
--rw-rw-rw-   0        0        0     2598 2024-04-21 15:32:53.000000 cellworld_game-0.0.60/cellworld_game/__pycache__/navigation.cpython-312.pyc
--rw-rw-rw-   0        0        0     5807 2024-04-26 17:03:42.000000 cellworld_game-0.0.60/cellworld_game/__pycache__/navigation_agent.cpython-312.pyc
--rw-rw-rw-   0        0        0     6071 2024-04-21 15:32:53.000000 cellworld_game-0.0.60/cellworld_game/__pycache__/ray_tracing.cpython-312.pyc
--rw-rw-rw-   0        0        0      870 2024-04-21 15:16:32.000000 cellworld_game-0.0.60/cellworld_game/__pycache__/resources.cpython-312.pyc
--rw-rw-rw-   0        0        0     2743 2024-04-26 16:48:26.000000 cellworld_game-0.0.60/cellworld_game/__pycache__/robot.cpython-312.pyc
--rw-rw-rw-   0        0        0     9945 2024-04-23 16:16:30.000000 cellworld_game-0.0.60/cellworld_game/__pycache__/util.cpython-312.pyc
--rw-rw-rw-   0        0        0     9683 2024-04-26 17:03:42.000000 cellworld_game-0.0.60/cellworld_game/__pycache__/view.cpython-312.pyc
--rw-rw-rw-   0        0        0    10037 2024-04-11 19:37:36.000000 cellworld_game-0.0.60/cellworld_game/__pycache__/visibility.cpython-312.pyc
--rw-rw-rw-   0        0        0     6294 2024-04-26 17:03:41.000000 cellworld_game-0.0.60/cellworld_game/agent.py
--rw-rw-rw-   0        0        0     3712 2024-04-25 23:24:36.000000 cellworld_game-0.0.60/cellworld_game/cellworld_loader.py
-drwxrwxrwx   0        0        0        0 2024-04-26 19:48:36.801063 cellworld_game-0.0.60/cellworld_game/files/
--rw-rw-rw-   0        0        0     8477 2024-03-30 14:47:10.000000 cellworld_game-0.0.60/cellworld_game/files/agent.png
--rw-rw-rw-   0        0        0    41740 2024-04-02 20:09:30.000000 cellworld_game-0.0.60/cellworld_game/files/predator.png
--rw-rw-rw-   0        0        0    47356 2024-04-02 20:07:49.000000 cellworld_game-0.0.60/cellworld_game/files/prey.png
--rw-rw-rw-   0        0        0      431 2024-04-10 15:24:24.000000 cellworld_game-0.0.60/cellworld_game/geometry.py
--rw-rw-rw-   0        0        0     1636 2024-04-26 19:48:36.000000 cellworld_game-0.0.60/cellworld_game/license.txt
--rw-rw-rw-   0        0        0     7506 2024-04-26 19:45:27.000000 cellworld_game-0.0.60/cellworld_game/model.py
--rw-rw-rw-   0        0        0     1167 2024-04-23 16:26:41.000000 cellworld_game-0.0.60/cellworld_game/mouse.py
--rw-rw-rw-   0        0        0     1717 2024-04-21 15:19:56.000000 cellworld_game-0.0.60/cellworld_game/navigation.py
--rw-rw-rw-   0        0        0     4455 2024-04-26 17:03:41.000000 cellworld_game-0.0.60/cellworld_game/navigation_agent.py
--rw-rw-rw-   0        0        0     4973 2024-04-21 15:20:54.000000 cellworld_game-0.0.60/cellworld_game/ray_tracing.py
--rw-rw-rw-   0        0        0      220 2024-04-19 14:17:58.000000 cellworld_game-0.0.60/cellworld_game/resources.py
--rw-rw-rw-   0        0        0     1542 2024-04-26 16:24:32.000000 cellworld_game-0.0.60/cellworld_game/robot.py
--rw-rw-rw-   0        0        0      183 2024-04-26 19:48:36.000000 cellworld_game-0.0.60/cellworld_game/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-26 19:48:36.806062 cellworld_game-0.0.60/cellworld_game/tasks/
--rw-rw-rw-   0        0        0       92 2024-04-26 16:46:54.000000 cellworld_game-0.0.60/cellworld_game/tasks/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 19:48:36.810063 cellworld_game-0.0.60/cellworld_game/tasks/__pycache__/
--rw-rw-rw-   0        0        0      280 2024-04-26 16:48:27.000000 cellworld_game-0.0.60/cellworld_game/tasks/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     6831 2024-04-26 16:50:52.000000 cellworld_game-0.0.60/cellworld_game/tasks/__pycache__/botevade.cpython-312.pyc
--rw-rw-rw-   0        0        0     9943 2024-04-26 17:34:24.000000 cellworld_game-0.0.60/cellworld_game/tasks/__pycache__/dualevade.cpython-312.pyc
--rw-rw-rw-   0        0        0     9261 2024-04-26 16:51:24.000000 cellworld_game-0.0.60/cellworld_game/tasks/__pycache__/oasis.cpython-312.pyc
--rw-rw-rw-   0        0        0     5436 2024-04-26 17:38:02.000000 cellworld_game-0.0.60/cellworld_game/tasks/botevade.py
--rw-rw-rw-   0        0        0     8037 2024-04-26 17:47:12.000000 cellworld_game-0.0.60/cellworld_game/tasks/dualevade.py
--rw-rw-rw-   0        0        0     7476 2024-04-26 16:51:20.000000 cellworld_game-0.0.60/cellworld_game/tasks/oasis.py
--rw-rw-rw-   0        0        0     7912 2024-04-23 16:14:29.000000 cellworld_game-0.0.60/cellworld_game/util.py
--rw-rw-rw-   0        0        0     6637 2024-04-26 19:48:33.000000 cellworld_game-0.0.60/cellworld_game/view.py
--rw-rw-rw-   0        0        0     9497 2024-04-11 19:37:32.000000 cellworld_game-0.0.60/cellworld_game/visibility.py
-drwxrwxrwx   0        0        0        0 2024-04-26 19:48:36.812063 cellworld_game-0.0.60/cellworld_game.egg-info/
--rw-rw-rw-   0        0        0      474 2024-04-26 19:48:36.000000 cellworld_game-0.0.60/cellworld_game.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1902 2024-04-26 19:48:36.000000 cellworld_game-0.0.60/cellworld_game.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 19:48:36.000000 cellworld_game-0.0.60/cellworld_game.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-26 19:48:36.000000 cellworld_game-0.0.60/cellworld_game.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2024-04-26 19:48:36.000000 cellworld_game-0.0.60/cellworld_game.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-26 19:48:36.000000 cellworld_game-0.0.60/cellworld_game.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 19:48:36.814063 cellworld_game-0.0.60/setup.cfg
--rw-rw-rw-   0        0        0      667 2024-04-26 19:48:36.000000 cellworld_game-0.0.60/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:23:50.730209 cellworld_game-0.0.61/
+-rw-rw-rw-   0        0        0       36 2024-04-29 16:23:49.000000 cellworld_game-0.0.61/MANIFEST.in
+-rw-rw-rw-   0        0        0      474 2024-04-29 16:23:50.729208 cellworld_game-0.0.61/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2024-04-29 16:23:49.000000 cellworld_game-0.0.61/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 16:23:50.690217 cellworld_game-0.0.61/cellworld_game/
+-rw-rw-rw-   0        0        0       33 2024-04-29 16:23:49.000000 cellworld_game-0.0.61/cellworld_game/README.md
+-rw-rw-rw-   0        0        0      447 2024-04-26 16:52:38.000000 cellworld_game-0.0.61/cellworld_game/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:23:50.713208 cellworld_game-0.0.61/cellworld_game/__pycache__/
+-rw-rw-rw-   0        0        0      782 2024-04-26 16:52:40.000000 cellworld_game-0.0.61/cellworld_game/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0    10222 2024-04-26 17:03:42.000000 cellworld_game-0.0.61/cellworld_game/__pycache__/agent.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5043 2024-04-26 16:48:26.000000 cellworld_game-0.0.61/cellworld_game/__pycache__/cellworld_loader.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1424 2024-04-10 15:31:18.000000 cellworld_game-0.0.61/cellworld_game/__pycache__/geometry.cpython-312.pyc
+-rw-rw-rw-   0        0        0     9662 2024-04-25 18:38:43.000000 cellworld_game-0.0.61/cellworld_game/__pycache__/model.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2208 2024-04-23 16:26:46.000000 cellworld_game-0.0.61/cellworld_game/__pycache__/mouse.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2598 2024-04-21 15:32:53.000000 cellworld_game-0.0.61/cellworld_game/__pycache__/navigation.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5807 2024-04-26 17:03:42.000000 cellworld_game-0.0.61/cellworld_game/__pycache__/navigation_agent.cpython-312.pyc
+-rw-rw-rw-   0        0        0     6071 2024-04-21 15:32:53.000000 cellworld_game-0.0.61/cellworld_game/__pycache__/ray_tracing.cpython-312.pyc
+-rw-rw-rw-   0        0        0      870 2024-04-21 15:16:32.000000 cellworld_game-0.0.61/cellworld_game/__pycache__/resources.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2743 2024-04-26 16:48:26.000000 cellworld_game-0.0.61/cellworld_game/__pycache__/robot.cpython-312.pyc
+-rw-rw-rw-   0        0        0     9945 2024-04-23 16:16:30.000000 cellworld_game-0.0.61/cellworld_game/__pycache__/util.cpython-312.pyc
+-rw-rw-rw-   0        0        0     9683 2024-04-26 17:03:42.000000 cellworld_game-0.0.61/cellworld_game/__pycache__/view.cpython-312.pyc
+-rw-rw-rw-   0        0        0    10037 2024-04-11 19:37:36.000000 cellworld_game-0.0.61/cellworld_game/__pycache__/visibility.cpython-312.pyc
+-rw-rw-rw-   0        0        0     6294 2024-04-26 17:03:41.000000 cellworld_game-0.0.61/cellworld_game/agent.py
+-rw-rw-rw-   0        0        0     3712 2024-04-25 23:24:36.000000 cellworld_game-0.0.61/cellworld_game/cellworld_loader.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:23:50.717209 cellworld_game-0.0.61/cellworld_game/files/
+-rw-rw-rw-   0        0        0     8477 2024-03-30 14:47:10.000000 cellworld_game-0.0.61/cellworld_game/files/agent.png
+-rw-rw-rw-   0        0        0    41740 2024-04-02 20:09:30.000000 cellworld_game-0.0.61/cellworld_game/files/predator.png
+-rw-rw-rw-   0        0        0    47356 2024-04-02 20:07:49.000000 cellworld_game-0.0.61/cellworld_game/files/prey.png
+-rw-rw-rw-   0        0        0      431 2024-04-10 15:24:24.000000 cellworld_game-0.0.61/cellworld_game/geometry.py
+-rw-rw-rw-   0        0        0     1636 2024-04-29 16:23:49.000000 cellworld_game-0.0.61/cellworld_game/license.txt
+-rw-rw-rw-   0        0        0     8159 2024-04-29 16:23:49.000000 cellworld_game-0.0.61/cellworld_game/model.py
+-rw-rw-rw-   0        0        0     1167 2024-04-23 16:26:41.000000 cellworld_game-0.0.61/cellworld_game/mouse.py
+-rw-rw-rw-   0        0        0     1717 2024-04-21 15:19:56.000000 cellworld_game-0.0.61/cellworld_game/navigation.py
+-rw-rw-rw-   0        0        0     4455 2024-04-26 17:03:41.000000 cellworld_game-0.0.61/cellworld_game/navigation_agent.py
+-rw-rw-rw-   0        0        0     4973 2024-04-21 15:20:54.000000 cellworld_game-0.0.61/cellworld_game/ray_tracing.py
+-rw-rw-rw-   0        0        0      220 2024-04-19 14:17:58.000000 cellworld_game-0.0.61/cellworld_game/resources.py
+-rw-rw-rw-   0        0        0     1542 2024-04-26 16:24:32.000000 cellworld_game-0.0.61/cellworld_game/robot.py
+-rw-rw-rw-   0        0        0      183 2024-04-29 16:23:49.000000 cellworld_game-0.0.61/cellworld_game/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-29 16:23:50.721208 cellworld_game-0.0.61/cellworld_game/tasks/
+-rw-rw-rw-   0        0        0       92 2024-04-26 16:46:54.000000 cellworld_game-0.0.61/cellworld_game/tasks/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:23:50.726208 cellworld_game-0.0.61/cellworld_game/tasks/__pycache__/
+-rw-rw-rw-   0        0        0      280 2024-04-26 16:48:27.000000 cellworld_game-0.0.61/cellworld_game/tasks/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     6831 2024-04-26 16:50:52.000000 cellworld_game-0.0.61/cellworld_game/tasks/__pycache__/botevade.cpython-312.pyc
+-rw-rw-rw-   0        0        0     9943 2024-04-26 17:34:24.000000 cellworld_game-0.0.61/cellworld_game/tasks/__pycache__/dualevade.cpython-312.pyc
+-rw-rw-rw-   0        0        0     9261 2024-04-26 16:51:24.000000 cellworld_game-0.0.61/cellworld_game/tasks/__pycache__/oasis.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5436 2024-04-26 17:38:02.000000 cellworld_game-0.0.61/cellworld_game/tasks/botevade.py
+-rw-rw-rw-   0        0        0     8039 2024-04-29 15:41:10.000000 cellworld_game-0.0.61/cellworld_game/tasks/dualevade.py
+-rw-rw-rw-   0        0        0     7476 2024-04-26 16:51:20.000000 cellworld_game-0.0.61/cellworld_game/tasks/oasis.py
+-rw-rw-rw-   0        0        0     7912 2024-04-23 16:14:29.000000 cellworld_game-0.0.61/cellworld_game/util.py
+-rw-rw-rw-   0        0        0     6637 2024-04-26 19:48:33.000000 cellworld_game-0.0.61/cellworld_game/view.py
+-rw-rw-rw-   0        0        0     9497 2024-04-11 19:37:32.000000 cellworld_game-0.0.61/cellworld_game/visibility.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:23:50.728208 cellworld_game-0.0.61/cellworld_game.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-04-29 16:23:50.000000 cellworld_game-0.0.61/cellworld_game.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1902 2024-04-29 16:23:50.000000 cellworld_game-0.0.61/cellworld_game.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 16:23:50.000000 cellworld_game-0.0.61/cellworld_game.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-29 16:23:50.000000 cellworld_game-0.0.61/cellworld_game.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2024-04-29 16:23:50.000000 cellworld_game-0.0.61/cellworld_game.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-29 16:23:50.000000 cellworld_game-0.0.61/cellworld_game.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 16:23:50.730209 cellworld_game-0.0.61/setup.cfg
+-rw-rw-rw-   0        0        0      667 2024-04-29 16:23:49.000000 cellworld_game-0.0.61/setup.py
```

### Comparing `cellworld_game-0.0.60/cellworld_game/__pycache__/__init__.cpython-312.pyc` & `cellworld_game-0.0.61/cellworld_game/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/__pycache__/agent.cpython-312.pyc` & `cellworld_game-0.0.61/cellworld_game/__pycache__/agent.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/__pycache__/cellworld_loader.cpython-312.pyc` & `cellworld_game-0.0.61/cellworld_game/__pycache__/cellworld_loader.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/__pycache__/geometry.cpython-312.pyc` & `cellworld_game-0.0.61/cellworld_game/__pycache__/geometry.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/__pycache__/model.cpython-312.pyc` & `cellworld_game-0.0.61/cellworld_game/__pycache__/model.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/__pycache__/mouse.cpython-312.pyc` & `cellworld_game-0.0.61/cellworld_game/__pycache__/mouse.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/__pycache__/navigation.cpython-312.pyc` & `cellworld_game-0.0.61/cellworld_game/__pycache__/navigation.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/__pycache__/navigation_agent.cpython-312.pyc` & `cellworld_game-0.0.61/cellworld_game/__pycache__/navigation_agent.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/__pycache__/ray_tracing.cpython-312.pyc` & `cellworld_game-0.0.61/cellworld_game/__pycache__/ray_tracing.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/__pycache__/resources.cpython-312.pyc` & `cellworld_game-0.0.61/cellworld_game/__pycache__/resources.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/__pycache__/robot.cpython-312.pyc` & `cellworld_game-0.0.61/cellworld_game/__pycache__/robot.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/__pycache__/util.cpython-312.pyc` & `cellworld_game-0.0.61/cellworld_game/__pycache__/util.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/__pycache__/view.cpython-312.pyc` & `cellworld_game-0.0.61/cellworld_game/__pycache__/view.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/__pycache__/visibility.cpython-312.pyc` & `cellworld_game-0.0.61/cellworld_game/__pycache__/visibility.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/agent.py` & `cellworld_game-0.0.61/cellworld_game/agent.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/cellworld_loader.py` & `cellworld_game-0.0.61/cellworld_game/cellworld_loader.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/files/agent.png` & `cellworld_game-0.0.61/cellworld_game/files/agent.png`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/files/predator.png` & `cellworld_game-0.0.61/cellworld_game/files/predator.png`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/files/prey.png` & `cellworld_game-0.0.61/cellworld_game/files/prey.png`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/license.txt` & `cellworld_game-0.0.61/cellworld_game/license.txt`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/model.py` & `cellworld_game-0.0.61/cellworld_game/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,20 @@
         self.time_step = time_step
         self.agents: typing.Dict[str, Agent] = {}
         self.visibility = Visibility(arena=self.arena, occlusions=self.occlusions)
         self.last_step = None
         self.time = 0
         self.running = False
         self.step_count = 0
+        self.before_step = None
+        self.after_step = None
+        self.before_reset = None
+        self.after_reset = None
+        self.before_close = None
+        self.after_close = None
 
     def set_agents_state(self, agents_state: typing.Dict[str, AgentState],
                          delta_t: float = 0):
         for agent_name, agent_state in agents_state.items():
             if agent_name in self.agents:
                 self.agents[agent_name].set_state(agent_state)
         self.__update_state__(delta_t)
@@ -38,22 +44,26 @@
 
     def add_agent(self, name: str, agent: Agent):
         self.agents[name] = agent
         agent.name = name
         agent.model = self
 
     def reset(self):
+        if self.before_reset is not None:
+            self.before_reset.reset()
         self.running = True
         for name, agent in self.agents.items():
             agent.reset()
         observations = self.get_observations()
         for name, agent in self.agents.items():
             agent.start()
         self.last_step = time.time()
         self.step_count = 0
+        if self.after_reset is not None:
+            self.after_reset()
 
     def is_valid_state(self, agent_polygon: sp.Polygon, collisions: bool) -> bool:
         if not self.arena.contains(agent_polygon):
             return False
         if collisions:
             for occlusion in self.occlusions:
                 if agent_polygon.intersects(occlusion):
@@ -122,14 +132,17 @@
             if is_visible:
                 observation["agent_states"][dst_name] = self.agents[dst_name].state.location, self.agents[dst_name].state.direction
             else:
                 observation["agent_states"][dst_name] = None
         return observation
 
     def step(self) -> float:
+        if self.before_step is not None:
+            self.before_step()
+
         if self.real_time:
             while self.last_step + self.time_step > time.time():
                 pass
 
         self.last_step = time.time()
         for name, agent in self.agents.items():
             dynamics = agent.dynamics
@@ -154,8 +167,16 @@
                     if self.is_valid_state(agent_polygon=agent_polygon,
                                            collisions=agent.collision):
                         agent.set_state(state=new_state)
         for name, agent in self.agents.items():
             agent.step(delta_t=self.time_step)
         self.time += self.time_step
         self.step_count += 1
+        if self.after_step is not None:
+            self.after_step()
         return self.time_step
+
+    def close(self):
+        if self.before_close:
+            self.before_close()
+        if self.after_close:
+            self.after_close()
```

### Comparing `cellworld_game-0.0.60/cellworld_game/mouse.py` & `cellworld_game-0.0.61/cellworld_game/mouse.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/navigation.py` & `cellworld_game-0.0.61/cellworld_game/navigation.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/navigation_agent.py` & `cellworld_game-0.0.61/cellworld_game/navigation_agent.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/ray_tracing.py` & `cellworld_game-0.0.61/cellworld_game/ray_tracing.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/robot.py` & `cellworld_game-0.0.61/cellworld_game/robot.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/tasks/__pycache__/botevade.cpython-312.pyc` & `cellworld_game-0.0.61/cellworld_game/tasks/__pycache__/botevade.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/tasks/__pycache__/dualevade.cpython-312.pyc` & `cellworld_game-0.0.61/cellworld_game/tasks/__pycache__/dualevade.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/tasks/__pycache__/oasis.cpython-312.pyc` & `cellworld_game-0.0.61/cellworld_game/tasks/__pycache__/oasis.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/tasks/botevade.py` & `cellworld_game-0.0.61/cellworld_game/tasks/botevade.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/tasks/dualevade.py` & `cellworld_game-0.0.61/cellworld_game/tasks/dualevade.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         self.puffed = False
         self.goal_achieved = False
         self.predator_visible = False
         self.predator_prey_distance = 1
         self.prey_goal_distance = 0
         self.puff_count = 0
 
+
 class DualEvade(Model):
     def __init__(self,
                  world_name: str = "21_05",
                  use_predator: bool = True,
                  puff_cool_down_time: float = .5,
                  puff_threshold: float = .1,
                  goal_location=(1.0, 0.5),
```

### Comparing `cellworld_game-0.0.60/cellworld_game/tasks/oasis.py` & `cellworld_game-0.0.61/cellworld_game/tasks/oasis.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/util.py` & `cellworld_game-0.0.61/cellworld_game/util.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/view.py` & `cellworld_game-0.0.61/cellworld_game/view.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game/visibility.py` & `cellworld_game-0.0.61/cellworld_game/visibility.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/cellworld_game.egg-info/SOURCES.txt` & `cellworld_game-0.0.61/cellworld_game.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.60/setup.py` & `cellworld_game-0.0.61/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,9 +7,9 @@
       author_email='germanespinosa@gmail.com',
       long_description=open('./cellworld_game/README.md').read() + '\n---\n<small>Package created with Easy-pack</small>\n',
       long_description_content_type='text/markdown',
       packages=['cellworld_game'],
       install_requires=['cellworld', 'pygame', 'shapely'],
       license='MIT',
       include_package_data=True,
-      version='0.0.60',
+      version='0.0.61',
       zip_safe=False)
```

