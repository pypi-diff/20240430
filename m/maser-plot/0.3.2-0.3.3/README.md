# Comparing `tmp/maser_plot-0.3.2.tar.gz` & `tmp/maser_plot-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maser_plot-0.3.2.tar", max compression
+gzip compressed data, was "maser_plot-0.3.3.tar", max compression
```

## Comparing `maser_plot-0.3.2.tar` & `maser_plot-0.3.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     2582 2024-03-15 09:04:50.806732 maser_plot-0.3.2/README.md
--rw-r--r--   0        0        0       80 2024-03-14 14:17:35.227635 maser_plot-0.3.2/maser/__init__.py
--rw-r--r--   0        0        0     1797 2024-03-15 09:04:50.797860 maser_plot-0.3.2/maser/plot/__init__.py
--rw-r--r--   0        0        0      533 2024-03-15 09:04:50.798014 maser_plot-0.3.2/maser/plot/base/__init__.py
--rw-r--r--   0        0        0    13234 2024-03-15 09:04:50.798169 maser_plot-0.3.2/maser/plot/base/base.py
--rw-r--r--   0        0        0     1306 2024-03-15 09:04:50.798380 maser_plot-0.3.2/maser/plot/base/dataset_filename_regex.json
--rw-r--r--   0        0        0      673 2024-03-15 09:04:50.798506 maser_plot-0.3.2/maser/plot/cdpp/__init__.py
--rw-r--r--   0        0        0       89 2024-03-15 09:04:50.798737 maser_plot-0.3.2/maser/plot/cdpp/interball/__init__.py
--rw-r--r--   0        0        0      501 2024-03-15 09:04:50.798852 maser_plot-0.3.2/maser/plot/cdpp/interball/plot.py
--rw-r--r--   0        0        0      208 2024-03-15 09:04:50.798965 maser_plot-0.3.2/maser/plot/cdpp/stereo/__init__.py
--rw-r--r--   0        0        0     2406 2024-03-15 09:04:50.799094 maser_plot-0.3.2/maser/plot/cdpp/stereo/plot.py
--rw-r--r--   0        0        0       75 2024-03-15 09:04:50.799252 maser_plot-0.3.2/maser/plot/cdpp/viking/__init__.py
--rw-r--r--   0        0        0      198 2024-03-15 09:04:50.799392 maser_plot-0.3.2/maser/plot/cdpp/viking/plot.py
--rw-r--r--   0        0        0      346 2024-03-15 09:04:50.799562 maser_plot-0.3.2/maser/plot/cdpp/wind/__init__.py
--rw-r--r--   0        0        0     2198 2024-03-15 09:04:50.799743 maser_plot-0.3.2/maser/plot/cdpp/wind/plot.py
--rw-r--r--   0        0        0      403 2024-03-15 09:04:50.799949 maser_plot-0.3.2/maser/plot/ecallisto/__init__.py
--rw-r--r--   0        0        0      622 2024-03-15 09:04:50.800086 maser_plot-0.3.2/maser/plot/ecallisto/plot.py
--rw-r--r--   0        0        0      826 2024-03-15 09:04:50.800296 maser_plot-0.3.2/maser/plot/nancay/__init__.py
--rw-r--r--   0        0        0      273 2024-03-15 09:04:50.800431 maser_plot-0.3.2/maser/plot/nancay/nda/__init__.py
--rw-r--r--   0        0        0     2511 2024-03-15 09:04:50.800571 maser_plot-0.3.2/maser/plot/nancay/nda/plot.py
--rw-r--r--   0        0        0      128 2024-03-15 09:04:50.800808 maser_plot-0.3.2/maser/plot/nancay/nenufar/__init__.py
--rw-r--r--   0        0        0      525 2024-03-15 09:04:50.801039 maser_plot-0.3.2/maser/plot/nancay/nenufar/plot.py
--rw-r--r--   0        0        0      690 2024-03-15 09:04:50.801191 maser_plot-0.3.2/maser/plot/padc/__init__.py
--rw-r--r--   0        0        0       73 2024-03-15 09:04:50.801341 maser_plot-0.3.2/maser/plot/padc/bepi/__init__.py
--rw-r--r--   0        0        0      118 2024-03-15 09:04:50.801504 maser_plot-0.3.2/maser/plot/padc/bepi/sorbet/__init__.py
--rw-r--r--   0        0        0      633 2024-03-15 09:04:50.801719 maser_plot-0.3.2/maser/plot/padc/bepi/sorbet/plot.py
--rw-r--r--   0        0        0      114 2024-03-15 09:04:50.801873 maser_plot-0.3.2/maser/plot/padc/cassini/__init__.py
--rw-r--r--   0        0        0     2295 2024-03-15 09:04:50.802083 maser_plot-0.3.2/maser/plot/padc/cassini/plot.py
--rw-r--r--   0        0        0     1243 2024-03-15 09:04:50.802221 maser_plot-0.3.2/maser/plot/padc/expres/__init__.py
--rw-r--r--   0        0        0     1562 2024-03-15 09:04:50.802400 maser_plot-0.3.2/maser/plot/padc/expres/plot.py
--rw-r--r--   0        0        0       87 2024-03-15 09:04:50.802630 maser_plot-0.3.2/maser/plot/padc/juno/__init__.py
--rw-r--r--   0        0        0     2321 2024-03-15 09:04:50.802835 maser_plot-0.3.2/maser/plot/padc/juno/plot.py
--rw-r--r--   0        0        0      260 2024-03-15 09:04:50.803049 maser_plot-0.3.2/maser/plot/padc/stereo/__init__.py
--rw-r--r--   0        0        0     2112 2024-03-15 09:04:50.803383 maser_plot-0.3.2/maser/plot/padc/stereo/plot.py
--rw-r--r--   0        0        0      148 2024-03-15 09:04:50.803237 maser_plot-0.3.2/maser/plot/padc/wind/__init__.py
--rw-r--r--   0        0        0     1376 2024-03-15 09:04:50.803906 maser_plot-0.3.2/maser/plot/padc/wind/plot.py
--rw-r--r--   0        0        0      524 2024-03-15 09:04:50.803647 maser_plot-0.3.2/maser/plot/pds/__init__.py
--rw-r--r--   0        0        0      131 2024-03-15 09:04:50.804105 maser_plot-0.3.2/maser/plot/pds/co/__init__.py
--rw-r--r--   0        0        0      544 2024-03-15 09:04:50.804287 maser_plot-0.3.2/maser/plot/pds/co/plot.py
--rw-r--r--   0        0        0     2555 2024-03-15 09:04:50.804485 maser_plot-0.3.2/maser/plot/pds/plot.py
--rw-r--r--   0        0        0      371 2024-03-15 09:04:50.804649 maser_plot-0.3.2/maser/plot/pds/vg/__init__.py
--rw-r--r--   0        0        0     4510 2024-03-15 09:04:50.804939 maser_plot-0.3.2/maser/plot/pds/vg/plot.py
--rw-r--r--   0        0        0      286 2024-03-15 09:04:50.804788 maser_plot-0.3.2/maser/plot/psa/__init__.py
--rw-r--r--   0        0        0      287 2024-03-15 09:04:50.805078 maser_plot-0.3.2/maser/plot/psa/mex/__init__.py
--rw-r--r--   0        0        0     1221 2024-03-15 09:04:50.805226 maser_plot-0.3.2/maser/plot/psa/mex/plot.py
--rw-r--r--   0        0        0      443 2024-03-15 09:04:50.806115 maser_plot-0.3.2/maser/plot/rpw/__init__.py
--rw-r--r--   0        0        0     3629 2024-03-14 14:17:35.233813 maser_plot-0.3.2/maser/plot/rpw/cross_section.py
--rw-r--r--   0        0        0     4565 2024-03-14 14:17:35.233993 maser_plot-0.3.2/maser/plot/rpw/lfr.py
--rw-r--r--   0        0        0     2733 2024-03-15 09:04:50.806557 maser_plot-0.3.2/maser/plot/rpw/plot.py
--rw-r--r--   0        0        0     5339 2024-03-14 14:17:35.233719 maser_plot-0.3.2/maser/plot/rpw/plot_mean.py
--rw-r--r--   0        0        0     5518 2024-03-14 14:17:35.234796 maser_plot-0.3.2/maser/plot/rpw/quick_look.py
--rw-r--r--   0        0        0     1920 2024-04-29 08:34:17.733548 maser_plot-0.3.2/maser/plot/rpw/tnr.py
--rw-r--r--   0        0        0      440 2024-04-29 08:41:52.604978 maser_plot-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     3216 1970-01-01 00:00:00.000000 maser_plot-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     2582 2024-03-15 09:04:50.806732 maser_plot-0.3.3/README.md
+-rw-r--r--   0        0        0       80 2024-03-14 14:17:35.227635 maser_plot-0.3.3/maser/__init__.py
+-rw-r--r--   0        0        0     1797 2024-03-15 09:04:50.797860 maser_plot-0.3.3/maser/plot/__init__.py
+-rw-r--r--   0        0        0      533 2024-03-15 09:04:50.798014 maser_plot-0.3.3/maser/plot/base/__init__.py
+-rw-r--r--   0        0        0    13234 2024-03-15 09:04:50.798169 maser_plot-0.3.3/maser/plot/base/base.py
+-rw-r--r--   0        0        0     1306 2024-03-15 09:04:50.798380 maser_plot-0.3.3/maser/plot/base/dataset_filename_regex.json
+-rw-r--r--   0        0        0      673 2024-03-15 09:04:50.798506 maser_plot-0.3.3/maser/plot/cdpp/__init__.py
+-rw-r--r--   0        0        0       89 2024-03-15 09:04:50.798737 maser_plot-0.3.3/maser/plot/cdpp/interball/__init__.py
+-rw-r--r--   0        0        0      501 2024-03-15 09:04:50.798852 maser_plot-0.3.3/maser/plot/cdpp/interball/plot.py
+-rw-r--r--   0        0        0      208 2024-03-15 09:04:50.798965 maser_plot-0.3.3/maser/plot/cdpp/stereo/__init__.py
+-rw-r--r--   0        0        0     2406 2024-03-15 09:04:50.799094 maser_plot-0.3.3/maser/plot/cdpp/stereo/plot.py
+-rw-r--r--   0        0        0       75 2024-03-15 09:04:50.799252 maser_plot-0.3.3/maser/plot/cdpp/viking/__init__.py
+-rw-r--r--   0        0        0      198 2024-03-15 09:04:50.799392 maser_plot-0.3.3/maser/plot/cdpp/viking/plot.py
+-rw-r--r--   0        0        0      346 2024-03-15 09:04:50.799562 maser_plot-0.3.3/maser/plot/cdpp/wind/__init__.py
+-rw-r--r--   0        0        0     2198 2024-03-15 09:04:50.799743 maser_plot-0.3.3/maser/plot/cdpp/wind/plot.py
+-rw-r--r--   0        0        0      403 2024-03-15 09:04:50.799949 maser_plot-0.3.3/maser/plot/ecallisto/__init__.py
+-rw-r--r--   0        0        0      622 2024-03-15 09:04:50.800086 maser_plot-0.3.3/maser/plot/ecallisto/plot.py
+-rw-r--r--   0        0        0      826 2024-03-15 09:04:50.800296 maser_plot-0.3.3/maser/plot/nancay/__init__.py
+-rw-r--r--   0        0        0      273 2024-03-15 09:04:50.800431 maser_plot-0.3.3/maser/plot/nancay/nda/__init__.py
+-rw-r--r--   0        0        0     2511 2024-03-15 09:04:50.800571 maser_plot-0.3.3/maser/plot/nancay/nda/plot.py
+-rw-r--r--   0        0        0      128 2024-03-15 09:04:50.800808 maser_plot-0.3.3/maser/plot/nancay/nenufar/__init__.py
+-rw-r--r--   0        0        0      525 2024-03-15 09:04:50.801039 maser_plot-0.3.3/maser/plot/nancay/nenufar/plot.py
+-rw-r--r--   0        0        0      690 2024-03-15 09:04:50.801191 maser_plot-0.3.3/maser/plot/padc/__init__.py
+-rw-r--r--   0        0        0       73 2024-03-15 09:04:50.801341 maser_plot-0.3.3/maser/plot/padc/bepi/__init__.py
+-rw-r--r--   0        0        0      118 2024-03-15 09:04:50.801504 maser_plot-0.3.3/maser/plot/padc/bepi/sorbet/__init__.py
+-rw-r--r--   0        0        0      633 2024-03-15 09:04:50.801719 maser_plot-0.3.3/maser/plot/padc/bepi/sorbet/plot.py
+-rw-r--r--   0        0        0      114 2024-03-15 09:04:50.801873 maser_plot-0.3.3/maser/plot/padc/cassini/__init__.py
+-rw-r--r--   0        0        0     2295 2024-03-15 09:04:50.802083 maser_plot-0.3.3/maser/plot/padc/cassini/plot.py
+-rw-r--r--   0        0        0     1243 2024-03-15 09:04:50.802221 maser_plot-0.3.3/maser/plot/padc/expres/__init__.py
+-rw-r--r--   0        0        0     1562 2024-03-15 09:04:50.802400 maser_plot-0.3.3/maser/plot/padc/expres/plot.py
+-rw-r--r--   0        0        0       87 2024-03-15 09:04:50.802630 maser_plot-0.3.3/maser/plot/padc/juno/__init__.py
+-rw-r--r--   0        0        0     2321 2024-03-15 09:04:50.802835 maser_plot-0.3.3/maser/plot/padc/juno/plot.py
+-rw-r--r--   0        0        0      260 2024-03-15 09:04:50.803049 maser_plot-0.3.3/maser/plot/padc/stereo/__init__.py
+-rw-r--r--   0        0        0     2112 2024-03-15 09:04:50.803383 maser_plot-0.3.3/maser/plot/padc/stereo/plot.py
+-rw-r--r--   0        0        0      148 2024-03-15 09:04:50.803237 maser_plot-0.3.3/maser/plot/padc/wind/__init__.py
+-rw-r--r--   0        0        0     1376 2024-03-15 09:04:50.803906 maser_plot-0.3.3/maser/plot/padc/wind/plot.py
+-rw-r--r--   0        0        0      524 2024-03-15 09:04:50.803647 maser_plot-0.3.3/maser/plot/pds/__init__.py
+-rw-r--r--   0        0        0      131 2024-03-15 09:04:50.804105 maser_plot-0.3.3/maser/plot/pds/co/__init__.py
+-rw-r--r--   0        0        0      544 2024-03-15 09:04:50.804287 maser_plot-0.3.3/maser/plot/pds/co/plot.py
+-rw-r--r--   0        0        0     2555 2024-03-15 09:04:50.804485 maser_plot-0.3.3/maser/plot/pds/plot.py
+-rw-r--r--   0        0        0      371 2024-03-15 09:04:50.804649 maser_plot-0.3.3/maser/plot/pds/vg/__init__.py
+-rw-r--r--   0        0        0     4510 2024-03-15 09:04:50.804939 maser_plot-0.3.3/maser/plot/pds/vg/plot.py
+-rw-r--r--   0        0        0      286 2024-03-15 09:04:50.804788 maser_plot-0.3.3/maser/plot/psa/__init__.py
+-rw-r--r--   0        0        0      287 2024-03-15 09:04:50.805078 maser_plot-0.3.3/maser/plot/psa/mex/__init__.py
+-rw-r--r--   0        0        0     1221 2024-03-15 09:04:50.805226 maser_plot-0.3.3/maser/plot/psa/mex/plot.py
+-rw-r--r--   0        0        0      443 2024-03-15 09:04:50.806115 maser_plot-0.3.3/maser/plot/rpw/__init__.py
+-rw-r--r--   0        0        0     3629 2024-03-14 14:17:35.233813 maser_plot-0.3.3/maser/plot/rpw/cross_section.py
+-rw-r--r--   0        0        0     4565 2024-03-14 14:17:35.233993 maser_plot-0.3.3/maser/plot/rpw/lfr.py
+-rw-r--r--   0        0        0     2733 2024-03-15 09:04:50.806557 maser_plot-0.3.3/maser/plot/rpw/plot.py
+-rw-r--r--   0        0        0     5339 2024-03-14 14:17:35.233719 maser_plot-0.3.3/maser/plot/rpw/plot_mean.py
+-rw-r--r--   0        0        0     5518 2024-03-14 14:17:35.234796 maser_plot-0.3.3/maser/plot/rpw/quick_look.py
+-rw-r--r--   0        0        0     2011 2024-04-30 15:52:05.427864 maser_plot-0.3.3/maser/plot/rpw/tnr.py
+-rw-r--r--   0        0        0      442 2024-04-30 15:53:36.207257 maser_plot-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     3210 1970-01-01 00:00:00.000000 maser_plot-0.3.3/PKG-INFO
```

### Comparing `maser_plot-0.3.2/README.md` & `maser_plot-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.2/maser/plot/__init__.py` & `maser_plot-0.3.3/maser/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.2/maser/plot/base/__init__.py` & `maser_plot-0.3.3/maser/plot/base/__init__.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.2/maser/plot/base/base.py` & `maser_plot-0.3.3/maser/plot/base/base.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.2/maser/plot/base/dataset_filename_regex.json` & `maser_plot-0.3.3/maser/plot/base/dataset_filename_regex.json`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.2/maser/plot/cdpp/__init__.py` & `maser_plot-0.3.3/maser/plot/cdpp/__init__.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.2/maser/plot/cdpp/stereo/plot.py` & `maser_plot-0.3.3/maser/plot/cdpp/stereo/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.2/maser/plot/cdpp/wind/plot.py` & `maser_plot-0.3.3/maser/plot/cdpp/wind/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.2/maser/plot/ecallisto/plot.py` & `maser_plot-0.3.3/maser/plot/ecallisto/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.2/maser/plot/nancay/__init__.py` & `maser_plot-0.3.3/maser/plot/nancay/__init__.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.2/maser/plot/nancay/nda/plot.py` & `maser_plot-0.3.3/maser/plot/nancay/nda/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.2/maser/plot/nancay/nenufar/plot.py` & `maser_plot-0.3.3/maser/plot/nancay/nenufar/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.2/maser/plot/padc/__init__.py` & `maser_plot-0.3.3/maser/plot/padc/__init__.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.2/maser/plot/padc/bepi/sorbet/plot.py` & `maser_plot-0.3.3/maser/plot/padc/bepi/sorbet/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.2/maser/plot/padc/cassini/plot.py` & `maser_plot-0.3.3/maser/plot/padc/cassini/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.2/maser/plot/padc/expres/__init__.py` & `maser_plot-0.3.3/maser/plot/padc/expres/__init__.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.2/maser/plot/padc/expres/plot.py` & `maser_plot-0.3.3/maser/plot/padc/expres/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.2/maser/plot/padc/juno/plot.py` & `maser_plot-0.3.3/maser/plot/padc/juno/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.2/maser/plot/padc/stereo/plot.py` & `maser_plot-0.3.3/maser/plot/padc/stereo/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.2/maser/plot/padc/wind/plot.py` & `maser_plot-0.3.3/maser/plot/padc/wind/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.2/maser/plot/pds/__init__.py` & `maser_plot-0.3.3/maser/plot/pds/__init__.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.2/maser/plot/pds/co/plot.py` & `maser_plot-0.3.3/maser/plot/pds/co/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.2/maser/plot/pds/plot.py` & `maser_plot-0.3.3/maser/plot/pds/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.2/maser/plot/pds/vg/plot.py` & `maser_plot-0.3.3/maser/plot/pds/vg/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.2/maser/plot/psa/mex/plot.py` & `maser_plot-0.3.3/maser/plot/psa/mex/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.2/maser/plot/rpw/cross_section.py` & `maser_plot-0.3.3/maser/plot/rpw/cross_section.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.2/maser/plot/rpw/lfr.py` & `maser_plot-0.3.3/maser/plot/rpw/lfr.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.2/maser/plot/rpw/plot.py` & `maser_plot-0.3.3/maser/plot/rpw/plot.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.2/maser/plot/rpw/plot_mean.py` & `maser_plot-0.3.3/maser/plot/rpw/plot_mean.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.2/maser/plot/rpw/quick_look.py` & `maser_plot-0.3.3/maser/plot/rpw/quick_look.py`

 * *Files identical despite different names*

