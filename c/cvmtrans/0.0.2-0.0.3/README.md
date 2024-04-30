# Comparing `tmp/cvmtrans-0.0.2.tar.gz` & `tmp/cvmtrans-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvmtrans-0.0.2.tar", last modified: Tue Apr 30 07:22:39 2024, max compression
+gzip compressed data, was "cvmtrans-0.0.3.tar", last modified: Tue Apr 30 07:31:00 2024, max compression
```

## Comparing `cvmtrans-0.0.2.tar` & `cvmtrans-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2024-04-30 07:22:39.043439 cvmtrans-0.0.2/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     4807 2024-04-30 07:22:39.043327 cvmtrans-0.0.2/PKG-INFO
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     4058 2024-04-30 07:16:28.000000 cvmtrans-0.0.2/README.md
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2024-04-30 07:22:39.042356 cvmtrans-0.0.2/cvmtrans/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      297 2024-04-30 07:22:22.000000 cvmtrans-0.0.2/cvmtrans/__init__.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6571 2024-04-03 11:00:48.000000 cvmtrans-0.0.2/cvmtrans/cvmtrans.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     3719 2024-04-30 06:48:59.000000 cvmtrans-0.0.2/cvmtrans/cvmtrans_cut_tags.py
--rwx------   0 cuiqingpo   (501) staff       (20)     3539 2024-04-03 13:02:47.000000 cvmtrans-0.0.2/cvmtrans/cvmtrans_extract_reads.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      536 2024-04-03 12:21:00.000000 cvmtrans-0.0.2/cvmtrans/data_process.sh
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     4417 2024-04-03 03:57:33.000000 cvmtrans-0.0.2/cvmtrans/embl_parse.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     4689 2024-04-03 06:52:24.000000 cvmtrans-0.0.2/cvmtrans/embl_parse_test.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      152 2024-04-03 11:01:42.000000 cvmtrans-0.0.2/cvmtrans/gb2fa.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     3216 2024-04-03 03:02:06.000000 cvmtrans-0.0.2/cvmtrans/parse_bam.py
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2024-04-30 07:22:39.043153 cvmtrans-0.0.2/cvmtrans.egg-info/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     4807 2024-04-30 07:22:38.000000 cvmtrans-0.0.2/cvmtrans.egg-info/PKG-INFO
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      452 2024-04-30 07:22:38.000000 cvmtrans-0.0.2/cvmtrans.egg-info/SOURCES.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        1 2024-04-30 07:22:38.000000 cvmtrans-0.0.2/cvmtrans.egg-info/dependency_links.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      190 2024-04-30 07:22:38.000000 cvmtrans-0.0.2/cvmtrans.egg-info/entry_points.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       40 2024-04-30 07:22:38.000000 cvmtrans-0.0.2/cvmtrans.egg-info/requires.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        9 2024-04-30 07:22:38.000000 cvmtrans-0.0.2/cvmtrans.egg-info/top_level.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       85 2024-04-30 07:07:54.000000 cvmtrans-0.0.2/requirements.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       38 2024-04-30 07:22:39.043480 cvmtrans-0.0.2/setup.cfg
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2305 2024-04-30 07:22:18.000000 cvmtrans-0.0.2/setup.py
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2024-04-30 07:31:00.427434 cvmtrans-0.0.3/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     4807 2024-04-30 07:31:00.427281 cvmtrans-0.0.3/PKG-INFO
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     4058 2024-04-30 07:16:28.000000 cvmtrans-0.0.3/README.md
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2024-04-30 07:31:00.426005 cvmtrans-0.0.3/cvmtrans/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      297 2024-04-30 07:30:52.000000 cvmtrans-0.0.3/cvmtrans/__init__.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     8775 2024-04-08 10:09:38.000000 cvmtrans-0.0.3/cvmtrans/cvmtrans.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     3719 2024-04-30 06:48:59.000000 cvmtrans-0.0.3/cvmtrans/cvmtrans_cut_tags.py
+-rwx------   0 cuiqingpo   (501) staff       (20)     3539 2024-04-03 13:02:47.000000 cvmtrans-0.0.3/cvmtrans/cvmtrans_extract_reads.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      536 2024-04-03 12:21:00.000000 cvmtrans-0.0.3/cvmtrans/data_process.sh
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     4417 2024-04-03 03:57:33.000000 cvmtrans-0.0.3/cvmtrans/embl_parse.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     4689 2024-04-03 06:52:24.000000 cvmtrans-0.0.3/cvmtrans/embl_parse_test.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      152 2024-04-03 11:01:42.000000 cvmtrans-0.0.3/cvmtrans/gb2fa.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     3216 2024-04-03 03:02:06.000000 cvmtrans-0.0.3/cvmtrans/parse_bam.py
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2024-04-30 07:31:00.427056 cvmtrans-0.0.3/cvmtrans.egg-info/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     4807 2024-04-30 07:31:00.000000 cvmtrans-0.0.3/cvmtrans.egg-info/PKG-INFO
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      452 2024-04-30 07:31:00.000000 cvmtrans-0.0.3/cvmtrans.egg-info/SOURCES.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        1 2024-04-30 07:31:00.000000 cvmtrans-0.0.3/cvmtrans.egg-info/dependency_links.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      167 2024-04-30 07:31:00.000000 cvmtrans-0.0.3/cvmtrans.egg-info/entry_points.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       40 2024-04-30 07:31:00.000000 cvmtrans-0.0.3/cvmtrans.egg-info/requires.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        9 2024-04-30 07:31:00.000000 cvmtrans-0.0.3/cvmtrans.egg-info/top_level.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       85 2024-04-30 07:07:54.000000 cvmtrans-0.0.3/requirements.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       38 2024-04-30 07:31:00.427482 cvmtrans-0.0.3/setup.cfg
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2282 2024-04-30 07:30:47.000000 cvmtrans-0.0.3/setup.py
```

### Comparing `cvmtrans-0.0.2/PKG-INFO` & `cvmtrans-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvmtrans
-Version: 0.0.2
+Version: 0.0.3
 Summary: Transposon data process
 Home-page: https://github.com/hbucqp/cvmtrans
 Author: Qingpo Cui
 Author-email: cqp@cau.edu.cn
 License: MIT Licence
 Keywords: pip,transposon,transposon sequecing
 Platform: any
