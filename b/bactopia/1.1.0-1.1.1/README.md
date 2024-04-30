# Comparing `tmp/bactopia-1.1.0.tar.gz` & `tmp/bactopia-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bactopia-1.1.0.tar", max compression
+gzip compressed data, was "bactopia-1.1.1.tar", max compression
```

## Comparing `bactopia-1.1.0.tar` & `bactopia-1.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1065 2024-04-25 18:34:53.309856 bactopia-1.1.0/LICENSE
--rw-r--r--   0        0        0    35126 2024-04-25 18:34:53.309856 bactopia-1.1.0/README.md
--rw-r--r--   0        0        0      113 2024-04-25 18:34:53.309856 bactopia-1.1.0/bactopia/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 18:34:53.309856 bactopia-1.1.0/bactopia/cli/__init__.py
--rw-r--r--   0        0        0     4738 2024-04-25 18:34:53.309856 bactopia-1.1.0/bactopia/cli/atb_formatter.py
--rw-r--r--   0        0        0     2667 2024-04-25 18:34:53.309856 bactopia-1.1.0/bactopia/cli/citations.py
--rw-r--r--   0        0        0     5118 2024-04-25 18:34:53.309856 bactopia-1.1.0/bactopia/cli/datasets.py
--rw-r--r--   0        0        0    19587 2024-04-25 18:34:53.309856 bactopia-1.1.0/bactopia/cli/download.py
--rw-r--r--   0        0        0     2416 2024-04-25 18:34:53.309856 bactopia-1.1.0/bactopia/cli/jsonify.py
--rw-r--r--   0        0        0    19701 2024-04-25 18:34:53.309856 bactopia-1.1.0/bactopia/cli/prepare.py
--rw-r--r--   0        0        0    20195 2024-04-25 18:34:53.309856 bactopia-1.1.0/bactopia/cli/search.py
--rw-r--r--   0        0        0    16657 2024-04-25 18:34:53.309856 bactopia-1.1.0/bactopia/cli/summary.py
--rw-r--r--   0        0        0     5716 2024-04-25 18:34:53.309856 bactopia-1.1.0/bactopia/cli/update.py
--rw-r--r--   0        0        0     1388 2024-04-25 18:34:53.309856 bactopia-1.1.0/bactopia/parse.py
--rw-r--r--   0        0        0      267 2024-04-25 18:34:53.309856 bactopia-1.1.0/bactopia/parsers/__init__.py
--rw-r--r--   0        0        0      408 2024-04-25 18:34:53.309856 bactopia-1.1.0/bactopia/parsers/amrfinderplus.py
--rw-r--r--   0        0        0     1000 2024-04-25 18:34:53.313856 bactopia-1.1.0/bactopia/parsers/annotator.py
--rw-r--r--   0        0        0     2783 2024-04-25 18:34:53.313856 bactopia-1.1.0/bactopia/parsers/ariba.py
--rw-r--r--   0        0        0      664 2024-04-25 18:34:53.313856 bactopia-1.1.0/bactopia/parsers/assembler.py
--rw-r--r--   0        0        0     4673 2024-04-25 18:34:53.313856 bactopia-1.1.0/bactopia/parsers/blast.py
--rw-r--r--   0        0        0     1365 2024-04-25 18:34:53.313856 bactopia-1.1.0/bactopia/parsers/error.py
--rw-r--r--   0        0        0      372 2024-04-25 18:34:53.313856 bactopia-1.1.0/bactopia/parsers/gather.py
--rw-r--r--   0        0        0     1492 2024-04-25 18:34:53.313856 bactopia-1.1.0/bactopia/parsers/generic.py
--rw-r--r--   0        0        0     2683 2024-04-25 18:34:53.313856 bactopia-1.1.0/bactopia/parsers/mapping.py
--rw-r--r--   0        0        0      640 2024-04-25 18:34:53.313856 bactopia-1.1.0/bactopia/parsers/mlst.py
--rw-r--r--   0        0        0     1763 2024-04-25 18:34:53.313856 bactopia-1.1.0/bactopia/parsers/parsables.py
--rw-r--r--   0        0        0     3093 2024-04-25 18:34:53.313856 bactopia-1.1.0/bactopia/parsers/qc.py
--rw-r--r--   0        0        0     5014 2024-04-25 18:34:53.313856 bactopia-1.1.0/bactopia/parsers/sketcher.py
--rw-r--r--   0        0        0     2574 2024-04-25 18:34:53.313856 bactopia-1.1.0/bactopia/parsers/variants.py
--rw-r--r--   0        0        0      874 2024-04-25 18:34:53.313856 bactopia-1.1.0/bactopia/parsers/versions.py
--rw-r--r--   0        0        0     5292 2024-04-25 18:34:53.313856 bactopia-1.1.0/bactopia/summary.py
--rw-r--r--   0        0        0     4496 2024-04-25 18:34:53.313856 bactopia-1.1.0/bactopia/utils.py
--rw-r--r--   0        0        0     1138 2024-04-25 18:34:53.313856 bactopia-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    36972 1970-01-01 00:00:00.000000 bactopia-1.1.0/setup.py
--rw-r--r--   0        0        0    36040 1970-01-01 00:00:00.000000 bactopia-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-30 16:21:08.286363 bactopia-1.1.1/LICENSE
+-rw-r--r--   0        0        0    35312 2024-04-30 16:21:08.286363 bactopia-1.1.1/README.md
+-rw-r--r--   0        0        0      113 2024-04-30 16:21:08.286363 bactopia-1.1.1/bactopia/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 16:21:08.286363 bactopia-1.1.1/bactopia/cli/__init__.py
+-rw-r--r--   0        0        0     5050 2024-04-30 16:21:08.286363 bactopia-1.1.1/bactopia/cli/atb_formatter.py
+-rw-r--r--   0        0        0     2667 2024-04-30 16:21:08.286363 bactopia-1.1.1/bactopia/cli/citations.py
+-rw-r--r--   0        0        0     5118 2024-04-30 16:21:08.286363 bactopia-1.1.1/bactopia/cli/datasets.py
+-rw-r--r--   0        0        0    19587 2024-04-30 16:21:08.286363 bactopia-1.1.1/bactopia/cli/download.py
+-rw-r--r--   0        0        0     2416 2024-04-30 16:21:08.286363 bactopia-1.1.1/bactopia/cli/jsonify.py
+-rw-r--r--   0        0        0    19701 2024-04-30 16:21:08.286363 bactopia-1.1.1/bactopia/cli/prepare.py
+-rw-r--r--   0        0        0    20195 2024-04-30 16:21:08.286363 bactopia-1.1.1/bactopia/cli/search.py
+-rw-r--r--   0        0        0    16654 2024-04-30 16:21:08.286363 bactopia-1.1.1/bactopia/cli/summary.py
+-rw-r--r--   0        0        0     5716 2024-04-30 16:21:08.286363 bactopia-1.1.1/bactopia/cli/update.py
+-rw-r--r--   0        0        0     1388 2024-04-30 16:21:08.286363 bactopia-1.1.1/bactopia/parse.py
+-rw-r--r--   0        0        0      267 2024-04-30 16:21:08.286363 bactopia-1.1.1/bactopia/parsers/__init__.py
+-rw-r--r--   0        0        0      408 2024-04-30 16:21:08.286363 bactopia-1.1.1/bactopia/parsers/amrfinderplus.py
+-rw-r--r--   0        0        0     1330 2024-04-30 16:21:08.286363 bactopia-1.1.1/bactopia/parsers/annotator.py
+-rw-r--r--   0        0        0     2783 2024-04-30 16:21:08.286363 bactopia-1.1.1/bactopia/parsers/ariba.py
+-rw-r--r--   0        0        0      664 2024-04-30 16:21:08.290362 bactopia-1.1.1/bactopia/parsers/assembler.py
+-rw-r--r--   0        0        0     4673 2024-04-30 16:21:08.290362 bactopia-1.1.1/bactopia/parsers/blast.py
+-rw-r--r--   0        0        0     1365 2024-04-30 16:21:08.290362 bactopia-1.1.1/bactopia/parsers/error.py
+-rw-r--r--   0        0        0      372 2024-04-30 16:21:08.290362 bactopia-1.1.1/bactopia/parsers/gather.py
+-rw-r--r--   0        0        0     1492 2024-04-30 16:21:08.290362 bactopia-1.1.1/bactopia/parsers/generic.py
+-rw-r--r--   0        0        0     2683 2024-04-30 16:21:08.290362 bactopia-1.1.1/bactopia/parsers/mapping.py
+-rw-r--r--   0        0        0      640 2024-04-30 16:21:08.290362 bactopia-1.1.1/bactopia/parsers/mlst.py
+-rw-r--r--   0        0        0     2583 2024-04-30 16:21:08.290362 bactopia-1.1.1/bactopia/parsers/parsables.py
+-rw-r--r--   0        0        0     3093 2024-04-30 16:21:08.290362 bactopia-1.1.1/bactopia/parsers/qc.py
+-rw-r--r--   0        0        0     5014 2024-04-30 16:21:08.290362 bactopia-1.1.1/bactopia/parsers/sketcher.py
+-rw-r--r--   0        0        0     2574 2024-04-30 16:21:08.290362 bactopia-1.1.1/bactopia/parsers/variants.py
+-rw-r--r--   0        0        0      874 2024-04-30 16:21:08.290362 bactopia-1.1.1/bactopia/parsers/versions.py
+-rw-r--r--   0        0        0     5292 2024-04-30 16:21:08.290362 bactopia-1.1.1/bactopia/summary.py
+-rw-r--r--   0        0        0     4496 2024-04-30 16:21:08.290362 bactopia-1.1.1/bactopia/utils.py
+-rw-r--r--   0        0        0     1138 2024-04-30 16:21:08.290362 bactopia-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    37160 1970-01-01 00:00:00.000000 bactopia-1.1.1/setup.py
+-rw-r--r--   0        0        0    36226 1970-01-01 00:00:00.000000 bactopia-1.1.1/PKG-INFO
```

### Comparing `bactopia-1.1.0/LICENSE` & `bactopia-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bactopia-1.1.0/README.md` & `bactopia-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -296,14 +296,16 @@
 │ --bactopia-dir  -b  TEXT            The path you would like to place bactopia        │
 │                                     structure                                        │
 │                                     [default: bactopia]                              │
 │ --publish-mode  -m  [symlink|copy]  Designates plascement of assemblies will be      │
 │                                     handled                                          │
 │                                     [default: symlink]                               │
 │ --recursive     -r                  Traverse recursively through provided path       │
