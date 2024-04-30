# Comparing `tmp/emzed-3.0.0a8.tar.gz` & `tmp/emzed-3.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emzed-3.0.0a8.tar", last modified: Mon Jan  9 17:20:10 2023, max compression
+gzip compressed data, was "emzed-3.0.0a9.tar", last modified: Mon Jan  9 20:01:52 2023, max compression
```

## Comparing `emzed-3.0.0a8.tar` & `emzed-3.0.0a9.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.301602 emzed-3.0.0a8/
--rw-rw-rw-   0 root         (0) root         (0)    35149 2023-01-04 13:15:32.000000 emzed-3.0.0a8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-01-04 13:15:32.000000 emzed-3.0.0a8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      207 2023-01-09 17:20:10.301602 emzed-3.0.0a8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-01-04 13:15:32.000000 emzed-3.0.0a8/README.md
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-01-09 17:20:10.301602 emzed-3.0.0a8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2818 2023-01-09 17:16:02.000000 emzed-3.0.0a8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.279602 emzed-3.0.0a8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.282602 emzed-3.0.0a8/src/emzed/
--rw-rw-rw-   0 root         (0) root         (0)     3253 2023-01-05 15:50:38.000000 emzed-3.0.0a8/src/emzed/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1163 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.284602 emzed-3.0.0a8/src/emzed/align/
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/align/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4123 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/align/mz_align.py
--rw-rw-rw-   0 root         (0) root         (0)     4784 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/align/mz_align_routines.py
--rw-rw-rw-   0 root         (0) root         (0)    11487 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/align/rt_align.py
--rw-rw-rw-   0 root         (0) root         (0)     3484 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/align/sample_alignment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.284602 emzed-3.0.0a8/src/emzed/annotate/
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/annotate/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9430 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/annotate/annotate_adducts.py
--rw-rw-rw-   0 root         (0) root         (0)     2008 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/check_pyopenms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.285602 emzed-3.0.0a8/src/emzed/chemistry/
--rw-rw-rw-   0 root         (0) root         (0)    51165 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/chemistry/Elements.xml
--rw-rw-rw-   0 root         (0) root         (0)      391 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/chemistry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/chemistry/abundance.py
--rwxrwxrwx   0 root         (0) root         (0)     3823 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/chemistry/adducts.py
--rw-rw-rw-   0 root         (0) root         (0)     7458 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/chemistry/elements.py
--rw-rw-rw-   0 root         (0) root         (0)    82021 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/chemistry/elements_pubchem.json
--rw-rw-rw-   0 root         (0) root         (0)     2102 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/chemistry/fetch_elements_pubchem.py
--rw-rw-rw-   0 root         (0) root         (0)     5361 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/chemistry/fit_formula.py
--rw-rw-rw-   0 root         (0) root         (0)     3894 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/chemistry/formula_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     9345 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/chemistry/isotope_generator.py
--rw-rw-rw-   0 root         (0) root         (0)      473 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/chemistry/mass.py
--rw-rw-rw-   0 root         (0) root         (0)     3364 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/chemistry/molecular_formula.py
--rw-rw-rw-   0 root         (0) root         (0)    16981 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/chemistry/pubchem.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.286602 emzed-3.0.0a8/src/emzed/config/
--rw-rw-rw-   0 root         (0) root         (0)      830 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2727 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/config/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.286602 emzed-3.0.0a8/src/emzed/core/
--rw-rw-rw-   0 root         (0) root         (0)     1038 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5854 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/core/db_backed_dictionary.py
--rw-rw-rw-   0 root         (0) root         (0)     1124 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/core/db_backed_model.py
--rw-rw-rw-   0 root         (0) root         (0)      831 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/core/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1201 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/core/hashes.py
--rw-rw-rw-   0 root         (0) root         (0)     2301 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/core/multiprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)     2651 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/db.py
--rw-rw-rw-   0 root         (0) root         (0)     1535 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/ext.py
--rw-rw-rw-   0 root         (0) root         (0)      412 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/gui.py
--rw-rw-rw-   0 root         (0) root         (0)    11213 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.287602 emzed-3.0.0a8/src/emzed/ms2/
--rw-rw-rw-   0 root         (0) root         (0)      944 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/ms2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10404 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/ms2/attach_ms2_spectra.py
--rw-rw-rw-   0 root         (0) root         (0)     1899 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/ms2/merge_spectra.py
--rw-rw-rw-   0 root         (0) root         (0)     3490 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/ms2/sirius_export.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.287602 emzed-3.0.0a8/src/emzed/ms_data/
--rw-rw-rw-   0 root         (0) root         (0)      860 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/ms_data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    46312 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/ms_data/peak_map.py
--rw-rw-rw-   0 root         (0) root         (0)     1503 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/ms_data/peak_map_hasher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.287602 emzed-3.0.0a8/src/emzed/optimized/
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/optimized/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   276714 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/optimized/formula_fit.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.288602 emzed-3.0.0a8/src/emzed/peak_picking/
--rw-rw-rw-   0 root         (0) root         (0)     1014 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/peak_picking/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13558 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/peak_picking/_run_feature_finder_metabo.py
--rw-rw-rw-   0 root         (0) root         (0)     5039 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/peak_picking/_run_feature_finder_metabo_on_folder.py
--rw-rw-rw-   0 root         (0) root         (0)     2777 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/peak_picking/extract_chromatograms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.288602 emzed-3.0.0a8/src/emzed/pyopenms/
--rw-rw-rw-   0 root         (0) root         (0)     8279 2023-01-09 17:16:02.000000 emzed-3.0.0a8/src/emzed/pyopenms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.280602 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.280602 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.280602 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.280602 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.280602 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.280602 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.280602 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.289602 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/
--rwxr-xr-x   0 root         (0) root         (0)    19116 2023-01-09 17:16:49.000000 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/Enzymes.xml
--rw-r--r--   0 root         (0) root         (0)     5225 2023-01-09 17:16:49.000000 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/Enzymes_RNA.xml
--rw-r--r--   0 root         (0) root         (0)    11210 2023-01-09 17:16:49.000000 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/XTandem_default_config.xml
--rw-r--r--   0 root         (0) root         (0)     1081 2023-01-09 17:16:49.000000 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/XTandem_residue_mass.bioml.xml
--rw-r--r--   0 root         (0) root         (0)  2430277 2023-01-09 17:16:49.000000 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/unimod.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.291602 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/DESKTOP/
--rw-r--r--   0 root         (0) root         (0)     1413 2023-01-09 17:16:49.000000 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/DESKTOP/TOPPAS.appdata.xml
--rw-r--r--   0 root         (0) root         (0)     1709 2023-01-09 17:16:49.000000 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/DESKTOP/TOPPView.appdata.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.292602 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/
--rw-r--r--   0 root         (0) root         (0)    18270 2023-01-09 17:16:49.000000 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/TraML-mapping.xml
--rw-r--r--   0 root         (0) root         (0)    21658 2023-01-09 17:16:49.000000 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/ms-mapping.xml
--rw-r--r--   0 root         (0) root         (0)    25231 2023-01-09 17:16:49.000000 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/mzIdentML-mapping.xml
--rw-r--r--   0 root         (0) root         (0)    25621 2023-01-09 17:16:49.000000 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/mzdata-mapping.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.280602 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/setuptools/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.292602 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/setuptools/command/
--rw-r--r--   0 root         (0) root         (0)      628 2023-01-09 17:16:41.000000 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/setuptools/command/launcher manifest.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.280602 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.280602 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.281602 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.280602 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.281602 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.281602 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.292602 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/
--rwxr-xr-x   0 root         (0) root         (0)    19116 2023-01-09 17:16:49.000000 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/Enzymes.xml
--rw-r--r--   0 root         (0) root         (0)     5225 2023-01-09 17:16:49.000000 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/Enzymes_RNA.xml
--rw-r--r--   0 root         (0) root         (0)    11210 2023-01-09 17:16:49.000000 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/XTandem_default_config.xml
--rw-r--r--   0 root         (0) root         (0)     1081 2023-01-09 17:16:49.000000 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/XTandem_residue_mass.bioml.xml
--rw-r--r--   0 root         (0) root         (0)  2430277 2023-01-09 17:16:49.000000 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/unimod.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.295602 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/DESKTOP/
--rw-r--r--   0 root         (0) root         (0)     1413 2023-01-09 17:16:49.000000 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/DESKTOP/TOPPAS.appdata.xml
--rw-r--r--   0 root         (0) root         (0)     1709 2023-01-09 17:16:49.000000 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/DESKTOP/TOPPView.appdata.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.295602 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/
--rw-r--r--   0 root         (0) root         (0)    18270 2023-01-09 17:16:49.000000 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/TraML-mapping.xml
--rw-r--r--   0 root         (0) root         (0)    21658 2023-01-09 17:16:49.000000 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/ms-mapping.xml
--rw-r--r--   0 root         (0) root         (0)    25231 2023-01-09 17:16:49.000000 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/mzIdentML-mapping.xml
--rw-r--r--   0 root         (0) root         (0)    25621 2023-01-09 17:16:49.000000 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/mzdata-mapping.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.281602 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/setuptools/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.295602 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/setuptools/command/
--rw-r--r--   0 root         (0) root         (0)      628 2023-01-09 17:16:41.000000 emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/setuptools/command/launcher manifest.xml
--rw-rw-rw-   0 root         (0) root         (0)     1963 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/pyopenms/object_handling.py
--rw-rw-rw-   0 root         (0) root         (0)     9327 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/pyopenms/optimizations.py
--rw-rw-rw-   0 root         (0) root         (0)     2957 2023-01-09 17:16:02.000000 emzed-3.0.0a8/src/emzed/pyopenms/pyopenms_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.296602 emzed-3.0.0a8/src/emzed/quantification/
--rw-rw-rw-   0 root         (0) root         (0)      927 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/quantification/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10998 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/quantification/peak_integration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.296602 emzed-3.0.0a8/src/emzed/quantification/peak_shape_models/
--rw-rw-rw-   0 root         (0) root         (0)     1185 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/quantification/peak_shape_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4216 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/quantification/peak_shape_models/asymmetric_gauss_model.py
--rw-rw-rw-   0 root         (0) root         (0)     2084 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/quantification/peak_shape_models/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1733 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/quantification/peak_shape_models/linear_interpolation_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1496 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/quantification/peak_shape_models/no_model.py
--rw-rw-rw-   0 root         (0) root         (0)     2363 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/quantification/peak_shape_models/savgol_model.py
--rw-rw-rw-   0 root         (0) root         (0)     6666 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/quantification/peak_shape_models/simplified_emg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.297602 emzed-3.0.0a8/src/emzed/r_connect/
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/r_connect/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1400 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/r_connect/patched_pyper.py
--rwxrwxrwx   0 root         (0) root         (0)    10324 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/r_connect/r_executor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.299602 emzed-3.0.0a8/src/emzed/table/
--rw-rw-rw-   0 root         (0) root         (0)      838 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/table/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3550 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/table/add_column.py
--rw-rw-rw-   0 root         (0) root         (0)    21258 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/table/base_models.py
--rw-rw-rw-   0 root         (0) root         (0)     3092 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/table/col_types.py
--rw-rw-rw-   0 root         (0) root         (0)     2922 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/table/collapse.py
--rw-rw-rw-   0 root         (0) root         (0)     1469 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/table/delete_rows.py
--rw-rw-rw-   0 root         (0) root         (0)    26572 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/table/expressions.py
--rw-rw-rw-   0 root         (0) root         (0)     1879 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/table/extract_columns_model.py
--rw-rw-rw-   0 root         (0) root         (0)     2328 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/table/filter_model.py
--rw-rw-rw-   0 root         (0) root         (0)    14204 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/table/full_table_model.py
--rw-rw-rw-   0 root         (0) root         (0)     7549 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/table/group_by.py
--rw-rw-rw-   0 root         (0) root         (0)     2981 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/table/immutable_table_model.py
--rw-rw-rw-   0 root         (0) root         (0)     9464 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/table/join.py
--rw-rw-rw-   0 root         (0) root         (0)     1301 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/table/load_into_from.py
--rw-rw-rw-   0 root         (0) root         (0)     1189 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/table/prepare_table_cell_content.py
--rw-rw-rw-   0 root         (0) root         (0)     5639 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/table/replace_column.py
--rw-rw-rw-   0 root         (0) root         (0)     2886 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/table/row_class.py
--rw-rw-rw-   0 root         (0) root         (0)     2880 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/table/select_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1882 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/table/sort_model.py
--rw-rw-rw-   0 root         (0) root         (0)    66504 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/table/table.py
--rw-rw-rw-   0 root         (0) root         (0)     1097 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/table/table_migrations.py
--rw-rw-rw-   0 root         (0) root         (0)    14565 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/table/table_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.299602 emzed-3.0.0a8/src/emzed/targeted/
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/targeted/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3077 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/targeted/solution_space.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.300602 emzed-3.0.0a8/src/emzed/utils/
--rw-rw-rw-   0 root         (0) root         (0)     1098 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2155 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/utils/align_spectra.py
--rw-rw-rw-   0 root         (0) root         (0)     2358 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/utils/busy_indicator.py
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/utils/download.py
--rw-rw-rw-   0 root         (0) root         (0)     1756 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/utils/functools.py
--rw-rw-rw-   0 root         (0) root         (0)      550 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/utils/has_emzed_gui.py
--rw-rw-rw-   0 root         (0) root         (0)     1950 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/utils/lookup.py
--rw-rw-rw-   0 root         (0) root         (0)     9268 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/utils/sqlite.py
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-01-04 13:15:32.000000 emzed-3.0.0a8/src/emzed/utils/temp_file_handling.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 17:20:10.283602 emzed-3.0.0a8/src/emzed.egg-info/
--rw-r--r--   0 root         (0) root         (0)      207 2023-01-09 17:20:09.000000 emzed-3.0.0a8/src/emzed.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6299 2023-01-09 17:20:10.000000 emzed-3.0.0a8/src/emzed.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-09 17:20:09.000000 emzed-3.0.0a8/src/emzed.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-09 17:16:38.000000 emzed-3.0.0a8/src/emzed.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      165 2023-01-09 17:20:09.000000 emzed-3.0.0a8/src/emzed.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-01-09 17:20:09.000000 emzed-3.0.0a8/src/emzed.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.520801 emzed-3.0.0a9/
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-01-04 13:15:32.000000 emzed-3.0.0a9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-01-04 13:15:32.000000 emzed-3.0.0a9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      207 2023-01-09 20:01:52.520801 emzed-3.0.0a9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-01-04 13:15:32.000000 emzed-3.0.0a9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-01-09 20:01:52.520801 emzed-3.0.0a9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2818 2023-01-09 19:57:38.000000 emzed-3.0.0a9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.497801 emzed-3.0.0a9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.501801 emzed-3.0.0a9/src/emzed/
+-rw-rw-rw-   0 root         (0) root         (0)     3253 2023-01-05 15:50:38.000000 emzed-3.0.0a9/src/emzed/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1163 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.503801 emzed-3.0.0a9/src/emzed/align/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/align/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4123 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/align/mz_align.py
+-rw-rw-rw-   0 root         (0) root         (0)     4784 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/align/mz_align_routines.py
+-rw-rw-rw-   0 root         (0) root         (0)    11487 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/align/rt_align.py
+-rw-rw-rw-   0 root         (0) root         (0)     3484 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/align/sample_alignment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.503801 emzed-3.0.0a9/src/emzed/annotate/
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/annotate/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9430 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/annotate/annotate_adducts.py
+-rw-rw-rw-   0 root         (0) root         (0)     2008 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/check_pyopenms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.504801 emzed-3.0.0a9/src/emzed/chemistry/
+-rw-rw-rw-   0 root         (0) root         (0)    51165 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/chemistry/Elements.xml
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/chemistry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/chemistry/abundance.py
+-rwxrwxrwx   0 root         (0) root         (0)     3823 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/chemistry/adducts.py
+-rw-rw-rw-   0 root         (0) root         (0)     7458 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/chemistry/elements.py
+-rw-rw-rw-   0 root         (0) root         (0)    82021 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/chemistry/elements_pubchem.json
+-rw-rw-rw-   0 root         (0) root         (0)     2102 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/chemistry/fetch_elements_pubchem.py
+-rw-rw-rw-   0 root         (0) root         (0)     5361 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/chemistry/fit_formula.py
+-rw-rw-rw-   0 root         (0) root         (0)     3894 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/chemistry/formula_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     9345 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/chemistry/isotope_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)      473 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/chemistry/mass.py
+-rw-rw-rw-   0 root         (0) root         (0)     3364 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/chemistry/molecular_formula.py
+-rw-rw-rw-   0 root         (0) root         (0)    16981 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/chemistry/pubchem.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.505801 emzed-3.0.0a9/src/emzed/config/
+-rw-rw-rw-   0 root         (0) root         (0)      830 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2727 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/config/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.505801 emzed-3.0.0a9/src/emzed/core/
+-rw-rw-rw-   0 root         (0) root         (0)     1038 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5854 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/core/db_backed_dictionary.py
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/core/db_backed_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      831 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/core/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1201 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/core/hashes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2301 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/core/multiprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2651 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/db.py
+-rw-rw-rw-   0 root         (0) root         (0)     1535 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/ext.py
+-rw-rw-rw-   0 root         (0) root         (0)      412 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/gui.py
+-rw-rw-rw-   0 root         (0) root         (0)    11213 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.506801 emzed-3.0.0a9/src/emzed/ms2/
+-rw-rw-rw-   0 root         (0) root         (0)      944 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/ms2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10404 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/ms2/attach_ms2_spectra.py
+-rw-rw-rw-   0 root         (0) root         (0)     1899 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/ms2/merge_spectra.py
+-rw-rw-rw-   0 root         (0) root         (0)     3490 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/ms2/sirius_export.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.506801 emzed-3.0.0a9/src/emzed/ms_data/
+-rw-rw-rw-   0 root         (0) root         (0)      860 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/ms_data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    46312 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/ms_data/peak_map.py
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/ms_data/peak_map_hasher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.506801 emzed-3.0.0a9/src/emzed/optimized/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/optimized/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   276714 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/optimized/formula_fit.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.507801 emzed-3.0.0a9/src/emzed/peak_picking/
+-rw-rw-rw-   0 root         (0) root         (0)     1014 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/peak_picking/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13558 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/peak_picking/_run_feature_finder_metabo.py
+-rw-rw-rw-   0 root         (0) root         (0)     5039 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/peak_picking/_run_feature_finder_metabo_on_folder.py
+-rw-rw-rw-   0 root         (0) root         (0)     2777 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/peak_picking/extract_chromatograms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.507801 emzed-3.0.0a9/src/emzed/pyopenms/
+-rw-rw-rw-   0 root         (0) root         (0)     8324 2023-01-09 19:57:38.000000 emzed-3.0.0a9/src/emzed/pyopenms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.499801 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.498801 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.498801 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.499801 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.498801 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.499801 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.499801 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.508801 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/
+-rwxr-xr-x   0 root         (0) root         (0)    19116 2023-01-09 19:58:26.000000 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/Enzymes.xml
+-rw-r--r--   0 root         (0) root         (0)     5225 2023-01-09 19:58:26.000000 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/Enzymes_RNA.xml
+-rw-r--r--   0 root         (0) root         (0)    11210 2023-01-09 19:58:26.000000 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/XTandem_default_config.xml
+-rw-r--r--   0 root         (0) root         (0)     1081 2023-01-09 19:58:26.000000 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/XTandem_residue_mass.bioml.xml
+-rw-r--r--   0 root         (0) root         (0)  2430277 2023-01-09 19:58:26.000000 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/unimod.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.510801 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/DESKTOP/
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-01-09 19:58:26.000000 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/DESKTOP/TOPPAS.appdata.xml
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-01-09 19:58:26.000000 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/DESKTOP/TOPPView.appdata.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.511801 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/
+-rw-r--r--   0 root         (0) root         (0)    18270 2023-01-09 19:58:26.000000 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/TraML-mapping.xml
+-rw-r--r--   0 root         (0) root         (0)    21658 2023-01-09 19:58:26.000000 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/ms-mapping.xml
+-rw-r--r--   0 root         (0) root         (0)    25231 2023-01-09 19:58:26.000000 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/mzIdentML-mapping.xml
+-rw-r--r--   0 root         (0) root         (0)    25621 2023-01-09 19:58:26.000000 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/mzdata-mapping.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.499801 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/setuptools/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.511801 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/setuptools/command/
+-rw-r--r--   0 root         (0) root         (0)      628 2023-01-09 19:58:18.000000 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/setuptools/command/launcher manifest.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.499801 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.499801 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.499801 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.499801 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.499801 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.499801 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.511801 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/
+-rwxr-xr-x   0 root         (0) root         (0)    19116 2023-01-09 19:58:26.000000 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/Enzymes.xml
+-rw-r--r--   0 root         (0) root         (0)     5225 2023-01-09 19:58:26.000000 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/Enzymes_RNA.xml
+-rw-r--r--   0 root         (0) root         (0)    11210 2023-01-09 19:58:26.000000 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/XTandem_default_config.xml
+-rw-r--r--   0 root         (0) root         (0)     1081 2023-01-09 19:58:26.000000 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/XTandem_residue_mass.bioml.xml
+-rw-r--r--   0 root         (0) root         (0)  2430277 2023-01-09 19:58:26.000000 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/unimod.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.514801 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/DESKTOP/
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-01-09 19:58:26.000000 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/DESKTOP/TOPPAS.appdata.xml
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-01-09 19:58:26.000000 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/DESKTOP/TOPPView.appdata.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.514801 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/
+-rw-r--r--   0 root         (0) root         (0)    18270 2023-01-09 19:58:26.000000 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/TraML-mapping.xml
+-rw-r--r--   0 root         (0) root         (0)    21658 2023-01-09 19:58:26.000000 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/ms-mapping.xml
+-rw-r--r--   0 root         (0) root         (0)    25231 2023-01-09 19:58:26.000000 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/mzIdentML-mapping.xml
+-rw-r--r--   0 root         (0) root         (0)    25621 2023-01-09 19:58:26.000000 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/mzdata-mapping.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.499801 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/setuptools/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.514801 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/setuptools/command/
+-rw-r--r--   0 root         (0) root         (0)      628 2023-01-09 19:58:18.000000 emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/setuptools/command/launcher manifest.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1963 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/pyopenms/object_handling.py
+-rw-rw-rw-   0 root         (0) root         (0)     9327 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/pyopenms/optimizations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2957 2023-01-09 17:16:02.000000 emzed-3.0.0a9/src/emzed/pyopenms/pyopenms_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.514801 emzed-3.0.0a9/src/emzed/quantification/
+-rw-rw-rw-   0 root         (0) root         (0)      927 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/quantification/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10998 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/quantification/peak_integration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.515801 emzed-3.0.0a9/src/emzed/quantification/peak_shape_models/
+-rw-rw-rw-   0 root         (0) root         (0)     1185 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/quantification/peak_shape_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4216 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/quantification/peak_shape_models/asymmetric_gauss_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2084 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/quantification/peak_shape_models/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1733 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/quantification/peak_shape_models/linear_interpolation_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1496 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/quantification/peak_shape_models/no_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2363 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/quantification/peak_shape_models/savgol_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     6666 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/quantification/peak_shape_models/simplified_emg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.516801 emzed-3.0.0a9/src/emzed/r_connect/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/r_connect/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1400 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/r_connect/patched_pyper.py
+-rwxrwxrwx   0 root         (0) root         (0)    10324 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/r_connect/r_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.518801 emzed-3.0.0a9/src/emzed/table/
+-rw-rw-rw-   0 root         (0) root         (0)      838 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/table/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3550 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/table/add_column.py
+-rw-rw-rw-   0 root         (0) root         (0)    21258 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/table/base_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3092 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/table/col_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     2922 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/table/collapse.py
+-rw-rw-rw-   0 root         (0) root         (0)     1469 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/table/delete_rows.py
+-rw-rw-rw-   0 root         (0) root         (0)    26572 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/table/expressions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1879 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/table/extract_columns_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2328 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/table/filter_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    14204 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/table/full_table_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     7549 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/table/group_by.py
+-rw-rw-rw-   0 root         (0) root         (0)     2981 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/table/immutable_table_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     9464 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/table/join.py
+-rw-rw-rw-   0 root         (0) root         (0)     1301 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/table/load_into_from.py
+-rw-rw-rw-   0 root         (0) root         (0)     1189 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/table/prepare_table_cell_content.py
+-rw-rw-rw-   0 root         (0) root         (0)     5639 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/table/replace_column.py
+-rw-rw-rw-   0 root         (0) root         (0)     2886 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/table/row_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     2880 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/table/select_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1882 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/table/sort_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    66504 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/table/table.py
+-rw-rw-rw-   0 root         (0) root         (0)     1097 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/table/table_migrations.py
+-rw-rw-rw-   0 root         (0) root         (0)    14565 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/table/table_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.518801 emzed-3.0.0a9/src/emzed/targeted/
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/targeted/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3077 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/targeted/solution_space.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.519801 emzed-3.0.0a9/src/emzed/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     1098 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2155 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/utils/align_spectra.py
+-rw-rw-rw-   0 root         (0) root         (0)     2358 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/utils/busy_indicator.py
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/utils/download.py
+-rw-rw-rw-   0 root         (0) root         (0)     1756 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/utils/functools.py
+-rw-rw-rw-   0 root         (0) root         (0)      550 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/utils/has_emzed_gui.py
+-rw-rw-rw-   0 root         (0) root         (0)     1950 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/utils/lookup.py
+-rw-rw-rw-   0 root         (0) root         (0)     9268 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/utils/sqlite.py
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-01-04 13:15:32.000000 emzed-3.0.0a9/src/emzed/utils/temp_file_handling.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 20:01:52.502801 emzed-3.0.0a9/src/emzed.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      207 2023-01-09 20:01:52.000000 emzed-3.0.0a9/src/emzed.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6299 2023-01-09 20:01:52.000000 emzed-3.0.0a9/src/emzed.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-09 20:01:52.000000 emzed-3.0.0a9/src/emzed.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-09 19:58:14.000000 emzed-3.0.0a9/src/emzed.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      165 2023-01-09 20:01:52.000000 emzed-3.0.0a9/src/emzed.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-01-09 20:01:52.000000 emzed-3.0.0a9/src/emzed.egg-info/top_level.txt
```

### Comparing `emzed-3.0.0a8/LICENSE` & `emzed-3.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/setup.py` & `emzed-3.0.0a9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         "emzed.optimized.formula_fit",
         [os.path.join("src", "emzed", "optimized", "formula_fit.c")],
     )
 ]
 
 setup(
     name="emzed",
-    version="3.0.0a8",
+    version="3.0.0a9",
     description="",
     url="",
     author="Uwe Schmitt",
     author_email="uwe.schmitt@id.ethz.ch",
     license="MIT",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
```

### Comparing `emzed-3.0.0a8/src/emzed/__init__.py` & `emzed-3.0.0a9/src/emzed/__init__.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/__main__.py` & `emzed-3.0.0a9/src/emzed/__main__.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/align/mz_align.py` & `emzed-3.0.0a9/src/emzed/align/mz_align.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/align/mz_align_routines.py` & `emzed-3.0.0a9/src/emzed/align/mz_align_routines.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/align/rt_align.py` & `emzed-3.0.0a9/src/emzed/align/rt_align.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/align/sample_alignment.py` & `emzed-3.0.0a9/src/emzed/align/sample_alignment.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/annotate/annotate_adducts.py` & `emzed-3.0.0a9/src/emzed/annotate/annotate_adducts.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/check_pyopenms.py` & `emzed-3.0.0a9/src/emzed/check_pyopenms.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/chemistry/Elements.xml` & `emzed-3.0.0a9/src/emzed/chemistry/Elements.xml`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/chemistry/adducts.py` & `emzed-3.0.0a9/src/emzed/chemistry/adducts.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/chemistry/elements.py` & `emzed-3.0.0a9/src/emzed/chemistry/elements.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/chemistry/elements_pubchem.json` & `emzed-3.0.0a9/src/emzed/chemistry/elements_pubchem.json`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/chemistry/fetch_elements_pubchem.py` & `emzed-3.0.0a9/src/emzed/chemistry/fetch_elements_pubchem.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/chemistry/fit_formula.py` & `emzed-3.0.0a9/src/emzed/chemistry/fit_formula.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/chemistry/formula_parser.py` & `emzed-3.0.0a9/src/emzed/chemistry/formula_parser.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/chemistry/isotope_generator.py` & `emzed-3.0.0a9/src/emzed/chemistry/isotope_generator.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/chemistry/molecular_formula.py` & `emzed-3.0.0a9/src/emzed/chemistry/molecular_formula.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/chemistry/pubchem.py` & `emzed-3.0.0a9/src/emzed/chemistry/pubchem.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/config/__init__.py` & `emzed-3.0.0a9/src/emzed/config/__init__.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/config/config.py` & `emzed-3.0.0a9/src/emzed/config/config.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/core/__init__.py` & `emzed-3.0.0a9/src/emzed/core/__init__.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/core/db_backed_dictionary.py` & `emzed-3.0.0a9/src/emzed/core/db_backed_dictionary.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/core/db_backed_model.py` & `emzed-3.0.0a9/src/emzed/core/db_backed_model.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/core/exceptions.py` & `emzed-3.0.0a9/src/emzed/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/core/hashes.py` & `emzed-3.0.0a9/src/emzed/core/hashes.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/core/multiprocessing.py` & `emzed-3.0.0a9/src/emzed/core/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/db.py` & `emzed-3.0.0a9/src/emzed/db.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/ext.py` & `emzed-3.0.0a9/src/emzed/ext.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/io.py` & `emzed-3.0.0a9/src/emzed/io.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/ms2/__init__.py` & `emzed-3.0.0a9/src/emzed/ms2/__init__.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/ms2/attach_ms2_spectra.py` & `emzed-3.0.0a9/src/emzed/ms2/attach_ms2_spectra.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/ms2/merge_spectra.py` & `emzed-3.0.0a9/src/emzed/ms2/merge_spectra.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/ms2/sirius_export.py` & `emzed-3.0.0a9/src/emzed/ms2/sirius_export.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/ms_data/__init__.py` & `emzed-3.0.0a9/src/emzed/ms_data/__init__.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/ms_data/peak_map.py` & `emzed-3.0.0a9/src/emzed/ms_data/peak_map.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/ms_data/peak_map_hasher.py` & `emzed-3.0.0a9/src/emzed/ms_data/peak_map_hasher.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/optimized/formula_fit.c` & `emzed-3.0.0a9/src/emzed/optimized/formula_fit.c`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/peak_picking/__init__.py` & `emzed-3.0.0a9/src/emzed/peak_picking/__init__.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/peak_picking/_run_feature_finder_metabo.py` & `emzed-3.0.0a9/src/emzed/peak_picking/_run_feature_finder_metabo.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/peak_picking/_run_feature_finder_metabo_on_folder.py` & `emzed-3.0.0a9/src/emzed/peak_picking/_run_feature_finder_metabo_on_folder.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/peak_picking/extract_chromatograms.py` & `emzed-3.0.0a9/src/emzed/peak_picking/extract_chromatograms.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/pyopenms/__init__.py` & `emzed-3.0.0a9/src/emzed/pyopenms/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,19 +182,19 @@
                 env_path,
             ],
             stdout=subprocess.PIPE,
             text=True,
         ) as proc:
             for l in iter(proc.stdout.readline, ""):
                 l = l.rstrip()
-                print(f"pyopenms: {l}", flush=True)
                 if l.startswith("PORT="):
                     _, _, port = l.partition("=")
-                    print("pyopenms client ready.")
+                    print("pyopenms client started.")
                     continue
+                print(f"pyopenms: {l}", flush=True)
 
     t = Thread(target=start_listener)
     t.daemon = True
     t.start()
 
     while True:
         if port is None:
@@ -202,14 +202,15 @@
             continue
         try:
             conn = Client(("127.0.0.1", int(port)), authkey=b"secret password")
             break
         except ConnectionRefusedError:
             time.sleep(0.1)
             continue
+    print("connected to pyopenms client.")
     return conn, proc
 
 
 class DirWrapper:
     def __init__(self, dir_):
         self.dir_ = dir_
```

### Comparing `emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/Enzymes.xml` & `emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/Enzymes.xml`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/Enzymes_RNA.xml` & `emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/Enzymes_RNA.xml`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/XTandem_default_config.xml` & `emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/XTandem_default_config.xml`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/XTandem_residue_mass.bioml.xml` & `emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/XTandem_residue_mass.bioml.xml`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/unimod.xml` & `emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/unimod.xml`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/DESKTOP/TOPPAS.appdata.xml` & `emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/DESKTOP/TOPPAS.appdata.xml`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/DESKTOP/TOPPView.appdata.xml` & `emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/DESKTOP/TOPPView.appdata.xml`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/TraML-mapping.xml` & `emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/TraML-mapping.xml`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/ms-mapping.xml` & `emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/ms-mapping.xml`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/mzIdentML-mapping.xml` & `emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/mzIdentML-mapping.xml`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/mzdata-mapping.xml` & `emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/mzdata-mapping.xml`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/setuptools/command/launcher manifest.xml` & `emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib/python3.9/site-packages/setuptools/command/launcher manifest.xml`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/Enzymes.xml` & `emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/Enzymes.xml`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/Enzymes_RNA.xml` & `emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/Enzymes_RNA.xml`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/XTandem_default_config.xml` & `emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/XTandem_default_config.xml`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/XTandem_residue_mass.bioml.xml` & `emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/XTandem_residue_mass.bioml.xml`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/unimod.xml` & `emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/CHEMISTRY/unimod.xml`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/DESKTOP/TOPPAS.appdata.xml` & `emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/DESKTOP/TOPPAS.appdata.xml`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/DESKTOP/TOPPView.appdata.xml` & `emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/DESKTOP/TOPPView.appdata.xml`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/TraML-mapping.xml` & `emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/TraML-mapping.xml`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/ms-mapping.xml` & `emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/ms-mapping.xml`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/mzIdentML-mapping.xml` & `emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/mzIdentML-mapping.xml`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/mzdata-mapping.xml` & `emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/pyopenms/share/OpenMS/MAPPING/mzdata-mapping.xml`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/setuptools/command/launcher manifest.xml` & `emzed-3.0.0a9/src/emzed/pyopenms/_pyopenms_venv/lib64/python3.9/site-packages/setuptools/command/launcher manifest.xml`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/pyopenms/object_handling.py` & `emzed-3.0.0a9/src/emzed/pyopenms/object_handling.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/pyopenms/optimizations.py` & `emzed-3.0.0a9/src/emzed/pyopenms/optimizations.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/pyopenms/pyopenms_client.py` & `emzed-3.0.0a9/src/emzed/pyopenms/pyopenms_client.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/quantification/__init__.py` & `emzed-3.0.0a9/src/emzed/quantification/__init__.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/quantification/peak_integration.py` & `emzed-3.0.0a9/src/emzed/quantification/peak_integration.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/quantification/peak_shape_models/__init__.py` & `emzed-3.0.0a9/src/emzed/quantification/peak_shape_models/__init__.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/quantification/peak_shape_models/asymmetric_gauss_model.py` & `emzed-3.0.0a9/src/emzed/quantification/peak_shape_models/asymmetric_gauss_model.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/quantification/peak_shape_models/base.py` & `emzed-3.0.0a9/src/emzed/quantification/peak_shape_models/base.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/quantification/peak_shape_models/linear_interpolation_model.py` & `emzed-3.0.0a9/src/emzed/quantification/peak_shape_models/linear_interpolation_model.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/quantification/peak_shape_models/no_model.py` & `emzed-3.0.0a9/src/emzed/quantification/peak_shape_models/no_model.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/quantification/peak_shape_models/savgol_model.py` & `emzed-3.0.0a9/src/emzed/quantification/peak_shape_models/savgol_model.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/quantification/peak_shape_models/simplified_emg.py` & `emzed-3.0.0a9/src/emzed/quantification/peak_shape_models/simplified_emg.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/r_connect/patched_pyper.py` & `emzed-3.0.0a9/src/emzed/r_connect/patched_pyper.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/r_connect/r_executor.py` & `emzed-3.0.0a9/src/emzed/r_connect/r_executor.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/table/__init__.py` & `emzed-3.0.0a9/src/emzed/table/__init__.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/table/add_column.py` & `emzed-3.0.0a9/src/emzed/table/add_column.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/table/base_models.py` & `emzed-3.0.0a9/src/emzed/table/base_models.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/table/col_types.py` & `emzed-3.0.0a9/src/emzed/table/col_types.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/table/collapse.py` & `emzed-3.0.0a9/src/emzed/table/collapse.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/table/delete_rows.py` & `emzed-3.0.0a9/src/emzed/table/delete_rows.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/table/expressions.py` & `emzed-3.0.0a9/src/emzed/table/expressions.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/table/extract_columns_model.py` & `emzed-3.0.0a9/src/emzed/table/extract_columns_model.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/table/filter_model.py` & `emzed-3.0.0a9/src/emzed/table/filter_model.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/table/full_table_model.py` & `emzed-3.0.0a9/src/emzed/table/full_table_model.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/table/group_by.py` & `emzed-3.0.0a9/src/emzed/table/group_by.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/table/immutable_table_model.py` & `emzed-3.0.0a9/src/emzed/table/immutable_table_model.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/table/join.py` & `emzed-3.0.0a9/src/emzed/table/join.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/table/load_into_from.py` & `emzed-3.0.0a9/src/emzed/table/load_into_from.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/table/prepare_table_cell_content.py` & `emzed-3.0.0a9/src/emzed/table/prepare_table_cell_content.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/table/replace_column.py` & `emzed-3.0.0a9/src/emzed/table/replace_column.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/table/row_class.py` & `emzed-3.0.0a9/src/emzed/table/row_class.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/table/select_model.py` & `emzed-3.0.0a9/src/emzed/table/select_model.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/table/sort_model.py` & `emzed-3.0.0a9/src/emzed/table/sort_model.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/table/table.py` & `emzed-3.0.0a9/src/emzed/table/table.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/table/table_migrations.py` & `emzed-3.0.0a9/src/emzed/table/table_migrations.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/table/table_utils.py` & `emzed-3.0.0a9/src/emzed/table/table_utils.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/targeted/solution_space.py` & `emzed-3.0.0a9/src/emzed/targeted/solution_space.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/utils/__init__.py` & `emzed-3.0.0a9/src/emzed/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/utils/align_spectra.py` & `emzed-3.0.0a9/src/emzed/utils/align_spectra.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/utils/busy_indicator.py` & `emzed-3.0.0a9/src/emzed/utils/busy_indicator.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/utils/functools.py` & `emzed-3.0.0a9/src/emzed/utils/functools.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/utils/has_emzed_gui.py` & `emzed-3.0.0a9/src/emzed/utils/has_emzed_gui.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/utils/lookup.py` & `emzed-3.0.0a9/src/emzed/utils/lookup.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed/utils/sqlite.py` & `emzed-3.0.0a9/src/emzed/utils/sqlite.py`

 * *Files identical despite different names*

### Comparing `emzed-3.0.0a8/src/emzed.egg-info/SOURCES.txt` & `emzed-3.0.0a9/src/emzed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