### Comparing `maser_plot-0.3.2/maser/plot/rpw/tnr.py` & `maser_plot-0.3.3/maser/plot/rpw/tnr.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,24 +5,27 @@
 def plot_auto(
     data_wrapper: Data,
     ax,
     *,
     sensor: str = "V1-V2",
     bands: list = ["A", "B", "C", "D"],
     cbar_ax=None,
+    interpol_gap=True,
     **kwargs
 ):
     from matplotlib import colors
     import matplotlib.colorbar as cbar
 
     # create a colorbar axis
     if cbar_ax is None:
         cbar_ax, kw = cbar.make_axes(ax)
 
     auto = data_wrapper.as_xarray()[sensor]
+    if interpol_gap:
+        auto = auto.interpolate_na(dim='time')
 
     # determine min/max for the colorbar
     # use q5 and q95 for vmin and vmax to avoid outliers
     positive_auto = auto.where(auto > 0)
     vmin, vmax = positive_auto.quantile([0.05, 0.95])
 
     plot_kwargs = {
```

### Comparing `maser_plot-0.3.2/PKG-INFO` & `maser_plot-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: maser-plot
-Version: 0.3.2
+Version: 0.3.3
 Summary: Maser4py submodule to plot radio data
 License: CeCILL
 Author: MASER team
 Author-email: contact.maser@obspm.fr
 Requires-Python: >=3.8,<4
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: matplotlib (>=3.5.2,<4.0.0)
+Requires-Dist: matplotlib (>=3.5,<4)
 Description-Content-Type: text/markdown
 
 # About maser-plot
 
 maser-plot is a submodule of [maser4py](https://pypi.org/project/maser4py/).
 
 It can be used with [maser.data](https://pypi.org/project/maser.data/) to plot radio data from the following missions:
```

