# Comparing `tmp/pub_analyzer-0.2.0.tar.gz` & `tmp/pub_analyzer-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pub_analyzer-0.2.0.tar", max compression
+gzip compressed data, was "pub_analyzer-0.3.0.tar", max compression
```

## Comparing `pub_analyzer-0.2.0.tar` & `pub_analyzer-0.3.0.tar`

### file list

```diff
@@ -1,63 +1,68 @@
--rw-r--r--   0        0        0     1080 2022-12-26 20:01:03.907758 pub_analyzer-0.2.0/LICENSE
--rw-r--r--   0        0        0     3052 2023-11-01 04:32:38.425562 pub_analyzer-0.2.0/README.md
--rw-r--r--   0        0        0       40 2023-07-10 19:44:33.060421 pub_analyzer-0.2.0/pub_analyzer/__init__.py
--rw-r--r--   0        0        0     1461 2023-11-01 04:32:38.429562 pub_analyzer-0.2.0/pub_analyzer/css/author.tcss
--rw-r--r--   0        0        0     1400 2023-11-01 04:32:38.429562 pub_analyzer-0.2.0/pub_analyzer/css/body.tcss
--rw-r--r--   0        0        0      581 2023-11-09 01:45:49.365779 pub_analyzer-0.2.0/pub_analyzer/css/buttons.tcss
--rw-r--r--   0        0        0      506 2023-11-01 04:32:38.429562 pub_analyzer-0.2.0/pub_analyzer/css/checkbox.tcss
--rw-r--r--   0        0        0      605 2023-11-01 04:32:38.430562 pub_analyzer-0.2.0/pub_analyzer/css/collapsible.tcss
--rw-r--r--   0        0        0      994 2023-11-01 04:32:38.430562 pub_analyzer-0.2.0/pub_analyzer/css/datatable.tcss
--rw-r--r--   0        0        0     1527 2023-11-01 04:32:38.430562 pub_analyzer-0.2.0/pub_analyzer/css/institution.tcss
--rw-r--r--   0        0        0      816 2023-11-01 04:32:38.430562 pub_analyzer-0.2.0/pub_analyzer/css/main.tcss
--rw-r--r--   0        0        0     2066 2023-11-01 04:32:38.430562 pub_analyzer-0.2.0/pub_analyzer/css/report.tcss
--rw-r--r--   0        0        0     1326 2023-11-01 04:32:38.430562 pub_analyzer-0.2.0/pub_analyzer/css/search.tcss
--rw-r--r--   0        0        0      311 2023-11-01 04:32:38.430562 pub_analyzer-0.2.0/pub_analyzer/css/tabs.tcss
--rw-r--r--   0        0        0      818 2023-11-01 04:32:38.430562 pub_analyzer-0.2.0/pub_analyzer/css/tree.tcss
--rw-r--r--   0        0        0       22 2023-07-25 02:23:02.223194 pub_analyzer-0.2.0/pub_analyzer/internal/__init__.py
--rw-r--r--   0        0        0     2268 2023-11-01 04:32:38.430562 pub_analyzer-0.2.0/pub_analyzer/internal/identifier.py
--rw-r--r--   0        0        0     2144 2023-11-01 04:32:38.430562 pub_analyzer-0.2.0/pub_analyzer/internal/render.py
--rw-r--r--   0        0        0    14666 2023-11-01 04:32:38.430562 pub_analyzer-0.2.0/pub_analyzer/internal/report.py
--rw-r--r--   0        0        0     2407 2023-08-09 21:25:58.963224 pub_analyzer-0.2.0/pub_analyzer/internal/templates/author/author_resume.typ
--rw-r--r--   0        0        0     1378 2023-11-01 04:32:38.430562 pub_analyzer-0.2.0/pub_analyzer/internal/templates/author/report.typ
--rw-r--r--   0        0        0      593 2023-11-01 04:32:38.430562 pub_analyzer-0.2.0/pub_analyzer/internal/templates/author/sources.typ
--rw-r--r--   0        0        0     1966 2023-11-01 04:32:38.431562 pub_analyzer-0.2.0/pub_analyzer/internal/templates/author/works.typ
--rw-r--r--   0        0        0     3436 2023-11-01 04:32:38.431562 pub_analyzer-0.2.0/pub_analyzer/internal/templates/author/works_extended.typ
--rw-r--r--   0        0        0     2204 2023-11-01 04:32:38.431562 pub_analyzer-0.2.0/pub_analyzer/main.py
--rw-r--r--   0        0        0       59 2023-07-11 19:12:41.033667 pub_analyzer-0.2.0/pub_analyzer/models/__init__.py
--rw-r--r--   0        0        0     2435 2023-11-01 04:32:38.431562 pub_analyzer-0.2.0/pub_analyzer/models/author.py
--rw-r--r--   0        0        0     2826 2023-11-01 04:32:38.431562 pub_analyzer-0.2.0/pub_analyzer/models/institution.py
--rw-r--r--   0        0        0     2575 2023-11-01 04:32:38.431562 pub_analyzer-0.2.0/pub_analyzer/models/report.py
--rw-r--r--   0        0        0      453 2023-11-01 04:32:38.431562 pub_analyzer-0.2.0/pub_analyzer/models/source.py
--rw-r--r--   0        0        0     3593 2023-11-01 04:32:38.431562 pub_analyzer-0.2.0/pub_analyzer/models/work.py
--rw-r--r--   0        0        0       18 2023-07-25 02:25:16.966008 pub_analyzer-0.2.0/pub_analyzer/widgets/__init__.py
--rw-r--r--   0        0        0       22 2023-07-05 01:08:16.930978 pub_analyzer-0.2.0/pub_analyzer/widgets/author/__init__.py
--rw-r--r--   0        0        0     2416 2023-11-01 04:32:38.431562 pub_analyzer-0.2.0/pub_analyzer/widgets/author/cards.py
--rw-r--r--   0        0        0     5032 2023-11-01 04:32:38.431562 pub_analyzer-0.2.0/pub_analyzer/widgets/author/core.py
--rw-r--r--   0        0        0      793 2023-11-01 04:32:38.432562 pub_analyzer-0.2.0/pub_analyzer/widgets/author/tables.py
--rw-r--r--   0        0        0      972 2023-08-02 21:18:14.509439 pub_analyzer-0.2.0/pub_analyzer/widgets/body.py
--rw-r--r--   0        0        0      287 2023-11-01 04:32:38.432562 pub_analyzer-0.2.0/pub_analyzer/widgets/common/__init__.py
--rw-r--r--   0        0        0      595 2023-07-05 00:41:47.490136 pub_analyzer-0.2.0/pub_analyzer/widgets/common/card.py
--rw-r--r--   0        0        0     6460 2023-11-01 04:32:38.432562 pub_analyzer-0.2.0/pub_analyzer/widgets/common/filesystem.py
--rw-r--r--   0        0        0     3373 2023-11-01 04:32:38.432562 pub_analyzer-0.2.0/pub_analyzer/widgets/common/filters.py
--rw-r--r--   0        0        0     2649 2023-11-01 04:32:38.432562 pub_analyzer-0.2.0/pub_analyzer/widgets/common/input.py
--rw-r--r--   0        0        0      882 2023-11-01 04:48:22.732265 pub_analyzer-0.2.0/pub_analyzer/widgets/common/modal.py
--rw-r--r--   0        0        0     1493 2023-11-01 04:32:38.432562 pub_analyzer-0.2.0/pub_analyzer/widgets/common/selector.py
--rw-r--r--   0        0        0       27 2023-08-03 06:51:44.172868 pub_analyzer-0.2.0/pub_analyzer/widgets/institution/__init__.py
--rw-r--r--   0        0        0     2862 2023-11-01 04:32:38.432562 pub_analyzer-0.2.0/pub_analyzer/widgets/institution/cards.py
--rw-r--r--   0        0        0     5279 2023-11-01 04:32:38.432562 pub_analyzer-0.2.0/pub_analyzer/widgets/institution/core.py
--rw-r--r--   0        0        0      838 2023-11-01 04:32:38.432562 pub_analyzer-0.2.0/pub_analyzer/widgets/institution/tables.py
--rw-r--r--   0        0        0       54 2023-07-04 07:25:06.831900 pub_analyzer-0.2.0/pub_analyzer/widgets/report/__init__.py
--rw-r--r--   0        0        0     1227 2023-08-02 04:47:16.018134 pub_analyzer-0.2.0/pub_analyzer/widgets/report/author.py
--rw-r--r--   0        0        0     4818 2023-11-01 04:32:38.432562 pub_analyzer-0.2.0/pub_analyzer/widgets/report/cards.py
--rw-r--r--   0        0        0    10902 2023-11-01 04:32:38.432562 pub_analyzer-0.2.0/pub_analyzer/widgets/report/core.py
--rw-r--r--   0        0        0     4762 2023-11-01 04:32:38.433562 pub_analyzer-0.2.0/pub_analyzer/widgets/report/export.py
--rw-r--r--   0        0        0     1297 2023-08-04 07:15:14.238626 pub_analyzer-0.2.0/pub_analyzer/widgets/report/institution.py
--rw-r--r--   0        0        0     2892 2023-11-01 04:32:38.433562 pub_analyzer-0.2.0/pub_analyzer/widgets/report/locations.py
--rw-r--r--   0        0        0     2750 2023-11-01 04:32:38.433562 pub_analyzer-0.2.0/pub_analyzer/widgets/report/source.py
--rw-r--r--   0        0        0     7873 2023-11-01 04:32:38.433562 pub_analyzer-0.2.0/pub_analyzer/widgets/report/work.py
--rw-r--r--   0        0        0      239 2023-11-01 04:32:38.433562 pub_analyzer-0.2.0/pub_analyzer/widgets/search/__init__.py
--rw-r--r--   0        0        0     3861 2023-11-01 04:32:38.433562 pub_analyzer-0.2.0/pub_analyzer/widgets/search/core.py
--rw-r--r--   0        0        0     3692 2023-11-01 04:32:38.433562 pub_analyzer-0.2.0/pub_analyzer/widgets/search/results.py
--rw-r--r--   0        0        0     2330 2023-11-01 04:32:38.433562 pub_analyzer-0.2.0/pub_analyzer/widgets/sidebar.py
--rw-r--r--   0        0        0     2931 2023-11-09 01:50:44.968944 pub_analyzer-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4376 1970-01-01 00:00:00.000000 pub_analyzer-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-10-06 05:46:06.880454 pub_analyzer-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3132 2024-04-30 06:16:38.329285 pub_analyzer-0.3.0/README.md
+-rw-r--r--   0        0        0       40 2023-10-06 05:46:06.890639 pub_analyzer-0.3.0/pub_analyzer/__init__.py
+-rw-r--r--   0        0        0     1682 2024-01-18 00:45:36.189087 pub_analyzer-0.3.0/pub_analyzer/css/body.tcss
+-rw-r--r--   0        0        0      546 2023-12-22 01:48:25.522822 pub_analyzer-0.3.0/pub_analyzer/css/buttons.tcss
+-rw-r--r--   0        0        0      506 2023-10-06 05:46:06.891722 pub_analyzer-0.3.0/pub_analyzer/css/checkbox.tcss
+-rw-r--r--   0        0        0      605 2023-10-30 19:25:59.898394 pub_analyzer-0.3.0/pub_analyzer/css/collapsible.tcss
+-rw-r--r--   0        0        0      994 2023-10-06 05:46:06.891923 pub_analyzer-0.3.0/pub_analyzer/css/datatable.tcss
+-rw-r--r--   0        0        0      834 2023-12-31 06:43:19.855015 pub_analyzer-0.3.0/pub_analyzer/css/main.tcss
+-rw-r--r--   0        0        0     2066 2023-10-06 05:46:06.892534 pub_analyzer-0.3.0/pub_analyzer/css/report.tcss
+-rw-r--r--   0        0        0     1326 2023-10-06 05:46:06.892749 pub_analyzer-0.3.0/pub_analyzer/css/search.tcss
+-rw-r--r--   0        0        0     1350 2024-01-10 22:08:32.420163 pub_analyzer-0.3.0/pub_analyzer/css/summary.tcss
+-rw-r--r--   0        0        0      311 2023-10-06 05:46:06.892974 pub_analyzer-0.3.0/pub_analyzer/css/tabs.tcss
+-rw-r--r--   0        0        0      818 2023-10-06 05:46:06.893211 pub_analyzer-0.3.0/pub_analyzer/css/tree.tcss
+-rw-r--r--   0        0        0       22 2023-10-06 05:46:06.893573 pub_analyzer-0.3.0/pub_analyzer/internal/__init__.py
+-rw-r--r--   0        0        0     2939 2024-01-25 21:20:17.706390 pub_analyzer-0.3.0/pub_analyzer/internal/identifier.py
+-rw-r--r--   0        0        0     2144 2024-01-11 01:51:43.020088 pub_analyzer-0.3.0/pub_analyzer/internal/render.py
+-rw-r--r--   0        0        0    16320 2024-04-30 05:41:03.010803 pub_analyzer-0.3.0/pub_analyzer/internal/report.py
+-rw-r--r--   0        0        0     2478 2024-04-30 04:54:12.008066 pub_analyzer-0.3.0/pub_analyzer/internal/templates/author/author_summary.typ
+-rw-r--r--   0        0        0     1444 2024-04-30 04:57:16.559322 pub_analyzer-0.3.0/pub_analyzer/internal/templates/author/report.typ
+-rw-r--r--   0        0        0      814 2024-01-29 01:00:53.427275 pub_analyzer-0.3.0/pub_analyzer/internal/templates/author/sources.typ
+-rw-r--r--   0        0        0     1980 2024-01-11 01:51:43.020553 pub_analyzer-0.3.0/pub_analyzer/internal/templates/author/works.typ
+-rw-r--r--   0        0        0     3527 2024-01-29 00:58:51.880732 pub_analyzer-0.3.0/pub_analyzer/internal/templates/author/works_extended.typ
+-rw-r--r--   0        0        0     2201 2024-01-18 00:40:08.587286 pub_analyzer-0.3.0/pub_analyzer/main.py
+-rw-r--r--   0        0        0       59 2023-10-06 05:46:06.896463 pub_analyzer-0.3.0/pub_analyzer/models/__init__.py
+-rw-r--r--   0        0        0     1900 2024-04-30 04:29:31.079326 pub_analyzer-0.3.0/pub_analyzer/models/author.py
+-rw-r--r--   0        0        0      677 2023-12-31 23:47:20.257076 pub_analyzer-0.3.0/pub_analyzer/models/concept.py
+-rw-r--r--   0        0        0     3067 2024-01-02 03:49:26.000414 pub_analyzer-0.3.0/pub_analyzer/models/institution.py
+-rw-r--r--   0        0        0     2574 2024-01-25 04:36:57.248463 pub_analyzer-0.3.0/pub_analyzer/models/report.py
+-rw-r--r--   0        0        0     2730 2024-04-30 03:54:35.174796 pub_analyzer-0.3.0/pub_analyzer/models/source.py
+-rw-r--r--   0        0        0     1825 2024-04-30 03:54:35.175094 pub_analyzer-0.3.0/pub_analyzer/models/topic.py
+-rw-r--r--   0        0        0     4115 2024-04-30 04:45:23.457064 pub_analyzer-0.3.0/pub_analyzer/models/work.py
+-rw-r--r--   0        0        0       18 2023-10-06 05:46:06.897980 pub_analyzer-0.3.0/pub_analyzer/widgets/__init__.py
+-rw-r--r--   0        0        0       22 2023-10-06 05:46:06.898262 pub_analyzer-0.3.0/pub_analyzer/widgets/author/__init__.py
+-rw-r--r--   0        0        0     2445 2024-04-30 04:33:33.124054 pub_analyzer-0.3.0/pub_analyzer/widgets/author/cards.py
+-rw-r--r--   0        0        0     5069 2024-01-10 22:19:54.718672 pub_analyzer-0.3.0/pub_analyzer/widgets/author/core.py
+-rw-r--r--   0        0        0      793 2023-10-30 19:25:59.901942 pub_analyzer-0.3.0/pub_analyzer/widgets/author/tables.py
+-rw-r--r--   0        0        0      972 2023-10-06 05:46:06.899226 pub_analyzer-0.3.0/pub_analyzer/widgets/body.py
+-rw-r--r--   0        0        0      287 2023-10-30 19:25:59.902231 pub_analyzer-0.3.0/pub_analyzer/widgets/common/__init__.py
+-rw-r--r--   0        0        0      595 2023-10-06 05:46:06.899886 pub_analyzer-0.3.0/pub_analyzer/widgets/common/card.py
+-rw-r--r--   0        0        0     6460 2023-10-30 19:25:59.902550 pub_analyzer-0.3.0/pub_analyzer/widgets/common/filesystem.py
+-rw-r--r--   0        0        0     3373 2023-10-30 19:25:59.902729 pub_analyzer-0.3.0/pub_analyzer/widgets/common/filters.py
+-rw-r--r--   0        0        0     2649 2023-10-31 22:04:33.176888 pub_analyzer-0.3.0/pub_analyzer/widgets/common/input.py
+-rw-r--r--   0        0        0      882 2023-10-06 05:46:06.900441 pub_analyzer-0.3.0/pub_analyzer/widgets/common/modal.py
+-rw-r--r--   0        0        0     1493 2023-10-30 19:25:59.903205 pub_analyzer-0.3.0/pub_analyzer/widgets/common/selector.py
+-rw-r--r--   0        0        0      165 2024-01-10 22:16:52.121514 pub_analyzer-0.3.0/pub_analyzer/widgets/common/summary.py
+-rw-r--r--   0        0        0       27 2023-10-06 05:46:06.900858 pub_analyzer-0.3.0/pub_analyzer/widgets/institution/__init__.py
+-rw-r--r--   0        0        0     2862 2023-10-30 19:25:59.903531 pub_analyzer-0.3.0/pub_analyzer/widgets/institution/cards.py
+-rw-r--r--   0        0        0     5332 2024-01-10 22:19:51.039328 pub_analyzer-0.3.0/pub_analyzer/widgets/institution/core.py
+-rw-r--r--   0        0        0      838 2023-10-30 19:25:59.904121 pub_analyzer-0.3.0/pub_analyzer/widgets/institution/tables.py
+-rw-r--r--   0        0        0       54 2023-10-06 05:46:06.901867 pub_analyzer-0.3.0/pub_analyzer/widgets/report/__init__.py
+-rw-r--r--   0        0        0     1227 2023-10-06 05:46:06.902096 pub_analyzer-0.3.0/pub_analyzer/widgets/report/author.py
+-rw-r--r--   0        0        0     4826 2024-01-10 22:34:27.173038 pub_analyzer-0.3.0/pub_analyzer/widgets/report/cards.py
+-rw-r--r--   0        0        0     1485 2024-01-10 23:19:36.355230 pub_analyzer-0.3.0/pub_analyzer/widgets/report/concept.py
+-rw-r--r--   0        0        0    11436 2023-12-24 21:47:47.234203 pub_analyzer-0.3.0/pub_analyzer/widgets/report/core.py
+-rw-r--r--   0        0        0     4762 2024-01-11 01:51:43.021988 pub_analyzer-0.3.0/pub_analyzer/widgets/report/export.py
+-rw-r--r--   0        0        0     1347 2024-01-03 02:14:44.323528 pub_analyzer-0.3.0/pub_analyzer/widgets/report/grants.py
+-rw-r--r--   0        0        0     1297 2023-10-06 05:46:06.903059 pub_analyzer-0.3.0/pub_analyzer/widgets/report/institution.py
+-rw-r--r--   0        0        0     2892 2023-10-30 19:25:59.905352 pub_analyzer-0.3.0/pub_analyzer/widgets/report/locations.py
+-rw-r--r--   0        0        0     3045 2024-01-25 21:26:12.536612 pub_analyzer-0.3.0/pub_analyzer/widgets/report/source.py
+-rw-r--r--   0        0        0     1969 2024-04-30 03:54:35.176820 pub_analyzer-0.3.0/pub_analyzer/widgets/report/topic.py
+-rw-r--r--   0        0        0     9590 2024-04-30 03:54:35.178115 pub_analyzer-0.3.0/pub_analyzer/widgets/report/work.py
+-rw-r--r--   0        0        0      239 2023-10-30 19:25:59.906252 pub_analyzer-0.3.0/pub_analyzer/widgets/search/__init__.py
+-rw-r--r--   0        0        0     3861 2024-04-30 04:13:10.715020 pub_analyzer-0.3.0/pub_analyzer/widgets/search/core.py
+-rw-r--r--   0        0        0     3702 2024-01-10 22:19:49.617260 pub_analyzer-0.3.0/pub_analyzer/widgets/search/results.py
+-rw-r--r--   0        0        0     2704 2024-03-25 20:30:55.069531 pub_analyzer-0.3.0/pub_analyzer/widgets/sidebar.py
+-rw-r--r--   0        0        0     3011 2024-04-30 06:01:45.220179 pub_analyzer-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4508 1970-01-01 00:00:00.000000 pub_analyzer-0.3.0/PKG-INFO
```

### Comparing `pub_analyzer-0.2.0/LICENSE` & `pub_analyzer-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pub_analyzer-0.2.0/README.md` & `pub_analyzer-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Pub Analyzer
 
 <p align="center">
