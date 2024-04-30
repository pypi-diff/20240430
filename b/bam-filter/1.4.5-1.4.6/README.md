# Comparing `tmp/bam-filter-1.4.5.tar.gz` & `tmp/bam-filter-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bam-filter-1.4.5.tar", last modified: Tue Mar 26 16:22:57 2024, max compression
+gzip compressed data, was "bam-filter-1.4.6.tar", last modified: Tue Apr 30 13:07:24 2024, max compression
```

## Comparing `bam-filter-1.4.5.tar` & `bam-filter-1.4.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:22:57.291911 bam-filter-1.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-03-26 16:22:52.000000 bam-filter-1.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-26 16:22:52.000000 bam-filter-1.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-26 16:22:57.291911 bam-filter-1.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21415 2024-03-26 16:22:52.000000 bam-filter-1.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:22:57.291911 bam-filter-1.4.5/bam_filter/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-26 16:22:52.000000 bam-filter-1.4.5/bam_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-03-26 16:22:52.000000 bam-filter-1.4.5/bam_filter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-26 16:22:57.291911 bam-filter-1.4.5/bam_filter/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-03-26 16:22:52.000000 bam-filter-1.4.5/bam_filter/entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9535 2024-03-26 16:22:52.000000 bam-filter-1.4.5/bam_filter/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    23868 2024-03-26 16:22:52.000000 bam-filter-1.4.5/bam_filter/lca.py
--rw-r--r--   0 runner    (1001) docker     (127)    38887 2024-03-26 16:22:52.000000 bam-filter-1.4.5/bam_filter/reassign.py
--rw-r--r--   0 runner    (1001) docker     (127)    50137 2024-03-26 16:22:52.000000 bam-filter-1.4.5/bam_filter/sam_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    43631 2024-03-26 16:22:52.000000 bam-filter-1.4.5/bam_filter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:22:57.291911 bam-filter-1.4.5/bam_filter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-26 16:22:57.000000 bam-filter-1.4.5/bam_filter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-26 16:22:57.000000 bam-filter-1.4.5/bam_filter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 16:22:57.000000 bam-filter-1.4.5/bam_filter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-26 16:22:57.000000 bam-filter-1.4.5/bam_filter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-26 16:22:57.000000 bam-filter-1.4.5/bam_filter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-26 16:22:57.000000 bam-filter-1.4.5/bam_filter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-03-26 16:22:57.291911 bam-filter-1.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-26 16:22:52.000000 bam-filter-1.4.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    70238 2024-03-26 16:22:52.000000 bam-filter-1.4.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:07:24.536532 bam-filter-1.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-30 13:07:20.000000 bam-filter-1.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 13:07:20.000000 bam-filter-1.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-30 13:07:24.536532 bam-filter-1.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21540 2024-04-30 13:07:20.000000 bam-filter-1.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:07:24.536532 bam-filter-1.4.6/bam_filter/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-30 13:07:20.000000 bam-filter-1.4.6/bam_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-30 13:07:20.000000 bam-filter-1.4.6/bam_filter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-30 13:07:24.536532 bam-filter-1.4.6/bam_filter/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-04-30 13:07:20.000000 bam-filter-1.4.6/bam_filter/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-04-30 13:07:20.000000 bam-filter-1.4.6/bam_filter/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23868 2024-04-30 13:07:20.000000 bam-filter-1.4.6/bam_filter/lca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40437 2024-04-30 13:07:20.000000 bam-filter-1.4.6/bam_filter/reassign.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50203 2024-04-30 13:07:20.000000 bam-filter-1.4.6/bam_filter/sam_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44025 2024-04-30 13:07:20.000000 bam-filter-1.4.6/bam_filter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:07:24.536532 bam-filter-1.4.6/bam_filter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-30 13:07:24.000000 bam-filter-1.4.6/bam_filter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-30 13:07:24.000000 bam-filter-1.4.6/bam_filter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:07:24.000000 bam-filter-1.4.6/bam_filter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-30 13:07:24.000000 bam-filter-1.4.6/bam_filter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-30 13:07:24.000000 bam-filter-1.4.6/bam_filter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-30 13:07:24.000000 bam-filter-1.4.6/bam_filter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-30 13:07:24.536532 bam-filter-1.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-30 13:07:20.000000 bam-filter-1.4.6/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70238 2024-04-30 13:07:20.000000 bam-filter-1.4.6/versioneer.py
```

### Comparing `bam-filter-1.4.5/LICENSE` & `bam-filter-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bam-filter-1.4.5/README.md` & `bam-filter-1.4.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -89,19 +89,19 @@
 
 ## Read reassignment
 
 Full list of options:
 
 ```bash
 $ filterBAM reassign --help
-usage: filterBAM reassign [-h] --bam BAM [-p STR] [-r FILE] [-t INT] [-i INT] [-s FLOAT]
-                          [-A FLOAT] [-l INT] [-n INT] [--match-reward INT]
+usage: filterBAM reassign [-h] --bam BAM [-p STR] [-r FILE] [-t INT] [-i INT]
+                          [-s FLOAT] [-A FLOAT] [-l INT] [-n INT] [--match-reward INT]
                           [--mismatch-penalty INT] [--gap-open-penalty INT]
-                          [--gap-extension-penalty INT] [--lambda FLOAT] [-k FLOAT] [-o [FILE]]
-                          [-m STR] [-N] [--tmp-dir DIR]
+                          [--gap-extension-penalty INT] [--lambda FLOAT] [-k FLOAT]
+                          [-o [FILE]] [-m STR] [-N] [--tmp-dir DIR] [--disable-sort]
 
 optional arguments:
   -h, --help            show this help message and exit
   -p STR, --prefix STR  Prefix used for the output files (default: None)
   -r FILE, --reference-lengths FILE
                         File with references lengths (default: None)
   -t INT, --threads INT
@@ -128,18 +128,21 @@
   --gap-extension-penalty INT
                         Gap extension penalty for the alignment score (default: 2)
   --lambda FLOAT        Lambda parameter for the alignment score (default: 1.33)
   -k FLOAT              K parameter for the alignment score algorithm (default: 0.621)
   -o [FILE], --out-bam [FILE]
                         Save a BAM file without multimapping reads (default: None)
   -m STR, --sort-memory STR
-                        Set maximum memory per thread for sorting; suffix K/M/G recognized
-                        (default: 1G)
+                        Set maximum memory per thread for sorting; suffix K/M/G
+                        recognized (default: 1G)
   -N, --sort-by-name    Sort by read names (default: False)
   --tmp-dir DIR         Temporary directory (default: None)
+
+miscellaneous arguments:
+  --disable-sort        Disable sorting of the filtered BAM file (default: False)
 ```
 
 
 One would run filterBAM `reassign` as follows:
 
 ```bash
 filterBAM reassign --bam c55d4e2df1.dedup.bam  --threads 10 --iters 0 --min-read-ani 92 --reference-lengths gtdb-r202.len.map --out-bam c55d4e2df1.reassigned.bam
```

