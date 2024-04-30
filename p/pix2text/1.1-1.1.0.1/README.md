# Comparing `tmp/pix2text-1.1.tar.gz` & `tmp/pix2text-1.1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pix2text-1.1.tar", last modified: Sun Apr 28 15:17:52 2024, max compression
+gzip compressed data, was "pix2text-1.1.0.1.tar", last modified: Tue Apr 30 03:15:23 2024, max compression
```

## Comparing `pix2text-1.1.tar` & `pix2text-1.1.0.1.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-28 15:17:52.802331 pix2text-1.1/
--rw-r--r--   0 king       (501) staff       (20)     1067 2022-09-07 14:44:50.000000 pix2text-1.1/LICENSE
--rw-r--r--   0 king       (501) staff       (20)    14010 2024-04-28 15:17:52.802182 pix2text-1.1/PKG-INFO
--rw-r--r--   0 king       (501) staff       (20)    12900 2024-04-28 15:01:52.000000 pix2text-1.1/README.md
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-28 15:17:52.790881 pix2text-1.1/pix2text/
--rw-r--r--   0 king       (501) staff       (20)      456 2024-04-02 11:11:40.000000 pix2text-1.1/pix2text/__init__.py
--rw-r--r--   0 king       (501) staff       (20)      199 2024-04-23 07:32:19.000000 pix2text-1.1/pix2text/__version__.py
--rw-r--r--   0 king       (501) staff       (20)     1709 2022-09-10 15:50:05.000000 pix2text-1.1/pix2text/app.py
--rw-r--r--   0 king       (501) staff       (20)     2092 2022-09-08 07:30:17.000000 pix2text-1.1/pix2text/category_mapping.py
--rw-r--r--   0 king       (501) staff       (20)    10451 2024-04-22 00:51:42.000000 pix2text-1.1/pix2text/cli.py
--rw-r--r--   0 king       (501) staff       (20)     3710 2024-04-16 14:50:16.000000 pix2text-1.1/pix2text/consts.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-28 15:17:52.793545 pix2text-1.1/pix2text/doc_xl_layout/
--rw-r--r--   0 king       (501) staff       (20)      192 2024-04-03 01:13:56.000000 pix2text-1.1/pix2text/doc_xl_layout/__init__.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-28 15:17:52.794415 pix2text-1.1/pix2text/doc_xl_layout/detectors/
--rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1/pix2text/doc_xl_layout/detectors/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     8390 2024-04-02 08:34:16.000000 pix2text-1.1/pix2text/doc_xl_layout/detectors/base_detector_subfield.py
--rw-r--r--   0 king       (501) staff       (20)     8722 2024-04-02 07:16:21.000000 pix2text-1.1/pix2text/doc_xl_layout/detectors/ctdet_subfield.py
--rw-r--r--   0 king       (501) staff       (20)      137 2024-04-02 06:45:51.000000 pix2text-1.1/pix2text/doc_xl_layout/detectors/detector_factory.py
--rw-r--r--   0 king       (501) staff       (20)    17874 2024-04-23 15:41:22.000000 pix2text-1.1/pix2text/doc_xl_layout/doc_xl_layout_parser.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-28 15:17:52.794748 pix2text-1.1/pix2text/doc_xl_layout/external/
--rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1/pix2text/doc_xl_layout/external/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     2510 2024-04-01 15:18:57.000000 pix2text-1.1/pix2text/doc_xl_layout/external/shapelyNMS.py
--rw-r--r--   0 king       (501) staff       (20)      365 2024-04-01 15:18:57.000000 pix2text-1.1/pix2text/doc_xl_layout/huntie_subfield.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-28 15:17:52.796266 pix2text-1.1/pix2text/doc_xl_layout/models/
--rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1/pix2text/doc_xl_layout/models/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     5178 2024-04-01 15:18:57.000000 pix2text-1.1/pix2text/doc_xl_layout/models/data_parallel.py
--rw-r--r--   0 king       (501) staff       (20)    23840 2024-04-02 07:32:06.000000 pix2text-1.1/pix2text/doc_xl_layout/models/decode.py
--rw-r--r--   0 king       (501) staff       (20)     3443 2024-04-10 11:32:17.000000 pix2text-1.1/pix2text/doc_xl_layout/models/model.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-28 15:17:52.796593 pix2text-1.1/pix2text/doc_xl_layout/models/networks/
--rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1/pix2text/doc_xl_layout/models/networks/__init__.py
--rw-r--r--   0 king       (501) staff       (20)    24395 2024-04-01 15:18:57.000000 pix2text-1.1/pix2text/doc_xl_layout/models/networks/dlav0_subfield.py
--rw-r--r--   0 king       (501) staff       (20)     1528 2024-04-01 15:18:57.000000 pix2text-1.1/pix2text/doc_xl_layout/models/scatter_gather.py
--rw-r--r--   0 king       (501) staff       (20)     1800 2024-04-02 07:31:48.000000 pix2text-1.1/pix2text/doc_xl_layout/models/utils.py
--rw-r--r--   0 king       (501) staff       (20)    23801 2024-04-02 00:43:23.000000 pix2text-1.1/pix2text/doc_xl_layout/opts.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-28 15:17:52.798435 pix2text-1.1/pix2text/doc_xl_layout/utils/
--rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1/pix2text/doc_xl_layout/utils/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     4818 2024-04-01 15:18:57.000000 pix2text-1.1/pix2text/doc_xl_layout/utils/ddd_utils.py
--rw-r--r--   0 king       (501) staff       (20)    26623 2024-04-02 06:59:29.000000 pix2text-1.1/pix2text/doc_xl_layout/utils/debugger.py
--rw-r--r--   0 king       (501) staff       (20)    18383 2024-04-02 06:47:12.000000 pix2text-1.1/pix2text/doc_xl_layout/utils/evaluation_bk.py
--rw-r--r--   0 king       (501) staff       (20)     7851 2024-04-01 15:18:57.000000 pix2text-1.1/pix2text/doc_xl_layout/utils/image.py
--rw-r--r--   0 king       (501) staff       (20)     5368 2024-04-02 06:47:54.000000 pix2text-1.1/pix2text/doc_xl_layout/utils/post_process.py
--rw-r--r--   0 king       (501) staff       (20)      533 2024-04-01 15:18:57.000000 pix2text-1.1/pix2text/doc_xl_layout/utils/utils.py
--rw-r--r--   0 king       (501) staff       (20)     8844 2024-04-02 06:20:49.000000 pix2text-1.1/pix2text/doc_xl_layout/wrapper.py
--rw-r--r--   0 king       (501) staff       (20)    12517 2024-03-27 09:59:17.000000 pix2text-1.1/pix2text/element.py
--rw-r--r--   0 king       (501) staff       (20)    17431 2024-04-22 02:21:39.000000 pix2text-1.1/pix2text/latex_ocr.py
--rw-r--r--   0 king       (501) staff       (20)    13244 2024-01-11 04:27:38.000000 pix2text-1.1/pix2text/latex_ocr0.py
--rw-r--r--   0 king       (501) staff       (20)    22526 2024-01-10 13:35:10.000000 pix2text-1.1/pix2text/latex_recog.py
--rw-r--r--   0 king       (501) staff       (20)     4016 2024-04-06 13:32:28.000000 pix2text-1.1/pix2text/layout_parser.py
--rw-r--r--   0 king       (501) staff       (20)     3567 2022-09-13 02:10:01.000000 pix2text-1.1/pix2text/object_detector.py
--rw-r--r--   0 king       (501) staff       (20)     7285 2024-04-27 13:58:01.000000 pix2text-1.1/pix2text/ocr_engine.py
--rw-r--r--   0 king       (501) staff       (20)    10461 2024-04-26 06:27:40.000000 pix2text-1.1/pix2text/page_elements.py
--rw-r--r--   0 king       (501) staff       (20)    28192 2024-04-24 14:01:37.000000 pix2text-1.1/pix2text/pix_to_text.py
--rw-r--r--   0 king       (501) staff       (20)     5395 2024-03-29 15:11:40.000000 pix2text-1.1/pix2text/render.py
--rw-r--r--   0 king       (501) staff       (20)     8692 2022-09-07 08:30:37.000000 pix2text-1.1/pix2text/screenshot_daemon_with_server2.py
--rw-r--r--   0 king       (501) staff       (20)     2776 2024-04-21 15:29:44.000000 pix2text-1.1/pix2text/serve.py
--rw-r--r--   0 king       (501) staff       (20)    38505 2024-03-27 14:55:51.000000 pix2text-1.1/pix2text/table_inference.py
--rw-r--r--   0 king       (501) staff       (20)    38298 2024-04-22 02:22:30.000000 pix2text-1.1/pix2text/table_ocr.py
--rw-r--r--   0 king       (501) staff       (20)    37328 2024-03-29 23:43:03.000000 pix2text-1.1/pix2text/table_postprocess.py
--rw-r--r--   0 king       (501) staff       (20)    24628 2024-04-22 00:24:28.000000 pix2text-1.1/pix2text/text_formula_ocr.py
--rw-r--r--   0 king       (501) staff       (20)    31700 2024-04-21 13:52:16.000000 pix2text-1.1/pix2text/utils.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-28 15:17:52.792208 pix2text-1.1/pix2text.egg-info/
--rw-r--r--   0 king       (501) staff       (20)    14010 2024-04-28 15:17:52.000000 pix2text-1.1/pix2text.egg-info/PKG-INFO
--rw-r--r--   0 king       (501) staff       (20)     2405 2024-04-28 15:17:52.000000 pix2text-1.1/pix2text.egg-info/SOURCES.txt
--rw-r--r--   0 king       (501) staff       (20)        1 2024-04-28 15:17:52.000000 pix2text-1.1/pix2text.egg-info/dependency_links.txt
--rw-r--r--   0 king       (501) staff       (20)       42 2024-04-28 15:17:52.000000 pix2text-1.1/pix2text.egg-info/entry_points.txt
--rw-r--r--   0 king       (501) staff       (20)        1 2022-09-07 15:32:44.000000 pix2text-1.1/pix2text.egg-info/not-zip-safe
--rw-r--r--   0 king       (501) staff       (20)      269 2024-04-28 15:17:52.000000 pix2text-1.1/pix2text.egg-info/requires.txt
--rw-r--r--   0 king       (501) staff       (20)       17 2024-04-28 15:17:52.000000 pix2text-1.1/pix2text.egg-info/top_level.txt
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-28 15:17:52.801470 pix2text-1.1/scripts/
--rw-r--r--   0 king       (501) staff       (20)       16 2022-09-08 02:47:44.000000 pix2text-1.1/scripts/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     2586 2023-06-09 10:01:38.000000 pix2text-1.1/scripts/convert_label_studio_to_yolov7.py
--rw-r--r--   0 king       (501) staff       (20)     6678 2024-01-03 07:40:48.000000 pix2text-1.1/scripts/extract_p2t_results.py
--rw-r--r--   0 king       (501) staff       (20)     4198 2023-06-19 02:59:28.000000 pix2text-1.1/scripts/gen_label_studio_json.py
--rw-r--r--   0 king       (501) staff       (20)     1966 2023-06-09 09:46:06.000000 pix2text-1.1/scripts/gen_pure_formula_to_yolov7.py
--rw-r--r--   0 king       (501) staff       (20)     1609 2023-06-03 02:41:33.000000 pix2text-1.1/scripts/merge_label_studio_anno_pred_json.py
--rw-r--r--   0 king       (501) staff       (20)     4409 2022-09-08 06:37:58.000000 pix2text-1.1/scripts/object_detection3.py
--rw-r--r--   0 king       (501) staff       (20)     2413 2023-07-03 03:10:18.000000 pix2text-1.1/scripts/screenshot_daemon.py
--rw-r--r--   0 king       (501) staff       (20)      143 2024-01-01 08:28:55.000000 pix2text-1.1/scripts/try_easyocr.py
--rw-r--r--   0 king       (501) staff       (20)      796 2024-03-13 15:31:39.000000 pix2text-1.1/scripts/try_latex_correction.py
--rw-r--r--   0 king       (501) staff       (20)      787 2022-09-23 04:41:39.000000 pix2text-1.1/scripts/try_layout.py
--rw-r--r--   0 king       (501) staff       (20)      861 2024-03-29 15:11:40.000000 pix2text-1.1/scripts/try_pix2text_mfr.py
--rw-r--r--   0 king       (501) staff       (20)      845 2024-04-21 15:31:13.000000 pix2text-1.1/scripts/try_service.py
--rw-r--r--   0 king       (501) staff       (20)     1614 2024-01-05 04:02:17.000000 pix2text-1.1/scripts/try_texify.py
--rw-r--r--   0 king       (501) staff       (20)       38 2024-04-28 15:17:52.802375 pix2text-1.1/setup.cfg
--rw-r--r--   0 king       (501) staff       (20)     2424 2024-04-28 15:13:23.000000 pix2text-1.1/setup.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-28 15:17:52.801961 pix2text-1.1/tests/
--rw-r--r--   0 king       (501) staff       (20)     5861 2024-04-10 11:52:24.000000 pix2text-1.1/tests/test_pix2text.py
--rw-r--r--   0 king       (501) staff       (20)     1761 2023-07-01 07:49:03.000000 pix2text-1.1/tests/test_sort_boxes.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-30 03:15:23.758790 pix2text-1.1.0.1/
+-rw-r--r--   0 king       (501) staff       (20)     1067 2022-09-07 14:44:50.000000 pix2text-1.1.0.1/LICENSE
+-rw-r--r--   0 king       (501) staff       (20)    14122 2024-04-30 03:15:23.758627 pix2text-1.1.0.1/PKG-INFO
+-rw-r--r--   0 king       (501) staff       (20)    12903 2024-04-28 15:49:28.000000 pix2text-1.1.0.1/README.md
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-30 03:15:23.745408 pix2text-1.1.0.1/pix2text/
+-rw-r--r--   0 king       (501) staff       (20)      456 2024-04-02 11:11:40.000000 pix2text-1.1.0.1/pix2text/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)      203 2024-04-30 03:00:46.000000 pix2text-1.1.0.1/pix2text/__version__.py
+-rw-r--r--   0 king       (501) staff       (20)     1709 2022-09-10 15:50:05.000000 pix2text-1.1.0.1/pix2text/app.py
+-rw-r--r--   0 king       (501) staff       (20)     2092 2022-09-08 07:30:17.000000 pix2text-1.1.0.1/pix2text/category_mapping.py
+-rw-r--r--   0 king       (501) staff       (20)    10451 2024-04-22 00:51:42.000000 pix2text-1.1.0.1/pix2text/cli.py
+-rw-r--r--   0 king       (501) staff       (20)     3710 2024-04-16 14:50:16.000000 pix2text-1.1.0.1/pix2text/consts.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-30 03:15:23.750090 pix2text-1.1.0.1/pix2text/doc_xl_layout/
+-rw-r--r--   0 king       (501) staff       (20)      192 2024-04-03 01:13:56.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/__init__.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-30 03:15:23.751016 pix2text-1.1.0.1/pix2text/doc_xl_layout/detectors/
+-rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/detectors/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     8390 2024-04-02 08:34:16.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/detectors/base_detector_subfield.py
+-rw-r--r--   0 king       (501) staff       (20)     8722 2024-04-02 07:16:21.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/detectors/ctdet_subfield.py
+-rw-r--r--   0 king       (501) staff       (20)      137 2024-04-02 06:45:51.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/detectors/detector_factory.py
+-rw-r--r--   0 king       (501) staff       (20)    17861 2024-04-30 02:52:35.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/doc_xl_layout_parser.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-30 03:15:23.751358 pix2text-1.1.0.1/pix2text/doc_xl_layout/external/
+-rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/external/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     2510 2024-04-01 15:18:57.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/external/shapelyNMS.py
+-rw-r--r--   0 king       (501) staff       (20)      365 2024-04-01 15:18:57.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/huntie_subfield.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-30 03:15:23.752794 pix2text-1.1.0.1/pix2text/doc_xl_layout/models/
+-rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/models/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     5178 2024-04-01 15:18:57.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/models/data_parallel.py
+-rw-r--r--   0 king       (501) staff       (20)    23840 2024-04-02 07:32:06.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/models/decode.py
+-rw-r--r--   0 king       (501) staff       (20)     3443 2024-04-10 11:32:17.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/models/model.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-30 03:15:23.753115 pix2text-1.1.0.1/pix2text/doc_xl_layout/models/networks/
+-rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/models/networks/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)    24395 2024-04-01 15:18:57.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/models/networks/dlav0_subfield.py
+-rw-r--r--   0 king       (501) staff       (20)     1528 2024-04-01 15:18:57.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/models/scatter_gather.py
+-rw-r--r--   0 king       (501) staff       (20)     1800 2024-04-02 07:31:48.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/models/utils.py
+-rw-r--r--   0 king       (501) staff       (20)    23801 2024-04-02 00:43:23.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/opts.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-30 03:15:23.755031 pix2text-1.1.0.1/pix2text/doc_xl_layout/utils/
+-rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/utils/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     4818 2024-04-01 15:18:57.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/utils/ddd_utils.py
+-rw-r--r--   0 king       (501) staff       (20)    26623 2024-04-02 06:59:29.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/utils/debugger.py
+-rw-r--r--   0 king       (501) staff       (20)    18383 2024-04-02 06:47:12.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/utils/evaluation_bk.py
+-rw-r--r--   0 king       (501) staff       (20)     7851 2024-04-01 15:18:57.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/utils/image.py
+-rw-r--r--   0 king       (501) staff       (20)     5368 2024-04-02 06:47:54.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/utils/post_process.py
+-rw-r--r--   0 king       (501) staff       (20)      533 2024-04-01 15:18:57.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/utils/utils.py
+-rw-r--r--   0 king       (501) staff       (20)     8844 2024-04-02 06:20:49.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/wrapper.py
+-rw-r--r--   0 king       (501) staff       (20)    12517 2024-03-27 09:59:17.000000 pix2text-1.1.0.1/pix2text/element.py
+-rw-r--r--   0 king       (501) staff       (20)    17431 2024-04-22 02:21:39.000000 pix2text-1.1.0.1/pix2text/latex_ocr.py
+-rw-r--r--   0 king       (501) staff       (20)    13244 2024-01-11 04:27:38.000000 pix2text-1.1.0.1/pix2text/latex_ocr0.py
+-rw-r--r--   0 king       (501) staff       (20)    22526 2024-01-10 13:35:10.000000 pix2text-1.1.0.1/pix2text/latex_recog.py
+-rw-r--r--   0 king       (501) staff       (20)     4016 2024-04-06 13:32:28.000000 pix2text-1.1.0.1/pix2text/layout_parser.py
+-rw-r--r--   0 king       (501) staff       (20)     3567 2022-09-13 02:10:01.000000 pix2text-1.1.0.1/pix2text/object_detector.py
+-rw-r--r--   0 king       (501) staff       (20)     7285 2024-04-27 13:58:01.000000 pix2text-1.1.0.1/pix2text/ocr_engine.py
+-rw-r--r--   0 king       (501) staff       (20)    10497 2024-04-30 02:55:47.000000 pix2text-1.1.0.1/pix2text/page_elements.py
+-rw-r--r--   0 king       (501) staff       (20)    28192 2024-04-24 14:01:37.000000 pix2text-1.1.0.1/pix2text/pix_to_text.py
+-rw-r--r--   0 king       (501) staff       (20)     5413 2024-04-30 02:57:49.000000 pix2text-1.1.0.1/pix2text/render.py
+-rw-r--r--   0 king       (501) staff       (20)     8692 2022-09-07 08:30:37.000000 pix2text-1.1.0.1/pix2text/screenshot_daemon_with_server2.py
+-rw-r--r--   0 king       (501) staff       (20)     2776 2024-04-21 15:29:44.000000 pix2text-1.1.0.1/pix2text/serve.py
+-rw-r--r--   0 king       (501) staff       (20)    38505 2024-03-27 14:55:51.000000 pix2text-1.1.0.1/pix2text/table_inference.py
+-rw-r--r--   0 king       (501) staff       (20)    38370 2024-04-30 02:58:35.000000 pix2text-1.1.0.1/pix2text/table_ocr.py
+-rw-r--r--   0 king       (501) staff       (20)    37328 2024-03-29 23:43:03.000000 pix2text-1.1.0.1/pix2text/table_postprocess.py
+-rw-r--r--   0 king       (501) staff       (20)    24628 2024-04-22 00:24:28.000000 pix2text-1.1.0.1/pix2text/text_formula_ocr.py
+-rw-r--r--   0 king       (501) staff       (20)    31700 2024-04-21 13:52:16.000000 pix2text-1.1.0.1/pix2text/utils.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-30 03:15:23.746924 pix2text-1.1.0.1/pix2text.egg-info/
+-rw-r--r--   0 king       (501) staff       (20)    14122 2024-04-30 03:15:23.000000 pix2text-1.1.0.1/pix2text.egg-info/PKG-INFO
+-rw-r--r--   0 king       (501) staff       (20)     2405 2024-04-30 03:15:23.000000 pix2text-1.1.0.1/pix2text.egg-info/SOURCES.txt
+-rw-r--r--   0 king       (501) staff       (20)        1 2024-04-30 03:15:23.000000 pix2text-1.1.0.1/pix2text.egg-info/dependency_links.txt
+-rw-r--r--   0 king       (501) staff       (20)       42 2024-04-30 03:15:23.000000 pix2text-1.1.0.1/pix2text.egg-info/entry_points.txt
+-rw-r--r--   0 king       (501) staff       (20)        1 2022-09-07 15:32:44.000000 pix2text-1.1.0.1/pix2text.egg-info/not-zip-safe
+-rw-r--r--   0 king       (501) staff       (20)      269 2024-04-30 03:15:23.000000 pix2text-1.1.0.1/pix2text.egg-info/requires.txt
+-rw-r--r--   0 king       (501) staff       (20)       17 2024-04-30 03:15:23.000000 pix2text-1.1.0.1/pix2text.egg-info/top_level.txt
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-30 03:15:23.757838 pix2text-1.1.0.1/scripts/
+-rw-r--r--   0 king       (501) staff       (20)       16 2022-09-08 02:47:44.000000 pix2text-1.1.0.1/scripts/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     2586 2023-06-09 10:01:38.000000 pix2text-1.1.0.1/scripts/convert_label_studio_to_yolov7.py
+-rw-r--r--   0 king       (501) staff       (20)     6678 2024-01-03 07:40:48.000000 pix2text-1.1.0.1/scripts/extract_p2t_results.py
+-rw-r--r--   0 king       (501) staff       (20)     4198 2023-06-19 02:59:28.000000 pix2text-1.1.0.1/scripts/gen_label_studio_json.py
+-rw-r--r--   0 king       (501) staff       (20)     1966 2023-06-09 09:46:06.000000 pix2text-1.1.0.1/scripts/gen_pure_formula_to_yolov7.py
+-rw-r--r--   0 king       (501) staff       (20)     1609 2023-06-03 02:41:33.000000 pix2text-1.1.0.1/scripts/merge_label_studio_anno_pred_json.py
+-rw-r--r--   0 king       (501) staff       (20)     4409 2022-09-08 06:37:58.000000 pix2text-1.1.0.1/scripts/object_detection3.py
+-rw-r--r--   0 king       (501) staff       (20)     2413 2023-07-03 03:10:18.000000 pix2text-1.1.0.1/scripts/screenshot_daemon.py
+-rw-r--r--   0 king       (501) staff       (20)      143 2024-01-01 08:28:55.000000 pix2text-1.1.0.1/scripts/try_easyocr.py
+-rw-r--r--   0 king       (501) staff       (20)      796 2024-03-13 15:31:39.000000 pix2text-1.1.0.1/scripts/try_latex_correction.py
+-rw-r--r--   0 king       (501) staff       (20)      787 2022-09-23 04:41:39.000000 pix2text-1.1.0.1/scripts/try_layout.py
+-rw-r--r--   0 king       (501) staff       (20)      861 2024-03-29 15:11:40.000000 pix2text-1.1.0.1/scripts/try_pix2text_mfr.py
+-rw-r--r--   0 king       (501) staff       (20)      845 2024-04-21 15:31:13.000000 pix2text-1.1.0.1/scripts/try_service.py
+-rw-r--r--   0 king       (501) staff       (20)     1614 2024-01-05 04:02:17.000000 pix2text-1.1.0.1/scripts/try_texify.py
+-rw-r--r--   0 king       (501) staff       (20)       38 2024-04-30 03:15:23.758845 pix2text-1.1.0.1/setup.cfg
+-rw-r--r--   0 king       (501) staff       (20)     2522 2024-04-30 03:06:08.000000 pix2text-1.1.0.1/setup.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-30 03:15:23.758424 pix2text-1.1.0.1/tests/
+-rw-r--r--   0 king       (501) staff       (20)     5861 2024-04-10 11:52:24.000000 pix2text-1.1.0.1/tests/test_pix2text.py
+-rw-r--r--   0 king       (501) staff       (20)     1761 2023-07-01 07:49:03.000000 pix2text-1.1.0.1/tests/test_sort_boxes.py
```

### Comparing `pix2text-1.1/LICENSE` & `pix2text-1.1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/PKG-INFO` & `pix2text-1.1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: pix2text
-Version: 1.1
-Summary: An Open-Source Python3 tool for Optical Character Recognition (OCR) and LaTeX expression extraction from images; a Free Alternative to Mathpix
+Version: 1.1.0.1
+Summary: An Open-Source Python3 tool for recognizing layouts, tables, math formulas, and text in images, converting them into Markdown format. A free alternative to Mathpix, empowering seamless conversion of visual content into text-based representations.
 Home-page: https://github.com/breezedeus/pix2text
 Author: breezedeus
 Author-email: breezedeus@163.com
 License: MIT
 Platform: Mac
 Platform: Linux
 Platform: Windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 Provides-Extra: multilingual
 Provides-Extra: dev
 Provides-Extra: serve
 License-File: LICENSE
 