+│ --extension     -e  TEXT            The extension of the assemblies e.g .fa,.fa.gz   │
+│                                     [default: .fa]                                   │
 ╰──────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Additional Options ─────────────────────────────────────────────────────────────────╮
 │ --verbose        Increase the verbosity of output                                    │
 │ --silent         Only critical errors will be printed                                │
 │ --version  -V    Show the version and exit.                                          │
 │ --help           Show this message and exit.                                         │
 ╰──────────────────────────────────────────────────────────────────────────────────────╯
```

### Comparing `bactopia-1.1.0/bactopia/cli/atb_formatter.py` & `bactopia-1.1.1/bactopia/cli/atb_formatter.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         {"name": "Required Options", "options": ["--path"]},
         {
             "name": "Bactopia Directory Structure Options",
             "options": [
                 "--bactopia-dir",
                 "--publish-mode",
                 "--recursive",
+                "--extension",
             ],
         },
         {
             "name": "Additional Options",
             "options": [
                 "--verbose",
                 "--silent",
@@ -55,24 +56,27 @@
     # Make remaining subdirectories (which will be empty)
     Path(f"{bactopia_dir}/{sample}/main").mkdir(parents=True, exist_ok=True)
     Path(f"{bactopia_dir}/{sample}/main/gather").mkdir(parents=True, exist_ok=True)
     Path(f"{bactopia_dir}/{sample}/main/assembler").mkdir(parents=True, exist_ok=True)
 
     # Write the meta.tsv file
     logging.debug(f"Writing {sample}-meta.tsv")
+    is_compressed = "true" if str(assembly).endswith(".gz") else "false"
     with open(f"{bactopia_dir}/{sample}/main/gather/{sample}-meta.tsv", "w") as meta_fh:
         meta_fh.write(
             "sample\truntype\toriginal_runtype\tis_paired\tis_compressed\tspecies\tgenome_size\n"
         )
         meta_fh.write(
-            f"{sample}\tassembly_accession\tassembly_accession\tfalse\tfalse\null\0\n"
+            f"{sample}\tassembly_accession\tassembly_accession\tfalse\t{is_compressed}\tnull\t0\n"
         )
 
     # Write the assembly file
     final_assembly = f"{bactopia_dir}/{sample}/main/assembler/{sample}.fna"
+    if is_compressed:
+        final_assembly = f"{final_assembly}.gz"
     final_assembly_path = Path(final_assembly)
     if publish_mode == "symlink":
         logging.debug(f"Creating symlink of {assembly} at {final_assembly}")
         final_assembly_path.symlink_to(assembly)
     else:
         logging.debug(f"Copying {assembly} to {final_assembly}")
         shutil.copyfile(assembly, final_assembly)
@@ -97,22 +101,30 @@
     "-m",
     default="symlink",
     show_default=True,
     type=click.Choice(["symlink", "copy"], case_sensitive=False),
     help="Designates plascement of assemblies will be handled",
 )
 @click.option(
+    "--extension",
+    "-e",
+    default=".fa",
+    show_default=True,
+    help="The extension of the FASTA files",
+)
+@click.option(
     "--recursive", "-r", is_flag=True, help="Traverse recursively through provided path"
 )
 @click.option("--verbose", is_flag=True, help="Increase the verbosity of output")
 @click.option("--silent", is_flag=True, help="Only critical errors will be printed")
 def atb_formatter(
     path,
     bactopia_dir,
     publish_mode,
+    extension,
     recursive,
     verbose,
     silent,
 ):
     """Restructure All-the-Bacteria assemblies to allow usage with Bactopia Tools"""
     # Setup logs
     logging.basicConfig(
@@ -123,23 +135,22 @@
         ],
     )
     logging.getLogger().setLevel(
         logging.ERROR if silent else logging.DEBUG if verbose else logging.INFO
     )
 
     abspath = Path(path).absolute()
-    fasta_ext = ".fa"
 
     # Match Assemblies
     count = 0
     logging.info(
         "Setting up Bactopia directory structure (use --verbose to see more details)"
     )
-    for fasta in search_path(abspath, f"*{fasta_ext}", recursive=recursive):
-        fasta_name = fasta.name.replace(fasta_ext, "")
+    for fasta in search_path(abspath, f"*{extension}", recursive=recursive):
+        fasta_name = fasta.name.replace(extension, "")
         create_sample_directory(fasta_name, fasta, bactopia_dir, publish_mode)
         count += 1
     logging.info(f"Bactopia directory structure created at {bactopia_dir}")
     logging.info(f"Total assemblies processed: {count}")
 
 
 def main():
