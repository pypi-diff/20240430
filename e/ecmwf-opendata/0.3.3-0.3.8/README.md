# Comparing `tmp/ecmwf-opendata-0.3.3.tar.gz` & `tmp/ecmwf-opendata-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecmwf-opendata-0.3.3.tar", last modified: Mon Mar  4 14:15:38 2024, max compression
+gzip compressed data, was "ecmwf-opendata-0.3.8.tar", last modified: Tue Apr 30 08:14:27 2024, max compression
```

## Comparing `ecmwf-opendata-0.3.3.tar` & `ecmwf-opendata-0.3.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:15:38.833519 ecmwf-opendata-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-04 14:15:24.000000 ecmwf-opendata-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22113 2024-03-04 14:15:38.833519 ecmwf-opendata-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21147 2024-03-04 14:15:24.000000 ecmwf-opendata-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:15:38.829519 ecmwf-opendata-0.3.3/ecmwf/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:15:38.833519 ecmwf-opendata-0.3.3/ecmwf/opendata/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-04 14:15:24.000000 ecmwf-opendata-0.3.3/ecmwf/opendata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-03-04 14:15:24.000000 ecmwf-opendata-0.3.3/ecmwf/opendata/bufr.py
--rw-r--r--   0 runner    (1001) docker     (127)    15358 2024-03-04 14:15:24.000000 ecmwf-opendata-0.3.3/ecmwf/opendata/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-03-04 14:15:24.000000 ecmwf-opendata-0.3.3/ecmwf/opendata/date.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-03-04 14:15:24.000000 ecmwf-opendata-0.3.3/ecmwf/opendata/grib.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-03-04 14:15:24.000000 ecmwf-opendata-0.3.3/ecmwf/opendata/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:15:38.833519 ecmwf-opendata-0.3.3/ecmwf_opendata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22113 2024-03-04 14:15:38.000000 ecmwf-opendata-0.3.3/ecmwf_opendata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-04 14:15:38.000000 ecmwf-opendata-0.3.3/ecmwf_opendata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 14:15:38.000000 ecmwf-opendata-0.3.3/ecmwf_opendata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-04 14:15:38.000000 ecmwf-opendata-0.3.3/ecmwf_opendata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-04 14:15:38.000000 ecmwf-opendata-0.3.3/ecmwf_opendata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 14:15:38.000000 ecmwf-opendata-0.3.3/ecmwf_opendata.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 14:15:38.833519 ecmwf-opendata-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-03-04 14:15:24.000000 ecmwf-opendata-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:14:27.510915 ecmwf-opendata-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 08:14:16.000000 ecmwf-opendata-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22113 2024-04-30 08:14:27.510915 ecmwf-opendata-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21147 2024-04-30 08:14:16.000000 ecmwf-opendata-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:14:27.506915 ecmwf-opendata-0.3.8/ecmwf/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:14:27.506915 ecmwf-opendata-0.3.8/ecmwf/opendata/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-30 08:14:16.000000 ecmwf-opendata-0.3.8/ecmwf/opendata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-30 08:14:16.000000 ecmwf-opendata-0.3.8/ecmwf/opendata/bufr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15504 2024-04-30 08:14:16.000000 ecmwf-opendata-0.3.8/ecmwf/opendata/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-30 08:14:16.000000 ecmwf-opendata-0.3.8/ecmwf/opendata/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-30 08:14:16.000000 ecmwf-opendata-0.3.8/ecmwf/opendata/grib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-30 08:14:16.000000 ecmwf-opendata-0.3.8/ecmwf/opendata/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:14:27.506915 ecmwf-opendata-0.3.8/ecmwf_opendata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22113 2024-04-30 08:14:27.000000 ecmwf-opendata-0.3.8/ecmwf_opendata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-30 08:14:27.000000 ecmwf-opendata-0.3.8/ecmwf_opendata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 08:14:27.000000 ecmwf-opendata-0.3.8/ecmwf_opendata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 08:14:27.000000 ecmwf-opendata-0.3.8/ecmwf_opendata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 08:14:27.000000 ecmwf-opendata-0.3.8/ecmwf_opendata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 08:14:27.000000 ecmwf-opendata-0.3.8/ecmwf_opendata.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 08:14:27.510915 ecmwf-opendata-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-30 08:14:16.000000 ecmwf-opendata-0.3.8/setup.py
```

### Comparing `ecmwf-opendata-0.3.3/LICENSE` & `ecmwf-opendata-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ecmwf-opendata-0.3.3/PKG-INFO` & `ecmwf-opendata-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecmwf-opendata
-Version: 0.3.3
+Version: 0.3.8
 Summary: A package to download ECMWF open data
 Home-page: https://github.com/ecmwf/ecmwf-opendata
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
 Keywords: tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ecmwf-opendata-0.3.3/README.md` & `ecmwf-opendata-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `ecmwf-opendata-0.3.3/ecmwf/opendata/bufr.py` & `ecmwf-opendata-0.3.8/ecmwf/opendata/bufr.py`

 * *Files identical despite different names*

### Comparing `ecmwf-opendata-0.3.3/ecmwf/opendata/client.py` & `ecmwf-opendata-0.3.8/ecmwf/opendata/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,14 +225,18 @@
             args["_yyyymmdd"] = date.strftime("%Y%m%d")
             args["_H"] = date.strftime("%H")
             args["_yyyymmddHHMMSS"] = date.strftime("%Y%m%d%H%M%S")
             args["_extension"] = EXTENSIONS.get(args["type"], "grib2")
             args["_stream"] = self.patch_stream(args)
 
             url = pattern.format(**args)
+
+            if self.resol == "0p4-beta":
+                url = url.replace("/ifs/", "/")
+
             if url not in seen:
                 data_urls.append(url)
                 seen.add(url)
 
         if for_index and use_index:
             data_urls = self.get_parts(data_urls, for_index)
 
@@ -277,14 +281,15 @@
                     parts.append((tuple(matches), (line["_offset"], line["_length"])))
 
             if parts:
                 result.append((url, tuple(p[1] for p in sorted(parts))))
 
         for name, values in for_index.items():
             diff = set(values).difference(possible_values[name])
+            print(diff, sorted(possible_values[name]))
             for d in diff:
                 warning_once(
                     "No index entries for %s=%s",
                     name,
                     d,
                     did_you_mean=(d, possible_values[name]),
                 )
```

### Comparing `ecmwf-opendata-0.3.3/ecmwf/opendata/date.py` & `ecmwf-opendata-0.3.8/ecmwf/opendata/date.py`

 * *Files identical despite different names*

### Comparing `ecmwf-opendata-0.3.3/ecmwf/opendata/grib.py` & `ecmwf-opendata-0.3.8/ecmwf/opendata/grib.py`

 * *Files identical despite different names*

### Comparing `ecmwf-opendata-0.3.3/ecmwf/opendata/urls.py` & `ecmwf-opendata-0.3.8/ecmwf/opendata/urls.py`

 * *Files identical despite different names*

### Comparing `ecmwf-opendata-0.3.3/ecmwf_opendata.egg-info/PKG-INFO` & `ecmwf-opendata-0.3.8/ecmwf_opendata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecmwf-opendata
-Version: 0.3.3
+Version: 0.3.8
 Summary: A package to download ECMWF open data
 Home-page: https://github.com/ecmwf/ecmwf-opendata
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
 Keywords: tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ecmwf-opendata-0.3.3/setup.py` & `ecmwf-opendata-0.3.8/setup.py`

 * *Files identical despite different names*

