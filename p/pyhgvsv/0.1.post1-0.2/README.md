# Comparing `tmp/pyhgvsv-0.1.post1.tar.gz` & `tmp/pyhgvsv-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhgvsv-0.1.post1.tar", last modified: Wed Apr 24 15:49:39 2024, max compression
+gzip compressed data, was "pyhgvsv-0.2.tar", last modified: Tue Apr 30 13:00:45 2024, max compression
```

## Comparing `pyhgvsv-0.1.post1.tar` & `pyhgvsv-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 i9a5000   (1000) i9a5000   (1000)        0 2024-04-24 15:49:39.629853 pyhgvsv-0.1.post1/
--rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)     1100 2024-04-24 14:01:21.000000 pyhgvsv-0.1.post1/LICENSE
--rw-r--r--   0 i9a5000   (1000) i9a5000   (1000)     8864 2024-04-24 15:49:39.629853 pyhgvsv-0.1.post1/PKG-INFO
--rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)     8380 2024-04-24 15:43:44.000000 pyhgvsv-0.1.post1/README.md
--rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)      586 2024-04-24 15:48:18.000000 pyhgvsv-0.1.post1/pyproject.toml
--rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)       38 2024-04-24 15:49:39.629853 pyhgvsv-0.1.post1/setup.cfg
-drwxrwxr-x   0 i9a5000   (1000) i9a5000   (1000)        0 2024-04-24 15:49:39.621853 pyhgvsv-0.1.post1/src/
-drwxrwxr-x   0 i9a5000   (1000) i9a5000   (1000)        0 2024-04-24 15:49:39.629853 pyhgvsv-0.1.post1/src/pyhgvsv/
--rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)    50833 2024-04-24 15:15:07.000000 pyhgvsv-0.1.post1/src/pyhgvsv/__init__.py
--rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)     4354 2024-04-24 14:01:21.000000 pyhgvsv-0.1.post1/src/pyhgvsv/models.py
--rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)     3970 2024-04-24 14:01:21.000000 pyhgvsv-0.1.post1/src/pyhgvsv/utils.py
--rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)    11661 2024-04-24 14:01:21.000000 pyhgvsv-0.1.post1/src/pyhgvsv/variants.py
-drwxrwxr-x   0 i9a5000   (1000) i9a5000   (1000)        0 2024-04-24 15:49:39.629853 pyhgvsv-0.1.post1/src/pyhgvsv.egg-info/
--rw-r--r--   0 i9a5000   (1000) i9a5000   (1000)     8864 2024-04-24 15:49:39.000000 pyhgvsv-0.1.post1/src/pyhgvsv.egg-info/PKG-INFO
--rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)      263 2024-04-24 15:49:39.000000 pyhgvsv-0.1.post1/src/pyhgvsv.egg-info/SOURCES.txt
--rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)        1 2024-04-24 15:49:39.000000 pyhgvsv-0.1.post1/src/pyhgvsv.egg-info/dependency_links.txt
--rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)        8 2024-04-24 15:49:39.000000 pyhgvsv-0.1.post1/src/pyhgvsv.egg-info/top_level.txt
+drwxrwxr-x   0 i9a5000   (1000) i9a5000   (1000)        0 2024-04-30 13:00:45.302464 pyhgvsv-0.2/
+-rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)     1100 2024-04-24 14:01:21.000000 pyhgvsv-0.2/LICENSE
+-rw-r--r--   0 i9a5000   (1000) i9a5000   (1000)     8858 2024-04-30 13:00:45.302464 pyhgvsv-0.2/PKG-INFO
+-rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)     8380 2024-04-24 15:43:44.000000 pyhgvsv-0.2/README.md
+-rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)      580 2024-04-30 13:00:20.000000 pyhgvsv-0.2/pyproject.toml
+-rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)       38 2024-04-30 13:00:45.302464 pyhgvsv-0.2/setup.cfg
+drwxrwxr-x   0 i9a5000   (1000) i9a5000   (1000)        0 2024-04-30 13:00:45.298464 pyhgvsv-0.2/src/
+drwxrwxr-x   0 i9a5000   (1000) i9a5000   (1000)        0 2024-04-30 13:00:45.302464 pyhgvsv-0.2/src/pyhgvsv/
+-rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)    50833 2024-04-24 18:53:44.000000 pyhgvsv-0.2/src/pyhgvsv/__init__.py
+-rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)     4354 2024-04-24 14:01:21.000000 pyhgvsv-0.2/src/pyhgvsv/models.py
+-rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)     4133 2024-04-29 18:52:11.000000 pyhgvsv-0.2/src/pyhgvsv/utils.py
+-rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)    11661 2024-04-24 14:01:21.000000 pyhgvsv-0.2/src/pyhgvsv/variants.py
+drwxrwxr-x   0 i9a5000   (1000) i9a5000   (1000)        0 2024-04-30 13:00:45.302464 pyhgvsv-0.2/src/pyhgvsv.egg-info/
+-rw-r--r--   0 i9a5000   (1000) i9a5000   (1000)     8858 2024-04-30 13:00:45.000000 pyhgvsv-0.2/src/pyhgvsv.egg-info/PKG-INFO
+-rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)      263 2024-04-30 13:00:45.000000 pyhgvsv-0.2/src/pyhgvsv.egg-info/SOURCES.txt
+-rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)        1 2024-04-30 13:00:45.000000 pyhgvsv-0.2/src/pyhgvsv.egg-info/dependency_links.txt
+-rw-rw-r--   0 i9a5000   (1000) i9a5000   (1000)        8 2024-04-30 13:00:45.000000 pyhgvsv-0.2/src/pyhgvsv.egg-info/top_level.txt
```

### Comparing `pyhgvsv-0.1.post1/LICENSE` & `pyhgvsv-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhgvsv-0.1.post1/PKG-INFO` & `pyhgvsv-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhgvsv
-Version: 0.1.post1
+Version: 0.2
 Summary: HGVS variant name parsing and generation with SV (structural variant) support
 Author-email: Parker Payne <parker.payne@bcm.edu>
 Project-URL: Homepage, https://github.com/parkerpayne/hgvsv
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.6
```

### Comparing `pyhgvsv-0.1.post1/README.md` & `pyhgvsv-0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyhgvsv-0.1.post1/pyproject.toml` & `pyhgvsv-0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyhgvsv"
-version = "0.1.post1"
+version = "0.2"
 authors = [
   { name="Parker Payne", email="parker.payne@bcm.edu" },
 ]
 description = "HGVS variant name parsing and generation with SV (structural variant) support"
 readme = "README.md"
 requires-python = ">=2.6"
 classifiers = [
```

### Comparing `pyhgvsv-0.1.post1/src/pyhgvsv/__init__.py` & `pyhgvsv-0.2/src/pyhgvsv/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1480,19 +1480,19 @@
     sv_length: Length of structural variant. Negative length denotes deletion, positive length denotes insertion.
     use_prefix: Include a transcript/gene/chromosome prefix in HGVS name.
     use_gene: Include gene name in HGVS prefix.
     max_allele_length: If allele is greater than this use allele length.
     """
     match sv_length:
         case sv_length if sv_length > 0:
-            ref = getbases(genome, chrom, offset-2, 1)
-            alt = getbases(genome, chrom, offset-2, 1) + alt
+            ref = getbases(genome, chrom, offset-1, 1)
+            alt = getbases(genome, chrom, offset-1, 1) + alt
         case sv_length if sv_length < 0:
-            ref = getbases(genome, chrom, offset-2, abs(sv_length)+1)
-            alt = getbases(genome, chrom, offset-2, 1)
+            ref = getbases(genome, chrom, offset-1, abs(sv_length)+1)
+            alt = getbases(genome, chrom, offset-1, 1)
         case default:
             pass
 
     hgvs = variant_to_hgvs_name(chrom, offset, ref, alt, genome, transcript,
                                 max_allele_length=max_allele_length,
                                 use_counsyl=use_counsyl)
     return hgvs.format(use_prefix=use_prefix, use_gene=use_gene,
```

### Comparing `pyhgvsv-0.1.post1/src/pyhgvsv/models.py` & `pyhgvsv-0.2/src/pyhgvsv/models.py`

 * *Files identical despite different names*

### Comparing `pyhgvsv-0.1.post1/src/pyhgvsv/utils.py` & `pyhgvsv-0.2/src/pyhgvsv/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,23 +65,28 @@
         }
 
 
 def make_transcript(transcript_json):
     """
     Make a Transcript form a JSON object.
     """
+    transcript_chrom = transcript_json['chrom']
+    if '_' in transcript_chrom:
+        patch = transcript_chrom.split('_')[-1]
+    else:
+        patch = ''
 
     transcript_name = transcript_json['id']
     if '.' in transcript_name:
         name, version = transcript_name.split('.')
     else:
         name, version = transcript_name, None
 
     transcript = Transcript(
-        name=name,
+        name=name+patch,
         version=int(version) if version is not None else None,
         gene=transcript_json['gene_name'],
         tx_position=Position(
             transcript_json['chrom'],
             transcript_json['start'],
             transcript_json['end'],
             transcript_json['strand'] == '+'),
```

### Comparing `pyhgvsv-0.1.post1/src/pyhgvsv/variants.py` & `pyhgvsv-0.2/src/pyhgvsv/variants.py`

 * *Files identical despite different names*

### Comparing `pyhgvsv-0.1.post1/src/pyhgvsv.egg-info/PKG-INFO` & `pyhgvsv-0.2/src/pyhgvsv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhgvsv
-Version: 0.1.post1
+Version: 0.2
 Summary: HGVS variant name parsing and generation with SV (structural variant) support
 Author-email: Parker Payne <parker.payne@bcm.edu>
 Project-URL: Homepage, https://github.com/parkerpayne/hgvsv
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.6
```