```

### Comparing `cvmtrans-0.0.2/README.md` & `cvmtrans-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cvmtrans-0.0.2/cvmtrans/cvmtrans.py` & `cvmtrans-0.0.3/cvmtrans/cvmtrans.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,17 +2,38 @@
 import os
 import re
 import sys
 import pysam
 import pandas as pd
 import numpy as np
 import tempfile
+import argparse
 from Bio import SeqIO
 
 
+def args_parse():
+    "Parse the input argument, use '-h' for help."
+    parser = argparse.ArgumentParser(
+        usage='cvmtrans -bam_file <sorted_bam_files> -embl_file <reference embl file> -output <tab delimited text file> \n\nAuthor: Qingpo Cui(SZQ Lab, China Agricultural University)\n')
+    # group = parser.add_mutually_exclusive_group(required=False)
+    parser.add_argument(
+        "-bam_file", help="<input_fastq>: output filename of the fastq file")
+    parser.add_argument(
+        "-embl_file", help="<input_file>: the tag sequence")
+    parser.add_argument(
+        "-output", help="<output_fastq>: output filename of the fastq file")
+
+    # parser.add_argument('-v', '--version', action='version',
+    #                     version='Version: ' + get_version("__init__.py"), help='<display version>')
+    if len(sys.argv) == 1:
+        parser.print_help(sys.stderr)
+        sys.exit(1)
+    return parser.parse_args()
+
+
 def bam2insdict(bamfile):
     """
     Genreate the insertion dictionary from bam files
     Paramters:
     ----------
     bamfile: str
         The sorted bam file of transposon sequencing data
@@ -112,86 +133,111 @@
         return feature.qualifiers["product"][0]
     elif "pseudo" in feature.qualifiers:
         return "pseudogene"
     else:
         return ""
 
 
-bamfile = pysam.AlignmentFile("1-18W_cuttags_2_sorted.bam", "rb")
-
-
-insert_read_counts = bam2insdict(bamfile)
-# print(insert_read_counts.keys())
-# print(len(read_counts))
-
-
-# parse embl file
-
-
-# Replace 'your_embl_file.embl' with the actual path to your EMBL file
-embl_file = 'H16SD2BY4_gxw.embl'
-
-
-cds_coordinates = cds_locations(embl_file)
-
-
-# output.write(
-#     'locus_tag\tgene_name\tncrna\tstart\tend\tstrand\tread_count\tins_count\tins_index\tproduct')
-
-records = SeqIO.parse(embl_file, 'embl')
-for record in records:
-    seq_id = record.id
-    if seq_id == '':
-        sys.exit(
-            "Could not find sequence name from your given embl file. Exiting ...")
-
-    # print(dir(record))
-    # Access information from the SeqRecord
-    # print(f"Accession: {record.id}")
-    # print(f"Description: {record.description}")
-    # print(f"Sequence length: {len(record.seq)}")
-    # ... other relevant information
+def get_insertion_stat(bam_file, embl_file, output):
+    """
+    Get insertion information from sorted bam files
 