### Comparing `bam-filter-1.4.5/bam_filter/__main__.py` & `bam-filter-1.4.6/bam_filter/__main__.py`

 * *Files identical despite different names*

### Comparing `bam-filter-1.4.5/bam_filter/entropy.py` & `bam-filter-1.4.6/bam_filter/entropy.py`

 * *Files identical despite different names*

### Comparing `bam-filter-1.4.5/bam_filter/filter.py` & `bam-filter-1.4.6/bam_filter/filter.py`

 * *Files 8% similar despite different names*

```diff
@@ -89,14 +89,15 @@
         read_hits_count=args.read_hits_count,
         knee_plot=args.knee_plot,
         coverage_plots=args.coverage_plots,
         tmp_dir=tmp_dir,
         mode="filter",
     )
 
+    sorted_bam = args.bam.replace(".bam", ".bf-sorted.bam")
     bam = check_bam_file(
         bam=args.bam,
         threads=4,
         reference_lengths=args.reference_lengths,
         sort_memory=args.sort_memory,
     )
     if bam is None:
@@ -123,16 +124,17 @@
     )
     if args.low_memory:
         bam = out_files["bam_tmp_sorted"]
 
     logging.info("Reducing results to a single dataframe")
     # data = list(filter(None, data))
     data_df = [x[0] for x in data if x[0] is not None]
+    # remove empty dataframes
+    data_df = [x for x in data_df if not x.empty]
     data_df = concat_df(data_df)
-
     if args.read_length_freqs is not None:
         logging.info("Calculating read length frequencies...")
         lens = [x[1] for x in data if x[1] is not None]
         lens = json.dumps(lens, default=obj_dict, ensure_ascii=False, indent=4)
         with open(out_files["read_length_freqs"], "w", encoding="utf-8") as outfile:
             print(lens, file=outfile)
 
@@ -252,8 +254,16 @@
             disable_sort=args.disable_sort,
         )
     else:
         logging.info("Skipping filtering of reference BAM file.")
 
     if args.low_memory:
         os.remove(out_files["bam_tmp_sorted"])
+    # check if sorted BAM file exists, if yes remove it
+    if os.path.exists(sorted_bam):
+        os.remove(sorted_bam)
+    # check if sorted BAM index file exists, if yes remove it
+    if os.path.exists(sorted_bam + ".bai"):
+        os.remove(sorted_bam + ".bai")
+    elif os.path.exists(sorted_bam + ".csi"):
+        os.remove(sorted_bam + ".csi")
     logging.info("ALL DONE.")
```

### Comparing `bam-filter-1.4.5/bam_filter/lca.py` & `bam-filter-1.4.6/bam_filter/lca.py`

 * *Files identical despite different names*

