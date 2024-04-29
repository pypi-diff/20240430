# Comparing `tmp/pyppbox-3.6b2.tar.gz` & `tmp/pyppbox-3.6b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyppbox-3.6b2.tar", last modified: Sat Apr 13 13:49:14 2024, max compression
+gzip compressed data, was "pyppbox-3.6b3.tar", last modified: Mon Apr 29 23:25:47 2024, max compression
```

## Comparing `pyppbox-3.6b2.tar` & `pyppbox-3.6b3.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.237316 pyppbox-3.6b2/
--rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-04-13 13:49:08.000000 pyppbox-3.6b2/GETSTARTED.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-13 13:49:08.000000 pyppbox-3.6b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-13 13:49:08.000000 pyppbox-3.6b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-13 13:49:14.233316 pyppbox-3.6b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-13 13:49:08.000000 pyppbox-3.6b2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    14373 2024-04-13 13:49:08.000000 pyppbox-3.6b2/RELEASENOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.213316 pyppbox-3.6b2/pyppbox/
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.217316 pyppbox-3.6b2/pyppbox/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.217316 pyppbox-3.6b2/pyppbox/config/cfg/
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/config/cfg/cfg.zip
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/config/cfg/detectors.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/config/cfg/main.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/config/cfg/reiders.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/config/cfg/trackers.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13021 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/config/configtools.py
--rw-r--r--   0 runner    (1001) docker     (127)    65155 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/config/myconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.217316 pyppbox-3.6b2/pyppbox/config/strings/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/config/strings/strings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/config/strings/strings.zip
--rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/config/unifiedstrings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.209315 pyppbox-3.6b2/pyppbox/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.217316 pyppbox-3.6b2/pyppbox/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/data/datasets/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.221315 pyppbox-3.6b2/pyppbox/data/logs/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/data/logs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.221315 pyppbox-3.6b2/pyppbox/data/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/data/modules/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.221315 pyppbox-3.6b2/pyppbox/data/res/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/data/res/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/data/res/idmap.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.221315 pyppbox-3.6b2/pyppbox/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.225316 pyppbox-3.6b2/pyppbox/gui/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   833181 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/assets/TReID.png
--rw-r--r--   0 runner    (1001) docker     (127)    12690 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/assets/icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    33692 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/assets/settings.ico
--rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/guidemo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/guihub.py
--rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/guitools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.225316 pyppbox-3.6b2/pyppbox/gui/tmp/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/tmp/input.tmp
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/tmp/ui.tmp
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/ui_centroid.py
--rw-r--r--   0 runner    (1001) docker     (127)     8716 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/ui_deepsort.py
--rw-r--r--   0 runner    (1001) docker     (127)    15884 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/ui_facenet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/ui_gt.py
--rw-r--r--   0 runner    (1001) docker     (127)    23388 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/ui_launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/ui_sort.py
--rw-r--r--   0 runner    (1001) docker     (127)    13079 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/ui_torchreid.py
--rw-r--r--   0 runner    (1001) docker     (127)    13276 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/ui_yolocls.py
--rw-r--r--   0 runner    (1001) docker     (127)    13885 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/ui_yoloult.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.225316 pyppbox-3.6b2/pyppbox/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.225316 pyppbox-3.6b2/pyppbox/modules/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.225316 pyppbox-3.6b2/pyppbox/modules/detectors/yolocls/
--rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/detectors/yolocls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.225316 pyppbox-3.6b2/pyppbox/modules/detectors/yoloult/
--rw-r--r--   0 runner    (1001) docker     (127)    13251 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/detectors/yoloult/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.225316 pyppbox-3.6b2/pyppbox/modules/reiders/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/reiders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.225316 pyppbox-3.6b2/pyppbox/modules/reiders/facenet/
--rw-r--r--   0 runner    (1001) docker     (127)    12514 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/reiders/facenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.225316 pyppbox-3.6b2/pyppbox/modules/reiders/facenet/origin/
--rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    31858 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/reiders/facenet/origin/detect_face.py
--rw-r--r--   0 runner    (1001) docker     (127)    23601 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/reiders/facenet/origin/facenet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.229316 pyppbox-3.6b2/pyppbox/modules/reiders/torchreid/
--rw-r--r--   0 runner    (1001) docker     (127)     7463 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/reiders/torchreid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/reiders/torchreid/model_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/reiders/torchreid/model_dict.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/reiders/torchreid/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.229316 pyppbox-3.6b2/pyppbox/modules/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.229316 pyppbox-3.6b2/pyppbox/modules/trackers/centroid/
--rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/centroid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.229316 pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/
--rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.229316 pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/generate_detections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/iou_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/nn_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/track.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/voc_classes.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.229316 pyppbox-3.6b2/pyppbox/modules/trackers/sort/
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/sort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.233316 pyppbox-3.6b2/pyppbox/modules/trackers/sort/origin/
--rw-r--r--   0 runner    (1001) docker     (127)    13893 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/sort/origin/sort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.233316 pyppbox-3.6b2/pyppbox/ppb/
--rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/ppb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52182 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/ppb/mt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.233316 pyppbox-3.6b2/pyppbox/standalone/
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/standalone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.233316 pyppbox-3.6b2/pyppbox/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/utils/commontools.py
--rw-r--r--   0 runner    (1001) docker     (127)    25985 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/utils/evatools.py
--rw-r--r--   0 runner    (1001) docker     (127)    13446 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/utils/gttools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/utils/logtools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/utils/mot2pyppbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/utils/persontools.py
--rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/utils/restools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9611 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/utils/visualizetools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.233316 pyppbox-3.6b2/pyppbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-13 13:49:14.000000 pyppbox-3.6b2/pyppbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-13 13:49:14.000000 pyppbox-3.6b2/pyppbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:49:14.000000 pyppbox-3.6b2/pyppbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-13 13:49:14.000000 pyppbox-3.6b2/pyppbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-13 13:49:14.000000 pyppbox-3.6b2/pyppbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.233316 pyppbox-3.6b2/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-13 13:49:08.000000 pyppbox-3.6b2/requirements/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-13 13:49:08.000000 pyppbox-3.6b2/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-13 13:49:08.000000 pyppbox-3.6b2/requirements/test_gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 13:49:14.237316 pyppbox-3.6b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-13 13:49:08.000000 pyppbox-3.6b2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-13 13:49:08.000000 pyppbox-3.6b2/setup_extra.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.759677 pyppbox-3.6b3/
+-rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-04-29 23:25:42.000000 pyppbox-3.6b3/GETSTARTED.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-29 23:25:42.000000 pyppbox-3.6b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-29 23:25:42.000000 pyppbox-3.6b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-29 23:25:47.759677 pyppbox-3.6b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-29 23:25:42.000000 pyppbox-3.6b3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    14547 2024-04-29 23:25:42.000000 pyppbox-3.6b3/RELEASENOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.743677 pyppbox-3.6b3/pyppbox/
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.743677 pyppbox-3.6b3/pyppbox/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.743677 pyppbox-3.6b3/pyppbox/config/cfg/
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/config/cfg/cfg.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/config/cfg/detectors.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/config/cfg/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/config/cfg/reiders.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/config/cfg/trackers.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13021 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/config/configtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65155 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/config/myconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.743677 pyppbox-3.6b3/pyppbox/config/strings/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/config/strings/strings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/config/strings/strings.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/config/unifiedstrings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.739677 pyppbox-3.6b3/pyppbox/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.743677 pyppbox-3.6b3/pyppbox/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/data/datasets/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.743677 pyppbox-3.6b3/pyppbox/data/logs/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/data/logs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.747677 pyppbox-3.6b3/pyppbox/data/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/data/modules/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.747677 pyppbox-3.6b3/pyppbox/data/res/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/data/res/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/data/res/idmap.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.747677 pyppbox-3.6b3/pyppbox/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.751677 pyppbox-3.6b3/pyppbox/gui/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   833181 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/gui/assets/TReID.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12690 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/gui/assets/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    33692 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/gui/assets/settings.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/gui/guidemo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/gui/guihub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/gui/guitools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.751677 pyppbox-3.6b3/pyppbox/gui/tmp/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/gui/tmp/input.tmp
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/gui/tmp/ui.tmp
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/gui/ui_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8716 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/gui/ui_deepsort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15884 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/gui/ui_facenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/gui/ui_gt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23388 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/gui/ui_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/gui/ui_sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13079 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/gui/ui_torchreid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13276 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/gui/ui_yolocls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13885 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/gui/ui_yoloult.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.751677 pyppbox-3.6b3/pyppbox/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.751677 pyppbox-3.6b3/pyppbox/modules/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/modules/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.751677 pyppbox-3.6b3/pyppbox/modules/detectors/yolocls/
+-rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/modules/detectors/yolocls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.751677 pyppbox-3.6b3/pyppbox/modules/detectors/yoloult/
+-rw-r--r--   0 runner    (1001) docker     (127)    13251 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/modules/detectors/yoloult/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.751677 pyppbox-3.6b3/pyppbox/modules/reiders/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/modules/reiders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.751677 pyppbox-3.6b3/pyppbox/modules/reiders/facenet/
+-rw-r--r--   0 runner    (1001) docker     (127)    12514 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/modules/reiders/facenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.751677 pyppbox-3.6b3/pyppbox/modules/reiders/facenet/origin/
+-rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31858 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/modules/reiders/facenet/origin/detect_face.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23601 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/modules/reiders/facenet/origin/facenet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.751677 pyppbox-3.6b3/pyppbox/modules/reiders/torchreid/
+-rw-r--r--   0 runner    (1001) docker     (127)     7463 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/modules/reiders/torchreid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/modules/reiders/torchreid/model_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/modules/reiders/torchreid/model_dict.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/modules/reiders/torchreid/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.751677 pyppbox-3.6b3/pyppbox/modules/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/modules/trackers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.751677 pyppbox-3.6b3/pyppbox/modules/trackers/centroid/
+-rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/modules/trackers/centroid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.751677 pyppbox-3.6b3/pyppbox/modules/trackers/deepsort/
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/modules/trackers/deepsort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.755677 pyppbox-3.6b3/pyppbox/modules/trackers/deepsort/origin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/modules/trackers/deepsort/origin/detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/modules/trackers/deepsort/origin/generate_detections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/modules/trackers/deepsort/origin/iou_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/modules/trackers/deepsort/origin/nn_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/modules/trackers/deepsort/origin/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/modules/trackers/deepsort/origin/track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/modules/trackers/deepsort/origin/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/modules/trackers/deepsort/origin/voc_classes.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.755677 pyppbox-3.6b3/pyppbox/modules/trackers/sort/
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/modules/trackers/sort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.755677 pyppbox-3.6b3/pyppbox/modules/trackers/sort/origin/
+-rw-r--r--   0 runner    (1001) docker     (127)    13893 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/modules/trackers/sort/origin/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.755677 pyppbox-3.6b3/pyppbox/ppb/
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/ppb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52182 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/ppb/mt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.755677 pyppbox-3.6b3/pyppbox/standalone/
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/standalone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.759677 pyppbox-3.6b3/pyppbox/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/utils/commontools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25985 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/utils/evatools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13446 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/utils/gttools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/utils/logtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/utils/mot2pyppbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/utils/persontools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/utils/restools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9611 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyppbox/utils/visualizetools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.759677 pyppbox-3.6b3/pyppbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-29 23:25:47.000000 pyppbox-3.6b3/pyppbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-29 23:25:47.000000 pyppbox-3.6b3/pyppbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 23:25:47.000000 pyppbox-3.6b3/pyppbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-29 23:25:47.000000 pyppbox-3.6b3/pyppbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 23:25:47.000000 pyppbox-3.6b3/pyppbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-29 23:25:42.000000 pyppbox-3.6b3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:25:47.759677 pyppbox-3.6b3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-29 23:25:42.000000 pyppbox-3.6b3/requirements/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-29 23:25:42.000000 pyppbox-3.6b3/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-29 23:25:42.000000 pyppbox-3.6b3/requirements/test_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 23:25:47.759677 pyppbox-3.6b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-29 23:25:42.000000 pyppbox-3.6b3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-29 23:25:42.000000 pyppbox-3.6b3/setup_extra.yaml
```

### Comparing `pyppbox-3.6b2/GETSTARTED.md` & `pyppbox-3.6b3/GETSTARTED.md`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/LICENSE` & `pyppbox-3.6b3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/PKG-INFO` & `pyppbox-3.6b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyppbox
-Version: 3.6b2
+Version: 3.6b3
 Summary: Toolbox for people detecting, tracking, and re-identifying.
 Home-page: https://github.com/rathaumons/pyppbox
 Author: Ratha SIV
 Maintainer: rathaROG
 License: GPL-3.0-or-later
 Keywords: Toolbox,People Detecting,People Tracking,People Re-Identification
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyppbox-3.6b2/README.md` & `pyppbox-3.6b3/README.md`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/RELEASENOTES.md` & `pyppbox-3.6b3/RELEASENOTES.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,20 @@
   - `pyppbox.utils.persontools` will change to adapt [`vsensebox`](https://github.com/rathaumons/vsensebox)
   - `pyppbox.ppb` will replace `pyppbox.standalone`
   - All configuration files will also change
   - More changes will be added here! Stay tuned!
 
 ## **pyppbox V3 - Make Simpler and Faster**
 
+* `pyppbox` [v3.6b3](https://github.com/rathaumons/pyppbox/tree/v3.6b3) - The Last V3
+
+  - Fix typo and update workflow
+  - **Known issue/limitation**:
+    - You tell me :)
+
 * `pyppbox` [v3.6b2](https://github.com/rathaumons/pyppbox/tree/v3.6b2)
 
   - Add a warning for the changes in the coming major version 4
   - Update documentations
   - **Known issue/limitation**:
     - You tell me :)
```

### Comparing `pyppbox-3.6b2/pyppbox/__init__.py` & `pyppbox-3.6b3/pyppbox/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,13 +43,13 @@
     useInternalConfigDir, 
     useThisConfigDir,
     resetInternalConfig,
     generateConfig
 )
 
 
