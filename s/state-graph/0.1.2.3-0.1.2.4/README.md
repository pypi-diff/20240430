# Comparing `tmp/state_graph-0.1.2.3.tar.gz` & `tmp/state_graph-0.1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "state_graph-0.1.2.3.tar", last modified: Sat Apr 27 13:08:39 2024, max compression
+gzip compressed data, was "state_graph-0.1.2.4.tar", last modified: Tue Apr 30 05:50:25 2024, max compression
```

## Comparing `state_graph-0.1.2.3.tar` & `state_graph-0.1.2.4.tar`

### file list

```diff
@@ -1,12 +1,17 @@
-drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-04-27 13:08:39.571547 state_graph-0.1.2.3/
--rw-r--r--   0 salamanderxing   (501) staff       (20)      198 2024-04-27 13:08:39.571324 state_graph-0.1.2.3/PKG-INFO
--rw-r--r--   0 salamanderxing   (501) staff       (20)       38 2024-04-27 13:08:39.571588 state_graph-0.1.2.3/setup.cfg
--rw-r--r--   0 salamanderxing   (501) staff       (20)      321 2024-04-27 13:08:35.000000 state_graph-0.1.2.3/setup.py
-drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-04-27 13:08:39.570199 state_graph-0.1.2.3/state_graph/
--rw-r--r--   0 salamanderxing   (501) staff       (20)    19350 2024-04-27 13:08:17.000000 state_graph-0.1.2.3/state_graph/__init__.py
-drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-04-27 13:08:39.571116 state_graph-0.1.2.3/state_graph.egg-info/
--rw-r--r--   0 salamanderxing   (501) staff       (20)      198 2024-04-27 13:08:39.000000 state_graph-0.1.2.3/state_graph.egg-info/PKG-INFO
--rw-r--r--   0 salamanderxing   (501) staff       (20)      206 2024-04-27 13:08:39.000000 state_graph-0.1.2.3/state_graph.egg-info/SOURCES.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)        1 2024-04-27 13:08:39.000000 state_graph-0.1.2.3/state_graph.egg-info/dependency_links.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)       51 2024-04-27 13:08:39.000000 state_graph-0.1.2.3/state_graph.egg-info/requires.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)       12 2024-04-27 13:08:39.000000 state_graph-0.1.2.3/state_graph.egg-info/top_level.txt
+drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-04-30 05:50:25.546682 state_graph-0.1.2.4/
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      198 2024-04-30 05:50:25.546480 state_graph-0.1.2.4/PKG-INFO
+-rw-r--r--   0 salamanderxing   (501) staff       (20)       38 2024-04-30 05:50:25.546727 state_graph-0.1.2.4/setup.cfg
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      321 2024-04-30 05:50:20.000000 state_graph-0.1.2.4/setup.py
+drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-04-30 05:50:25.545459 state_graph-0.1.2.4/state_graph/
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      148 2024-04-30 05:32:27.000000 state_graph-0.1.2.4/state_graph/__init__.py
+-rw-r--r--   0 salamanderxing   (501) staff       (20)     2221 2024-04-30 05:31:01.000000 state_graph-0.1.2.4/state_graph/__main__.py
+-rw-r--r--   0 salamanderxing   (501) staff       (20)     2594 2024-04-30 05:36:31.000000 state_graph-0.1.2.4/state_graph/edge.py
+-rw-r--r--   0 salamanderxing   (501) staff       (20)    11426 2024-04-30 05:46:21.000000 state_graph-0.1.2.4/state_graph/graph.py
+-rw-r--r--   0 salamanderxing   (501) staff       (20)     2135 2024-04-30 05:26:30.000000 state_graph-0.1.2.4/state_graph/node.py
+-rw-r--r--   0 salamanderxing   (501) staff       (20)     2841 2024-04-30 05:45:17.000000 state_graph-0.1.2.4/state_graph/utils.py
+drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-04-30 05:50:25.546250 state_graph-0.1.2.4/state_graph.egg-info/
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      198 2024-04-30 05:50:25.000000 state_graph-0.1.2.4/state_graph.egg-info/PKG-INFO
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      312 2024-04-30 05:50:25.000000 state_graph-0.1.2.4/state_graph.egg-info/SOURCES.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)        1 2024-04-30 05:50:25.000000 state_graph-0.1.2.4/state_graph.egg-info/dependency_links.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)       51 2024-04-30 05:50:25.000000 state_graph-0.1.2.4/state_graph.egg-info/requires.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)       12 2024-04-30 05:50:25.000000 state_graph-0.1.2.4/state_graph.egg-info/top_level.txt
```