### Comparing `bam-filter-1.4.5/bam_filter/reassign.py` & `bam-filter-1.4.6/bam_filter/reassign.py`

 * *Files 5% similar despite different names*

```diff
@@ -263,27 +263,29 @@
     out_files,
     threads,
     entries,
     sort_memory="1G",
     sort_by_name=False,
     min_read_ani=90,
     min_read_length=30,
+    disable_sort=False,
 ):
     # if out_files["bam_reassigned"] is not None:
     #     out_bam = out_files["bam_reassigned"]
     # else:
     #     out_bam = out_files["bam_reassigned_sorted"]
     out_bam = out_files["bam_reassigned"]
     if threads > 4:
         s_threads = 4
     else:
         s_threads = threads
     samfile = pysam.AlignmentFile(bam, "rb", threads=s_threads)
     references = list(entries.keys())
     refs_dict = {x: samfile.get_reference_length(x) for x in references}
+    # get group reads
     header = samfile.header
     samfile.close()
     (ref_names, ref_lengths) = zip(*refs_dict.items())
 
     refs_idx = {sys.intern(str(x)): i for i, x in enumerate(ref_names)}
     if threads > 4:
         write_threads = 4
@@ -292,14 +294,15 @@
 
     out_bam_file = pysam.AlignmentFile(
         out_files["bam_reassigned_tmp"],
         "wb",
         referencenames=list(ref_names),
         referencelengths=list(ref_lengths),
         threads=write_threads,
+        header=header,
     )
 
     # num_cores should be multiple of the write_threads
     num_cores = threads // write_threads
     # num_cores = min(threads, cpu_count())
     # batch_size = len(references) // num_cores + 1  # Ensure non-zero batch size
     # batch_size = calc_chunksize(n_workers=num_cores, len_iterable=len(references))
@@ -360,110 +363,114 @@
     out_bam_file.close()
     entries = None
     gc.collect()
     # prof.disable()
     # # print profiling output
     # stats = pstats.Stats(prof).strip_dirs().sort_stats("tottime")
     # stats.print_stats(5)  # top 10 rows
-    log.info("::: ::: Sorting BAM file...")
-    if threads > 4:
-        s_threads = 4
-    else:
-        s_threads = threads
-    if sort_by_name:
-        log.info("::: ::: Sorting by name...")
-        pysam.sort(
-            "-n",
-            "-@",
-            str(s_threads),
-            "-m",
-            str(sort_memory),
-            "-o",
-            out_bam,
-            out_files["bam_reassigned_tmp"],
-        )
-    else:
-        pysam.sort(
-            "-@",
-            str(s_threads),
-            "-m",
-            str(sort_memory),
-            "-o",
-            out_bam,
-            out_files["bam_reassigned_tmp"],
-        )
+    if not disable_sort:
+        log.info("::: ::: Sorting BAM file...")
+        if threads > 4:
+            s_threads = 4
+        else:
+            s_threads = threads
+        if sort_by_name:
+            log.info("::: ::: Sorting by name...")
+            pysam.sort(
+                "-n",
+                "-@",
+                str(s_threads),
+                "-m",
+                str(sort_memory),
+                "-o",
+                out_bam,
+                out_files["bam_reassigned_tmp"],
+            )
+        else:
+            pysam.sort(
+                "-@",
+                str(s_threads),
+                "-m",
+                str(sort_memory),
+                "-o",
+                out_bam,
+                out_files["bam_reassigned_tmp"],
+            )
 
-    logging.info("BAM index not found. Indexing...")
-    save = pysam.set_verbosity(0)
-    if threads > 4:
-        s_threads = 4
-    else:
-        s_threads = threads
-    samfile = pysam.AlignmentFile(out_bam, "rb", threads=s_threads)
-    chr_lengths = []
-    for chrom in samfile.references:
-        chr_lengths.append(samfile.get_reference_length(chrom))
-    max_chr_length = np.max(chr_lengths)
-    pysam.set_verbosity(save)
-    samfile.close()
+        logging.info("BAM index not found. Indexing...")
+        save = pysam.set_verbosity(0)
+        if threads > 4:
+            s_threads = 4
+        else:
+            s_threads = threads
+        samfile = pysam.AlignmentFile(out_bam, "rb", threads=s_threads)
+        chr_lengths = []
+        for chrom in samfile.references:
+            chr_lengths.append(samfile.get_reference_length(chrom))
+        max_chr_length = np.max(chr_lengths)
+        pysam.set_verbosity(save)
+        samfile.close()
+
+        if max_chr_length > 536870912:
+            logging.info("A reference is longer than 2^29, indexing with csi")
+            pysam.index(
+                "-c",
+                "-@",
+                str(threads),
+                out_bam,
+            )
+        else:
+            pysam.index(
+                "-@",
+                str(threads),
+                out_bam,
+            )
 
-    if max_chr_length > 536870912:
-        logging.info("A reference is longer than 2^29, indexing with csi")
-        pysam.index(
-            "-c",
-            "-@",
-            str(threads),
-            out_bam,
-        )
+        os.remove(out_files["bam_reassigned_tmp"])
     else:
-        pysam.index(
-            "-@",
-            str(threads),
-            out_bam,
-        )
-
-    os.remove(out_files["bam_reassigned_tmp"])
+        logging.info("Skipping BAM file sorting...")
+        os.rename(out_files["bam_reassigned_tmp"], out_bam)
 
 
 # def calculate_alignment_score(identity, read_length):
 #     return (identity / math.log(read_length)) * math.sqrt(read_length)
 
 # Values from:
 # https://www.ncbi.nlm.nih.gov/IEB/ToolBox/CPP_DOC/lxr/source/src/algo/blast/core/blast_stat.c
 # def calculate_alignment_score(
-#         num_matches, 
-#         num_mismatches, 
-#         num_gaps, 
-#         gap_extensions, 
+#         num_matches,
+#         num_mismatches,
+#         num_gaps,
+#         gap_extensions,
 #         match_reward,
-#         mismatch_penalty, 
-#         gap_open_penalty, 
-#         gap_extension_penalty, 
-#         lambda_value, 
+#         mismatch_penalty,
+#         gap_open_penalty,
+#         gap_extension_penalty,
+#         lambda_value,
 #         K_value
 #     ):
 #     # Calculate the raw alignment score
 #     S = (num_matches * match_reward) - (num_mismatches * mismatch_penalty) - (num_gaps * gap_open_penalty) - (gap_extensions * gap_extension_penalty)
 
 #     # Calculate the approximate bit score
 #     bit_score = (lambda_value * S - math.log(K_value)) / math.log(2)
 
 #     return bit_score
 
 # def get_bam_data(
-#         parms, 
+#         parms,
 #         ref_lengths=None,
-#         percid=90, 
-#         min_read_length=30, 
-#         threads=1, 
-#         match_reward=1, 
-#         mismatch_penalty=-1, 
-#         gap_open_penalty=1, 
-#         gap_extension_penalty=2, 
-#         lambda_value=1.02, 
+#         percid=90,
+#         min_read_length=30,
+#         threads=1,
+#         match_reward=1,
+#         mismatch_penalty=-1,
+#         gap_open_penalty=1,
+#         gap_extension_penalty=2,
+#         lambda_value=1.02,
 #         K_value=0.21
 #     ):
 #     bam, references = parms
 #     dt.options.progress.enabled = False
 #     dt.options.progress.clear_on_success = True
 #     if threads > 1:
 #         dt.options.nthreads = threads - 1
@@ -530,46 +537,52 @@
 #             results.append(dt.Frame())
 #             empty_df += 1
 #     samfile.close()
 #     return (dt.rbind(results), reads, refs, empty_df)
 
 
 def calculate_alignment_score(
-        num_matches, 
-        num_mismatches, 
-        num_gaps, 
-        gap_extensions, 
-        match_reward,
-        mismatch_penalty, 
-        gap_open_penalty, 
-        gap_extension_penalty, 
-        precomputed_factor, # This is lambda_value * match_reward / math.log(2)
-        precomputed_log_K # This is math.log(K_value) / math.log(2)
-    ):
+    num_matches,
+    num_mismatches,
+    num_gaps,
+    gap_extensions,
+    match_reward,
+    mismatch_penalty,
+    gap_open_penalty,
+    gap_extension_penalty,
+    precomputed_factor,  # This is lambda_value * match_reward / math.log(2)
+    precomputed_log_K,  # This is math.log(K_value) / math.log(2)
+):
     # Calculate the raw alignment score with reduced arithmetic operations
-    S = (num_matches * match_reward) - (num_mismatches * mismatch_penalty) - (num_gaps * gap_open_penalty) - (gap_extensions * gap_extension_penalty)
+    S = (
+        (num_matches * match_reward)
+        - (num_mismatches * mismatch_penalty)
+        - (num_gaps * gap_open_penalty)
+        - (gap_extensions * gap_extension_penalty)
+    )
 
     # Use precomputed factors to calculate the approximate bit score
     bit_score = precomputed_factor * S - precomputed_log_K
 
     return bit_score
 
+
 def get_bam_data(
-        parms, 
-        ref_lengths=None,
-        percid=90, 
-        min_read_length=30, 
-        threads=1, 
-        match_reward=1, 
-        mismatch_penalty=-1, 
-        gap_open_penalty=1, 
-        gap_extension_penalty=2, 
-        lambda_value=1.02, 
-        K_value=0.21
-    ):
+    parms,
+    ref_lengths=None,
+    percid=90,
+    min_read_length=30,
+    threads=1,
+    match_reward=1,
+    mismatch_penalty=-1,
+    gap_open_penalty=1,
+    gap_extension_penalty=2,
+    lambda_value=1.02,
+    K_value=0.21,
+):
     # Precompute factors for the score calculation to avoid redundant computation
     precomputed_factor = lambda_value * match_reward / math.log(2)
     precomputed_log_K = math.log(K_value) / math.log(2)
 
     bam, references = parms
     dt.options.progress.enabled = False
     dt.options.progress.clear_on_success = True
@@ -579,45 +592,74 @@
 
     results = []
     reads = set()
     refs = set()
     empty_df = 0
 
     for reference in references:
-        reference_length = int(samfile.get_reference_length(reference)) if ref_lengths is None else int(ref_lengths[reference])
+        reference_length = (
+            int(samfile.get_reference_length(reference))
+            if ref_lengths is None
+            else int(ref_lengths[reference])
+        )
         aln_data = []
-        for aln in samfile.fetch(contig=reference, multiple_iterators=False, until_eof=True):
-            query_length = aln.query_length if aln.query_length != 0 else aln.infer_query_length()
+        for aln in samfile.fetch(
+            contig=reference, multiple_iterators=False, until_eof=True
+        ):
+            query_length = (
+                aln.query_length if aln.query_length != 0 else aln.infer_query_length()
+            )
 
             if query_length >= min_read_length:
                 num_mismatches = aln.get_tag("NM")
                 pident = (1 - (num_mismatches / query_length)) * 100
                 if pident >= percid:
                     num_matches = query_length - num_mismatches
                     num_gaps = aln.get_tag("XO") if aln.has_tag("XO") else 0
                     gap_extensions = aln.get_tag("XG") if aln.has_tag("XG") else 0
 
-                    bit_score = calculate_alignment_score(num_matches, num_mismatches, num_gaps, gap_extensions, match_reward, mismatch_penalty, gap_open_penalty, gap_extension_penalty, precomputed_factor, precomputed_log_K)
-                    aln_data.append((aln.query_name, aln.reference_name, bit_score, reference_length))
+                    bit_score = calculate_alignment_score(
+                        num_matches,
+                        num_mismatches,
+                        num_gaps,
+                        gap_extensions,
+                        match_reward,
+                        mismatch_penalty,
+                        gap_open_penalty,
+                        gap_extension_penalty,
+                        precomputed_factor,
+                        precomputed_log_K,
+                    )
+                    aln_data.append(
+                        (
+                            aln.query_name,
+                            aln.reference_name,
+                            bit_score,
+                            reference_length,
+                        )
+                    )
                     reads.add(aln.query_name)
                     refs.add(aln.reference_name)
-        
+
         if aln_data:
-            aln_data_dt = dt.Frame(aln_data, names=["queryId", "subjectId", "bitScore", "slen"])
+            aln_data_dt = dt.Frame(
+                aln_data, names=["queryId", "subjectId", "bitScore", "slen"]
+            )
             aln_data_dt = aln_data_dt[
                 :1, :, dt.by(dt.f.queryId, dt.f.subjectId), dt.sort(-dt.f.bitScore)
             ]
             results.append(aln_data_dt)
         else:
             empty_df += 1
 
     samfile.close()
     combined_results = dt.rbind(results)
     return (combined_results, reads, refs, empty_df)
 
+
 def reassign_reads(
     bam,
     out_files,
     match_reward,
     mismatch_penalty,
     gap_open_penalty,
     gap_extension_penalty,
@@ -628,14 +670,15 @@
     min_read_count=1,
     min_read_ani=90,
     min_read_length=30,
     reassign_iters=25,
     reassign_scale=0.9,
     sort_memory="4G",
     sort_by_name=False,
+    disable_sort=False,
 ):
     dt.options.progress.enabled = True
     dt.options.progress.clear_on_success = True
     if threads > 1:
         dt.options.nthreads = threads - 1
     else:
         dt.options.nthreads = 1
@@ -714,15 +757,14 @@
                         match_reward=match_reward,
                         mismatch_penalty=mismatch_penalty,
                         gap_open_penalty=gap_open_penalty,
                         gap_extension_penalty=gap_extension_penalty,
                         lambda_value=lambda_value,
                         K_value=K_value,
                         threads=4,
-
                     ),
                     parms,
                     chunksize=1,
                 ),
                 total=len(parms),
                 leave=False,
                 ncols=80,
@@ -744,15 +786,14 @@
                         match_reward=match_reward,
                         mismatch_penalty=mismatch_penalty,
                         gap_open_penalty=gap_open_penalty,
                         gap_extension_penalty=gap_extension_penalty,
                         lambda_value=lambda_value,
                         K_value=K_value,
                         threads=4,
-
                     ),
                     parms,
                     chunksize=1,
                 ),
                 total=len(parms),
                 leave=False,
                 ncols=80,
@@ -865,63 +906,66 @@
     #     n_alns_0 += x.shape[0]
     #     del x["queryId"]
     #     del x["subjectId"]
     #     x = x[:, [dt.f.qidx, dt.f.sidx, dt.f.var, dt.f.slen]].to_numpy()
     #     # Substitute the original DataFrame with the joined version in the list
     #     data[i] = x
 
-
     # Calculate the total number of rows in advance
-    total_rows = sum(x.shape[0] for x in data)  # This assumes `data` is a list of DataFrames/NumPy arrays
+    total_rows = sum(
+        x.shape[0] for x in data
+    )  # This assumes `data` is a list of DataFrames/NumPy arrays
 
     # Assuming all `x` arrays have the same number of columns after processing, use the first one to determine this
     # IMPORTANT: This line needs to be executed before the loop and assumes all `x` arrays are similar after processing
     num_columns = 4  # Adjust based on your actual data structure
 
     # Preallocate the NumPy array
-    mat = np.empty((total_rows, num_columns), dtype=np.float32)  # Adjust dtype as necessary
+    mat = np.empty(
+        (total_rows, num_columns), dtype=np.float32
+    )  # Adjust dtype as necessary
 
     current_index = 0
     for i, x in tqdm.tqdm(
         enumerate(data),
         total=len(data),
         desc="Processing batches",
         unit="batch",
         disable=is_debug(),
         leave=False,
         ncols=80,
     ):
         # Perform join with reads and then refs
-        if x.shape[0] > 0:   
+        if x.shape[0] > 0:
             x = x[:, :, dt.join(reads)]
             x = x[:, :, dt.join(refs)]
             n_alns_0 += x.shape[0]
-            
+
             # Process `x` as before, but directly update `mat`
-            x_processed = x[:, [dt.f.qidx, dt.f.sidx, dt.f.bitScore, dt.f.slen]].to_numpy()
+            x_processed = x[
+                :, [dt.f.qidx, dt.f.sidx, dt.f.bitScore, dt.f.slen]
+            ].to_numpy()
             num_rows = x_processed.shape[0]
-            
+
             # Fill the preallocated array
-            mat[current_index:current_index + num_rows, :] = x_processed
-            
+            mat[current_index : current_index + num_rows, :] = x_processed
+
             # Update the current index
             current_index += num_rows
 
     # After the loop, `mat` is already the concatenated array, so there's no need for further concatenation or conversion.
     data = None  # Free the memory if `data` is no longer needed
 
     # Log the final stats
     n_reads_0 = reads.shape[0]
     n_refs_0 = refs.shape[0]
     log.info(
         f"::: References: {n_refs_0:,} | Reads: {n_reads_0:,} | Alignments: {n_alns_0:,}"
     )
 
-
-
     # After the loop, use dt.rbind() to combine all the DataFrames in the list
     # data = dt.rbind([x for x in data])
 
     # del data["queryId"]
     # del data["subjectId"]
     # n_alns_0 = data.shape[0]
     # n_reads_0 = reads.shape[0]
@@ -958,35 +1002,38 @@
 
     # # Convert the unstructured array to structured array
     # m = rf.unstructured_to_structured(m, dtype)
     # gc.collect()
 
     log.info("::: Allocating data...")
 
-
     # Define the dtype for the structured array
-    dtype = np.dtype([
-        ("source", "int"),
-        ("subject", "int"),
-        ("var", "float"),
-        ("slen", "int"),
-        ("s_W", "float"),  # This and following fields are initialized to 0 or a default value
-        ("prob", "float"),
-        ("iter", "int"),
-        ("n_aln", "int"),
-        ("max_prob", "float"),
-    ])
+    dtype = np.dtype(
+        [
+            ("source", "int"),
+            ("subject", "int"),
+            ("var", "float"),
+            ("slen", "int"),
+            (
+                "s_W",
+                "float",
+            ),  # This and following fields are initialized to 0 or a default value
+            ("prob", "float"),
+            ("iter", "int"),
+            ("n_aln", "int"),
+            ("max_prob", "float"),
+        ]
+    )
 
     # Initialize the structured array with zeros directly
     m = np.zeros(mat.shape[0], dtype=dtype)
-    m['source'] = mat[:, 0]
-    m['subject'] = mat[:, 1]
-    m['var'] = mat[:, 2]
-    m['slen'] = mat[:, 3]
-
+    m["source"] = mat[:, 0]
+    m["subject"] = mat[:, 1]
+    m["var"] = mat[:, 2]
+    m["slen"] = mat[:, 3]
 
     # Force a garbage collection to free up memory from any intermediate arrays that are no longer needed
     gc.collect()
 
     log.info("::: Initializing data structures...")
     init_data = initialize_subject_weights(m)
     if reassign_iters > 0:
@@ -1064,14 +1111,15 @@
         bam=bam,
         ref_counts=references_m,
         out_files=out_files,
         threads=threads,
         entries=entries,
         sort_memory=sort_memory,
         min_read_ani=min_read_ani,
+        disable_sort=disable_sort,
     )
 
 
 def reassign(args):
     logging.basicConfig(
         level=logging.DEBUG,
         format="%(levelname)s ::: %(asctime)s ::: %(message)s",
@@ -1085,14 +1133,15 @@
     out_files = create_output_files(
         prefix=args.prefix,
         bam=args.bam,
         tmp_dir=tmp_dir,
         mode="reassign",
         bam_reassigned=args.bam_reassigned,
     )
+    sorted_bam = bam.replace(".bam", ".bf-sorted.bam")
     bam = check_bam_file(
         bam=args.bam,
         threads=args.threads,
         reference_lengths=args.reference_lengths,
         sort_memory=args.sort_memory,
     )
     if bam is None:
@@ -1123,9 +1172,18 @@
         out_files=out_files,
         match_reward=args.match_reward,
         mismatch_penalty=args.mismatch_penalty,
         gap_open_penalty=args.gap_open_penalty,
         gap_extension_penalty=args.gap_extension_penalty,
         lambda_value=args.lambda_value,
         K_value=args.K_value,
+        disable_sort=args.disable_sort,
     )
+    # check if sorted BAM file exists, if yes remove it
+    if os.path.exists(sorted_bam):
+        os.remove(sorted_bam)
+    # check if sorted BAM index file exists, if yes remove it
+    if os.path.exists(sorted_bam + ".bai"):
+        os.remove(sorted_bam + ".bai")
+    elif os.path.exists(sorted_bam + ".csi"):
+        os.remove(sorted_bam + ".csi")
     log.info("Done!")
```