-    # check if embl seq id in the insertion site dictionary
+    Parameters:
+    -----------
+    bam_file: str
+        The path of bam format file
+    embl_file: str
+        The path of the embl reference file
+    output: str
+        The output filename
+    """
+
+    # parse bamfile
+    bamfile = pysam.AlignmentFile(bam_file, "rb")
+    insert_read_counts = bam2insdict(bamfile)
+
+    # parse the embl file
+    embl_file = embl_file
+    cds_coordinates = cds_locations(embl_file)
+
+    # process the insertion sites
+    records = SeqIO.parse(embl_file, 'embl')
+    for record in records:
+        seq_id = record.id
+        if seq_id == '':
+            sys.exit(
+                "Could not find sequence name from your given embl file. Exiting ...")
+
+        # print(dir(record))
+        # Access information from the SeqRecord
+        # print(f"Accession: {record.id}")
+        # print(f"Description: {record.description}")
+        # print(f"Sequence length: {len(record.seq)}")
+        # ... other relevant information
+
+        # check if embl seq id in the insertion site dictionary
+
+        try:
+            insert_sites = insert_read_counts[record.id]
+        except:
+            sys.exit("Could not found the corresponding seq name %s in insertion dictionary, please check your embl file and make sure your mapping reference file has the same header with your embl file." % record.id)
+        with open(output, 'w') as out:
+            out.write(
+                'locus_tag\tgene_name\tncrna\tstart\tend\tstrand\tread_count\tins_count\tins_index\tproduct\n')
+            # Access features (e.g., CDS, gene, etc.)
+            for feature in record.features:
+                if feature.type == "gene" and not is_gene_within_cds(cds_coordinates, feature):
+                    continue
+                # if feature.type in ["CDS", "polypeptide", "gene"]: remove gene in order to delete duplicates annotation
+                if feature.type in ["CDS", "polypeptide"]:
+                    feature_id = get_feature_id(feature)
+                    gene_name = get_gene_name(feature)
+                    product_value = get_product_value(feature)
+                    rna_value = "1" if "ncRNA" in feature.qualifiers else "0"
+                    strand = feature.location.strand
+
+                    start = feature.location.start
+                    end = feature.location.end - 1
+                    feature_start = start + 1
+                    feature_end = end + 1
+                    # print(
+                    # f'{feature_id}\t{gene_name}\t{rna_value}\t{start}\t{end}\t{strand}\t{product_value}')
+
+                    # calculate the insert_count and the total reads in the corresponding insertion gene
+                    count = 0
+                    inserts = 0
+
+                    for j in np.arange(start, end + 1):
+                        if j in insert_sites.keys():
+                            # print(j)
+                            count += insert_sites[j]
+                            inserts += 1
+                    ins_index = inserts / \
+                        (end - start + 1) if end != start else 0
+                    #         count += sum(insert_sites[j])
+                    #         inserts += 1 if sum(insert_sites[j]) > 0 else 0
+                    # ins_index = inserts / \
+                    #     (end - start +
+                    #      1) if end != start else 0
+                    print(
+                        f'{feature_id}\t{gene_name}\t{rna_value}\t{feature_start}\t{feature_end}\t{strand}\t{count}\t{inserts}\t{ins_index}\t{product_value}')
+                    out.write(
+                        f'{feature_id}\t{gene_name}\t{rna_value}\t{feature_start}\t{feature_end}\t{strand}\t{count}\t{inserts}\t{ins_index}\t{product_value}\n')
+
+
+def main():
+    args = args_parse()
+    bamfile = os.path.abspath(args.bam_file)
+    emblfile = os.path.abspath(args.embl_file)
+    current_path = os.path.abspath(os.path.dirname(__file__))
+    output = args.output
 
-    try:
-        insert_sites = insert_read_counts[record.id]
-    except:
-        sys.exit("Could not found the corresponding seq name %s in insertion dictionary, please check your embl file and make sure your mapping reference file has the same header with your embl file." % record.id)
+    if re.search(r'[\/]', output):
+        sys.exit('Please check your output file name, do not give a PATH string')
+    else:
+        output = os.path.join(current_path, args.output)
 
-    # Access features (e.g., CDS, gene, etc.)
-    for feature in record.features:
-        if feature.type == "gene" and not is_gene_within_cds(cds_coordinates, feature):
-            continue
-        if feature.type in ["CDS", "polypeptide", "gene"]:
-            feature_id = get_feature_id(feature)
-            gene_name = get_gene_name(feature)
-            product_value = get_product_value(feature)
-            rna_value = "1" if "ncRNA" in feature.qualifiers else "0"
-            strand = feature.location.strand
+    get_insertion_stat(bamfile, emblfile, output)
 
-            start = feature.location.start
-            end = feature.location.end - 1
-            feature_start = start + 1
-            feature_end = end + 1
-            # print(
-            # f'{feature_id}\t{gene_name}\t{rna_value}\t{start}\t{end}\t{strand}\t{product_value}')
 
-            # calculate the insert_count and the total reads in the corresponding insertion gene
-            count = 0
-            inserts = 0
-
-            for j in np.arange(start, end + 1):
-                if j in insert_sites.keys():
-                    # print(j)
-                    count += insert_sites[j]
-                    inserts += 1
-            ins_index = inserts / (end - start + 1) if end != start else 0
-            #         count += sum(insert_sites[j])
-            #         inserts += 1 if sum(insert_sites[j]) > 0 else 0
-            # ins_index = inserts / \
-            #     (end - start +
-            #      1) if end != start else 0
-            print(
-                f'{feature_id}\t{gene_name}\t{rna_value}\t{feature_start}\t{feature_end}\t{strand}\t{count}\t{inserts}\t{ins_index}\t{product_value}')
-        # output.write(
-        #     f'{feature_id}\t{gene_name}\t{rna_value}\t{feature_start}\t{feature_end}\t{strand}\t{count}\t{inserts}\t{ins_index}\t{product_value}\n')
+if __name__ == '__main__':
+    main()
```

### Comparing `cvmtrans-0.0.2/cvmtrans/cvmtrans_cut_tags.py` & `cvmtrans-0.0.3/cvmtrans/cvmtrans_cut_tags.py`

 * *Files identical despite different names*

### Comparing `cvmtrans-0.0.2/cvmtrans/cvmtrans_extract_reads.py` & `cvmtrans-0.0.3/cvmtrans/cvmtrans_extract_reads.py`

 * *Files identical despite different names*

### Comparing `cvmtrans-0.0.2/cvmtrans/data_process.sh` & `cvmtrans-0.0.3/cvmtrans/data_process.sh`

 * *Files identical despite different names*

### Comparing `cvmtrans-0.0.2/cvmtrans/embl_parse.py` & `cvmtrans-0.0.3/cvmtrans/embl_parse.py`

 * *Files identical despite different names*

### Comparing `cvmtrans-0.0.2/cvmtrans/embl_parse_test.py` & `cvmtrans-0.0.3/cvmtrans/embl_parse_test.py`

 * *Files identical despite different names*

### Comparing `cvmtrans-0.0.2/cvmtrans/parse_bam.py` & `cvmtrans-0.0.3/cvmtrans/parse_bam.py`

 * *Files identical despite different names*

### Comparing `cvmtrans-0.0.2/cvmtrans.egg-info/PKG-INFO` & `cvmtrans-0.0.3/cvmtrans.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvmtrans
-Version: 0.0.2
+Version: 0.0.3
 Summary: Transposon data process
 Home-page: https://github.com/hbucqp/cvmtrans
 Author: Qingpo Cui
 Author-email: cqp@cau.edu.cn
 License: MIT Licence
 Keywords: pip,transposon,transposon sequecing
 Platform: any
```

### Comparing `cvmtrans-0.0.2/setup.py` & `cvmtrans-0.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,12 +61,12 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11'
     ],
     entry_points={
         'console_scripts': [
             'cvmtrans=cvmtrans.cvmtrans:main',
-            'cvmtrans_cut_tags=cvmtrans_cut_tags.cvmtrans_cut_tags:main',
-            'cvmtrans_extract_reads=cvmtrans_extract_reads.cvmtrans_extract_reads:main'
+            'cvmtrans_cut_tags=cvmtrans.cvmtrans_cut_tags:main',
+            'cvmtrans_extract_reads=cvmtrans.cvmtrans_extract_reads:main'
         ],
     },
 )
```