-    <img src="docs/assets/img/logo.png" alt="PubAnalyzer" width="275">
+    <img src="https://raw.githubusercontent.com/alejandrgaspar/pub-analyzer/main/docs/assets/img/logo.png" alt="PubAnalyzer splash image" width="275">
 </p>
 
 <p align="center">
     <a href="https://github.com/alejandrgaspar/pub-analyzer/actions/workflows/python-test.yml" target="_blank">
         <img src="https://github.com/alejandrgaspar/pub-analyzer/actions/workflows/python-test.yml/badge.svg?branch=main" alt="Test status">
     </a>
     <a href="https://pypi.org/project/pub-analyzer/" target="_blank">
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # Pub Analyzer
-                                 [PubAnalyzer]
+                          [PubAnalyzer splash image]
        _[_T_e_s_t_ _s_t_a_t_u_s_]_[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_ _M_I_T_]
  Pub-Analyzer —_PP_uu_bb_ll_ii_cc_aa_tt_ii_oo_nn_ _AA_nn_aa_ll_yy_zz_ee_rr— is a Text User Interface —TTUUII— written in
  Python, which automates the generation of scientific production reports using
                                    _OO_pp_ee_nn_AA_ll_ee_xx.
 --- ## What is Pub Analyzer for? Pub Analyzer is a tool designed to retrieve,
 process and present in a concise and understandable way the scientific
 production of a researcher, including detailed information about their
```

### Comparing `pub_analyzer-0.2.0/pub_analyzer/css/author.tcss` & `pub_analyzer-0.3.0/pub_analyzer/css/search.tcss`

 * *Files 23% similar despite different names*

```diff
@@ -4,79 +4,78 @@
 $bg-secondary-color-accent: #d1d5db;
 $text-primary-color: black;
 
 $bg-main-color-darken: #1e293b;
 $bg-secondary-color-darken: #0f172a;
 $text-primary-color-darken: black;
 