### Comparing `bam-filter-1.4.5/bam_filter/sam_utils.py` & `bam-filter-1.4.6/bam_filter/sam_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,16 @@
     logging.info("::: Writing temporary filtered BAM file... (be patient)")
     if threads > 4:
         s_threads = 4
     else:
         s_threads = threads
     samfile = pysam.AlignmentFile(bam, "rb", threads=s_threads)
     header = samfile.header
+    # get read groups
+
     if threads > 4:
         threads = 4
 
     # convert the dictionary to an array
     refs_dict = dict(zip(samfile.references, samfile.lengths))
     my_array = np.array(list(refs_dict.items()))
 
@@ -132,15 +134,17 @@
 
     logging.info("::: ::: BAM index not found. Indexing...")
     save = pysam.set_verbosity(0)
     if threads > 4:
         s_threads = 4
     else:
         s_threads = threads
-    samfile = pysam.AlignmentFile(output_files["bam_tmp_sorted"], "rb", threads=s_threads)
+    samfile = pysam.AlignmentFile(
+        output_files["bam_tmp_sorted"], "rb", threads=s_threads
+    )
     chr_lengths = []
     for chrom in samfile.references:
         chr_lengths.append(samfile.get_reference_length(chrom))
     max_chr_length = np.max(chr_lengths)
     pysam.set_verbosity(save)
     samfile.close()
 
