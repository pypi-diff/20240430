# Comparing `tmp/nestipy_peewee-0.1.5.tar.gz` & `tmp/nestipy_peewee-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestipy_peewee-0.1.5.tar", max compression
+gzip compressed data, was "nestipy_peewee-0.1.6.tar", max compression
```

## Comparing `nestipy_peewee-0.1.5.tar` & `nestipy_peewee-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1054 2024-03-29 11:21:44.560810 nestipy_peewee-0.1.5/LICENSE
--rw-r--r--   0        0        0     1906 2024-04-26 13:39:21.397719 nestipy_peewee-0.1.5/README.md
--rw-r--r--   0        0        0      475 2024-04-29 13:44:09.302232 nestipy_peewee-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      185 2024-04-27 07:50:37.316624 nestipy_peewee-0.1.5/src/nestipy_peewee/__init__.py
--rw-r--r--   0        0        0      740 2024-04-29 10:45:37.648124 nestipy_peewee-0.1.5/src/nestipy_peewee/peewee_builder.py
--rw-r--r--   0        0        0      410 2024-04-29 11:05:46.313907 nestipy_peewee-0.1.5/src/nestipy_peewee/peewee_decorator.py
--rw-r--r--   0        0        0       58 2024-04-27 06:47:04.319886 nestipy_peewee-0.1.5/src/nestipy_peewee/peewee_meta.py
--rw-r--r--   0        0        0     2327 2024-04-29 11:04:32.938907 nestipy_peewee-0.1.5/src/nestipy_peewee/peewee_module.py
--rw-r--r--   0        0        0     2382 1970-01-01 00:00:00.000000 nestipy_peewee-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1054 2024-03-29 11:21:44.560810 nestipy_peewee-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1906 2024-04-26 13:39:21.397719 nestipy_peewee-0.1.6/README.md
+-rw-r--r--   0        0        0      501 2024-04-30 15:21:38.380098 nestipy_peewee-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      185 2024-04-27 07:50:37.316624 nestipy_peewee-0.1.6/src/nestipy_peewee/__init__.py
+-rw-r--r--   0        0        0      740 2024-04-29 10:45:37.648124 nestipy_peewee-0.1.6/src/nestipy_peewee/peewee_builder.py
+-rw-r--r--   0        0        0      410 2024-04-29 11:05:46.313907 nestipy_peewee-0.1.6/src/nestipy_peewee/peewee_decorator.py
+-rw-r--r--   0        0        0       58 2024-04-27 06:47:04.319886 nestipy_peewee-0.1.6/src/nestipy_peewee/peewee_meta.py
+-rw-r--r--   0        0        0     2327 2024-04-29 11:04:32.938907 nestipy_peewee-0.1.6/src/nestipy_peewee/peewee_module.py
+-rw-r--r--   0        0        0     2429 1970-01-01 00:00:00.000000 nestipy_peewee-0.1.6/PKG-INFO
```

### Comparing `nestipy_peewee-0.1.5/LICENSE` & `nestipy_peewee-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nestipy_peewee-0.1.5/README.md` & `nestipy_peewee-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `nestipy_peewee-0.1.5/src/nestipy_peewee/peewee_builder.py` & `nestipy_peewee-0.1.6/src/nestipy_peewee/peewee_builder.py`

 * *Files identical despite different names*

### Comparing `nestipy_peewee-0.1.5/src/nestipy_peewee/peewee_module.py` & `nestipy_peewee-0.1.6/src/nestipy_peewee/peewee_module.py`

 * *Files identical despite different names*

### Comparing `nestipy_peewee-0.1.5/PKG-INFO` & `nestipy_peewee-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: nestipy-peewee
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: tsiresymila
 Author-email: tsiresymila@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: nestipy (>=0.2.9,<0.3.0)
+Requires-Dist: nestipy (>=0.3.0,<0.4.0)
+Requires-Dist: nestipy-config (>=0.1.2,<0.2.0)
 Requires-Dist: peewee (>=3.17.3,<4.0.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a target="_blank"><img src="https://raw.githubusercontent.com/nestipy/nestipy/release-v1/nestipy.png" width="200" alt="Nestipy Logo" /></a></p>
 <p align="center">
     <a href="https://pypi.org/project/nestipy">
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: nestipy-peewee Version: 0.1.5 Summary: Author:
+Metadata-Version: 2.1 Name: nestipy-peewee Version: 0.1.6 Summary: Author:
 tsiresymila Author-email: tsiresymila@gmail.com Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: nestipy
-(>=0.2.9,<0.3.0) Requires-Dist: peewee (>=3.17.3,<4.0.0) Description-Content-
-Type: text/markdown
+(>=0.3.0,<0.4.0) Requires-Dist: nestipy-config (>=0.1.2,<0.2.0) Requires-Dist:
+peewee (>=3.17.3,<4.0.0) Description-Content-Type: text/markdown
                                 [Nestipy Logo]
                           _[_V_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]_[_L_i_c_e_n_s_e_]
 ## Description
 Nestipy is a Python framework built on top of FastAPI that follows the modular
 architecture of NestJS
 Under the hood, Nestipy makes use of _F_a_s_t_A_P_I, but also provides compatibility
 with a wide range of other libraries, like _B_l_a_c_k_s_h_e_e_p, allowing for easy use of
```