-AuthorResumeWidget {
+/* Finder */
+FinderWidget {
     height: 1fr;
-    margin: 1 2;
 }
 
-.-dark-mode AuthorResumeWidget {
-    color: $text-primary-color-darken;
-    background: $bg-secondary-color;
+FinderWidget #results-container {
+    overflow: auto;
+    margin: 1 2;
 }
 
-/* Main Container */
-AuthorResumeWidget #main-container{
-    height: 1fr;
+/* Searchbar */
+FinderWidget .searchbar-container {
+    height: 4;
 }
 
-/* Block Container */
-AuthorResumeWidget .block-container {
-    padding: 1;
-    height: auto;
+SearchBar {
+    width: 3fr;
+    height: 3;
+    padding: 0 1;
+    margin: 1 1 0 1;
 }
 
-AuthorResumeWidget .block-title {
-    text-align: center;
-    width: 100%;
-    border-bottom: solid $text-primary-color;
+EntityTypeSelector {
+    width: 1fr;
+    margin-top: 1;
 }
 
-/* Info Container */
-AuthorResumeWidget .info-container {
-    height: auto;
+/* Result Widget */
+ResultWidget {
+    height: 9;
+    layout: horizontal;
+    border: $text-primary-color wide;
+    margin: 1 0;
+    background: $bg-secondary-color;
 }
 
-AuthorResumeWidget .info-container Label {
-    text-align: center;
-    width: 1fr;
+.-dark-mode ResultWidget {
+    color: $text-primary-color-darken;
 }
 
-/* Filter Container */
-AuthorResumeWidget CollapsibleTitle {
-    padding: 0;
+ResultWidget Button {
+    height: 100%;
+    width: 1fr;
+    text-align: center;
+    border: $text-primary-color solid;
+    padding: 0 1;
 }
 
-AuthorResumeWidget .filter-collapsible {
-    margin-top: 1;
+.-dark-mode ResultWidget Button {
+    background: $bg-secondary-color;
 }
 
-AuthorResumeWidget .filter-collapsible DateRangeFilter {
-    margin-top: 1;
+ResultWidget .vertical-content {
+    height: 100%;
+    width: 4fr;
+    border: black solid;
+    padding: 0 1;
 }
 
-/* Cards */
-AuthorResumeWidget .cards-container {
+ResultWidget .main-info-container {
     height: auto;
-    margin: 1 0 0 0 ;
-
-    layout: grid;
-    grid-size: 3 1;
-    grid-rows: 11;
-    grid-columns: 1fr;
-    grid-gutter: 1 2;
+    margin-bottom: 1;
 }
 
-/* Table */
-AuthorResumeWidget .table-container {
-    height: auto;
-    margin: 1 0 0 0;
+ResultWidget .main-info-container Static {
+    width: 1fr;
 }
 
-/* Buttons */
-AuthorResumeWidget .button-container {
-    align: center middle;
+ResultWidget .text-hint {
+    max-height: 3;
 }
```

### Comparing `pub_analyzer-0.2.0/pub_analyzer/css/body.tcss` & `pub_analyzer-0.3.0/pub_analyzer/css/body.tcss`

 * *Files 16% similar despite different names*

```diff
@@ -10,65 +10,78 @@
 /* SideBar CSS */
 SideBar {
     dock: left;
     width: 20;
 
     background: $bg-secondary-color;
     color: $text-primary-color;
-    transition: width 250ms in_out_cubic;
+
+    Button {
+        text-align: start;
+    }
+
+    #sidebar-title {
+        width: 100%;
+        content-align: left middle;
+        text-style: bold;
+        border-bottom: heavy $text-primary-color;
+    }
+
+    .sidebar-options-column {
+        margin: 1;
+        padding: 1 1;
+    }
+
+    .sidebar-buttons-column {
+        height: 1fr;
+
+        .sidebar-option {
+            content-align: left middle;
+            margin: 1 0;
+            width: 100%;
+        }
+    }
+
+    #module-version-label {
+        color: $text-primary-color 25%;
+        text-align: center;
+        width: 100%;
+    }
 }
 
 .-dark-mode SideBar {
     background: $bg-secondary-color-darken;
     color: $text-primary-color-darken;
-}
-
-SideBar.-hidden {
-    width: 0;
-}
-
-SideBar .sidebar-options-column {
-    margin: 1;
-    padding: 1 1;
-}
-
-SideBar #sidebar-title {
-    width: 100%;
-    content-align: left middle;
-    text-style: bold;
-    border-bottom: heavy $text-primary-color;
-}
-
-.-dark-mode SideBar #sidebar-title {
-    border-bottom: heavy $text-primary-color-darken;
-}
 
-SideBar .sidebar-option {
-    content-align: left middle;
-    margin: 1 0;
-    width: 100%;
+    #sidebar-title {
+        border-bottom: heavy $text-primary-color-darken;
+    }
+
+    #module-version-label {
+        color: $text-primary-color-darken 25%;
+    }
 }
 
 /* Main Content CSS */
 MainContent {
     background: $bg-main-color;
     color: $text-primary-color;
 
     padding: 2 1 0 1;
     height: 100%;
+
+    .title {
+        content-align: left middle;
+        text-style: bold;
+        border-bottom: heavy $text-primary-color;
+        width: 100%
+    }
 }
 
 .-dark-mode MainContent {
     background: $bg-main-color-darken;
     color: $text-primary-color-darken;
-}
-
-MainContent .title {
-    content-align: left middle;
-    text-style: bold;
-    border-bottom: heavy $text-primary-color;
-    width: 100%
-}
 
-.-dark-mode MainContent .title {
-    border-bottom: heavy $text-primary-color-darken;
+    .title {
+        border-bottom: heavy $text-primary-color-darken;
+    }
 }
```

### Comparing `pub_analyzer-0.2.0/pub_analyzer/css/buttons.tcss` & `pub_analyzer-0.3.0/pub_analyzer/css/buttons.tcss`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 /* COLORS */
 $primary-color: #b91c1c;
 $primary-color-accent: #991b1b;
 $primary-color-highlight: #dc2626;
 
-Button {
-    text-align: start;
-}
-
 /* Primary variant */
 Button.-primary {
     background: $primary-color;
     color: white;
     border-top: tall $primary-color-highlight;
     border-bottom: tall black;
 }
```

### Comparing `pub_analyzer-0.2.0/pub_analyzer/css/collapsible.tcss` & `pub_analyzer-0.3.0/pub_analyzer/css/collapsible.tcss`

 * *Files identical despite different names*

### Comparing `pub_analyzer-0.2.0/pub_analyzer/css/datatable.tcss` & `pub_analyzer-0.3.0/pub_analyzer/css/datatable.tcss`

 * *Files identical despite different names*

### Comparing `pub_analyzer-0.2.0/pub_analyzer/css/main.tcss` & `pub_analyzer-0.3.0/pub_analyzer/css/main.tcss`

 * *Files 13% similar despite different names*

```diff
@@ -35,10 +35,10 @@
     background: $primary-color-accent
 }
 
 LoadingIndicator {
     color: $primary-color-accent;
 }
 
-LoadingIndicator.-overlay {
+LoadingIndicator.-textual-loading-indicator {
     background: transparent;
 }
```

### Comparing `pub_analyzer-0.2.0/pub_analyzer/css/report.tcss` & `pub_analyzer-0.3.0/pub_analyzer/css/report.tcss`

 * *Files identical despite different names*

### Comparing `pub_analyzer-0.2.0/pub_analyzer/css/tree.tcss` & `pub_analyzer-0.3.0/pub_analyzer/css/tree.tcss`

 * *Files identical despite different names*

### Comparing `pub_analyzer-0.2.0/pub_analyzer/internal/identifier.py` & `pub_analyzer-0.3.0/pub_analyzer/internal/identifier.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Functions to extract OpenAlex IDs from Models."""
 
 from pub_analyzer.models.author import Author, AuthorOpenAlexKey, AuthorResult, DehydratedAuthor
 from pub_analyzer.models.institution import DehydratedInstitution, Institution, InstitutionOpenAlexKey, InstitutionResult
+from pub_analyzer.models.source import DehydratedSource, Source
 from pub_analyzer.models.work import Work
 
 
 def get_author_id(author: Author | AuthorResult | DehydratedAuthor) -> AuthorOpenAlexKey:
     """Extract OpenAlex ID from author Model.
 
     Args:
@@ -74,7 +75,32 @@
         # 'W000000000'
         ```
     """
     if work.id.path:
         return work.id.path.rpartition("/")[2]
     else:
         return ""
+
+
+def get_source_id(source: DehydratedSource | Source) -> str:
+    """Extract OpenAlex ID from Source Model.
+
+    Args:
+        source: Source model instance.
+
+    Returns:
+        Source OpenAlex ID.
+
+    Example:
+        ```python
+        from pub_analyzer.internal.identifier import get_source_id
+        from pub_analyzer.models.source import Source
+
+        source = Source(id="https://openalex.org/S000000000", **kwargs)
+        print(get_source_id(source))
+        # 'S000000000'
+        ```
+    """
+    if source.id.path:
+        return source.id.path.rpartition("/")[2]
+    else:
+        return ""
```

### Comparing `pub_analyzer-0.2.0/pub_analyzer/internal/render.py` & `pub_analyzer-0.3.0/pub_analyzer/internal/render.py`

 * *Files identical despite different names*

### Comparing `pub_analyzer-0.2.0/pub_analyzer/internal/report.py` & `pub_analyzer-0.3.0/pub_analyzer/internal/report.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,22 +9,23 @@
 
 from pub_analyzer.internal import identifier
 from pub_analyzer.models.author import Author, AuthorOpenAlexKey, AuthorResult, DehydratedAuthor
 from pub_analyzer.models.institution import DehydratedInstitution, Institution, InstitutionOpenAlexKey, InstitutionResult
 from pub_analyzer.models.report import (
     AuthorReport,
     CitationReport,
-    CitationResume,
+    CitationSummary,
     CitationType,
     InstitutionReport,
-    OpenAccessResume,
-    SourcesResume,
+    OpenAccessSummary,
+    SourcesSummary,
     WorkReport,
     WorkTypeCounter,
 )
+from pub_analyzer.models.source import DehydratedSource, Source
 from pub_analyzer.models.work import Authorship, Work
 
 FromDate = NewType("FromDate", datetime.datetime)
 """DateTime marker for works published from this date."""
 
 ToDate = NewType("ToDate", datetime.datetime)
 """DateTime marker for works published up to this date."""
@@ -167,14 +168,33 @@
     for page_number in range(1, page_count):
         page_result = (await client.get(url + f"&page={page_number + 1}")).json()
         works_data.extend(_get_valid_works(page_result["results"]))
 
     return TypeAdapter(list[Work]).validate_python(works_data)
 
 
+async def _get_source(client: httpx.AsyncClient, url: str) -> Source:
+    """Get source given a URL.
+
+    Args:
+        client: HTTPX asynchronous client to be used to make the requests.
+        url: URL of works with all filters.
+
+    Returns:
+        Source Model.
+
+    Raises:
+        httpx.HTTPStatusError: One response from OpenAlex API had an error HTTP status of 4xx or 5xx.
+    """
+    response = await client.get(url=url)
+    response.raise_for_status()
+
+    return Source(**response.json())
+
+
 async def make_author_report(
     author: Author,
     extra_profiles: list[Author | AuthorResult | DehydratedAuthor] | None = None,
     pub_from_date: FromDate | None = None,
     pub_to_date: ToDate | None = None,
     cited_from_date: FromDate | None = None,
     cited_to_date: ToDate | None = None,
@@ -212,64 +232,75 @@
 
         # Extra filters
         cited_from_filter = f",from_publication_date:{cited_from_date:%Y-%m-%d}" if cited_from_date else ""
         cited_to_filter = f",to_publication_date:{cited_to_date:%Y-%m-%d}" if cited_to_date else ""
 
         # Report fields.
         works: list[WorkReport] = []
-        report_citation_resume = CitationResume()
-        open_access_resume = OpenAccessResume()
+        report_citation_summary = CitationSummary()
+        open_access_summary = OpenAccessSummary()
         works_type_counter: list[WorkTypeCounter] = []
-        sources_resume = SourcesResume(sources=[])
+        dehydrated_sources: list[DehydratedSource] = []
 
         # Getting all works that have cited the author.
         for author_work in author_works:
             work_id = identifier.get_work_id(author_work)
             work_authors = _get_authors_list(authorships=author_work.authorships)
             cited_by_api_url = (
                 f"https://api.openalex.org/works?filter=cites:{work_id}{cited_from_filter}{cited_to_filter}&sort=publication_date"
             )
 
             # Adding the type of OpenAccess in the counter.
-            open_access_resume.add_oa_type(author_work.open_access.oa_status)
+            open_access_summary.add_oa_type(author_work.open_access.oa_status)
 
             # Adding the work type to works type counter.
             work_type = next((work_type for work_type in works_type_counter if work_type.type_name == author_work.type), None)
             if work_type:
                 work_type.count += 1
             else:
                 works_type_counter.append(WorkTypeCounter(type_name=author_work.type, count=1))
 
             # Add Sources to global list.
             for location in author_work.locations:
-                if location.source and not any(source.display_name == location.source.display_name for source in sources_resume.sources):
-                    sources_resume.sources.append(location.source)
+                if location.source and not any(source.id == location.source.id for source in dehydrated_sources):
+                    dehydrated_sources.append(location.source)
 
             cited_by_works = await _get_works(client, cited_by_api_url)
             cited_by: list[CitationReport] = []
-            work_citation_resume = CitationResume()
+            work_citation_summary = CitationSummary()
             for cited_by_work in cited_by_works:
                 cited_authors = _get_authors_list(authorships=cited_by_work.authorships)
                 citation_type = _get_citation_type(work_authors, cited_authors)
 
                 # Adding the type of cites in the counters.
-                report_citation_resume.add_cite_type(citation_type)
-                work_citation_resume.add_cite_type(citation_type)
+                report_citation_summary.add_cite_type(citation_type)
+                work_citation_summary.add_cite_type(citation_type)
 
                 cited_by.append(CitationReport(work=cited_by_work, citation_type=citation_type))
 
-            works.append(WorkReport(work=author_work, cited_by=cited_by, citation_resume=work_citation_resume))
+            works.append(WorkReport(work=author_work, cited_by=cited_by, citation_summary=work_citation_summary))
+
+        # Get sources full info.
+        sources: list[Source] = []
+        for dehydrated_source in dehydrated_sources:
+            source_id = identifier.get_source_id(dehydrated_source)
+            source_url = f"https://api.openalex.org/sources/{source_id}"
+            sources.append(await _get_source(client, source_url))
+
+        # Sort sources by h_index
+        sources_sorted = sorted(sources, key=lambda source: source.summary_stats.two_yr_mean_citedness, reverse=True)
+        sources_summary = SourcesSummary(sources=sources_sorted)
 
     return AuthorReport(
         author=author,
         works=works,
-        citation_resume=report_citation_resume,
-        open_access_resume=open_access_resume,
-        works_type_resume=works_type_counter,
-        sources_resume=sources_resume,
+        citation_summary=report_citation_summary,
+        open_access_summary=open_access_summary,
+        works_type_summary=works_type_counter,
+        sources_summary=sources_summary,
     )
 
 
 async def make_institution_report(
     institution: Institution,
     extra_profiles: list[Institution | InstitutionResult | DehydratedInstitution] | None = None,
     pub_from_date: FromDate | None = None,
@@ -308,58 +339,69 @@
 
         # Extra filters
         cited_from_filter = f",from_publication_date:{cited_from_date:%Y-%m-%d}" if cited_from_date else ""
         cited_to_filter = f",to_publication_date:{cited_to_date:%Y-%m-%d}" if cited_to_date else ""
 
         # Report fields.
         works: list[WorkReport] = []
-        report_citation_resume = CitationResume()
-        open_access_resume = OpenAccessResume()
+        report_citation_summary = CitationSummary()
+        open_access_summary = OpenAccessSummary()
         works_type_counter: list[WorkTypeCounter] = []
-        sources_resume = SourcesResume(sources=[])
+        dehydrated_sources: list[DehydratedSource] = []
 
         # Getting all works that have cited a work.
         for institution_work in institution_works:
             work_id = identifier.get_work_id(institution_work)
             work_authors = _get_authors_list(authorships=institution_work.authorships)
             cited_by_api_url = (
                 f"https://api.openalex.org/works?filter=cites:{work_id}{cited_from_filter}{cited_to_filter}&sort=publication_date"
             )
 
             # Adding the type of OpenAccess in the counter.
-            open_access_resume.add_oa_type(institution_work.open_access.oa_status)
+            open_access_summary.add_oa_type(institution_work.open_access.oa_status)
 
             # Adding the work type to works type counter.
             work_type = next((work_type for work_type in works_type_counter if work_type.type_name == institution_work.type), None)
             if work_type:
                 work_type.count += 1
             else:
                 works_type_counter.append(WorkTypeCounter(type_name=institution_work.type, count=1))
 
             # Add Sources to global list.
             for location in institution_work.locations:
-                if location.source and not any(source.display_name == location.source.display_name for source in sources_resume.sources):
-                    sources_resume.sources.append(location.source)
+                if location.source and not any(source.id == location.source.id for source in dehydrated_sources):
+                    dehydrated_sources.append(location.source)
 
             cited_by_works = await _get_works(client, cited_by_api_url)
             cited_by: list[CitationReport] = []
-            work_citation_resume = CitationResume()
+            work_citation_summary = CitationSummary()
             for cited_by_work in cited_by_works:
                 cited_authors = _get_authors_list(authorships=cited_by_work.authorships)
                 citation_type = _get_citation_type(work_authors, cited_authors)
 
                 # Adding the type of cites in the counters.
-                report_citation_resume.add_cite_type(citation_type)
-                work_citation_resume.add_cite_type(citation_type)
+                report_citation_summary.add_cite_type(citation_type)
+                work_citation_summary.add_cite_type(citation_type)
 
                 cited_by.append(CitationReport(work=cited_by_work, citation_type=citation_type))
 
-            works.append(WorkReport(work=institution_work, cited_by=cited_by, citation_resume=work_citation_resume))
+            works.append(WorkReport(work=institution_work, cited_by=cited_by, citation_summary=work_citation_summary))
+
+        # Get sources full info.
+        sources: list[Source] = []
+        for dehydrated_source in dehydrated_sources:
+            source_id = identifier.get_source_id(dehydrated_source)
+            source_url = f"https://api.openalex.org/sources/{source_id}"
+            sources.append(await _get_source(client, source_url))
+
+        # Sort sources by h_index
+        sources_sorted = sorted(sources, key=lambda source: source.summary_stats.two_yr_mean_citedness, reverse=True)
+        sources_summary = SourcesSummary(sources=sources_sorted)
 
     return InstitutionReport(
         institution=institution,
         works=works,
-        citation_resume=report_citation_resume,
-        open_access_resume=open_access_resume,
-        works_type_resume=works_type_counter,
-        sources_resume=sources_resume,
+        citation_summary=report_citation_summary,
+        open_access_summary=open_access_summary,
+        works_type_summary=works_type_counter,
+        sources_summary=sources_summary,
     )
```

### Comparing `pub_analyzer-0.2.0/pub_analyzer/internal/templates/author/author_resume.typ` & `pub_analyzer-0.3.0/pub_analyzer/internal/templates/author/author_summary.typ`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Author Resume
+// Author Summary
 = Author.
 
 // Cards
 #grid(
   columns: (1fr, 1fr, 1fr),
   column-gutter: 15pt,
   [
@@ -18,16 +18,17 @@
         columns: 1fr,
         row-gutter: (15pt, 12pt),
 
         // Card Title
         [#align(center)[#text(size: 12pt)[Last institution:]]],
 
         // Card content
-        {% if report.author.last_known_institution %}
-        [#align(left)[#text(size: 10pt)[- *Name:* {{ report.author.last_known_institution.display_name }}]]],
+        {% if report.author.last_known_institutions%}
+        {% set last_known_institution = report.author.last_known_institutions[0] %}
+        [#align(left)[#text(size: 10pt)[- *Name:* {{ last_known_institution.display_name }}]]],
         [#align(left)[#text(size: 10pt)[- *Country:* MX]]],
         [#align(left)[#text(size: 10pt)[- *Type:* education]]],
         {% endif %}
       )]
     )
   ],
   [
```

### Comparing `pub_analyzer-0.2.0/pub_analyzer/internal/templates/author/report.typ` & `pub_analyzer-0.3.0/pub_analyzer/internal/templates/author/report.typ`

 * *Files 18% similar despite different names*

```diff
@@ -35,20 +35,21 @@
 }
 
 // Title
 #grid(
   columns: (1fr),
   row-gutter: 11pt,
   [#align(center, text(size: 17pt, weight: "bold")[{{ report.author.display_name }}])],
-  {% if report.author.last_known_institution %}
-  [#align(center, text(size: 15pt, weight: "thin")[{{ report.author.last_known_institution.display_name }}])],
+  {% if report.author.last_known_institutions %}
+  {% set last_known_institution = report.author.last_known_institutions[0] %}
+  [#align(center, text(size: 15pt, weight: "thin")[{{ last_known_institution.display_name }}])],
   {% endif %}
 )
 
-{% include 'author_resume.typ' %}
+{% include 'author_summary.typ' %}
 
 {% include 'works.typ' %}
 
 {% include 'works_extended.typ' %}
 
 {% include 'sources.typ' %}
```

### Comparing `pub_analyzer-0.2.0/pub_analyzer/internal/templates/author/sources.typ` & `pub_analyzer-0.3.0/pub_analyzer/internal/templates/author/sources.typ`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 // Sources
 = Sources.
 
 #table(
-  columns: (auto, 3fr, 2fr, auto, auto, auto),
+  columns: (auto, 3fr, 2fr, auto, auto, auto, auto, auto),
   inset: 8pt,
   align: horizon,
   // Headers
-  [], [*Name*], [*Publisher or institution*], [*Type*], [*ISSN-L*], [*Is Open Access*],
+  [], [*Name*], [*Publisher or institution*], [*Type*], [*ISSN-L*], [*Impact factor*], [*h-index*], [*Is OA*],
 
   // Content
-  {% for source in report.sources_resume.sources %}
-  [{{ loop.index }}],
-  [#underline([#link("{{ source.id }}")[#"{{ source.display_name }}"]])],
+  {% for source in report.sources_summary.sources %}
+  [#underline[3.{{ loop.index }}. #label("source_{{ source.id.path.rpartition("/")[2] }}")]],
+  [#underline([#link("{{ source.homepage_url }}")[#"{{ source.display_name }}"]])],
   [{{ source.host_organization_name or "-" }}],
   [{{source.type }}],
   [{{ source.issn_l or "-" }}],
+  [{{ source.summary_stats.two_yr_mean_citedness|round(3) }}],
+  [{{ source.summary_stats.h_index }}],
   [{% if source.is_oa %}#text(rgb("909d63"))[True]{% else %}#text(rgb("bc5653"))[False]{% endif %}],
   {% endfor %}
 )
```

### Comparing `pub_analyzer-0.2.0/pub_analyzer/internal/templates/author/works.typ` & `pub_analyzer-0.3.0/pub_analyzer/internal/templates/author/works.typ`

 * *Files 8% similar despite different names*

```diff
@@ -5,39 +5,39 @@
 
 #grid(
   columns: (1fr, 1fr, 1fr),
   column-gutter: 30pt,
   [
     #align(center)[_Citation metrics_]
     #parbreak()
-    - *Count:* {{ report.citation_resume.type_a_count + report.citation_resume.type_b_count }}
-    - *Type A:* {{ report.citation_resume.type_a_count }}
-    - *Type B:* {{ report.citation_resume.type_b_count }}
+    - *Count:* {{ report.citation_summary.type_a_count + report.citation_summary.type_b_count }}
+    - *Type A:* {{ report.citation_summary.type_a_count }}
+    - *Type B:* {{ report.citation_summary.type_b_count }}
   ],
   [
     #align(center)[_Work Type_]
     #parbreak()
-    {% for work_type in report.works_type_resume %}
+    {% for work_type in report.works_type_summary %}
     - *{{ work_type.type_name }}:* {{ work_type.count }}
     {% endfor %}
   ],
   [
     #align(center)[_Open Access_]
     #parbreak()
     #grid(
       columns: (1fr, 1fr),
       column-gutter: 15pt,
       [
-        - *gold:* {{report.open_access_resume.gold}}
-        - *green:* {{report.open_access_resume.green}}
-        - *hybrid:* {{report.open_access_resume.hybrid}}
+        - *gold:* {{report.open_access_summary.gold}}
+        - *green:* {{report.open_access_summary.green}}
+        - *hybrid:* {{report.open_access_summary.hybrid}}
       ],
       [
-        - *bronze:* {{report.open_access_resume.bronze}}
-        - *closed:* {{report.open_access_resume.closed}}
+        - *bronze:* {{report.open_access_summary.bronze}}
+        - *closed:* {{report.open_access_summary.closed}}
       ],
     )
   ],
 )
 
 #linebreak()
 
@@ -52,14 +52,14 @@
   // Content
   {% for work in report.works %}
   [#underline([#link(label("work_{{ loop.index }}"))[@work_{{ loop.index }}]])],
   [#"{{ work.work.title.replace('"', '\\"') }}"],
   [{{ work.work.type }}],
   [{% if work.work.ids.doi %}#underline([#link("{{ work.work.ids.doi }}")[DOI]]){% else %}-{% endif %}],
   [{{ work.work.publication_date }}],
-  [{{ work.citation_resume.type_a_count + work.citation_resume.type_b_count }}],
-  [{{ work.citation_resume.type_a_count }}],
-  [{{ work.citation_resume.type_b_count }}],
+  [{{ work.citation_summary.type_a_count + work.citation_summary.type_b_count }}],
+  [{{ work.citation_summary.type_a_count }}],
+  [{{ work.citation_summary.type_b_count }}],
   [{{ work.work.open_access.oa_status.value }}],
   {% endfor %}
 )
 #pagebreak()
```

### Comparing `pub_analyzer-0.2.0/pub_analyzer/internal/templates/author/works_extended.typ` & `pub_analyzer-0.3.0/pub_analyzer/internal/templates/author/works_extended.typ`

 * *Files 5% similar despite different names*

```diff
@@ -35,17 +35,17 @@
     #parbreak()
     - *Status:* {{ work.work.open_access.oa_status.value }}
     {% if work.work.open_access.oa_url %}- *URL:* #underline([#link("{{ work.work.open_access.oa_url }}")[{{ work.work.open_access.oa_url }}]]){% endif %}
   ],
   [
     #align(center)[_Citation_]
     #parbreak()
-    - *Count:* {{ work.citation_resume.type_a_count + work.citation_resume.type_b_count }}
-    - *Type A:* {{ work.citation_resume.type_a_count }}
-    - *Type B:* {{ work.citation_resume.type_b_count }}
+    - *Count:* {{ work.citation_summary.type_a_count + work.citation_summary.type_b_count }}
+    - *Type A:* {{ work.citation_summary.type_a_count }}
+    - *Type B:* {{ work.citation_summary.type_b_count }}
   ],
 )
 
 #linebreak()
 
 // Cited by Table
 {% if work.cited_by %}
@@ -79,15 +79,15 @@
   align: horizon,
   // Headers
   [], [*Name*], [*Publisher or institution*], [*Type*], [*ISSN-L*], [*Is OA*], [*License*], [*Version*],
 
   // Content
   {% for location in work.work.locations %}
   {% if location.source %}
-  [{{ loop.index }}],
+  [#underline([#link(label("source_{{ location.source.id.path.rpartition("/")[2] }}"))[{{ loop.index }}]])],
   [#underline([#link("{{ location.landing_page_url }}")[#"{{ location.source.display_name }}"]])],
   [{{ location.source.host_organization_name or "-" }}],
   [{{ location.source.type }}],
   [{{ location.source.issn_l or "-" }}],
   [{% if location.is_oa %}#text(rgb("909d63"))[True]{% else %}#text(rgb("bc5653"))[False]{% endif %}],
   [{{ location.license or "-" }}],
   [{{ location.version.name or "-" }}],
```

### Comparing `pub_analyzer-0.2.0/pub_analyzer/main.py` & `pub_analyzer-0.3.0/pub_analyzer/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,24 +14,25 @@
 from pub_analyzer.widgets.body import Body
 from pub_analyzer.widgets.sidebar import SideBar
 
 
 class PubAnalyzerApp(App[DOMNode]):
     """Pub Analyzer App entrypoint."""
 
+    TITLE = "Pub Analyzer"
+
     CSS_PATH: ClassVar[CSSPathType | None] = [
-        "css/author.tcss",
         "css/body.tcss",
         "css/buttons.tcss",
         "css/checkbox.tcss",
         "css/collapsible.tcss",
         "css/datatable.tcss",
-        "css/institution.tcss",
         "css/main.tcss",
         "css/report.tcss",
+        "css/summary.tcss",
         "css/search.tcss",
         "css/tabs.tcss",
         "css/tree.tcss",
     ]
     BINDINGS: ClassVar[list[BindingType]] = [
         Binding(key="ctrl+d", action="toggle_dark", description="Dark mode"),
         Binding(key="ctrl+s", action="toggle_sidebar", description="Sidebar"),
```

### Comparing `pub_analyzer-0.2.0/pub_analyzer/models/author.py` & `pub_analyzer-0.3.0/pub_analyzer/models/author.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,30 @@
 """Authors models from OpenAlex API Schema definition."""
 
 from typing import TypeAlias
 
-from pydantic import BaseModel, ConfigDict, Field, HttpUrl, field_validator
+from pydantic import BaseModel, Field, HttpUrl
 
 from pub_analyzer.models.institution import DehydratedInstitution
 
 AuthorOpenAlexID: TypeAlias = HttpUrl
 """OpenAlex ID for Author Objects with the format `https://openalex.org/A000000000`"""
 
 AuthorOpenAlexKey: TypeAlias = str
 """OpenAlex author entity Key with the format `A000000000`"""
 
 
 class AuthorIDs(BaseModel):
     """IDs from an Author."""
 
-    openalex: str
-    orcid: str | None = ""
-    scopus: str | None = ""
-    twitter: str | None = ""
-    wikipedia: str | None = ""
-
-    # Allowing a value to be assigned during validation.
-    model_config = ConfigDict(validate_assignment=True)
-
-    @field_validator("scopus", "twitter", "wikipedia")
-    def set_default(cls, value: str) -> str:
-        """Define a default text."""
-        return value or ""
+    openalex: AuthorOpenAlexID
+    orcid: HttpUrl | None = None
+    scopus: HttpUrl | None = None
+    twitter: HttpUrl | None = None
+    wikipedia: HttpUrl | None = None
 
 
 class AuthorYearCount(BaseModel):
     """Summary of published papers and number of citations in a year."""
 
     year: int
     works_count: int
@@ -56,15 +48,15 @@
 
     display_name: str
     display_name_alternatives: list[str]
 
     works_count: int
     cited_by_count: int
 
-    last_known_institution: DehydratedInstitution | None
+    last_known_institutions: list[DehydratedInstitution]
     counts_by_year: list[AuthorYearCount]
 
     summary_stats: AuthorSummaryStats
 
     works_api_url: str
 
 
@@ -77,20 +69,12 @@
 
 
 class AuthorResult(BaseModel):
     """Author result Model resulting from a search in OpenAlex."""
 
     id: AuthorOpenAlexID
     display_name: str
-    hint: str | None = ""
+    hint: str | None = None
     cited_by_count: int
     works_count: int
     entity_type: str
-    external_id: str | None = ""
-
-    # Allowing a value to be assigned during validation.
-    model_config = ConfigDict(validate_assignment=True)
-
-    @field_validator("hint", "external_id")
-    def set_default(cls, value: str) -> str:
-        """Define a default text."""
-        return value or ""
+    external_id: str | None = None
```

### Comparing `pub_analyzer-0.2.0/pub_analyzer/models/institution.py` & `pub_analyzer-0.3.0/pub_analyzer/models/institution.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,29 +73,39 @@
     """Institution role."""
 
     role: InstitutionRoleType
     id: HttpUrl
     works_count: int
 
 
+class International(BaseModel):
+    """The institution's display name in different languages."""
+
+    display_name: dict[str, str]
+
+
 class Institution(BaseModel):
     """Universities and other organizations to which authors claim affiliations."""
 
     id: InstitutionOpenAlexID
     ids: InstitutionIDs
 
     display_name: str
     country_code: str
     type: InstitutionType
     homepage_url: HttpUrl | None = None
+    image_url: HttpUrl | None = None
+
+    display_name_acronyms: list[str]
+    international: International
 
     works_count: int
     cited_by_count: int
-    counts_by_year: list[InstitutionYearCount]
     summary_stats: InstitutionSummaryStats
+    counts_by_year: list[InstitutionYearCount]
 
     geo: InstitutionGeo
     roles: list[InstitutionRole]
 
     works_api_url: str
```

### Comparing `pub_analyzer-0.2.0/pub_analyzer/models/report.py` & `pub_analyzer-0.3.0/pub_analyzer/models/report.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from enum import Enum
 
 from pydantic import BaseModel
 
 from .author import Author
 from .institution import Institution
-from .source import DehydratedSource
+from .source import Source
 from .work import OpenAccessStatus, Work
 
 
 class CitationType(Enum):
     """Citation type Work."""
 
     TypeA = 0
@@ -20,29 +20,29 @@
 class CitationReport(BaseModel):
     """Cited by Works with stats."""
 
     work: Work
     citation_type: CitationType
 
 
-class CitationResume(BaseModel):
+class CitationSummary(BaseModel):
     """Summary of citation information in all works."""
 
     type_a_count: int = 0
     type_b_count: int = 0
 
     def add_cite_type(self, cite_type: CitationType) -> None:
         """Add the type of cite in the corresponding counter."""
         if cite_type.value == CitationType.TypeA.value:
             self.type_a_count += 1
         elif cite_type.value == CitationType.TypeB.value:
             self.type_b_count += 1
 
 
-class OpenAccessResume(BaseModel):
+class OpenAccessSummary(BaseModel):
     """Open Access Type counter."""
 
     gold: int = 0
     green: int = 0
     hybrid: int = 0
     bronze: int = 0
     closed: int = 0
@@ -71,38 +71,38 @@
 
 class WorkReport(BaseModel):
     """Work model with stats."""
 
     work: Work
     cited_by: list[CitationReport]
 
-    citation_resume: CitationResume
+    citation_summary: CitationSummary
 
 
-class SourcesResume(BaseModel):
+class SourcesSummary(BaseModel):
     """Sources model with stats."""
 
-    sources: list[DehydratedSource]
+    sources: list[Source]
 
 
 class AuthorReport(BaseModel):
     """Report of scientific production of an author."""
 
     author: Author
     works: list[WorkReport]
 
-    citation_resume: CitationResume
-    open_access_resume: OpenAccessResume
-    works_type_resume: list[WorkTypeCounter]
-    sources_resume: SourcesResume
+    citation_summary: CitationSummary
+    open_access_summary: OpenAccessSummary
+    works_type_summary: list[WorkTypeCounter]
+    sources_summary: SourcesSummary
 
 
 class InstitutionReport(BaseModel):
     """Scientific production report of the Institution."""
 
     institution: Institution
     works: list[WorkReport]
 
-    citation_resume: CitationResume
-    open_access_resume: OpenAccessResume
-    works_type_resume: list[WorkTypeCounter]
-    sources_resume: SourcesResume
+    citation_summary: CitationSummary
+    open_access_summary: OpenAccessSummary
+    works_type_summary: list[WorkTypeCounter]
+    sources_summary: SourcesSummary
```

### Comparing `pub_analyzer-0.2.0/pub_analyzer/models/work.py` & `pub_analyzer-0.3.0/pub_analyzer/models/work.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 from enum import Enum
 from typing import Any
 
 from pydantic import BaseModel, HttpUrl, field_validator
 
 from .author import DehydratedAuthor
+from .concept import DehydratedConcept
 from .source import DehydratedSource
+from .topic import DehydratedTopic
 
 
 class WorkIDs(BaseModel):
     """IDs from a Work."""
 
     openalex: HttpUrl
     doi: HttpUrl | None = None
@@ -68,14 +70,30 @@
 
     value: int
     currency: str
     provenance: str
     value_usd: int | None
 
 
+class Grant(BaseModel):
+    """Grant Model Object from OpenAlex API definition."""
+
+    funder: HttpUrl
+    funder_display_name: str
+    award_id: str | None = None
+
+
+class Keyword(BaseModel):
+    """Keyword extracted from the work's title and confidence score."""
+
+    id: HttpUrl
+    display_name: str
+    score: float
+
+
 class Work(BaseModel):
     """Work Model Object from OpenAlex API definition."""
 
     id: HttpUrl
     ids: WorkIDs
 
     title: str
@@ -93,14 +111,19 @@
     authorships: list[Authorship]
 
     cited_by_count: int
     """This number comes from the OpenAlex API, represents ALL citations to this work, and may not always be correct.
        To use a verified number that respects the applied filters use [WorkReport][pub_analyzer.models.report.WorkReport].
     """
 
+    grants: list[Grant]
+    keywords: list[Keyword]
+    concepts: list[DehydratedConcept]
+    topics: list[DehydratedTopic]
+
     referenced_works: list[HttpUrl]
     cited_by_api_url: HttpUrl
 
     apc_list: ArticleProcessingCharge | None = None
     """The price as listed by the journal's publisher."""
     apc_paid: ArticleProcessingCharge | None = None
     """APC actually paid by authors."""
```

### Comparing `pub_analyzer-0.2.0/pub_analyzer/widgets/author/cards.py` & `pub_analyzer-0.3.0/pub_analyzer/widgets/author/cards.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,15 +50,16 @@
         self.author = author
         super().__init__()
 
     def compose(self) -> ComposeResult:
         """Compose card."""
         yield Label("[italic]Last Institution:[/italic]", classes="card-title")
 
-        if self.author.last_known_institution:
-            ror = self.author.last_known_institution.ror
-            institution_name = self.author.last_known_institution.display_name
+        if self.author.last_known_institutions:
+            last_known_institution = self.author.last_known_institutions[0]
+            ror = last_known_institution.ror
+            institution_name = last_known_institution.display_name
 
             with Vertical(classes="card-container"):
                 yield Label(f"""[bold]Name:[/bold] [@click=app.open_link('{quote(str(ror))}')]{institution_name}[/]""")
-                yield Label(f"[bold]Country:[/bold] {self.author.last_known_institution.country_code}")
-                yield Label(f"[bold]Type:[/bold] {self.author.last_known_institution.type.value}")
+                yield Label(f"[bold]Country:[/bold] {last_known_institution.country_code}")
+                yield Label(f"[bold]Type:[/bold] {last_known_institution.type.value}")
```

### Comparing `pub_analyzer-0.2.0/pub_analyzer/widgets/author/core.py` & `pub_analyzer-0.3.0/pub_analyzer/widgets/author/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """Module with Widgets that allows to display the complete information of an Author using OpenAlex."""
 
 from typing import Any
 
 import httpx
 from textual import on
 from textual.app import ComposeResult
-from textual.containers import Container, Horizontal, Vertical, VerticalScroll
+from textual.containers import Container, Horizontal, Vertical
 from textual.widgets import Button, Collapsible, Label, Static
 
 from pub_analyzer.internal.identifier import get_author_id
 from pub_analyzer.models.author import Author, AuthorResult
 from pub_analyzer.widgets.common.filters import DateRangeFilter, Filter
+from pub_analyzer.widgets.common.summary import SummaryWidget
 from pub_analyzer.widgets.report.core import CreateAuthorReportWidget
 
 from .cards import CitationMetricsCard, IdentifiersCard, LastInstitutionCard
 from .tables import AuthorWorksByYearTable
 
 
-class _AuthorResumeWidget(Static):
-    """Author info resume."""
+class _AuthorSummaryWidget(Static):
+    """Author info summary."""
 
     def __init__(self, author: Author) -> None:
         self.author = author
         super().__init__()
 
     def compose(self) -> ComposeResult:
         """Compose author info."""
@@ -58,20 +59,20 @@
                 # Author publication Date Range
                 yield DateRangeFilter(checkbox_label="Publication date range:", id="author-date-range-filter")
 
                 # Cite Date Range
                 yield DateRangeFilter(checkbox_label="Cited date range:", id="cited-date-range-filter")
 
             # Button
-            with Vertical(classes="block-container button-container"):
+            with Vertical(classes="button-container"):
                 yield Button("Make Report", variant="primary", id="make-report-button")
 
 
-class AuthorResumeWidget(VerticalScroll):
-    """Author info resume container."""
+class AuthorSummaryWidget(SummaryWidget):
+    """Author info summary container."""
 
     def __init__(self, author_result: AuthorResult) -> None:
         self.author_result = author_result
         self.author: Author
         super().__init__()
 
     def on_mount(self) -> None:
@@ -87,25 +88,25 @@
         async with httpx.AsyncClient() as client:
             results = (await client.get(url)).json()
             self.author = Author(**results)
 
     async def load_data(self) -> None:
         """Query OpenAlex API and composing the widget."""
         await self._get_info()
-        await self.mount(_AuthorResumeWidget(author=self.author))
+        await self.mount(_AuthorSummaryWidget(author=self.author))
 
         self.loading = False
 
     @on(Filter.Changed)
     def filter_change(self) -> None:
         """Handle filter changes."""
-        filters = [filter for filter in self.query("_AuthorResumeWidget Filter").results(Filter) if not filter.filter_disabled]
+        filters = [filter for filter in self.query("_AuthorSummaryWidget Filter").results(Filter) if not filter.filter_disabled]
         all_filters_valid = all(filter.validation_state for filter in filters)
 
-        self.query_one("_AuthorResumeWidget #make-report-button", Button).disabled = not all_filters_valid
+        self.query_one("_AuthorSummaryWidget #make-report-button", Button).disabled = not all_filters_valid
 
     @on(Button.Pressed, "#make-report-button")
     async def make_report(self) -> None:
         """Make the author report."""
         filters: dict[str, Any] = {}
         pub_date_range = self.query_one("#author-date-range-filter", DateRangeFilter)
         cited_date_range = self.query_one("#cited-date-range-filter", DateRangeFilter)
@@ -114,8 +115,8 @@
             filters.update({"pub_from_date": pub_date_range.from_date, "pub_to_date": pub_date_range.to_date})
 
         if not cited_date_range.filter_disabled:
             filters.update({"cited_from_date": cited_date_range.from_date, "cited_to_date": cited_date_range.to_date})
 
         report_widget = CreateAuthorReportWidget(author=self.author, **filters)
         await self.app.query_one("MainContent").mount(report_widget)
-        await self.app.query_one("AuthorResumeWidget").remove()
+        await self.app.query_one("AuthorSummaryWidget").remove()
```

### Comparing `pub_analyzer-0.2.0/pub_analyzer/widgets/author/tables.py` & `pub_analyzer-0.3.0/pub_analyzer/widgets/author/tables.py`

 * *Files identical despite different names*

### Comparing `pub_analyzer-0.2.0/pub_analyzer/widgets/body.py` & `pub_analyzer-0.3.0/pub_analyzer/widgets/body.py`

 * *Files identical despite different names*

### Comparing `pub_analyzer-0.2.0/pub_analyzer/widgets/common/card.py` & `pub_analyzer-0.3.0/pub_analyzer/widgets/common/card.py`

 * *Files identical despite different names*

### Comparing `pub_analyzer-0.2.0/pub_analyzer/widgets/common/filesystem.py` & `pub_analyzer-0.3.0/pub_analyzer/widgets/common/filesystem.py`

 * *Files identical despite different names*

### Comparing `pub_analyzer-0.2.0/pub_analyzer/widgets/common/filters.py` & `pub_analyzer-0.3.0/pub_analyzer/widgets/common/filters.py`

 * *Files identical despite different names*

### Comparing `pub_analyzer-0.2.0/pub_analyzer/widgets/common/input.py` & `pub_analyzer-0.3.0/pub_analyzer/widgets/common/input.py`

 * *Files identical despite different names*

### Comparing `pub_analyzer-0.2.0/pub_analyzer/widgets/common/modal.py` & `pub_analyzer-0.3.0/pub_analyzer/widgets/common/modal.py`

 * *Files identical despite different names*

### Comparing `pub_analyzer-0.2.0/pub_analyzer/widgets/common/selector.py` & `pub_analyzer-0.3.0/pub_analyzer/widgets/common/selector.py`

 * *Files identical despite different names*

### Comparing `pub_analyzer-0.2.0/pub_analyzer/widgets/institution/cards.py` & `pub_analyzer-0.3.0/pub_analyzer/widgets/institution/cards.py`

 * *Files identical despite different names*

### Comparing `pub_analyzer-0.2.0/pub_analyzer/widgets/institution/core.py` & `pub_analyzer-0.3.0/pub_analyzer/widgets/institution/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """Module with Widgets that allows to display the complete information of Institution using OpenAlex."""
 
 from typing import Any
 
 import httpx
 from textual import on
 from textual.app import ComposeResult
-from textual.containers import Container, Horizontal, Vertical, VerticalScroll
+from textual.containers import Container, Horizontal, Vertical
 from textual.widgets import Button, Collapsible, Label, Static
 
 from pub_analyzer.internal.identifier import get_institution_id
 from pub_analyzer.models.institution import Institution, InstitutionResult
 from pub_analyzer.widgets.common.filters import DateRangeFilter, Filter
+from pub_analyzer.widgets.common.summary import SummaryWidget
 from pub_analyzer.widgets.report.core import CreateInstitutionReportWidget
 
 from .cards import CitationMetricsCard, IdentifiersCard, RolesCard
 from .tables import InstitutionWorksByYearTable
 
 
-class _InstitutionResumeWidget(Static):
-    """Institution info resume."""
+class _InstitutionSummaryWidget(Static):
+    """Institution info summary."""
 
     def __init__(self, institution: Institution) -> None:
         self.institution = institution
         super().__init__()
 
     def compose(self) -> ComposeResult:
         """Compose institution info."""
@@ -62,16 +63,16 @@
                 yield DateRangeFilter(checkbox_label="Cited date range:", id="cited-date-range-filter")
 
             # Button
             with Vertical(classes="block-container button-container"):
                 yield Button("Make Report", variant="primary", id="make-report-button")
 
 
-class InstitutionResumeWidget(VerticalScroll):
-    """Institution info resume container."""
+class InstitutionSummaryWidget(SummaryWidget):
+    """Institution info summary container."""
 
     def __init__(self, institution_result: InstitutionResult) -> None:
         self.institution_result = institution_result
         self.institution: Institution
         super().__init__()
 
     def on_mount(self) -> None:
@@ -87,25 +88,25 @@
         async with httpx.AsyncClient() as client:
             results = (await client.get(url)).json()
             self.institution = Institution(**results)
 
     async def load_data(self) -> None:
         """Query OpenAlex API and composing the widget."""
         await self._get_info()
-        await self.mount(_InstitutionResumeWidget(institution=self.institution))
+        await self.mount(_InstitutionSummaryWidget(institution=self.institution))
 
         self.loading = False
 
     @on(Filter.Changed)
     def filter_change(self) -> None:
         """Handle filter changes."""
-        filters = [filter for filter in self.query("_InstitutionResumeWidget Filter").results(Filter) if not filter.filter_disabled]
+        filters = [filter for filter in self.query("_InstitutionSummaryWidget Filter").results(Filter) if not filter.filter_disabled]
         all_filters_valid = all(filter.validation_state for filter in filters)
 
-        self.query_one("_InstitutionResumeWidget #make-report-button", Button).disabled = not all_filters_valid
+        self.query_one("_InstitutionSummaryWidget #make-report-button", Button).disabled = not all_filters_valid
 
     @on(Button.Pressed, "#make-report-button")
     async def make_report(self) -> None:
         """Make the author report."""
         filters: dict[str, Any] = {}
         pub_date_range = self.query_one("#institution-date-range-filter", DateRangeFilter)
         cited_date_range = self.query_one("#cited-date-range-filter", DateRangeFilter)
@@ -114,8 +115,8 @@
             filters.update({"pub_from_date": pub_date_range.from_date, "pub_to_date": pub_date_range.to_date})
 
         if not cited_date_range.filter_disabled:
             filters.update({"cited_from_date": cited_date_range.from_date, "cited_to_date": cited_date_range.to_date})
 
         report_widget = CreateInstitutionReportWidget(institution=self.institution, **filters)
         await self.app.query_one("MainContent").mount(report_widget)
-        await self.app.query_one("InstitutionResumeWidget").remove()
+        await self.app.query_one("InstitutionSummaryWidget").remove()
```

### Comparing `pub_analyzer-0.2.0/pub_analyzer/widgets/institution/tables.py` & `pub_analyzer-0.3.0/pub_analyzer/widgets/institution/tables.py`

 * *Files identical despite different names*

### Comparing `pub_analyzer-0.2.0/pub_analyzer/widgets/report/author.py` & `pub_analyzer-0.3.0/pub_analyzer/widgets/report/author.py`

 * *Files identical despite different names*

### Comparing `pub_analyzer-0.2.0/pub_analyzer/widgets/report/cards.py` & `pub_analyzer-0.3.0/pub_analyzer/widgets/report/cards.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,67 +7,66 @@
 from textual.widgets import Label
 
 from pub_analyzer.models.author import Author
 from pub_analyzer.models.report import AuthorReport, InstitutionReport, WorkReport
 from pub_analyzer.models.work import Work
 from pub_analyzer.widgets.common import Card
 
-# Works pane cards.
-
 
+# Works pane cards.
 class ReportCitationMetricsCard(Card):
     """Citation metrics for this report."""
 
     def __init__(self, report: AuthorReport | InstitutionReport) -> None:
         self.report = report
         super().__init__()
 
     def compose(self) -> ComposeResult:
         """Compose card."""
         yield Label("[italic]Citation metrics:[/italic]", classes="card-title")
 
         with Vertical(classes="card-container"):
-            type_a_count = self.report.citation_resume.type_a_count
-            type_b_count = self.report.citation_resume.type_b_count
+            type_a_count = self.report.citation_summary.type_a_count
+            type_b_count = self.report.citation_summary.type_b_count
             cited_by_count = type_a_count + type_b_count
 
             yield Label(f"[bold]Count:[/bold] {cited_by_count}")
             yield Label(f"[bold]Type A:[/bold] {type_a_count}")
             yield Label(f"[bold]Type B:[/bold] {type_b_count}")
 
 
-class WorksTypeResumeCard(Card):
-    """Works Type Counters Resume Card."""
+class WorksTypeSummaryCard(Card):
+    """Works Type Counters Summary Card."""
 
     def __init__(self, report: AuthorReport | InstitutionReport) -> None:
         self.report = report
         super().__init__()
 
     def compose(self) -> ComposeResult:
         """Compose card."""
         yield Label("[italic]Work Type[/italic]", classes="card-title")
 
         with VerticalScroll(classes="card-container"):
-            for work_type_counter in self.report.works_type_resume:
+            for work_type_counter in self.report.works_type_summary:
                 yield Label(f"[bold]{work_type_counter.type_name}:[/bold] {work_type_counter.count}")
 
 
-class OpenAccessResumeCard(Card):
+class OpenAccessSummaryCard(Card):
     """Open Access counts for this report."""
 
     def __init__(self, report: AuthorReport | InstitutionReport) -> None:
         self.report = report
         super().__init__()
 
     def compose(self) -> ComposeResult:
         """Compose card."""
         yield Label("[italic]Open Access[/italic]", classes="card-title")
 
         with VerticalScroll(classes="card-container"):
-            for status, count in self.report.open_access_resume.model_dump().items():
+            for status, count in self.report.open_access_summary.model_dump().items():
                 yield Label(f"[bold]{status}:[/bold] {count}")
 
 
 # Work Info cards.
 class AuthorshipCard(Card):
     """Card that enumerate the authorships of a work."""
 
@@ -116,16 +115,16 @@
 
     def __init__(self, work_report: WorkReport) -> None:
         self.work_report = work_report
         super().__init__()
 
     def compose(self) -> ComposeResult:
         """Compose card."""
-        type_a_count = self.work_report.citation_resume.type_a_count
-        type_b_count = self.work_report.citation_resume.type_b_count
+        type_a_count = self.work_report.citation_summary.type_a_count
+        type_b_count = self.work_report.citation_summary.type_b_count
         cited_by_count = type_a_count + type_b_count
 
         yield Label("[italic]Citation[/italic]", classes="card-title")
 
         yield Label(f"[bold]Count:[/bold] {cited_by_count}")
         yield Label(f"[bold]Type A:[/bold] {type_a_count}")
         yield Label(f"[bold]Type B:[/bold] {type_b_count}")
```

### Comparing `pub_analyzer-0.2.0/pub_analyzer/widgets/report/core.py` & `pub_analyzer-0.3.0/pub_analyzer/widgets/report/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """Main Report widgets."""
 
 import datetime
 import pathlib
 from enum import Enum
+from typing import ClassVar
 
 import httpx
 from pydantic import TypeAdapter, ValidationError
 from textual import on
 from textual.app import ComposeResult
+from textual.binding import Binding, BindingType
 from textual.containers import Container, Horizontal
+from textual.reactive import reactive
 from textual.widget import Widget
 from textual.widgets import Button, LoadingIndicator, Static, TabbedContent, TabPane
 
 from pub_analyzer.internal.report import FromDate, ToDate, make_author_report, make_institution_report
 from pub_analyzer.models.author import Author
 from pub_analyzer.models.institution import Institution
 from pub_analyzer.models.report import AuthorReport, InstitutionReport
@@ -24,14 +27,25 @@
 from .source import SourcesReportPane
 from .work import WorkReportPane
 
 
 class ReportWidget(Static):
     """Base report widget."""
 
+    BINDINGS: ClassVar[list[BindingType]] = [
+        Binding(key="ctrl+y", action="toggle_works", description="Toggle empty works"),
+    ]
+
+    show_empty_works: reactive[bool] = reactive(True)
+
+    async def action_toggle_works(self) -> None:
+        """Toggle show empty works attribute."""
+        self.show_empty_works = not self.show_empty_works
+        await self.query_one(WorkReportPane).toggle_empty_works()
+
 
 class AuthorReportWidget(ReportWidget):
     """Author report generator view."""
 
     def __init__(self, report: AuthorReport) -> None:
         self.report = report
         super().__init__()
```

### Comparing `pub_analyzer-0.2.0/pub_analyzer/widgets/report/export.py` & `pub_analyzer-0.3.0/pub_analyzer/widgets/report/export.py`

 * *Files identical despite different names*

### Comparing `pub_analyzer-0.2.0/pub_analyzer/widgets/report/institution.py` & `pub_analyzer-0.3.0/pub_analyzer/widgets/report/institution.py`

 * *Files identical despite different names*

### Comparing `pub_analyzer-0.2.0/pub_analyzer/widgets/report/locations.py` & `pub_analyzer-0.3.0/pub_analyzer/widgets/report/locations.py`

 * *Files identical despite different names*

### Comparing `pub_analyzer-0.2.0/pub_analyzer/widgets/report/source.py` & `pub_analyzer-0.3.0/pub_analyzer/widgets/report/source.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,62 +5,69 @@
 from rich.table import Table
 from rich.text import Text
 from textual.app import ComposeResult
 from textual.containers import VerticalScroll
 from textual.widgets import Static
 
 from pub_analyzer.models.report import AuthorReport, InstitutionReport
-from pub_analyzer.models.source import DehydratedSource
+from pub_analyzer.models.source import Source
 
 
 class SourcesTable(Static):
     """All Sources from an author in a table."""
 
     DEFAULT_CSS = """
     SourcesTable .sources-table {
         height: auto;
         margin: 1 0 0 0;
     }
     """
 
-    def __init__(self, sources_list: list[DehydratedSource]) -> None:
+    def __init__(self, sources_list: list[Source]) -> None:
         self.sources_list = sources_list
         super().__init__()
 
     def compose(self) -> ComposeResult:
         """Compose Table."""
         sources_table = Table(title="Sources", expand=True, show_lines=True)
 
         # Define Columns
         sources_table.add_column("", justify="center", vertical="middle")
         sources_table.add_column("Name", ratio=3)
         sources_table.add_column("Publisher or institution", ratio=2)
         sources_table.add_column("Type")
         sources_table.add_column("ISSN-L")
-        sources_table.add_column("Is Open Access")
+        sources_table.add_column("Impact factor")
+        sources_table.add_column("h-index")
+        sources_table.add_column("Is OA")
 
         for idx, source in enumerate(self.sources_list):
             if source.host_organization_name:
                 host_organization = (
                     f"""[@click=app.open_link('{quote(str(source.host_organization))}')][u]{source.host_organization_name}[/u][/]"""
                 )
             else:
                 host_organization = "-"
 
             title = f"""[@click=app.open_link('{quote(str(source.id))}')][u]{source.display_name}[/u][/]"""
             type_source = source.type
             issn_l = source.issn_l if source.issn_l else "-"
+            impact_factor = f"{source.summary_stats.two_yr_mean_citedness:.3f}"
+            h_index = f"{source.summary_stats.h_index}"
+
             is_open_access = "[#909d63]True[/]" if source.is_oa else "[#bc5653]False[/]"
 
             sources_table.add_row(
                 str(idx),
                 Text.from_markup(title, overflow="ellipsis"),
                 Text.from_markup(host_organization),
                 Text.from_markup(type_source),
                 Text.from_markup(issn_l),
+                Text.from_markup(impact_factor),
+                Text.from_markup(h_index),
                 Text.from_markup(is_open_access),
             )
 
         yield Static(sources_table, classes="sources-table")
 
 
 class SourcesReportPane(VerticalScroll):
@@ -76,8 +83,8 @@
 
     def __init__(self, report: AuthorReport | InstitutionReport) -> None:
         self.report = report
         super().__init__()
 
     def compose(self) -> ComposeResult:
         """Compose content pane."""
-        yield SourcesTable(sources_list=self.report.sources_resume.sources)
+        yield SourcesTable(sources_list=self.report.sources_summary.sources)
```

### Comparing `pub_analyzer-0.2.0/pub_analyzer/widgets/report/work.py` & `pub_analyzer-0.3.0/pub_analyzer/widgets/report/work.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,20 +13,23 @@
 from pub_analyzer.models.author import Author
 from pub_analyzer.models.report import AuthorReport, CitationReport, CitationType, InstitutionReport, WorkReport
 from pub_analyzer.widgets.common import Modal
 from pub_analyzer.widgets.report.cards import (
     AuthorshipCard,
     CitationMetricsCard,
     OpenAccessCard,
-    OpenAccessResumeCard,
+    OpenAccessSummaryCard,
     ReportCitationMetricsCard,
-    WorksTypeResumeCard,
+    WorksTypeSummaryCard,
 )
 
+from .concept import ConceptsTable
+from .grants import GrantsTable
 from .locations import LocationsTable
+from .topic import TopicsTable
 
 
 class CitedByTable(Static):
     """Table with the summary of the works that cite a work."""
 
     DEFAULT_CSS = """
     CitedByTable .citations-table {
@@ -104,44 +107,63 @@
                 # OpenAccess Info
                 yield OpenAccessCard(work=self.work_report.work)
 
                 # Citation Metrics
                 yield CitationMetricsCard(work_report=self.work_report)
 
             with TabbedContent(id="tables-container"):
+                # Abtract if exists
+                if self.work_report.work.abstract:
+                    with TabPane("Abstract"):
+                        yield Label(self.work_report.work.abstract, classes="abstract")
                 # Citations Table
                 with TabPane("Cited By Works"):
                     if len(self.work_report.cited_by):
                         yield CitedByTable(citations_list=self.work_report.cited_by)
                     else:
                         yield Label("No works found.")
+                # Concepts Table
+                with TabPane("Concepts"):
+                    if len(self.work_report.work.concepts):
+                        yield ConceptsTable(self.work_report.work.concepts)
+                    else:
+                        yield Label("No Concepts found.")
+                # Grants Table
+                with TabPane("Grants"):
+                    if len(self.work_report.work.grants):
+                        yield GrantsTable(self.work_report.work.grants)
+                    else:
+                        yield Label("No Grants found.")
                 # Locations Table
                 with TabPane("Locations"):
                     if len(self.work_report.work.locations):
                         yield LocationsTable(self.work_report.work.locations)
                     else:
                         yield Label("No sources found.")
-                # Abtract if exists
-                if self.work_report.work.abstract:
-                    with TabPane("Abstract"):
-                        yield Label(self.work_report.work.abstract, classes="abstract")
+                # Topics Table
+                with TabPane("Topics"):
+                    if len(self.work_report.work.topics):
+                        yield TopicsTable(self.work_report.work.topics)
+                    else:
+                        yield Label("No Topics found.")
 
 
 class WorksTable(Static):
     """Table with all works produced by an author."""
 
     DEFAULT_CSS = """
     WorksTable {
         height: auto;
         margin: 1 0 0 0;
     }
     """
 
-    def __init__(self, report: AuthorReport | InstitutionReport) -> None:
+    def __init__(self, report: AuthorReport | InstitutionReport, show_empty_works: bool = True) -> None:
         self.report = report
+        self.show_empty_works = show_empty_works
         super().__init__()
 
     class _WorksTableRenderer(Static):
         """Virtual Static Widget to handle table actions calls."""
 
         def __init__(self, renderable: RenderableType, report: AuthorReport | InstitutionReport) -> None:
             self.report = report
@@ -170,14 +192,17 @@
         work_table.add_column("Type", ratio=2)
         work_table.add_column("DOI")
         work_table.add_column("Publication Date")
         work_table.add_column("Cited by count")
 
         for idx, work_report in enumerate(self.report.works):
             work = work_report.work
+            if not self.show_empty_works and len(work_report.cited_by) < 1:
+                continue
+
             doi = work.ids.doi
             doi_url = f"""[@click=app.open_link("{quote(str(doi))}")]DOI[/]""" if doi else "-"
 
             work_table.add_row(
                 str(f"""[@click=open_work_details({idx})]{idx}[/]"""),
                 Text(work.title, overflow="ellipsis"),
                 Text(work.type),
@@ -200,16 +225,27 @@
     }
     """
 
     def __init__(self, report: AuthorReport | InstitutionReport) -> None:
         self.report = report
         super().__init__()
 
+    async def toggle_empty_works(self) -> None:
+        """Hide/show works if cites are cero."""
+        report_works_status: bool = self.app.query_one("ReportWidget").show_empty_works  # type: ignore
+        table_works_status = self.query_one(WorksTable).show_empty_works
+
+        if self.report.works and (report_works_status != table_works_status):
+            self.loading = True
+            await self.query_one(WorksTable).remove()
+            await self.mount(WorksTable(report=self.report, show_empty_works=report_works_status))
+            self.loading = False
+
     def compose(self) -> ComposeResult:
         """Compose content pane."""
         with Horizontal(classes="cards-container"):
             yield ReportCitationMetricsCard(report=self.report)
-            yield WorksTypeResumeCard(report=self.report)
-            yield OpenAccessResumeCard(report=self.report)
+            yield WorksTypeSummaryCard(report=self.report)
+            yield OpenAccessSummaryCard(report=self.report)
 
         if self.report.works:
             yield WorksTable(report=self.report)
```

### Comparing `pub_analyzer-0.2.0/pub_analyzer/widgets/search/core.py` & `pub_analyzer-0.3.0/pub_analyzer/widgets/search/core.py`

 * *Files identical despite different names*

### Comparing `pub_analyzer-0.2.0/pub_analyzer/widgets/search/results.py` & `pub_analyzer-0.3.0/pub_analyzer/widgets/search/results.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 from textual.app import ComposeResult
 from textual.containers import Horizontal, Vertical
 from textual.widgets import Button, Label, Static
 
 from pub_analyzer.models.author import AuthorResult
 from pub_analyzer.models.institution import InstitutionResult
-from pub_analyzer.widgets.author.core import AuthorResumeWidget
-from pub_analyzer.widgets.institution.core import InstitutionResumeWidget
+from pub_analyzer.widgets.author.core import AuthorSummaryWidget
+from pub_analyzer.widgets.institution.core import InstitutionSummaryWidget
 
 
 class ResultWidget(Static):
     """Result Widget."""
 
     DEFAULT_CLASSES = "result-widget"
 
@@ -35,22 +35,22 @@
                 yield Label(f"[bold]Works count:[/bold] {self.author_result.works_count}", classes="works-count")
                 yield Label(f"""[@click=app.open_link('{quote(str(self.author_result.external_id))}')]ORCID[/]""", classes="external-id")
 
             # Author hint
             yield Label(self.author_result.hint or "", classes="text-hint")
 
     async def on_button_pressed(self, event: Button.Pressed) -> None:
-        """Go to the Author resume page."""
+        """Go to the Author summary page."""
         from pub_analyzer.widgets.body import MainContent
 
-        author_resume_widget = AuthorResumeWidget(author_result=self.author_result)
+        author_summary_widget = AuthorSummaryWidget(author_result=self.author_result)
 
         main_content = self.app.query_one(MainContent)
         main_content.update_title(title=self.author_result.display_name)
-        await main_content.mount(author_resume_widget)
+        await main_content.mount(author_summary_widget)
 
         await self.app.query_one("FinderWidget").remove()
 
 
 class InstitutionResultWidget(ResultWidget):
     """Institution result widget."""
 
@@ -70,17 +70,17 @@
                 yield Label(f"[bold]Works count:[/bold] {self.institution_result.works_count}", classes="works-count")
                 yield Label(f"""[@click=app.open_link('{quote(str(external_id))}')]External ID[/]""", classes="external-id")
 
             # Institution hint
             yield Label(self.institution_result.hint or "", classes="text-hint")
 
     async def on_button_pressed(self, event: Button.Pressed) -> None:
-        """Go to the Institution resume page."""
+        """Go to the Institution summary page."""
         from pub_analyzer.widgets.body import MainContent
 
-        institution_resume_widget = InstitutionResumeWidget(institution_result=self.institution_result)
+        institution_summary_widget = InstitutionSummaryWidget(institution_result=self.institution_result)
 
         main_content = self.app.query_one(MainContent)
         main_content.update_title(title=self.institution_result.display_name)
-        await main_content.mount(institution_resume_widget)
+        await main_content.mount(institution_summary_widget)
 
         await self.app.query_one("FinderWidget").remove()
```

### Comparing `pub_analyzer-0.2.0/pub_analyzer/widgets/sidebar.py` & `pub_analyzer-0.3.0/pub_analyzer/widgets/sidebar.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Sidebar components and options."""
+
 from enum import Enum
+from importlib.metadata import version
 
 from textual import on
 from textual.app import ComposeResult
 from textual.containers import Vertical
 from textual.widget import Widget
 from textual.widgets import Button, Label, Static
 
@@ -21,27 +23,34 @@
 class SideBar(Static):
     """SideBar Widget."""
 
     DEFAULT_CLASSES = "sidebar"
 
     def compose(self) -> ComposeResult:
         """Compose dynamically the sidebar options."""
+        pub_analyzer_version = version("pub-analyzer")
+
         with Vertical(classes="sidebar-options-column"):
             yield Label("Menu", id="sidebar-title")
 
-            yield Button(SideBarOptionsName.SEARCH.value, variant="primary", id="search-sidebar-button", classes="sidebar-option")
-            yield Button(SideBarOptionsName.LOAD_REPORT.value, variant="primary", id="load-sidebar-button", classes="sidebar-option")
+            with Vertical(classes="sidebar-buttons-column"):
+                yield Button(SideBarOptionsName.SEARCH.value, variant="primary", id="search-sidebar-button", classes="sidebar-option")
+                yield Button(SideBarOptionsName.LOAD_REPORT.value, variant="primary", id="load-sidebar-button", classes="sidebar-option")
+
+            yield Label(f"v{pub_analyzer_version}", id="module-version-label")
 
     def toggle(self) -> None:
         """Show/Hide Sidebar."""
         if self.has_class("-hidden"):
             self.remove_class("-hidden")
+            self.styles.animate("width", value=20, duration=0.5)
         else:
             if self.query("*:focus"):
                 self.screen.set_focus(None)
+            self.styles.animate("width", value=0, duration=0.5)
             self.add_class("-hidden")
 
     async def _replace_main_content(self, new_title: str, new_widget: Widget) -> None:
         """Delete the old widgets in the main section, update the main title and replace it with the given Widget."""
         from pub_analyzer.widgets.body import MainContent
 
         main_content = self.app.query_one(MainContent)
```

### Comparing `pub_analyzer-0.2.0/pyproject.toml` & `pub_analyzer-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pub-analyzer"
-version = "0.2.0"
+version = "0.3.0"
 description = "A text user interface, written in python, which automates the generation of scientific production reports using OpenAlex"
 
 authors = ["Alejandro Gaspar <alejandro@gaspar.land>"]
 maintainers = ["Alejandro Gaspar <alejandro@gaspar.land>"]
 
 homepage = "https://github.com/alejandrgaspar/pub-analyzer"
 repository = "https://github.com/alejandrgaspar/pub-analyzer"
@@ -26,59 +26,62 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows :: Windows 10",
     "Operating System :: Microsoft :: Windows :: Windows 11",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Typing :: Typed",
 ]
 
 [tool.poetry.scripts]
 pub-analyzer = "pub_analyzer.main:run"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
-textual = "0.41.0"
-httpx = "0.25.1"
-pydantic = "2.4.2"
+textual = "0.58.0"
+httpx = "0.27.0"
+pydantic = "2.7.1"
 
-typst = "0.8.0"
-jinja2 = "3.1.2"
+typst = "0.11.0"
+jinja2 = "3.1.3"
 
 [tool.poetry.group.dev.dependencies]
-textual-dev = "1.2.1"
+textual-dev = "1.5.1"
 
-pre-commit = "3.5.0"
-mypy = "1.6.1"
-ruff = "0.1.3"
+pre-commit = "3.7.0"
+mypy = "1.10.0"
+ruff = "0.4.2"
 
-pytest = "7.4.3"
+pytest = "8.2.0"
 pytest-asyncio = "0.21.1"
-respx = "0.20.2"
-vcrpy = "5.1.0"
-pytest-recording = "0.13.0"
+respx = "0.21.1"
+vcrpy = "6.0.1"
+pytest-recording = "0.13.1"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "1.5.3"
-mkdocs-material = "9.4.7"
+mkdocs-material = "9.5.18"
 
-mkdocstrings = {extras = ["python"], version = "0.23.0"}
-mkdocstrings-python = "1.7.3"
+mkdocstrings = {extras = ["python"], version = "0.25.0"}
+mkdocstrings-python = "1.10.0"
 
 [tool.mypy]
 strict = true
 
 [tool.ruff]
-required-version = "0.1.3"
+required-version = ">=0.3.4"
 target-version = "py310"
 
 line-length = 140
 
+
+[tool.ruff.lint]
 select = [
     "B",   # flake8-bugbear
     "C",   # flake8-comprehensions
     "D",   # pydocstyle
     "E",   # pycodestyle errors
     "F",   # pyflakes
     "I",   # isort
@@ -97,16 +100,16 @@
     "D402",  # First line should not be the function's signature
     "D413",  # Missing blank line after last section ("{name}")
     "D415",  # First line should end with a period, question mark, or exclamation point
     "D416",  # Section name should end with a colon ("{name}")
     "D417",  # Missing argument description in the docstring: {name}
 ]
 
-[tool.ruff.format]
-indent-style = "space"
-quote-style = "double"
-
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "google"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
+
+[tool.ruff.format]
+indent-style = "space"
+quote-style = "double"
```

### Comparing `pub_analyzer-0.2.0/PKG-INFO` & `pub_analyzer-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pub-analyzer
-Version: 0.2.0
+Version: 0.3.0
 Summary: A text user interface, written in python, which automates the generation of scientific production reports using OpenAlex
 Home-page: https://github.com/alejandrgaspar/pub-analyzer
 License: MIT
 Author: Alejandro Gaspar
 Author-email: alejandro@gaspar.land
 Maintainer: Alejandro Gaspar
 Maintainer-email: alejandro@gaspar.land
@@ -16,28 +16,29 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
-Requires-Dist: httpx (==0.25.1)
-Requires-Dist: jinja2 (==3.1.2)
-Requires-Dist: pydantic (==2.4.2)
-Requires-Dist: textual (==0.41.0)
-Requires-Dist: typst (==0.8.0)
+Requires-Dist: httpx (==0.27.0)
+Requires-Dist: jinja2 (==3.1.3)
+Requires-Dist: pydantic (==2.7.1)
+Requires-Dist: textual (==0.58.0)
+Requires-Dist: typst (==0.11.0)
 Project-URL: Documentation, https://pub-analyzer.com/
 Project-URL: Repository, https://github.com/alejandrgaspar/pub-analyzer
 Description-Content-Type: text/markdown
 
 # Pub Analyzer
 
 <p align="center">
-    <img src="docs/assets/img/logo.png" alt="PubAnalyzer" width="275">
+    <img src="https://raw.githubusercontent.com/alejandrgaspar/pub-analyzer/main/docs/assets/img/logo.png" alt="PubAnalyzer splash image" width="275">
 </p>
 
 <p align="center">
     <a href="https://github.com/alejandrgaspar/pub-analyzer/actions/workflows/python-test.yml" target="_blank">
         <img src="https://github.com/alejandrgaspar/pub-analyzer/actions/workflows/python-test.yml/badge.svg?branch=main" alt="Test status">
     </a>
     <a href="https://pypi.org/project/pub-analyzer/" target="_blank">
```

#### html2text {}

```diff
@@ -1,26 +1,27 @@
-Metadata-Version: 2.1 Name: pub-analyzer Version: 0.2.0 Summary: A text user
+Metadata-Version: 2.1 Name: pub-analyzer Version: 0.3.0 Summary: A text user
 interface, written in python, which automates the generation of scientific
 production reports using OpenAlex Home-page: https://github.com/alejandrgaspar/
 pub-analyzer License: MIT Author: Alejandro Gaspar Author-email:
 alejandro@gaspar.land Maintainer: Alejandro Gaspar Maintainer-email:
 alejandro@gaspar.land Requires-Python: >=3.10,<4.0 Classifier: Development
 Status :: 3 - Alpha Classifier: Environment :: Console Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS Classifier: Operating System :: Microsoft
 :: Windows :: Windows 10 Classifier: Operating System :: Microsoft :: Windows
 :: Windows 11 Classifier: Operating System :: POSIX :: Linux Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier: Typing
-:: Typed Requires-Dist: httpx (==0.25.1) Requires-Dist: jinja2 (==3.1.2)
-Requires-Dist: pydantic (==2.4.2) Requires-Dist: textual (==0.41.0) Requires-
-Dist: typst (==0.8.0) Project-URL: Documentation, https://pub-analyzer.com/
-Project-URL: Repository, https://github.com/alejandrgaspar/pub-analyzer
-Description-Content-Type: text/markdown # Pub Analyzer
-                                 [PubAnalyzer]
+:: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Classifier: Typing :: Typed Requires-
+Dist: httpx (==0.27.0) Requires-Dist: jinja2 (==3.1.3) Requires-Dist: pydantic
+(==2.7.1) Requires-Dist: textual (==0.58.0) Requires-Dist: typst (==0.11.0)
+Project-URL: Documentation, https://pub-analyzer.com/ Project-URL: Repository,
+https://github.com/alejandrgaspar/pub-analyzer Description-Content-Type: text/
+markdown # Pub Analyzer
+                          [PubAnalyzer splash image]
        _[_T_e_s_t_ _s_t_a_t_u_s_]_[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_ _M_I_T_]
  Pub-Analyzer —_PP_uu_bb_ll_ii_cc_aa_tt_ii_oo_nn_ _AA_nn_aa_ll_yy_zz_ee_rr— is a Text User Interface —TTUUII— written in
  Python, which automates the generation of scientific production reports using
                                    _OO_pp_ee_nn_AA_ll_ee_xx.
 --- ## What is Pub Analyzer for? Pub Analyzer is a tool designed to retrieve,
 process and present in a concise and understandable way the scientific
 production of a researcher, including detailed information about their
```