@@ -266,15 +270,14 @@
     # prof.enable()
     bam, references = params
     results = []
 
     if threads > 4:
         threads = 4
     samfile = pysam.AlignmentFile(bam, "rb", threads=threads)
-
     read_hits = defaultdict(int)
     for reference in references:
         edit_distances = []
         # edit_distances_md = []
         ani_nm = []
         # ani_md = []
         read_length = []
@@ -540,14 +543,15 @@
     # # print profiling output
     # stats = pstats.Stats(prof).strip_dirs().sort_stats("tottime")
     # stats.print_stats(5)  # top 10 rows
     # exit()
     # results = [x[0] for x in results if x[0] is not None]
     results = list(filter(None, results))
     data_df = pd.DataFrame([x.to_summary() for x in results])
+
     # read_hits = (
     #     pd.DataFrame.from_dict(read_hits, orient="index", columns=["count"])
     #     .rename_axis("read_id")
     #     .reset_index()
     # )
     if read_length_freqs:
         read_lens = [x.get_read_length_freqs() for x in results]
@@ -1012,15 +1016,14 @@
                     ),
                     total=len(ref_chunks),
                     leave=False,
                     ncols=80,
                     desc="References processed",
                 )
             )
-
             p.close()
             p.join()
 
     except KeyboardInterrupt:
         logging.info("User canceled the operation. Terminating jobs.")
         p.terminate()
         p.join()