@@ -217,23 +217,23 @@
 
 ## Online Demo 🤗
 
 You can also try the **[Online Demo](https://huggingface.co/spaces/breezedeus/Pix2Text-Demo)** to see the performance of **P2T** in various languages. However, the online demo operates on lower hardware specifications and may be slower. For Simplified Chinese or English images, it is recommended to use the **[P2T Online Service](https://p2t.breezedeus.com)**.
 
 ## Examples
 
-See: [Pix2Text Online Documentation/Examples](https://pix2text.readthedocs.io/en/latest/examples/).
+See: [Pix2Text Online Documentation/Examples](https://pix2text.readthedocs.io/zh/latest/examples_en/).
 
 ## Usage
 
-See: [Pix2Text Online Documentation/Usage](https://pix2text.readthedocs.io/en/latest/usage/).
+See: [Pix2Text Online Documentation/Usage](https://pix2text.readthedocs.io/zh/latest/usage/).
 
 ## Models
 
-See: [Pix2Text Online Documentation/Models](https://pix2text.readthedocs.io/en/latest/models/).
+See: [Pix2Text Online Documentation/Models](https://pix2text.readthedocs.io/zh/latest/models/).
 
 ## Install
 
 Well, one line of command is enough if it goes well.
 
 ```bash
 pip install pix2text
```

### Comparing `pix2text-1.1/README.md` & `pix2text-1.1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -188,23 +188,23 @@
 
 ## Online Demo 🤗
 
 You can also try the **[Online Demo](https://huggingface.co/spaces/breezedeus/Pix2Text-Demo)** to see the performance of **P2T** in various languages. However, the online demo operates on lower hardware specifications and may be slower. For Simplified Chinese or English images, it is recommended to use the **[P2T Online Service](https://p2t.breezedeus.com)**.
 
 ## Examples
 
-See: [Pix2Text Online Documentation/Examples](https://pix2text.readthedocs.io/en/latest/examples/).
+See: [Pix2Text Online Documentation/Examples](https://pix2text.readthedocs.io/zh/latest/examples_en/).
 
 ## Usage
 
-See: [Pix2Text Online Documentation/Usage](https://pix2text.readthedocs.io/en/latest/usage/).
+See: [Pix2Text Online Documentation/Usage](https://pix2text.readthedocs.io/zh/latest/usage/).
 
 ## Models
 
-See: [Pix2Text Online Documentation/Models](https://pix2text.readthedocs.io/en/latest/models/).
+See: [Pix2Text Online Documentation/Models](https://pix2text.readthedocs.io/zh/latest/models/).
 
 ## Install
 
 Well, one line of command is enough if it goes well.
 
 ```bash
 pip install pix2text
```

### Comparing `pix2text-1.1/pix2text/app.py` & `pix2text-1.1.0.1/pix2text/app.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/category_mapping.py` & `pix2text-1.1.0.1/pix2text/category_mapping.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/cli.py` & `pix2text-1.1.0.1/pix2text/cli.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/consts.py` & `pix2text-1.1.0.1/pix2text/consts.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/doc_xl_layout/detectors/base_detector_subfield.py` & `pix2text-1.1.0.1/pix2text/doc_xl_layout/detectors/base_detector_subfield.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/doc_xl_layout/detectors/ctdet_subfield.py` & `pix2text-1.1.0.1/pix2text/doc_xl_layout/detectors/ctdet_subfield.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/doc_xl_layout/doc_xl_layout_parser.py` & `pix2text-1.1.0.1/pix2text/doc_xl_layout/doc_xl_layout_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,20 +201,18 @@
 
         layout_out = out.to_json()
         debug_dir = None
         if kwargs.get('save_debug_res', None):
             debug_dir = Path(kwargs.get('save_debug_res'))
             debug_dir.mkdir(exist_ok=True, parents=True)
         if debug_dir is not None:
-            json.dump(
-                layout_out,
-                open(debug_dir / 'layout_out.json', 'w'),
-                indent=2,
-                ensure_ascii=False,
-            )
+            with open(debug_dir / 'layout_out.json', 'w', encoding='utf-8') as f:
+                json.dump(
+                    layout_out, f, indent=2, ensure_ascii=False,
+                )
         if layout_out:
             layout_out = self._preprocess_outputs(img0, layout_out)
             layout_out, column_meta = self._format_outputs(
                 img0, layout_out, table_as_image
             )
         else:
             layout_out, column_meta = [], {}
@@ -335,16 +333,15 @@
                 cur_box_ymin, cur_box_ymax = cur_box[0, 1], cur_box[2, 1]
                 if (
                     box_info['type'] == ElementType.TEXT
                     and (
                         cur_box_xmax < full_column_xmin
                         or cur_box_xmin > full_column_xmax
                     )
-                    and cur_box_ymax - cur_box_ymin
-                    > 5 * (cur_box_xmax - cur_box_xmin)
+                    and cur_box_ymax - cur_box_ymin > 5 * (cur_box_xmax - cur_box_xmin)
                 ):  # unnecessary block
                     box_info['type'] = ElementType.IGNORED
                 filtered_out.append(box_info)
 
             final_out = filtered_out
 
         # handle abnormal elements (col_number == -2)
```

### Comparing `pix2text-1.1/pix2text/doc_xl_layout/external/shapelyNMS.py` & `pix2text-1.1.0.1/pix2text/doc_xl_layout/external/shapelyNMS.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/doc_xl_layout/models/data_parallel.py` & `pix2text-1.1.0.1/pix2text/doc_xl_layout/models/data_parallel.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/doc_xl_layout/models/decode.py` & `pix2text-1.1.0.1/pix2text/doc_xl_layout/models/decode.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/doc_xl_layout/models/model.py` & `pix2text-1.1.0.1/pix2text/doc_xl_layout/models/model.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/doc_xl_layout/models/networks/dlav0_subfield.py` & `pix2text-1.1.0.1/pix2text/doc_xl_layout/models/networks/dlav0_subfield.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/doc_xl_layout/models/scatter_gather.py` & `pix2text-1.1.0.1/pix2text/doc_xl_layout/models/scatter_gather.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/doc_xl_layout/models/utils.py` & `pix2text-1.1.0.1/pix2text/doc_xl_layout/models/utils.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/doc_xl_layout/opts.py` & `pix2text-1.1.0.1/pix2text/doc_xl_layout/opts.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/doc_xl_layout/utils/ddd_utils.py` & `pix2text-1.1.0.1/pix2text/doc_xl_layout/utils/ddd_utils.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/doc_xl_layout/utils/debugger.py` & `pix2text-1.1.0.1/pix2text/doc_xl_layout/utils/debugger.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/doc_xl_layout/utils/evaluation_bk.py` & `pix2text-1.1.0.1/pix2text/doc_xl_layout/utils/evaluation_bk.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/doc_xl_layout/utils/image.py` & `pix2text-1.1.0.1/pix2text/doc_xl_layout/utils/image.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/doc_xl_layout/utils/post_process.py` & `pix2text-1.1.0.1/pix2text/doc_xl_layout/utils/post_process.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/doc_xl_layout/utils/utils.py` & `pix2text-1.1.0.1/pix2text/doc_xl_layout/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/doc_xl_layout/wrapper.py` & `pix2text-1.1.0.1/pix2text/doc_xl_layout/wrapper.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/element.py` & `pix2text-1.1.0.1/pix2text/element.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/latex_ocr.py` & `pix2text-1.1.0.1/pix2text/latex_ocr.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/latex_ocr0.py` & `pix2text-1.1.0.1/pix2text/latex_ocr0.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/latex_recog.py` & `pix2text-1.1.0.1/pix2text/latex_recog.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/layout_parser.py` & `pix2text-1.1.0.1/pix2text/layout_parser.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/object_detector.py` & `pix2text-1.1.0.1/pix2text/object_detector.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/ocr_engine.py` & `pix2text-1.1.0.1/pix2text/ocr_engine.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/page_elements.py` & `pix2text-1.1.0.1/pix2text/page_elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,15 +216,15 @@
                 md_out += '\n\n' + cur_txt
 
         line_sep = '\n'
         md_out = re.sub(
             rf'{line_sep}{{2,}}', f'{line_sep}{line_sep}', md_out
         )  # 把2个以上的连续 '\n' 替换为 '\n\n'
         if markdown_fn:
-            with open(out_dir / markdown_fn, 'w') as f:
+            with open(out_dir / markdown_fn, 'w', encoding='utf-8') as f:
                 f.write(md_out)
         return md_out
 
     def _ele_to_markdown(self, element: Element, root_url: Optional[str], out_dir: Union[str, Path]):
         type = element.type
         text = element.text
         if type in (ElementType.TEXT, ElementType.TABLE):
@@ -310,10 +310,10 @@
                 md_out += '\n\n' + cur_txt
 
         line_sep = '\n'
         md_out = re.sub(
             rf'{line_sep}{{2,}}', f'{line_sep}{line_sep}', md_out
         )  # 把2个以上的连续 '\n' 替换为 '\n\n'
         if markdown_fn:
-            with open(out_dir / markdown_fn, 'w') as f:
+            with open(out_dir / markdown_fn, 'w', encoding='utf-8') as f:
                 f.write(md_out)
         return md_out
```

### Comparing `pix2text-1.1/pix2text/pix_to_text.py` & `pix2text-1.1.0.1/pix2text/pix_to_text.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/render.py` & `pix2text-1.1.0.1/pix2text/render.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,9 +209,9 @@
         console.log(data)
       })()
     </script>
   </body>
 </html>
     """
 
-    with open(out_html_fp, 'w') as f:
+    with open(out_html_fp, 'w', encoding='utf-8') as f:
         f.writelines(html_str)
```

### Comparing `pix2text-1.1/pix2text/screenshot_daemon_with_server2.py` & `pix2text-1.1.0.1/pix2text/screenshot_daemon_with_server2.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/serve.py` & `pix2text-1.1.0.1/pix2text/serve.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/table_inference.py` & `pix2text-1.1.0.1/pix2text/table_inference.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/table_ocr.py` & `pix2text-1.1.0.1/pix2text/table_ocr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1094,40 +1094,40 @@
 def output_result(key, val, args, img, img_file):
     import json
 
     if key == 'objects':
         # if args.verbose:
         #     print(val)
         out_file = img_file.replace(".jpg", "_objects.json")
-        with open(os.path.join(args.out_dir, out_file), 'w') as f:
+        with open(os.path.join(args.out_dir, out_file), 'w', encoding='utf-8') as f:
             json.dump(val, f)
         # if args.visualize:
         #     out_file = img_file.replace(".jpg", "_fig_tables.jpg")
         #     out_path = os.path.join(args.out_dir, out_file)
         #     visualize_detected_tables(img, val, out_path)
     elif not key == 'image' and not key == 'tokens':
         for idx, elem in enumerate(val):
             if key == 'crops':
                 for idx, cropped_table in enumerate(val):
                     out_img_file = img_file.replace(".jpg", "_table_{}.jpg".format(idx))
                     cropped_table['image'].save(
                         os.path.join(args.out_dir, out_img_file)
                     )
                     out_words_file = out_img_file.replace(".jpg", "_words.json")
-                    with open(os.path.join(args.out_dir, out_words_file), 'w') as f:
+                    with open(os.path.join(args.out_dir, out_words_file), 'w', encoding='utf-8') as f:
                         json.dump(cropped_table['tokens'], f)
             elif key == 'cells':
                 out_file = img_file.replace(".jpg", "_{}_objects.json".format(idx))
-                with open(os.path.join(args.out_dir, out_file), 'w') as f:
+                with open(os.path.join(args.out_dir, out_file), 'w', encoding='utf-8') as f:
                     json.dump(elem, f)
                 # if args.verbose:
                 #     print(elem)
                 if True:
                     out_file = img_file.replace(".jpg", "_fig_cells.jpg")
                     out_path = os.path.join(args.out_dir, out_file)
                     visualize_cells(img, elem, out_path)
             else:
                 out_file = img_file.replace(".jpg", "_{}.{}".format(idx, key))
-                with open(os.path.join(args.out_dir, out_file), 'w') as f:
+                with open(os.path.join(args.out_dir, out_file), 'w', encoding='utf-8') as f:
                     f.write(elem)
                 if args.verbose:
                     print(elem)
```

### Comparing `pix2text-1.1/pix2text/table_postprocess.py` & `pix2text-1.1.0.1/pix2text/table_postprocess.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/text_formula_ocr.py` & `pix2text-1.1.0.1/pix2text/text_formula_ocr.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text/utils.py` & `pix2text-1.1.0.1/pix2text/utils.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/pix2text.egg-info/PKG-INFO` & `pix2text-1.1.0.1/pix2text.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: pix2text
-Version: 1.1
-Summary: An Open-Source Python3 tool for Optical Character Recognition (OCR) and LaTeX expression extraction from images; a Free Alternative to Mathpix
+Version: 1.1.0.1
+Summary: An Open-Source Python3 tool for recognizing layouts, tables, math formulas, and text in images, converting them into Markdown format. A free alternative to Mathpix, empowering seamless conversion of visual content into text-based representations.
 Home-page: https://github.com/breezedeus/pix2text
 Author: breezedeus
 Author-email: breezedeus@163.com
 License: MIT
 Platform: Mac
 Platform: Linux
 Platform: Windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 Provides-Extra: multilingual
 Provides-Extra: dev
 Provides-Extra: serve
 License-File: LICENSE
 
@@ -217,23 +217,23 @@
 
 ## Online Demo 🤗
 
 You can also try the **[Online Demo](https://huggingface.co/spaces/breezedeus/Pix2Text-Demo)** to see the performance of **P2T** in various languages. However, the online demo operates on lower hardware specifications and may be slower. For Simplified Chinese or English images, it is recommended to use the **[P2T Online Service](https://p2t.breezedeus.com)**.
 
 ## Examples
 
-See: [Pix2Text Online Documentation/Examples](https://pix2text.readthedocs.io/en/latest/examples/).
+See: [Pix2Text Online Documentation/Examples](https://pix2text.readthedocs.io/zh/latest/examples_en/).
 
 ## Usage
 
-See: [Pix2Text Online Documentation/Usage](https://pix2text.readthedocs.io/en/latest/usage/).
+See: [Pix2Text Online Documentation/Usage](https://pix2text.readthedocs.io/zh/latest/usage/).
 
 ## Models
 
-See: [Pix2Text Online Documentation/Models](https://pix2text.readthedocs.io/en/latest/models/).
+See: [Pix2Text Online Documentation/Models](https://pix2text.readthedocs.io/zh/latest/models/).
 
 ## Install
 
 Well, one line of command is enough if it goes well.
 
 ```bash
 pip install pix2text
```

### Comparing `pix2text-1.1/pix2text.egg-info/SOURCES.txt` & `pix2text-1.1.0.1/pix2text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/scripts/convert_label_studio_to_yolov7.py` & `pix2text-1.1.0.1/scripts/convert_label_studio_to_yolov7.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/scripts/extract_p2t_results.py` & `pix2text-1.1.0.1/scripts/extract_p2t_results.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/scripts/gen_label_studio_json.py` & `pix2text-1.1.0.1/scripts/gen_label_studio_json.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/scripts/gen_pure_formula_to_yolov7.py` & `pix2text-1.1.0.1/scripts/gen_pure_formula_to_yolov7.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/scripts/merge_label_studio_anno_pred_json.py` & `pix2text-1.1.0.1/scripts/merge_label_studio_anno_pred_json.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/scripts/object_detection3.py` & `pix2text-1.1.0.1/scripts/object_detection3.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/scripts/screenshot_daemon.py` & `pix2text-1.1.0.1/scripts/screenshot_daemon.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/scripts/try_latex_correction.py` & `pix2text-1.1.0.1/scripts/try_latex_correction.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/scripts/try_layout.py` & `pix2text-1.1.0.1/scripts/try_layout.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/scripts/try_pix2text_mfr.py` & `pix2text-1.1.0.1/scripts/try_pix2text_mfr.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/scripts/try_service.py` & `pix2text-1.1.0.1/scripts/try_service.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/scripts/try_texify.py` & `pix2text-1.1.0.1/scripts/try_texify.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/setup.py` & `pix2text-1.1.0.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 )
 
 required = [
     "click",
     "tqdm",
     "numpy",
     "opencv-python",
-    "cnocr[ort-cpu]>=2.3.0.1",
-    "cnstd>=1.2.3.5",
+    "cnocr[ort-cpu]>=2.3.0.2",
+    "cnstd>=1.2.3.6",
     "pillow",
     "torch",
     "torchvision",
     "transformers>=4.37.0",
     "optimum[onnxruntime]",
     "PyMuPDF",
     "pyspellchecker",
@@ -46,16 +46,15 @@
 [console_scripts]
 p2t = pix2text.cli:cli
 """
 
 setup(
     name=PACKAGE_NAME,
     version=about['__version__'],
-    description="An Open-Source Python3 tool for Optical Character Recognition (OCR) "
-    "and LaTeX expression extraction from images; a Free Alternative to Mathpix",
+    description="An Open-Source Python3 tool for recognizing layouts, tables, math formulas, and text in images, converting them into Markdown format. A free alternative to Mathpix, empowering seamless conversion of visual content into text-based representations.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='breezedeus',
     author_email='breezedeus@163.com',
     license='MIT',
     url='https://github.com/breezedeus/pix2text',
     platforms=["Mac", "Linux", "Windows"],
@@ -70,14 +69,14 @@
         'Development Status :: 4 - Beta',
         'Operating System :: OS Independent',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: Implementation',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
     ],
 )
```

### Comparing `pix2text-1.1/tests/test_pix2text.py` & `pix2text-1.1.0.1/tests/test_pix2text.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1/tests/test_sort_boxes.py` & `pix2text-1.1.0.1/tests/test_sort_boxes.py`

 * *Files identical despite different names*