```

### Comparing `bactopia-1.1.0/bactopia/cli/citations.py` & `bactopia-1.1.1/bactopia/cli/citations.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.1.0/bactopia/cli/datasets.py` & `bactopia-1.1.1/bactopia/cli/datasets.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.1.0/bactopia/cli/download.py` & `bactopia-1.1.1/bactopia/cli/download.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.1.0/bactopia/cli/jsonify.py` & `bactopia-1.1.1/bactopia/cli/jsonify.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.1.0/bactopia/cli/prepare.py` & `bactopia-1.1.1/bactopia/cli/prepare.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.1.0/bactopia/cli/search.py` & `bactopia-1.1.1/bactopia/cli/search.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.1.0/bactopia/cli/summary.py` & `bactopia-1.1.1/bactopia/cli/summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -400,22 +400,22 @@
                         rank, reason = process_sample(df, RANK_CUTOFF)
                         processed_samples[sample["id"]] = True
                         df["rank"] = rank
                         df["reason"] = reason
                         dfs.append(df)
                         logging.debug(f"\tRank: {rank} ({reason})")
                     else:
-                        logging.debug(
+                        logging.info(
                             f"Skipping {sample['id']} ({sample['path']}) due to missing files. Missing:"
                         )
                         for missing_file in parsable_files:
-                            logging.debug(f"\t{missing_file}")
+                            logging.info(f"\t{missing_file}")
                         increment_and_append("ignore-unknown", sample["id"])
             else:
-                logging.debug(
+                logging.info(
                     f"Skipping {sample['id']} ({sample['path']}), incomplete or not a Bactopia directory"
                 )
                 increment_and_append("ignore-unknown", sample["id"])
     if dfs:
         final_df = pd.concat(dfs)
         for col in EXCLUDE_COLUMNS:
             if col in final_df.columns:
```

### Comparing `bactopia-1.1.0/bactopia/cli/update.py` & `bactopia-1.1.1/bactopia/cli/update.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.1.0/bactopia/parse.py` & `bactopia-1.1.1/bactopia/parse.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.1.0/bactopia/parsers/annotator.py` & `bactopia-1.1.1/bactopia/parsers/annotator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,64 @@
 """
 Parsers for Annotation related results.
 """
+BAKTA_METADATA = [
+    "tRNAs",
+    "tmRNAs",
+    "rRNAs",
+    "ncRNAs",
+    "ncRNA regions",
+    "CRISPR arrays",
+    "CDSs",
+    "pseudogenes",
+    "hypotheticals",
+    "signal peptides",
+    "sORFs",
+    "gaps",
+    "oriCs",
+    "oriVs",
+    "oriTs",
+]
+PROKKA_METADATA = [
+    "CDS",
+    "rRNA",
+    "tRNA",
+]
 
 
 def parse(path: str, name: str) -> dict:
     """
     Parse basic annotation information from Prokka and Bakta
 
     Args:
         path (str): input file to be parsed
         name (str): the name of the sample
 
     Returns:
         dict: parsed results
     """
-    if "prokka" in str(path):
-        return _parse_prokka_annotation(path, name)
-    # else:
-    #    return _parse_bakta_annotation(path)
+    return _parse_annotation(path, name)
 
 
-def _parse_prokka_annotation(path: str, name: str) -> dict:
+def _parse_annotation(path: str, name: str) -> dict:
     """
-    Parse Prokka summary text file.
+    Parse Prokka or Bakta summary text file.
 
     Args:
-        filename (str): input file to be parsed
+        path (str): input file to be parsed
+        name (str): the name of the sample
 
     Returns:
         dict: the parsed Prokka summary
     """
+    COLS = PROKKA_METADATA if "prokka" in path else BAKTA_METADATA
     results = {
         "sample": name,
     }
     with open(path, "rt") as fh:
         for line in fh:
             line = line.rstrip()
-            key, val = line.split(":")
-            if key not in ["organism", "contigs", "bases"]:
-                results[f"annotator_total_{key}"] = int(val.lstrip())
+            if ":" in line:
+                key, val = line.split(":")
+                if key in COLS:
+                    results[f"annotator_total_{key}"] = int(val.lstrip())
     return results
```

### Comparing `bactopia-1.1.0/bactopia/parsers/ariba.py` & `bactopia-1.1.1/bactopia/parsers/ariba.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.1.0/bactopia/parsers/assembler.py` & `bactopia-1.1.1/bactopia/parsers/assembler.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.1.0/bactopia/parsers/blast.py` & `bactopia-1.1.1/bactopia/parsers/blast.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.1.0/bactopia/parsers/error.py` & `bactopia-1.1.1/bactopia/parsers/error.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.1.0/bactopia/parsers/generic.py` & `bactopia-1.1.1/bactopia/parsers/generic.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.1.0/bactopia/parsers/mapping.py` & `bactopia-1.1.1/bactopia/parsers/mapping.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.1.0/bactopia/parsers/mlst.py` & `bactopia-1.1.1/bactopia/parsers/mlst.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.1.0/bactopia/parsers/qc.py` & `bactopia-1.1.1/bactopia/parsers/qc.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.1.0/bactopia/parsers/sketcher.py` & `bactopia-1.1.1/bactopia/parsers/sketcher.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.1.0/bactopia/parsers/variants.py` & `bactopia-1.1.1/bactopia/parsers/variants.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.1.0/bactopia/parsers/versions.py` & `bactopia-1.1.1/bactopia/parsers/versions.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.1.0/bactopia/summary.py` & `bactopia-1.1.1/bactopia/summary.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.1.0/bactopia/utils.py` & `bactopia-1.1.1/bactopia/utils.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.1.0/pyproject.toml` & `bactopia-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bactopia"
-version = "1.1.0"
+version = "1.1.1"
 description = "A Python package for working with Bactopia"
 authors = [
     "Robert A. Petit III <robbie.petit@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://bactopia.github.io/"
```

### Comparing `bactopia-1.1.0/setup.py` & `bactopia-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,17 +22,17 @@
                      'bactopia-prepare = bactopia.cli.prepare:main',
                      'bactopia-search = bactopia.cli.search:main',
                      'bactopia-summary = bactopia.cli.summary:main',
                      'bactopia-update = bactopia.cli.update:main']}
 
 setup_kwargs = {
     'name': 'bactopia',
-    'version': '1.1.0',
+    'version': '1.1.1',
     'description': 'A Python package for working with Bactopia',
-    'long_description': "[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-908a85?logo=gitpod)](https://gitpod.io/#https://github.com/bactopia/bactopia-py)\n\n![Bactopia Logo](https://raw.githubusercontent.com/bactopia/bactopia/master/data/bactopia-logo.png)\n\n# bactopia-py\nA Python package for working with [Bactopia](https://bactopia.github.io/)\n\n## Bactopia Subcommands\n\nThere are many subcommands available in Bactopia. Here is a brief description of each command:\n\n| Command              | Description                                                                |\n|----------------------|----------------------------------------------------------------------------|\n| `bactopia-citations` | Print out tools and citations used throughout Bactopia                     |\n| `bactopia-datasets`  | Download optional datasets to supplement your analyses with Bactopia       |\n| `bactopia-download`  | Builds Bactopia environments for use with Nextflow.                        |\n| `bactopia-prepare`   | Create a 'file of filenames' (FOFN) of samples to be processed by Bactopia |\n| `bactopia-search`    | Query against ENA and SRA for public accessions to process with Bactopia   |\n| `bactopia-summary`   | Generate a summary table from the Bactopia results.                        |\n\nBelow is the `--help` output for each subcommand.\n\n### `bactopia-citations`\n\n```{bash}\n Usage: bactopia-citations [OPTIONS]\n\n Print out tools and citations used throughout Bactopia\n\n╭─ Options ────────────────────────────────────────────────────────────────────────────╮\n│    --version        -V        Show the version and exit.                             │\n│ *  --bactopia-path  -b  TEXT  Directory where Bactopia repository is stored          │\n│                               [required]                                             │\n│    --name           -n  TEXT  Only print citation matching a given name              │\n│    --plain-text     -p        Disable rich formatting                                │\n│    --help                     Show this message and exit.                            │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n### `bactopia-datasets`\n\n```{bash}\n Usage: bactopia-datasets [OPTIONS] [UNKNOWN]...\n\n Download optional datasets to supplement your analyses with Bactopia\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --bactopia-path    TEXT  Directory where Bactopia repository is stored [required] │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Download Related Options ───────────────────────────────────────────────────────────╮\n│ --datasets_cache    TEXT     Base directory to download datasets to (Defaults to env │\n│                              variable BACTOPIA_CACHEDIR, a subfolder called datasets │\n│                              will be created)                                        │\n│                              [default: ${HOME}/.bactopia]                 │\n│ --force                      Force overwrite of existing pre-built environments.     │\n│ --max_retry         INTEGER  Maximum times to attempt creating Conda environment.    │\n│                              (Default: 3)                                            │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --verbose      Print debug related text.                                             │\n│ --silent       Only critical errors will be printed.                                 │\n│ --version      Show the version and exit.                                            │\n│ --help         Show this message and exit.                                           │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n\n```\n\n### `bactopia-download`\n\n```{bash}\n Usage: bactopia-download [OPTIONS] [UNKNOWN]...\n\n Builds Bactopia environments for use with Nextflow.\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --bactopia-path    TEXT  Directory where Bactopia results are stored [required]   │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Build Related Options ──────────────────────────────────────────────────────────────╮\n│ --envtype                     [conda|docker|singularity|  The type of environment to │\n│                               all]                        build.                     │\n│                                                           [default: conda]           │\n│ --wf                          TEXT                        Build a environment for a  │\n│                                                           the given workflow         │\n│                                                           [default: bactopia]        │\n│ --condadir                    TEXT                        Directory to create Conda  │\n│                                                           environments               │\n│                                                           (NXF_CONDA_CACHEDIR env    │\n│                                                           variable takes precedence) │\n│ --use_conda                                               Use Conda for building     │\n│                                                           Conda environments instead │\n│                                                           of Mamba                   │\n│ --singularity_cache           TEXT                        Directory to download      │\n│                                                           Singularity images         │\n│                                                           (NXF_SINGULARITY_CACHEDIR  │\n│                                                           env variable takes         │\n│                                                           precedence)                │\n│ --singularity_pull_docker…                                Force conversion of Docker │\n│                                                           containers, instead        │\n│                                                           downloading Singularity    │\n│                                                           images directly            │\n│ --force_rebuild                                           Force overwrite of         │\n│                                                           existing pre-built         │\n│                                                           environments.              │\n│ --max_retry                   INTEGER                     Maximum times to attempt   │\n│                                                           creating Conda             │\n│                                                           environment. (Default: 3)  │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --verbose      Print debug related text.                                             │\n│ --silent       Only critical errors will be printed.                                 │\n│ --version      Show the version and exit.                                            │\n│ --help         Show this message and exit.                                           │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Options ────────────────────────────────────────────────────────────────────────────╮\n│ --build-all         Builds all environments for Bactopia workflows                   │\n│ --build-nfcore      Builds all nf-core related environments                          │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n### `bactopia-prepare`\n\n```{bash}\n Usage: bactopia-prepare [OPTIONS]\n\n Create a 'file of filenames' (FOFN) of samples to be processed by Bactopia\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --path  -p  TEXT  Directory where FASTQ files are stored [required]               │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Matching Options ───────────────────────────────────────────────────────────────────╮\n│ --assembly-ext     -a  TEXT  Extension of the FASTA assemblies [default: .fna.gz]    │\n│ --fastq-ext        -f  TEXT  Extension of the FASTQs [default: .fastq.gz]            │\n│ --fastq-separator      TEXT  Split FASTQ name on the last occurrence of the          │\n│                              separator                                               │\n│                              [default: _]                                            │\n│ --pe1-pattern          TEXT  Designates difference first set of paired-end reads     │\n│                              [default: [Aa]|[Rr]1|1]                                 │\n│ --pe2-pattern          TEXT  Designates difference second set of paired-end reads    │\n│                              [default: [Bb]|[Rr]2|2]                                 │\n│ --merge                      Flag samples with multiple read sets to be merged by    │\n│                              Bactopia                                                │\n│ --ont                        Single-end reads should be treated as Oxford Nanopore   │\n│                              reads                                                   │\n│ --recursive        -r        Directories will be traversed recursively               │\n│ --prefix               TEXT  Prefix to add to the path                               │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Sample Information Options ─────────────────────────────────────────────────────────╮\n│ --metadata             TEXT     Metadata per sample with genome size and species     │\n│                                 information                                          │\n│ --genome-size  -gsize  INTEGER  Genome size to use for all samples                   │\n│ --species      -s      TEXT     Species to use for all samples (If available, can be │\n│                                 used to determine genome size)                       │\n│ --taxid                TEXT     Use the genome size of the Taxon ID for all samples  │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --examples        Print example usage                                                │\n│ --verbose         Increase the verbosity of output                                   │\n│ --silent          Only critical errors will be printed                               │\n│ --version   -V    Show the version and exit.                                         │\n│ --help            Show this message and exit.                                        │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n### `bactopia-search`\n\n```{bash}\n Usage: bactopia-search [OPTIONS]\n\n Query against ENA and SRA for public accessions to process with Bactopia\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --query  -q  TEXT  Taxon ID or Study, BioSample, or Run accession (can also be    │\n│                       comma separated or a file of accessions)                       │\n│                       [required]                                                     │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Query Options ──────────────────────────────────────────────────────────────────────╮\n│ --exact-taxon                     Exclude Taxon ID descendants                       │\n│ --limit             -l   INTEGER  Maximum number of results (per query) to return    │\n│                                   [default: 1000000]                                 │\n│ --accession-limit   -al  INTEGER  Maximum number of accessions to query at once      │\n│                                   [default: 5000]                                    │\n│ --biosample-subset       INTEGER  If a BioSample has multiple Experiments, maximum   │\n│                                   number to randomly select (0 = disabled)           │\n│                                   [default: 0]                                       │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Filtering Options ──────────────────────────────────────────────────────────────────╮\n│ --min-base-count   -mbc  INTEGER  Filters samples based on minimum base pair count   │\n│                                   (0 = disabled)                                     │\n│                                   [default: 0]                                       │\n│ --min-read-length  -mrl  INTEGER  Filters samples based on minimum mean read length  │\n│                                   (0 = disabled)                                     │\n│                                   [default: 0]                                       │\n│ --min-coverage     -mc   INTEGER  Filter samples based on minimum coverage (requires │\n│                                   --genome_size, 0 = disabled)                       │\n│                                   [default: 0]                                       │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --genome-size  -gsize  INTEGER  Genome size to be used for all samples, and for      │\n│                                 calculating min coverage                             │\n│                                 [default: 0]                                         │\n│ --outdir       -o      TEXT     Directory to write output [default: ./]              │\n│ --prefix       -p      TEXT     Prefix to use for output file names                  │\n│                                 [default: bactopia]                                  │\n│ --force                         Overwrite existing reports                           │\n│ --verbose                       Increase the verbosity of output                     │\n│ --silent                        Only critical errors will be printed                 │\n│ --version      -V               Show the version and exit.                           │\n│ --help                          Show this message and exit.                          │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n### `bactopia-summary`\n\n```{bash}\n Usage: bactopia-summary [OPTIONS]\n\n Generate a summary table from the Bactopia results.\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --bactopia-path  -b  TEXT  Directory where Bactopia results are stored [required] │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Gold Cutoffs ───────────────────────────────────────────────────────────────────────╮\n│ --gold-coverage     -gcov      INTEGER  Minimum amount of coverage required for Gold │\n│                                         status                                       │\n│                                         [default: 100]                               │\n│ --gold-quality      -gqual     INTEGER  Minimum per-read mean quality score required │\n│                                         for Gold status                              │\n│                                         [default: 30]                                │\n│ --gold-read-length  -glen      INTEGER  Minimum mean read length required for Gold   │\n│                                         status                                       │\n│                                         [default: 95]                                │\n│ --gold-contigs      -gcontigs  INTEGER  Maximum contig count required for Gold       │\n│                                         status                                       │\n│                                         [default: 100]                               │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Silver Cutoffs ─────────────────────────────────────────────────────────────────────╮\n│ --silver-coverage     -scov      INTEGER  Minimum amount of coverage required for    │\n│                                           Silver status                              │\n│                                           [default: 50]                              │\n│ --silver-quality      -squal     INTEGER  Minimum per-read mean quality score        │\n│                                           required for Silver status                 │\n│                                           [default: 20]                              │\n│ --silver-read-length  -slen      INTEGER  Minimum mean read length required for      │\n│                                           Silver status                              │\n│                                           [default: 75]                              │\n│ --silver-contigs      -scontigs  INTEGER  Maximum contig count required for Silver   │\n│                                           status                                     │\n│                                           [default: 200]                             │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Fail Cutoffs ───────────────────────────────────────────────────────────────────────╮\n│ --min-coverage        -mincov   INTEGER  Minimum amount of coverage required to pass │\n│                                          [default: 20]                               │\n│ --min-quality         -minqual  INTEGER  Minimum per-read mean quality score         │\n│                                          required to pass                            │\n│                                          [default: 12]                               │\n│ --min-read-length     -minlen   INTEGER  Minimum mean read length required to pass   │\n│                                          [default: 49]                               │\n│ --max-contigs                   INTEGER  Maximum contig count required to pass       │\n│                                          [default: 500]                              │\n│ --min-assembled-size            INTEGER  Minimum assembled genome size               │\n│ --max-assembled-size            INTEGER  Maximum assembled genome size               │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --outdir   -o  PATH  Directory to write output [default: ./]                         │\n│ --prefix   -p  TEXT  Prefix to use for output files [default: bactopia]              │\n│ --force              Overwrite existing reports                                      │\n│ --verbose            Increase the verbosity of output                                │\n│ --silent             Only critical errors will be printed                            │\n│ --version  -V        Show the version and exit.                                      │\n│ --help               Show this message and exit.                                     │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n# All The Bacteria (ATB)\n\nThe [AllTheBacteria](https://www.biorxiv.org/content/10.1101/2024.03.08.584059v1) is a collection\nof nearly 2,000,000 bacterial genomes. Using available FASTQ files from the European Nucleotide\nArchive (ENA) and Sequence Read Archive (SRA), the genomes were assembled using [Shovill] and made\npublicly available from the [Iqbal Lab](https://github.com/iqbal-lab-org/AllTheBacteria).\n\nTo make it easy to utilize [Bactopia Tools](https://bactopia.github.io/latest/bactopia-tools/) with\nassemblies from AllTheBacteria, `bactopia-atb-formatter` was created. This tool will create a \ndirectory structure that resembles output from an actual Bactopia run.\n\n### `bactopia-atb-formatter`\n\n```{bash}\n Usage: bactopia-atb-formatter [OPTIONS]\n\n Restructure All-the-Bacteria assemblies to allow usage with Bactopia Tools\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --path  -p  TEXT  Directory where FASTQ files are stored [required]               │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Bactopia Directory Structure Options ───────────────────────────────────────────────╮\n│ --bactopia-dir  -b  TEXT            The path you would like to place bactopia        │\n│                                     structure                                        │\n│                                     [default: bactopia]                              │\n│ --publish-mode  -m  [symlink|copy]  Designates plascement of assemblies will be      │\n│                                     handled                                          │\n│                                     [default: symlink]                               │\n│ --recursive     -r                  Traverse recursively through provided path       │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --verbose        Increase the verbosity of output                                    │\n│ --silent         Only critical errors will be printed                                │\n│ --version  -V    Show the version and exit.                                          │\n│ --help           Show this message and exit.                                         │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n### Example Usage for _Legionella pneumophila_\n\nTo demonstrate the usage of `bactopia-atb-formatter`, we will use assemblies for\n_Legionella pneumophila_. The following steps will download the assemblies, build the\nBactopia directory structure, and then run [legsta](https://github.com/tseemann/legsta)\nvia the [Bactopia Tool](https://bactopia.github.io/latest/bactopia-tools/legsta/).\n\n#### Download the Assemblies\n\nFirst will download the _Legionella pneumophila_ assemblies from AllTheBacteria. After downloading\nwe will extract them into a folder called `legionella-assemblies`. Within this folder, there will be\nsubdirectories for each tarball that was downloaded.\n\n```{bash}\nmkdir atb-legionella\ncd atb-legionella\n\n# Download the assemblies\nwget https://ftp.ebi.ac.uk/pub/databases/AllTheBacteria/Releases/0.1/assembly/legionella_pneumophila__01.asm.tar.xz\nwget https://ftp.ebi.ac.uk/pub/databases/AllTheBacteria/Releases/0.1/assembly/legionella_pneumophila__02.asm.tar.xz\n\n# Extract the assemblies\nmkdir legionella-assemblies\ntar -C legionella-assemblies -xJf legionella_pneumophila__01.asm.tar.xz\ntar -C legionella-assemblies -xJf legionella_pneumophila__02.asm.tar.xz\n```\n\n#### Create the Bactopia Directory Structure\n\nWith the assemblies extracted, we can now create the Bactopia directory structure using\n`bactopia-atb-formatter`. Once complete, each assembly will have its own folder created\nwhich matches the BioSample accession of the assembly.\n\n```{bash}\n# Create the Bactopia directory structure\nbactopia atb-formatter --path legionella-assemblies --recursive\n2024-03-22 14:30:07 INFO     2024-03-22 14:30:07:root:INFO - Setting up Bactopia directory structure (use --verbose to see more details)                                                                                                                  atb_formatter.py:129\n2024-03-22 14:30:08 INFO     2024-03-22 14:30:08:root:INFO - Bactopia directory structure created at bactopia                                                                                                                                             atb_formatter.py:134\n                    INFO     2024-03-22 14:30:08:root:INFO - Total assemblies processed: 5393\n```\n\nPlease note the usage of `--recursive` which will traverse the `legionella-assemblies` directory\nto find all assemblies contained. At this point, the `bactopia` directory structure has been\ncreated for 5,393 assemblies and is ready for use with Bactopia Tools.\n\n#### Use Bactopia to run Legsta\n\nAs mentioned above, we will use [legsta](https://github.com/tseemann/legsta) to analyze each\nof the _Legionella pneumophila_ assemblies. To do this, we will use the\n[legsta Bactopia Tool](https://bactopia.github.io/latest/bactopia-tools/legsta/).\n\n```{bash}\n# Run legsta (please utilize Docker or Singularity only for reproducibility)\nbactopia --wf legsta -profile singularity\n```\n\nPlease note, for reproducibility, it is recommended to use Docker or Singularity with\nBactopia Tools.\n\nUpon completion, you should be met with something like the following:\n\n```{bash}\n[5d/d04297] process > BACTOPIATOOLS:LEGSTA:LEGSTA_MODULE (SAMN29911258) [100%] 5393 of 5393 ✔\n[71/c63bf7] process > BACTOPIATOOLS:LEGSTA:CSVTK_CONCAT (legsta)        [100%] 1 of 1 ✔\n[16/833262] process > BACTOPIATOOLS:CUSTOM_DUMPSOFTWAREVERSIONS (1)     [100%] 1 of 1 ✔\n\n    Bactopia Tools: `legsta Execution Summary\n    ---------------------------\n    Bactopia Version : 3.0.1\n    Nextflow Version : 23.10.1\n    Command Line     : nextflow run /home/rpetit3/bactopia/main.nf --wf legsta --bactopia bactopia/ -profile singularity\n    Resumed          : false\n    Completed At     : 2024-03-22T15:09:54.959834620-06:00\n    Duration         : 32m 51s\n    Success          : true\n    Exit Code        : 0\n    Error Report     : -\n    Launch Dir       : /home/rpetit3/test-legsta\n\nWARN: Graphviz is required to render the execution DAG in the given format -- See http://www.graphviz.org for more info.\nCompleted at: 22-Mar-2024 15:09:55\nDuration    : 32m 52s\nCPU hours   : 5.2\nSucceeded   : 5'395\n```\n\nThat's it! Now you can take advantage of any of the [Bactopia Tools](https://bactopia.github.io/latest/bactopia-tools/)\nthat utilize assemblies as inputs.\n\n# Feedback\nYour feedback is very valuable! If you run into any issues using Bactopia, have questions, or have some ideas to improve Bactopia, I highly encourage you to submit it to the [Issue Tracker](https://github.com/bactopia/bactopia/issues).\n\n# License\n[MIT License](https://raw.githubusercontent.com/bactopia/bactopia/master/LICENSE)\n\n# Citation\n\nPetit III RA, Read TD, *Bactopia: a flexible pipeline for complete analysis of bacterial genomes.* __mSystems__. 5 (2020), https://doi.org/10.1128/mSystems.00190-20.\n\n# Author\n\n* Robert A. Petit III\n* Twitter: [@rpetit3](https://twitter.com/rpetit3)\n",
+    'long_description': "[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-908a85?logo=gitpod)](https://gitpod.io/#https://github.com/bactopia/bactopia-py)\n\n![Bactopia Logo](https://raw.githubusercontent.com/bactopia/bactopia/master/data/bactopia-logo.png)\n\n# bactopia-py\nA Python package for working with [Bactopia](https://bactopia.github.io/)\n\n## Bactopia Subcommands\n\nThere are many subcommands available in Bactopia. Here is a brief description of each command:\n\n| Command              | Description                                                                |\n|----------------------|----------------------------------------------------------------------------|\n| `bactopia-citations` | Print out tools and citations used throughout Bactopia                     |\n| `bactopia-datasets`  | Download optional datasets to supplement your analyses with Bactopia       |\n| `bactopia-download`  | Builds Bactopia environments for use with Nextflow.                        |\n| `bactopia-prepare`   | Create a 'file of filenames' (FOFN) of samples to be processed by Bactopia |\n| `bactopia-search`    | Query against ENA and SRA for public accessions to process with Bactopia   |\n| `bactopia-summary`   | Generate a summary table from the Bactopia results.                        |\n\nBelow is the `--help` output for each subcommand.\n\n### `bactopia-citations`\n\n```{bash}\n Usage: bactopia-citations [OPTIONS]\n\n Print out tools and citations used throughout Bactopia\n\n╭─ Options ────────────────────────────────────────────────────────────────────────────╮\n│    --version        -V        Show the version and exit.                             │\n│ *  --bactopia-path  -b  TEXT  Directory where Bactopia repository is stored          │\n│                               [required]                                             │\n│    --name           -n  TEXT  Only print citation matching a given name              │\n│    --plain-text     -p        Disable rich formatting                                │\n│    --help                     Show this message and exit.                            │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n### `bactopia-datasets`\n\n```{bash}\n Usage: bactopia-datasets [OPTIONS] [UNKNOWN]...\n\n Download optional datasets to supplement your analyses with Bactopia\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --bactopia-path    TEXT  Directory where Bactopia repository is stored [required] │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Download Related Options ───────────────────────────────────────────────────────────╮\n│ --datasets_cache    TEXT     Base directory to download datasets to (Defaults to env │\n│                              variable BACTOPIA_CACHEDIR, a subfolder called datasets │\n│                              will be created)                                        │\n│                              [default: ${HOME}/.bactopia]                 │\n│ --force                      Force overwrite of existing pre-built environments.     │\n│ --max_retry         INTEGER  Maximum times to attempt creating Conda environment.    │\n│                              (Default: 3)                                            │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --verbose      Print debug related text.                                             │\n│ --silent       Only critical errors will be printed.                                 │\n│ --version      Show the version and exit.                                            │\n│ --help         Show this message and exit.                                           │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n\n```\n\n### `bactopia-download`\n\n```{bash}\n Usage: bactopia-download [OPTIONS] [UNKNOWN]...\n\n Builds Bactopia environments for use with Nextflow.\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --bactopia-path    TEXT  Directory where Bactopia results are stored [required]   │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Build Related Options ──────────────────────────────────────────────────────────────╮\n│ --envtype                     [conda|docker|singularity|  The type of environment to │\n│                               all]                        build.                     │\n│                                                           [default: conda]           │\n│ --wf                          TEXT                        Build a environment for a  │\n│                                                           the given workflow         │\n│                                                           [default: bactopia]        │\n│ --condadir                    TEXT                        Directory to create Conda  │\n│                                                           environments               │\n│                                                           (NXF_CONDA_CACHEDIR env    │\n│                                                           variable takes precedence) │\n│ --use_conda                                               Use Conda for building     │\n│                                                           Conda environments instead │\n│                                                           of Mamba                   │\n│ --singularity_cache           TEXT                        Directory to download      │\n│                                                           Singularity images         │\n│                                                           (NXF_SINGULARITY_CACHEDIR  │\n│                                                           env variable takes         │\n│                                                           precedence)                │\n│ --singularity_pull_docker…                                Force conversion of Docker │\n│                                                           containers, instead        │\n│                                                           downloading Singularity    │\n│                                                           images directly            │\n│ --force_rebuild                                           Force overwrite of         │\n│                                                           existing pre-built         │\n│                                                           environments.              │\n│ --max_retry                   INTEGER                     Maximum times to attempt   │\n│                                                           creating Conda             │\n│                                                           environment. (Default: 3)  │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --verbose      Print debug related text.                                             │\n│ --silent       Only critical errors will be printed.                                 │\n│ --version      Show the version and exit.                                            │\n│ --help         Show this message and exit.                                           │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Options ────────────────────────────────────────────────────────────────────────────╮\n│ --build-all         Builds all environments for Bactopia workflows                   │\n│ --build-nfcore      Builds all nf-core related environments                          │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n### `bactopia-prepare`\n\n```{bash}\n Usage: bactopia-prepare [OPTIONS]\n\n Create a 'file of filenames' (FOFN) of samples to be processed by Bactopia\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --path  -p  TEXT  Directory where FASTQ files are stored [required]               │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Matching Options ───────────────────────────────────────────────────────────────────╮\n│ --assembly-ext     -a  TEXT  Extension of the FASTA assemblies [default: .fna.gz]    │\n│ --fastq-ext        -f  TEXT  Extension of the FASTQs [default: .fastq.gz]            │\n│ --fastq-separator      TEXT  Split FASTQ name on the last occurrence of the          │\n│                              separator                                               │\n│                              [default: _]                                            │\n│ --pe1-pattern          TEXT  Designates difference first set of paired-end reads     │\n│                              [default: [Aa]|[Rr]1|1]                                 │\n│ --pe2-pattern          TEXT  Designates difference second set of paired-end reads    │\n│                              [default: [Bb]|[Rr]2|2]                                 │\n│ --merge                      Flag samples with multiple read sets to be merged by    │\n│                              Bactopia                                                │\n│ --ont                        Single-end reads should be treated as Oxford Nanopore   │\n│                              reads                                                   │\n│ --recursive        -r        Directories will be traversed recursively               │\n│ --prefix               TEXT  Prefix to add to the path                               │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Sample Information Options ─────────────────────────────────────────────────────────╮\n│ --metadata             TEXT     Metadata per sample with genome size and species     │\n│                                 information                                          │\n│ --genome-size  -gsize  INTEGER  Genome size to use for all samples                   │\n│ --species      -s      TEXT     Species to use for all samples (If available, can be │\n│                                 used to determine genome size)                       │\n│ --taxid                TEXT     Use the genome size of the Taxon ID for all samples  │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --examples        Print example usage                                                │\n│ --verbose         Increase the verbosity of output                                   │\n│ --silent          Only critical errors will be printed                               │\n│ --version   -V    Show the version and exit.                                         │\n│ --help            Show this message and exit.                                        │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n### `bactopia-search`\n\n```{bash}\n Usage: bactopia-search [OPTIONS]\n\n Query against ENA and SRA for public accessions to process with Bactopia\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --query  -q  TEXT  Taxon ID or Study, BioSample, or Run accession (can also be    │\n│                       comma separated or a file of accessions)                       │\n│                       [required]                                                     │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Query Options ──────────────────────────────────────────────────────────────────────╮\n│ --exact-taxon                     Exclude Taxon ID descendants                       │\n│ --limit             -l   INTEGER  Maximum number of results (per query) to return    │\n│                                   [default: 1000000]                                 │\n│ --accession-limit   -al  INTEGER  Maximum number of accessions to query at once      │\n│                                   [default: 5000]                                    │\n│ --biosample-subset       INTEGER  If a BioSample has multiple Experiments, maximum   │\n│                                   number to randomly select (0 = disabled)           │\n│                                   [default: 0]                                       │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Filtering Options ──────────────────────────────────────────────────────────────────╮\n│ --min-base-count   -mbc  INTEGER  Filters samples based on minimum base pair count   │\n│                                   (0 = disabled)                                     │\n│                                   [default: 0]                                       │\n│ --min-read-length  -mrl  INTEGER  Filters samples based on minimum mean read length  │\n│                                   (0 = disabled)                                     │\n│                                   [default: 0]                                       │\n│ --min-coverage     -mc   INTEGER  Filter samples based on minimum coverage (requires │\n│                                   --genome_size, 0 = disabled)                       │\n│                                   [default: 0]                                       │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --genome-size  -gsize  INTEGER  Genome size to be used for all samples, and for      │\n│                                 calculating min coverage                             │\n│                                 [default: 0]                                         │\n│ --outdir       -o      TEXT     Directory to write output [default: ./]              │\n│ --prefix       -p      TEXT     Prefix to use for output file names                  │\n│                                 [default: bactopia]                                  │\n│ --force                         Overwrite existing reports                           │\n│ --verbose                       Increase the verbosity of output                     │\n│ --silent                        Only critical errors will be printed                 │\n│ --version      -V               Show the version and exit.                           │\n│ --help                          Show this message and exit.                          │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n### `bactopia-summary`\n\n```{bash}\n Usage: bactopia-summary [OPTIONS]\n\n Generate a summary table from the Bactopia results.\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --bactopia-path  -b  TEXT  Directory where Bactopia results are stored [required] │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Gold Cutoffs ───────────────────────────────────────────────────────────────────────╮\n│ --gold-coverage     -gcov      INTEGER  Minimum amount of coverage required for Gold │\n│                                         status                                       │\n│                                         [default: 100]                               │\n│ --gold-quality      -gqual     INTEGER  Minimum per-read mean quality score required │\n│                                         for Gold status                              │\n│                                         [default: 30]                                │\n│ --gold-read-length  -glen      INTEGER  Minimum mean read length required for Gold   │\n│                                         status                                       │\n│                                         [default: 95]                                │\n│ --gold-contigs      -gcontigs  INTEGER  Maximum contig count required for Gold       │\n│                                         status                                       │\n│                                         [default: 100]                               │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Silver Cutoffs ─────────────────────────────────────────────────────────────────────╮\n│ --silver-coverage     -scov      INTEGER  Minimum amount of coverage required for    │\n│                                           Silver status                              │\n│                                           [default: 50]                              │\n│ --silver-quality      -squal     INTEGER  Minimum per-read mean quality score        │\n│                                           required for Silver status                 │\n│                                           [default: 20]                              │\n│ --silver-read-length  -slen      INTEGER  Minimum mean read length required for      │\n│                                           Silver status                              │\n│                                           [default: 75]                              │\n│ --silver-contigs      -scontigs  INTEGER  Maximum contig count required for Silver   │\n│                                           status                                     │\n│                                           [default: 200]                             │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Fail Cutoffs ───────────────────────────────────────────────────────────────────────╮\n│ --min-coverage        -mincov   INTEGER  Minimum amount of coverage required to pass │\n│                                          [default: 20]                               │\n│ --min-quality         -minqual  INTEGER  Minimum per-read mean quality score         │\n│                                          required to pass                            │\n│                                          [default: 12]                               │\n│ --min-read-length     -minlen   INTEGER  Minimum mean read length required to pass   │\n│                                          [default: 49]                               │\n│ --max-contigs                   INTEGER  Maximum contig count required to pass       │\n│                                          [default: 500]                              │\n│ --min-assembled-size            INTEGER  Minimum assembled genome size               │\n│ --max-assembled-size            INTEGER  Maximum assembled genome size               │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --outdir   -o  PATH  Directory to write output [default: ./]                         │\n│ --prefix   -p  TEXT  Prefix to use for output files [default: bactopia]              │\n│ --force              Overwrite existing reports                                      │\n│ --verbose            Increase the verbosity of output                                │\n│ --silent             Only critical errors will be printed                            │\n│ --version  -V        Show the version and exit.                                      │\n│ --help               Show this message and exit.                                     │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n# All The Bacteria (ATB)\n\nThe [AllTheBacteria](https://www.biorxiv.org/content/10.1101/2024.03.08.584059v1) is a collection\nof nearly 2,000,000 bacterial genomes. Using available FASTQ files from the European Nucleotide\nArchive (ENA) and Sequence Read Archive (SRA), the genomes were assembled using [Shovill] and made\npublicly available from the [Iqbal Lab](https://github.com/iqbal-lab-org/AllTheBacteria).\n\nTo make it easy to utilize [Bactopia Tools](https://bactopia.github.io/latest/bactopia-tools/) with\nassemblies from AllTheBacteria, `bactopia-atb-formatter` was created. This tool will create a \ndirectory structure that resembles output from an actual Bactopia run.\n\n### `bactopia-atb-formatter`\n\n```{bash}\n Usage: bactopia-atb-formatter [OPTIONS]\n\n Restructure All-the-Bacteria assemblies to allow usage with Bactopia Tools\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --path  -p  TEXT  Directory where FASTQ files are stored [required]               │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Bactopia Directory Structure Options ───────────────────────────────────────────────╮\n│ --bactopia-dir  -b  TEXT            The path you would like to place bactopia        │\n│                                     structure                                        │\n│                                     [default: bactopia]                              │\n│ --publish-mode  -m  [symlink|copy]  Designates plascement of assemblies will be      │\n│                                     handled                                          │\n│                                     [default: symlink]                               │\n│ --recursive     -r                  Traverse recursively through provided path       │\n│ --extension     -e  TEXT            The extension of the assemblies e.g .fa,.fa.gz   │\n│                                     [default: .fa]                                   │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --verbose        Increase the verbosity of output                                    │\n│ --silent         Only critical errors will be printed                                │\n│ --version  -V    Show the version and exit.                                          │\n│ --help           Show this message and exit.                                         │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n### Example Usage for _Legionella pneumophila_\n\nTo demonstrate the usage of `bactopia-atb-formatter`, we will use assemblies for\n_Legionella pneumophila_. The following steps will download the assemblies, build the\nBactopia directory structure, and then run [legsta](https://github.com/tseemann/legsta)\nvia the [Bactopia Tool](https://bactopia.github.io/latest/bactopia-tools/legsta/).\n\n#### Download the Assemblies\n\nFirst will download the _Legionella pneumophila_ assemblies from AllTheBacteria. After downloading\nwe will extract them into a folder called `legionella-assemblies`. Within this folder, there will be\nsubdirectories for each tarball that was downloaded.\n\n```{bash}\nmkdir atb-legionella\ncd atb-legionella\n\n# Download the assemblies\nwget https://ftp.ebi.ac.uk/pub/databases/AllTheBacteria/Releases/0.1/assembly/legionella_pneumophila__01.asm.tar.xz\nwget https://ftp.ebi.ac.uk/pub/databases/AllTheBacteria/Releases/0.1/assembly/legionella_pneumophila__02.asm.tar.xz\n\n# Extract the assemblies\nmkdir legionella-assemblies\ntar -C legionella-assemblies -xJf legionella_pneumophila__01.asm.tar.xz\ntar -C legionella-assemblies -xJf legionella_pneumophila__02.asm.tar.xz\n```\n\n#### Create the Bactopia Directory Structure\n\nWith the assemblies extracted, we can now create the Bactopia directory structure using\n`bactopia-atb-formatter`. Once complete, each assembly will have its own folder created\nwhich matches the BioSample accession of the assembly.\n\n```{bash}\n# Create the Bactopia directory structure\nbactopia atb-formatter --path legionella-assemblies --recursive\n2024-03-22 14:30:07 INFO     2024-03-22 14:30:07:root:INFO - Setting up Bactopia directory structure (use --verbose to see more details)                                                                                                                  atb_formatter.py:129\n2024-03-22 14:30:08 INFO     2024-03-22 14:30:08:root:INFO - Bactopia directory structure created at bactopia                                                                                                                                             atb_formatter.py:134\n                    INFO     2024-03-22 14:30:08:root:INFO - Total assemblies processed: 5393\n```\n\nPlease note the usage of `--recursive` which will traverse the `legionella-assemblies` directory\nto find all assemblies contained. At this point, the `bactopia` directory structure has been\ncreated for 5,393 assemblies and is ready for use with Bactopia Tools.\n\n#### Use Bactopia to run Legsta\n\nAs mentioned above, we will use [legsta](https://github.com/tseemann/legsta) to analyze each\nof the _Legionella pneumophila_ assemblies. To do this, we will use the\n[legsta Bactopia Tool](https://bactopia.github.io/latest/bactopia-tools/legsta/).\n\n```{bash}\n# Run legsta (please utilize Docker or Singularity only for reproducibility)\nbactopia --wf legsta -profile singularity\n```\n\nPlease note, for reproducibility, it is recommended to use Docker or Singularity with\nBactopia Tools.\n\nUpon completion, you should be met with something like the following:\n\n```{bash}\n[5d/d04297] process > BACTOPIATOOLS:LEGSTA:LEGSTA_MODULE (SAMN29911258) [100%] 5393 of 5393 ✔\n[71/c63bf7] process > BACTOPIATOOLS:LEGSTA:CSVTK_CONCAT (legsta)        [100%] 1 of 1 ✔\n[16/833262] process > BACTOPIATOOLS:CUSTOM_DUMPSOFTWAREVERSIONS (1)     [100%] 1 of 1 ✔\n\n    Bactopia Tools: `legsta Execution Summary\n    ---------------------------\n    Bactopia Version : 3.0.1\n    Nextflow Version : 23.10.1\n    Command Line     : nextflow run /home/rpetit3/bactopia/main.nf --wf legsta --bactopia bactopia/ -profile singularity\n    Resumed          : false\n    Completed At     : 2024-03-22T15:09:54.959834620-06:00\n    Duration         : 32m 51s\n    Success          : true\n    Exit Code        : 0\n    Error Report     : -\n    Launch Dir       : /home/rpetit3/test-legsta\n\nWARN: Graphviz is required to render the execution DAG in the given format -- See http://www.graphviz.org for more info.\nCompleted at: 22-Mar-2024 15:09:55\nDuration    : 32m 52s\nCPU hours   : 5.2\nSucceeded   : 5'395\n```\n\nThat's it! Now you can take advantage of any of the [Bactopia Tools](https://bactopia.github.io/latest/bactopia-tools/)\nthat utilize assemblies as inputs.\n\n# Feedback\nYour feedback is very valuable! If you run into any issues using Bactopia, have questions, or have some ideas to improve Bactopia, I highly encourage you to submit it to the [Issue Tracker](https://github.com/bactopia/bactopia/issues).\n\n# License\n[MIT License](https://raw.githubusercontent.com/bactopia/bactopia/master/LICENSE)\n\n# Citation\n\nPetit III RA, Read TD, *Bactopia: a flexible pipeline for complete analysis of bacterial genomes.* __mSystems__. 5 (2020), https://doi.org/10.1128/mSystems.00190-20.\n\n# Author\n\n* Robert A. Petit III\n* Twitter: [@rpetit3](https://twitter.com/rpetit3)\n",
     'author': 'Robert A. Petit III',
     'author_email': 'robbie.petit@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://bactopia.github.io/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `bactopia-1.1.0/PKG-INFO` & `bactopia-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bactopia
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python package for working with Bactopia
 Home-page: https://bactopia.github.io/
 License: MIT
 Keywords: bioinformatics,bacteria,bactopia,SRA,ENA
 Author: Robert A. Petit III
 Author-email: robbie.petit@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
@@ -320,14 +320,16 @@
 │ --bactopia-dir  -b  TEXT            The path you would like to place bactopia        │
 │                                     structure                                        │
 │                                     [default: bactopia]                              │
 │ --publish-mode  -m  [symlink|copy]  Designates plascement of assemblies will be      │
 │                                     handled                                          │
 │                                     [default: symlink]                               │
 │ --recursive     -r                  Traverse recursively through provided path       │
+│ --extension     -e  TEXT            The extension of the assemblies e.g .fa,.fa.gz   │
+│                                     [default: .fa]                                   │
 ╰──────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Additional Options ─────────────────────────────────────────────────────────────────╮
 │ --verbose        Increase the verbosity of output                                    │
 │ --silent         Only critical errors will be printed                                │
 │ --version  -V    Show the version and exit.                                          │
 │ --help           Show this message and exit.                                         │
 ╰──────────────────────────────────────────────────────────────────────────────────────╯
```