@@ -1163,15 +1166,14 @@
             if threads > 4:
                 s_threads = 4
             else:
                 s_threads = threads
             samfile = pysam.AlignmentFile(bam, "rb", threads=s_threads)
             refs_dict = {x: samfile.get_reference_length(x) for x in references}
             header = samfile.header
-
             (ref_names, ref_lengths) = zip(*refs_dict.items())
             ref_dict_m = {
                 chrom.contig: chrom.mapped
                 for chrom in samfile.get_index_statistics()
                 if chrom.contig in ref_names
             }
             samfile.close()
@@ -1183,14 +1185,15 @@
 
             out_bam_file = pysam.AlignmentFile(
                 out_files["bam_filtered_tmp"],
                 "wb",
                 referencenames=list(ref_names),
                 referencelengths=list(ref_lengths),
                 threads=write_threads,
+                header=header,
             )
 
             # logging.info(
             #     f"::: Filtering {len(references):,} references sequentially..."
             # )
             # for reference in tqdm.tqdm(
             #     references,
```

### Comparing `bam-filter-1.4.5/bam_filter/utils.py` & `bam-filter-1.4.6/bam_filter/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,18 @@
     if tmpdir is None:
         tmpdir = tempfile.TemporaryDirectory(dir=os.getcwd())
     else:
         if not os.path.exists(tmpdir):
             log.error(f"Temporary directory {tmpdir} does not exist")
             exit(1)
         tmpdir = tempfile.TemporaryDirectory(dir=os.path.abspath(tmpdir))