-__version__ = '3.6b2'
+__version__ = '3.6b3'
 __author__ = 'Ratha SIV'
 __description__ = 'Toolbox for people detecting, tracking, and re-identifying.'
 __homepage__ = 'https://rathaumons.github.io/pyppbox'
 __url__ = 'https://github.com/rathaumons/pyppbox.git'
```

### Comparing `pyppbox-3.6b2/pyppbox/config/__init__.py` & `pyppbox-3.6b3/pyppbox/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/config/cfg/cfg.zip` & `pyppbox-3.6b3/pyppbox/config/cfg/cfg.zip`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/config/cfg/detectors.yaml` & `pyppbox-3.6b3/pyppbox/config/cfg/detectors.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/config/cfg/reiders.yaml` & `pyppbox-3.6b3/pyppbox/config/cfg/reiders.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/config/cfg/trackers.yaml` & `pyppbox-3.6b3/pyppbox/config/cfg/trackers.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/config/configtools.py` & `pyppbox-3.6b3/pyppbox/config/configtools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/config/myconfig.py` & `pyppbox-3.6b3/pyppbox/config/myconfig.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/config/unifiedstrings.py` & `pyppbox-3.6b3/pyppbox/config/unifiedstrings.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/gui/__init__.py` & `pyppbox-3.6b3/pyppbox/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/gui/assets/TReID.png` & `pyppbox-3.6b3/pyppbox/gui/assets/TReID.png`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/gui/assets/icon.ico` & `pyppbox-3.6b3/pyppbox/gui/assets/icon.ico`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/gui/assets/settings.ico` & `pyppbox-3.6b3/pyppbox/gui/assets/settings.ico`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/gui/guidemo.py` & `pyppbox-3.6b3/pyppbox/gui/guidemo.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/gui/guihub.py` & `pyppbox-3.6b3/pyppbox/gui/guihub.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/gui/guitools.py` & `pyppbox-3.6b3/pyppbox/gui/guitools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/gui/ui_centroid.py` & `pyppbox-3.6b3/pyppbox/gui/ui_centroid.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/gui/ui_deepsort.py` & `pyppbox-3.6b3/pyppbox/gui/ui_deepsort.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/gui/ui_facenet.py` & `pyppbox-3.6b3/pyppbox/gui/ui_facenet.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/gui/ui_gt.py` & `pyppbox-3.6b3/pyppbox/gui/ui_gt.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/gui/ui_launcher.py` & `pyppbox-3.6b3/pyppbox/gui/ui_launcher.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/gui/ui_sort.py` & `pyppbox-3.6b3/pyppbox/gui/ui_sort.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/gui/ui_torchreid.py` & `pyppbox-3.6b3/pyppbox/gui/ui_torchreid.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/gui/ui_yolocls.py` & `pyppbox-3.6b3/pyppbox/gui/ui_yolocls.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/gui/ui_yoloult.py` & `pyppbox-3.6b3/pyppbox/gui/ui_yoloult.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/modules/__init__.py` & `pyppbox-3.6b3/pyppbox/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/modules/detectors/__init__.py` & `pyppbox-3.6b3/pyppbox/modules/detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/modules/detectors/yolocls/__init__.py` & `pyppbox-3.6b3/pyppbox/modules/detectors/yolocls/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/modules/detectors/yoloult/__init__.py` & `pyppbox-3.6b3/pyppbox/modules/detectors/yoloult/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/modules/reiders/__init__.py` & `pyppbox-3.6b3/pyppbox/modules/reiders/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/modules/reiders/facenet/__init__.py` & `pyppbox-3.6b3/pyppbox/modules/reiders/facenet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py` & `pyppbox-3.6b3/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/modules/reiders/facenet/origin/detect_face.py` & `pyppbox-3.6b3/pyppbox/modules/reiders/facenet/origin/detect_face.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/modules/reiders/facenet/origin/facenet.py` & `pyppbox-3.6b3/pyppbox/modules/reiders/facenet/origin/facenet.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/modules/reiders/torchreid/__init__.py` & `pyppbox-3.6b3/pyppbox/modules/reiders/torchreid/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/modules/reiders/torchreid/model_dict.py` & `pyppbox-3.6b3/pyppbox/modules/reiders/torchreid/model_dict.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/modules/reiders/torchreid/model_dict.yaml` & `pyppbox-3.6b3/pyppbox/modules/reiders/torchreid/model_dict.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/modules/reiders/torchreid/utils.py` & `pyppbox-3.6b3/pyppbox/modules/reiders/torchreid/utils.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/modules/trackers/__init__.py` & `pyppbox-3.6b3/pyppbox/modules/trackers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/modules/trackers/centroid/__init__.py` & `pyppbox-3.6b3/pyppbox/modules/trackers/centroid/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/__init__.py` & `pyppbox-3.6b3/pyppbox/modules/trackers/deepsort/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/detection.py` & `pyppbox-3.6b3/pyppbox/modules/trackers/deepsort/origin/detection.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py` & `pyppbox-3.6b3/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/generate_detections.py` & `pyppbox-3.6b3/pyppbox/modules/trackers/deepsort/origin/generate_detections.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/iou_matching.py` & `pyppbox-3.6b3/pyppbox/modules/trackers/deepsort/origin/iou_matching.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py` & `pyppbox-3.6b3/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py` & `pyppbox-3.6b3/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/nn_matching.py` & `pyppbox-3.6b3/pyppbox/modules/trackers/deepsort/origin/nn_matching.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/preprocessing.py` & `pyppbox-3.6b3/pyppbox/modules/trackers/deepsort/origin/preprocessing.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/track.py` & `pyppbox-3.6b3/pyppbox/modules/trackers/deepsort/origin/track.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/tracker.py` & `pyppbox-3.6b3/pyppbox/modules/trackers/deepsort/origin/tracker.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/modules/trackers/sort/__init__.py` & `pyppbox-3.6b3/pyppbox/modules/trackers/sort/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/modules/trackers/sort/origin/sort.py` & `pyppbox-3.6b3/pyppbox/modules/trackers/sort/origin/sort.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/ppb/__init__.py` & `pyppbox-3.6b3/pyppbox/ppb/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/ppb/mt.py` & `pyppbox-3.6b3/pyppbox/ppb/mt.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/standalone/__init__.py` & `pyppbox-3.6b3/pyppbox/standalone/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from pyppbox.ppb import *
 from pyppbox.utils.logtools import add_warning_log
 
 msg = ("\n! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! !\n"
        "!                                                                       !\n"
        "!  For the coming major version 4:                                      !\n"
        "!   * 'pyppbox' will leverage 'vsensebox' for detection and tracking    !\n"
-       "!   * 'pyppbox.utils.persontools' will change to adapt 'vesensebox'     !\n"
+       "!   * 'pyppbox.utils.persontools' will change to adapt 'vsensebox'      !\n"
        "!   * 'pyppbox.ppb' will replace 'pyppbox.standalone'                   !\n"
        "!   * All configuration files will also change                          !\n"
        "!   * More changes will be added to release notes                       !\n"
        "!                                                                       !\n"
        "! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! ! !\n")
 
 add_warning_log(msg)
