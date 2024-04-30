# Comparing `tmp/pypanasonic-0.0.1.tar.gz` & `tmp/pypanasonic-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypanasonic-0.0.1.tar", last modified: Sat Mar  2 04:15:20 2024, max compression
+gzip compressed data, was "pypanasonic-0.0.2.tar", last modified: Tue Apr 30 14:19:16 2024, max compression
```

## Comparing `pypanasonic-0.0.1.tar` & `pypanasonic-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-02 04:15:20.541875 pypanasonic-0.0.1/
--rw-rw-rw-   0        0        0      184 2024-03-02 04:15:20.540898 pypanasonic-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-02 04:15:20.538947 pypanasonic-0.0.1/pypanasonic.egg-info/
--rw-rw-rw-   0        0        0      184 2024-03-02 04:15:20.000000 pypanasonic-0.0.1/pypanasonic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      148 2024-03-02 04:15:20.000000 pypanasonic-0.0.1/pypanasonic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-02 04:15:20.000000 pypanasonic-0.0.1/pypanasonic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-03-02 04:15:20.000000 pypanasonic-0.0.1/pypanasonic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-02 04:15:20.541875 pypanasonic-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      312 2024-03-02 04:15:14.000000 pypanasonic-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:19:16.880830 pypanasonic-0.0.2/
+-rw-rw-rw-   0        0        0     1083 2024-04-30 13:58:47.000000 pypanasonic-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      206 2024-04-30 14:05:37.000000 pypanasonic-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1749 2024-04-30 14:19:16.879830 pypanasonic-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      936 2024-04-30 13:56:36.000000 pypanasonic-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 14:19:16.879830 pypanasonic-0.0.2/pypanasonic.egg-info/
+-rw-rw-rw-   0        0        0     1749 2024-04-30 14:19:16.000000 pypanasonic-0.0.2/pypanasonic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2024-04-30 14:19:16.000000 pypanasonic-0.0.2/pypanasonic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 14:19:16.000000 pypanasonic-0.0.2/pypanasonic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      129 2024-04-30 14:19:16.000000 pypanasonic-0.0.2/pypanasonic.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2024-04-30 14:19:16.000000 pypanasonic-0.0.2/pypanasonic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 14:19:16.000000 pypanasonic-0.0.2/pypanasonic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1157 2024-04-30 14:18:00.000000 pypanasonic-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       81 2024-04-30 14:19:16.882831 pypanasonic-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      324 2024-04-30 14:04:03.000000 pypanasonic-0.0.2/setup.py
```