+        # Check if tmpdir has more than 107 characters
+        if len(tmpdir.name) > 107:
+            log.error(f"Temporary directory {tmpdir.name} has more than 107 characters")
+            exit(1)
     return tmpdir
 
 
 def is_debug():
     return logging.getLogger("my_logger").getEffectiveLevel() == logging.DEBUG
 
 
@@ -80,24 +84,24 @@
     # Remove empty chunks
     chunks = [chunk for chunk in chunks if chunk]
 
     return chunks
 
 
 def sort_keys_by_approx_weight(
-    input_dict, scale=1, num_cores=1, refinement_steps=10,verbose=False
+    input_dict, scale=1, num_cores=1, refinement_steps=10, verbose=False
 ):
     if scale == 0:
         raise ValueError("Scale cannot be zero.")
 
     # Calculate the target weight for each chunk
     target_weight = scale * int(max(input_dict.values()))
 
     # Determine the initial number of chunks based on the number of cores
-    #num_chunks = num_cores * scale
+    # num_chunks = num_cores * scale
     num_chunks = (((sum(input_dict.values()) // target_weight)) // num_cores) + 1
     if num_chunks < num_cores:
         num_chunks = num_cores
     # Sort keys by their weights in descending order
     sorted_keys = sorted(input_dict, key=lambda k: input_dict[k], reverse=True)
 
     # Initialize chunks
@@ -573,14 +577,15 @@
     # createdb_required_args = parser_createdb.add_argument_group("required arguments")
     # reassign_required_args = parser_reassign.add_argument_group(
     #     "Re-assign required arguments"
     # )
     reassign_optional_args = parser_reassign.add_argument_group(
         "Re-assign optional arguments"
     )
+    misc_reassign_args = parser_reassign.add_argument_group("miscellaneous arguments")
 
     filter_required_args = parser_filter.add_argument_group("Filter required arguments")
     # filter_optional_args = parser_filter.add_argument_group("Filter optional arguments")
 
     # lca_required_args = parser_lca.add_argument_group("LCA required arguments")
     lca_optional_args = parser_lca.add_argument_group("LCA optional arguments")
 
@@ -717,29 +722,25 @@
         metavar="INT",
         dest="gap_extension_penalty",
         help=help_msg["reassign_gap_extension_penalty"],
     )
     reassign_optional_args.add_argument(
         "--lambda",
         type=lambda x: float(
-            check_values(
-                x, minval=0, maxval=np.Inf, parser=parser, var="--lambda"
-            )
+            check_values(x, minval=0, maxval=np.Inf, parser=parser, var="--lambda")
         ),
         default=defaults["reassign_lambda"],
         metavar="FLOAT",
         dest="lambda_value",
         help=help_msg["reassign_lambda"],
     )
     reassign_optional_args.add_argument(
         "-k",
         type=lambda x: float(
-            check_values(
-                x, minval=0, maxval=np.Inf, parser=parser, var="-K"
-            )
+            check_values(x, minval=0, maxval=np.Inf, parser=parser, var="-K")
         ),
         default=defaults["reassign_k"],
         metavar="FLOAT",
         dest="K_value",
         help=help_msg["reassign_k"],
     )
     reassign_optional_args.add_argument(
@@ -773,14 +774,20 @@
         "--tmp-dir",
         type=str,
         default=defaults["tmp_dir"],
         metavar="DIR",
         dest="tmp_dir",
         help=help_msg["tmp_dir"],
     )
+    misc_reassign_args.add_argument(
+        "--disable-sort",
+        dest="disable_sort",
+        action="store_true",
+        help=help_msg["disable_sort"],
+    )
     misc_filter_args.add_argument(
         "--reference-trim-length",
         type=lambda x: int(
             check_values(
                 x, minval=0, maxval=10000, parser=parser, var="---reference-trim-length"
             )
         ),
```

### Comparing `bam-filter-1.4.5/setup.cfg` & `bam-filter-1.4.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `bam-filter-1.4.5/setup.py` & `bam-filter-1.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `bam-filter-1.4.5/versioneer.py` & `bam-filter-1.4.6/versioneer.py`

 * *Files identical despite different names*