```

### Comparing `pyppbox-3.6b2/pyppbox/utils/__init__.py` & `pyppbox-3.6b3/pyppbox/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/utils/commontools.py` & `pyppbox-3.6b3/pyppbox/utils/commontools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/utils/evatools.py` & `pyppbox-3.6b3/pyppbox/utils/evatools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/utils/gttools.py` & `pyppbox-3.6b3/pyppbox/utils/gttools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/utils/logtools.py` & `pyppbox-3.6b3/pyppbox/utils/logtools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/utils/mot2pyppbox.py` & `pyppbox-3.6b3/pyppbox/utils/mot2pyppbox.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/utils/persontools.py` & `pyppbox-3.6b3/pyppbox/utils/persontools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/utils/restools.py` & `pyppbox-3.6b3/pyppbox/utils/restools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox/utils/visualizetools.py` & `pyppbox-3.6b3/pyppbox/utils/visualizetools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/pyppbox.egg-info/PKG-INFO` & `pyppbox-3.6b3/pyppbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyppbox
-Version: 3.6b2
+Version: 3.6b3
 Summary: Toolbox for people detecting, tracking, and re-identifying.
 Home-page: https://github.com/rathaumons/pyppbox
 Author: Ratha SIV
 Maintainer: rathaROG
 License: GPL-3.0-or-later
 Keywords: Toolbox,People Detecting,People Tracking,People Re-Identification
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyppbox-3.6b2/pyppbox.egg-info/SOURCES.txt` & `pyppbox-3.6b3/pyppbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/requirements/requirements.txt` & `pyppbox-3.6b3/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/requirements/test_gpu.py` & `pyppbox-3.6b3/requirements/test_gpu.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/setup.py` & `pyppbox-3.6b3/setup.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b2/setup_extra.yaml` & `pyppbox-3.6b3/setup_extra.yaml`

 * *Files identical despite different names*

