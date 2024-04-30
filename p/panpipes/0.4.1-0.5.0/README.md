# Comparing `tmp/panpipes-0.4.1.tar.gz` & `tmp/panpipes-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panpipes-0.4.1.tar", last modified: Fri Dec  1 14:30:48 2023, max compression
+gzip compressed data, was "panpipes-0.5.0.tar", last modified: Tue Apr 30 15:32:01 2024, max compression
```

## Comparing `panpipes-0.4.1.tar` & `panpipes-0.5.0.tar`

### file list

```diff
@@ -1,141 +1,145 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-01 14:30:48.608026 panpipes-0.4.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1518 2023-12-01 14:30:13.000000 panpipes-0.4.1/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3826 2023-12-01 14:30:48.608026 panpipes-0.4.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2190 2023-12-01 14:30:13.000000 panpipes-0.4.1/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-01 14:30:48.592026 panpipes-0.4.1/panpipes/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-01 14:30:48.592026 panpipes-0.4.1/panpipes/R_scripts/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/R_scripts/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      553 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/R_scripts/install_R_libs.R
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20671 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/R_scripts/plotQC.R
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8292 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/R_scripts/plot_cluster_metrics.R
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8135 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/R_scripts/plot_metrics.R
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1165 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/R_scripts/plotclustree.R
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9674 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/R_scripts/produce_barplot_10xmetric.v3.R
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4460 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/R_scripts/refmap_wnn.R
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2504 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/entry.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-01 14:30:48.596026 panpipes-0.4.1/panpipes/funcs/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      101 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/funcs/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26482 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/funcs/io.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14766 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/funcs/plotting.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14463 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/funcs/processing.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22380 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/funcs/scmethods.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/funcs.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-01 14:30:48.596026 panpipes-0.4.1/panpipes/panpipes/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/panpipes/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-01 14:30:48.596026 panpipes-0.4.1/panpipes/panpipes/pipeline_clustering/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7644 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/panpipes/pipeline_clustering/pipeline.yml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16065 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/panpipes/pipeline_clustering.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-01 14:30:48.596026 panpipes-0.4.1/panpipes/panpipes/pipeline_deconvolution_spatial/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5634 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/panpipes/pipeline_deconvolution_spatial/pipeline.yml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5310 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/panpipes/pipeline_deconvolution_spatial.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-01 14:30:48.596026 panpipes-0.4.1/panpipes/panpipes/pipeline_ingest/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19149 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/panpipes/pipeline_ingest/pipeline.yml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24639 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/panpipes/pipeline_ingest.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-01 14:30:48.596026 panpipes-0.4.1/panpipes/panpipes/pipeline_integration/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14534 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/panpipes/pipeline_integration/pipeline.yml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34124 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/panpipes/pipeline_integration.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-01 14:30:48.596026 panpipes-0.4.1/panpipes/panpipes/pipeline_preprocess/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15212 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/panpipes/pipeline_preprocess/pipeline.yml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10845 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/panpipes/pipeline_preprocess.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-01 14:30:48.596026 panpipes-0.4.1/panpipes/panpipes/pipeline_preprocess_spatial/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5820 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/panpipes/pipeline_preprocess_spatial/pipeline.yml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6233 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/panpipes/pipeline_preprocess_spatial.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-01 14:30:48.596026 panpipes-0.4.1/panpipes/panpipes/pipeline_qc_spatial/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4027 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/panpipes/pipeline_qc_spatial/pipeline.yml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7249 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/panpipes/pipeline_qc_spatial.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-01 14:30:48.596026 panpipes-0.4.1/panpipes/panpipes/pipeline_refmap/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4943 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/panpipes/pipeline_refmap/pipeline.yml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6047 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/panpipes/pipeline_refmap.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-01 14:30:48.596026 panpipes-0.4.1/panpipes/panpipes/pipeline_vis/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4862 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/panpipes/pipeline_vis/pipeline.yml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9114 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/panpipes/pipeline_vis.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-01 14:30:48.604026 panpipes-0.4.1/panpipes/python_scripts/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12225 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/aggregate_cellranger_summary_metrics.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2811 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/aggregate_csvs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9277 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/assess_background.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4384 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/batch_correct_bbknn.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3294 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/batch_correct_combat.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5569 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/batch_correct_harmony.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3314 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/batch_correct_merge.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6341 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/batch_correct_mofa.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9217 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/batch_correct_multivi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4213 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/batch_correct_none.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5441 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/batch_correct_scanorama.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6210 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/batch_correct_scvi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9849 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/batch_correct_totalvi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8102 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/batch_correct_wnn.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3071 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/collate_mdata.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8592 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/concat_adata.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2720 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/downsample.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3350 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/generate_cellxgene.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1841 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/integrate_wnn.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6388 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/make_adata_from_csv.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6077 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/make_mudataspatial_from_csv.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       80 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/plot_atac_qc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3796 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/plot_cluster_umaps.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5215 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/plot_custom_markers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3831 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/plot_custom_markers_umap.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2045 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/plot_features_scatter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1795 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/plot_pca.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5310 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/plot_qc_spatial.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4261 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/plot_scanpy_markers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7614 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/plot_umaps_batch_correct.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3747 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/plot_variables_umaps.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2846 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/refmap_generatescanvi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1469 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/refmap_plot_umaps.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3668 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/refmap_scib.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15781 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/refmap_scvitools.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3302 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/rerun_find_neighbors_for_clustering.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11959 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/run_cell2location.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2535 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/run_clustering.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5167 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/run_collate_mtd_files.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       69 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/run_differential_peaks_ATAC.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8791 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/run_dsb_clr.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7719 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/run_filter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7014 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/run_filter_spatial.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6716 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/run_find_markers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9111 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/run_find_markers_multi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2763 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/run_find_neighbors.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4183 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/run_lisi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8706 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/run_preprocess_atac.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13206 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/run_preprocess_prot.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8821 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/run_preprocess_rna.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6063 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/run_preprocess_spatial.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6239 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/run_scanpyQC_atac.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6259 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/run_scanpyQC_prot.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4527 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/run_scanpyQC_rep.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5782 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/run_scanpyQC_rna.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5246 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/run_scanpyQC_spatial.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3754 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/run_scib_metrics.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5720 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/run_scrublet_scores.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2598 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/run_umap.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2872 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/subtract_scrublet.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      756 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/python_scripts/write_metadata.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-01 14:30:48.608026 panpipes-0.4.1/panpipes/resources/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/resources/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      877 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/resources/cell_cycle_genes.tsv
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9169 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/resources/metrics_summary_col_conversion.tsv
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22859 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/resources/qc_genelist_1.0.csv
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      438 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/resources/sample_file_inc_demultiplexing.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      367 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/resources/sample_file_qc_atac.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      264 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/resources/sample_file_qc_mm.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      264 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/resources/sample_file_qc_mm_gex_only.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      391 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/resources/sample_file_qc_multiome.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      341 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/resources/sample_file_qc_multiome_cellranger.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      530 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/resources/sample_file_qc_spatial.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-12-01 14:30:13.000000 panpipes-0.4.1/panpipes/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-01 14:30:48.608026 panpipes-0.4.1/panpipes.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3826 2023-12-01 14:30:48.000000 panpipes-0.4.1/panpipes.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5005 2023-12-01 14:30:48.000000 panpipes-0.4.1/panpipes.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-12-01 14:30:48.000000 panpipes-0.4.1/panpipes.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       49 2023-12-01 14:30:48.000000 panpipes-0.4.1/panpipes.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      413 2023-12-01 14:30:48.000000 panpipes-0.4.1/panpipes.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-12-01 14:30:48.000000 panpipes-0.4.1/panpipes.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2321 2023-12-01 14:30:13.000000 panpipes-0.4.1/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-12-01 14:30:48.608026 panpipes-0.4.1/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-01 14:30:48.608026 panpipes-0.4.1/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      982 2023-12-01 14:30:13.000000 panpipes-0.4.1/tests/test_anndata.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2062 2023-12-01 14:30:13.000000 panpipes-0.4.1/tests/test_ingest_funcs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7785 2023-12-01 14:30:13.000000 panpipes-0.4.1/tests/test_processing.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 15:32:01.722044 panpipes-0.5.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1518 2024-04-30 15:26:28.000000 panpipes-0.5.0/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5419 2024-04-30 15:32:01.722044 panpipes-0.5.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3394 2024-04-30 15:26:28.000000 panpipes-0.5.0/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 15:32:01.702044 panpipes-0.5.0/panpipes/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 15:32:01.702044 panpipes-0.5.0/panpipes/R_scripts/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/R_scripts/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      553 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/R_scripts/install_R_libs.R
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21808 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/R_scripts/plotQC.R
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8292 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/R_scripts/plot_cluster_metrics.R
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8632 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/R_scripts/plot_metrics.R
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1205 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/R_scripts/plotclustree.R
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9674 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/R_scripts/produce_barplot_10xmetric.v3.R
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4460 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/R_scripts/refmap_wnn.R
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2504 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/entry.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 15:32:01.702044 panpipes-0.5.0/panpipes/funcs/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      101 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/funcs/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26482 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/funcs/io.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17669 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/funcs/plotting.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14463 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/funcs/processing.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22380 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/funcs/scmethods.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/funcs.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 15:32:01.706044 panpipes-0.5.0/panpipes/panpipes/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/panpipes/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 15:32:01.706044 panpipes-0.5.0/panpipes/panpipes/pipeline_clustering/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4135 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/panpipes/pipeline_clustering/pipeline.yml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17687 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/panpipes/pipeline_clustering.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 15:32:01.706044 panpipes-0.5.0/panpipes/panpipes/pipeline_deconvolution_spatial/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7733 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/panpipes/pipeline_deconvolution_spatial/pipeline.yml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8959 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/panpipes/pipeline_deconvolution_spatial.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 15:32:01.706044 panpipes-0.5.0/panpipes/panpipes/pipeline_ingest/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5352 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/panpipes/pipeline_ingest/pipeline.yml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27113 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/panpipes/pipeline_ingest.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 15:32:01.706044 panpipes-0.5.0/panpipes/panpipes/pipeline_integration/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5344 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/panpipes/pipeline_integration/pipeline.yml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    38695 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/panpipes/pipeline_integration.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 15:32:01.706044 panpipes-0.5.0/panpipes/panpipes/pipeline_preprocess/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4733 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/panpipes/pipeline_preprocess/pipeline.yml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11859 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/panpipes/pipeline_preprocess.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 15:32:01.706044 panpipes-0.5.0/panpipes/panpipes/pipeline_preprocess_spatial/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5870 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/panpipes/pipeline_preprocess_spatial/pipeline.yml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6755 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/panpipes/pipeline_preprocess_spatial.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 15:32:01.706044 panpipes-0.5.0/panpipes/panpipes/pipeline_qc_spatial/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4025 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/panpipes/pipeline_qc_spatial/pipeline.yml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7784 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/panpipes/pipeline_qc_spatial.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 15:32:01.706044 panpipes-0.5.0/panpipes/panpipes/pipeline_refmap/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4944 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/panpipes/pipeline_refmap/pipeline.yml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6674 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/panpipes/pipeline_refmap.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 15:32:01.706044 panpipes-0.5.0/panpipes/panpipes/pipeline_vis/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4862 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/panpipes/pipeline_vis/pipeline.yml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10317 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/panpipes/pipeline_vis.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 15:32:01.718044 panpipes-0.5.0/panpipes/python_scripts/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12887 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/aggregate_cellranger_summary_metrics.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3049 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/aggregate_csvs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10032 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/assess_background.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4573 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/batch_correct_bbknn.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3432 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/batch_correct_combat.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5696 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/batch_correct_harmony.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3489 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/batch_correct_merge.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6699 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/batch_correct_mofa.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10217 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/batch_correct_multivi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4148 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/batch_correct_none.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5537 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/batch_correct_scanorama.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7096 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/batch_correct_scvi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11306 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/batch_correct_totalvi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8288 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/batch_correct_wnn.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3396 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/collate_mdata.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8789 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/concat_adata.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2885 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/downsample.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3350 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/generate_cellxgene.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1841 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/integrate_wnn.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6948 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/make_adata_from_csv.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6408 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/make_mudataspatial_from_csv.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       80 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/plot_atac_qc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4183 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/plot_cluster_umaps.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5791 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/plot_custom_markers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3939 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/plot_custom_markers_umap.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2325 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/plot_features_scatter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1795 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/plot_pca.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5749 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/plot_qc_spatial.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5271 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/plot_scanpy_markers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8067 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/plot_umaps_batch_correct.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3884 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/plot_variables_umaps.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2846 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/refmap_generatescanvi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1469 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/refmap_plot_umaps.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4151 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/refmap_scib.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17553 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/refmap_scvitools.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3693 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/rerun_find_neighbors_for_clustering.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13963 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/run_cell2location.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3270 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/run_clustering.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5289 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/run_collate_mtd_files.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       69 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/run_differential_peaks_ATAC.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8791 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/run_dsb_clr.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8344 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/run_filter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7140 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/run_filter_spatial.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6716 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/run_find_markers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9685 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/run_find_markers_multi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2763 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/run_find_neighbors.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4422 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/run_lisi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9889 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/run_preprocess_atac.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13809 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/run_preprocess_prot.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9004 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/run_preprocess_rna.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6820 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/run_preprocess_spatial.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7210 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/run_scanpyQC_atac.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6924 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/run_scanpyQC_prot.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4969 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/run_scanpyQC_rep.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6913 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/run_scanpyQC_rna.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6441 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/run_scanpyQC_spatial.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5165 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/run_scib.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3754 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/run_scib_metrics.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5891 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/run_scrublet_scores.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6324 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/run_tangram.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2912 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/run_umap.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2872 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/subtract_scrublet.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      893 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/python_scripts/write_metadata.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 15:32:01.718044 panpipes-0.5.0/panpipes/resources/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/resources/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      877 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/resources/cell_cycle_genes.tsv
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9169 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/resources/metrics_summary_col_conversion.tsv
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1159 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/resources/mouse_cell_cycle_genes.tsv
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4280 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/resources/qc_gene_list_mouse.csv
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22859 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/resources/qc_genelist_1.0.csv
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      438 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/resources/sample_file_inc_demultiplexing.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      367 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/resources/sample_file_qc_atac.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      264 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/resources/sample_file_qc_mm.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      264 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/resources/sample_file_qc_mm_gex_only.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      391 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/resources/sample_file_qc_multiome.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      341 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/resources/sample_file_qc_multiome_cellranger.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      530 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/resources/sample_file_qc_spatial.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2024-04-30 15:26:28.000000 panpipes-0.5.0/panpipes/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 15:32:01.718044 panpipes-0.5.0/panpipes.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5419 2024-04-30 15:32:01.000000 panpipes-0.5.0/panpipes.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5168 2024-04-30 15:32:01.000000 panpipes-0.5.0/panpipes.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-30 15:32:01.000000 panpipes-0.5.0/panpipes.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       49 2024-04-30 15:32:01.000000 panpipes-0.5.0/panpipes.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      465 2024-04-30 15:32:01.000000 panpipes-0.5.0/panpipes.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-04-30 15:32:01.000000 panpipes-0.5.0/panpipes.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1565 2024-04-30 15:26:51.000000 panpipes-0.5.0/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-30 15:32:01.722044 panpipes-0.5.0/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 15:32:01.718044 panpipes-0.5.0/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      982 2024-04-30 15:26:28.000000 panpipes-0.5.0/tests/test_anndata.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2062 2024-04-30 15:26:28.000000 panpipes-0.5.0/tests/test_ingest_funcs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7785 2024-04-30 15:26:28.000000 panpipes-0.5.0/tests/test_processing.py
```

### Comparing `panpipes-0.4.1/LICENSE` & `panpipes-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `panpipes-0.4.1/panpipes/R_scripts/install_R_libs.R` & `panpipes-0.5.0/panpipes/R_scripts/install_R_libs.R`

 * *Files identical despite different names*

### Comparing `panpipes-0.4.1/panpipes/R_scripts/plotQC.R` & `panpipes-0.5.0/panpipes/R_scripts/plotQC.R`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     {if(qc=="doublet_scores") geom_hline(yintercept=0.25, color="grey50", linetype="dashed") }+
     {if("pct_counts" %in% qc) geom_hline(yintercept=c(5, 10, 20 ,70), color="grey50", linetype="dashed")}+
     {if("pct_counts" %in% qc) coord_cartesian(ylim=c(0,100))}+
     theme_bw()+
     theme(axis.text.x=element_text(size=8, angle=90),
           axis.text.y=element_text(size=8))
   if(length(unique(df[[group]])) > 10){
-    message(paste0(sc, "has too many categories, removing legend"))
+    print(paste(sc, "has too many categories, removing legend"))
     g <- g + theme(legend.position="none")
   }
   
   return(g)
 }
 
 do_bar_plot <- function(df, qc, group){
@@ -78,23 +78,20 @@
   make_option(c("--sampleprefix"), default="",
               help="the prefix to prepend to save summary filtering plots"),
   make_option(c("--scanpy_or_muon"), default="scanpy", 
               help="was the input file written out from the obs of scanpy or muon")
 )
 
 
-message("Plot QC data")
 opt <- parse_args(OptionParser(option_list=option_list))
 
 if(is.null(opt$outdir)) { opt$outdir <- paste0(getwd(),"/")}
 if(!grepl("\\/$", opt$outdir)){opt$outdir <- paste(opt$outdir, "/", sep = "")}
 if(!file.exists(opt$outdir)){dir.create(opt$outdir)}
 
-print("Running with options:")
-print(opt)
 
 run<- opt$outdir
 opt[which(opt=="NULL")] <- NULL
 opt[which(opt=="None")] <- NULL
 opt$prefilter <- as.logical(opt$prefilter)
 
 # load_data --------------------------------------------------------------------
@@ -114,24 +111,24 @@
       }
     }
   }
 
   source_facet <- source_facet[source_facet %in% colnames(data_plot)]
   source_facet <- unique(c(source_facet, keep_source) )
   if(length(source_facet)>0){
-    print("Facet plotting with")
     # add sample_id as a minimum requirement if it's not there already
     source_facet = unique(c("sample_id", source_facet))
-    print(source_facet)
+    print(paste("Facet plotting with",source_facet))
   }
 }else{
-  stop("i don't have the minimum variable _sampleid_ to facet on, will stop here")
+  stop("Need the minimum variable _sampleid_ to facet on, will stop here")
 }
 # RNA plots --------------------------------------------------------------------
 
+print("RNA plots")
 
 if(opt$scanpy_or_muon=="scanpy"){
   rna_data_plot <- data_plot
 }else{
   rna_data_plot <- data_plot[,grep("^rna\\.",colnames(data_plot))]
   colnames(rna_data_plot) <- gsub("^rna\\.", "", colnames(rna_data_plot))
 }
@@ -158,17 +155,16 @@
 }
 qcmetrics <- qcmetrics[qcmetrics %in% colnames(rna_data_plot)]
 uniq_sample_id <- nrow(unique(rna_data_plot["sample_id"]))
 rna_source_facet <- gsub("^rna\\.", "",grep("^rna.", source_facet, value = TRUE))
 rna_source_facet <- unique(c(rna_source_facet, source_facet[!grepl("^rna.", source_facet)]))
 rna_source_facet <- rna_source_facet[rna_source_facet %in% colnames(rna_data_plot)]
 for (qc in qcmetrics){
-  print(qc)
+  print(paste("Plotting violin plots of", qc))
   for (sc in rna_source_facet){ #add gsub temp here
-    print(sc)
     g <- do_violin_plot(rna_data_plot, qc, sc)
     if (uniq_sample_id  > 50){width=12}else{width=6}
     ggsave(g, filename=file.path(outpath, paste0("violin_", sc, "_rna-", qc,".png")), type="cairo", width= width, height=6)
     
   }
 }
 
@@ -179,45 +175,51 @@
     nrows=ceiling(uniq_source/6)
   }else{
     ncols=uniq_source
     nrows=1
   }
   # plot once per source facet
   if (all(c("total_counts","n_genes_by_counts")%in% colnames(rna_data_plot))){
+    print("Plotting scatter plot of total_counts and n_genes_by_counts")
     g <- do_scatter_plot(rna_data_plot,x="total_counts",y="n_genes_by_counts", facet=sc)
     ggsave(g, filename=file.path(outpath, paste0("scatter_", sc, "_rna-nUMI_v_rna-genes.png")), type="cairo",
            width= 3*ncols, height=3*nrows, dpi=200)
   }
   
   if (all(c("log1p_total_counts","log1p_n_genes_by_counts")%in% colnames(rna_data_plot))){
-    
+    print("Plotting scatter plot of log1p_total_counts and n_genes_by_counts")
     g <- do_scatter_plot(rna_data_plot,x="log1p_total_counts",y="log1p_n_genes_by_counts", facet=sc)
     ggsave(g, filename=file.path(outpath, paste0("scatter_", sc, "_rna-log1p_nUMI_v_rna-log1p_genes.png")), type="cairo",
            width= 3*ncols, height=3*nrows, dpi=200)
   }
   if (all(c("total_counts","pct_counts_mt")%in% colnames(rna_data_plot))){
+    print("Plotting scatter plot of total_counts and pct_counts_mt")
     g <- do_scatter_plot(rna_data_plot,x="total_counts",y="pct_counts_mt", facet=sc)
     ggsave(g, filename=file.path(outpath, paste0("scatter_", sc, "_rna-nUMI_v_rna-pct_mt.png")), type="cairo",
            width= 3*ncols, height=3*nrows, dpi=200)
   }
   if (all(c("n_genes_by_counts","doublet_scores","total_counts")%in% colnames(rna_data_plot))){
+    print("Plotting scatter plot of n_genes_by_counts and doublet_scores")
     g <- do_scatter_plot(rna_data_plot,x="n_genes_by_counts",y="doublet_scores",
                          hue="total_counts", facet=sc)
     ggsave(g, filename=file.path(outpath, paste0("scatter_", sc, "_rna-genes_rna-doublet_scores_rna-numi.png")),    
            type="cairo", width= 3*ncols, height=3*nrows, dpi=200)
   }
   
 }
 
 
 
 # Protein plots ----------------------------------------------------------------
 
 
+
 if(!is.null(opt$prot_qc_metrics)){
+  print("Protein plots")
+
   qcmetrics <- strsplit(opt$prot_qc_metrics,",")[[1]]
   prot_data_plot <- data_plot[,grep("^prot\\.",colnames(data_plot))]
   colnames(prot_data_plot) <- gsub("^prot\\.", "", colnames(prot_data_plot))
   prot_source_facet <- gsub("^prot\\.", "",grep("^prot.", source_facet, value = TRUE))
   prot_source_facet <- unique(c(prot_source_facet, source_facet[!grepl("^prot.", source_facet)]))
   prot_source_facet <- prot_source_facet[prot_source_facet %in% colnames(prot_data_plot)]
 
@@ -226,15 +228,15 @@
     dir.create(outpath)
     }
   uniq_sample_id <- nrow(unique(prot_data_plot["sample_id"]))
 
   # check these qc metrics are in the file
   qcmetrics <- qcmetrics[qcmetrics %in% colnames(prot_data_plot)]
   for (qc in qcmetrics){
-    print(qc)
+    print(paste("Plotting violin plots of", qc))
     for (sc in prot_source_facet){
       g <- do_violin_plot(prot_data_plot, qc, sc)
       if (uniq_sample_id  > 50){width=12}else{width=6}
       ggsave(g, filename=file.path(outpath, paste0("violin_", sc, "_prot-", qc,".png")), type="cairo", width= width, height=6)
     }
   }
   
@@ -251,48 +253,53 @@
       ncols=6
       nrows=ceiling(uniq_source/6)
     }else{
       ncols=uniq_source
       nrows=1
     }
     # plot once per source facet
-    message("protein scatter plots")  
+
     if (all(c("total_counts","n_prot_by_counts")%in% colnames(prot_data_plot))){
+      print("Plotting scatter plot of total_counts and n_prot_by_counts")
       g <- do_scatter_plot(prot_data_plot,x="total_counts",y="n_prot_by_counts", facet=sc)
       ggsave(g, filename=file.path(outpath, paste0("scatter_", sc, "_prot-nUMI_v_prot-prot.png")), type="cairo",
              width= 3*ncols, height=3*nrows, dpi=200)
     }
     if (all(c("log1p_total_counts","log1p_n_prot_by_counts")%in% colnames(prot_data_plot))){
+      print("Plotting scatter plot of log1p_total_counts and log1p_n_prot_by_counts")
       g <- do_scatter_plot(prot_data_plot,x="log1p_total_counts",y="log1p_n_prot_by_counts", facet=sc)
       ggsave(g, filename=file.path(outpath, paste0("scatter_", sc, "_prot-log1p_nUMI_v_prot-log1p_prot.png")), type="cairo",
              width= 3*ncols, height=3*nrows, dpi=200)
     }
     if (all(c("total_counts","pct_counts_isotype")%in% colnames(prot_data_plot))){
+      print("Plotting scatter plot of total_counts and pct_counts_isotype")
       g <- do_scatter_plot(prot_data_plot,x="total_counts",y="pct_counts_isotype", facet=sc)
       ggsave(g, filename=file.path(outpath, paste0("scatter_", sc, "_prot-nUMI_v_prot-pct_isotype.png")), type="cairo",
              width= 3*ncols, height=3*nrows, dpi=200)
     }
     if (all(c("total_counts","total_counts_isotype")%in% colnames(prot_data_plot))){
+      print("Plotting scatter plot of total_counts and total_counts_isotype")
       g <- do_scatter_plot(prot_data_plot,x="total_counts",y="total_counts_isotype", facet=sc)
       ggsave(g, filename=file.path(outpath, paste0("scatter_", sc, "_prot-nUMI_v_prot-total_counts_isotype.png")), type="cairo",
              width= 3*ncols, height=3*nrows, dpi=200)
     }
     if (all(c("log1p_total_counts","log1p_total_counts_isotype", "isotype_exclude")%in% colnames(prot_data_plot))){
+      print("Plotting scatter plot of log1p_total_counts and log1p_total_counts_isotype")
       g <- do_scatter_plot(prot_data_plot,x="log1p_total_counts",y="log1p_total_counts_isotype", hue="isotype_exclude", facet=sc)
       ggsave(g, filename=file.path(outpath, paste0("scatter_", sc, "_prot-log1p_nUMI_v_prot-log1p_total_counts_isotype.png")), type="cairo",
              width= 3*ncols, height=3*nrows, dpi=200)
     }
   }
 
 }
 # Atac plots ----------------------------------------------------------------
 
 
 if(!is.null(opt$atac_qc_metrics)){
-  message("Atac plots")
+  print("ATAC plots")
   atac_data_plot <- data_plot[,grep("^atac\\.",colnames(data_plot))]
   colnames(atac_data_plot) <- gsub("^atac\\.", "", colnames(atac_data_plot))
   atac_source_facet <- gsub("^atac\\.", "",grep("^atac.", source_facet, value = TRUE))
   atac_source_facet <- unique(c(atac_source_facet, source_facet[!grepl("^atac.", source_facet)]))
   atac_source_facet <- atac_source_facet[atac_source_facet %in% colnames(atac_data_plot)]
 
 
@@ -300,28 +307,28 @@
   if (!dir.exists(outpath)) dir.create(outpath)
   
   uniq_sample_id <- nrow(unique(atac_data_plot["sample_id"]))
 
   # check these qc metrics are in the file
   qcmetrics <- qcmetrics[qcmetrics %in% colnames(atac_data_plot)]
   for (qc in qcmetrics){
-    print(qc)
+    print(paste("Plotting violin plots of", qc))
     for (sc in atac_source_facet){
       g <- do_violin_plot(atac_data_plot, qc, sc)
       if (uniq_sample_id  > 50){width=12}else{width=6}
       ggsave(g, filename=file.path(outpath, paste0("violin_", sc, "_atac-", qc,".png")), type="cairo", width= width, height=6)
     }
   }
 }
   
 # Rep plots ----------------------------------------------------------------
 
 
 if (!is.null(opt$rep_qc_metrics)) {
-  message("Repertoire plots")
+  print("Repertoire plots")
   qcmetrics <- strsplit(opt$rep_qc_metrics,",")[[1]]
   qcmetrics <- gsub("rep:", "", qcmetrics)
   rep_data_plot <- data_plot[,grep("^rep\\.",colnames(data_plot))]
   colnames(rep_data_plot) <- gsub("^rep\\.", "", colnames(rep_data_plot))
   rep_data_plot = rep_data_plot %>% filter(sample_id!="")
   
   rep_source_facet <- gsub("^rep\\.", "",grep("^rep.", source_facet, value = TRUE))
@@ -334,14 +341,15 @@
   
   
   uniq_sample_id <- nrow(unique(rep_data_plot["sample_id"]))
 
   # check these qc metrics are in the file
   qcmetrics <- qcmetrics[qcmetrics %in% colnames(rep_data_plot)]
   for (qc in qcmetrics){
+    print(paste("Plotting bar plots of", qc))
     for (sc in rep_source_facet){
       g <- do_bar_plot(rep_data_plot, qc, sc)
       if (uniq_sample_id  > 50){width=12}else{width=6}
         ggsave(g, filename=file.path(outpath, paste0("bar_", sc, "_rep-", qc,".png")), type="cairo", width= width, height=6)
 
       if (!(qc %in% c('has_ir', "receptor_type"))){
         g <- do_bar_plot(rep_data_plot, qc, sc) + facet_grid(~receptor_type)
@@ -350,73 +358,74 @@
       }
     }
   }
 }
 
 
 if(!is.null(opt$prot_qc_metrics)){
+print("RNA vs. Protein plots")
 
 # rna vs prot plots ----------------------------------------------------------------
   
 
   outpath = file.path(run, "rna_v_prot")
   if (!dir.exists(outpath)) dir.create(outpath)    
   
 
   for (sc in source_facet){
-    
-    message(sc)
     uniq_source <- nrow(unique(data_plot[sc]))
     if(uniq_source >6){
       ncols=6
       nrows=ceiling(uniq_source/6)
     }else{
       ncols=uniq_source
       nrows=1
     }
-    message("rna v protein scatter plots")  
     if (all(c("rna.total_counts","prot.total_counts")%in% colnames(data_plot))){
+      print("Plotting scatter plot of rna.total_counts and prot.total_counts")
       g <- do_scatter_plot(data_plot,x="rna.total_counts",y="prot.total_counts", facet=sc)
       ggsave(g, filename=file.path(outpath, paste0("scatter_", sc, "-nUMI_v_rna-nUMI.png")), type="cairo",
               width= 3*ncols, height=3*nrows, dpi=200)
     }
     if (all(c("rna.log1p_total_counts","prot.log1p_total_counts")%in% colnames(data_plot))){
+      print("Plotting scatter plot of rna.log1p_total_counts and prot.log1p_total_counts")
       g <- do_scatter_plot(data_plot,x="rna.log1p_total_counts",y="prot.log1p_total_counts", facet=sc)
       ggsave(g, filename=file.path(outpath, paste0("scatter_", sc, "-log1p_nUMI_v_rna-log1p_nUMI.png")), type="cairo",
               width= 3*ncols, height=3*nrows, dpi=200)
     }
     if (all(c("rna.total_counts","prot.total_counts_isotype")%in% colnames(data_plot))){
+      print("Plotting scatter plot of rna.total_counts and prot.total_counts_isotype")
       g <-  do_scatter_plot(data_plot,x="rna.total_counts",y="prot.total_counts_isotype", facet=sc)
       ggsave(g, filename=file.path(outpath, paste0("scatter_", sc, "-nUMI_v_prot-counts_isotype.png")), type="cairo",
               width= 3*ncols, height=3*nrows, dpi=200)
     }    
     if (all(c("rna.log1p_total_counts","prot.log1p_total_counts_isotype") %in% colnames(data_plot))){
+      print("Plotting scatter plot of rna.log1p_total_counts and prot.log1p_total_counts_isotype")
       g <-  do_scatter_plot(data_plot,x="rna.log1p_total_counts",y="prot.log1p_total_counts_isotype", facet=sc)
       ggsave(g, filename=file.path(outpath, paste0("scatter_", sc, "-log1p_nUMI_v_prot-log1p_counts_isotype.png")), type="cairo",
               width= 3*ncols, height=3*nrows, dpi=200)
     }
     if (all(c("rna.doublet_scores","prot.log1p_total_counts") %in% colnames(data_plot))){
+      print("Plotting scatter plot of rna.doublet_scores and prot.log1p_total_counts")
       g <-  do_scatter_plot(data_plot,x="rna.doublet_scores",y="prot.log1p_total_counts", facet=sc)
       ggsave(g, filename=file.path(outpath, paste0("scatter_", sc, "-doublet_scores_v_prot-log1p_nUMI.png")), type="cairo",
               width= 3*ncols, height=3*nrows, dpi=200)
       
     }
     
     
   }
   
 }
 
 
 sprefix <- opt$sampleprefix
-print(sprefix)
-message ("saving some counts tables for references")
-
 
 if(opt$prefilter){
+  print("Saving counts tables for references")
   if(all(c("pct_counts_mt", "pct_counts_hb", "n_genes_by_counts", "doublet_scores") %in% colnames(rna_data_plot))){
     f1 <- rna_data_plot %>% 
       dplyr::filter(pct_counts_mt<=20 & pct_counts_hb<=70 &n_genes_by_counts>=100 & doublet_scores<=0.25) %>%
       group_by_at(.vars=c(rna_source_facet)) %>%
       group_by_at(.vars=c(rna_source_facet)) %>%
       summarise(cell.count= n()) %>%
       group_by_at(.vars="sample_id") %>% 
@@ -476,15 +485,15 @@
                         limits=c("percent_retain_f1","percent_retain_f2","percent_retain_f3")) + 
       coord_cartesian(ylim=c(0,100)) 
     
     ggsave(g, file = paste0(run,"barplot_cellcounts_thresholds_filter.png"), type="cairo", width=9, height=9)
   }
   
 }else{
-  message("producing files with final counts for cells after filtering")
+  print("Producing files with final counts for cells after filtering")
   
   baseline <- rna_data_plot %>% 
     group_by_at(.vars=c(rna_source_facet)) %>% 
     summarise(cell.count= n()) %>% 
     group_by_at(.vars="sample_id") 
   
   write.table(baseline, file=paste0( sprefix,"_filtered_data.tsv"), col.names=T, row.names=F, sep="\t", quote=F)
@@ -496,8 +505,8 @@
     theme(axis.text.x=element_text(size=8,angle=45, hjust=1.05, vjust=0.95),
           axis.text.y=element_text(size=13)) 
   ggsave(g, file = file.path(run, "rna","barplot_cellcounts_filtered_data.png"), type="cairo", width=9, height=6)
   
 }
 
 
-message("done")
+print("Done")
```

### Comparing `panpipes-0.4.1/panpipes/R_scripts/plot_cluster_metrics.R` & `panpipes-0.5.0/panpipes/R_scripts/plot_cluster_metrics.R`

 * *Files identical despite different names*

### Comparing `panpipes-0.4.1/panpipes/R_scripts/plot_metrics.R` & `panpipes-0.5.0/panpipes/R_scripts/plot_metrics.R`

 * *Files 4% similar despite different names*

```diff
@@ -43,20 +43,23 @@
 	cmtd %<>% mutate(across(grp_vars$variable, factor))
 	return(cmtd)
 }
 
 parse_vars <- function(cat_vars){
     if (is.list(cat_vars)){
         uniq_cat_vars <- unique(unlist(cat_vars))
-        uniq_cat_vars
-        # cat vars
+        if (!is.null(uniq_cat_vars)){
         cat_split = data.frame(str_split(uniq_cat_vars, ":", simplify = T)) %>%
             mutate(mod =ifelse(X1 %in% c('rna', 'prot', 'atac', 'rep'), X1, "multimodal"),
                         variable = gsub(":", "_", uniq_cat_vars)) %>% 
             select(mod, variable)
+        }
+        else{
+            cat_split = NULL
+        }
     }else{
         cat_split = data.frame(variable=gsub(":", "_", cat_vars))
     }
 	return(cat_split)
 }
 
 # Get options ----------------------------------------------------------------
@@ -83,18 +86,18 @@
 cat_vars = parse_vars(PARAMS$categorical_vars)
 
 cmtd <- parse_cell_metadata(cmtd, cat_vars, grp_vars)
 
 
 
 # Barplots ----------------------------------------------------------------
-if( PARAMS$do_plots$categorical_barplots){
+if( PARAMS$do_plots$categorical_barplots & !is.null(cat_vars)){
     for( mod in unique(cat_vars$mod)){
         if (!dir.exists(file.path(mod))) dir.create(file.path(mod))
-        print(mod)
+        print(paste("Plotting barplots for modality", mod))
         uniq_cat_vars = cat_vars[cat_vars$mod == mod, 'variable']
         
         for (cat_v in uniq_cat_vars){
             print(cat_v)
             plt_title <- cat_v
             plot_dat = cmtd %>% 
                 mutate(!! cat_v  := factor(!! rlang::sym(cat_v))) %>% 
@@ -111,37 +114,36 @@
                 scale_y_origin() + 
                 panpipes_theme() + 
                 theme(legend.position = "none")
             if (flip_axes){
                 p1 <- p1 + coord_flip()
             }
         
-        print(paste0("saving to: ", file.path(mod, paste0("bar_", cat_v, ".png"))))
+        print(paste0("Saving plot to: ", file.path(mod, paste0("bar_", cat_v, ".png"))))
         save_plot(filename=file.path(mod, paste0("bar_", cat_v, ".png")),
                             plot=p1, ncol=1, 
                             nrow=1,base_asp = 1.3, base_height = 5) 
     }
 }
 }
 # Stacked barplots by grouping var ----------------------------------------------------------------
-if( PARAMS$do_plots$categorical_stacked_barplots){
+if( PARAMS$do_plots$categorical_stacked_barplots & !is.null(cat_vars) & !is.null(grp_vars)){
 
     for( mod in unique(cat_vars$mod)){
-        print(mod)
+        print(paste("Plotting stacked barplots for modality", mod))
         uniq_cat_vars = cat_vars[cat_vars$mod == mod, 'variable']
         
         for( gv in grp_vars$variable){
-            print(gv)
             if (!dir.exists(file.path(mod, gv))) dir.create(file.path(mod, gv), recursive=T)
             stacked_barplots <- list()
         
             for (cat_v in uniq_cat_vars){
                 
                 if( gv == cat_v){
-                    print("skipping")
+                    #print("skipping")
                     next
                 }
                 
                 plot_dat = cmtd %>% select(!!sym(gv), !!sym(cat_v)) %>% 
                     drop_na() %>% 
                     group_by( !!sym(gv), !!sym(cat_v)) %>% 
                     summarise(n_cells=n()) %>% ungroup() %>% group_by(!!sym(gv)) %>% 
@@ -163,31 +165,32 @@
                     panpipes_theme(font_size = 10)
                 
                 if (flip_axes){
                     p1 <- p1 + coord_flip()
                     p2 <- p2 + coord_flip()
                 }
                 pg <- cowplot::plot_grid(p1, p2)
+                print(paste0("Saving plot to: ", file.path(mod, gv, paste0("stackedbar_", cat_v, ".png"))))
                 save_plot(filename=file.path(mod, gv, paste0("stackedbar_", cat_v, ".png")),
                                     plot=pg, ncol=2, 
                                     nrow=1, base_height = 5, 
                                     base_asp = ifelse(flip_axes, 1.5, 1.1)) 
             }
         }
         
         
     }
 }
 
 # Violin by grouping var ----------------------------------------------------------------
-if( PARAMS$do_plots$continuous_violin){
+if( PARAMS$do_plots$continuous_violin & !is.null(cont_vars) & !is.null(grp_vars)){
 
 
     for( mod in unique(cont_vars$mod)){
-        print(mod)
+        print(paste("Plotting violin plots for modality", mod))
         uniq_cont_vars = cont_vars[cont_vars$mod == mod, 'variable']
         
         for( gv in grp_vars$variable){
             print(gv)
             if (!dir.exists(file.path(mod, gv))) dir.create(file.path(mod, gv), recursive=T)
 
             stacked_barplots <- list()
@@ -210,15 +213,15 @@
                     scale_y_origin() + 
                     panpipes_theme(font_size = 10) 
                 
                 
                 if (flip_axes){
                     p1 <- p1 + coord_flip()
                 }
-
+                print(paste0("Saving plot to: ", file.path(mod, gv, paste0("violin_", cont_v, ".png"))))
                 save_plot(filename=file.path(mod, gv, paste0("violin_", cont_v, ".png")),
                                     plot=p1, ncol=1, 
                                     nrow=1, base_height = 5, 
                                     base_asp = ifelse(flip_axes, 1.5, 1.1)) 
             }
         }
```

### Comparing `panpipes-0.4.1/panpipes/R_scripts/plotclustree.R` & `panpipes-0.5.0/panpipes/R_scripts/plotclustree.R`

 * *Files 15% similar despite different names*

```diff
@@ -30,18 +30,20 @@
 
 # # run clustree
 m = readr::read_tsv(opt$infile)
 # this is a little dodge, but works ;) 
 example_column=colnames(m)[2]
 col_prefix=substr(example_column, 1, nchar(example_column)-3 )
 # run clustree
+print("Running Clustree")
 gg <- clustree(m, prefix =col_prefix) + ggtitle(opt$plot_title)
 
 
 if (!(dir.exists(dirname(opt$outfile)))){
 	dir.create(dirname(opt$outfile))
 }
 
 # save
+print("Saving Clustree")
 ggsave(gg, filename=opt$outfile, height=10,width=12, type="cairo")
 
-message("clustree done")
+print("Done")
```

### Comparing `panpipes-0.4.1/panpipes/R_scripts/produce_barplot_10xmetric.v3.R` & `panpipes-0.5.0/panpipes/R_scripts/produce_barplot_10xmetric.v3.R`

 * *Files identical despite different names*

### Comparing `panpipes-0.4.1/panpipes/R_scripts/refmap_wnn.R` & `panpipes-0.5.0/panpipes/R_scripts/refmap_wnn.R`

 * *Files identical despite different names*

### Comparing `panpipes-0.4.1/panpipes/entry.py` & `panpipes-0.5.0/panpipes/entry.py`

 * *Files identical despite different names*

### Comparing `panpipes-0.4.1/panpipes/funcs/io.py` & `panpipes-0.5.0/panpipes/funcs/io.py`

 * *Files identical despite different names*

### Comparing `panpipes-0.4.1/panpipes/funcs/plotting.py` & `panpipes-0.5.0/panpipes/funcs/plotting.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,25 @@
 import itertools
 import logging
 from matplotlib import use
 import muon as mu
 import matplotlib
 from scipy.sparse import issparse
 from scvi import REGISTRY_KEYS
+import scanpy as sc
+
+from typing import Union, List, Optional, Iterable, Sequence, Dict
+import warnings
+from matplotlib.axes import Axes
+
+from anndata import AnnData
+
+from mudata import MuData
+from muon._core.utils import _get_values
+
 
 use('Agg')
 plt.ioff()
 
 
 def cell2loc_plot_history(model,fig_path, iter_start=0, iter_end=-1, ax=None):
 # Adapted from: https://github.com/BayraktarLab/cell2location/blob/master/cell2location/models/base/_pyro_mixin.py#L407
@@ -306,17 +317,18 @@
 
         ax.yaxis.set_tick_params(tick1On=False)
         ax.set_ylim(-1, len(features_sub) + 3)
 
         ax.yaxis.set_tick_params(labelleft=True)
         ax.set_yticks(np.arange(len(features_sub)))
         ax.set_yticklabels(features_sub)
+        for tick in ax.get_yticklabels():
+            tick.set_fontsize(10)
         for tick in ax.yaxis.get_major_ticks():
-            tick.label.set_fontsize(10)
-            tick.label.set_verticalalignment("bottom")
+            tick.label1.set_verticalalignment("bottom")
 
     fig.tight_layout()
     return fig, ax
 
 
 
 def get_layer(key, mdata, layers):
@@ -338,14 +350,93 @@
             result.append(subst(item, val, rep))
         elif item == val:
             result.append(rep)
         else:
             result.append(item)
     return result
 
+# substitute mu plotting scatters
+
+def alt_scatter(
+    data: Union[AnnData, MuData],
+    x: Optional[str] = None,
+    y: Optional[str] = None,
+    color: Optional[Union[str, Sequence[str]]] = None,
+    use_raw: Optional[bool] = None,
+    layers: Optional[Union[str, Sequence[str]]] = None,
+    **kwargs,
+):
+    """
+    Scatter plot along observations or variables axes.
+    Variables in each modality can be referenced,
+    e.g. ``"rna:X_pca"``.
+
+    See :func:`scanpy.pl.scatter` for details.
+
+    Parameters
+    ----------
+    data : Union[AnnData, MuData]
+        MuData or AnnData object
+    x : Optional[str]
+        x coordinate
+    y : Optional[str]
+        y coordinate
+    color : Optional[Union[str, Sequence[str]]], optional (default: None)
+        Keys for variables or annotations of observations (.obs columns),
+        or a hex colour specification.
+    use_raw : Optional[bool], optional (default: None)
+        Use `.raw` attribute of the modality where a feature (from `color`) is derived from.
+        If `None`, defaults to `True` if `.raw` is present and a valid `layer` is not provided.
+    layers : Optional[Union[str, Sequence[str]]], optional (default: None)
+        Names of the layers where x, y, and color come from.
+        No layer is used by default. A single layer value will be expanded to [layer, layer, layer].
+    """
+    if isinstance(data, AnnData):
+        return sc.pl.embedding(
+            data, x=x, y=y, color=color, use_raw=use_raw, layers=layers, **kwargs
+        )
+
+    if isinstance(layers, str) or layers is None:
+        layers = [layers, layers, layers]
+
+    obs = pd.DataFrame(
+        {
+            x: _get_values(data, x, use_raw=use_raw, layer=layers[0]),
+            y: _get_values(data, y, use_raw=use_raw, layer=layers[1]),
+        }
+    )
+    obs.index = data.obs_names
+    if color is not None:
+        
+        if isinstance(color, str):
+            color_obs = _get_values(data, color, use_raw=use_raw, layer=layers[2])
+            color_obs = pd.DataFrame({color: color_obs})
+            
+        else:
+            print(color)    
+            raise TypeError("Expected color to be a string.")
+        color_obs.index = data.obs_names
+        obs = pd.concat([obs, color_obs], axis=1, ignore_index=False)
+
+    ad = AnnData(obs=obs, uns=data.uns)
+
+    # Note that use_raw and layers are not provided to the plotting function
+    # as the corresponding values were fetched from individual modalities
+    # and are now stored in .obs
+    retval = sc.pl.scatter(ad, x=x, y=y, color=color, **kwargs)
+    if color is not None:
+        for col in color:
+            try:
+                data.uns[f"{col}_colors"] = ad.uns[f"{col}_colors"]
+            except KeyError:
+                pass
+    return retval
+
+
+
 def plot_scatters(mdata, features_list, layers_list):
     layers_listed = [x if type(x) is list else [x] for x in layers_list]
     layers_listed =   subst(layers_listed, "X", None)
 #     print(layers_listed)
     fig_dims = [len(x) for x in layers_listed]
 
     fig, ax = plt.subplots(nrows=fig_dims[0], ncols=fig_dims[1], figsize=(6*fig_dims[1], 6*fig_dims[0]))
@@ -355,25 +446,19 @@
     except AttributeError:
         ax=[ax]
     for ix, x in enumerate(list(itertools.product(*layers_listed))):
         print(ix, x)
         plt_title = "layers:" + " - ".join([x1 if x1 is not None else "X" for x1 in x ])
         if len(x) == 3:
             plt_title = plt_title + "\ncolor:" + features_list[2] 
-        mu.pl.scatter(mdata, 
+        # mu.pl.scatter when #1986 `scanpy.pl.scatter` fails if list is provided for `color` 
+        # https://github.com/scverse/muon/pull/134   
+        alt_scatter(mdata, 
                       features_list[0],
                       features_list[1],
                       color = features_list[2], 
                       layers=x, show=False,
                       save=False, ax= ax[ix] 
                      )
         ax[ix].set_title(plt_title)
     
-        # Shrink current axis by 20%
-#         box = ax[ix].get_position()
-#         ax[ix].set_position([box.x0, box.y0, box.width * 0.8, box.height])
-
-#         # Put a legend to the right of the current axis
-#         ax[ix].legend(loc='center left', bbox_to_anchor=(1, 0.5))
-    return fig, ax
-
-
+    return fig, ax
```

### Comparing `panpipes-0.4.1/panpipes/funcs/processing.py` & `panpipes-0.5.0/panpipes/funcs/processing.py`

 * *Files identical despite different names*

### Comparing `panpipes-0.4.1/panpipes/funcs/scmethods.py` & `panpipes-0.5.0/panpipes/funcs/scmethods.py`

 * *Files identical despite different names*

### Comparing `panpipes-0.4.1/panpipes/panpipes/pipeline_clustering.py` & `panpipes-0.5.0/panpipes/panpipes/pipeline_clustering.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 import pandas as pd
 import cgatcore.iotools as IOTools
 import re
 from itertools import chain, product
 import glob
 
 from panpipes.funcs.processing import extract_parameter_from_fname
+
+import logging
+def get_logger():
+    return logging.getLogger("cgatcore.pipeline")
+
 PARAMS = P.get_parameters(
     ["%s/pipeline.yml" % os.path.splitext(__file__)[0],
      "pipeline.yml"])
 
 PARAMS['py_path'] =  os.path.join(os.path.dirname(os.path.dirname(__file__)), 'python_scripts')
 PARAMS['r_path'] = os.path.join(os.path.dirname(os.path.dirname(__file__)), 'R_scripts')
 PARAMS['mudata_with_knn'] = 'mudata_w_neighbors.h5mu'
@@ -39,34 +44,37 @@
         os.makedirs(os.path.join(mod, "figures"))
     IOTools.touch_file(log_file)
     pass
 ## ------------------------------------
 ## Single modality scripts
 ## ------------------------------------
 
-# -----------------------------------=
+# --------------------------------------
 # neighbors
 # --------------------------------------
+# TO DO create task to re-run neighbours on multimodal outer representations (this script can only read in each mod layer)
 @follows(set_up_dirs)
 @originate(PARAMS['mudata_with_knn'])
 def run_neighbors(outfile):
     mods =  [key for key, value in PARAMS['modalities'].items() if value is True]
     if  any([PARAMS['neighbors'][mod]['use_existing'] is False for mod in mods]):
         # this means we want to rerun neighbors for at least one assay
         #we want to replace thhe scaled obj with the new neighbors
-        log_file="logs/run_single_mod_neighbors.log"
+        log_file="logs/1_run_neighbors.log"
         cmd="""
         python %(py_path)s/rerun_find_neighbors_for_clustering.py \
             --infile %(scaled_obj)s \
             --outfile %(outfile)s  \
             --neighbor_dict '%(neighbors)s' \
             --n_threads %(resources_threads_high)s
             """
         cmd += " > %(log_file)s"
         job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+        log_msg = f"TASK: 'run_neighbors'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{log_file}' FOR MORE INFORMATION."
+        get_logger().info(log_msg)        
         P.run(cmd, **job_kwargs)
     else:
         P.run('ln -s %(scaled_obj)s %(outfile)s', without_cluster=True)
 
 
 
 
@@ -84,15 +92,15 @@
     mods =  [key for key, value in PARAMS['modalities'].items() if value is True]
     if PARAMS["multimodal"]["run_clustering"] is True :
         mods.append("multimodal")
     for mod in mods:
         for md in PARAMS['umap'][mod]['mindist']:
             if PARAMS['umap'][mod]['mindist'] is not None:
                 output_file = os.path.join(mod,  'md' + str(md) +"_umap.txt.gz")
-                log_file = os.path.join("logs","_".join([mod,  'md' + str(md) +"_umap.log"]))
+                log_file = os.path.join("logs","_".join(["2_run_UMAP", mod + '_md' + str(md) + ".log"]))
                 yield [infile, output_file, mod, md, log_file]
 
 @follows(run_neighbors)
 @follows(set_up_dirs)
 @files(gen_umap_jobs)
 def calc_sm_umaps(infile, outfile, mod, mindist, log_file):
     prefix = os.path.split(infile)[0]
@@ -106,14 +114,16 @@
         # if this is not specified it will use rna default
         cmd += " --modality %(mod)s"
     elif mod=="multimodal":
         if PARAMS['multimodal_integration_method'].lower() == "wnn":
             cmd += " --neighbors_key wnn"
     cmd += " > %(log_file)s"
     job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+    log_msg = f"TASK: 'run_umap'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{log_file}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 
 # ------------------------------------
 # Clustering
 # ------------------------------------
 
@@ -128,15 +138,15 @@
     if PARAMS['multimodal']['run_clustering'] is True:
         mods.append("multimodal")
     for mod in mods:
         for res in PARAMS['clusterspecs'][mod]['resolutions']:
             if PARAMS['clusterspecs'][mod]['resolutions'] is not None:
                 alg = PARAMS['clusterspecs'][mod]['algorithm']
                 output_file = os.path.join(mod, 'alg' + alg + '_res' + str(res), "clusters.txt.gz")
-                log_file = os.path.join("logs", "_".join([mod, 'alg' + alg + '_res' + str(res), "clusters.log"]))
+                log_file = os.path.join("logs", "_".join(["3_run_clustering_", mod + '_alg' + alg + '_res' + str(res), ".log"]))
                 yield [infile, output_file, mod, res, alg, log_file]
 
 @follows(set_up_dirs)
 @files(gen_cluster_jobs)
 @follows(run_neighbors)
 def calc_cluster(infile, outfile,  mod, res, alg, log_file):
     cmd = """python %(py_path)s/run_clustering.py 
@@ -149,29 +159,33 @@
         # if this is not specified it will use rna default
         cmd += " --modality %(mod)s"
     elif mod=="multimodal":
         if PARAMS['multimodal_integration_method'].lower() == "wnn":
             cmd += " --neighbors_key wnn"
     cmd += " > %(log_file)s"
     job_kwargs["job_threads"] = PARAMS['resources_threads_medium']
+    log_msg = f"TASK: 'run_clustering'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{log_file}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 
 @collate(calc_cluster,
          regex("(.*)/(.*)/clusters.txt.gz"),
          r"\1/all_res_clusters_list.txt.gz")
 def aggregate_clusters(infiles, outfile):
-    print(infiles)
-    print(outfile)
     infiles_str = ','.join(infiles)
     cmd = "python %(py_path)s/aggregate_csvs.py \
                --input_files_str %(infiles_str)s \
                --output_file %(outfile)s \
-               --clusters_or_markers clusters > logs/aggregate_clusters.log"
-    job_kwargs["job_threads"] = PARAMS['resources_threads_low']           
+               --clusters_or_markers clusters"
+    logfile = "logs/4_aggregate_clusters.log"
+    cmd += f" > {logfile}"
+    job_kwargs["job_threads"] = PARAMS['resources_threads_low'] 
+    log_msg = f"TASK: 'aggregate_clusters'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{logfile}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)          
     P.run(cmd, **job_kwargs)
 
 
 @collate([[calc_cluster], [calc_sm_umaps]], formatter(), PARAMS['sample_prefix'] + "_clustered.h5mu")
 def collate_mdata(infiles,outfile):
     cluster_files = infiles[0]
     cluster_mods = [os.path.dirname(os.path.dirname(x)) for x in cluster_files]
@@ -193,49 +207,57 @@
         --output_mudata %(outfile)s 
     """
     if PARAMS['full_obj'] is None:
         mdata_in = PARAMS['mudata_with_knn']
         cmd += "--input_mudata %(mdata_in)s"
     else:
         cmd += "--input_mudata  %(full_obj)s"
-    cmd += " > logs/collate_data.log"
+    logfile = "logs/5_collate_data.log"
+    cmd += f" > {logfile}"
     job_kwargs["job_threads"] = PARAMS['resources_threads_medium']
+    log_msg = f"TASK: 'collate_mdata'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{logfile}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)  
     P.run(cmd, **job_kwargs)
 
 
 @transform(collate_mdata, 
             formatter(""),
-            'logs/plot_clusters_umaps.log')
+            'logs/6_plot_clusters_umaps.log')
 def plot_cluster_umaps(infile, log_file,):
     # get associated umap
     mods =  [key for key, value in PARAMS['modalities'].items() if value is True]
     if PARAMS['multimodal']['run_clustering']:
         mods.append("multimodal")
     mods = ','.join(mods)
     cmd = """python %(py_path)s/plot_cluster_umaps.py \
     --infile %(infile)s 
     --modalities '%(mods)s'
     """
     cmd += " >> %(log_file)s"
     job_kwargs["job_threads"] = PARAMS['resources_threads_medium']
+    log_msg = f"TASK: 'plot_cluster_umaps'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{log_file}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)  
     P.run(cmd, jobs_limit=1, **job_kwargs)
 
+
 @transform(aggregate_clusters, regex("(.*)/all_res_clusters_list.txt.gz"),
-            r'logs/\1_clustree.log',
+            r'logs/7_\1_run_clustree.log',
             r'\1/figures/clustree.png', ) 
 def plot_clustree(infile, log_file, outfile):
     # convert infiles to comma sep. string
     prefix = re.sub('_dir', '', os.path.dirname(infile))
     # call R
     cmd = "Rscript %(r_path)s/plotclustree.R \
         --infile %(infile)s  \
         --plot_title %(prefix)s \
         --outfile %(outfile)s > %(log_file)s"
     
     job_kwargs["job_threads"] = PARAMS['resources_threads_low']
+    log_msg = f"TASK: 'clustree'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{log_file}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)  
     P.run(cmd,  **job_kwargs)
 
 
 
 # # all the defs
 # # def clustering_umbrella
 @follows(calc_cluster, collate_mdata, plot_cluster_umaps, plot_clustree)
@@ -256,15 +278,15 @@
     mods =  [key for key, value in PARAMS['modalities'].items() if value is True]
     for md in mods:
         IOTools.touch_file(os.path.join(base_dir, md + "_markers.txt"))
 
 @follows(collate_mdata)
 @transform(gen_marker_jobs,
            regex("(.*)/(.*)/(.*)_markers.txt"),
-           r"logs/\1_\2_\3_markers.log",
+           r"logs/8_find_markers_\1_\2_\3.log",
            r"\1/\2/\3_markers",
            r"\1",
            r"\1/\2",
            r"\3"
            )
 def find_markers(infile, log_file, outfile_prefix, base_mod, cluster_dir, data_mod):
     """
@@ -290,14 +312,16 @@
         threshuse =  PARAMS["markerspecs"][data_mod]["threshuse"]
         cmd += """ --pseudo_seurat True 
         --minpct %(min_pct)s 
         --threshuse %(threshuse)s 
         """
     cmd += " > %(log_file)s "
     job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+    log_msg = f"TASK: 'find_markers'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{log_file}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)  
     P.run(cmd, **job_kwargs)
 
 
 
 
 # # limit jobs because reading the h5 file simultaneouly is problematic
 # @collate([ [collate_mdata],[find_markers]],
@@ -320,15 +344,15 @@
 
 # this transforms gen_marker_jobs instead of find_markers because gen_marker_jobs creates empty marker files
 # which are then filled by find_markers.
 @follows(collate_mdata)
 @follows(find_markers)
 @transform(gen_marker_jobs,
             regex(r"(.*)/alg(.*)/(.*)_markers.txt"),
-            r"logs/cluster\1_alg\2_exprs_\3_dotplots.log",
+            r"logs/9_plot_markers_\1_alg\2_exprs_\3.log",
             r"\1/alg\2/figures/dotplot_top_markers_\3.png",
             r"\1/alg\2/figures",
              r"\1", r"\2", r"\3")
 def plot_marker_dotplots(marker_file, log_file, outfile, 
                          fig_path, cluster_mod, cluster_col, expr_mod):
     """
     Plots some additional marker plots
@@ -352,14 +376,16 @@
     if cluster_mod != "multimodal":
         cluster_col = cluster_mod + ":" + cluster_col
     cmd += " --group_col %(cluster_col)s"
     layer_choice = PARAMS["markerspecs"][expr_mod]["layer"]
     cmd += " --layer %(layer_choice)s"
     cmd += " > %(log_file)s "
     job_kwargs["job_threads"] = PARAMS['resources_threads_medium']
+    log_msg = f"TASK: 'plot_markers'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{log_file}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)  
     P.run(cmd, **job_kwargs)
 
 
 
 
 
 @follows(find_markers, plot_marker_dotplots)
```

### Comparing `panpipes-0.4.1/panpipes/panpipes/pipeline_deconvolution_spatial/pipeline.yml` & `panpipes-0.5.0/panpipes/panpipes/pipeline_deconvolution_spatial/pipeline.yml`

 * *Files 23% similar despite different names*

```diff
@@ -1,98 +1,129 @@
-# ============================================================
-# Spatial Deconvolution workflow Panpipes (pipeline_deconvolution_spatial.py)
-# ============================================================
-# written by Sarah Ouologuem
+# =============================================================================================
+# Deconvolution, spatial transcriptomics workflow Panpipes (pipeline_deconvolution_spatial.py)
+# =============================================================================================
+# Written by Sarah Ouologuem
 
 
-# ----------------------
+# ---------------------------
 # 0. Compute resource options
-# ------------------------
+# ---------------------------
 resources:
   # Number of threads used for parallel jobs
-  threads_high: 1 # Must be enough memory to load all input files and create MuDatas
+  threads_high: 1 # Number of threads used for high intensity computing tasks
   threads_medium: 1  # Must be enough memory to load your mudata and do computationally light tasks
   threads_low: 1 # Must be enough memory to load text files and do plotting, requires much less memory
 
 condaenv:  # Path to conda env, leave blank if running native or your cluster automatically inherits the login node environment
 
 
 
 # ----------------------
 # 1. Specify input 
 # ----------------------
 
 # One or multiple slides can be deconvoluted with the same reference in one run. For that, one MuData object for each slide is expected. 
-
-input_spatial: data/spatial_data # Path to folder containing one or multiple MuDatas of spatial data. For all MuData files in that folder, deconvolution is run by the pipeline.
-# In the MuData objects, the spatial data is expected to be saved in mudata.mod["spatial"]. For each spatial MuData, deconvolution is run with "input_singlecell" (see below) as a reference
-
-input_singlecell: data/single_cell_reference.h5mu # Path to the MuData file of the reference single-cell data, reference data expected to be saved in mudata.mod["rna"]
+input: 
+  spatial:  # Path to folder containing one or multiple MuDatas of spatial data. The pipeline is reading in all MuData files in that folder and assuming that they are MuDatas of spatial slides. 
+# For all MuData files in that folder, deconvolution is run by the pipeline.
+# In the MuData objects, the spatial data is expected to be saved in mudata.mod["spatial"]. For each spatial MuData, deconvolution is run with "singlecell" (see below) as a reference
+  singlecell:  # Path to the MuData file of the reference single-cell data, reference data expected to be saved in mudata.mod["rna"]
 
 
 
 # ----------------------
 ## 2. Cell2Location
 # ----------------------
+
 Cell2Location: 
   run: True # Whether to run Cell2Location 
   
   # -------------------------------
   # Feature selection paramaters
   # -------------------------------
-  
+  feature_selection:
   # Reduced feature set can either be given  a) via a csv file of genes or b) feature selection will be performed à la Cell2Location, i.e. via the function: cell2location.utils.filtering.filter_genes()
   # If no file is given in a), b) will be run, i.e. feature selection is not optional. 
   
-  #  a) Path to a csv file containing a reduced feature set
-  gene_list: # A header in the csv is expected in the first row
+    # a) Path to a csv file containing a reduced feature set
+    gene_list: # A header in the csv is expected in the first row
   
-  # b) Parameters for Cell2Location's feature selection, leave empty to use defaults
-  # Whether to remove mitochondrial genes before feature selection 
-  remove_mt: False # Default True
-  # All genes detected in less than cell_count_cutoff cells will be excluded.
-  cell_count_cutoff: # Default 15, parameter of function cell2location.utils.filtering.filter_genes()
-  # All genes detected in at least this percentage of cells will be included.
-  cell_percentage_cutoff2: # Default 0.05, parameter of function cell2location.utils.filtering.filter_genes()
-  # Genes detected in the number of cells between the above-mentioned cutoffs are selected only when their average expression in non-zero cells is above this cutoff
-  nonz_mean_cutoff:  # Default 1.12, parameter of function cell2location.utils.filtering.filter_genes()
-
+    # b) Parameters for Cell2Location's feature selection, leave empty to use defaults
+    # Whether to remove mitochondrial genes before feature selection 
+    remove_mt: False # Default True
+    # All genes detected in less than cell_count_cutoff cells will be excluded.
+    cell_count_cutoff: # Default 15, parameter of function cell2location.utils.filtering.filter_genes()
+    # All genes detected in at least this percentage of cells will be included.
+    cell_percentage_cutoff2: # Default 0.05, parameter of function cell2location.utils.filtering.filter_genes()
+    # Genes detected in the number of cells between the above-mentioned cutoffs are selected only when their average expression in non-zero cells is above this cutoff
+    nonz_mean_cutoff:  # Default 1.12, parameter of function cell2location.utils.filtering.filter_genes()
 
   # -------------------------------
   # Reference model paramaters
   # Leave empty to use defaults
   # -------------------------------
-  labels_key_reference: cell_type # Default None, key in adata.obs for label (cell type) information
-  batch_key_reference: # Default None, key in adata.obs for batch information
-  layer_reference: raw_counts # Default None (if None, X will be used), Layer of the raw (!) counts
-  categorical_covariate_keys_reference: key1,key2,key3 # Comma-separated without spaces; default None; keys in adata.obs that correspond to categorical data. These covariates can be added in addition to the batch covariate and are also treated as nuisance factors (i.e., the model tries to minimize their effects on the latent space)
-  continuous_covariate_keys_reference: key1,key2,key3 # Comma-separated without spaces; default None; keys in adata.obs that correspond to continuous data. These covariates can be added in addition to the batch covariate and are also treated as nuisance factors (i.e., the model tries to minimize their effects on the latent space)
-  
-  max_epochs_reference: 500 # Default np.min([round((20000 / n_cells) * 400), 400])
-
+  reference: 
+    labels_key: cell_type # Default None, key in adata.obs for label (cell type) information
+    batch_key: # Default None, key in adata.obs for batch information
+    layer: raw_counts # Default None (if None, X will be used), Layer of the raw (!) counts
+    categorical_covariate_keys: key1,key2,key3 # Comma-separated without spaces; default None; keys in adata.obs that correspond to categorical data. These covariates can be added in addition to the batch covariate and are also treated as nuisance factors (i.e., the model tries to minimize their effects on the latent space)
+    continuous_covariate_keys: key1,key2,key3 # Comma-separated without spaces; default None; keys in adata.obs that correspond to continuous data. These covariates can be added in addition to the batch covariate and are also treated as nuisance factors (i.e., the model tries to minimize their effects on the latent space)
+    max_epochs: 500 # Default np.min([round((20000 / n_cells) * 400), 400])
+    use_gpu: # Default True; whether to use GPU for training 
 
   # -------------------------------
   # Spatial mapping model paramaters
   # Leave empty to use defaults
   # -------------------------------
-  batch_key_st: # Default None, key in adata.obs for batch information
-  layer_st: raw_counts # Default None (if None, X will be used), Layer of the raw (!) counts
-  categorical_covariate_keys_st: key1,key2,key3 # Comma-separated without spaces; default None; keys in adata.obs that correspond to categorical data. These covariates can be added in addition to the batch covariate and are also treated as nuisance factors (i.e., the model tries to minimize their effects on the latent space)
-  continuous_covariate_keys_st: key1,key2,key3 # Comma-separated without spaces; default None; keys in adata.obs that correspond to continuous data. These covariates can be added in addition to the batch covariate and are also treated as nuisance factors (i.e., the model tries to minimize their effects on the latent space)
-  
-  # The following two parameters must be specified (cannot leave empty), otherwise an error will be thrown:
-  N_cells_per_location: 30 # Expected cell abundance per voxel
-  detection_alpha: 20 # Regularization of with-in experiment variation in RNA detection sensitivity
+  spatial: 
+    batch_key: # Default None, key in adata.obs for batch information
+    layer: raw_counts # Default None (if None, X will be used), Layer of the raw (!) counts
+    categorical_covariate_keys: key1,key2,key3 # Comma-separated without spaces; default None; keys in adata.obs that correspond to categorical data. These covariates can be added in addition to the batch covariate and are also treated as nuisance factors (i.e., the model tries to minimize their effects on the latent space)
+    continuous_covariate_keys: key1,key2,key3 # Comma-separated without spaces; default None; keys in adata.obs that correspond to continuous data. These covariates can be added in addition to the batch covariate and are also treated as nuisance factors (i.e., the model tries to minimize their effects on the latent space)
+  
+    # The following two parameters must be specified (cannot leave empty), otherwise an error will be thrown:
+    N_cells_per_location: 30 # Expected cell abundance per voxel
+    detection_alpha: 20 # Regularization of with-in experiment variation in RNA detection sensitivity
   
-  max_epochs_st: 500 # Default np.min([round((20000 / n_cells) * 400), 400])
-
+    max_epochs: 500 # Default np.min([round((20000 / n_cells) * 400), 400])
+    use_gpu: # Default True; whether to use GPU for training
 
  # -------------------------------
-  save_models: False # Whether to save the reference and spatial mapping models
+  save_models: False # Default False; whether to save the reference and spatial mapping models
+
 
 
+# -------------
+## 3. Tangram
+# -------------
 
+Tangram: 
+  run: True # Whether to run Tangram 
 
+  # -------------------------------
+  # Feature selection paramaters
+  # -------------------------------
+  # Reduced feature set can either be given  a) via a csv file of genes or b) sc.tl.rank_genes_groups() is run and the top n markers of each group are selected 
+  # If no file is given in a), b) will be run, i.e. feature selection is not optional.  
+  feature_selection: 
+    #  a) Path to a csv file containing a reduced feature set
+    gene_list: # A header in the csv is expected in the first row
+
+    # b) Parameters for sc.tl.rank_genes_groups() gene selection.
+    rank_genes: 
+      labels_key: cell_type # Which column in .obs of the reference to use for the 'groupby' parameter of sc.tl.rank_genes_groups()
+      layer: Null # Default None, which layer to use of the reference for sc.tl.rank_genes_groups(). if Null (i.e. None), uses .X
+      n_genes: 100 # Default 100, how many top genes to select of each 'groupby' group
+      test_method: wilcoxon # Default t-test_overestim_var, which test method to use. one of ['logreg', 't-test', 'wilcoxon', 't-test_overestim_var']
+      correction_method: benjamini-hochberg # Default benjamini-hochberg, which p-value correction method to use. one of ['benjamini-hochberg', 'bonferroni']. Used only for 't-test', 't-test_overestim_var', and 'wilcoxon'
+
+  model: 
+    labels_key: # Default None, cell type key in the reference .obs
+    num_epochs: # Default 1000. Number of epochs for tangram.mapping_utils.map_cells_to_space()
+    device: cpu # Default cpu. Device to use for deconvolution
+    kwargs: # Parameters for tangram.mapping_utils.map_cells_to_space(), feel free to add or remove parameters below 
+      learning_rate: 0.1
+      lambda_d: 0
```

### Comparing `panpipes-0.4.1/panpipes/panpipes/pipeline_ingest.py` & `panpipes-0.5.0/panpipes/panpipes/pipeline_ingest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,14 +16,25 @@
 import warnings
 
 # warnings.simplefilter('ignore', category=NumbaDeprecationWarning)
 # warnings.simplefilter('ignore', category=NumbaPendingDeprecationWarning)
 
 import yaml
 
+import logging
+# L = logging.getLogger('panpipes')
+# L.setLevel(logging.INFO)
+# log_handler = logging.StreamHandler(sys.stdout)
+# log_formatter = logging.Formatter('%(asctime)s: %(levelname)s - %(message)s')
+# log_handler.setFormatter(log_formatter)
+# L.addHandler(log_handler)
+
+def get_logger():
+    return logging.getLogger("cgatcore.pipeline")
+
 
 PARAMS = P.get_parameters(
     ["%s/pipeline.yml" % os.path.splitext(__file__)[0],
      "pipeline.yml"])
 
 PARAMS['py_path'] =  os.path.join(os.path.dirname(os.path.dirname(__file__)), 'python_scripts')
 PARAMS['r_path'] = os.path.join(os.path.dirname(os.path.dirname(__file__)), 'R_scripts')
@@ -46,27 +57,29 @@
 
 # TODO: update this to check for each modality csv file
 # TODO: check this works with current submission file
 @active_if(PARAMS['plot_10X_metrics'])
 @follows(mkdir('figures'))
 @follows(mkdir('figures/tenx_metrics'))
 @follows(mkdir("logs"))
-@originate("logs/tenx_metrics_multi_aggregate.log")
+@originate("logs/0_tenx_metrics_multi_aggregate.log")
 def aggregate_tenx_metrics_multi(outfile):
     """this is to aggregate all the cellranger multi metric_summary files
     it also does some plotting
     """    
     cmd = """
         python %(py_path)s/aggregate_cellranger_summary_metrics.py
             --pipe_df %(submission_file)s
             --figdir figures/tenx_metrics/
             --cellranger_column_conversion_df %(resources_path)s/metrics_summary_col_conversion.tsv
             --output_file 10x_metrics.csv > %(outfile)s
             """
     job_kwargs["job_threads"] = PARAMS['resources_threads_low']
+    log_msg = f"TASK: 'aggregate_tenx_metrics_multi'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{outfile}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)   
     P.run(cmd, **job_kwargs)
 
 
 @follows(aggregate_tenx_metrics_multi)
 def process_all_tenx_metrics():
     pass
 # -----------------------------------------------------------------------------------------------
@@ -137,17 +150,20 @@
       # ~ means this tests "is not nan"
     if tcr_path is not None and pd.notna(tcr_path):
         cmd += " --tcr_filtered_contigs %(tcr_path)s"
         cmd += " --tcr_filetype %(tcr_filetype)s"
     if bcr_path is not None and pd.notna(bcr_path):
         cmd += " --bcr_filtered_contigs %(bcr_path)s"
         cmd += " --bcr_filetype %(bcr_filetype)s"
-    cmd += " > logs/load_mudatas_%(sample_id)s.log"
+    logfile = f"logs/1_load_mudatas_{sample_id}.log"
+    cmd += f" > {logfile}"
     # print(cmd)
     job_kwargs["job_threads"] = PARAMS['resources_threads_medium']
+    log_msg = f"TASK: 'load_mudatas'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{logfile}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 
 
 @active_if(PARAMS["use_existing_h5mu"] is False)
 @collate(load_mudatas,
          formatter(""),
@@ -169,16 +185,19 @@
     if PARAMS["barcode_mtd_include"] is True:
         cmd += " --barcode_mtd_df %(barcode_mtd_path)s"
         cmd += " --barcode_mtd_metadatacols %(barcode_mtd_metadatacols)s"
     if PARAMS['protein_metadata_table'] is not None:
         cmd += " --protein_var_table %(protein_metadata_table)s"
     if PARAMS['index_col_choice'] is not None:
         cmd += " --protein_new_index_col %(index_col_choice)s"
-    cmd += " > logs/concat_filtered_mudatas.log"
+    logfile = "logs/1_concat_filtered_mudatas.log"
+    cmd += f" > {logfile}"
     job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+    log_msg = f"TASK: 'concat_filtered_mudatas'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{logfile}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
     # P.run("rm tmp/*", job_threads=PARAMS['resources_threads_low'])
 
 
 # -----------------------------------------------------------------------------------------------
 ## Creating h5mu from bg data files
 # -----------------------------------------------------------------------------------------------
@@ -250,33 +269,37 @@
         cmd += " --fragments_file %(fragments_file)s"
     if peak_annotation_file is not None and pd.notna(peak_annotation_file):
         cmd += " --peak_annotation_file %(peak_annotation_file)s"
     if PARAMS['protein_metadata_table'] is not None:
         cmd += " --protein_var_table %(protein_metadata_table)s"  #check which of these 2 needs to stay!!!
     if PARAMS['index_col_choice'] is not None:
         cmd += " --protein_new_index_col %(index_col_choice)s"
-    cmd += " > logs/load_bg_mudatas_%(sample_id)s.log"
+    logfile = f"logs/1_load_bg_mudatas_%(sample_id)s.log"
+    cmd += " > {logfile}"
     job_kwargs["job_threads"] = PARAMS['resources_threads_medium']
+    log_msg = f"TASK: 'load_bg_mudatas'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{logfile}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 
 @active_if(PARAMS["bg_required"])
 @active_if(PARAMS['downsample_background'])
 @follows(load_bg_mudatas)
 @transform(load_bg_mudatas, 
            regex("./tmp/(.*)_raw.h5(.*)"), 
-           r"./logs/\1_bg_downsampled.log")
+           r"./logs/1_\1_bg_downsampled.log")
 def downsample_bg_mudatas(infile, outfile):
     cmd = """
     python %(py_path)s/downsample.py 
     --input_mudata %(infile)s
     --output_mudata "%(infile)s" 
     --downsample_value 20000  > %(outfile)s
     """
     job_kwargs["job_threads"] = PARAMS['resources_threads_medium']
+    # TODO: add log file?
     P.run(cmd, **job_kwargs)
 
 
 @active_if(PARAMS["bg_required"])
 @active_if(PARAMS["assess_background"])
 @active_if(PARAMS["use_existing_h5mu"] is False)
 @follows(load_bg_mudatas)
@@ -297,16 +320,19 @@
         --join_type %(concat_join_type)s
         """
     if PARAMS['metadatacols'] is not None and PARAMS['metadatacols'] != "":
         cmd += " --metadatacols  %(metadatacols)s"
   #  if PARAMS["barcode_mtd_include"] is True:
    #     cmd += " --barcode_mtd_df %(barcode_mtd_path)s"
     #    cmd += " --barcode_mtd_metadatacols %(barcode_mtd_metadatacols)s"
-    cmd += " > logs/concat_bg_mudatas.log"
+    logfile = "logs/1_concat_bg_mudatas.log"
+    cmd += " > {logfile}"
     job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+    log_msg = f"TASK: 'concat_bg_mudatas'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{logfile}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
     # P.run("rm tmp/*", job_threads=PARAMS['resources_threads_low'])
 
 # -----------------------------------------------------------------------------------------------
 ## rna QC 
 # -----------------------------------------------------------------------------------------------
 
@@ -340,25 +366,28 @@
         cmd += " --min_gene_variability_pctl %(scr_min_gene_variability_pctl)s"
     if PARAMS['scr_n_prin_comps'] is not None:
         cmd += " --n_prin_comps %(scr_n_prin_comps)s"
     if PARAMS['scr_use_thr'] is not None:
         cmd += " --use_thr %(scr_use_thr)s"
     if PARAMS['scr_call_doublets_thr'] is not None:
         cmd += " --call_doublets_thr %(scr_call_doublets_thr)s"
-    cmd += " > logs/run_scrublet_" + sample_id + ".log"
+    logfile = "logs/2_run_scrublet_" + sample_id + ".log"
+    cmd += f" > {logfile}"
     job_kwargs["job_threads"] = PARAMS['resources_threads_medium']
+    log_msg = f"TASK: 'run_scrublet'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{logfile}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd,**job_kwargs)
     IOTools.touch_file(outfile)
 
 
 @active_if(PARAMS['modalities_rna'])
 @follows(mkdir("figures"))
 @follows(mkdir("figures/rna"))
 @follows(concat_filtered_mudatas, run_scrublet)
-@originate("logs/run_scanpy_qc_rna.log", orfile(), unfilt_file())
+@originate("logs/3_run_scanpy_qc_rna.log", orfile(), unfilt_file())
 def run_rna_qc(log_file, outfile, unfilt_file):
     # infile = submission file
     resources_path = os.path.join(os.path.dirname(os.path.dirname(__file__)), "resources")
     customgenesfile = PARAMS["custom_genes_file"]
     calcproportions= PARAMS["calc_proportions"]
     cmd = """
         python %(py_path)s/run_scanpyQC_rna.py
@@ -387,14 +416,16 @@
     # if PARAMS['isotype_upper_quantile'] is not None:
     #     cmd += " --isotype_upper_quantile %(isotype_upper_quantile)s"
     # if PARAMS['isotype_n_pass'] is not None:
     #     cmd += " --isotype_n_pass %(isotype_n_pass)s"
     # add log file
     cmd += " > %(log_file)s"
     job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+    log_msg = f"TASK: 'run_rna_qc'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{log_file}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
     if os.path.exists("cache"):
         P.run("rm -r cache")
     #IOTools.touch_file(metadata)
 
 #TO DO ADD the other modalities in this order:
 
@@ -408,15 +439,15 @@
 # this is because we don't want to try and load the file during the `config` stage
 
 # def prot_cell_mtd():
 #     return PARAMS['sample_prefix'] + "_prot_cell_metadata.tsv"
 @active_if(PARAMS['modalities_prot'])
 @follows(mkdir('figures/prot'))
 @follows(concat_filtered_mudatas, run_rna_qc)
-@originate("logs/run_scanpy_qc_prot.log", orfile(), unfilt_file())
+@originate("logs/3_run_scanpy_qc_prot.log", orfile(), unfilt_file())
 def run_scanpy_prot_qc(log_file, outfile, unfilt_file):
     # infile = submission file
     cmd = """
         python %(py_path)s/run_scanpyQC_prot.py
           --sampleprefix %(sample_prefix)s
           --input_anndata %(unfilt_file)s
           --outfile %(unfilt_file)s
@@ -433,20 +464,22 @@
     if PARAMS['identify_isotype_outliers']:
         cmd += " --identify_isotype_outliers %(identify_isotype_outliers)s"
         cmd += " --isotype_upper_quantile %(isotype_upper_quantile)s"
         cmd += " --isotype_n_pass %(isotype_n_pass)s"
     # add log file
     cmd += " > %(log_file)s"
     job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+    log_msg = f"TASK: 'run_scanpy_prot_qc'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{log_file}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
     pass
 
 @active_if(PARAMS['modalities_prot'])
 @follows(run_scanpy_prot_qc, concat_filtered_mudatas, concat_bg_mudatas)
-@originate("logs/run_dsb_clr.log", unfilt_file(), bg_file())
+@originate("logs/3_run_dsb_clr.log", unfilt_file(), bg_file())
 def run_dsb_clr(outfile, unfilt_file, bg_file):
     print(unfilt_file)
     # infile = mdata_unfilt
     # outfile sampleprefix + "prot_qc_per_cell.tsv"
     cmd = """
         python %(py_path)s/run_preprocess_prot.py
         --filtered_mudata %(unfilt_file)s
@@ -463,49 +496,53 @@
     if PARAMS['save_norm_prot_mtx'] is True:
         cmd += " --save_mtx True"
     # find the bg data if available
     if os.path.exists(bg_file):
         cmd += " --bg_mudata %(bg_file)s"
     cmd += " > %(outfile)s"
     job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+    log_msg = f"TASK: 'run_dsb_clr'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{outfile}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 @follows(run_scanpy_prot_qc, run_dsb_clr)
 def run_prot_qc():
     pass
 
 
 # -----------------------------------------------------------------------------------------------
 ## Repertoire QC  # Repertoire run_scanpy_qc_rep.log
 # -----------------------------------------------------------------------------------------------
 # toggle_rep_qc = ()
 @active_if(PARAMS['modalities_bcr'] or PARAMS['modalities_tcr']  )
 @follows(mkdir('figures/rep'))
 @follows(run_rna_qc, run_prot_qc)
-@originate("logs/run_scanpy_qc_rep.log", unfilt_file())
+@originate("logs/3_run_scanpy_qc_rep.log", unfilt_file())
 def run_repertoire_qc(logfile, unfilt_file):
     cmd = """python %(py_path)s/run_scanpyQC_rep.py
           --sampleprefix %(sample_prefix)s
           --input_mudata %(unfilt_file)s
           --output_mudata %(unfilt_file)s
           --figdir figures/rep/
           --distance_metrics "%(ir_dist)s"
           --clonotype_metrics "%(clonotype_definition)s"
           """
     cmd += " > %(logfile)s"
     job_kwargs["job_threads"] = PARAMS['resources_threads_low']
+    log_msg = f"TASK: 'run_repertoire_qc'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{logfile}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 # -----------------------------------------------------------------------------------------------
 ## atac QC # run_scanpy_qc_atac.log
 # -----------------------------------------------------------------------------------------------
 @active_if(PARAMS['modalities_atac'])
 @mkdir('figures/atac')
 @follows(run_rna_qc, run_prot_qc, run_repertoire_qc)
-@originate("logs/run_scanpy_qc_atac.log", orfile(), unfilt_file())
+@originate("logs/3_run_scanpy_qc_atac.log", orfile(), unfilt_file())
 def run_atac_qc(log_file, outfile, unfilt_file):
     # if this is a multiple samples project
     # they should be run together upfront 
     # for independent atac run cellranger-atac count, then cellranger-atac aggr
     # https://support.10xgenomics.com/single-cell-atac/software/pipelines/latest/using/aggr
     # for multiome run cellranger-arc count then cellranger-arc aggr
     # https://support.10xgenomics.com/single-cell-multiome-atac-gex/software/pipelines/latest/using/aggr
@@ -534,27 +571,29 @@
         prna_file = PARAMS["partner_rna"]
         cmd += " --paired_rna %(prna_file)s"
     
     cmd += " --use_muon True"
 
     cmd += " > %(log_file)s"
     job_kwargs["job_threads"] = PARAMS['resources_threads_low']
+    log_msg = f"TASK: 'run_atac_qc'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{log_file}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 @follows(run_rna_qc, run_prot_qc, run_repertoire_qc, run_atac_qc)
 def run_qc():
     pass
 
 
 # -----------------------------------------------------------------------------------------------
 ## QC plotting
 # -----------------------------------------------------------------------------------------------
 
 @follows(run_qc)
-@originate("logs/plot_qc.log", orfile())
+@originate("logs/4_plot_qc.log", orfile())
 def plot_qc(log_file, cell_file):
     qcmetrics = PARAMS['plotqc_rna_metrics']
     cmd = """
     Rscript %(r_path)s/plotQC.R 
     --prefilter TRUE
     --cell_metadata %(cell_file)s 
     --sampleprefix %(sample_prefix)s
@@ -569,36 +608,40 @@
         cmd += " --atac_qc_metrics %(plotqc_atac_metrics)s"
     if PARAMS['modalities_bcr'] or PARAMS['modalities_tcr']:
         if PARAMS['plotqc_rep_metrics'] is not None:
             pqrm = ','.join(['plotqc_rep_metrics'])
             cmd += " --rep_qc_metrics %(pqrm)s"
     cmd += " > %(log_file)s"
     job_kwargs["job_threads"] = PARAMS['resources_threads_low']
+    log_msg = f"TASK: 'plot_qc'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{log_file}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 
 # ------
 # assess background
 # -------
 
 @active_if(PARAMS['assess_background'])
 @follows(mkdir("figures/background"))
 @follows(run_qc)
 @follows(concat_bg_mudatas)
-@originate("logs/assess_background.log", unfilt_file(), bg_file())
+@originate("logs/5_assess_background.log", unfilt_file(), bg_file())
 def run_assess_background(log_file, unfilt_file, bg_file):
     cmd = """
     python %(py_path)s/assess_background.py
         --filtered_mudata %(unfilt_file)s
         --bg_mudata %(bg_file)s
         --channel_col %(channel_col)s
         --figpath "./figures/background/"
     """
     cmd += " > %(log_file)s"
     job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+    log_msg = f"TASK: 'run_assess_background'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{log_file}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 
 
 # # ------------
 # TO DO change the decorator to follow all qc plots?
 @follows(plot_qc)
```

### Comparing `panpipes-0.4.1/panpipes/panpipes/pipeline_integration.py` & `panpipes-0.5.0/panpipes/panpipes/pipeline_integration.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 import os
 from cgatcore import pipeline as P
 import pandas as pd
 import cgatcore.iotools as IOTools
 import re
 from itertools import chain
 import glob
+import logging
+
+def get_logger():
+    return logging.getLogger("cgatcore.pipeline")
 
 
 PARAMS = P.get_parameters(
     ["%s/pipeline.yml" % os.path.splitext(__file__)[0],
      "pipeline.yml"])
 
 
@@ -77,19 +81,21 @@
         cmd += " --neighbors_method %s" % neighbor_params['method']
     if neighbor_params['metric'] is not None:
         cmd += " --neighbors_metric %s" % neighbor_params['metric']
     if neighbor_params['npcs'] is not None:
         cmd += " --neighbors_n_pcs %s"  % neighbor_params['npcs']
     if neighbor_params['k'] is not None:
         cmd += " --neighbors_k %s" % neighbor_params['k']
-    cmd += " > logs/rna_no_correct.log"
+    cmd += " > logs/1_rna_no_correct.log"
     
     if PARAMS['queues_long'] is not None:
         job_kwargs["job_queue"] = job_queue=PARAMS['queues_long']
-    job_kwargs["job_threads"] = PARAMS['resources_threads_high']    
+    job_kwargs["job_threads"] = PARAMS['resources_threads_high']  
+    log_msg = f"TASK: 'run_no_batch_correct_rna'" + f" IN CASE OF ERROR, PLEASE REFER TO : 'logs/1_rna_no_correct.log' FOR MORE INFORMATION."
+    get_logger().info(log_msg)  
     P.run(cmd, **job_kwargs) 
 
 
 
 # rna BBKNN
 @follows(set_up_dirs)
 @active_if(PARAMS['rna_run'])
@@ -103,19 +109,21 @@
      --integration_col %(rna_column)s
      --modality rna
      """
     if PARAMS['rna']['bbknn']['neighbors_within_batch'] is not None:
         cmd += " --neighbors_within_batch %i" % PARAMS['rna']['bbknn']['neighbors_within_batch']
     if PARAMS['rna']['neighbors']['npcs'] is not None:
         cmd += " --neighbors_n_pcs %s" % PARAMS['rna']['neighbors']['npcs']
-    cmd += " > logs/rna_bbknn.log "
+    cmd += " > logs/1_rna_bbknn.log "
     
     if PARAMS['queues_long'] is not None:
         job_kwargs["job_queue"] = job_queue=PARAMS['queues_long']
     job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+    log_msg = f"TASK: 'run_bbknn_rna'" + f" IN CASE OF ERROR, PLEASE REFER TO : 'logs/1_rna_bbknn.log' FOR MORE INFORMATION."
+    get_logger().info(log_msg)  
     P.run(cmd, **job_kwargs) 
 
 
 # rna COMBAT
 @follows(set_up_dirs)
 @active_if(PARAMS['rna_run'])
 @active_if(PARAMS['rna_tools'] is not None and 'combat' in PARAMS['rna_tools'])
@@ -134,20 +142,22 @@
         cmd += " --neighbors_method %s" % neighbor_params['method']
     if neighbor_params['metric'] is not None:
         cmd += " --neighbors_metric %s" % neighbor_params['metric']
     if neighbor_params['npcs'] is not None:
         cmd += " --neighbors_n_pcs %s"  % neighbor_params['npcs']
     if neighbor_params['k'] is not None:
         cmd += " --neighbors_k %s" % neighbor_params['k']
-    cmd += " > logs/rna_combat.log "
+    cmd += " > logs/1_rna_combat.log "
     
     if PARAMS['queues_long'] is not None:
         job_kwargs["job_queue"] = job_queue=PARAMS['queues_long']
 
     job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+    log_msg = f"TASK: 'run_combat_rna'" + f" IN CASE OF ERROR, PLEASE REFER TO : 'logs/1_rna_combat.log' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs) 
 
 # rna HARMONY
 @follows(set_up_dirs)
 @active_if(PARAMS['rna_run'])
 @active_if(PARAMS['rna_tools'] is not None and 'harmony' in PARAMS['rna_tools'])
 @originate("batch_correction/umap_rna_harmony.csv")
@@ -172,20 +182,22 @@
         cmd += " --neighbors_method %s" % neighbor_params['method']
     if neighbor_params['metric'] is not None:
         cmd += " --neighbors_metric %s" % neighbor_params['metric']
     if neighbor_params['npcs'] is not None:
         cmd += " --neighbors_n_pcs %s"  % neighbor_params['npcs']
     if neighbor_params['k'] is not None:
         cmd += " --neighbors_k %s" % neighbor_params['k']
-    cmd += " > logs/rna_harmony.log " 
+    cmd += " > logs/1_rna_harmony.log " 
      #job arguments
     
     if PARAMS['queues_long'] is not None:
         job_kwargs["job_queue"] = job_queue=PARAMS['queues_long']
     job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+    log_msg = f"TASK: 'run_harmony_rna'" + f" IN CASE OF ERROR, PLEASE REFER TO : 'logs/1_rna_harmony.log' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 # rna SCANORAMA
 @follows(set_up_dirs)
 @active_if(PARAMS['rna_run'])
 @active_if(PARAMS['rna_tools'] is not None and 'scanorama' in PARAMS['rna_tools'])
 @originate("batch_correction/umap_rna_scanorama.csv")
@@ -203,20 +215,22 @@
         cmd += " --neighbors_method %s" % neighbor_params['method']
     if neighbor_params['metric'] is not None:
         cmd += " --neighbors_metric %s" % neighbor_params['metric']
     if neighbor_params['npcs'] is not None:
         cmd += " --neighbors_n_pcs %s"  % neighbor_params['npcs']
     if neighbor_params['k'] is not None:
         cmd += " --neighbors_k %s" % neighbor_params['k']
-    cmd += " > logs/rna_scanorama.log " 
+    cmd += " > logs/1_rna_scanorama.log " 
     #job arguments
     
     if PARAMS['queues_long'] is not None:
         job_kwargs["job_queue"] = job_queue=PARAMS['queues_long']
     job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+    log_msg = f"TASK: 'run_scanorama_rna'" + f" IN CASE OF ERROR, PLEASE REFER TO : 'logs/1_rna_scanorama.log' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 # rna scvi
 @follows(set_up_dirs)
 @active_if(PARAMS['rna_run'])
 @active_if(PARAMS['rna_tools'] is not None and 'scvi' in PARAMS['rna_tools'])
 @originate("batch_correction/umap_rna_scvi.csv")
@@ -224,33 +238,38 @@
     cmd = """python %(py_path)s/batch_correct_scvi.py 
      --scaled_anndata %(preprocessed_obj)s
      --output_csv %(outfile)s 
      --integration_col %(rna_column)s
      --figdir figures/rna/
      """
     # cannot use the normal method for importing params from yaml, because it only works up to depth 2
+    # fetch seeds
+    scvi_params =  PARAMS['rna']['scvi']
+    cmd += " --scvi_seed %i" % scvi_params['seed']
     neighbor_params = PARAMS['rna']['neighbors']
     if neighbor_params['method'] is not None:
         cmd += " --neighbors_method %s" % neighbor_params['method']
     if neighbor_params['metric'] is not None:
         cmd += " --neighbors_metric %s" % neighbor_params['metric']
     if neighbor_params['npcs'] is not None:
         cmd += " --neighbors_n_pcs %s"  % neighbor_params['npcs']
     if neighbor_params['k'] is not None:
         cmd += " --neighbors_k %s" % neighbor_params['k']
-    cmd += " > logs/rna_scvi.log "
+    cmd += " > logs/1_rna_scvi.log "
     job_kwargs = {}
     if PARAMS['queues_gpu'] is not None:
         job_kwargs["job_queue"] = PARAMS['queues_gpu']
         job_kwargs["job_threads"] = int(PARAMS['resources_threads_gpu'])
     elif PARAMS['queues_long'] is not None:
             job_kwargs["job_queue"] = job_queue=PARAMS['queues_long']
             job_kwargs["job_threads"] = int(PARAMS['resources_threads_high'])
     else:
         job_kwargs["job_threads"] = int(PARAMS['resources_threads_high'])
+    log_msg = f"TASK: 'run_scvi_rna'" + f" IN CASE OF ERROR, PLEASE REFER TO : 'logs/1_rna_scvi.log' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 # rna scib
 # @transform([run_scvi, run_scanorama, run_bbknn, run_harmony, run_combat],
 #             regex(r"batch_correction/umap_rna_(.*).csv"),
 #             r'batch_correction/scib_metrics_\1.csv',r'\1', 
 #             scaled_file)
@@ -304,19 +323,21 @@
         cmd += " --neighbors_method %s" % neighbor_params['method']
     if neighbor_params['metric'] is not None:
         cmd += " --neighbors_metric %s" % neighbor_params['metric']
     if neighbor_params['npcs'] is not None:
         cmd += " --neighbors_n_pcs %s"  % neighbor_params['npcs']
     if neighbor_params['k'] is not None:
         cmd += " --neighbors_k %s" % neighbor_params['k']
-    cmd += " > logs/prot_no_correct.log"
+    cmd += " > logs/2_prot_no_correct.log"
     
     if PARAMS['queues_long'] is not None:
         job_kwargs["job_queue"] = job_queue=PARAMS['queues_long']
     job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+    log_msg = f"TASK: 'run_no_batch_correct_prot'" + f" IN CASE OF ERROR, PLEASE REFER TO : 'logs/2_prot_no_correct.log' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs) 
 
 # prot HARMONY
 @follows(set_up_dirs)
 @active_if(PARAMS['prot_run'])
 @active_if(PARAMS['prot_tools'] is not None and 'harmony' in PARAMS['prot_tools'])
 @originate("batch_correction/umap_prot_harmony.csv")
@@ -340,20 +361,22 @@
         cmd += " --neighbors_method %s" % neighbor_params['method']
     if neighbor_params['metric'] is not None:
         cmd += " --neighbors_metric %s" % neighbor_params['metric']
     if neighbor_params['npcs'] is not None:
         cmd += " --neighbors_n_pcs %s"  % neighbor_params['npcs']
     if neighbor_params['k'] is not None:
         cmd += " --neighbors_k %s" % neighbor_params['k']
-    cmd += " > logs/prot_harmony.log " 
+    cmd += " > logs/2_prot_harmony.log " 
      #job arguments
     
     if PARAMS['queues_long'] is not None:
         job_kwargs["job_queue"] = job_queue=PARAMS['queues_long']
     job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+    log_msg = f"TASK: 'run_harmony_prot'" + f" IN CASE OF ERROR, PLEASE REFER TO : 'logs/2_prot_harmony.log' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 
 
 # prot BBKNN
 @follows(set_up_dirs)
 @active_if(PARAMS['prot_run'])
@@ -367,19 +390,21 @@
      --integration_col %(prot_column)s
      --modality prot
      """
     if PARAMS['prot']['bbknn']['neighbors_within_batch'] is not None:
         cmd += " --neighbors_within_batch %i" % PARAMS['prot']['bbknn']['neighbors_within_batch']
     if PARAMS['prot']['neighbors']['npcs'] is not None:
         cmd += " --neighbors_n_pcs %s" % PARAMS['prot']['neighbors']['npcs']
-    cmd += " > logs/prot_bbknn.log "
+    cmd += " > logs/2_prot_bbknn.log "
     
     if PARAMS['queues_long'] is not None:
         job_kwargs["job_queue"] = job_queue=PARAMS['queues_long']
     job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+    log_msg = f"TASK: 'run_bbknn_prot'" + f" IN CASE OF ERROR, PLEASE REFER TO : 'logs/2_prot_bbknn.log' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs) 
 
 
 # prot COMBAT
 @follows(set_up_dirs)
 @active_if(PARAMS['prot_run'])
 @active_if(PARAMS['prot_tools'] is not None and 'combat' in PARAMS['prot_tools'])
@@ -398,20 +423,22 @@
         cmd += " --neighbors_method %s" % neighbor_params['method']
     if neighbor_params['metric'] is not None:
         cmd += " --neighbors_metric %s" % neighbor_params['metric']
     if neighbor_params['npcs'] is not None:
         cmd += " --neighbors_n_pcs %s"  % neighbor_params['npcs']
     if neighbor_params['k'] is not None:
         cmd += " --neighbors_k %s" % neighbor_params['k']
-    cmd += " > logs/prot_combat.log "
+    cmd += " > logs/2_prot_combat.log "
     
     if PARAMS['queues_long'] is not None:
         job_kwargs["job_queue"] = PARAMS['queues_long']
 
     job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+    log_msg = f"TASK: 'run_combat_prot'" + f" IN CASE OF ERROR, PLEASE REFER TO : 'logs/2_prot_combat.log' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs) 
     
 
 @active_if(PARAMS['prot_run'])
 @follows(run_harmony_prot, run_bbknn_prot,run_combat_prot, run_no_batch_umap_prot)
 def run_unimodal_integration_prot():
     pass
@@ -443,19 +470,21 @@
     if neighbor_params['k'] is not None:
         cmd += " --neighbors_k %s" % neighbor_params['k']
     atac_dimred = PARAMS['atac']['dimred']
     if PARAMS['atac']['dimred'] is not None:
         cmd += " --dimred %s" % atac_dimred
     else:
         cmd += " --dimred PCA"
-    cmd += " > logs/atac_no_correct.log"
+    cmd += " > logs/3_atac_no_correct.log"
     
     if PARAMS['queues_long'] is not None:
         job_kwargs["job_queue"] = job_queue=PARAMS['queues_long']
     job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+    log_msg = f"TASK: 'run_no_batch_correct_atac'" + f" IN CASE OF ERROR, PLEASE REFER TO : 'logs/3_atac_no_correct.log' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs) 
 
 # atac HARMONY
 @follows(set_up_dirs)
 @active_if(PARAMS['atac_run'])
 @active_if(PARAMS['atac_tools'] is not None and 'harmony' in PARAMS['atac_tools'])
 @originate("batch_correction/umap_atac_harmony.csv")
@@ -485,20 +514,22 @@
     if neighbor_params['k'] is not None:
         cmd += " --neighbors_k %s" % neighbor_params['k']
     atac_dimred = PARAMS['atac']['dimred']
     if PARAMS['atac']['dimred'] is not None:
         cmd += " --dimred %s" % atac_dimred
     else:
         cmd += " --dimred PCA"
-    cmd += " > logs/atac_harmony.log " 
+    cmd += " > logs/3_atac_harmony.log " 
      #job arguments
     
     if PARAMS['queues_long'] is not None:
         job_kwargs["job_queue"] = job_queue=PARAMS['queues_long']
     job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+    log_msg = f"TASK: 'run_harmony_atac'" + f" IN CASE OF ERROR, PLEASE REFER TO : 'logs/3_atac_harmony.log' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 # atac BBKNN
 @follows(set_up_dirs)
 @active_if(PARAMS['atac_run'] )
 @active_if(PARAMS['atac_tools'] is not None and 'bbknn' in PARAMS['atac_tools'])
 # @follows(normalise_log_hvg_regress_scale)
@@ -512,18 +543,20 @@
      """
     if PARAMS['atac']['bbknn']['neighbors_within_batch'] is not None:
         cmd += " --neighbors_within_batch %i" % PARAMS['atac']['bbknn']['neighbors_within_batch']
     if PARAMS['atac']['neighbors']['npcs'] is not None:
         cmd += " --neighbors_n_pcs %s" % PARAMS['atac']['neighbors']['npcs']
     #Forcing bbknn to run on PCA in case of atac
     cmd += " --dimred PCA"
-    cmd += " > logs/atac_bbknn.log "
+    cmd += " > logs/3_atac_bbknn.log "
     if PARAMS['queues_long'] is not None:
         job_kwargs["job_queue"] = PARAMS['queues_long']
     job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+    log_msg = f"TASK: 'run_bbknn_atac'" + f" IN CASE OF ERROR, PLEASE REFER TO : 'logs/3_atac_bbknn.log' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs) 
 
 
 @active_if(PARAMS['atac_run'])
 @follows(run_harmony_atac, run_no_batch_umap_atac, run_bbknn_atac)
 def run_unimodal_integration_atac():
     pass
@@ -546,34 +579,40 @@
     if os.path.exists("figures/multimodal") is False:
         os.makedirs("figures/multimodal")
     cmd = """python %(py_path)s/batch_correct_totalvi.py 
      --scaled_anndata %(preprocessed_obj)s
      --output_csv %(outfile)s 
      --figdir figures/
      """
+    scvi_params =  PARAMS['multimodal']['totalvi']
+    cmd += " --scvi_seed %i" % scvi_params['seed']
+    
+
     if PARAMS['multimodal_column_categorical'] is not None:
-        cmd += "--integration_col_categorical %(multimodal_column_categorical)s "
+        cmd += " --integration_col_categorical %(multimodal_column_categorical)s "
     neighbor_params = PARAMS['multimodal']['neighbors']
     if neighbor_params['method'] is not None:
         cmd += " --neighbors_method %s" % neighbor_params['method']
     if neighbor_params['metric'] is not None:
         cmd += " --neighbors_metric %s" % neighbor_params['metric']
     if neighbor_params['npcs'] is not None:
         cmd += " --neighbors_n_pcs %s"  % neighbor_params['npcs']
     if neighbor_params['k'] is not None:
         cmd += " --neighbors_k %s" % neighbor_params['k']
-    cmd += " > logs/multimodal_totalvi.log "
+    cmd += " > logs/4_multimodal_totalvi.log "
     
     if PARAMS['queues_gpu'] is not None:
         job_kwargs["job_queue"] = PARAMS['queues_gpu']
         job_kwargs["job_threads"] = int(PARAMS['resources_threads_gpu'])
     else:
         if PARAMS['queues_long'] is not None:
             job_kwargs["job_queue"] = job_queue=PARAMS['queues_long']
         job_kwargs["job_threads"] = int(PARAMS['resources_threads_high'])
+    log_msg = f"TASK: 'run_totalvi'" + f" IN CASE OF ERROR, PLEASE REFER TO : 'logs/4_multimodal_totalvi.log' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 # Run MultiVI
 
 @follows(set_up_dirs)
 @active_if(PARAMS['multimodal_run'])
 @active_if( PARAMS['multimodal_tools'] is not None)
@@ -583,39 +622,44 @@
     if os.path.exists("figures/multimodal") is False:
         os.makedirs("figures/multimodal")
     cmd = """python %(py_path)s/batch_correct_multivi.py 
      --scaled_anndata %(preprocessed_obj)s
      --output_csv %(outfile)s 
      --figdir figures/
      """
+    scvi_params =  PARAMS['multimodal']['MultiVI']
+    cmd += " --scvi_seed %i" % scvi_params['seed']
     
+
     if PARAMS['multimodal_column_categorical'] is not None:
-        cmd += "--integration_col_categorical %(multimodal_column_categorical)s "
+        cmd += " --integration_col_categorical %(multimodal_column_categorical)s "
 
     if PARAMS['multimodal_column_continuous'] is not None:
         cmd += "--integration_col_continuous %(multimodal_column_continuous)s "
 
     neighbor_params = PARAMS['multimodal']['neighbors']
     if neighbor_params['method'] is not None:
         cmd += " --neighbors_method %s" % neighbor_params['method']
     if neighbor_params['metric'] is not None:
         cmd += " --neighbors_metric %s" % neighbor_params['metric']
     if neighbor_params['npcs'] is not None:
         cmd += " --neighbors_n_pcs %s"  % neighbor_params['npcs']
     if neighbor_params['k'] is not None:
         cmd += " --neighbors_k %s" % neighbor_params['k']
-    cmd += " > logs/multimodal_multivi.log "
+    cmd += " > logs/4_multimodal_multivi.log "
     
     if PARAMS['queues_gpu'] is not None:
         job_kwargs["job_queue"] = PARAMS['queues_gpu']
         job_kwargs["job_threads"] = int(PARAMS['resources_threads_gpu'])
     else:
         if PARAMS['queues_long'] is not None:
             job_kwargs["job_queue"] = job_queue=PARAMS['queues_long']
         job_kwargs["job_threads"] = int(PARAMS['resources_threads_high'])
+    log_msg = f"TASK: 'run_multivi'" + f" IN CASE OF ERROR, PLEASE REFER TO : 'logs/4_multimodal_multivi.log' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 
 
 # Run Mofa
 @follows(set_up_dirs)
 @active_if(PARAMS['multimodal_run'])
@@ -655,15 +699,17 @@
         cmd += " --use_gpu True"
         job_kwargs["job_queue"] = PARAMS['queues_gpu']
         job_kwargs["job_threads"] = int(PARAMS['resources_threads_gpu'])
     else:
         if PARAMS['queues_long'] is not None:
             job_kwargs["job_queue"] = job_queue=PARAMS['queues_long']
         job_kwargs["job_threads"] = int(PARAMS['resources_threads_high'])
-    cmd += " > logs/multimodal_mofa.log "
+    cmd += " > logs/4_multimodal_mofa.log "
+    log_msg = f"TASK: 'run_mofa'" + f" IN CASE OF ERROR, PLEASE REFER TO : 'logs/4_multimodal_mofa.log' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 # Run WNN
 
 @follows(set_up_dirs)
 @follows(run_unimodal_integration)
 @active_if(PARAMS['multimodal_run'])
@@ -685,25 +731,26 @@
        cmd += " --n_bandwidth_neighbors %s" % wnn_params['n_bandwidth_neighbors']
     if wnn_params['n_multineighbors'] is not None:
        cmd += " --n_multineighbors %s" % wnn_params['n_multineighbors']
     if wnn_params['metric'] is not None:
        cmd += " --metric %s" % wnn_params['metric']
     if wnn_params['low_memory'] is not None:
        cmd += " --low_memory %s" % wnn_params['low_memory']
-    cmd += " > logs/multimodal_wnn.log"
+    cmd += " > logs/4_multimodal_wnn.log"
 
     
     if PARAMS['queues_gpu'] is not None:
         job_kwargs["job_queue"] = PARAMS['queues_gpu']
         job_kwargs["job_threads"] = int(PARAMS['resources_threads_gpu'])
     else:
         if PARAMS['queues_long'] is not None:
             job_kwargs["job_queue"] = job_queue=PARAMS['queues_long']
         job_kwargs["job_threads"] = int(PARAMS['resources_threads_high'])
-        
+    log_msg = f"TASK: 'run_wnn'" + f" IN CASE OF ERROR, PLEASE REFER TO : 'logs/4_multimodal_wnn.log' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 # end of multimodal
 @follows(run_mofa, run_wnn, run_totalvi, run_multivi)
 def run_multimodal_integration():
     pass
 # ------------------------------------------------------------------------
@@ -735,22 +782,24 @@
         cmd += " --rna_integration_col %(rna_column)s"
     if PARAMS['prot_run']:
         cmd += " --prot_integration_col %(prot_column)s"
     if PARAMS['atac_run']:
         cmd += " --atac_integration_col %(atac_column)s"
     if PARAMS['multimodal_run']:
         cmd += " --multimodal_integration_col %(multimodal_column_categorical)s"
-    cmd += " > logs/collate_mtd.log "
+    cmd += " > logs/5_collate_mtd.log "
     job_kwargs["job_threads"] = PARAMS['resources_threads_medium']
+    log_msg = f"TASK: 'collate_integration_outputs'" + f" IN CASE OF ERROR, PLEASE REFER TO : 'logs/5_collate_mtd.log' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)  
 
 
 # this COLLATE job will become the big final collate job across all possible combinations you may have run
 @follows(set_up_dirs)
-@transform(collate_integration_outputs, formatter(), "logs/plot_batch_corrected_umaps.log")
+@transform(collate_integration_outputs, formatter(), "logs/6_plot_batch_corrected_umaps.log")
 def plot_umaps(infile, outfile):
     print(infile, outfile)
     cell_mtd_file = sprefix + "_cell_mtd.csv"
     cmd = """python %(py_path)s/plot_umaps_batch_correct.py 
     --fig_dir figures/
     --combined_umaps_tsv %(infile)s
     --batch_dict batch_correction/batch_dict.yml
@@ -758,35 +807,60 @@
     """
     # 
     # Parse the whole dict of metrics
     # this contains grouping var and qc_metrics per modality
     cmd += ' --qc_dict "%(plotqc)s"'
     cmd += " > %(outfile)s" 
     job_kwargs["job_threads"] = PARAMS['resources_threads_medium']
+    log_msg = f"TASK: 'plot_umaps'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{outfile}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd,**job_kwargs)
 
 
 #this can follow now any mtd generation, but it will collate only RNA jobs for lisi
 @follows(collate_integration_outputs)
 @transform(collate_integration_outputs, 
-           formatter(),  'logs/lisi.log')
+           formatter(),  'logs/7_lisi.log')
 def run_lisi(infile, outfile):
     cell_mtd_file = sprefix + "_cell_mtd.csv"  
     cmd = """python %(py_path)s/run_lisi.py 
     --combined_umaps_df %(infile)s 
     --cell_meta_df %(cell_mtd_file)s
     --integration_dict batch_correction/batch_dict.yml
     --fig_dir figures/  > %(outfile)s 
     """ 
     job_kwargs["job_threads"] = PARAMS['resources_threads_low']
+    log_msg = f"TASK: 'run_lisi'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{outfile}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd,**job_kwargs)
 
 
+@follows(collate_integration_outputs)
+@transform(collate_integration_outputs, formatter(),  'logs/scib.log')
+def run_scib_metrics(infile, outfile):
+    cell_mtd_file = sprefix + "_cell_mtd.csv"
+    cmd = """python %(py_path)s/run_scib.py 
+    --combined_umaps_df %(infile)s 
+    --cell_meta_df %(cell_mtd_file)s
+    --integration_dict batch_correction/batch_dict.yml
+    --n_threads %(resources_threads_medium)s
+    --fig_dir figures/  > %(outfile)s 
+    """
+
+    if PARAMS['scib_rna']:
+        cmd += " --rna_cell_type %(scib_rna)s"
+    if PARAMS['scib_prot']:
+        cmd += " --prot_cell_type %(scib_prot)s"
+    if PARAMS['scib_atac']:
+        cmd += " --atac_cell_type %(scib_atac)s"
+
+    P.run(cmd, **job_kwargs)
+
 
-@follows(run_unimodal_integration, run_multimodal_integration,run_lisi, plot_umaps)
+@follows(run_unimodal_integration, run_multimodal_integration, run_lisi, run_scib_metrics, plot_umaps)
 @originate("logs/batch_correction_complete.log")
 def batch_correction(outfile):
     IOTools.touch_file(outfile)
 
 
 
 
@@ -822,16 +896,18 @@
         cmd += " --prot_correction_choice %(prot_choice)s"
     if choices['atac']['include'] and choices['atac']['bc_choice'] is not None:
         atac_choice = choices['atac']['bc_choice']
         cmd += " --atac_correction_choice %(atac_choice)s"
     if choices['multimodal']['include'] and choices['multimodal']['bc_choice'] is not None:
         multimodal_choice = choices['multimodal']['bc_choice']
         cmd += " --multimodal_correction_choice %(multimodal_choice)s"
-    cmd += " > logs/merge_final_obj.log"
+    cmd += " > logs/8_merge_final_obj.log"
     job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+    log_msg = f"TASK: 'merge_integration'" + f" IN CASE OF ERROR, PLEASE REFER TO : 'logs/8_merge_final_obj.log' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd,**job_kwargs)
     # clear up tmp since it is no longer required
     # P.run("rm -r tmp")
 
 
 def main(argv=None):
     if argv is None:
```

### Comparing `panpipes-0.4.1/panpipes/panpipes/pipeline_preprocess.py` & `panpipes-0.5.0/panpipes/panpipes/pipeline_preprocess.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 import logging
 from panpipes.funcs.io import dictionary_stripper
 # from itertools import chain
 # import glob
 
 # import pandas as pd
 
+
+def get_logger():
+    return logging.getLogger("cgatcore.pipeline")
+
+
 PARAMS = P.get_parameters(
     ["%s/pipeline.yml" % os.path.splitext(__file__)[0],
      "pipeline.yml"])
 
 
 PARAMS['py_path'] =  os.path.join(os.path.dirname(os.path.dirname(__file__)), 'python_scripts')
 PARAMS['r_path'] = os.path.join(os.path.dirname(os.path.dirname(__file__)), 'R_scripts')
@@ -48,16 +53,19 @@
         --output_mudata %(outfile)s
         --filter_dict "%(filter_dict)s"
         """
         if PARAMS['filtering_keep_barcodes'] is not None:
             cmd += " --keep_barcodes %(filtering_keep_barcodes)s"
         if PARAMS['intersect_mods'] is not None:
             cmd += " --intersect_mods %(intersect_mods)s"
-        cmd += " > logs/filtering.log "
+        logfile = "logs/1_filtering.log"
+        cmd += f" > {logfile}"
         job_kwargs["job_threads"] = PARAMS['resources_threads_low']
+        log_msg = f"TASK: 'filter_mudata'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{logfile}' FOR MORE INFORMATION."
+        get_logger().info(log_msg)
         P.run(cmd, **job_kwargs)
     else:
         try:
             f = open(outfile)
             f.close(outfile)
         except IOError:
             print("filter is not set to True, but there is no %s file" % outfile)
@@ -70,15 +78,15 @@
     del pqc['grouping_var']
     return any([x != None for x in pqc.values()])
 
 
 @active_if(PARAMS['filtering_run'])
 @active_if(run_plotqc_query(PARAMS['plotqc']))
 @follows(filter_mudata)
-@originate("logs/postfilterplot.log")
+@originate("logs/2_postfilterplot.log")
 def postfilterplot(log_file):
     cell_mtd_file = PARAMS['sample_prefix'] + "_filtered_cell_metadata.tsv"
     cmd = """
     Rscript %(r_path)s/plotQC.R 
     --prefilter FALSE
     --cell_metadata %(cell_mtd_file)s 
     --sampleprefix %(sample_prefix)s
@@ -91,45 +99,49 @@
         cmd += " --prot_qc_metrics %(plotqc_prot_metrics)s"
     if PARAMS['plotqc']['atac_metrics'] is not None:
         cmd += " --atac_qc_metrics %(plotqc_atac_metrics)s"
     if PARAMS['plotqc']['rep_metrics'] is not None:
         cmd += " --rep_qc_metrics %(plotqc_rep_metrics)s"
     cmd += " > %(log_file)s "
     job_kwargs["job_threads"] = PARAMS['resources_threads_low']
+    log_msg = f"TASK: 'postfilterplot'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{log_file}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 
 
 
 @active_if(PARAMS['downsample_n'] is not None)
 @follows(filter_mudata)
-@originate("logs/downsample.log", PARAMS['mudata_file'])
+@originate("logs/3_downsample.log", PARAMS['mudata_file'])
 def downsample(log_file, filt_obj):
     if PARAMS['downsample'] is not None:
         cmd="""
         python %(py_path)s/downsample.py
          --input_mudata %(filt_obj)s \
          --output_mudata %(filt_obj)s \
          --sampleprefix %(sample_prefix)s \
          --downsample_value %(downsample_n)s \
          --downsample_col %(downsample_col)s
          --intersect_mods %(downsample_mods)s
         """
         cmd += " > %(log_file)s  "
         job_kwargs["job_threads"] = PARAMS['resources_threads_low']
+        log_msg = f"TASK: 'downsample'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{log_file}' FOR MORE INFORMATION."
+        get_logger().info(log_msg)
         P.run(cmd, **job_kwargs)
     IOTools.touch_file(log_file)
     pass
 
 
 # setting these follows means that it still works if filter is False
 @active_if(mode_dictionary['rna'] is True)
 @follows(downsample)
 @follows(mkdir('figures/rna'))
-@transform(filter_mudata, formatter(), "logs/preprocess_rna.log")
+@transform(filter_mudata, formatter(), "logs/4_preprocess_rna.log")
 def rna_preprocess(adata_obj, log_file):
     cmd = """python %(py_path)s/run_preprocess_rna.py 
             --input_mudata %(adata_obj)s 
             --fig_dir figures/rna/ 
             --output_scaled_mudata %(adata_obj)s
             """
     # add in the options if specified in pipeline.yml
@@ -168,20 +180,22 @@
             cmd += " --pca_solver arpack"
         else:
             cmd += " --pca_solver %(pca_solver)s"
     if PARAMS['pca_color_by'] is not None:
         cmd += " --color_by %(pca_color_by)s"
     cmd += " > %(log_file)s "
     job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+    log_msg = f"TASK: 'rna_preprocess'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{log_file}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 
 @active_if(mode_dictionary['prot'] is True)
 @follows(rna_preprocess)
-@originate("logs/preprocess_prot.log", PARAMS['mudata_file'])
+@originate("logs/4_preprocess_prot.log", PARAMS['mudata_file'])
 def prot_preprocess( log_file, scaled_file, ):
     if os.path.exists("figures/prot") is False:
         os.mkdir("figures/prot" )
     cmd = """
         python %(py_path)s/run_preprocess_prot.py
         --filtered_mudata %(scaled_file)s
         --figpath ./figures/prot
@@ -200,29 +214,31 @@
     if PARAMS['prot_save_norm_prot_mtx'] is True:
         cmd += " --save_mtx True"
     if PARAMS["prot_pca"] is True:
         if PARAMS['prot_solver'] is not None:
             if PARAMS['prot_solver'] == "default":
                 cmd += " --pca_solver arpack"
             else:
-                cmd += " --pca_solver %(pca_solver)s"
+                cmd += " --pca_solver %(prot_solver)s"
         cmd += """ 
         --run_pca True
         --n_pcs %(prot_n_pcs)s
         --color_by %(prot_color_by)s
         """
     cmd += " > %(log_file)s"
     job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+    log_msg = f"TASK: 'prot_preprocess'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{log_file}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 
 @active_if(mode_dictionary['atac'] is True)
 @follows(prot_preprocess)
 # @transform(rna_preprocess,formatter(),"logs/preprocess_atac.log")
-@originate("logs/preprocess_atac.log", PARAMS['mudata_file'])
+@originate("logs/4_preprocess_atac.log", PARAMS['mudata_file'])
 def atac_preprocess(log_file, scaled_file):
     if os.path.exists("figures/atac") is False:
         os.mkdir("figures/atac" )
     cmd = """
         python %(py_path)s/run_preprocess_atac.py
         --input_mudata %(scaled_file)s
         --output_mudata %(scaled_file)s
@@ -265,14 +281,16 @@
     if PARAMS['atac_feature_selection_flavour'] is not None:
         cmd += " --feature_selection_flavour %(atac_feature_selection_flavour)s"
     if PARAMS['atac_min_cutoff'] is not None:
         cmd += " --min_cutoff %(atac_min_cutoff)s"
     cmd += " --color_by %(atac_color_by)s" 
     cmd += " > %(log_file)s"
     job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+    log_msg = f"TASK: 'atac_preprocess'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{log_file}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 
 
 # @active_if(mode_dictionary['rep'] is True)
 # @follows(atac_preprocess)
 # # @transform(rna_preprocess,formatter(),"logs/preprocess_rep.log")
```

### Comparing `panpipes-0.4.1/panpipes/panpipes/pipeline_preprocess_spatial/pipeline.yml` & `panpipes-0.5.0/panpipes/panpipes/pipeline_preprocess_spatial/pipeline.yml`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # ---------------------------
 # 0. Compute resource options
 # ---------------------------
 
 resources:
   # Number of threads used for parallel jobs
-  threads_high: 1 # Must be enough memory to load all input files and create MuDatas
+  threads_high: 1 # Number of threads used for high intensity computing tasks
   threads_medium: 1  # Must be enough memory to load your mudata and do computationally light tasks
   threads_low: 1 # Must be enough memory to load text files and do plotting, requires much less memory
 
 condaenv:  # Path to conda env, leave blank if running native or your cluster automatically inherits the login node environment
 
 
 # ------------------
@@ -115,16 +115,16 @@
   clip: # Leave blank to use default (None)
   # 'clip' can be specified as:
   #    None: residuals are clipped to the interval [-sqrt(n_obs), sqrt(n_obs)]
   #    a float value: if float c specified: clipped to the interval [-c, c]
   #    np.Inf: no clipping
 
   # Parameters for both cases norm_hvg_flavour = "seurat" and "squidpy":
-  n_top_genes: 2000 # Default is None; mandatory for norm_hvg_flavour = "seurat" and squidpy_hvg_flavor: "seurat_v3"
+  n_top_genes: 2000 # Leave blank to use default (2000); mandatory for norm_hvg_flavour = "seurat" and squidpy_hvg_flavor: "seurat_v3"
   filter_by_hvg: False # Leave blank to use default (False); if True, subset the data to highly-variable genes after finding them
   hvg_batch_key: # Leave blank to use default (None); if specified, highly-variable genes are selected within each batch separately and merged
 
-  n_pcs: 50 # Leave blank to use default (50); how many PCs to compute with sc.pp.PCA()
+  n_pcs: 50 # Leave blank to use default (50); how many PCs to compute with sc.pp.PCA() and plot in sc.pl.pca_variance_ratio()
```

### Comparing `panpipes-0.4.1/panpipes/panpipes/pipeline_preprocess_spatial.py` & `panpipes-0.5.0/panpipes/panpipes/pipeline_preprocess_spatial.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import sys
 import os
 from cgatcore import pipeline as P
 import glob
 import logging
 from panpipes.funcs.io import dictionary_stripper
 
-
+def get_logger():
+    return logging.getLogger("cgatcore.pipeline")
 
 PARAMS = P.get_parameters(
     ["%s/pipeline.yml" % os.path.splitext(__file__)[0],
      "pipeline.yml"])
 
 
 PARAMS['py_path'] =  os.path.join(os.path.dirname(os.path.dirname(__file__)), 'python_scripts')
@@ -50,28 +51,30 @@
 @mkdir("figures")
 @mkdir("tables")
 @mkdir("filtered.data")
 @files(gen_filter_jobs)
 def filter_mudata(infile_path,outfile):
     print('processing file = %s' % str(infile_path))
     log_file = os.path.basename(outfile)
-    log_file= "filtering."+log_file.replace("filtered.h5mu","") + ".log"
+    log_file= "1_filtering."+log_file.replace("filtered.h5mu","") + ".log"
 
 
     filter_dict = dictionary_stripper(PARAMS['filtering'])
     cmd = """
         python %(py_path)s/run_filter_spatial.py
         --input_mudata %(infile_path)s
         --output_mudata %(outfile)s
         --filter_dict "%(filter_dict)s"
         """
     if PARAMS['filtering_keep_barcodes'] is not None:
         cmd += " --keep_barcodes %(filtering_keep_barcodes)s"
     cmd += " > logs/%(log_file)s "
     job_kwargs["job_threads"] = PARAMS['resources_threads_low']
+    log_msg = f"TASK: 'filter_mudata'" + f" IN CASE OF ERROR, PLEASE REFER TO : 'logs/{log_file}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
     
 
 
 def run_plotqc_query(pqc_dict):
     # avoid deleting from PARAMS
     pqc = pqc_dict.copy()
@@ -79,15 +82,15 @@
     return any([x != None for x in pqc.values()])
 
 
 @active_if(run_plotqc_query(PARAMS['plotqc']))
 @active_if(PARAMS['filtering_run'])
 @transform(filter_mudata,
            regex("./filtered.data/(.*)_filtered.h5(.*)"), 
-           r"./logs/postfilterplot.\1.log")
+           r"./logs/2_postfilterplot.\1.log")
 def postfilterplot_spatial(filt_file,log_file):
     print(filt_file)    
     print(log_file)
     spatial_filetype = PARAMS["assay"]
     cmd = """
             python %(py_path)s/plot_qc_spatial.py
              --input_mudata %(filt_file)s
@@ -96,20 +99,22 @@
             """
     if PARAMS['plotqc']['grouping_var'] is not None:
         cmd += " --grouping_var %(plotqc_grouping_var)s"
     if PARAMS['plotqc']['spatial_metrics'] is not None:
         cmd += " --spatial_qc_metrics %(plotqc_spatial_metrics)s"
     cmd += " > %(log_file)s "
     job_kwargs["job_threads"] = PARAMS['resources_threads_low']
+    log_msg = f"TASK: 'postfilterplot'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{log_file}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 
 @transform(filter_mudata,
            regex("./filtered.data/(.*)_filtered.h5(.*)"), 
-           r"./logs/st_preprocess.\1.log")
+           r"./logs/3_preprocess.\1.log")
 def spatial_preprocess(filt_file,log_file):
     if os.path.exists("figures/spatial") is False:
         os.mkdir("figures/spatial")
     if os.path.exists("./tmp") is False:
         os.mkdir("./tmp")
     write_output = os.path.join("./tmp/",os.path.basename(filt_file))
     cmd = """
@@ -141,14 +146,16 @@
     if PARAMS['spatial_clip'] is not None:
         cmd += " --clip %(spatial_clip)s"
     if PARAMS['spatial_n_pcs'] is not None:
         cmd += " --n_pcs %(spatial_n_pcs)s"
 
     cmd += " > %(log_file)s"
     job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+    log_msg = f"TASK: 'spatial_preprocess'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{log_file}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 @follows(filter_mudata, postfilterplot_spatial, spatial_preprocess)
 @originate("cleanup_done.txt")
 def cleanup(file):
     # remove any ctmp fails
     P.run("rm ctmp*", without_cluster=True)
```

### Comparing `panpipes-0.4.1/panpipes/panpipes/pipeline_qc_spatial/pipeline.yml` & `panpipes-0.5.0/panpipes/panpipes/pipeline_qc_spatial/pipeline.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# ============================================================
+# =============================================================================
 # Ingestion, spatial transcriptomics workflow Panpipes (pipeline_qc_spatial.py)
-# ============================================================
+# =============================================================================
 # Written by Fabiola Curion and Sarah Ouologuem
 
 
 # This pipeline needs a sample metadata file (see resources for an example)
 # Will run :
 #   scanpy QC
 #   summary QC plots
@@ -72,10 +72,10 @@
 # ---------------
 # Plot QC metrics
 # ---------------
 
 # All metrics and grouping variables should be inputted as a comma separated string without spaces, e.g. a,b,c
 
 plotqc:
-  grouping_var: sample_id # sample_id is the name of each spatial slide (specified in the submission file) and it will always be used to plot.
+  grouping_var: sample_id # sample_id is the name of each spatial slide (specified in the submission file)
   spatial_metrics: total_counts,n_genes_by_counts # If metric is present in both, .obs and .var, both will be plotted
```

### Comparing `panpipes-0.4.1/panpipes/panpipes/pipeline_qc_spatial.py` & `panpipes-0.5.0/panpipes/panpipes/pipeline_qc_spatial.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,20 +10,23 @@
 from panpipes.funcs.io import gen_load_spatial_jobs
 # from scpipelines.funcs.processing import intersection
 import warnings
 warnings.simplefilter(action='ignore', category=FutureWarning)
 warnings.filterwarnings("ignore", category=DeprecationWarning) 
 
 import warnings
+import logging
 
 # warnings.simplefilter('ignore', category=NumbaDeprecationWarning)
 # warnings.simplefilter('ignore', category=NumbaPendingDeprecationWarning)
 
 import yaml
 
+def get_logger():
+    return logging.getLogger("cgatcore.pipeline")
 
 PARAMS = P.get_parameters(
     ["%s/pipeline.yml" % os.path.splitext(__file__)[0],
      "pipeline.yml"])
 
 PARAMS['py_path'] =  os.path.join(os.path.dirname(os.path.dirname(__file__)), 'python_scripts')
 PARAMS['r_path'] = os.path.join(os.path.dirname(os.path.dirname(__file__)), 'R_scripts')
@@ -104,28 +107,29 @@
         --spatial_counts %(spatial_counts)s
     """
     if spatial_filetype == "vizgen":
         cmd += """
         --spatial_metadata %(spatial_metadata)s 
         --spatial_transformation %(spatial_transformation)s
         """
-    cmd += " > logs/make_mudatas_%(sample_id)s.log"
-    print(cmd)
+    cmd += " > logs/1_make_mudatas_%(sample_id)s.log"
     job_kwargs["job_threads"] = PARAMS['resources_threads_medium']
+    log_msg = f"TASK: 'load_mudatas'" + f" IN CASE OF ERROR, PLEASE REFER TO : 'logs/1_make_mudatas_{sample_id}.log' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 
 
 
 @follows(load_mudatas)
 @follows(mkdir("qc.data"))
 @follows(mkdir("./figures"))
 @transform(load_mudatas,
            regex("./tmp/(.*)_raw.h5(.*)"), 
-           r"./logs/spatialQC_\1.log")
+           r"./logs/2_spatialQC_\1.log")
 def spatialQC(infile,log_file):
     spatial_filetype = assays[infile]
     resources_path = os.path.join(os.path.dirname(os.path.dirname(__file__)), "resources")
     outfile = infile.replace("_raw","_unfilt")
     outfile = outfile.replace("tmp", "qc.data")
     cmd = """
             python %(py_path)s/run_scanpyQC_spatial.py
@@ -147,16 +151,17 @@
             customgenesfile = PARAMS['custom_genes_file']
         cmd += " --customgenesfile %(customgenesfile)s"
     if PARAMS['score_genes'] is not None:
         cmd += " --score_genes %(score_genes)s"
     if PARAMS['calc_proportions'] is not None:
         cmd += " --calc_proportions %(calc_proportions)s"
     cmd += " > %(log_file)s"
-
     job_kwargs["job_threads"] = PARAMS['resources_threads_medium']
+    log_msg = f"TASK: 'spatialQC'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{log_file}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 
 def run_plotqc_query(pqc_dict):
     # avoid deleting from PARAMS
     pqc = pqc_dict.copy()
     del pqc['grouping_var']
@@ -164,15 +169,15 @@
 
 
 @follows(spatialQC)
 @follows(mkdir("./figures/spatial"))
 @active_if(run_plotqc_query(PARAMS['plotqc']))
 @transform(load_mudatas, 
            regex("./tmp/(.*)_raw.h5(.*)"),
-           r"./logs/qcplot.\1.log")
+           r"./logs/3_qcplot.\1.log")
 def plotQC_spatial(unfilt_file,log_file):
     spatial_filetype = assays[unfilt_file]
     unfilt_file = unfilt_file.replace("_raw","_unfilt")
     unfilt_file = unfilt_file.replace("tmp", "qc.data")
     cmd = """
             python %(py_path)s/plot_qc_spatial.py
              --input_mudata %(unfilt_file)s
@@ -181,14 +186,16 @@
             """
     if PARAMS['plotqc']['grouping_var'] is not None:
         cmd += " --grouping_var %(plotqc_grouping_var)s"
     if PARAMS['plotqc']['spatial_metrics'] is not None:
         cmd += " --spatial_qc_metrics %(plotqc_spatial_metrics)s"
     cmd += " > %(log_file)s "
     job_kwargs["job_threads"] = PARAMS['resources_threads_low']
+    log_msg = f"TASK: 'plotQC_spatial'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{log_file}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
     
 #----- end
 
 @follows(plotQC_spatial)
 def full():
```

### Comparing `panpipes-0.4.1/panpipes/panpipes/pipeline_refmap/pipeline.yml` & `panpipes-0.5.0/panpipes/panpipes/pipeline_refmap/pipeline.yml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   threads_medium: 1
   # this must be enough memory to load text files and do plotting, requires much less memory than the other two
   threads_low: 1
 # path to conda env, leave blank if running native or your cluster automatically inherits the login node environment
 condaenv:
 
 # allows for tweaking which queues jobs get submitted to, 
-# in case there is a special queue for long jobs or you have access to a gpu-sepcific queue
+# in case there is a special queue for long jobs or you have access to a gpu-specific queue
 # the default queue should be specified in your .cgat.yml file
 # leave as is if you do not want to use the alternative queues
 queues:
   long: 
   gpu:  
 
 #----------------------
@@ -49,15 +49,15 @@
 # specify the reference anndata/mudata with RNA. you need this only if you want to calc umap on both reference and query data.
 # otherwise leave blank and only provide model paths
 reference_data: path_to_mudata 
 # path to tovalvi saved model
 totalvi: 
   - path_to_totalvi1
   - path_to_totalvi2
-impute_proteins: True
+impute_proteins: False
 # transform_batch is a batch-covariate specific to totalvi, allows the model to use the batch information in the query to mitigate 
 # differences in protein sequencing depth
 transform_batch:
 # Specify the full path to the model, i.e. Path/to/scanvi/model.pt
 # if not running the method, remove the dummy - path_to_xxx and leave blank
 scvi:
   - path_to_scvi
```

### Comparing `panpipes-0.4.1/panpipes/panpipes/pipeline_refmap.py` & `panpipes-0.5.0/panpipes/panpipes/pipeline_refmap.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,20 @@
 import os
 from cgatcore import pipeline as P
 import pandas as pd
 import cgatcore.iotools as IOTools
 import re
 from itertools import chain
 import glob
+import logging
+
+def get_logger():
+    return logging.getLogger("cgatcore.pipeline")
+
 
-# __file__="/well/cartography/users/zsj686/non_cart_projects/005-multimodal_scpipelines/src/sc_pipelines_muon_dev/panpipes/pipeline_refmap.py"
 PARAMS = P.get_parameters(
     ["%s/pipeline.yml" % os.path.splitext(__file__)[0],
      "pipeline.yml"])
 
 job_kwargs = {}
 
 if PARAMS['condaenv'] is not None:
@@ -58,15 +62,15 @@
                 # this is creating output files based on the model folder name
                 out_prefix=os.path.basename(os.path.dirname(infile))
                 model_name = ''.join(e for e in out_prefix if e.isalnum())
                 latent_choice = "X_" + ref_architecture
                 file_name= "umap_" + model_name + "_" + latent_choice
                 outfile = os.path.join("./refmap/",(file_name + ".csv"))
 
-                log_file = os.path.join('logs/', out_prefix + ".log")
+                log_file = os.path.join('logs/', "1_"+out_prefix + ".log")
                 yield infile, outfile, log_file, ref_architecture
                 
 
 
 # error if modality is not rna
 
 # ------------------------------
@@ -100,15 +104,26 @@
         cmd += " --adata_reference %(reference_data)s "
     if ref_architecture == "totalvi":
        cmd += "  --impute_proteins %(impute_proteins)s"
     if PARAMS['run_randomforest'] is not None:
         cmd += " --predict_rf %(run_randomforest)s"
        
     cmd += " > %(log_file)s"
-    job_kwargs["job_threads"] = PARAMS['resources_threads_low']
+
+    if PARAMS['queues_gpu'] is not None:
+        job_kwargs["job_queue"] = PARAMS['queues_gpu']
+        job_kwargs["job_threads"] = int(PARAMS['resources_threads_gpu'])
+    elif PARAMS['queues_long'] is not None:
+            job_kwargs["job_queue"] = job_queue=PARAMS['queues_long']
+            job_kwargs["job_threads"] = int(PARAMS['resources_threads_high'])
+    else:
+        job_kwargs["job_threads"] = int(PARAMS['resources_threads_high'])
+
+    log_msg = f"TASK: 'run_refmap_scvi'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{log_file}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 
 ##TODO remove this collate job cause plotting is now in the script
 # @collate([run_refmap_scvi], #multimodal
 #          regex(r"refmap/(.*)"), # this does nothing
 #           r'refmap/combined_umaps.tsv')
@@ -122,15 +137,15 @@
 #     """ 
 #     cmd += " > logs/collate_outputs.log "
 #     job_kwargs["job_threads"] = PARAMS['resources_threads_low']
 #     P.run(cmd, **job_kwargs)  
 @active_if(PARAMS["scib_run"])
 @transform(run_refmap_scvi,
            regex(r"refmap/umap_(.*).csv"),
-           r'logs/refmapscib_\1.log')
+           r'logs/2_refmapscib_\1.log')
 def run_scib_refmap(infile,logfile):
     str_use = os.path.splitext(os.path.basename(infile).replace("umap_", "").replace(".csv", ""))[0]
     mudata_input= "query_to_reference_" + str_use + ".h5mu"
     repuse = "X_"+ str_use.split("_")[-1]    
     cmd="""
     python %(py_path)s/refmap_scib.py
     --query ./refmap/%(mudata_input)s
@@ -146,15 +161,17 @@
         cmd += " --cluster_key %(scib_cluster_key)s" 
     if PARAMS["scib_celltype_key"] is not None:
         cmd += " --covariate %(scib_celltype_key)s"
     else: 
         if PARAMS['query_celltype'] is not None:
             cmd += " --covariate %(query_celltype)s"
     cmd += " > %(logfile)s"
-    job_kwargs["job_threads"] = PARAMS['resources_threads_medium']
+    job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+    log_msg = f"TASK: 'run_scib_refmap'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{logfile}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)  
 
 
 @follows(run_scib_refmap)
 def full():
     """
     All cgat pipelines should end with a full() function which updates,
```

### Comparing `panpipes-0.4.1/panpipes/panpipes/pipeline_vis/pipeline.yml` & `panpipes-0.5.0/panpipes/panpipes/pipeline_vis/pipeline.yml`

 * *Files identical despite different names*

### Comparing `panpipes-0.4.1/panpipes/panpipes/pipeline_vis.py` & `panpipes-0.5.0/panpipes/panpipes/pipeline_vis.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,20 @@
 from cgatcore import pipeline as P
 import pandas as pd
 import cgatcore.iotools as IOTools
 import re
 from itertools import chain, product
 import glob
 from panpipes.funcs.io import dictionary_stripper 
+import logging
+
+def get_logger():
+    return logging.getLogger("cgatcore.pipeline")
+
+
 
 PARAMS = P.get_parameters(
     ["%s/pipeline.yml" % os.path.splitext(__file__)[0],
      "pipeline.yml"])
 
 PARAMS['py_path'] =  os.path.join(os.path.dirname(os.path.dirname(__file__)), 'python_scripts')
 PARAMS['r_path'] = os.path.join(os.path.dirname(os.path.dirname(__file__)), 'R_scripts')
@@ -46,15 +52,15 @@
 
 do_plot_features = (PARAMS['custom_markers']['files']['full'] is not None or PARAMS['custom_markers']['files']['minimal'] is not None) and \
                 (PARAMS['do_plots_marker_dotplots'] or PARAMS['do_plots_marker_matrixplots'])
 
 
 @follows(set_up_dirs)
 @active_if(do_plot_features)
-@transform(marker_files, formatter(), "logs/markers_by_group__{basename[0]}.log")
+@transform(marker_files, formatter(), "logs/1_plot_markers_by_group__{basename[0]}.log")
 def plot_custom_markers_per_group(marker_file, log_file):
     print(marker_file)
     print(log_file)
     group_vars = " ".join(PARAMS["grouping_vars"])
     # pull out the modalities to use, not including multimodal.
     modalities = [key for key, val in PARAMS['modalities'].items() if val and key not in ["multimodal", "rep"]]
     modalities = ",".join(modalities)
@@ -68,22 +74,24 @@
             --layers "%(layer_vars)s" \
             --marker_file %(marker_file)s \
             --group_cols %(group_vars)s \
             --base_figure_dir ./
      """
     cmd += " > %(log_file)s "
     job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+    log_msg = f"TASK: 'plot_custom_markers_per_group'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{log_file}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 
 plot_embeddings = any([True if val['run'] is True else False for val in PARAMS["embedding"].values() ])
 @active_if(plot_embeddings )
 @follows(set_up_dirs)
 @active_if(PARAMS['custom_markers']['files']['minimal'] is not None)
-@transform(PARAMS['custom_markers']['files']['minimal'], formatter(), "logs/markers_umap_{basename[0]}.log")
+@transform(PARAMS['custom_markers']['files']['minimal'], formatter(), "logs/2_plot_markers_umap_{basename[0]}.log")
 def plot_custom_markers_umap(marker_file, log_file):
     embedding_dict = PARAMS["embedding"]
     embedding_dict =  {mod:val['basis'] for mod, val in embedding_dict.items() if val['run'] is True}
     embedding_dict = dictionary_stripper(embedding_dict)
     layer_vars = {key:val  for key, val in PARAMS['custom_markers_layers'].items() if PARAMS['modalities'][key]}
     layer_vars = dictionary_stripper(layer_vars)
     modalities = ",".join([key for key, val in PARAMS['modalities'].items() if val])
@@ -94,23 +102,25 @@
             --layers "%(layer_vars)s" \
             --basis_dict "%(embedding_dict)s" \
             --marker_file %(marker_file)s \
             --base_figure_dir ./
     """
     cmd += " > %(log_file)s "
     job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+    log_msg = f"TASK: 'plot_custom_markers_umap'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{log_file}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 
 
 
 # @transform(PARAMS['custom_markers']['files']['minimal'], formatter(), "logs/markers_umap__{basename[0]}.log")
 @active_if(plot_embeddings )
 @follows(set_up_dirs)
-@originate("logs/categorical_variables_umap.log")
+@originate("logs/3_plot_categorical_variables_umap.log")
 def plot_categorical_umaps(log_file):
     embedding_dict = PARAMS["embedding"]
     embedding_dict =  {mod:val['basis'] for mod, val in embedding_dict.items() if val['run'] is True}
     cat_vars = PARAMS['categorical_vars']
     if "all" in cat_vars.keys() and cat_vars["all"] is not None:    
         for k, v in cat_vars.items():
             if v is None:
@@ -128,20 +138,22 @@
             --basis_dict "%(embedding_dict)s" \
             --categorical_variables "%(cat_vars)s" \
             --base_figure_dir ./
             --fig_suffix categorical_vars.png
     """
     cmd += " > %(log_file)s "
     job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+    log_msg = f"TASK: 'plot_categorical_umaps'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{log_file}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 
 @active_if(plot_embeddings)
 @follows(set_up_dirs)
-@originate("logs/continuous_variables_umap.log")
+@originate("logs/4_plot_continuous_variables_umap.log")
 def plot_continuous_umaps(log_file):
     embedding_dict = PARAMS["embedding"]
     embedding_dict =  {mod:val['basis'] for mod, val in embedding_dict.items() if val['run'] is True}
     cont_vars = PARAMS['continuous_vars']
     if "all" in cont_vars.keys() and cont_vars["all"] is not None:    
         for k, v in cont_vars.items():
             if v is None:
@@ -160,66 +172,74 @@
             --basis_dict "%(embedding_dict)s" 
             --continuous_variables "%(cont_vars)s" 
             --base_figure_dir ./
             --fig_suffix continuous_vars.png
     """
     cmd += " > %(log_file)s "
     job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+    log_msg = f"TASK: 'plot_continuous_umaps'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{log_file}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 
 do_plot_metrics = any([PARAMS['do_plots_categorical_barplots'],
                 PARAMS['do_plots_categorical_stacked_barplots'],
                 PARAMS['do_plots_continuous_violin']])
 # write metadata out
 @active_if(do_plot_metrics)
 @originate(PARAMS['sample_prefix'] + "_cell_metadata.tsv")
 def write_obs(cmtd):
     cmd = """
         python %(py_path)s/write_metadata.py
         --infile %(mudata_obj)s
-        --outfile %(cmtd)s > logs/write_obs.log
+        --outfile %(cmtd)s > logs/5_write_obs.log
         """
     job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+    log_msg = f"TASK: 'write_obs'" + f" IN CASE OF ERROR, PLEASE REFER TO : 'logs/5_write_obs.log' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
   
 
 # Plot cluster metrics
 @follows(set_up_dirs)
 @active_if(do_plot_metrics)
-@transform(write_obs, formatter(), "logs/plot_metrics.log")
+@transform(write_obs, formatter(), "logs/6_plot_metrics.log")
 def plot_metrics(mtd, log_file):
     cmd = """
     Rscript %(r_path)s/plot_metrics.R \
         --mtd_object %(mtd)s \
         --params_yaml pipeline.yml > %(log_file)s
     """
     job_kwargs["job_threads"] = PARAMS['resources_threads_low']
+    log_msg = f"TASK: 'plot_metrics'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{log_file}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)
 
 
 # parse the scatter files
 scatter_files = [PARAMS['paired_scatters'], PARAMS['custom_markers_files']['paired_scatters']]
 scatter_files = [sc if type(sc) is list else [sc] for sc in scatter_files if sc is not None]
 scatter_files = list(set(chain(*scatter_files)))
 @follows(set_up_dirs)
-@active_if(PARAMS['do_plots_paired_scatters'])
 @active_if(len(scatter_files) != 0)
+@active_if(PARAMS['do_plots_paired_scatters'])
 @transform(scatter_files,
-            formatter(), "logs/scatters__{basename[0]}.log")
+            formatter(), "logs/7_plot_scatters__{basename[0]}.log")
 def plot_scatters(infile, log_file):
     print(infile)
     cmd = """
         python %(py_path)s/plot_features_scatter.py
         --mdata_object %(mudata_obj)s
         --layers_dict "%(custom_markers_layers)s" 
         --scatters_csv %(infile)s
         > %(log_file)s
         """
     job_kwargs["job_threads"] = PARAMS['resources_threads_high']
+    log_msg = f"TASK: 'plot_scatters'" + f" IN CASE OF ERROR, PLEASE REFER TO : '{log_file}' FOR MORE INFORMATION."
+    get_logger().info(log_msg)
     P.run(cmd, **job_kwargs)    
 
 
 @follows(plot_custom_markers_per_group, plot_custom_markers_umap,
  plot_continuous_umaps, plot_categorical_umaps, plot_metrics, plot_scatters)
 def full():
     """
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/aggregate_cellranger_summary_metrics.py` & `panpipes-0.5.0/panpipes/python_scripts/aggregate_cellranger_summary_metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                     help='')
 parser.add_argument('--cellranger_column_conversion_df',
                     default='',
                     help='')
 parser.set_defaults(verbose=True)
 args = parser.parse_args()
 
-L.info(args)
+L.info("Running with params: %s", args)
 
 def check_path(path):
     if os.path.isfile(path):
         return os.path.dirname(path)
     elif os.path.isdir(path):
         return path
     else:
@@ -56,31 +56,31 @@
 
     Args:
         path (str):path to the folder called 'outs'
         sample_id (str): Required if path is to cellranger multi outputs, defaults to None
     """    
     # subset path to only go up to 'outs'
     if 'outs' not in path:
-        print("you are parsing a cellranger output but your path to raw data doesn't end wth the outs folder")
+        L.warning("You are parsing a cellranger output but your path to raw data doesn't end with the outs folder")
         path = check_path(path)
     else:
         path = path.split("outs")[0] + "outs"
     outpath=None
     # use the path to cellranger count or vdj outputs as default
     if os.path.exists(os.path.join(path, 'metrics_summary.csv') ):
         outpath = os.path.join(path, 'metrics_summary.csv') 
     elif os.path.exists(os.path.join(path, 'summary.csv') ):
         outpath = os.path.join(path, 'summary.csv') 
     elif sample_id is not None and os.path.exists(os.path.join(path, 'per_sample_outs', sample_id, 'metrics_summary.csv') ):
         outpath = os.path.join(path, 'per_sample_outs', sample_id, 'metrics_summary.csv')
     elif sample_id is None and os.path.exists(os.path.join(path, 'per_sample_outs')):
-        print('input folder appears to be from cellranger multi but no sample_id is given')
+        L.warning('Input folder appears to be from cellranger multi but no sample_id is given')
     else:
         # use the alternative path from cellranger_multi outputs
-        print('path not found')
+        L.warning('Path not found')
     return outpath
 
 
 def detect_cellranger_algorithm(pth):
     if 'per_sample_outs' in pth:
         filetype='multi'
     else:
@@ -174,59 +174,61 @@
     # convert percentages from string to numeric
     msums['metric_value'] = [re.sub(",|%", "", str(x)) for x in msums['metric_value']]
     msums['metric_value'] = msums['metric_value'].astype(float)
     msums = msums.sort_values(['library_type', 'metric_name', 'sample_id'])
     return msums
     
 
+L.info("Reading in tsv file '%s'" % args.cellranger_column_conversion_df)
 convert_df = pd.read_csv(args.cellranger_column_conversion_df, sep='\t')   
 
 # get the paths
 pipe_df = pd.read_csv(args.pipe_df, sep='\t')
-L.info('finding all the cellranger paths')
+L.info('Searching for all cellranger paths')
 all_paths_df = get_all_unique_paths(pipe_df)
 all_paths_df['metrics_summary_path'] = all_paths_df.apply(lambda x: get_metrics_summary_path(path=x.path, sample_id=x.sample_id), axis=1)
 # all_paths_df_uniq = all_paths_df.drop(columns=['path', 'path_type']).drop_duplicates().reset_index(drop=True)
 all_paths_df['cellranger_type'] = [detect_cellranger_algorithm(x) for x in all_paths_df['metrics_summary_path']]
-L.info('cellranger metrics_summary files found')
-L.info(all_paths_df)
+L.info("Cellranger metrics_summary files found: %s" % all_paths_df)
 
 # parse and concatenate the tenx x metrics summary files into long format
+L.info("Parsing and concatenating the 10X metrics summary files into long format")
 tenx_metrics = []
 if any(all_paths_df['cellranger_type']=='multi'):
     tenx_metrics.append(parse_10x_cellranger_multi(all_paths_df[all_paths_df['cellranger_type']=='multi']))
 
 if any(all_paths_df['cellranger_type']=='count'):
     tenx_metrics.append(parse_10x_cellranger_count(all_paths_df[all_paths_df['cellranger_type']=='count'], convert_df))
 
-
-
 tenx_metrics_full = pd.concat(tenx_metrics)
 tenx_metrics_full = tenx_metrics_full.sort_values(['library_type', 'metric_name'])
+L.info("Done. Saving to '%s'" % args.output_file)
 tenx_metrics_full.to_csv(args.output_file, index=False)
-L.info('done')
 
 
 # tenx_metrics['metric_value'] = [re.sub(",|%", "", x) for x in tenx_metrics['metric_value']]
 # tenx_metrics['metric_value'] = tenx_metrics['metric_value'].astype(float)
 # split by library_type and metric_name 
+L.info("Plotting metrics for each library_type and metric_name")
 for idx, row in tenx_metrics_full[['library_type','metric_name']].drop_duplicates().iterrows():
     mn = row['metric_name']
     lt = row['library_type']
     plt_df = tenx_metrics_full[(tenx_metrics_full['library_type'] == lt) & (tenx_metrics_full['metric_name'] == mn)]  
     if len(plt_df.category.unique()) > 1:
         # if multiple categories i.e. Cells and Libraries, these are likely duplicate rows
         plt_df = plt_df[['sample_id', 'metric_name', 'library_type' , 'metric_value']].drop_duplicates()
     if len(plt_df['sample_id']) == len(plt_df['sample_id'].unique()):
+        L.info("Plotting barplot for library_type %s and metric_name %s" % (lt, mn))
         fig = sns.barplot(plt_df, x='sample_id', y='metric_value', color='grey')
         fig.set_xticklabels(fig.get_xticklabels(), rotation=90)
         fig.set_title(lt + ':' + mn)
         plt.savefig(os.path.join(args.figdir, lt + '-' + mn + '.png'), bbox_inches='tight')
     else:
         # do a boxplot instead
+        L.info("Plotting boxplot for library_type %s and metric_name %s" % (lt, mn))
         fig = sns.boxplot(plt_df, x='sample_id', y='metric_value', color='grey')
         fig.set_xticklabels(fig.get_xticklabels(), rotation=90)
         fig.set_title(lt + ':' + mn)
         plt.savefig(os.path.join(args.figdir, lt + '-' + mn + '.png'), bbox_inches='tight')
     plt.clf()
 
 
@@ -240,14 +242,15 @@
 plt_df = plt_df[['sample_id', 'metric_name', 'metric_value']]
 plt_tab = plt_df.pivot_table(index='sample_id', columns='metric_name', values='metric_value', aggfunc=sum)
 # sns.scatterplot(data=plt_tab, 
 #                 x='Sequencing saturation', 
 #                 y='Number of reads', size='Mean reads per cell',sizes=(20, 200))
 
 if 'Sequencing saturation' in plt_df.metric_name.unique(): 
+    L.info("Plotting scatter plot of sequencing saturation against number of reads")
     f, ax = plt.subplots()
     points = ax.scatter(x=plt_tab['Sequencing saturation'], 
                 y=plt_tab['Number of reads'], 
                 c=plt_tab['Estimated number of cells'])
     # define labels
     plt.xlabel('Sequencing saturation')
     plt.ylabel('Number of reads')
@@ -259,14 +262,15 @@
     plt.grid(axis='both', color='0.95')
     # save
     plt.savefig(os.path.join(args.figdir,'10x_sequencing_saturation_summary.png'))
     plt.clf()
 
 # plot 2 -  cells vs UMI counts per cell
 
+L.info("Plotting scatter plot of estimated number of cells against median UMI counts per cell")
 fig, ax = plt.subplots()
 x=list(np.log10(plt_tab['Estimated number of cells']))
 y=list(np.log10(plt_tab['Median UMI counts per cell']))
 ax.scatter(x=x, 
             y=y)
 # annotate each point
 for i, txt in enumerate(plt_tab.index):
@@ -285,8 +289,10 @@
            colors='black', linestyles='dotted'
 )
 
 # put it on a grid
 plt.grid(axis='both', color='0.95')
 # save
 plt.savefig(os.path.join(args.figdir,'10x_cells_by_UMIs.png'))
-plt.clf()
+plt.clf()
+
+L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/aggregate_csvs.py` & `panpipes-0.5.0/panpipes/python_scripts/aggregate_csvs.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import logging
 L = logging.getLogger()
 L.setLevel(logging.INFO)
 log_handler = logging.StreamHandler(sys.stdout)
 formatter = logging.Formatter('%(asctime)s: %(levelname)s - %(message)s')
 log_handler.setFormatter(formatter)
 L.addHandler(log_handler)
-L.debug("test logging message")
+
 
 # parse arguments
 parser = argparse.ArgumentParser()
 parser.add_argument('--input_files_str',
                     default='',
                     help='')
 parser.add_argument('--output_file',
@@ -28,29 +28,32 @@
                     help='')
 parser.add_argument('--clusters_or_markers',
                     default='',
                     help='')
 parser.set_defaults(verbose=True)
 args = parser.parse_args()
 
-L.info(args)
+L.info("Running with params: %s", args)
 
 infiles = re.split(',', args.input_files_str)
 if args.clusters_or_markers == "clusters":
+    L.info("Aggregating cluster columns")
     combined_csv = pd.concat([pd.read_csv(f, sep='\t', index_col=0) for f in infiles], axis=1)
     # get colnames
     cnames = []
     for f in infiles:
         alg = extract_parameter_from_fname(f, 'alg', prefix=args.sample_prefix)
         res = extract_parameter_from_fname(f, 'res', prefix=args.sample_prefix)
         cnames.append(alg + '_res_' + str(res))
+    L.info("Saving combined cluster columns to tsv file '%s'" % args.output_file)
     combined_csv.to_csv(args.output_file, sep='\t', header=cnames, index=True)
 
 
 if args.clusters_or_markers == "markers":
+    L.info("Aggregating marker files")
     li = []
     all_markers_file = re.sub("_top", "_all", args.output_file)
     excel_file = re.sub("_top.txt.gz", "_all.xlsx", args.output_file)
     excel_file_top = re.sub("_top.txt.gz", "_top.xlsx", args.output_file)
     with pd.ExcelWriter(excel_file) as writer:
         with pd.ExcelWriter(excel_file_top) as writer2:
             for ff in infiles:
@@ -65,12 +68,13 @@
                 df_sub = df[df['p.adj.bonferroni'] < 0.05]
                 df_sub = df_sub[df_sub['avg_logFC'] > 0]
                 df_sub.to_excel(writer2, sheet_name=sname, index=False)
     frame = pd.concat(li, axis=0, ignore_index=True)
     frame.to_csv(all_markers_file, sep='\t', header=True, index=False)
     frame_sub = frame[frame['p.adj.bonferroni'] < 0.05]
     frame_sub = frame_sub[frame_sub['avg_logFC'] > 0]
+    L.info("Saving combined marker files to tsv file '%s'" % args.output_file)
     frame_sub.to_csv(args.output_file, sep='\t', header=True, index=False)
 
 
 L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/assess_background.py` & `panpipes-0.5.0/panpipes/python_scripts/assess_background.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 import logging
 L = logging.getLogger()
 L.setLevel(logging.INFO)
 log_handler = logging.StreamHandler(sys.stdout)
 formatter = logging.Formatter('%(asctime)s: %(levelname)s - %(message)s')
 log_handler.setFormatter(formatter)
 L.addHandler(log_handler)
-L.debug("test logging message")
 # parse arguments
 parser = argparse.ArgumentParser()
 
 
 parser.add_argument('--channel_col',
                     default="sample_id",
                     help='')
@@ -37,39 +36,44 @@
                     help='')    
 parser.add_argument('--figpath',
                     default="./figures/background",
                     help='')  
 
 
 args, opt = parser.parse_known_args()
-L.info(args)
+L.info("Running with params: %s", args)
 
 sc.settings.figdir = args.figpath
 # load filtered data - if use_umon is True this will return a mudata object, else returns an mudata object
 
-L.info("reading filtered mudata object")
 try:
+    L.info("Reading in MuData from '%s'" % args.filtered_mudata)
     mdata = mu.read(args.filtered_mudata)
     # need to delete rep else we lose too many cells in intersect_obs later
     if "rep" in mdata.mod.keys():
+        L.info("Deleting modality 'rep' from MuData")
         del mdata.mod["rep"]
 except FileNotFoundError:
-    sys.exit("filtered mudata object not found")
+    L.error("MuData object with path '%s' could not be found" % args.filtered_mudata)
+    sys.exit("MuData object with path '%s' could not be found" % args.filtered_mudata)
 
 
 # mu.pp.intersect_obs(mdata)
 # load bg data
 
-L.info("reading bg mudata object")
+
 try:
+    L.info("Reading in bg MuData from '%s'" % args.bg_mudata)
     mdata_bg = mu.read(args.bg_mudata)
 except FileNotFoundError:
-    sys.exit("bg_mudata object not found")
+    L.error("bg_mudata object with path '%s' could not be found" % args.bg_mudata)
+    sys.exit("bg_mudata object with path '%s' could not be found" % args.bg_mudata)
 
 # barcode rank plots
+L.info("Plotting barcode ranks")
 df = mdata_bg['rna'].obs.copy()
 df['total_counts'] = np.ravel(mdata_bg['rna'].X.sum(axis=1))
 df['log_total_counts'] = np.log(df['total_counts'])
 df['ranks'] = df.groupby('sample_id', as_index=False)['total_counts'].transform(lambda x: rankdata(x*-1, method="ordinal"))
 df['log_ranks'] = np.log(df['ranks'])
 df['is_cell'] = df.index.isin(mdata['rna'].obs_names.tolist())
 df['is_cell'] = df['is_cell'].astype('category')
@@ -102,20 +106,22 @@
 
 # mdata_bg.update()
 # mu.pp.intersect_obs(mdata_bg)
 
 # calculate qc metrics
 if 'rna' in mdata.mod.keys():
     # run stadard qc metrics
+    L.info("Computing standard QC metrics for RNA")
     sc.pp.calculate_qc_metrics(mdata['rna'], inplace=True, percent_top=None, log1p=True)
     sc.pp.calculate_qc_metrics(mdata_bg['rna'], inplace=True, percent_top=None, log1p=True)
 
 
 
 if 'prot' in mdata.mod.keys():
+    L.info("Computing standard QC metrics for prot")
     sc.pp.calculate_qc_metrics(mdata['prot'], inplace=True, percent_top=None, log1p=True)
     sc.pp.calculate_qc_metrics(mdata_bg['prot'], inplace=True, percent_top=None, log1p=True)
 
 
 mdata.update()
 mdata_bg.update()
 
@@ -125,14 +131,15 @@
     n_samples_prot=len(mdata['prot'].obs['sample_id'].unique())
 
 # quantifying the top background features
 if os.path.exists(args.figpath) is False:
     os.mkdirs(args.figpath)
 
 if 'rna' in mdata.mod.keys():
+    L.info("Quantifying the top background features for RNA")
     sc.pl.highest_expr_genes(mdata_bg['rna'],n_top=30, save="_rna_background.png")
     top_genes = pnp.scmethods.get_top_expressed_features(mdata_bg['rna'], n_top=30, group_by=args.channel_col)
     bg_df = pnp.scmethods.get_mean_background_fraction(mdata_bg['rna'], top_background=top_genes, group_by=args.channel_col)
     if bg_df.shape[0] >1:
         fig, ax= plt.subplots(figsize=(12,8))
         sns.heatmap(bg_df, ax=ax)
         fig.tight_layout()
@@ -146,14 +153,15 @@
         plt.savefig(os.path.join(args.figpath,"barplot_background_" + args.channel_col + "_rna_top_expressed.png"))
 
 
 # quantifying the top background features
 ## Repeat for protein (if it exists)
 if 'prot' in mdata.mod.keys():
     # this time we'll just use all the prot vars.
+    L.info("Quantifying the top background features for prot")
     top_genes = list(mdata_bg['prot'].var_names)
     bg_df = pnp.scmethods.get_mean_background_fraction(mdata_bg['prot'], top_background=top_genes, group_by=args.channel_col)
     if bg_df.shape[0] >1:
         if len(top_genes) > 50:
             # split the plot into two
             split_int = int(np.ceil(137/2))
             fig, ax = plt.subplots(nrows=2,ncols=1,figsize=(24,10), facecolor="white")
@@ -184,30 +192,32 @@
             fig.tight_layout()
         plt.savefig(os.path.join(args.figpath,"barplot_background_" + args.channel_col + "_prot_top_expressed.png"))
 
 
 ## QC for rna and protein comparing foreground and background
 
 if 'rna' in mdata.mod.keys():
+    L.info("Comparing foreground and background for RNA")
     pnp.pl.scatter_fg_vs_bg(mdata, mdata_bg,x="rna:log1p_n_genes_by_counts", y="rna:log1p_total_counts", facet_row=args.channel_col)
     plt.subplots_adjust(right=0.7)
     plt.savefig(os.path.join(args.figpath,"scatter_bg_fg_rna_nGene_rna_nUMI.png"),transparent=False)
     if 'prot' in mdata.mod.keys():
+        L.info("Comparing foreground and background for RNA and prot")
         if n_samples_rna != n_samples_prot:
-            L.info("n_samples are not equal in rna and prot,taking intrsect for mdata and mdata_bg")
+            L.warning("n_samples are not equal in rna and prot,taking intersect for mdata and mdata_bg")
             mu.pp.intersect_obs(mdata_bg)
             mu.pp.intersect_obs(mdata)
             pnp.pl.scatter_fg_vs_bg(mdata, mdata_bg,x="prot:log1p_total_counts", y="rna:log1p_n_genes_by_counts", facet_row=args.channel_col)
             plt.subplots_adjust(right=0.7)
             plt.savefig(os.path.join(args.figpath, "scatter_bg_fg_prot_nUMI_rna_nGene.png"),transparent=False)
             pnp.pl.scatter_fg_vs_bg(mdata, mdata_bg,x="rna:log1p_total_counts", y="prot:log1p_total_counts", facet_row=args.channel_col)
             plt.subplots_adjust(right=0.7)
             plt.savefig(os.path.join(args.figpath,"scatter_bg_fg_rna_nUMI_prot_nUMI.png"),transparent=False)
         else:
-            L.info("n_samples are equal in rna and prot")
+            L.info("n_samples are equal in RNA and prot")
             pnp.pl.scatter_fg_vs_bg(mdata, mdata_bg,x="prot:log1p_total_counts", y="rna:log1p_n_genes_by_counts", facet_row=args.channel_col)
             plt.subplots_adjust(right=0.7)
             plt.savefig(os.path.join(args.figpath, "scatter_bg_fg_prot_nUMI_rna_nGene.png"),transparent=False)
             pnp.pl.scatter_fg_vs_bg(mdata, mdata_bg,x="rna:log1p_total_counts", y="prot:log1p_total_counts", facet_row=args.channel_col)
             plt.subplots_adjust(right=0.7)
             plt.savefig(os.path.join(args.figpath,"scatter_bg_fg_rna_nUMI_prot_nUMI.png"),transparent=False)
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/batch_correct_bbknn.py` & `panpipes-0.5.0/panpipes/python_scripts/batch_correct_bbknn.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,78 +40,85 @@
 parser.add_argument('--modality', default='',
                     help='which mod to run bbknn on')
 
 
 args, opt = parser.parse_known_args()
 
 
+L.info("Running with params: %s", args)
 
-L.info("reading data and starting integration pipeline with script: ")
-L.info(os.path.basename(__file__))
-L.info("Running with options: %s", args)
 
 #adata = read_anndata(args.input_anndata, use_muon=use_muon, modality="rna")
+L.info("Reading in MuData from '%s'" % args.input_anndata)
 mdata = mu.read(args.input_anndata)
 adata = mdata.mod[args.modality] 
-L.info("read files")
+
 nnb = int(args.neighbors_within_batch)
 # bbknn can't integrate on 2+ variables, so create a fake column with combined information
 columns = [x.strip() for x in args.integration_col.split(",")]
 
 if args.modality =="atac":
     if "scaled_counts" in adata.layers.keys():
         pass
     else:
-        L.info("to run BBKNN on atac we need to compute PCA. Computing on the flight now")
+        L.info("To run BBKNN on ATAC, PCA is needed. Computing PCA now.")
+        L.info("Scaling data and saving scaled counts to .layers['scaled_counts']")
         sc.pp.scale(adata)
         adata.layers["scaled_counts"] = adata.X.copy()
+        L.info("Computing PCA")
         sc.tl.pca(adata, n_comps=min(50,adata.var.shape[0]-1), svd_solver='arpack', random_state=0) 
 
 if "X_pca" not in adata.obsm:
-    L.info("i need a dimred to start, computing pca with default param")
+    L.warning("X_pca could not be found in adata.obsm. Computing PCA with default parameters.")
     n_pcs = 50
     if adata.var.shape[0] < n_pcs:
         L.info("You have less features than number of PCs you intend to calculate")
         n_pcs = adata.var.shape[0] - 1
-        L.info("Setting n PCS to %i" % int(n_pcs))    
+        L.info("Setting n PCS to %i" % int(n_pcs))   
+    L.info("Scaling data") 
     sc.pp.scale(adata)
+    L.info("Computing PCA")
     sc.tl.pca(adata, n_comps=n_pcs, 
                     svd_solver='arpack', 
                     random_state=0) 
 
 
-L.info("preparing for integration")
+L.info("Preparing for integration")
+
 if len(columns) > 1:
-    L.info("using 2 columns to integrate on more variables")
+    L.info("Using 2 columns to integrate on more variables.")
     # comb_columns = "_".join(columns)
     adata.obs["comb_columns"] = adata.obs[columns].apply(lambda x: '|'.join(x), axis=1)
 
     # make sure that batch is a categorical
     adata.obs["comb_columns"] = adata.obs["comb_columns"].astype("category")
     # run bbknn
+    L.info("Running BBKNN")
     adata = sc.external.pp.bbknn(adata, batch_key="comb_columns", copy=True, neighbors_within_batch=nnb)
 else:
     adata.obs[args.integration_col] = adata.obs[args.integration_col].astype("category")
     # run bbknn
+    L.info("Running BBKNN")
     adata = sc.external.pp.bbknn(adata,
                         batch_key=args.integration_col,
                         copy=True,
                         n_pcs = int(args.neighbors_n_pcs),
                         neighbors_within_batch=nnb)  # calculates the neighbours
 
-L.info("integration run now calculate umap")
+L.info("Computing UMAP")
 sc.tl.umap(adata)
-L.info("done umap, saving stuff")
+
 # write out
+L.info("Saving UMAP coordinates to csv file '%s" % args.output_csv)
 umap = pd.DataFrame(adata.obsm['X_umap'], adata.obs.index)
 umap.to_csv(args.output_csv)
 
 
 
 # save full bbknn anndata in tmp, cause need more than just neighbors to work 
 outfiletmp = ("tmp/bbknn_scaled_adata_" + args.modality + ".h5ad" )
 
-L.info("saving bbknn corrected adata")
+L.info("Saving AnnData to '%s'" % outfiletmp)
 write_anndata(adata, outfiletmp, use_muon=False, modality=args.modality)
 
 L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/batch_correct_combat.py` & `panpipes-0.5.0/panpipes/python_scripts/batch_correct_combat.py`

 * *Files 22% similar despite different names*

```diff
@@ -41,60 +41,63 @@
                     help="neighbor metric, e.g. euclidean or cosine")
 parser.add_argument('--modality',
                     help="")
 
 
 args, opt = parser.parse_known_args()
 
+L.info("Running with params: %s", args)
 
-
-L.info("reading data and starting integration pipeline with script: ")
-L.info(os.path.basename(__file__))
-L.info("Running with options: %s", args)
-L.info("threads available: %s", threads_available)
 # this should be an object that contains the full log normalised data (adata_log1p.h5ad)
 # prior to hvgs and filtering
 #adata = read_anndata(args.input_anndata, use_muon=use_muon, modality="rna")
+L.info("Reading in MuData from '%s'" % args.input_anndata)
 mdata = mu.read(args.input_anndata)
 adata = mdata.mod[args.modality] 
 
 # combat can't integrate on 2+ variables, so create a fake column with combined information
 columns = [x.strip() for x in args.integration_col.split(",")]
 if len(columns) > 1: 
-    L.info("using 2 columns to integrate on more variables")
+    L.info("Using 2 columns to integrate on more variables")
     #comb_columns = "_".join(columns)
     adata.obs["comb_columns"] = adata.obs[columns].apply(lambda x: '|'.join(x), axis=1)
 
     # make sure that batch is a categorical
     adata.obs["comb_columns"] = adata.obs["comb_columns"].astype("category")
     # run combat
+    L.info("Running combat")
     sc.pp.combat(adata, key="comb_columns")
     
 else:
-
     # run combat
+    L.info("Running combat")
     sc.pp.combat(adata, key=args.integration_col)
 
-L.info("integration run now calculate umap")
+L.info("Computing PCA")
 sc.pp.pca(adata, use_highly_variable=True, svd_solver='arpack') #use same args as plot_pca.py
 
-# run neighbours and umap 
+# run neighbours and umap
+L.info("Computing neighbors") 
 run_neighbors_method_choice(adata, 
     method=args.neighbors_method, 
     n_neighbors=int(args.neighbors_k), 
     n_pcs=int(args.neighbors_n_pcs), 
     metric=args.neighbors_metric, 
     use_rep='X_pca',
     nthreads=max([threads_available, 6]))
 
 
+L.info("Computing UMAP")
 sc.tl.umap(adata)
-L.info("done umap, saving stuff")
+
 #write out
+L.info("Saving UMAP coordinates to csv file '%s" % args.output_csv)
 umap = pd.DataFrame(adata.obsm['X_umap'], adata.obs.index)
 umap.to_csv(args.output_csv)
 
+outfiletmp = "tmp/combat_scaled_adata_" + args.modality + ".h5ad"
+L.info("Saving AnnData to '%s'" % outfiletmp)
 adata.write("tmp/combat_scaled_adata_" + args.modality + ".h5ad")
 
 
 L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/batch_correct_harmony.py` & `panpipes-0.5.0/panpipes/python_scripts/batch_correct_harmony.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,108 +52,107 @@
                     help="neighbors k")
 parser.add_argument('--neighbors_metric',
                     help="neighbor metric, e.g. euclidean or cosine")
 
 
 args, opt = parser.parse_known_args()
 
-
-L.info("reading data and starting integration pipeline with script: ")
-L.info(os.path.basename(__file__))
-L.info("Running with options: %s", args)
+L.info("Running with params: %s", args)
 
 # this should be an object that contains the full log normalised data (adata_log1p.h5ad)
 # prior to hvgs and filtering
 #adata = read_anndata(args.input_anndata, use_muon=use_muon, modality=args.modality)
+L.info("Reading in MuData from '%s'" % args.input_anndata)
 mdata = mu.read(args.input_anndata)
 adata = mdata.mod[args.modality] 
 
 # Harmony can integrate on 2+ variables,
 # but for consistency with other approaches create a fake column with combined information
 columns = [x.strip() for x in args.integration_col.split(",")]
 if args.dimred == "PCA":
     dimred = "X_pca"
 elif args.dimred == "LSI":
     dimred = "X_lsi"
 
 if dimred not in adata.obsm:
-    L.info("i need a dimred to start, computing pca with default param")
+    L.warning("Dimred '%s' could not be found in adata.obsm. Computing PCA with default parameters." % dimred)
     dimred = "X_pca" 
     n_pcs = 50
     if adata.var.shape[0] < n_pcs:
         L.info("You have less features than number of PCs you intend to calculate")
         n_pcs = adata.var.shape[0] - 1
-        L.info("Setting n PCS to %i" % int(n_pcs))    
+        L.info("Setting n PCS to %i" % int(n_pcs)) 
+    L.info("Scaling data")   
     sc.pp.scale(adata)
+    L.info("Computing PCA")
     sc.tl.pca(adata, n_comps=n_pcs, 
                     svd_solver='arpack', 
                     random_state=0) 
 
 
 
 if len(columns)>1: 
-    L.info("using 2 columns to integrate on more variables")
+    L.info("Using 2 columns to integrate on more variables")
     #comb_columns = "_".join(columns)
     adata.obs["comb_columns"] = adata.obs[columns].apply(lambda x: '|'.join(x), axis=1)
 
     # make sure that batch is a categorical
     adata.obs["comb_columns"] = adata.obs["comb_columns"].astype("category")
     # run harmony
-
+    L.info("Running Harmony")
     ho = hm.run_harmony(adata.obsm[dimred][:,0:int(args.harmony_npcs)], adata.obs, ["comb_columns"], 
                                        sigma = float(args.sigma_val),theta = float(args.theta_val),verbose=True,max_iter_kmeans=30, 
                                        max_iter_harmony=40)
 
 else:
     # make sure that batch is a categorical
     adata.obs[args.integration_col] = adata.obs[args.integration_col].astype("category")
     # run harmony
+    L.info("Running Harmony")
     ho = hm.run_harmony(adata.obsm[dimred][:,0:int(args.harmony_npcs)],
                         adata.obs,
                         [args.integration_col],
                         sigma=float(args.sigma_val),
                         theta = float(args.theta_val),
                         verbose=True,max_iter_kmeans=30,
                         max_iter_harmony=40)
 
 
-L.info("integration run now calculate umap")
-
+L.info("Saving harmony co-ords to .obsm['X_harmony']")
 adjusted_pcs = pd.DataFrame(ho.Z_corr).T
 adata.obsm['X_harmony']=adjusted_pcs.values
-L.info("harmony co-ords derived")
 
 if int(args.neighbors_n_pcs) >adata.obsm['X_harmony'].shape[1]:
     L.warn(f"N PCs is larger than X_harmony dimensions, reducing n PCs to  {adata.obsm['X_harmony'].shape[1] -1}")
 
 n_pcs= min(int(args.neighbors_n_pcs), adata.obsm['X_harmony'].shape[1]-1)
 
 # run neighbours and umap 
+L.info("Computing neighbors")
 run_neighbors_method_choice(adata, 
     method=args.neighbors_method, 
     n_neighbors=int(args.neighbors_k), 
     n_pcs=n_pcs, 
     metric=args.neighbors_metric, 
     use_rep='X_harmony',
     nthreads=max([threads_available, 6]))
 
 
-L.info("done n_neighbours, moving to umap")
+L.info("Computing UMAP")
 sc.tl.umap(adata)
-L.info("done umap, saving stuff")
+
 # write out
+L.info("Saving UMAP coordinates to csv file '%s" % args.output_csv)
 umap = pd.DataFrame(adata.obsm['X_umap'], adata.obs.index)
 umap.to_csv(args.output_csv)
 
 
 #adata.write("tmp/harmony_scaled_adata_" + args.modality + ".h5ad")
 
 
 outfiletmp = ("tmp/harmony_scaled_adata_" + args.modality + ".h5ad" )
-
-L.info("saving harmony corrected adata")
+L.info("Saving AnnData to '%s'" % outfiletmp)
 write_anndata(adata, outfiletmp, use_muon=False, modality=args.modality)
 
-
 L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/batch_correct_merge.py` & `panpipes-0.5.0/panpipes/python_scripts/batch_correct_merge.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 parser.add_argument('--multimodal_correction_choice', default=None,
                     help='')
 
 
 args, opt = parser.parse_known_args()
 
 
-L.info(args)
+L.info("Running with params: %s", args)
 
 base_object = args.preprocessed_mudata
 
 multi_mod = args.multimodal_correction_choice
 if multi_mod is not None:
     base_object = "tmp/" + multi_mod.lower() + "_scaled_adata.h5mu"
 
@@ -49,36 +49,38 @@
     uni_mod_paths['rna']= "tmp/" + args.rna_correction_choice + "_scaled_adata_rna.h5ad"
 if args.prot_correction_choice is not None:
     uni_mod_paths['prot']= "tmp/" + args.prot_correction_choice + "_scaled_adata_prot.h5ad"
 if args.atac_correction_choice is not None:
     uni_mod_paths['atac'] = "tmp/" + args.atac_correction_choice + "_scaled_adata_atac.h5ad"
 uni_mod_paths
 
+L.info("Reading in data from '%s'" % base_object)
 base_obj = mu.read(base_object)
 
 
 if multi_mod=="totalvi":
     totalvi_extra_obsm = {'prot': ['totalvi_protein_foreground_prob', 'totalvi_denoised_protein'], 'rna': [ 'totalvi_denoised_rna']}
     # we will want to keep these so extract them first
     totalvi_extra_obsm_keep = {}
     for k, v in totalvi_extra_obsm.items():
         print(k,v)
         totalvi_extra_obsm_keep[k] = {w:base_obj[k].obsm[w] for w in v}
 
 
 # this overwrites the old modalities
 for k,v in uni_mod_paths.items():
+    L.info("Reading in data from '%s'" % v)
     mod_replace = mu.read(v)
     if mod_replace.shape[1] == base_obj[k].shape[1]:
-        L.info('replacing the whole anndata object with batch corrected')
+        L.info('Replacing the whole anndata object with batch corrected')
         base_obj.mod[k] = mod_replace
     else:
         # in this situation the vars in the mod has been subset but the 
         # original object contains all the genes.
-        L.info("number of genes does not match base object, only integrating obsp and obsm into full mdata[%s] object" % k)
+        L.info("Number of genes does not match base object, only integrating obsp and obsm into full mdata[%s] object" % k)
         base_obj.mod[k].obsm = mod_replace.obsm
         base_obj.mod[k].obsp = mod_replace.obsp
         base_obj.mod[k].uns = mod_replace.uns
         base_obj.mod[k].uns['batch_correct_gene_subset'] = mod_replace.var_names.tolist()
         # merge any extra obs columns
         new_obs = mod_replace.obs.iloc[:, ~ mod_replace.obs.columns.isin( base_obj.mod[k].obs.columns)]
         base_obj.mod[k].obs = base_obj.mod[k].obs.merge(new_obs, left_index=True, right_index=True)
@@ -86,11 +88,12 @@
 if multi_mod=="totalvi":
     # restore the totalvi extras
     for k, v in totalvi_extra_obsm_keep.items():
         for w in v:
             base_obj[k].obsm[ w] = totalvi_extra_obsm_keep[k][w]
 
 base_obj.update()
+L.info("Writing MuData to '%s'" % args.output_mudata)
 base_obj.write(args.output_mudata)
 
 L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/batch_correct_mofa.py` & `panpipes-0.5.0/panpipes/python_scripts/batch_correct_mofa.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,50 +52,51 @@
 parser.add_argument('--neighbors_k', default=30,
                     help="neighbors k")
 parser.add_argument('--neighbors_metric',default="euclidean",
                     help="neighbor metric, e.g. euclidean or cosine")
 
 args, opt = parser.parse_known_args()
 
-L.info(args)
+L.info("Running with params: %s", args)
 # scanpy settings
 sc.set_figure_params(facecolor="white")
 sc.settings.autoshow = False
 sc.settings.figdir = args.figdir
 
 
 # load parameters
 
 threads_available = multiprocessing.cpu_count()
 params = pp.io.read_yaml("pipeline.yml")
 
+L.info("Reading in MuData from '%s'" % args.scaled_anndata)
 mdata = mu.read(args.scaled_anndata)
 
 if params['multimodal']['mofa']['modalities'] is not None:
     modalities= params['multimodal']['mofa']['modalities']
     modalities = [x.strip() for x in modalities.split(",")]
-    L.info(f"using modalities :{modalities}")
+    L.info(f"Using modalities :{modalities}")
     removed_mods = None
     if all(x in modalities for x in mdata.mod.keys()):
         tmp = mdata.copy()
-        L.info('using all modalities')
+        L.info('Using all modalities')
     else:
         tmp = mdata.copy()
         removed_mods = list(set(mdata.mod.keys()) - set(modalities))
-        L.info(f"removing modalities {removed_mods}")
+        L.info(f"Removing modalities {removed_mods}")
         for rmod in removed_mods:
             del tmp.mod[rmod]
 else:
-    L.warning("""you specified no modalities, so i will default to all available
-                this may be a problem if you have repertoire in here""")
+    L.warning("""No modalities were specified, therefore all available modalities will be used.
+                This may be problematic if repertoire is present as modality.""")
     removed_mods = None
     tmp = mdata.copy()  
 
-print(tmp.mod.keys())
 
+L.info("Intersecting modality obs before running mofa")
 mu.pp.intersect_obs(tmp)
 
 mofa_kwargs={}
 #expected args:
 # n_factors: 10
 # n_iterations: 1000
 # convergence_mode: fast, medium, slow
@@ -107,15 +108,14 @@
 del mofa_kwargs['modalities']
 
 if mofa_kwargs['filter_by_hvg']:
     mofa_kwargs['use_var'] = "highly_variable"
     del mofa_kwargs['filter_by_hvg']
     for mod in tmp.mod.keys():
         if "highly_variable" not in tmp[mod].var.columns:
-            print(mod)
             tmp[mod].var["highly_variable"] = True
         
     tmp.update()
     
 
 
 if args.integration_col_categorical is not None:
@@ -144,44 +144,46 @@
     if args.convergence_mode is not None:
         mofa_kwargs['convergence_mode'] = args.convergence_mode
         
 # are we using the gpu?
 if args.use_gpu is True or args.use_gpu=='True':
      mofa_kwargs['gpu_mode'] = True
 
-L.info(mofa_kwargs)
-L.info(tmp.var.columns)
-
 
+L.info("Running mofa")
 mu.tl.mofa(tmp, **mofa_kwargs)
 #This adds X_mofa embeddings to the .obsm slot of the MuData object
 #write the discovered latent rep to the original mudata object
+L.info("Adding X_mofa to .obsm of MuData")
 mdata.obsm['X_mofa'] = tmp.obsm['X_mofa'].copy()   
 
 if int(args.neighbors_n_pcs) > mdata.obsm['X_mofa'].shape[1]:
     L.warning(f"N PCs is larger than X_mofa dimensions, reducing n PCs to  {mdata.obsm['X_mofa'].shape[1]-1}")
 n_pcs= min(int(args.neighbors_n_pcs), mdata.obsm['X_mofa'].shape[1]-1)
 
-
+L.info("Computing neighbors")
 run_neighbors_method_choice(mdata, 
     method=args.neighbors_method, 
     n_neighbors=int(args.neighbors_k), 
     n_pcs=n_pcs, #this should be the # rows of var, not obs ???????
     metric=args.neighbors_metric, 
     use_rep='X_mofa',
     nthreads=max([threads_available, 6]))
 
+L.info("Computing UMAP")
 sc.tl.umap(mdata, min_dist=0.4)
+L.info("Computing Leiden clustering")
 sc.tl.leiden(mdata,  key_added="leiden_mofa")
 
+L.info("Saving UMAP coordinates to csv file '%s" % args.output_csv)
 umap = pd.DataFrame(mdata.obsm['X_umap'], mdata.obs.index)
 umap.to_csv(args.output_csv)
 
 if removed_mods is not None:
     for rmd in removed_mods:
         tmp.mod[rmd] = mdata.mod[rmd].copy()
 
+L.info("Saving MuData to 'tmp/mofa_scaled_adata.h5mu'")
 tmp.write("tmp/mofa_scaled_adata.h5mu")
 
-
 L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/batch_correct_multivi.py` & `panpipes-0.5.0/panpipes/python_scripts/batch_correct_multivi.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,145 +42,159 @@
                     help="n_pcs", default=50)
 parser.add_argument('--neighbors_method', default="scanpy",
                     help="neighbours method, scanpy or hnsw")
 parser.add_argument('--neighbors_k', default=30,
                     help="neighbors k")
 parser.add_argument('--neighbors_metric',default="euclidean",
                     help="neighbor metric, e.g. euclidean or cosine")
+parser.add_argument('--scvi_seed',default=None,
+                    help="set explicitly seed to make runs reproducible")
 
 
 
 
 args, opt = parser.parse_known_args()
+L.info("Running with params: %s", args)
 
 # scanpy settings
 sc.set_figure_params(facecolor="white")
 sc.settings.autoshow = False
 sc.settings.figdir = args.figdir
 
-
+if args.scvi_seed is not None:
+    scvi.settings.seed = int(args.scvi_seed)
+else:
+    scvi.settings.seed = 1492
 # load parameters
 
 threads_available = multiprocessing.cpu_count()
 params = pp.io.read_yaml("pipeline.yml")
 
 test_script=False
 if test_script:
     L.info("this is a test run")
     params['MultiVI']['training_args']['max_epochs'] = 10
 
 # ------------------------------------------------------------------
-L.info("Running multivi")
-
-# mdata = mu.read(args.scaled_anndata)
-# rna = mdata['rna'].copy()
-# atac = mdata['atac'].copy()
-rna= mu.read(args.scaled_anndata +"/" + "rna")
-atac= mu.read(args.scaled_anndata +"/" + "atac")
+L.info("Reading in MuData from '%s'" % args.scaled_anndata)
+mdata = mu.read(args.scaled_anndata)
+rna = mdata['rna'].copy()
+atac = mdata['atac'].copy()
 
+del mdata
 
 if check_for_bool(params["multimodal"]["MultiVI"]["lowmem"]):
-    L.info("subsetting atac to top 25k HVF")
+    if 'hvg' in atac.uns.keys():
+        L.info("Subsetting ATAC to HVFs")
+        atac = atac[:, atac.var.highly_variable].copy()
+    L.info("Calculating and subsetting ATAC to top 25k HVF")
     sc.pp.highly_variable_genes(atac, n_top_genes=25000)
-    atac = atac[:, atac.var.highly_variable]
+    atac = atac[:, atac.var.highly_variable].copy()
 
 
 
 gc.collect()
 
 # if "modality" not in atac.var.keys():
 #     atac.var["modality"] = "Peaks"
 
 # if "modality" not in rna.var.keys():
 #     rna.var["modality"] = "Gene Expression"
 
 if rna.shape[0] == atac.shape[0]:
     n=int(rna.shape[0])
 else:
-    sys.exit("rna and atac have different number of cells, \
-        can't deal with this in this version of MultiVI integration")
+    sys.exit("RNA and ATAC have different number of cells, \
+        Can't deal with this in this version of MultiVI integration")
 
 gc.collect()
 
 n_genes = len(rna.var_names)
 n_regions = len(atac.var_names)
 
 
 if "raw_counts" in rna.layers.keys():
-    L.info("raw counts found in layer for RNA")
+    L.info("Found raw RNA counts in .layers['raw_counts']")
 elif X_is_raw(rna):
     # this means the X layer is already raw and we can make the layer we need
-    L.info("raw counts found in X for RNA")
+    L.info("Found raw RNA counts in .X. Saving raw RNA counts to .layers['raw_counts']")
     rna.layers["raw_counts"] = rna.X.copy()
 else:
-    sys.exit("please provide a mu/anndata with raw counts for RNA")
+    L.error("Could not find raw counts for RNA in .X and .layers['raw_counts']")
+    sys.exit("Could not find raw counts for RNA in .X and .layers['raw_counts']")
+
 
 if "raw_counts" in atac.layers.keys():
-    L.info("raw counts found in layer for ATAC")
+     L.info("Found raw ATAC counts in .layers['raw_counts']")
 elif X_is_raw(atac):
     # this means the X layer is already raw and we can make the layer we need
-    L.info("raw counts found in X for ATAC")
+    L.info("Found raw ATAC counts in .X. Saving raw ATAC counts to .layers['raw_counts']")
     atac.layers["raw_counts"] = atac.X.copy()
 else:
-    sys.exit("please provide a mu/anndata with raw counts for ATAC")
+    L.error("Could not find raw counts for ATAC in .X and .layers['raw_counts']")
+    sys.exit("Could not find raw counts for ATAC in .X and .layers['raw_counts']")
 
-L.info("concatenating modalities to comply with multiVI")
+L.info("Concatenating modalities to comply with multiVI")
 # adata_paired = ad.concat([rna, atac], join="outer")
 # adata_paired.var = pd.concat([rna.var,atac.var])
-
+if rna.is_view:
+    L.info("RNA is view")
+    rna = rna.copy()
+if atac.is_view:
+    L.info("ATAC is view")
+    atac = atac.copy()
 adata_paired = ad.concat([rna.T, atac.T]).T
 
 rna_cols=rna.obs.columns
 atac_cols=atac.obs.columns
 
 rnaobs = rna.obs.copy()
 rnaobs.columns= ["rna:"+ x for x in rna_cols]
 atacobs = atac.obs.copy()
 atacobs.columns= ["atac:"+ x for x in atac_cols]
 adata_paired.obs = pd.merge(rnaobs, atacobs, left_index=True, right_index=True)
 
 if "modality" not in adata_paired.obs.columns:
     adata_paired.obs["modality"] = "paired" 
 
-print(adata_paired)
 
 # adata = ad.concat([rna,atac],join="outer")
 # adata.var = pd.concat([rna.var,atac.var])
 
 del [rna , atac ]
 gc.collect()
 
+
+L.info("Organizing multiome AnnDatas")
 adata_mvi = scvi.data.organize_multiome_anndatas(adata_paired)
 
 
 # MultiVI integrates by modality, to use batch correction you need a batch covariate to specify in
 # categorical_covariate_keys
 if args.integration_col_categorical is not None :
     cols = [x.strip() for x in args.integration_col_categorical.split(",")]
     columns = []
     for cc in cols:
         if cc in rna_cols:
-            print("categorical batch covariate in rna")
             columns.append("rna:"+cc)
         elif cc in atac_cols:
-            print("categorical batch covariate in atac")
             columns.append("atac:"+cc)
 if args.integration_col_continuous is not None :
     if args.integration_col_continuous in rna_cols:
         args.integration_col_continuous = "rna:"+ args.integration_col_continuous
     elif args.integration_col_continuous in atac_cols:
         args.integration_col_continuous = "atac:"+ args.integration_col_continuous
 
 
 kwargs = {}
 # in case of more than 1 variable, create a fake column with combined information
 if columns is not None:
     print(columns)
     if len(columns) > 1:
-        L.info("using 2 columns to integrate on more variables")
+        L.info("Using 2 columns to integrate on more variables")
         # bc_batch = "_".join(columns)
         adata_mvi.obs["bc_batch"] = adata_mvi.obs[columns].apply(lambda x: '|'.join(x), axis=1) 
         # make sure that batch is a categorical
         adata_mvi.obs["bc_batch"] = adata_mvi.obs["bc_batch"].astype("category")
     else:
         adata_mvi.obs['bc_batch'] = adata_mvi.obs[columns]
         adata_mvi.obs["bc_batch"] = adata_mvi.obs["bc_batch"].astype("category")
@@ -189,61 +203,58 @@
     kwargs['categorical_covariate_keys'] = ["bc_batch"]
 
 if args.integration_col_continuous is not None :
     print(args.integration_col_continuous)
     adata_mvi.obs['bc_batch_continuous'] = adata_mvi.obs[args.integration_col_continuous]
     kwargs['continuous_covariate_keys'] = ["bc_batch_continuous"]
 
-print(kwargs)
 
 # 1 setup anndata
 #scvi.model.MULTIVI.setup_anndata(adata_mvi, batch_key='modality', **kwargs)
+L.info("Setting up AnnData")
 scvi.model.MULTIVI.setup_anndata(
     adata_mvi, 
     batch_key='modality',
     layer =  "raw_counts",
     **kwargs) 
 #2. setup model
 if params["multimodal"]['MultiVI']['model_args'] is None:
     multivi_model_args =  {}
 else:
     multivi_model_args =  {k: v for k, v in params["multimodal"]['MultiVI']['model_args'].items() if v is not None}
 
-print(multivi_model_args)
-
+L.info("Defining model")
 mvi = scvi.model.MULTIVI(
     adata_mvi,
     n_genes=n_genes,
     n_regions=n_regions,
     **multivi_model_args
 )
 
 #3.train
 
 if params["multimodal"]["MultiVI"]["training_args"] is None:
     multivi_training_args={}
 else:
     multivi_training_args =  {k: v for k, v in params["multimodal"]['MultiVI']['training_args'].items() if v is not None}
 
-print(multivi_training_args)
-
 if params["multimodal"]['MultiVI']['training_plan'] is None:
     multivi_training_plan = {}
 else:
     multivi_training_plan =  {k: v for k, v in params["multimodal"]['MultiVI']['training_plan'].items() if v is not None}
 
-print(multivi_training_plan)
-
 mvi.view_anndata_setup()
 
+L.info("Running multiVI")
 mvi.train( **multivi_training_args, **multivi_training_plan)
 
 mvi.save(os.path.join("batch_correction", "multivi_model"), 
                   anndata=False)
 
+L.info("Plotting ELBO")
 plt.plot(mvi.history["elbo_train"], label="train")
 plt.plot(mvi.history["elbo_validation"], label="validation")
 plt.title("Negative ELBO over training epochs")
 
 plt.legend()
 plt.savefig(os.path.join(args.figdir, "multivi_elbo_plot.png"))
 
@@ -252,31 +263,37 @@
         you would find in scvitools tutorial.
         We chose to save the learned SC representation in the 
         Mudata obsm slot, and any single modality processing in
         its own modality slot
             """)
 
 mdata = mu.read(args.scaled_anndata)
+L.info("Extracting latent space and saving latent to X_MultiVI")
 mdata.obsm["X_MultiVI"] = mvi.get_latent_representation()
 #adata_mvi.obsm["X_MultiVI"] = mvi.get_latent_representation()
 
 if int(args.neighbors_n_pcs) > mdata.obsm['X_MultiVI'].shape[1]:
     L.warn(f"N PCs is larger than X_MultiVI dimensions, reducing n PCs to  {mdata.obsm['X_MultiVI'].shape[1] -1}")
 n_pcs= min(int(args.neighbors_n_pcs), mdata.obsm['X_MultiVI'].shape[1]-1)
 
+L.info("Computing neighbors")
 run_neighbors_method_choice(mdata, 
     method=args.neighbors_method, 
     n_neighbors=int(args.neighbors_k), 
     n_pcs=n_pcs, 
     metric=args.neighbors_metric, 
     use_rep='X_MultiVI',
     nthreads=max([threads_available, 6]))
+L.info("Computing UMAP")
 sc.tl.umap(mdata, min_dist=0.4)
+L.info("Computing Leiden clustering")
 sc.tl.leiden(mdata, key_added="leiden_multiVI")
 
+L.info("Saving UMAP coordinates to csv file '%s" % args.output_csv)
 umap = pd.DataFrame(mdata.obsm['X_umap'], mdata.obs.index)
 umap.to_csv(args.output_csv)
 
+L.info("Saving MuData to 'tmp/multivi_scaled_adata.h5mu'")
 write_anndata(mdata, "tmp/multivi_scaled_adata.h5mu",use_muon=False)
 
 L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/batch_correct_none.py` & `panpipes-0.5.0/panpipes/python_scripts/batch_correct_none.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,26 +44,28 @@
                     help="neighbours method, scanpy or hnsw")
 parser.add_argument('--neighbors_k',
                     help="neighbors k")
 parser.add_argument('--neighbors_metric',
                     help="neighbor metric, e.g. euclidean or cosine")
 
 args, opt = parser.parse_known_args()
+L.info("Running with params: %s", args)
 
-L.info("reading data and starting integration pipeline with script: ")
-L.info(os.path.basename(__file__))
 
 
-# Scanorama is designed to be used in scRNA-seq pipelines downstream of noise-reduction methods,
-# including those for imputation and highly-variable gene filtering.
 
-# adata = sc.read(args.input_anndata)
-#adata = read_anndata(args.input_anndata, use_muon=True, modality=args.modality)
-adata = mu.read(args.input_anndata +"/" + args.modality)
-# adata = mdata.mod[args.modality] 
+
+
+adata_path = args.input_anndata +"/" + args.modality
+if os.path.exists(args.input_anndata):
+    L.info("Reading in data from '%s'" % adata_path)
+    adata = mu.read(args.input_anndata +"/" + args.modality)
+else:
+    L.info("missing input anndata")
+
 
 
 
 columns = [x.strip() for x in args.integration_col.split(",")]
 if len(columns)>1: 
     comb_columns = "|".join(columns)
     adata.obs[comb_columns] = adata.obs[columns].apply(lambda x: '|'.join(x), axis=1)
@@ -85,47 +87,47 @@
 else:
     # need to push scanpy to use .X if use_rep is None.
     pc_kwargs['use_rep'] = None
     pc_kwargs['n_pcs'] = int(args.neighbors_n_pcs)
 
 
 if dimred not in adata.obsm:
-    L.info("i need a dimred to start, computing pca with default param")
+    L.warning("Dimred '%s' could not be found in adata.obsm. Computing PCA with default parameters." % dimred)
     n_pcs = 50
     if adata.var.shape[0] < n_pcs:
         L.info("You have less features than number of PCs you intend to calculate")
         n_pcs = adata.var.shape[0] - 1
         L.info("Setting n PCS to %i" % int(n_pcs))    
+    L.info("Scaling data")
     sc.pp.scale(adata)
+    L.info("Computing PCA")
     sc.tl.pca(adata, n_comps=n_pcs, 
                     svd_solver='arpack', 
                     random_state=0) 
     pc_kwargs['use_rep'] = "X_pca"
     pc_kwargs['n_pcs'] = n_pcs
 
 
-
+L.info("Computing neighbors")
 run_neighbors_method_choice(adata, 
     method=args.neighbors_method, 
     n_neighbors=int(args.neighbors_k), 
     metric=args.neighbors_metric, 
     nthreads=max([threads_available, 6]), **pc_kwargs)
 
-L.info("done n_neighbours, saving stuff")
 
+L.info("Computing UMAP")
 sc.tl.umap(adata)
 
-L.info("done umap, saving stuff")
 #write out
+L.info("Saving UMAP coordinates to csv file '%s'" % args.output_csv)
 umap = pd.DataFrame(adata.obsm['X_umap'], adata.obs.index)
 umap.to_csv(args.output_csv)
 
-L.info("done")
-
 
 outfiletmp = ("tmp/no_correction_scaled_adata_" + args.modality + ".h5ad" )
 
-L.info("saving harmony corrected adata")
+L.info("Saving AnnData to '%s" % outfiletmp)
 write_anndata(adata, outfiletmp, use_muon=False, modality=args.modality)
 
-L.info("done")
+L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/batch_correct_scanorama.py` & `panpipes-0.5.0/panpipes/python_scripts/batch_correct_scanorama.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,59 +53,55 @@
 parser.add_argument('--modality',
                     help="modality")
 
 
 
 args, opt = parser.parse_known_args()
 
-
-
-L.info("Running with options: %s", args)
+L.info("Running with params: %s", args)
 
 # Scanorama is designed to be used in scRNA-seq pipelines downstream of noise-reduction methods,
 # including those for imputation and highly-variable gene filtering.
-L.info("reading data and starting integration pipeline with script: ")
-L.info(os.path.basename(__file__))
-
 #adata = read_anndata(args.input_anndata, use_muon=use_muon, modality="rna")
+L.info("Reading in MuData from '%s'" % args.input_anndata)
 mdata = mu.read(args.input_anndata)
 adata = mdata.mod[args.modality] 
 bcs = adata.obs_names.tolist()
 
 # scanorama can't integrate on 2+ variables, so create a fake column with combined information
 columns = [x.strip() for x in args.integration_col.split(",")]
 if len(columns) > 1:
-    L.info("using 2 columns to integrate on more variables")
+    L.info("Using 2 columns to integrate on more variables")
     # comb_columns = "_".join(columns)
     adata.obs["comb_columns"] = adata.obs[columns].apply(lambda x: '|'.join(x), axis=1)
 
     # make sure that batch is a categorical
     adata.obs["comb_columns"] = adata.obs["comb_columns"].astype("category")
     adata.obs['batch'] = adata.obs["comb_columns"]
 else:
     if args.integration_col != "batch":
         adata.obs['batch'] = adata.obs[args.integration_col]
 
 batches = adata.obs['batch'].unique()
-L.info("define scanorama inputs based on batches and number of PCs")
 # need contiguous batches
 scanorama_input = adata[adata.obs.sort_values(by="batch").index.tolist(), :]
 
 # filter by HVGs to make it equivalent to the old scripts,
 # which inputted the scaled object after filtering by hvgs.
+L.info("Filtering data by HVGs")
 scanorama_input = scanorama_input[:, scanorama_input.var.highly_variable]
 #also filter the X_PCA to be the number of PCs we actually want to use
+L.info("Subsetting X_pca to %s PCs" % args.neighbors_n_pcs)
 scanorama_input.obsm['X_pca'] = scanorama_input.obsm['X_pca'][:,0:int(args.neighbors_n_pcs)]
 
 
 # run scanoramam using the scanpy integrated approach
-L.info("run_scanorama")
+L.info("Running scanorama")
 
 sce.pp.scanorama_integrate(scanorama_input, key='batch', batch_size=int(args.batch_size))
-L.info("scanorama done")
 
 # not integrated
 
 # old method (simplified)
 # alldata = {}
 # for bb in batches:
 #     alldata[bb] = scanorama_input[scanorama_input.obs['batch'] == bb]
@@ -114,43 +110,45 @@
 # X_scanorama = scanorama.integrate_scanpy(adatas)
 # scanorama_input.obsm['X_scanorama'] = np.concatenate(X_scanorama)
 
 # put into the original order
 scanorama_input = scanorama_input[bcs, :]
 # check it worked
 if all(scanorama_input.obs_names == bcs):
-    L.info("barcode order is correct")
+    L.info("Barcode order is correct")
 else:
-    L.debug("barcode order in  batch corrected object is incorrect")
-    sys.exit("barcode order in  batch corrected object is incorrect")
+    L.error("Barcode order in  batch corrected object is incorrect")
+    sys.exit("Barcode order in  batch corrected object is incorrect")
 
-L.info(adata)
+L.info("Saving scanorama embedding to X_scanorama")
 # add to the AnnData object
 adata.obsm["X_scanorama"] = scanorama_input.obsm["X_scanorama"]
 
-L.info("integration run now calculate umap")
 
 if int(args.neighbors_n_pcs) > adata.obsm['X_scanorama'].shape[1]:
     L.warn(f"N PCs is larger than X_scanorama dimensions, reducing n PCs to  {adata.obsm['X_scanorama'].shape[1] -1}")
 n_pcs= min(int(args.neighbors_n_pcs), adata.obsm['X_scanorama'].shape[1]-1)
 
 # run neighbours and umap 
+L.info("Computing neighbors")
 run_neighbors_method_choice(adata, 
     method=args.neighbors_method, 
     n_neighbors=int(args.neighbors_k), 
     n_pcs=n_pcs, 
     metric=args.neighbors_metric, 
     use_rep='X_scanorama',
     nthreads=max([threads_available, 6]))
 
-
+L.info("Computing UMAP")
 sc.tl.umap(adata)
-L.info("done umap, saving stuff")
+
 # write out
 umap = pd.DataFrame(adata.obsm['X_umap'], adata.obs.index)
+L.info("Saving UMAP coordinates to csv file '%s" % args.output_csv)
 umap.to_csv(args.output_csv)
 
 # save the scanorama dim reduction in case scanorama is our favourite
+L.info("Saving AnnData to 'tmp/scanorama_scaled_adata.h5ad'")
 adata.write("tmp/scanorama_scaled_adata.h5ad")
 
-L.info("done")
+L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/batch_correct_scvi.py` & `panpipes-0.5.0/panpipes/python_scripts/batch_correct_scvi.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,174 +40,188 @@
                     help="n_pcs")
 parser.add_argument('--neighbors_method',
                     help="neighbours method, scanpy or hnsw")
 parser.add_argument('--neighbors_k',
                     help="neighbors k")
 parser.add_argument('--neighbors_metric',
                     help="neighbor metric, e.g. euclidean or cosine")
+parser.add_argument('--scvi_seed',default=None,
+                    help="set explicitly seed to make runs reproducible")
+
 
 
 args, opt = parser.parse_known_args()
-L.info(args)
+L.info("Running with params: %s", args)
 
 threads_available = multiprocessing.cpu_count()
 
 # load parameters
 params = read_yaml("pipeline.yml")
-L.info("Running scvi script")
-L.info("threads available: %s", threads_available)
 
 # scanpy settings
 sc.set_figure_params(facecolor="white")
 sc.settings.autoshow = False
 sc.settings.figdir = args.figdir
 
+if args.scvi_seed is not None:
+    scvi.settings.seed = int(args.scvi_seed)
+else:
+    scvi.settings.seed = 1492
+
+
 
 # test_script=params['rna']['scvi']['testrun']
 test_script=False
 if test_script:
     L.info("this is a test run")
     params['rna']['scvi']['training_args']['max_epochs'] = 10
 
 
 # load an process the scaled snRNAseq dataset --------------------------------------------------
 
 
-L.info("loading in anndata object ")
-
-
+L.info("Reading in Data from '%s'" % args.scaled_anndata)
 mdata = mu.read(args.scaled_anndata)
 if type(mdata) is mu.MuData:
     rna = mdata['rna']
     L.info(rna)
 elif type(mdata) is sc.AnnData:
     rna = mdata
     L.info(rna)
 else:
-    L.error("unknown file type")
-    sys.exit("file not MuData or Anndata")
+    L.error("Unknown file type. File not MuData or Anndata")
+    sys.exit("Unknown file type. File not MuData or Anndata")
 
 # this is a copy so we can subset vars and obs without changing the original object
 
 
 # in case of more than 1 variable, create a fake column with combined information
 columns = [x.strip() for x in args.integration_col.split(",")]
 if len(columns) > 1:
-    L.info("using 2 columns to integrate on more variables")
+    L.info("Using 2 columns to integrate on more variables")
     # bc_batch = "_".join(columns)
     rna.obs["bc_batch"] = rna.obs[columns].apply(lambda x: '|'.join(x), axis=1)
 
     # make sure that batch is a categorical
     rna.obs["bc_batch"] = rna.obs["bc_batch"].astype("category")
 else:
     rna.obs['bc_batch'] = rna.obs[args.integration_col]
 
 
 # add in raw counts as a layer 
 # add in test to see if raw layer exists alread
 if "raw_counts" in rna.layers.keys():
-    L.info("raw counts found in layer")
+    L.info("Found raw counts in .layers['raw_counts']")
 elif X_is_raw(rna):
+    L.info("Found raw counts in .X. Saving raw counts to .layers['raw_counts']")
     rna.layers["raw_counts"] = rna.X.copy()
 else:
-    L.info("merge in raw counts")
+    L.info("Merging in raw counts from '%s" % args.raw_anndata)
     sc_raw = read_anndata(args.raw_anndata, use_muon=True, modality="rna")
     #filter by barcodes in the scaled object
     sc_raw = sc_raw[sc_raw.obs_names.isin(rna.obs_names),: ]
+    L.info("Saving raw counts to .layers['raw_counts]")
     rna.layers["raw_counts"] = sc_raw.X.copy()
 
 
 # filter out mitochondria
 if params['rna']['scvi']['exclude_mt_genes']:
+    L.info("Filtering out mitochondrial genes")
     rna = rna[:, ~rna.var[params['rna']['scvi']['mt_column']]]
 
 # filter by Hvgs
+L.info("Filtering by HVGs")
 rna = rna[:, rna.var.highly_variable]
 
 
 if test_script:
     nn=1000
     L.info("this is a test so downsampling the dataset to %i cells" % nn)
     sc.pp.subsample(rna, n_obs=nn)
 
 rna = rna.copy()
 
-# scvi.model.data.setup_anndata(
+
+L.info("Setting up AnnData")
 scvi.model.SCVI.setup_anndata(
     rna,
     layer="raw_counts",
     batch_key='bc_batch'
 )
 
-
 scvi_model_args =  {k: v for k, v in params['rna']['scvi']['model_args'].items() if v is not None}
 print(scvi_model_args)
 scvi_training_args =  {k: v for k, v in params['rna']['scvi']['training_args'].items() if v is not None}
 print(scvi_training_args)
 scvi_training_plan =  {k: v for k, v in params['rna']['scvi']['training_plan'].items() if v is not None}
 print(scvi_training_plan)
 
-
-
+L.info("Defining model")
 vae = scvi.model.SCVI(rna, **scvi_model_args) 
-
+L.info("Running scVI")
 vae.train(**scvi_training_args, plan_kwargs=scvi_training_plan) 
-
+L.info("Finished Training now saving model")
 vae.save(os.path.join("batch_correction", "scvi_model"), 
                   anndata=False)
 
 # no early stopping?
+L.info("Plotting ELBO")
 vae.history["elbo_train"].plot()
 plt.savefig(os.path.join(args.figdir, "scvi_elbo_train.png"))
 
-fig, axs = plt.subplots(nrows=3, ncols=4, figsize=(16,8))
+fig, axs = plt.subplots(nrows=4, ncols=4, figsize=(16,10))
 axs = axs.ravel()
 for i, kk in enumerate(vae.history.keys()):
     vae.history[kk].plot(ax=axs[i])
     
 fig.tight_layout()
 plt.savefig(os.path.join(args.figdir, "scvi_metrics.png"))
 
 # vae.history['elbo_train']['elbo_train'].to_list()
-
+L.info("Extracting latent space")
 latent = vae.get_latent_representation()
-
+L.info("Saving latent to X_scVI")
 rna.obsm["X_scVI"] = latent
 rna.obs['bc_batch'] = rna.obs['bc_batch']
 
+L.info("Plotting latent")
 sc.pl.embedding(rna, "X_scVI", color="bc_batch", save="_batch.png")
 
 plot_df = pd.DataFrame(latent[:, 0:2])
 plot_df['bc_batch'] = rna.obs['bc_batch'].tolist()
 
 if int(args.neighbors_n_pcs) > rna.obsm['X_scVI'].shape[1]:
     L.warn(f"N PCs is larger than X_scVi dimensions, reducing n PCs to  {rna.obsm['X_scVI'].shape[1] -1}")
 
 n_pcs= min(int(args.neighbors_n_pcs), rna.obsm['X_scVI'].shape[1]-1)
 
-print(rna.obsm['X_scVI'].shape)
 # use scVI latent space for UMAP generation
 # sc.pp.neighbors(rna,n_neighbors=int(args.n_neighbors), use_rep="X_scVI")
+L.info("Computing neighbors")
 run_neighbors_method_choice(rna, 
     method=args.neighbors_method, 
     n_neighbors=int(args.neighbors_k), 
     n_pcs=n_pcs, 
     metric=args.neighbors_metric, 
     use_rep='X_scVI',
     nthreads=max([threads_available, 6]))
 
+L.info("Computing UMAP")
 sc.tl.umap(rna)
 
+L.info("Plotting UMAP")
 sc.pl.umap(
     rna,
     color=["bc_batch",],
     frameon=False, save="_scvi_batch.png"
 )
 
+L.info("Saving UMAP coordinates to csv file '%s" % args.output_csv)
 umap = pd.DataFrame(rna.obsm['X_umap'], rna.obs.index)
 umap.to_csv(args.output_csv)
 
 # save anndata to be used by other scvi tools applications
+L.info("Saving AnnData to 'tmp/scvi_scaled_adata_rna.h5ad'")
 rna.write(os.path.join("tmp", "scvi_scaled_adata_rna.h5ad"))
 
 L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/batch_correct_totalvi.py` & `panpipes-0.5.0/panpipes/python_scripts/batch_correct_totalvi.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,23 +42,33 @@
                     help="n_pcs", default=50)
 parser.add_argument('--neighbors_method', default="scanpy",
                     help="neighbours method, scanpy or hnsw")
 parser.add_argument('--neighbors_k', default=30,
                     help="neighbors k")
 parser.add_argument('--neighbors_metric',default="euclidean",
                     help="neighbor metric, e.g. euclidean or cosine")
+parser.add_argument('--scvi_seed',default=None,
+                    help="set explicitly seed to make runs reproducible")
+    
+    
+
 
 args, opt = parser.parse_known_args()
-L.info(args)
+L.info("Running with params: %s", args)
 # scanpy settings
 sc.set_figure_params(facecolor="white")
 sc.settings.autoshow = False
 sc.settings.figdir = args.figdir
 
 
+if args.scvi_seed is not None:
+    scvi.settings.seed = int(args.scvi_seed)
+else:
+    scvi.settings.seed = 1492
+
 # load parameters
 
 threads_available = multiprocessing.cpu_count()
 
 params = read_yaml("pipeline.yml")
 params['sample_prefix']
 
@@ -66,32 +76,32 @@
 
 test_script=False
 if test_script:
     L.info("this is a test run")
     params['multimodal']['totalvi']['training_args']['max_epochs'] = 10
 
 # ------------------------------------------------------------------
-L.info("Running totalvi script")
-
+L.info("Reading in MuData from '%s'" % args.scaled_anndata)
 mdata = mu.read(args.scaled_anndata)
 
 # we need to intersect the prot and rna modalities.
+L.info("Intersecting prot and rna modalities")
 intersect_obs_by_mod(mdata, ['rna', 'prot'])
 
 # this is a copy so we can subset vars and obs without changing the original object
 rna = mdata['rna'].copy()
 prot = mdata['prot'].copy()
 
 kwargs={}
 # in case of more than 1 variable, create a fake column with combined information
 if args.integration_col_categorical is not None :
     columns = [x.strip() for x in args.integration_col_categorical.split(",")]
     columns =[ x.replace("rna:","") for x in columns]
     if len(columns) > 1:
-        L.info("using 2 columns to integrate on more variables")
+        L.info("Using 2 columns to integrate on more variables")
         # bc_batch = "_".join(columns)
         rna.obs["bc_batch"] = rna.obs[columns].apply(lambda x: '|'.join(x), axis=1)
         # make sure that batch is a categorical
         rna.obs["bc_batch"] = rna.obs["bc_batch"].astype("category")
     else:
         rna.obs['bc_batch'] = rna.obs[columns] #since it's one
         rna.obs["bc_batch"] = rna.obs["bc_batch"].astype("category")
@@ -99,127 +109,134 @@
     kwargs["batch_key"] = "bc_batch"
 else:
     batch_categories = None
 if args.integration_col_continuous is not None :
         rna.obs['bc_batch_continuous'] = rna.obs[args.integration_col_continuous]
         kwargs["continuous_covariate_keys"] = ["bc_batch_continuous"]
 
-L.debug(kwargs)
 
 # add in raw counts as a layer 
 # try to find or load the raw counts
 if "counts" in rna.layers.keys():
-    L.info("raw counts found in layer")
+    L.info("Found raw RNA counts in .layers['counts']")
 elif "raw_counts" in rna.layers.keys():
+    L.info("Found raw RNA counts in .layers['raw_counts']")
+    L.info("Saving raw RNA counts to .layers['counts']")
     rna.layers["counts"] = rna.layers["raw_counts"].copy() 
-    L.info("raw counts found in layer")
 elif X_is_raw(rna):
     # this means the X layer is already raw and we can make the layer we need
-    L.info("raw counts found in X")
+    L.info("Found raw RNA counts in .X. Saving raw RNA counts to .layers['counts']")
     rna.layers["counts"] = rna.X.copy()
 else:
-    L.info("merge in raw counts")
+    L.info("Merging in raw RNA counts from '%s" % args.raw_anndata)
     sc_raw = read_anndata(args.raw_anndata, use_muon=True, modality="rna")
     #filter by barcodes in the scaled object
     sc_raw = sc_raw[sc_raw.obs_names.isin(rna.obs_names),: ]
+    L.info("Saving raw RNA counts to .layers['counts]")
     rna.layers["counts"] = sc_raw.X.copy()
 
 # filter prot outliers 
 if params['multimodal']['totalvi']['filter_prot_outliers']:
     # for this to work the user needs to (manually) make a column called prot_outliers
     # actually there is a thing in the qc pipe that calculates outliers, I don't like it very much though
     if "prot_outliers" in mdata['prot'].columns:
+        L.info("Filtering out prot outliers")
         mu.pp.filter_obs(mdata, "prot_outliers")
     else:
-        raise ValueError("prot_outliers column not found in mdata['prot'].obs")
+        raise ValueError("'prot_outliers' column not found in mdata['prot'].obs")
 
 # exluding isotypes
 if 'isotype' in prot.var.columns:
+    L.info("Excluding isotypes")
     prot = prot[:, ~prot.var.isotype]
 
 # filter out mitochondria
 if params['multimodal']['totalvi']['exclude_mt_genes']:
-    L.info("excluding mt genes")
+    L.info("Filtering out mitochondrial genes")
     rna = rna[:, ~rna.var[params['multimodal']['totalvi']['mt_column']]]
     
 # filter by Hvgs
 
 if params['multimodal']['totalvi']['filter_by_hvg']:
-    L.info("filtering by highly_variable")
+    L.info("Filtering by HVGs")
     rna = rna[:, rna.var.highly_variable]
 
 mdata.update()
 
 #make protein obsm pandas
 # need to find the raw counts in prot
 if X_is_raw(prot):
+    L.info("Found raw prot counts in .X")
     X_array = prot.X.copy()
 elif "raw_counts" in prot.layers.keys(): 
+    L.info("Found raw prot counts in .layers['raw_counts']")
     X_array = prot.layers['raw_counts'].copy()
 else:
-    raise AttributeError("raw counts not found in prot, \
-                        store in either X or in 'raw_counts' layer")
+    raise AttributeError("Raw counts not found in prot, \
+                        Store in either .X or in 'raw_counts' layer")
 
 
 X_df = pd.DataFrame(X_array.todense(), index=prot.obs_names, columns=prot.var_names)
 
 if X_df.shape[0] == rna.X.shape[0]:
-    L.info("adding protein_expression to obsm")
+    L.info("Adding protein_expression to .obsm['protein_expression']")
     #check the obs are in the correct order
     X_df = X_df.loc[rna.obs_names,:]
     X_df = X_df.astype('int')
     rna.obsm['protein_expression'] = X_df 
 else:
-    L.error("dimensions do not match, cannot integrate protein")
+    L.error("Dimension 0 of protein expression matrix and RNA expression matrix do not match")
+    sys.exit("Dimension 0 of protein expression matrix and RNA expression matrix do not match")
 
 # clear up to preserve ram
 del X_array, X_df
 gc.collect()
 
 mdata.update()
 
-L.debug(rna.obs.columns)
+L.info("Setting up AnnData")
 scvi.model.TOTALVI.setup_anndata(
     rna,
     layer="counts",
     protein_expression_obsm_key="protein_expression",
     # categorical_covariate_keys = "bc_batch"
     **kwargs
 )
 
 if params['multimodal']['totalvi']['model_args'] is None:
     totalvi_model_args =  {}
 else:
     totalvi_model_args =  {k: v for k, v in params['multimodal']['totalvi']['model_args'].items() if v is not None}
 
-print(totalvi_model_args)
 
 if params['multimodal']['totalvi']['training_args'] is None:
     totalvi_training_args = {}
 else:
     totalvi_training_args =  {k: v for k, v in params['multimodal']['totalvi']['training_args'].items() if v is not None}
 
-print(totalvi_training_args)
 
 if params['multimodal']['totalvi']['training_plan'] is None:
     totalvi_training_plan = {}
 else:
     totalvi_training_plan =  {k: v for k, v in params['multimodal']['totalvi']['training_plan'].items() if v is not None}
 
+print(totalvi_model_args)
+print(totalvi_training_args)
 print(totalvi_training_plan)
 
-
+L.info("Defining model")
 vae = scvi.model.TOTALVI(rna, **totalvi_model_args)
-
+L.info("Running totalVI")
 vae.train(**totalvi_training_args, plan_kwargs=totalvi_training_plan)
 
 vae.save(os.path.join("batch_correction", "totalvi_model"), 
                   anndata=False, overwrite=True )
 
 
+L.info("Plotting ELBO")
 plt.plot(vae.history["elbo_train"], label="train")
 plt.plot(vae.history["elbo_validation"], label="validation")
 plt.title("Negative ELBO over training epochs")
 # plt.ylim(1200, 1400)
 plt.legend()
 plt.savefig(os.path.join(args.figdir, "totalvi_elbo_plot.png"))
 
@@ -230,59 +247,67 @@
 L.info("""We support the use of mudata as a general framework for multimodal data
         For this reason, the object we save is not the classical anndata
         you would find in scvitools tutorial.
         We chose to save the learned SC representation in the 
         Mudata obsm slot, and any single modality processing in
         its own modality slot
             """)
+
+L.info("Extracting latent space and saving latent to X_totalVI")
 mdata.obsm["X_totalVI"] = vae.get_latent_representation()
 
 if batch_categories is not None:
     L.debug(batch_categories)
     if type(batch_categories) is not list:
         batch_categories = [batch_categories]
     normX, protein = vae.get_normalized_expression(
         n_samples=25,
         return_mean=True,
         transform_batch=batch_categories
     )
-
+    L.info("Saving denoised data to .obsm['totalvi_denoised_rna'] and .obsm['totalvi_denoised_protein']")
     # this is stored in obsm, because if we have filtered by hvg, it no longer fits specifications for a layer
     mdata['rna'].obsm["totalvi_denoised_rna"] = normX
     # reorder if rna and prot are in different orders
     mdata['prot'].obsm["totalvi_denoised_protein"] = protein.loc[mdata['prot'].obs_names,:]
     #
     df = vae.get_protein_foreground_probability(
         n_samples=25,
         return_mean=True,
         transform_batch=batch_categories
     )
+    L.info("Saving protein foreground prob to .obsm['totalvi_protein_foreground_prob']")
     mdata['prot'].obsm["totalvi_protein_foreground_prob"] = df.loc[mdata['prot'].obs_names,:]
 
 mdata.update()
 
 if int(args.neighbors_n_pcs) > mdata.obsm['X_totalVI'].shape[1]:
     L.warning(f"N PCs is larger than X_totalVI dimensions, reducing n PCs to  {mdata.obsm['X_totalVI'].shape[1] -1}")
 
 n_pcs= min(int(args.neighbors_n_pcs), mdata.obsm['X_totalVI'].shape[1]-1)
 
 
 # neighbors function has been made to magically calculate mudata neighbors using sc.pp.neighbors
 # because we want to use_rep = X_totalvi (as a pseudo single modality) not run multimodal mu.pp.neighbors
+L.info("Computing neighbors")
 run_neighbors_method_choice(mdata, 
     method=args.neighbors_method, 
     n_neighbors=int(args.neighbors_k), 
     n_pcs=n_pcs, 
     metric=args.neighbors_metric, 
     use_rep='X_totalVI',
     nthreads=max([threads_available, 6]))
 
+L.info("Computing UMAP")
 sc.tl.umap(mdata, min_dist=0.4)
+L.info("Computing Leiden clustering")
 sc.tl.leiden(mdata, key_added="leiden_totalVI")
 
+L.info("Saving UMAP coordinates to csv file '%s" % args.output_csv)
 umap = pd.DataFrame(mdata.obsm['X_umap'], mdata['rna'].obs.index)
 umap.to_csv(args.output_csv)
 
+L.info("Saving MuData to 'tmp/totalvi_scaled_adata.h5mu'")
 mdata.write("tmp/totalvi_scaled_adata.h5mu")
 
 L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/batch_correct_wnn.py` & `panpipes-0.5.0/panpipes/python_scripts/batch_correct_wnn.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,160 +39,161 @@
                     help="neighbor metric, e.g. euclidean or cosine")
 parser.add_argument('--low_memory',default=True,
                     help="set to True by default if cells in dataset >50k")
 
 
 args, opt = parser.parse_known_args()
 
-L.info(args)
+L.info("Running with params: %s", args)
 # scanpy settings
 sc.set_figure_params(facecolor="white")
 sc.settings.autoshow = False
 sc.settings.figdir = args.figdir
 
 params = pp.io.read_yaml("pipeline.yml")
 threads_available = multiprocessing.cpu_count()
 
 
 if params['multimodal']['WNN']['modalities'] is not None:
     modalities= params['multimodal']['WNN']['modalities']
     modalities = [x.strip() for x in modalities.split(",")]
-    L.info(f"using modalities :{modalities}")
+    L.info(f"Using modalities :{modalities}")
 
-L.info("running with batch corrections:")
+L.info("Running with batch corrections:")
 wnn_params_bc = params['multimodal']['WNN']['batch_corrected'] 
 if modalities is not None:
     wnn_params_bc= {k: wnn_params_bc[k] for k in wnn_params_bc.keys() & modalities}
 L.info( wnn_params_bc )
 
+L.info("Reading in MuData from '%s'" % args.scaled_anndata)
 mdata = mu.read(args.scaled_anndata)
 
 if all(x in modalities for x in mdata.mod.keys()):
     tmp = mdata.copy()
     removed_mods = None
 else:
     tmp = mdata.copy()
     removed_mods = list(set(mdata.mod.keys()) - set(modalities))
-    L.info(f"removing modalities {removed_mods}")
+    L.info(f"Removing modalities {removed_mods}")
     for rmod in removed_mods:
         del tmp.mod[rmod]
 
-L.info("intersecting modality obs before running wnn")
+L.info("Intersecting modality obs before running WNN")
 mu.pp.intersect_obs(tmp)
 
 
 #one could also check of obsp is not empty and use precomputed connectivities but i assume that if batch corrected the obsp is populated, if not, calc on the flight on pca
 dict_graph = {}
 for x in wnn_params_bc.keys():
     dict_graph[x] = {}
     if wnn_params_bc[x] is not None:
         dict_graph[x]["obsm"] = "X_" + wnn_params_bc[x]
         dict_graph[x]["anndata"] = "tmp/" + wnn_params_bc[x].lower() + "_scaled_adata_" + x +".h5ad"
     else: 
         dict_graph[x]["obsm"] = None
 
-L.debug(dict_graph)
+L.info(dict_graph)
 
 if dict_graph["rna"]["obsm"] == "X_scvi":
     dict_graph["rna"]["obsm"] = "X_scVI"
 
 for kmod in dict_graph.keys():
     L.info(kmod)
     pkmod=params['multimodal']['WNN']['knn'][kmod]
     if dict_graph[kmod]["obsm"] is not None:
         if dict_graph[kmod]["obsm"] not in tmp.mod[kmod].obsm.keys():
-            L.info("provided mdata doesn't have the desired obsm, just checking if it's bbknn you want.")
+            L.info("Provided mdata doesn't have the desired obsm, just checking if it's bbknn you want.")
             if dict_graph[kmod]["obsm"] == "X_bbknn":
                 if len(tmp.mod[kmod].obsp.keys()) > 0 and "neighbors" in tmp.mod[kmod].uns.keys() : 
-                     L.info("i found a populated obsp slot and I assume it's bbknn")
+                     L.info("Populated obsp slot found. Assuming it's bbknn")
                 else:
                     if dict_graph[kmod]["anndata"] is not None:
-                        L.info("reading precomputed connectivities for bbknn")
+                        L.info("Reading precomputed connectivities for bbknn")
                         adata = mu.read(dict_graph[kmod]["anndata"])
                         tmp.mod[kmod].obsp = adata.obsp.copy()
                         tmp.mod[kmod].obsm[dict_graph[kmod]["obsm"]] = adata.obsm[dict_graph[kmod]["obsm"]].copy()
                         tmp.mod[kmod].uns["neighbors"]= adata.uns["neighbors"].copy()
                         tmp.update()
             else:
                 if dict_graph[kmod]["anndata"] is not None:
-                    L.info("provided mdata doesn't have the desired obsm. reading the batch corrected data from another stored object")
+                    L.info("Provided mdata doesn't have the desired obsm. reading the batch corrected data from another stored object")
                     adata = mu.read(dict_graph[kmod]["anndata"])
                     L.debug(kmod + "object")
                     L.debug(adata)
                     tmp.mod[kmod].obsm[dict_graph[kmod]["obsm"]] = adata.obsm[dict_graph[kmod]["obsm"]].copy()
                     tmp.mod[kmod].obsp = adata.obsp.copy()
                     tmp.mod[kmod].uns['neighbors'] = adata.uns['neighbors'].copy()
                     tmp.update()
                     repuse = dict_graph[kmod]["obsm"] 
                 else:
-                    L.info("could not find the desired obsm and the anndata slot is empty, will calculate on the flight")
+                    L.warning("Could not find the desired obsm and the anndata slot is empty, will calculate on the flight")
                     if kmod =="atac":
                         if "X_lsi" in tmp.mod[kmod].obsm.keys():
                             repuse = "X_lsi"
                         else:
                             repuse = "X_pca"
-                        L.info("falling back on %s" %(repuse) )
+                        L.info("Falling back on %s" %(repuse) )
             
-                    L.info("calculating neighbours")
+                    L.info("Computing neighbours")
                     if repuse != "X_bbknn":
                         run_neighbors_method_choice(tmp.mod[kmod], 
                             method=pkmod['method'], 
                             n_neighbors=int(pkmod['k']), 
                             n_pcs=min(int(pkmod['npcs']), mdata.var.shape[0]-1), #this should be the # rows of var, not obs
                             metric=pkmod['metric'], 
                             #does this throw an error if no PCA for any single mod is stored?
                             use_rep=repuse,
                             nthreads=max([threads_available, 6]))
         else:
             L.info("Using %s" %(dict_graph[kmod]["obsm"]))            
     else:
-        L.info("could not find the desired obsm and the anndata slot is empty, will calculate on the flight")
+        L.warning("Could not find the desired obsm and the anndata slot is empty, will calculate on the flight")
         repuse ="X_pca"
         if kmod =="atac":
             if "X_lsi" in tmp.mod[kmod].obsm.keys():
                 repuse = "X_lsi"
             else:
                 repuse = "X_pca"
             L.info("falling back on %s" %(repuse) )
 
-        L.info("calculating neighbours")
-        
+        L.info("Computing neighbours")
         run_neighbors_method_choice(tmp.mod[kmod], 
             method=pkmod['method'], 
             n_neighbors=int(pkmod['k']), 
             n_pcs=min(int(pkmod['npcs']), mdata.var.shape[0]-1), #this should be the # rows of var, not obs
             metric=pkmod['metric'], 
             #does this throw an error if no PCA for any single mod is stored?
             use_rep=repuse,
             nthreads=max([threads_available, 6]))
 
-L.debug(tmp)
 tmp.update()
-L.debug(tmp)
-L.info("Now running WNN")
 
+L.info("Running WNN")
 mu.pp.neighbors(tmp, 
                 n_neighbors= int(args.n_neighbors),
                 n_bandwidth_neighbors= int(args.n_bandwidth_neighbors),
                 n_multineighbors= int(args.n_multineighbors),
                 metric= args.metric,
                 low_memory= check_for_bool(args.low_memory),   
                 key_added='wnn')
-L.info("WNN finished now calculate umap")
 
+L.info("Computing UMAP")
 mu.tl.umap(tmp,min_dist=0.4, neighbors_key='wnn')
 #For taking use of mdata.obsp['connectivities'], it’s scanpy.tl.leiden() that should be used. not muon.tl.leiden
+L.info("Computing Leiden clustering")
 sc.tl.leiden(tmp, neighbors_key='wnn', key_added='leiden_wnn') 
 
+L.info("Saving UMAP coordinates to csv file '%s" % args.output_csv)
 umap = pd.DataFrame(tmp.obsm['X_umap'], tmp.obs.index)
 umap.to_csv(args.output_csv)
 
 #add back modalities that were not used for this run
 
 if removed_mods is not None:
     for rmd in removed_mods:
         tmp.mod[rmd] = mdata.mod[rmd].copy()
 
+L.info("Saving MuData to 'tmp/wnn_scaled_adata.h5mu'")
 tmp.write("tmp/wnn_scaled_adata.h5mu")
 
 L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/collate_mdata.py` & `panpipes-0.5.0/panpipes/python_scripts/collate_mdata.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,65 +27,74 @@
 parser.add_argument("--umap_files_csv",
                     default=None,
                     help = "comma separated  table of mod,txt file containing umap coordinates")
 parser.add_argument("--output_mudata",
                     default="mdata.h5mu",
                     help="file name, format: .h5mu")
 args, opt = parser.parse_known_args()
-L.info(args)
+
+L.info("Running with params: %s", args)
+
+L.info("Reading in MuData from '%s'" % args.input_mudata)
 mdata = mu.read(args.input_mudata)
 
-L.info("loading clusters")
+L.info("Reading in cluster information")
 cf = pd.read_csv(args.clusters_files_csv)
 
 if isinstance(mdata, MuData):
     pass
 elif isinstance(mdata, AnnData):
     mds = cf['mod'].unique().tolist()
     if len(mds)>1:
         sys.exit("You have clustered multiple modalities but are providing only a unimodal anndata")
     else:
-        L.warn("found one modality, converting to mudata: %s " % mds[0] )    
+        L.warn("Found one modality, converting to mudata: %s " % mds[0] )    
         tmp = MuData({mds[0]:mdata})
         del mdata
         mdata = tmp
         del tmp
 
 # add in the clusters
 
 
-
+L.info("Adding cluster information to MuData")
 for i in range(cf.shape[0]):
     cf_df = pd.read_csv(cf['fpath'][i], sep='\t', index_col=0) 
     cf_df['clusters'] = cf_df['clusters'].astype('str').astype('category')
     cf_df = cf_df.rename(columns={"clusters":cf['new_key'][i]})
     
     if cf['mod'][i] != "multimodal":
         mdata[cf['mod'][i]].obs = mdata[cf['mod'][i]].obs.merge(cf_df, left_index=True, right_index=True)
     else:
         mdata.obs = mdata.obs.merge(cf_df, left_index=True, right_index=True)
 
-uf = pd.read_csv(args.umap_files_csv)
 
+L.info("Adding UMAP coordinates to MuData")
+uf = pd.read_csv(args.umap_files_csv)
 
 for i in range(uf.shape[0]):
     uf_df = pd.read_csv(uf['fpath'][i], sep='\t', index_col=0) 
     mod = uf['mod'][i]
     new_key = uf['new_key'][i]
     if uf['mod'][i] != "multimodal":
         if all(mdata[mod].obs_names == uf_df.index):
             mdata[mod].obsm[new_key] =  uf_df.to_numpy()
         else:
-            L.warn("cannot integrate %s into mdata as obs_names mismatch" % uf.iloc[i,:] )
+            L.warn("Cannot integrate %s into mdata as obs_names mismatch" % uf.iloc[i,:] )
     else:
         # check the observations are the same
         if set(mdata.obs_names).difference(uf_df.index) == set():
             # put the observations in the same order
             uf_df = uf_df.loc[mdata.obs_names,:]
             mdata.obsm[new_key] =  uf_df.to_numpy()
         else:
-            L.warning("cannot integrate %s into mdata as obs_names mismatch" % uf.iloc[i,:] )
+            L.warning("Cannot integrate %s into mdata as obs_names mismatch" % uf.iloc[i,:] )
+
 
+L.info("Saving updated MuData to '%s'" % args.output_mudata)
 mdata.write(args.output_mudata)
-mdata.obs.to_csv(re.sub(".h5mu", "_cell_metdata.tsv", args.output_mudata), sep='\t')
 
-L.info("done")
+output_csv = re.sub(".h5mu", "_cell_metdata.tsv", args.output_mudata)
+L.info("Saving metadata to '%s'" % output_csv)
+mdata.obs.to_csv(output_csv, sep='\t')
+
+L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/concat_adata.py` & `panpipes-0.5.0/panpipes/python_scripts/concat_adata.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,27 +58,28 @@
                     help='')
 parser.add_argument('--protein_new_index_col',
                     default=None,
                     help='')        
 
 parser.set_defaults(verbose=True)
 args, opt = parser.parse_known_args()
-L.info("running with:")
-L.info(args)
+L.info("Running with params: %s", args)
 
 if len(args.input_files_str) == 0:
-    sys.exit("no input files detected")
+    L.error("No input files detected")
+    sys.exit("No input files detected")
     
 lf = re.split(',', args.input_files_str)
 
 sfile=args.submissionfile
 
 #  lf = glob.glob("./tmp/*raw.h5mu")
 # sfile= "CARTC_bonemarrow_samples.tsv"
 
+L.info("Reading in submission file from '%s'" % sfile)
 caf = pd.read_csv(sfile, sep="\t")
 # the modality argument is relevent only if use_muon is True.
 # mdatas = [read_anndata(i, use_muon, modality="all") for i in lf]
 mdatas = [mu.read(i) for i in lf]
 # [x.var_names_make_unique() for x in mdatas]
 
 
@@ -91,26 +92,27 @@
     # that atac shouldn't be concatenated?
     temp = mdatas[0]
     if 'atac' in temp.mod.keys():
         mdata=mdatas[0]
         del temp
     elif 'prot' in temp.mod.keys() or 'rna' in temp.mod.keys():
         ## IF RNA and PROT is ok to concatenate ----------
+        L.info("Concatenating RNA and prot")
         mdata = concat_mdatas(mdatas,
             batch_key="sample_id", 
             join_type=args.join_type)
 
 # remove to avoid mem issues
 del mdatas
 
 ### add metmdata from caf
 L.debug(mdata.obs.columns)
 L.debug(mdata.obs.head())
 
-L.info("add metadata")
+L.info("Adding metadata")
 # add metmdata to each object
 metadatacols = args.metadatacols
 # metadatacols="mdata_cols"
 # check sample_id is in metadatacols as a minimum requirement
 if metadatacols == None :
     pass
 elif metadatacols == 'None':
@@ -144,25 +146,25 @@
         mdata.obs.index.name = None
         mdata.obs['cellbarcode'] = mdata.obs.index
         mdata.update_obs()
     else:
         # which column is missing?
         missingcols= " ".join([x for x in metadatacols if x not in caf.columns])
         L.error("Required columns missing form samples file: %s" % missingcols)
-        sys.exit("Exiting because required columns not in samples file, check the log file for details")
+        sys.exit("Required columns missing form samples file: %s" % missingcols)
 
 
 # if 'rep' in mdata.mod.keys():
 #     col_update = mdata['rep'].obs.columns[mdata['rep'].obs.columns.str.contains("count")]
 #     mdata['rep'].obs[col_update] = mdata['rep'].obs[col_update].apply(pd.to_numeric)
 #     mdata.update()
     
 # add in cell level metadata
 if args.barcode_mtd_df is not None :
-    L.info("Add barcode level metadata")
+    L.info("Adding barcode level metadata")
     # check demult_metadatacols exists and contains antibody
     barcode_metadatacols = args.barcode_mtd_metadatacols.split(',')
     # load the demultiplexing data
     barcode_mtd_df = pd.read_csv(args.barcode_mtd_df, index_col=None)
     if len(barcode_mtd_df['sample_id'].unique().tolist()) > 1:
         barcode_mtd_df.index = barcode_mtd_df[['barcode_id', 'sample_id']].apply(lambda row: "-".join(row.values.astype(str)), axis=1)
     else:
@@ -177,20 +179,21 @@
 
 
 L.debug(mdata.obs.columns)
 L.debug(mdata.obs.head())
 # update the protein variable to add in extra info like isotype and alternate name for prot
 if args.protein_var_table is not None:
     try:
+        L.info("Reading in protein var table from '%s'" % args.protein_var_table)
         df = pd.read_csv(args.protein_var_table, sep='\t', index_col=0)
-        L.info("merging protein table with var")
+        L.info("Merging protein table with var")
         # add_var_mtd(mdata['prot'], df)
         var_df = mdata['prot'].var.merge(df, left_index=True, right_index=True)
         if args.protein_new_index_col is not None:
-            L.info("updating prot.var index")
+            L.info("Updating prot.var index")
             # update_var_index(mdata['prot'], args.protein_new_index_col)
             var_df =var_df.reset_index().set_index(args.protein_new_index_col)
             var_df = var_df.rename(columns={'index':'orig_id'})
             var_df.index.name = None
         mdata['prot'].var = var_df
         mdata.update_var()
         mdata.update()
@@ -198,21 +201,21 @@
         # we assume this has been inidicated in a "hashing_ab" column in the protein metadata file
         if "hashing_ab" in mdata['prot'].var.columns:
             # create new modality for hashing
             mdata.mod["hashing_ab"]=mdata["prot"][:, mdata["prot"].var["hashing_ab"]]
             # subset old modality to remove hashing
             mdata.mod['prot'] = mdata["prot"][:, ~mdata["prot"].var["hashing_ab"]]
     except FileNotFoundError:
-        warnings.warn("protein metadata table not found")
+        warnings.warn("Protein metadata table not found")
 mdata.update()
 # tidy up metadata
 # move sample_id to the front
 # cols = mdata.obs.columns.tolist()
 # cols.insert(0, cols.pop(cols.index('sample_id')))
 # mdata.obs = mdata.obs.reindex(columns=cols)
 L.debug(mdata.obs.dtypes)
 
-L.info("writing to file {}".format(str(args.output_file)))
+L.info("Writing to file '%s'" % args.output_file)
 
 mdata.write(args.output_file)
 
-L.info("done")
+L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/downsample.py` & `panpipes-0.5.0/panpipes/python_scripts/downsample.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,29 +38,29 @@
                     help='')
 parser.add_argument('--downsample_col', default=None,
                     help='')
 parser.add_argument('--intersect_mods', default=None,
                     help='comma separated string of modalities we want to intersect_obs on')                 
 
 
-L.warning("Running filter_mudata")
-
 parser.set_defaults(verbose=True)
 args, opt = parser.parse_known_args()
+L.info("Running with params: %s", args)
 
 # load data
+L.info("Reading in MuData from '%s'" % args.input_mudata)
 mdata = mu.read(args.input_mudata)
 
 if isinstance(mdata, AnnData):
     # convert anndata to muon
     mdata=MuData({'mod':mdata})
 
 orig_obs = mdata.obs
 
-L.info("Number of cells per sample \n%s" % mdata.obs.sample_id.value_counts())
+L.info("Before downsampling: number of cells per sample \n%s" % mdata.obs.sample_id.value_counts())
 
 
 if args.downsample_col == "None":
     args.downsample_col = None
 
 if args.intersect_mods is None:
     # we assume all mods
@@ -70,28 +70,27 @@
 
 
 # remove unused categories in batch col
 if args.downsample_col is not None:
     mdata.obs[args.downsample_col] = mdata.obs[args.downsample_col].cat.remove_unused_categories()
 
 # do the downsample.
-
+L.info("Downsampling modalities %s" % mods)
 downsample_mudata(mdata, nn=int(args.downsample_value),
     cat_col=args.downsample_col,
     mods = mods,
     inplace=True)
 print(mdata)
 
 
 mdata.update()
-    
-L.info("Number of cells per sample")
-L.info(mdata.obs.sample_id.value_counts())
+L.info("After downsampling: number of cells per sample \n%s" % mdata.obs.sample_id.value_counts())
 
 # write out the observations
-write_obs(mdata, output_prefix=re.sub("\\.(.*)", "", args.output_mudata), 
-        output_suffix="_downsampled_cell_metadata.tsv")
-
+prefix = re.sub("\\.(.*)", "", args.output_mudata)
+L.info("Saving updated obs in a metadata tsv file to " + prefix + "_downsampled_cell_metadata.tsv")
+write_obs(mdata, output_prefix=prefix, output_suffix="_downsampled_cell_metadata.tsv")
 
+L.info("Saving updated MuData to '%s'" % args.output_mudata)
 mdata.write(args.output_mudata)
-#This stage is the point (i.e. pre-normalisation) where the mdata file can be outputted so that we can extract raw matrix for the cellphonedb.
+
 L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/generate_cellxgene.py` & `panpipes-0.5.0/panpipes/python_scripts/generate_cellxgene.py`

 * *Files identical despite different names*

### Comparing `panpipes-0.4.1/panpipes/python_scripts/integrate_wnn.py` & `panpipes-0.5.0/panpipes/python_scripts/integrate_wnn.py`

 * *Files identical despite different names*

### Comparing `panpipes-0.4.1/panpipes/python_scripts/make_adata_from_csv.py` & `panpipes-0.5.0/panpipes/python_scripts/make_adata_from_csv.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 parser.add_argument('--fragments_file',
                     default=None,
                     help='ATAC/Multiome specific input file from csv')                    
 
 
 parser.set_defaults(verbose=True)
 args, opt = parser.parse_known_args()
-L.info(args)
+L.info("Running with params: %s", args)
 # Make mdata object
 
 # unimodal mu (check if all the modalities)
 if isinstance(args.mode_dictionary, dict):
     mode_dictionary = args.mode_dictionary
 else:
     mode_dictionary = read_yaml(args.mode_dictionary) 
@@ -95,68 +95,78 @@
             "atac": [args.atac_infile, args.atac_filetype], 
             "tcr":[args.tcr_filtered_contigs, args.tcr_filetype],
             "bcr":[args.bcr_filtered_contigs, args.bcr_filetype]}
 #subset to the modalities we want from permf
 all_files = {nm: x  for (nm, x) in all_files.items() if nm in permf}
 # this will work for any combination of modalities or number of modalities in all_files.
 [check_filetype(x[0], x[1]) for x in all_files.values()]
+L.info("Creating MuData")
 mdata = load_mdata_from_multiple_files(all_files)
                 
 # now lets do some extra processing on the different modalities
+L.info("Preprocessing each modality")
 if 'rna' in mdata.mod.keys():
+    L.info("Modality: RNA")
+    L.info("Making var names unique")
     mdata['rna'].var_names_make_unique()
     # keep only rna with at least 1 count (relevent when loading raw data)
     mdata['rna'].obs['total_counts'] = mdata['rna'].X.sum(axis=1) 
+    L.info("Subsetting on cells with total_counts > 1.")
     mu.pp.filter_obs(mdata['rna'], 'total_counts', lambda x: (x > 1))
     # drop this columns as we don't need it anymore, and it will confuse things downstream
     mdata['rna'].obs = mdata['rna'].obs.drop(columns="total_counts")
     mdata.update()
 
 if 'prot' in mdata.mod.keys():
+    L.info("Modality: prot")
     if 'rna' in mdata.mod.keys():
         if check_for_bool(args.subset_prot_barcodes_to_rna):
+            L.info("Intersecting observations of modalities RNA and prot")
             intersect_obs_by_mod(mdata, ['rna', 'prot'])
             mdata.update()
-    L.info(mdata['prot'].var.head())
 
 if 'atac' in mdata.mod.keys():
+    L.info("Modality: ATAC")
+    L.info("Making var names unique")
     mdata['atac'].var_names_make_unique()
     if args.per_barcode_metrics_file is not None:
-        L.info("Returning mudata with metadata from barcode metrics csv")
+        L.info("Merging in metadata from barcode metrics csv '%s'" % args.per_barcode_metrics_file)
         per_barcode_metrics_file = pd.read_csv(args.per_barcode_metrics_file, index_col=0) #it's a csv by default and goes in atac obs
         mdata.mod['atac'].obs = mdata.mod['atac'].obs.merge(per_barcode_metrics_file, left_index=True, right_index=True)
     if args.peak_annotation_file is not None:
-        L.info("Returning mudata with peak annotation in mdata['atac'].uns['atac']['peak_annotation']")
+        L.info("Saving peak annotation from '%s' to mdata['atac'].uns['atac']['peak_annotation']" % args.peak_annotation_file)
         add_peak_annotation(mdata, annotation=args.peak_annotation_file, sep="\t", return_annotation= False)
     if args.fragments_file is not None:
-        L.info("Returning mudata with fragments file in mdata['atac'].uns['files']['fragments']")
+        L.info("Saving fragments file from '%s' to mdata['atac'].uns['files']['fragments']" % args.fragments_file)
         locate_fragments(mdata,fragments=args.fragments_file, return_fragments= False)
 
 
 if 'rep' in mdata.mod.keys():
+    L.info("Modality: rep")
+    L.info("Saving count metadata in .obs as numeric")
     col_update = mdata['rep'].obs.columns[mdata['rep'].obs.columns.str.contains("count")]
     mdata['rep'].obs[col_update] = mdata['rep'].obs[col_update].apply(pd.to_numeric)
     mdata.update()
     
 
 #make var names unique
 for mm in mdata.mod.keys():
     mdata[mm].var_names_make_unique()
 
+L.info("Saving sample id to mdata.obs['sample_id']")
 mdata.obs['sample_id'] = str(args.sample_id)
 
 # copy the  to each modality
+print("Saving sample_id to each modality")
 for mm in mdata.mod.keys():
-    print("saving sample_id to each modality")
     # mdata[mm].obs['sample_id'] = mdata.obs['sample_id']
     mdata[mm].obs['sample_id'] = mdata.obs.loc[mdata[mm].obs_names,:]['sample_id']
 
 mdata.update()
 
 
-L.info("saving data")
-L.debug(mdata)
+L.info("Saving MuData to '%s'" % args.output_file)
 # this will write the file as anndata or muon depending on the class of mdata.
 mdata.write(args.output_file)
 
-L.info("done")
+L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/make_mudataspatial_from_csv.py` & `panpipes-0.5.0/panpipes/python_scripts/make_mudataspatial_from_csv.py`

 * *Files 12% similar despite different names*

```diff
@@ -57,17 +57,16 @@
                     help='')
 parser.add_argument('--spatial_transformation', 
                     default=None,
                     help='')
 
 parser.set_defaults(verbose=True)
 args, opt = parser.parse_known_args()
-L.info(args)
+L.info("Running with params: %s", args)
 
-L.info("starting the code now")
 # unimodal mu (check if all the modalities)
 if isinstance(args.mode_dictionary, dict):
     mode_dictionary = args.mode_dictionary
 else:
     mode_dictionary = read_yaml(args.mode_dictionary) 
 #{'spatialT': True}
 
@@ -113,52 +112,57 @@
         create_soft_link(original_path, target_path)
     else:
         create_soft_link(os.path.abspath(transform_file), target_path)
 
 
 
 if args.spatial_filetype=="vizgen":
+    L.info("Reading in Vizgen data with squidpy.read.vizgen() into AnnData from directory " + args.spatial_infile)
     adata = sq.read.vizgen(path = args.spatial_infile, #path, mandatory for squidpy
                         counts_file=args.spatial_counts, #name of the counts file, mandatory for squidpy
                         meta_file = args.spatial_metadata, #name of the metadata file, mandatory for squidpy
                         transformation_file=args.spatial_transformation,
                         library_id = str(args.sample_id)) #this also has kwargs for read_10x_h5 but keep simple
     adata.uns["spatial"][str(args.sample_id)]["scalefactors"]["transformation_matrix"].columns = adata.uns["spatial"][str(args.sample_id)]["scalefactors"]["transformation_matrix"].columns.astype(str)
 elif args.spatial_filetype =="visium":
+    L.info("Reading in Visium data with squidpy.read.visium() into AnnData from directory " + args.spatial_infile)
     adata = sq.read.visium(path = args.spatial_infile, #path, mandatory for squidpy
                         counts_file=args.spatial_counts, #name of the counts file, mandatory for squidpy
                         library_id = str(args.sample_id)
                         ) #this also has kwargs for read_10x_h5 but keep simple
 
-L.info("adata is now: %s" % adata)
-L.info("creating mudata")
+L.info("Resulting AnnData is:")
+L.info(adata)
+L.info("Creating MuData with .mod['spatial']")
 
 mdata = MuData({"spatial": adata})
 
 
 #---------------
 # do some extra processing on the different modalities as needed
 #---------------
 
+L.info("Making var names unique")
 #make var names unique
 for mm in mdata.mod.keys():
     mdata[mm].var_names_make_unique()
 
+L.info("Adding sample_id '%s'to MuData.obs and MuData.mod['spatial'].obs" % args.sample_id)
 mdata.obs['sample_id'] = str(args.sample_id)
 
 # copy the sample_id to each modality
 for mm in mdata.mod.keys():
-    print("saving sample_id to each modality")
     # mdata[mm].obs['sample_id'] = mdata.obs['sample_id']
     mdata[mm].obs['sample_id'] = mdata.obs.loc[mdata[mm].obs_names,:]['sample_id']
 
 mdata.update()
 
+L.info("Resulting MuData is:")
+L.info(mdata)
 
-L.info("saving data")
+L.info("Saving MuData to '%s'" % args.output_file)
 L.debug(mdata)
-# this will write the file as anndata or muon depending on the class of mdata.
 mdata.write(args.output_file)
 
-L.info("done")
+L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/plot_cluster_umaps.py` & `panpipes-0.5.0/panpipes/python_scripts/plot_cluster_umaps.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,92 +29,95 @@
                     default="mdata.h5mu",
                     help="file name, format: .h5mu")
 parser.add_argument("--modalities",
                     default="rna",
                     help="list of modalities to search for UMAPs in")
 args, opt = parser.parse_known_args()
 
-L.info("running with:")
-L.info(args)
+L.info("Running with params: %s", args)
 # args = argparse.Namespace(infile='mdata_clustered.h5mu', figdir=None)
 # ---------
 
 def main(adata,figdir):
     # get all possible umap coords
     pattern="X_umap(.*)"
     obsm_keys = [x for x in adata.obsm.keys() if re.search(pattern, x)]
-    L.info("Umap keys founds %s" % obsm_keys)
-    # get all possible clustersclusters
+    L.info("UMAP keys found: %s" % obsm_keys)
+    # get all possible clusters
     pattern=re.compile(r'^leiden|^louvain') 
     cluster_keys  = [x for x in adata.obs.columns if re.search(pattern, x)]
-    L.info("Cluster keys founds %s" % cluster_keys)
+    L.info("Cluster keys found: %s" % cluster_keys)
     if len(obsm_keys) == 0  or len(cluster_keys) == 0:
         return
     
     # make sure clusters are categories
     for ck in cluster_keys:
         adata.obs[ck] = adata.obs[ck].astype('category')
     # plot all the umaps
     for ok in obsm_keys:
+        L.info("Plotting UMAP on %s coloured by %s" % (ok, cluster_keys))
         fig = sc.pl.embedding(adata, basis = ok,color=cluster_keys,
          show=False, return_fig=True, legend_loc='on data')
         for ax in fig.axes:
             ax.set(xlabel="UMAP_1", ylabel="UMAP_2")
         fig.suptitle(ok, y=1.0)
+        L.info("Saving figure to '%s'" % os.path.join(figdir, ok +  "_clusters.png"))
         fig.savefig(os.path.join(figdir, ok +  "_clusters.png"))
 
 def plot_spatial(adata,figdir):
     # get all possible umap coords
     pattern="spatial(.*)"
     obsm_keys = [x for x in adata.obsm.keys() if re.search(pattern, x)]
-    L.info("Umap keys founds %s" % obsm_keys)
+    L.info("UMAP keys found: %s" % obsm_keys)
     # get all possible clustersclusters
     pattern=re.compile(r'^leiden|^louvain') 
     cluster_keys  = [x for x in adata.obs.columns if re.search(pattern, x)]
-    L.info("Cluster keys founds %s" % cluster_keys)
+    L.info("Cluster keys found: %s" % cluster_keys)
     if len(obsm_keys) == 0  or len(cluster_keys) == 0:
         return
     
     # make sure clusters are categories
     for ck in cluster_keys:
         adata.obs[ck] = adata.obs[ck].astype('category')
     # plot all the umaps
     for ok in obsm_keys:
+        L.info("Plotting UMAP on %s coloured by %s" % (ok, cluster_keys))
         fig = sc.pl.embedding(adata, basis = ok,color=cluster_keys,
          show=False, return_fig=True, legend_loc='on data')
         for ax in fig.axes:
             ax.set(xlabel="spatial1", ylabel="spatial2")
         fig.suptitle(ok, y=1.0)
+        L.info("Saving figure to '%s'" % os.path.join(figdir, ok +  "_clusters.png"))
         fig.savefig(os.path.join(figdir, ok +  "_clusters.png"))
 
 
-L.debug("load data")
+
+L.info("Reading in MuData from '%s'" % args.infile)
 mdata = read(args.infile)
 
 mods = args.modalities.split(',')
 # detemin initial figure directory based on object type
 
 # do plotting
 if 'multimodal' in mods:
     if os.path.exists("multimodal/figures") is False:
         os.makedirs("multimodal/figures")
+    L.info("Plotting multimodal figures")
     main(mdata, figdir="multimodal/figures")
 
 
 # we also need to plot per modality
 if type(mdata) is MuData:
     for mod in mdata.mod.keys():
         if mod in mods:
-            L.info("plotting for modality: %s" % mod)
+            L.info("Plotting for modality: %s" % mod)
             figdir  = os.path.join(mod, "figures")
             if os.path.exists(figdir) is False:
                 os.makedirs(figdir)
             if mod == "spatial": # added separate function for spatial
                 plot_spatial(mdata[mod], figdir)
             else:
                 main(mdata[mod], figdir)
 
 
 
-
-
-L.info('done')
+L.info('Done')
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/plot_custom_markers.py` & `panpipes-0.5.0/panpipes/python_scripts/plot_custom_markers.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,16 +43,15 @@
                     default="Marker_Lists-myeloid.csv",
                     help="comma separateed list of marker_list csvs, one column of gene_ids")
 parser.add_argument("--base_figure_dir", default="figures/",
                     help="figures path")
 
 
 args, opt = parser.parse_known_args()
-L.info("running with:")
-L.info(args)
+L.info("Running with params: %s", args)
 sc.settings.figdir = args.base_figure_dir
 
 # ---- script
 
 def main(adata, mod, df, grouping_var, pfx, layer_choice=None):
     for gc in df['group'].unique():
         # define file name
@@ -63,53 +62,59 @@
             layer_string = layer_choice
         # get features
         fetches = df[df['group'] == gc]['feature']
         plot_features = [gg for gg in fetches if gg in adata.var_names]
         plot_features = list(set(plot_features))
         # do PCA if it is missing, (prerequisite for dendrogram)
         if "X_pca" not in adata.obsm.keys():
+            L.warning("X_pca was not found for modality %s, but is required for the dendogram. Computing PCA with default parameters." % mod)
             sc.pp.pca(adata)
         use_dendrogram=True
         if len(adata.obs[grouping_var].unique()) > 2:
             try:
+                L.info("Plotting dendogram for modality %s and group %s on X_pca" % (mod, gc))
                 sc.tl.dendrogram(adata, grouping_var, use_rep="X_pca",linkage_method="average")
                 use_dendrogram=True
             except ValueError: 
                 use_dendrogram=False
 
         sc.settings.figdir  = os.path.join(args.base_figure_dir, mod ,  re.sub(":", "_", grouping_var))
         fname_prefix = "_".join([layer_string, pfx, gc ])
         fname_prefix = re.sub(":", "_", fname_prefix)
+        L.info("Plotting dotplot for modality %s, group %s, and layer %s" % (mod, gc, layer_choice))
         sc.pl.dotplot(adata,
                         var_names=plot_features,
                         groupby=grouping_var,
                         layer=layer_choice,
                         dendrogram=use_dendrogram,
                         save=fname_prefix + '.png',
                         figsize=(24, 5))
+        L.info("Plotting matrix plot for modality %s, group %s, and layer %s" % (mod, gc, layer_choice))
         sc.pl.matrixplot(adata,
                         var_names=plot_features,
                         groupby=grouping_var,
                         dendrogram=use_dendrogram,
                         layer=layer_choice,
                         save=fname_prefix + '.png',
                         figsize=(24, 5))
 
-L.debug("load data")
+
+L.info("Reading in MuData from '%s'" % args.infile)
 mdata = mu.read(args.infile)
 modalities = args.modalities.split(',')
 
-L.debug("load marker file")
-df = pd.read_csv(args.marker_file )
+L.info("Reading in marker file from %s" % args.marker_file)
+df = pd.read_csv(args.marker_file)
 
 pfx = re.sub(".csv", "csv", os.path.basename(args.marker_file))
 # write out the features that are not found in adata var (due to filtering, or incorrect name)
 not_found = [gg for gg in df['feature'] if gg not in mdata.var_names]
 not_found_file = re.sub(".csv", "_features_not_found.txt", os.path.basename(args.marker_file))
 if len(not_found) > 0 :
+    L.info("Writing features from %s that were not found in MuData to file '%s'" % (args.marker_file, not_found_file))
     with open(not_found_file, 'w') as f:
         for item in not_found:
             f.write("%s\n" % item)
             
 # get layer
 try:
     layers = read_yaml(args.layers)
@@ -124,26 +129,24 @@
     adata = mdata
     for gv in group_vars:
         adata.obs[gv] = adata.obs[gv].astype('category')
         main(adata, layer_choice=args.layers, group = gv, pfx = pfx, df = df)
 else:
     # we have multimodal object
     for mod in modalities:
-        print(mod)
         df_sub = df[df['mod'] == mod]
         for gv in group_vars:
             mdata[mod].obs[gv] = mdata.obs.loc[mdata[mod].obs_names,gv].astype('category')
         mdata.update_obs()
         try:
             ll = layers[mod]
         except KeyError:
             ll = [None]
         if len(group_vars) > 0 and ll is not None:
             for gv, layer in product(group_vars, ll):
-                print(gv, layer)
                 main(adata=mdata[mod], 
                     mod=mod,
                     layer_choice = layer,
                     grouping_var=gv, 
                     pfx = pfx,
                     df=df_sub)
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/plot_custom_markers_umap.py` & `panpipes-0.5.0/panpipes/python_scripts/plot_custom_markers_umap.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,16 +42,16 @@
 parser.add_argument("--marker_file",
                     default="Marker_Lists-myeloid.csv",
                     help="comma separateed list of marker_list csvs, one column of gene_ids")
 parser.add_argument("--base_figure_dir", default="figures/",
                     help="figures path")
 
 args, opt = parser.parse_known_args()
-L.info("running with:")
-L.info(args)
+
+L.info("Running with params: %s", args)
 sc.settings.figdir = args.base_figure_dir
 
 # ---- script
 
 def main(adata, mod, layer_choice, df, basis):
     for gc in df['group'].unique():
         # define file name
@@ -61,25 +61,24 @@
         else:
             layer_string = layer_choice
         fname_prefix = "_".join(["_" + mod, layer_string, gc])
         # get features
         fetches = df[df['group'] == gc]['feature']
         plot_features = [gg for gg in fetches if gg in adata.var_names]
         plot_features = list(set(plot_features))
-        L.info("plotting")
-        L.info(plot_features)
+        L.info("Plotting embedding %s of modality %s with layer %s" % (basis, mod, layer_choice))
         sc.settings.figdir  = os.path.join(args.base_figure_dir, mod)
         mu.pl.embedding(adata, basis=basis, layer=layer_choice, color=plot_features, save = fname_prefix + ".png")
 
 
-L.debug("load data")
+L.info("Reading in MuData from '%s'" % args.infile)
 mdata = mu.read(args.infile)
 modalities = args.modalities.split(',')
 
-L.debug("load marker file")
+L.info("Reading in marker file from %s" % args.marker_file)
 df = pd.read_csv(args.marker_file )
 
 # get layer
 try:
     layers = read_yaml(args.layers)
 except AttributeError:
     # this assumes that we have tried to parse a dict and nstead found a string
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/plot_features_scatter.py` & `panpipes-0.5.0/panpipes/python_scripts/plot_features_scatter.py`

 * *Files 17% similar despite different names*

```diff
@@ -35,41 +35,44 @@
 parser.add_argument('--scatters_csv',
                     default='',
                     help='')
 
 parser.set_defaults(verbose=True)
 args, opt = parser.parse_known_args()
 
-L.info(args)
+L.info("Running with params: %s", args)
 
-sc.settings.figdir  = "./scatters/"
-sc.set_figure_params(fontsize=12)
+figdir = "./scatters/"
+if not os.path.exists(figdir):
+    os.mkdir(figdir)
 
+sc.settings.figdir  = figdir
+sc.set_figure_params(fontsize=12)
 
+L.info("Reading in MuData from '%s'" % args.mdata_object)
 mdata = mu.read(args.mdata_object)
 
 layers = read_yaml(args.layers_dict)
 
-
+L.info("Reading in scatter file from '%s'" % args.scatters_csv)
 df = pd.read_csv(args.scatters_csv)
-L.debug(df)
 
 layers = df.applymap(lambda x: get_layer(x,  mdata=mdata, layers=layers))
-L.info(layers)
 
 for idx in range(df.shape[0]):
     features_list = df.iloc[idx,:].tolist()
     # convert NAs and X to None
     features_list = [x  if pd.notna(x) else None for x in features_list]
     
     layers_list = layers.iloc[idx,:].tolist()
     # exclude any Nones to get the layers list to be the same length as features
     layers_list = [x for idx, x in enumerate(layers_list) if features_list[idx] is not None]
     
     fname = os.path.join("scatters", "_".join([x for x in features_list if x is not None]) + ".png")
+    L.info("Plotting scatters for features %s on layers %s" % (features_list,layers_list))
     plot_scatters(mdata, features_list, layers_list)
     # plt.legend(bbox_to_anchor=(1.04,0.5), loc="center left", borderaxespad=0)
     plt.subplots_adjust(right=0.85)
     plt.savefig(fname, bbox_inches="tight")
 
 L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/plot_pca.py` & `panpipes-0.5.0/panpipes/python_scripts/plot_pca.py`

 * *Files identical despite different names*

### Comparing `panpipes-0.4.1/panpipes/python_scripts/plot_qc_spatial.py` & `panpipes-0.5.0/panpipes/python_scripts/plot_qc_spatial.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,25 +43,25 @@
                     default="None",
                     help="variables to group the cells by")
 
 
 
 args, opt = parser.parse_known_args()
 
-L.info("running with args:")
-L.info(args)
+L.info("Running with params: %s", args)
 
 figdir = args.figdir
 
-if not os.path.exists(figdir):
-    os.mkdir(figdir)
+# if not os.path.exists(figdir):
+#     os.mkdir(figdir)
 
 sc.settings.figdir = figdir
 sc.set_figure_params(scanpy=True, fontsize=14, dpi=300, facecolor='white', figsize=(5,5))
 
+L.info("Reading in MuData from '%s'" % args.input_mudata)
 mdata = mu.read(args.input_mudata)
 spatial = mdata.mod['spatial']
 
 input_data = os.path.basename(args.input_mudata)
 pattern = r"_filtered.h5(.*)"
 match = re.search(pattern, input_data)
 if match is None:
@@ -94,42 +94,47 @@
     
     # check if in adata.obs:
     if metric in spatial.obs.columns: 
         # check that it's a numeric column, so that it can be plotted: 
         if metric not in spatial.obs._get_numeric_data().columns:
             L.warning("Variable '%s' not numerical in adata.obs, will not be plotted" % metric)
         else:
+            L.info("Creating violin plot for '%s' of .obs" % metric)
             if group_var is None: 
                 sc.pl.violin(spatial, keys = metric, xlabel = metric+ " in .obs",
                             save =  "_obs_" + metric+ "_" + "."+sprefix + ".png", show = False)
             
             else: #plot violin for each group
                 for group in group_var: 
                     sc.pl.violin(spatial, keys = metric,groupby = group, xlabel = group + ", "+ metric+ " in .obs",
                             save = "_obs_" + metric+ "_" + group+ "."+sprefix +".png", show = False)
             #plot spatial 
+            L.info("Creating spatial embedding plot for '%s' of .obs" % metric)
             sc.pl.embedding(spatial,basis="spatial", color = metric, save = "_spatial_" + metric + "."+sprefix +".png", show = False)
 
     #check if in adata.var: 
     if metric in spatial.var.columns:
         
         if metric not in spatial.var._get_numeric_data().columns:
             L.warning("Variable '%s' not numerical in adata.var, will not be plotted" % metric)
         else:
             # plot violins 
+            L.info("Creating violin plot for '%s' of .var" % metric)
             ax = sns.violinplot(
                     data=spatial.var[[metric]],
                     orient='vertical', 
                 )
             ax.set(xlabel=metric+ " in .var" )
             ax.figure.savefig(figdir + "/" +"violin_var_" + metric + "."+sprefix +".png")
 
 
 
 if args.spatial_filetype == "vizgen":
+    L.info("Creating histograms for 'Total transcripts per cell', 'Unique transcripts per cell', 'Transcripts per FOV', and 'Volume of segmented cells'")
+
     fig, axs = plt.subplots(1, 4, figsize=(15, 4))
 
     axs[0].set_title("Total transcripts per cell")
     sns.histplot(
         spatial.obs["total_counts"],
         kde=False,
         ax=axs[0],
@@ -140,15 +145,15 @@
         spatial.obs["n_genes_by_counts"],
         kde=False,
         ax=axs[1],
     )
 
     axs[2].set_title("Transcripts per FOV")
     sns.histplot(
-        spatial.obs.groupby("fov").sum()["total_counts"],
+        spatial.obs.groupby('fov')[['total_counts']].sum(),
         kde=False,
         ax=axs[2],
     )
 
     axs[3].set_title("Volume of segmented cells")
     sns.histplot(
         spatial.obs["volume"],
@@ -156,12 +161,12 @@
         ax=axs[3],
     )
 
     plt.tight_layout()  # Ensures proper spacing between subplots
     #plt.savefig("merfish_histo.png", dpi=300)
     plt.savefig(figdir + "/histograms."+sprefix +".png", dpi=300)  # Adjust dpi as needed
     plt.close()  # Close the figure to free up memory
-
-            
+     
+           
 
 L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/plot_scanpy_markers.py` & `panpipes-0.5.0/panpipes/python_scripts/plot_scanpy_markers.py`

 * *Files 20% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                     help="figures path")
 parser.add_argument("--n", default=None,
                     help="number of genes to plot per cluster, default=None will plot all genes in your marker_file")
 
 
 
 args, opt = parser.parse_known_args()
-L.info(args)
+L.info("Running with params: %s", args)
 
 sc.settings.figdir = args.figure_prefix
 
 # script
 
 def calc_dendrogram(adata, group_col):
     if len(adata.obs[group_col].cat.categories) > 5:
@@ -67,72 +67,92 @@
             incl_dendrogram = False
     else:
         incl_dendrogram = False
     return incl_dendrogram
 
 
 def do_plots(adata, mod, group_col, mf, n=10, layer=None):
-    L.debug("check layers")
     # get markers for plotting
+    L.info("Subsetting on markers with avg logFC > 0")
     mf = mf[mf['avg_logFC'] > 0]
+    L.info("Extracting top markers for each cluster")
+    mf['scores'] = pd.to_numeric(mf["scores"])
     df = mf.groupby(group_col).apply(lambda x: x.nlargest(n, ['scores'])).reset_index(drop=True)
     marker_list={str(k): list(v) for k,v in df.groupby(group_col)["gene"]}
     # add cluseter col to obs
     # check whether a dendrogram is computed/
     incl_dendrogram = calc_dendrogram(adata, group_col)
-    L.info("start plotting")
+    L.info("Plotting stacked violin")
     sc.pl.stacked_violin(adata,
                 marker_list,
                 groupby=group_col,
                 layer=layer,
                 save = '_top_markers'+ mod +'.png',
                 dendrogram=incl_dendrogram,
                 # figsize=(24, 5)
                 )
+    L.info("Plotting matrix plot")
     sc.pl.matrixplot(adata,
                     marker_list,
                     groupby=group_col,
                     save=  '_top_markers'+ mod +'.png',
                     dendrogram=incl_dendrogram,
                     figsize=(24, 5))
+    L.info("Plotting dotplot")
     sc.pl.dotplot(adata,
                 marker_list,
                 groupby=group_col,
                 save=  '_top_markers'+ mod +'.png',
                 dendrogram=incl_dendrogram,
                 figsize=(24, 5))
+    L.info("Plotting heatmap")
     sc.pl.heatmap(adata,
                 marker_list,
                 groupby=group_col,
                 save=  '_top_markers'+ mod +'.png',
                 dendrogram=incl_dendrogram,
                 # figsize=(24, 5)
                 )
 
 
 # read data
+L.info("Reading in MuData from '%s'" % args.infile)
 mdata = mu.read(args.infile)
 
 if type(mdata) is AnnData:
     adata = mdata
     # main function only does rank_gene_groups on X, so 
 elif type(mdata) is mu.MuData and args.modality is not None:
     adata = mdata[args.modality]    
 else:
-    sys.exit('if inputting a mudata object, you need to specify a modality')
-    
+    L.error("If the input is a MuData object, a modality needs to be specified")
+    sys.exit('If the input is a MuData object, a modality needs to be specified')
 
-L.info("load marker file")
+L.info("Loading marker information from '%s'" % args.marker_file)
 mf = pd.read_csv(args.marker_file, sep='\t' )
 mf[args.group_col] = mf['cluster'].astype('category')
+L.info(f"Dimensions of the marker file are: {mf.shape[0]} rows and {mf.shape[1]} columns.")
 
-# get layer
-adata.obs[args.group_col] = mdata.obs[args.group_col]
-do_plots(adata,
-         mod=args.modality, 
-         group_col=args.group_col,
-         mf=mf,
-         layer=args.layer, 
-         n=int(args.n))
+L.info("Top 5 rows of the marker file:")
+L.info("\n" + mf.head().to_string())
+
+L.info(mf.dtypes)
+mf['scores'] = pd.to_numeric(mf['scores'], errors='coerce')
+print(mf['scores'].isna().sum())
+mf.dropna(subset=['scores'], inplace=True)
+L.info(f"Dimensions of the marker file are: {mf.shape[0]} rows and {mf.shape[1]} columns.")
+
+ch=mf[mf['avg_logFC'] > 0]
+if mf.shape[0]>=2:
+    # get layer
+    adata.obs[args.group_col] = mdata.obs[args.group_col]
+    do_plots(adata,
+            mod=args.modality, 
+            group_col=args.group_col,
+            mf=mf,
+            layer=args.layer, 
+            n=int(args.n))
+else:
+    L.info("No markers were detected with positive LogFC, no plotting is done")
 
 L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/plot_umaps_batch_correct.py` & `panpipes-0.5.0/panpipes/python_scripts/plot_umaps_batch_correct.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,69 +29,71 @@
 parser.add_argument("--fig_dir")
 parser.add_argument("--batch_dict", default=None)
 parser.add_argument("--qc_dict", default=None)
 
 args, opt = parser.parse_known_args()
 
 
-L.info(args)
+L.info("Running with params: %s", args)
 palette_choice = ['#1f77b4', '#ff7f0e', '#2ca02c', '#d62728', '#9467bd', '#8c564b', '#e377c2', '#7f7f7f', '#bcbd22', '#17becf']
 # cmap_choice = "BuPu" # previous default = "viridis"
 bupu = cm.get_cmap('BuPu', 512)
 cmap_choice= ListedColormap(bupu(np.linspace(0.1, 1, 256)))
+dpi_use = 400 # previous default of 300 made the plots look blurry with high cell numbers (200k+)
 
 
 # load metadata
+L.info("Reading in cell metadata from '%s'" % args.cell_meta_df)
 cell_meta_df = pd.read_csv(args.cell_meta_df, index_col=0)
+L.info("Reading in UMAP coordinates from '%s'" % args.combined_umaps_tsv)
 umaps_df = pd.read_csv(args.combined_umaps_tsv, sep='\t', index_col=0)
 umaps_df = pd.merge(umaps_df, cell_meta_df, left_index=True, right_index=True)
 
+L.info("Reading in batch dictionary from '%s" % args.batch_dict)
 batch_dict = read_yaml(args.batch_dict)
 
 # parse the qc dict
 qc_dict = args.qc_dict
 if isinstance(args.qc_dict, dict):
     qc_dict = args.qc_dict
 else:
     qc_dict = read_yaml(args.qc_dict) 
 
 # extract the grouping vars which are expected to be categorical
 grpvar = [x.replace (" " ,"") for x in qc_dict['grouping_var'].split(",")]
 grpvar = [value for value in grpvar if value in cell_meta_df.columns] 
 del qc_dict['grouping_var']
-L.info("additional grouping vars:")
 # merge with the batch columns 
 from itertools import chain
 all_grpvar = list(batch_dict.values()) + [grpvar]
 # unnest the list
 grpvar = list(set(chain(*all_grpvar)))
-L.info(grpvar)
+L.info("Grouping vars used: %s" % grpvar)
 
 # modality level metrics
 # remove metrics from keys
 qc_dict = {re.sub("_metrics", "", k) : v for k, v in qc_dict.items()}
 
 # split the comma sep string of metrics (and remove Nones)
 qc_dict = {k: v.split(',') for k, v in qc_dict.items() if v is not None}
 # remove white spaces from list of the dictionary
 qc_dict ={i: [a.strip(" ") for a in j ] for i,j in qc_dict.items()}
 # make sure mod: prefaces each metric
 qc_dict = {k: [k + ":" + vi if ":" not in vi else vi for vi in v ]  for k, v in qc_dict.items()}
-L.info("additional qc vars:")
-L.info(qc_dict)
+L.info("Additional QC vars: %s" % qc_dict)
 
 
 # do plots
 for mod in umaps_df['mod'].unique():
     # create directory if it doesn't exist
     if os.path.exists(os.path.join(args.fig_dir, mod)) is False:
         os.mkdir(os.path.join(args.fig_dir, mod))
-    L.info("plotting modality: %s" % mod)
+    L.info("Plotting modality: %s" % mod)
     plt_df = umaps_df[umaps_df['mod'] == mod].copy()
-    pointsize = 10000 / plt_df.shape[0]
+    pointsize = 100000 / plt_df.shape[0]
     plt_df["method"] = plt_df["method"].astype("category")
     # put none at the top of the list
     if mod != "multimodal":
         umaps_methods_list = plt_df['method'].cat.categories.tolist()
         umaps_methods_list.insert(0, umaps_methods_list.pop(umaps_methods_list.index("none")))
         plt_df['method'] = plt_df['method'].cat.reorder_categories(umaps_methods_list, ordered=True)
     #  get grouing vars
@@ -102,26 +104,26 @@
             # this means no batch correction was run. 
             columns = set([mod +":"+ g for g in grpvar])
     else:
         columns = grpvar
     # keep only the columns that are actually in plt_df
     columns = [cl for cl in columns if cl in plt_df.columns ]
     for col in columns:
-        L.info("plotting grouping var %s" % col)
+        L.info("Plotting grouping var %s" % col)
         # make sure everything is a category so that when they get plotted it's the same color
         plt_df[col] = plt_df[col].astype(str).astype('category')
         plt_df = plt_df.sample(frac=1).reset_index(drop=True)
         #plt_df = plt_df.sort_values(by="umap_1")
         g = sns.FacetGrid(plt_df, col="method", col_wrap=3, sharex=False, sharey=False)
         g = (g.map(sns.scatterplot, "umap_1", "umap_2", col, s=pointsize, linewidth=0))
-        g.add_legend() 
+        plt.legend(loc = 'center left', bbox_to_anchor = (1, 0.5), markerscale = 20)
         g.savefig(os.path.join(args.fig_dir, mod, "umap_method_" + str(col) + ".png"))
         fig, ax = batch_scatter_two_var(plt_df, "method", col, palette_choice=palette_choice)
         if fig is not None:
-            fig.savefig(os.path.join(args.fig_dir, mod,  "umap_method_facet_" + str(col) + ".png"), dpi=300)
+            fig.savefig(os.path.join(args.fig_dir, mod,  "umap_method_facet_" + str(col) + ".png"), dpi=dpi_use)
         plt.clf()
 
     ncats  = len(plt_df['method'].unique())
     if ncats > 4:
         ncols=4
         nrows = int(np.ceil(ncats/4))
     else:
@@ -143,15 +145,15 @@
             for qc in qcmetrics:
                 fig, axes = plt.subplots(ncols=ncols, nrows=nrows, figsize=(5*ncols,4*nrows))
                 if nrows > 1 or ncols > 1:
                     axes = axes.ravel()
                 else:
                     axes=[axes]
                 if pd.api.types.is_numeric_dtype(plt_df[qc]):
-                    L.info("plotting qc var (numeric) %s" % qc)
+                    L.info("Plotting QC var (numeric) %s" % qc)
                     for idx, mm in enumerate(plt_df['method'].cat.categories):
                         im = axes[idx].scatter(data=plt_df[plt_df['method']== mm], 
                                         x="umap_1",
                                         y="umap_2",
                                         c=qc, 
                                         s=pointsize,
                                         cmap=cmap_choice)
@@ -161,23 +163,23 @@
                     for idx2 in range(idx,ncols*nrows):
                         axes[idx2].axis('off')
                     if pd.api.types.is_numeric_dtype(plt_df[qc]):
                         fig.subplots_adjust(top=0.925,right=0.8)
                         cbar_ax = fig.add_axes([0.85, 0.35, 0.025, 0.35])
                         fig.colorbar(im, cbar_ax)
                     fig.suptitle(qc)
-                    plt.savefig(os.path.join(args.fig_dir, mod , "umap_method_" + qc + ".png"), dpi = 300)
+                    plt.savefig(os.path.join(args.fig_dir, mod , "umap_method_" + qc + ".png"), dpi = dpi_use)
                     plt.clf()
                 else:
                     # this is a categorical colored plot
                     plt_df[qc] = plt_df[qc].fillna('nan')
                     if len(plt_df[qc].unique()) < 40:
-                        L.info("plotting qc var (categorical) %s"%qc)
+                        L.info("Plotting QC var (categorical) %s"%qc)
                         g = sns.FacetGrid(plt_df, col="method", col_wrap=3, sharex=False, sharey=False)
                         g = (g.map(sns.scatterplot, "umap_1", "umap_2", qc, s=pointsize, linewidth=0))
-                        g.add_legend() 
-                        g.savefig(os.path.join(args.fig_dir, mod, "umap_method_" + qc + ".png"), dpi = 300)
+                        plt.legend(loc = 'center left', bbox_to_anchor = (1, 0.5), markerscale = 20)
+                        g.savefig(os.path.join(args.fig_dir, mod, "umap_method_" + qc + ".png"), dpi = dpi_use)
                         plt.clf()
                     else:
-                        L.info('skipping plot as too many categorys %s' % qc )
+                        L.info('Skipping plot as too many categories %s' % qc )
 
-L.info('done')
+L.info('Done')
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/plot_variables_umaps.py` & `panpipes-0.5.0/panpipes/python_scripts/plot_variables_umaps.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,80 +41,79 @@
                     help="continuous values within mdata.obs")
 parser.add_argument("--base_figure_dir", default="figures/",
                     help="figures path")
 parser.add_argument("--fig_suffix", default="variables.png",
                     help="figures path")
 args, opt = parser.parse_known_args()
 
-L.info("running with:")
-L.info(args)
+
+L.info("Running with params: %s", args)
 # args = argparse.Namespace(infile='../run_clustering_mm/mdata_clustered.h5mu',
 #  basis_dict="{'prot': ['X_umap', 'X_pca']}", 
 #  base_figure_dir='./')
 
 # ---------
 def main(adata, mod, plot_features,  basis, fig_suffix):
     # define file name
     fname_prefix = "_".join(["_" + mod,  fig_suffix])
     # get features
-    L.info("plotting")
-    L.info(plot_features)
     sc.settings.figdir  = os.path.join(args.base_figure_dir, mod)
     plot_features = [pf for pf in plot_features if pf in mdata.obs.columns]
     pointsize = 120000 / adata.shape[0]
+    L.info("Plotting embedding %s for modality %s coloured by %s" % (basis, mod, plot_features))
     mu.pl.embedding(adata, basis=basis, color=plot_features, size=pointsize, save = fname_prefix + ".png")
 
 
-L.debug("load data")
+L.info("Reading in MuData from '%s'" % args.infile)
 mdata = mu.read(args.infile)
 
 
 # get bases
 basis_dict = dictionary_stripper(read_yaml(args.basis_dict))
 
 if args.categorical_variables is not None:
     cat_vars = dictionary_stripper(read_yaml(args.categorical_variables))
     
     uniq_discrete = list(set(chain(*cat_vars.values())))
     # make sure they are categories
     mdata.obs[uniq_discrete] = mdata.obs[uniq_discrete].apply(lambda x: x. astype('category'))
 else:
+    L.warning("No categorical variables were provided")
     cat_vars = {}
 
 
 if args.continuous_variables is not None:
     try:
         cont_vars = dictionary_stripper(read_yaml(args.continuous_variables))
     except AttributeError:
         # this assumes that we have tried to parse a dict and nstead found a string
         # there is probably a better solution
         cont_vars = args.continuous_variable_dict
 else:
+    L.warning("No continuous variables were provided")
     cont_vars = {}
 
 
 
 
 # we have multimodal object
 params_dict = {}
 for mod in ['rna', 'prot', 'atac', 'multimodal']:
     params_dict['mod' ] = mod
     try:
         basis_list = basis_dict[mod]
     except KeyError:
-        L.info("no basis given for mod: %s, no plot's produced" % mod)
+        L.warning("No basis given for mod: %s, no plot's produced" % mod)
         continue
     params_dict['plot_features'] = []
     if mod in cat_vars.keys():
         params_dict['plot_features'] = cat_vars[mod]
     if mod in cont_vars.keys():
-        params_dict['plot_features'] = params_dict['plot_features'] +  cont_vars[mod]
+        params_dict['plot_features'] = params_dict['plot_features'] + cont_vars[mod]
     params_dict['fig_suffix'] = args.fig_suffix
-    L.info("plotting with params")
-    L.info(params_dict)
     if len(basis_list) > 0:
         for basis in basis_list:
             main(adata=mdata, basis = mod + ":" + basis, **params_dict)
 
 
 
 L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/refmap_generatescanvi.py` & `panpipes-0.5.0/panpipes/python_scripts/refmap_generatescanvi.py`

 * *Files identical despite different names*

### Comparing `panpipes-0.4.1/panpipes/python_scripts/refmap_plot_umaps.py` & `panpipes-0.5.0/panpipes/python_scripts/refmap_plot_umaps.py`

 * *Files identical despite different names*

### Comparing `panpipes-0.4.1/panpipes/python_scripts/refmap_scib.py` & `panpipes-0.5.0/panpipes/python_scripts/refmap_scib.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,66 +35,71 @@
                     default=None,
                     help='string of column in query anndata/mudata containing cluster assignments you want to use to calculate the metrics (ARI/NMI)')
 parser.add_argument('--outdir', default=None,
                     help='directory to save the data to')
 
 args, opt = parser.parse_known_args()
 
-L.info(args)
+L.info("Running with params: %s", args)
 
 
 if args.covariate is not None:
     covariates_use = args.covariate.split(",")
     covariates_use = [a.strip() for a in covariates_use]
 else:
-    sys.exit("i don't have covariates to calculate metrics on")
+    L.error("Covariates need to be specified.")
+    sys.exit("Covariates need to be specified.")
 
 
 repuse = str(args.repuse)
 
+L.info("Reading in query data from '%s'" % args.query_data)
 mdata = mu.read(args.query)
+
 if type(mdata) is mu.MuData:
     if "rna" not in mdata.mod.keys():
-        sys.exit("we only support querying using RNA but your mdata doesn't contain rna")
+        L.error("Modality 'rna' could not be found in MuData '%s'. We only support querying using RNA." % args.query_data)
+        sys.exit("Modality 'rna' could not be found in MuData '%s'. We only support querying using RNA." % args.query_data)
     else:
         input_adata = mdata["rna"].copy()
 del mdata
 
 
 adata_query = input_adata[input_adata.obs['is_reference'] == 'Query'].copy()
-L.info("repuse is %s" %(repuse))
+L.info("Repuse is %s" %(repuse))
 if repuse not in adata_query.obsm.keys():
-    sys.exit("the latent representation is not in the obsm.keys of this query")
+    L.error("The latent representation '%s' could not be found in the obsm.keys of query '%s'" % (repuse, args.query_data))
+    sys.exit("The latent representation '%s' could not be found in the obsm.keys of query '%s'" % (repuse, args.query_data))
 
-L.info("query is:")
+L.info("The query AnnData is:")
 print(adata_query)
 
-L.info("Calculating scib metrics using ground truth covariates:")
+L.info("Calculating scib metrics using ground truth covariates: ")
 print(covariates_use)
 
 if args.cluster_key is None:
     cluster_key = "leiden_" + repuse 
-    L.info("you didn't specify cluster_key, so i'm using %s " % cluster_key)
+    L.warning("No cluster key specified. Using %s " % cluster_key)
 else:
     cluster_key = str(args.cluster_key)
     L.info("cluster_key used is: %s" %cluster_key)
 
+L.info("Calculating scIB metrics")
 results = {}
 for labelk in covariates_use:
     m={"ASW_scaled":scib.metrics.silhouette(adata_query, labelk, repuse, metric='euclidean', scale=True),
         "ARI":scib.metrics.ari(adata_query, label_key=labelk, cluster_key=cluster_key), #predictions or leiden clustering
         "NMI":scib.metrics.nmi(adata_query, label_key=labelk, cluster_key=cluster_key),
         "graph_connectivity":scib.metrics.graph_connectivity(adata_query, labelk)}    
     if args.batch_key is not None:
         m["clisi_graph_embed"]= scib.me.clisi_graph(adata_query, label_key=labelk, type_="knn", batch_key=str(args.batch_key))
 
     results[labelk] = m
 
 file_name= os.path.splitext(os.path.basename(args.query).replace("query_to_reference_", "").replace(".h5mu", ""))[0]
 #"query_to_reference_" + model_name + "_" + latent_choice + ".h5mu"
-L.info("saving file output")
-file_out = os.path.join(args.outdir,("scib.query_"+ file_name+".csv"))
-print(file_out)
+file_out = os.path.join(args.outdir,("scib.query_"+ file_name+".tsv"))
 #save file to txt
 pres = pd.DataFrame.from_dict(results,orient='index')
+L.info("Saving output to tsv file '%s'" % file_out)
 pres.to_csv(file_out, sep="\t")
-L.info("Finished scib")
+L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/refmap_scvitools.py` & `panpipes-0.5.0/panpipes/python_scripts/refmap_scvitools.py`

 * *Files 9% similar despite different names*

```diff
@@ -58,115 +58,126 @@
                     help="neighbor metric, e.g. euclidean or cosine")
 parser.add_argument('--outfile',default=None,
                     help="file where to save umap")
 
 args, opt = parser.parse_known_args()
 sc.settings.figdir = "figures/"
 sc.set_figure_params(figsize=(8, 6), dpi=300) 
-L.info("running with args:")
 args.predict_rf = check_for_bool(args.predict_rf)
 args.impute_proteins = check_for_bool(args.impute_proteins)
-L.info(args)
+
+L.info("Running with params: %s", args)
 
 threads_available = multiprocessing.cpu_count()
 
 # load parameters
 params = read_yaml("pipeline.yml")
 query_data = os.path.basename(args.query_data)
 
 reference_architecture = str(args.reference_architecture)
 
 
-
+L.info("Reading in query data from '%s'" % args.query_data)
 mdata = mu.read(args.query_data)
+
 if type(mdata) is mu.MuData:
     if "rna" not in mdata.mod.keys():
-        sys.exit("we only support querying using RNA but your mdata doesn't contain rna")
+        L.error("Modality 'rna' could not be found in MuData '%s'. We only support querying using RNA." % args.query_data)
+        sys.exit("Modality 'rna' could not be found in MuData '%s'. We only support querying using RNA." % args.query_data)
     else:
         adata_query = mdata["rna"].copy()
         if "prot" in mdata.mod.keys() and reference_architecture=="totalvi":
             if X_is_raw(mdata['prot']):
+                L.info("Using raw protein data from mdata.mod['prot'].X")
                 X_array = mdata['prot'].X.copy()
             elif "raw_counts" in mdata['prot'].layers.keys(): 
+                L.info("Using raw protein data from mdata.mod['prot'].layers['raw_counts']")
                 X_array = mdata['prot'].layers['raw_counts'].copy()
         
         X_df = pd.DataFrame(X_array.todense(), index=mdata['prot'].obs_names, columns=mdata['prot'].var_names)
         if X_df.shape[0] == adata_query.X.shape[0]:
-            L.info("adding protein_expression to obsm")
+            L.info("Adding raw protein expression to obsm")
             #check the obs are in the correct order
             X_df = X_df.loc[adata_query.obs_names,:]
             adata_query.obsm['protein_expression'] = X_df 
         else:
-            L.error("dimensions do not match, cannot create the raw obsm counts in query")
+            L.error("Dimension 0 of protein expression matrix and RNA expression matrix do not match. Cannot create the raw obsm counts in query.")
+            sys.exit("Dimension 0 of protein expression matrix and RNA expression matrix do not match. Cannot create the raw obsm counts in query.")
 else:
     adata_query = mdata.copy()
 
-L.info("this is your query anndata")
+L.info("The query AnnData is:")
 print(adata_query)
 
+L.info("Saving raw counts to adata.layers['counts']")
 if "counts" not in adata_query.layers.keys():
     if "raw_counts" in adata_query.layers.keys():
         adata_query.layers["counts"] = adata_query.layers["raw_counts"].copy()
     elif X_is_raw(adata_query):
         adata_query.layers["counts"] = adata_query.X.copy()
     else:
         raise AttributeError("raw counts not found in query, \
                         store in either X or in 'counts/raw_counts' layer")
 
 
 if reference_architecture in ['totalvi','scvi','scanvi']:
-    L.info("running using %s" % reference_architecture)
+    L.info("Running using %s" % reference_architecture)
 else:
-    sys.exit(" i don't recognise this architecture : %s") %reference_architecture
+    L.error("Architecture '%s' could not be found. The following architectures are available: 'totalvi', 'scvi', 'scanvi'" % reference_architecture)
+    sys.exit("Architecture '%s' could not be found. The following architectures are available: 'totalvi', 'scvi', 'scanvi'" % reference_architecture)
 
 reference_path = args.reference_path
 if not os.path.exists(reference_path):
-    L.info("The reference path you provided does not exist")
-    sys.exit("The reference path you provided does not exist")
+    L.info("The provided reference path '%s does not exist" % reference_path)
+    sys.exit("The provided reference path '%s' does not exist" % reference_path)
 else:
     reference_path = os.path.dirname(reference_path)
-    L.debug("Reference path: %s" % reference_path)
 
 train_kwargs = {}
 if params["training_plan"][reference_architecture] is not None:
     train_kwargs = params["training_plan"][reference_architecture]
     if train_kwargs["max_epochs"] is not None:
         max_epochs = train_kwargs["max_epochs"]
         del train_kwargs["max_epochs"]
     else:
         max_epochs = 200
 else:
     max_epochs = 200
     train_kwargs = {'weight_decay': 0.0}
 
+print(train_kwargs)
 
 if reference_architecture=="scvi":
+    L.info("Running scVI")
     scvi.model.SCVI.prepare_query_anndata(adata_query, reference_path)
     vae_q = scvi.model.SCVI.load_query_data(
     adata_query,
     reference_path)
     latent_choice= "X_scvi"
     vae_q.train(max_epochs= max_epochs , plan_kwargs=train_kwargs)
+    L.info("Saving latent to .obsm['X_scvi']")
     adata_query.obsm["X_scvi"] = vae_q.get_latent_representation()
     
 
 if reference_architecture=="scanvi":
     # Notice that adata_query.obs["labels_scanvi"] does not exist. 
     # The load_query_data method detects this and fills it in adata_query with the unlabeled category (here "Unknown").
+    L.info("Running scANVI")
     scvi.model.SCANVI.prepare_query_anndata(adata_query, reference_path)
     vae_q = scvi.model.SCANVI.load_query_data( 
     adata_query,
     reference_path)
     latent_choice= "X_scanvi"
     #vae_q.train(**train_kwargs) this doesn't work anymore cause max_epochs is not recognised as part of the plan kwargs
     vae_q.train(max_epochs= max_epochs , plan_kwargs=train_kwargs)
+    L.info("Saving latent to .obsm['X_scanvi'] and predictions to .obs['predictions']")
     adata_query.obsm["X_scanvi"] = vae_q.get_latent_representation()
     adata_query.obs["predictions"] = vae_q.predict()
     if args.query_celltype is not None:
-        L.info("Query has celltypes in column %s, i will plot what predictions look like from scanvi model" % args.query_celltype)
+        L.info("Plotting predictions from scANVI model")
         df = adata_query.obs.groupby([str(args.query_celltype), "predictions"]).size().unstack(fill_value=0)
         norm_df = df / df.sum(axis=0)
 
         plt.figure(figsize=(8, 8))
         _ = plt.pcolor(norm_df)
         _ = plt.xticks(np.arange(0.5, len(df.columns), 1), df.columns, rotation=90)
         _ = plt.yticks(np.arange(0.5, len(df.index), 1), df.index)
@@ -176,32 +187,33 @@
         file_name = "SCANVI_predicted_vs_observed_labels_query_data"
         plt.savefig(os.path.join("figures/", file_name + ".png"))
         
 if reference_architecture=="totalvi":
     # temporary fix is disabled for now, need to modify to allow to fix query to match reference
     fix_query = False
     if fix_query:
-        L.info(" will do some manipulation of query data to make it match to referece structure")
         if args.adata_reference is not None:
             reference_data = os.path.basename(args.adata_reference)
             mdata=mu.read(args.adata_reference)
             if type(mdata) is MuData:
                 if "rna" not in mdata.mod.keys():
-                    sys.exit("we only support querying using RNA but your mdata doesn't contain rna")
+                    L.error("Modality 'rna' could not be found in MuData '%s'. We only support querying using RNA." % args.adata_reference)
+                    sys.exit("Modality 'rna' could not be found in MuData '%s'. We only support querying using RNA." % args.adata_reference)
                 else:
                     adata_ref = mdata["rna"].copy()
                     adata_ref.obsm = mdata.obsm.copy()
                     adata_ref.obsp = mdata.obsp.copy()
             else:
                 adata_ref = mdata.copy()
             del mdata
             # match query and reference vars
             
             #adata_query.layers["counts"] = adata_query.X.copy()#already taken care of 
             # are the following necessary?
+            L.info("Normalizing query data")
             sc.pp.normalize_total(adata_query, target_sum=1e4)
             sc.pp.log1p(adata_query)
             adata_query.raw = adata_query
             # subset to reference vars
             adata_query = adata_query[:, adata_ref.var_names].copy()
             
             adata_query.obs["celltype.l2"] = "Unknown"
@@ -243,39 +255,42 @@
             # else: 
             #     sys.exit("I need var names from reference to make sure query has overlap")    
 
             # if args.reference_prot_assay is not None:
             #     L.info("name of obsm slot for reference is: %i" % args.reference_prot_assay)
             #     pname = args.reference_prot_assay
             sys.exit("need a reference dataset to check for matching query entries")        
-        
+    
+    L.info("Running totalVI")
     scvi.model.TOTALVI.prepare_query_anndata(adata_query, reference_path)
     vae_q = scvi.model.TOTALVI.load_query_data(
     adata_query,
     reference_path,
     freeze_expression=True)
     latent_choice= "X_totalvi"
     vae_q.train(max_epochs= max_epochs , plan_kwargs=train_kwargs)
+    L.info("Saving latent to .obsm['X_totalvi']")
     adata_query.obsm["X_totalvi"] = vae_q.get_latent_representation()
     #remove this after finishing
     adata_query.write(os.path.join( "query_temp_check_totvi.h5ad"))
         
     if args.predict_rf :
-        L.info("predicting celltypes")
+        L.info("Predicting cell types")
         predictions = (
            vae_q.latent_space_classifer_.predict(
             adata_query.obsm["X_totalvi"]
             )
         )
+        L.info("Saving predictions to .obs['predictions']")
         adata_query.obs["predictions"] = predictions
         #remove this after finishing
         adata_query.write(os.path.join( "query_temp_check_predictions_totvi.h5ad"))
     
         if args.query_celltype is not None:
-            L.info("Query has celltypes in column %s, i will plot what predictions look like from totalvi model" % args.query_celltype)
+            L.info("Plotting predictions from totalVI model")
             df = adata_query.obs.groupby([str(args.query_celltype), "predictions"]).size().unstack(fill_value=0)
             norm_df = df / df.sum(axis=0)
 
             plt.figure(figsize=(8, 8))
             _ = plt.pcolor(norm_df)
             _ = plt.xticks(np.arange(0.5, len(df.columns), 1), df.columns, rotation=90)
             _ = plt.yticks(np.arange(0.5, len(df.index), 1), df.index)
@@ -287,28 +302,31 @@
         
     
 L.info("Mapped Query to Reference, now some utilities")
 
 
 if args.adata_reference is not None:
     reference_data = os.path.basename(args.adata_reference)
+    L.info("Reading in data from '%s'" % args.adata_reference)
     mdata=mu.read(args.adata_reference)
     if type(mdata) is MuData:
         if "rna" not in mdata.mod.keys():
-            sys.exit("we only support querying using RNA but your mdata doesn't contain rna")
+            L.error("Modality 'rna' could not be found in MuData '%s'. We only support querying using RNA." % args.adata_reference)
+            sys.exit("Modality 'rna' could not be found in MuData '%s'. We only support querying using RNA." % args.adata_reference)
         else:
             adata_ref = mdata["rna"].copy()
             adata_ref.obsm = mdata.obsm.copy()
             adata_ref.obsp = mdata.obsp.copy()
     else:
         adata_ref = mdata.copy()
 
     adata_ref.obs.loc[:, 'is_reference'] = 'Reference'
     adata_query.obs.loc[:, 'is_reference'] = 'Query'
     #expect the batch to be always encoded as `batch` in both Q and R
+    L.info("Concatenating query and reference data")
     adata_full = ad.concat( [adata_ref,adata_query])
     # add param to decide if to recompute the total embedding or to recalc the embedding
     #if "X_totalvi" not in adata_ref.obsm.keys():
     adata_full.obsm[latent_choice] = vae_q.get_latent_representation(adata_full)
     
     if args.impute_proteins: 
         if args.transform_batch is not None:
@@ -316,59 +334,64 @@
         else:
             transform_batch = None
         normX, protein = vae_q.get_normalized_expression(
             adata_full,
             n_samples=25,
             return_mean=True,
             transform_batch= transform_batch) 
+        L.info("Saving denoised data to .obsm['totalvi_denoised_rna'] and .obsm['totalvi_denoised_protein']")
         adata_full.obsm["totalvi_denoised_rna"], adata_full.obsm["totalvi_denoised_protein"] = normX, protein    
 
     if reference_architecture=="scanvi":
         full_predictions = vae_q.predict(adata_full)
-        L.warn("Acc: {}".format(np.mean(full_predictions == adata_full.obs.celltype)))
+        L.warning("Acc of scANVI predictions: {}".format(np.mean(full_predictions == adata_full.obs.celltype)))
         adata_full.obs["predictions"] = full_predictions
 else:
     adata_query.obs.loc[:, 'is_reference'] = 'Query'
     adata_full = adata_query.copy()
 
 if int(args.neighbors_n_pcs) > adata_full.obsm[latent_choice].shape[1]:
-    L.warn("N PCs is larger than %i dimensions, reducing n PCs to " % adata_full.obsm[latent_choice].shape[1])
+    L.warning("N PCs is larger than %i dimensions, reducing n PCs to " % adata_full.obsm[latent_choice].shape[1])
 
 
 n_pcs= min(int(args.neighbors_n_pcs), adata_full.obsm[latent_choice].shape[1])
 
 
+L.info("Running neighbors")
 run_neighbors_method_choice(adata_full, 
             method=args.neighbors_method, 
             n_neighbors=int(args.neighbors_k), 
             n_pcs=n_pcs, 
             metric=args.neighbors_metric, 
             use_rep=latent_choice,
             nthreads=max([threads_available, 6]))
+L.info("Running UMAP and Leiden")
 sc.tl.umap(adata_full, min_dist=0.4)
 sc.tl.leiden(adata_full, key_added="leiden_" + latent_choice)
 
 model_name = os.path.basename(os.path.dirname(args.reference_path))
 model_name = ''.join(e for e in model_name if e.isalnum())
 
 
 file_name= "umap_" + model_name + "_" + latent_choice
 L.info ("filename is %s" % file_name )
 
+L.info("Plotting UMAP")
 fig = sc.pl.embedding(adata_full, basis = "umap",color=["is_reference"],
          show=False, return_fig=True)
 fig.tight_layout()
 fig.savefig(os.path.join("figures/", file_name + ".png"))
 
 umap = pd.DataFrame(adata_full.obsm['X_umap'], adata_full.obs.index)
-
+L.info("Saving UMAP coordinates to csv file")
 umap.to_csv(os.path.join("refmap/", file_name + ".csv") )
-file_name= "query_to_reference_" + model_name + "_" + latent_choice + ".h5mu" 
 
+file_name= "query_to_reference_" + model_name + "_" + latent_choice + ".h5mu" 
 mdata_save = MuData({"rna":adata_full})
 
+L.info("Saving MuData to refmap/" + file_name)
 mdata_save.write(os.path.join( "refmap/" , file_name))
 
-L.info('done')
+L.info('Done')
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/rerun_find_neighbors_for_clustering.py` & `panpipes-0.5.0/panpipes/python_scripts/rerun_find_neighbors_for_clustering.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,66 +22,68 @@
 parser.add_argument('--outfile', default='./anndata_wneighbors.h5ad',
                     help="file name, format: .h5ad")
 parser.add_argument('--neighbor_dict', default=None,
                     help="helps find the correct dimension reduction for sc.pp.neighbors(), default='X_pca'")
 parser.add_argument('--n_threads', default=1,help='number of threads available')
 
 args, opt = parser.parse_known_args()
-L.info(args)
+L.info("Running with params: %s", args)
 # load the filtering dictionary 
 neighbor_dict = args.neighbor_dict
 if isinstance(args.neighbor_dict, dict):
     neighbor_dict = args.neighbor_dict
 else:
     neighbor_dict = read_yaml(args.neighbor_dict) 
 
 sc.settings.n_jobs = int(args.n_threads)
-L.info("Running with options: %s", args)
 
 # read data
-L.info("reading mudata")
+L.info("Reading in MuData from '%s'" % args.infile)
 mdata = read(args.infile)
 
 
 
 for mod in neighbor_dict.keys():
-    if neighbor_dict[mod]['use_existing']:
-        L.info('using existing neighbors graph for %s' % mod)
-        pass
-    else:
-        L.info("computing new neighbors for %s" % mod)
-        if type(mdata) is MuData:
-            adata=mdata[mod]
-        if (neighbor_dict[mod]['dim_red'] == "X_pca") and ("X_pca" not in adata.obsm.keys()):
-            L.info("X_pca not found, computing it using default parameters")
-            sc.tl.pca(adata)
-            if (mod == "atac") and (neighbor_dict[mod]['dim_remove'] is not None):
-                dimrem = int(neighbor_dict[mod]['dim_remove'])
-                adata.obsm['X_pca'] = adata.obsm['X_pca'][:, dimrem:]
-                adata.varm["PCs"] = adata.varm["PCs"][:, dimrem:]
-        if mod == "atac":
-            if (neighbor_dict[mod]['dim_red'] == "X_lsi") and ("X_lsi" not in adata.obsm.keys()):
-                L.info("X_lsi not found, computing it using default parameters")
-                lsi(adata=adata, num_components=50)
-                if neighbor_dict[mod]['dim_remove'] is not None:
+    if mod in mdata.mod.keys():
+        if neighbor_dict[mod]['use_existing']:
+            L.info('Using existing neighbors graph for %s' % mod)
+            pass
+        else:
+            L.info("Computing new neighbors for modality %s on %s" % (mod, neighbor_dict[mod]['dim_red']))
+            if type(mdata) is MuData:
+                adata=mdata[mod]
+            if (neighbor_dict[mod]['dim_red'] == "X_pca") and ("X_pca" not in adata.obsm.keys()):
+                L.info("X_pca not found, computing it using default parameters")
+                sc.tl.pca(adata)
+                if (mod == "atac") and (neighbor_dict[mod]['dim_remove'] is not None):
                     dimrem = int(neighbor_dict[mod]['dim_remove'])
-                    adata.obsm['X_lsi'] = adata.obsm['X_lsi'][:, dimrem:]
-                    adata.varm["LSI"] = adata.varm["LSI"][:, dimrem:]
-                    adata.uns["lsi"]["stdev"] = adata.uns["lsi"]["stdev"][dimrem:]
+                    adata.obsm['X_pca'] = adata.obsm['X_pca'][:, dimrem:]
+                    adata.varm["PCs"] = adata.varm["PCs"][:, dimrem:]
+            if mod == "atac":
+                if (neighbor_dict[mod]['dim_red'] == "X_lsi") and ("X_lsi" not in adata.obsm.keys()):
+                    L.info("X_lsi not found, computing it using default parameters")
+                    lsi(adata=adata, num_components=50)
+                    if neighbor_dict[mod]['dim_remove'] is not None:
+                        L.info("Removing dimension %s from X_lsi" % neighbor_dict[mod]['dim_remove'])
+                        dimrem = int(neighbor_dict[mod]['dim_remove'])
+                        adata.obsm['X_lsi'] = adata.obsm['X_lsi'][:, dimrem:]
+                        adata.varm["LSI"] = adata.varm["LSI"][:, dimrem:]
+                        adata.uns["lsi"]["stdev"] = adata.uns["lsi"]["stdev"][dimrem:]
+
+            # run command
+            opts = dict(method=neighbor_dict[mod]['method'],
+                        n_neighbors=int(neighbor_dict[mod]['k']),
+                        n_pcs=int(neighbor_dict[mod]['n_dim_red']),
+                        metric=neighbor_dict[mod]['metric'],
+                        nthreads=args.n_threads,
+                        use_rep=neighbor_dict[mod]['dim_red'])
+
+
+            run_neighbors_method_choice(adata,**opts)
+            mdata.mod[mod] = adata
+            mdata.update()
 
-        # run command
-        opts = dict(method=neighbor_dict[mod]['method'],
-                    n_neighbors=int(neighbor_dict[mod]['k']),
-                    n_pcs=int(neighbor_dict[mod]['n_dim_red']),
-                    metric=neighbor_dict[mod]['metric'],
-                    nthreads=args.n_threads,
-                    use_rep=neighbor_dict[mod]['dim_red'])
 
 
-        run_neighbors_method_choice(adata,**opts)
-        mdata.update()
-
-
-
-L.info("saving data")
+L.info("Saving updated MuData to '%s'" % args.outfile)
 mdata.write(args.outfile)
-L.info("done")
+L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/run_cell2location.py` & `panpipes-0.5.0/panpipes/python_scripts/run_cell2location.py`

 * *Files 16% similar despite different names*

```diff
@@ -81,14 +81,17 @@
                     help="")
 parser.add_argument("--continuous_covariate_keys_reference",
                     default=None,
                     help="")
 parser.add_argument("--max_epochs_reference",
                     default=None,
                     help="")
+parser.add_argument("--use_gpu_reference",
+                    default=True,
+                    help="")
 
 # parameters for spatial model: 
 parser.add_argument("--labels_key_st",
                     default=None,
                     help="")
 parser.add_argument("--batch_key_st",
                     default=None,
@@ -107,20 +110,22 @@
                     help="")
 parser.add_argument("--detection_alpha",
                     default=None,
                     help="")
 parser.add_argument("--max_epochs_st",
                     default=None,
                     help="")  
+parser.add_argument("--use_gpu_st",
+                    default=True,
+                    help="")
 
 
 args, opt = parser.parse_known_args()
 
-L.info("running with args:")
-L.debug(args)
+L.info("Running with params: %s", args)
 
 figdir = args.figdir
 if not os.path.exists(figdir):
     os.mkdir(figdir)
 sc.settings.figdir = figdir
 sc.set_figure_params(scanpy=True, fontsize=14, dpi=300, facecolor='white', figsize=(5,5))
 
@@ -175,128 +180,165 @@
     max_epochs_reference = int(args.max_epochs_reference)
     
 if args.max_epochs_st is None: 
     max_epochs_st = None
 else: 
     max_epochs_st= int(args.max_epochs_st)
 
+if (args.use_gpu_reference is True) or (args.use_gpu_reference == "True"): 
+    use_gpu_reference = True
+else:
+    use_gpu_reference = False
+if (args.use_gpu_st is True) or (args.use_gpu_st == "True"): 
+    use_gpu_st = True
+else:
+    use_gpu_st = False
 
 
 
 #1. read in the data
 #spatial: 
+L.info("Reading in spatial MuData from '%s'" % args.input_spatial)
 mdata_spatial = mu.read(args.input_spatial)
 adata_st = mdata_spatial.mod['spatial']
 #single-cell: 
+L.info("Reading in reference MuData from '%s'" % args.input_singlecell)
 mdata_singlecell = mu.read(args.input_singlecell)
 adata_sc = mdata_singlecell.mod['rna']
 
 
 
 #2. Perform gene selection:
 if args.gene_list != "None": # read in csv and subset both anndatas
+    if os.path.exists(args.gene_list):
+        L.info("Reading in gene list file from '%s'" % args.gene_list)
+    else: 
+        L.error("File '%s' could not be found." % args.gene_list)
+        sys.exit("File '%s' could not be found." % args.gene_list)
     reduced_gene_set = pd.read_csv(args.gene_list, header = 0)
     reduced_gene_set.columns = ["HVGs"]
+    L.info("Subsetting data on gene list")
     adata_sc.var["selected_gene"] = adata_sc.var.index.isin(reduced_gene_set["HVGs"])
     adata_st.var["selected_gene"] = adata_st.var.index.isin(reduced_gene_set["HVGs"])
     adata_sc = adata_sc[:, adata_sc.var["selected_gene"]]
     adata_st = adata_st[:, adata_st.var["selected_gene"]]
     # check whether all genes are present in both, spatial & reference
     if set(adata_st.var.index) != set(adata_sc.var.index):
         L.error(
             "Not all genes of the gene list %s are present in the reference as well as in the ST data. Please provide a gene list where all genes are present in both, reference and ST.", args.gene_list)
         sys.exit(
             "Not all genes of the gene list are present in the reference as well as in the ST data. Please provide a gene list where all genes are present in both, reference and ST.")
 
 else: # perform feature selection according to cell2loc
     if remove_mt is True: 
+        L.info("Removing MT genes")
         adata_st.var["MT_gene"] = [gene.startswith("MT-") for gene in adata_st.var.index]
         adata_st.obsm["MT"] = adata_st[:, adata_st.var["MT_gene"].values].X.toarray()
         adata_st = adata_st[:, ~adata_st.var["MT_gene"].values]
     # intersect vars of reference and spatial
+    L.info("Intersecting vars of reference and spatial ")
     shared_features = [feature for feature in adata_st.var_names if feature in adata_sc.var_names]
     adata_sc = adata_sc[:, shared_features]
     adata_st = adata_st[:, shared_features]
     # select features
+    L.info("Selecting features using 'cell2location.utils.filtering.filter_genes() function'")
     selected = cell2loc_filter_genes(adata_sc, figdir + "/gene_filter.png", cell_count_cutoff=float(args.cell_count_cutoff),
                                                cell_percentage_cutoff2=float(args.cell_percentage_cutoff2),
                                                 nonz_mean_cutoff=float(args.nonz_mean_cutoff))
-
+    L.info("Subsetting data on selected features")
     adata_sc = adata_sc[:, selected]
     adata_st = adata_st[:, selected]
 
     
 
 # 3. Fit regression model 
+L.info("Setting up AnnData for the reference model")
 c2l.models.RegressionModel.setup_anndata(adata=adata_sc, 
                                          labels_key = args.labels_key_reference,
                                          layer= args.layer_reference, 
                                          batch_key= args.batch_key_reference,
                                          categorical_covariate_keys = categorical_covariate_keys_reference,
                                          continuous_covariate_keys =  continuous_covariate_keys_reference)
 model_ref = c2l.models.RegressionModel(adata_sc)
-model_ref.train(max_epochs=max_epochs_reference)
+L.info("Training the reference model")
+model_ref.train(max_epochs=max_epochs_reference, use_gpu = use_gpu_reference)
 
 # plot elbo
+L.info("Plotting ELBO")
 cell2loc_plot_history(model_ref, figdir + "/ELBO_reference_model.png")
 
 # export results
+L.info("Extracting the posterior of the reference model")
 adata_sc = model_ref.export_posterior(adata_sc)
 if "means_per_cluster_mu_fg" in adata_sc.varm.keys():
     inf_aver = adata_sc.varm["means_per_cluster_mu_fg"][[f"means_per_cluster_mu_fg_{i}" for i in adata_sc.uns["mod"]["factor_names"]]].copy()
 else:
     inf_aver = adata_sc.var[[f"means_per_cluster_mu_fg_{i}" for i in adata_sc.uns["mod"]["factor_names"]]].copy()
 inf_aver.columns = adata_sc.uns["mod"]["factor_names"]
 inf_aver.to_csv(output_dir+"/Cell2Loc_inf_aver.csv")
 
 # plot QC
+L.info("Plotting QC plots")
 cell2loc_plot_QC_reference(model_ref, figdir + "/QC_reference_reconstruction_accuracy.png", figdir + "/QC_reference_expression signatures_vs_avg_expression.png")
 
 # save model and update mudata
+if adata_sc.var.index.names[0] in adata_sc.var.columns: 
+	adata_sc.var.index.names = [None]
 mdata_singlecell.mod["rna"] = adata_sc
 mdata_singlecell.update()
 if save_models is True:
+    L.info("Saving reference model to '%s'" % output_dir)
     model_ref.save(output_dir +"/Reference_model", overwrite=True)
 
 
        
 # 4. Fit mapping model   
+L.info("Setting up AnnData for the spatial model")
 c2l.models.Cell2location.setup_anndata(adata=adata_st, 
                                          labels_key = args.labels_key_st,
                                          layer= args.layer_st, 
                                          batch_key= args.batch_key_st,
                                          categorical_covariate_keys = categorical_covariate_keys_st,
                                          continuous_covariate_keys =  continuous_covariate_keys_st)
 
         
 model_spatial = c2l.models.Cell2location(adata = adata_st, cell_state_df=inf_aver, 
                                         N_cells_per_location=float(args.N_cells_per_location),
                                         detection_alpha=float(args.detection_alpha))
-model_spatial.train(max_epochs=max_epochs_st)
+L.info("Training the spatial model")
+model_spatial.train(max_epochs=max_epochs_st, use_gpu = use_gpu_st)
 
 #plot elbo
+L.info("Plotting ELBO")
 cell2loc_plot_history(model_spatial, figdir + "/ELBO_spatial_model.png")
 #extract posterior
+L.info("Extracting the posterior of the spatial model")
 adata_st = model_spatial.export_posterior(adata_st)
 #plot QC
+L.info("Plotting QC plots")
 cell2loc_plot_QC_reconstr(model_spatial, figdir + "/QC_spatial_reconstruction_accuracy.png")
 
 
 #plot output
+L.info("Plotting spatial embedding plot coloured by 'q05_cell_abundance_w_sf'")
 adata_st.obs[adata_st.uns["mod"]["factor_names"]] = adata_st.obsm["q05_cell_abundance_w_sf"]
 sc.pl.spatial(adata_st,color=adata_st.uns["mod"]["factor_names"], show = False, save = "_Cell2Loc_q05_cell_abundance_w_sf.png") 
 
 
 # save model and update mudata
+if adata_st.var.index.names[0] in adata_st.var.columns: 
+	adata_st.var.index.names = [None]
 mdata_spatial.mod["spatial"] = adata_st
 mdata_spatial.update()
 if save_models is True: 
+    L.info("Saving spatial model to '%s'" % output_dir)
     model_spatial.save(output_dir+"/Spatial_mapping_model", overwrite=True)
 
 
 #6. save mudatas 
+L.info("Saving MuDatas to '%s'" % output_dir)
 mdata_singlecell.write(output_dir+"/Cell2Loc_screference_output.h5mu")
 mdata_spatial.write(output_dir+"/Cell2Loc_spatial_output.h5mu")
 
 
 L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/run_clustering.py` & `panpipes-0.5.0/panpipes/python_scripts/run_clustering.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,46 +26,54 @@
                     default=0.5, help="no. neighbours parameters for sc.pp.neighbors()")
 parser.add_argument("--algorithm", 
                     default="leiden", help="algortihm choice from louvain and leiden")
 parser.add_argument("--neighbors_key", 
                     default="neighbors", help="algortihm choice from louvain and leiden")
 
 args, opt = parser.parse_known_args()
-L.info(args)
+L.info("Running with params: %s", args)
 
 # read data
+L.info("Reading in data from '%s'" % args.infile)
 mdata = mu.read(args.infile)
 if type(mdata) is AnnData:
     adata = mdata
 elif args.modality is not None:
     adata = mdata[args.modality]
 else:
     adata = mdata
 
 uns_key=args.neighbors_key
 # check sc.pp.neihgbours has been run
 if uns_key not in adata.uns.keys():
     # sys.exit("Error: sc.pp.neighbours has not been run on this object")
+    L.warning("Running neighbors for modality %s with default parameters since no neighbors graph found in this data object" % args.modality)
     sc.pp.neighbors(adata)
     uns_key="neighbors"
 
 
 # run command
 if args.algorithm == "louvain":
+    L.info("Running Louvain clustering for modality %s and resolution %s on %s", (args.modality, args.resolution, uns_key))
     sc.tl.louvain(adata, resolution=float(args.resolution), key_added='clusters', neighbors_key=uns_key)
 elif args.algorithm == "leiden":
+    L.info("Running Leiden clustering for modality %s and resolution %s on %s", (args.modality, args.resolution, uns_key))
     sc.tl.leiden(adata, resolution=float(args.resolution), key_added='clusters', neighbors_key=uns_key)
 else:
-    sys.exit("algorithm not found: please specify 'louvain' or 'leiden'")
+    L.error("Could not find clustering algorithm '%s'. Please specify 'louvain' or 'leiden'" % args.algorithm)
+    sys.exit("Could not find clustering algorithm '%s'. Please specify 'louvain' or 'leiden'"  % args.algorithm)
 
 #mdata.update()
 ## write out clusters as text file
+L.info("Saving cluster column to csv file '%s'" % args.outfile)
 clusters = pd.DataFrame(adata.obs['clusters'])
 clusters.to_csv(args.outfile, sep='\t')
 
+L.info("Saving cell numbers per cluster to csv file")
+
 tmp = clusters['clusters'].value_counts().to_frame("cell_num").reset_index().rename(columns={"index":"cluster"})
 tmp.to_csv(os.path.dirname(args.outfile) + "/cellnum_per_cluster.csv")
 
 if "sample_id" in adata.obs.columns:
     ccounts = pd.DataFrame(adata.obs[['sample_id', 'clusters']])
     tmp = ccounts.value_counts().to_frame("cell_num").reset_index()
     tmp.to_csv(os.path.dirname(args.outfile) + "/cellnum_per_sample_id_per_cluster.csv")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/run_collate_mtd_files.py` & `panpipes-0.5.0/panpipes/python_scripts/run_collate_mtd_files.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 parser.add_argument('--prot_integration_col', default=None, help='the column in the adata.obs on which you have integrated')
 parser.add_argument('--atac_integration_col', default=None, help='the column in the adata.obs on which you have integrated')
 parser.add_argument('--multimodal_integration_col', default=None, help='the column in the adata.obs on which you have integrated')
 parser.add_argument("--output_cell_metadata_csv")
 parser.add_argument("--output_combined_umaps_tsv")
 parser.add_argument("--output_batch_yml")
 args, opt = parser.parse_known_args()
-L.info(args)
-L.info("reading in files")
+L.info("Running with params: %s", args)
 
+L.info("Reading in data from '%s'" % args.input_mudata)
 cell_meta_df = mu.read(args.input_mudata).obs
 mtd_columns = cell_meta_df.columns.to_list()
 
 # get all the batch columns 
 # load up all the batch columns
 batch_dict = dict(rna=args.rna_integration_col, 
                   prot=args.prot_integration_col, 
@@ -86,37 +86,34 @@
             for j in range(i + 1, len(v)):
                 col1 = v[i]
                 col2 = v[j]
                 
                 if mod_meta_df[col1].equals(mod_meta_df[col2]):
                     identical_column_pairs.append((col1, col2))
         if identical_column_pairs:
-            print("Identical column pairs:")
             for col1, col2 in identical_column_pairs:
                 print(f"{col1} and {col2} are identical.")
             batch_dict[k].append(col1)
         else:
-            print("No identical columns found.")
             cell_meta_df[str(k)+ ":bc_batch"] = mod_meta_df.apply(lambda x: '|'.join(x), axis=1)
             batch_dict[k].append(k+ ":bc_batch")
-    L.info("batch values %s" %(batch_dict[k]))
+    L.info("Batch values %s" %(batch_dict[k]))
 
 for k in batch_dict.keys():
     unique_values = list(set(batch_dict[k]))
     batch_dict[k] = unique_values
 
-L.info("saving batch dictionary")
-print(batch_dict)
-
+L.info("Saving cell metadata to csv file '%s'" % args.output_cell_metadata_csv)
 cell_meta_df.to_csv(args.output_cell_metadata_csv)
 
+L.info("Saving batch dictionary to '%s'" % args.output_batch_yml)
 with open(args.output_batch_yml, 'w') as outfile:
     yaml.dump(batch_dict, outfile, default_flow_style=False)
 
-L.info("reading in all umaps")
+L.info("Reading in all UMAP coordinates")
 # load files
 input_files = args.input_umap_files.split(",")
 umaps_list = [pd.read_csv(x, index_col=0) for x in input_files]
 umaps_index = [re.sub("umap_|.csv", "", os.path.basename(x)) for x in input_files]
 umaps_df = pd.concat(umaps_list, axis=0, keys=umaps_index).reset_index(level=0)
 umaps_df.columns = ["method", "umap_1", "umap_2"]
 umaps_df = umaps_df.merge(cell_meta_df, left_index=True, right_index=True)
@@ -130,14 +127,14 @@
     col = df.pop(col)
     df.insert(pos, col.name, col)
 move_column_inplace(umaps_df, "mod", 0)
 move_column_inplace(umaps_df, "method", 1)
 umaps_df = umaps_df.sort_values(by=['mod','method'])
 
 # save umap df to file
-L.info("save umap df to file")
+L.info("Saving combined UMAP dataframe to file '%s'" % args.output_combined_umaps_tsv)
 umaps_df = umaps_df.iloc[:,0:4]
 umaps_df['cellbarcode'] = umaps_df.index
 umaps_df.to_csv(args.output_combined_umaps_tsv, sep="\t")
 
-L.info("done")
+L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/run_dsb_clr.py` & `panpipes-0.5.0/panpipes/python_scripts/run_dsb_clr.py`

 * *Files identical despite different names*

### Comparing `panpipes-0.4.1/panpipes/python_scripts/run_filter.py` & `panpipes-0.5.0/panpipes/python_scripts/run_filter.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import argparse
 import pandas as pd
 import re
 import muon as mu
 from anndata import AnnData
 from muon import MuData
 import yaml
+import os
 
 # import scpipelines.funcs as scp
 from panpipes.funcs.processing import intersect_obs_by_mod, remove_unused_categories
 from panpipes.funcs.io import write_obs, read_yaml, dictionary_stripper
 import collections.abc
 import sys
 import logging
@@ -62,134 +63,136 @@
 parser.add_argument('--intersect_mods', default=None,
                     help='comma separated string of modalities we want to intersect_obs on')                 
 
 
 # load options
 parser.set_defaults(verbose=True)
 args, opt = parser.parse_known_args()
-L.info('running with args:')
-L.info(args)
+L.info("Running with params: %s", args)
  
 # load the filtering dictionary 
 filter_dict = args.filter_dict
 if isinstance(args.filter_dict, dict):
     filter_dict = args.filter_dict
 else:
     filter_dict = read_yaml(args.filter_dict) 
 
 # remove Nones for each level of filter dict
 filter_dict = map_nested_dicts_remove_none(filter_dict)
 filter_dict = dictionary_stripper(filter_dict)
-L.info("filter dictionary:\n %s" %filter_dict)
+L.info("Filter dictionary:\n %s" %filter_dict)
 
 # load mudata
+L.info("Reading in MuData from '%s'" % args.input_mudata)
 mdata = mu.read(args.input_mudata)
 
 if isinstance(mdata, AnnData):
-    raise TypeError("input_mudata should be of MuData format, not Anndata")
+    raise TypeError("Input '%s' should be of MuData format, not Anndata"  % args.input_mudata)
 
 orig_obs = mdata.obs.copy()
 
-L.info("Before filtering %d" % mdata.n_obs)
+L.info("Before filtering: "+ str(mdata.n_obs) + " cells and " + str(mdata.n_vars) + " features")
+
 # filter based on provided barcodes -----
 if args.keep_barcodes is not None:
-    L.info("filtering all modalities by keep_barcodes file")
-    keep_bc = pd.read_csv(args.keep_barcodes,header=None)
+    if os.path.exists(args.keep_barcodes):
+        L.info("Reading in keep_barcodes file from '%s'" % args.keep_barcodes)
+        keep_bc = pd.read_csv(args.keep_barcodes,header=None)
+    else:
+        L.error("The path of the keep_barcodes file '%s' could not be found" % args.keep_barcodes)
+        sys.exit("The path of the keep_barcodes file '%s' could not be found" %  args.keep_barcodes)
+
+    L.info("Filtering all modalities by keep_barcodes file")
     mdata = mdata[mdata.obs_names.isin(keep_bc[0]),:].copy()
     remove_unused_categories(mdata.obs)
     mdata.update()
     L.info("Remaining cells %d" % mdata.n_obs)
 
 # L.debug(mdata.obs['sample_id'].value_counts())
 
 # filter more than
 if filter_dict['run']:
     # this will go through the modalities one at a time,
     # then the categories max, min and bool
     for mod in mdata.mod.keys():
-        L.info(mod)
+        L.info("Filtering modality '%s'" % mod)
         if mod in filter_dict.keys():
             for marg in filter_dict[mod].keys():
                 if marg == "obs":
                     if "max" in filter_dict[mod][marg].keys():
                         for col, n in filter_dict[mod][marg]['max'].items():
-                            L.info("filter %s %s to less than %s" % (mod, col, n))
+                            L.info("Filtering cells of modality '%s' by '%s' in obs to less than %s" % (mod, col, n))
                             mu.pp.filter_obs(mdata.mod[mod], col, lambda x: x <= n)
                             L.info("Remaining cells %d" % mdata[mod].n_obs)
-                            L.info("Remaining cells %d" % mdata[mod].shape[0])
                     if "min" in filter_dict[mod][marg].keys():
                         for col, n in filter_dict[mod][marg]['min'].items():
-                            L.info("filter %s %s to more than %s" % (mod, col, n))
+                            L.info("Filtering cells of modality '%s' by '%s' in obs to more than %s" % (mod, col, n))
                             mu.pp.filter_obs(mdata.mod[mod], col, lambda x: x >= n)
                             L.info("Remaining cells %d" % mdata[mod].n_obs)
                     if "bool" in filter_dict[mod][marg].keys():
                         for col, n in filter_dict[mod][marg]['bool'].items():
-                            L.info("filter %s %s marked %s" % (mod, col, n))
+                            L.info("Filtering cells of modality '%s' by '%s' in obs marked %s" % (mod, col, n))
                             mu.pp.filter_obs(mdata.mod[mod], col, lambda x: x == n)
                             L.info("Remaining cells %d" % mdata[mod].n_obs)
                 if marg == "var":
                     if "max" in filter_dict[mod][marg].keys():
                         for col, n in filter_dict[mod][marg]['max'].items():
-                            L.info("filter %s %s to less than %s" % (mod, col, n))
+                            L.info("Filtering features of modality '%s' by '%s' in .var to less than %s" % (mod, col, n))
                             mu.pp.filter_var(mdata.mod[mod], col, lambda x: x <= n)
-                            L.info("Remaining cells %d" % mdata[mod].n_obs)
+                            L.info("Remaining features: %d" % mdata[mod].n_vars)
 
                     if "min" in filter_dict[mod][marg].keys():
                         for col, n in filter_dict[mod][marg]['min'].items():
-                            L.info("filter %s %s to more than %s" % (mod, col, n))
+                            L.info("Filtering features of modality '%s' by '%s' in .var to more than %s" % (mod, col, n))
                             mu.pp.filter_var(mdata.mod[mod], col, lambda x: x >= n)
-                            L.info("Remaining cells %d" % mdata[mod].n_obs)
+                            L.info("Remaining features: %d" % mdata[mod].n_vars)
 
                     if "bool" in filter_dict[mod][marg].keys():
                         for col, n in filter_dict[mod][marg]['bool'].items():
-                            L.info("filter %s %s marked %s" % (mod, col, n))
+                            L.info("Filtering features of modality '%s' by '%s' in .var marked %s" % (mod, col, n))
                             mu.pp.filter_var(mdata.mod[mod], col, lambda x: x == n)
-                            L.info("Remaining cells %d" % mdata[mod].n_obs)
+                            L.info("Remaining features: %d" % mdata[mod].n_vars)
                             
-L.debug(mdata.obs['sample_id'].value_counts())
-L.debug(mdata['rna'].obs['sample_id'].value_counts())
+
 mdata.update()
-L.debug(mdata.obs['sample_id'].value_counts())
-L.debug(mdata['rna'].obs['sample_id'].value_counts())
+
 # intersect specific modalities
 # we don't want to just use mu.pp.intersect_obs, 
 # because we don't want to necessarily filter by repertoire
 if args.intersect_mods is not None:
     intersect_mods = args.intersect_mods.split(',')
     intersect_mods= [a.strip() for a in intersect_mods]
-    L.info("intersecting barcodes in %s" % args.intersect_mods)
+    L.info("Intersecting barcodes of modalities %s" % args.intersect_mods)
     intersect_obs_by_mod(mdata, mods = intersect_mods)
-    L.info("Remaining cells %d" % mdata.n_obs)
-    L.info(mdata.shape)
-
 
+L.info("After filtering: "+ str(mdata.n_obs) + " cells and " + str(mdata.n_vars) + " features across all modalities")
 
 remove_unused_categories(mdata.obs)
 
 # run quick test before saving out.
 assert test_matching_df_ignore_cat(mdata.obs, orig_obs)  
 
 # write out obs
 output_prefix = re.sub(".h5mu", "", args.output_mudata)
+
+L.info("Saving updated obs in a metadata tsv file to '" + output_prefix + "_filtered_cell_metadata.tsv'")
 write_obs(mdata, output_prefix=output_prefix, output_suffix="_filtered_cell_metadata.tsv")
 
 # write out the per sample_id cell numbers 
 cell_counts_dict={}
 for mm in mdata.mod.keys():
     cell_counts_dict[mm] = mdata[mod].obs.sample_id.value_counts().to_frame('n_cells')
 
 cell_counts = pd.concat(cell_counts_dict).reset_index().rename(
     columns={"level_0": "modality", "level_1": "sample_id"})
 
 L.info("cell_counts\n%s" %cell_counts)
+L.info("Saving cell counts in a metadata csv file to '" + output_prefix + "_cell_counts.csv'")
 cell_counts.to_csv(output_prefix + "_cell_counts.csv", index=None)
 
 
 mdata.update()
-L.info("writing mdata h5mu")
-L.info(args.output_mudata)
-L.debug(mdata.obs['sample_id'].value_counts())
-L.debug(mdata['rna'].obs['sample_id'].value_counts())
+L.info("Saving updated MuData to '%s'" % args.output_mudata)
 mdata.write(args.output_mudata)
 
 L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/run_filter_spatial.py` & `panpipes-0.5.0/panpipes/python_scripts/run_filter_spatial.py`

 * *Files 20% similar despite different names*

```diff
@@ -54,130 +54,123 @@
 parser.add_argument('--keep_barcodes', default=None,
                     help='1 column list of barcodes to keep, note that they should match the mudata input, this filtering happens first')
 
 
 # load options
 parser.set_defaults(verbose=True)
 args, opt = parser.parse_known_args()
-L.info('running with args:')
-L.info(args)
+L.info("Running with params: %s", args)
  
 # load the filtering dictionary 
 filter_dict = args.filter_dict
 if isinstance(args.filter_dict, dict):
     filter_dict = args.filter_dict
 else:
     filter_dict = read_yaml(args.filter_dict) 
 
 # remove Nones for each level of filter dict
 filter_dict = map_nested_dicts_remove_none(filter_dict)
 filter_dict = dictionary_stripper(filter_dict)
-L.info("filter dictionary:\n %s" %filter_dict)
+L.info("Filter dictionary:\n %s" %filter_dict)
 
 # load mudata
+
+L.info("Reading in MuData from '%s'" % args.input_mudata)
+
 mdata = mu.read(args.input_mudata)
 
 if isinstance(mdata, AnnData):
-    raise TypeError("input_mudata should be of MuData format, not Anndata")
+    raise TypeError("Input '%s' should be of MuData format, not Anndata"  % args.input_mudata)
 
 orig_obs = mdata.obs.copy()
 
-L.info("Before filtering %d" % mdata.n_obs)
+L.info("Before filtering: "+ str(mdata.n_obs) + " cells and " + str(mdata.n_vars) + " features")
+
 # filter based on provided barcodes -----
 if args.keep_barcodes is not None:
-    L.info("filtering all modalities by keep_barcodes file")
+    L.info("Filtering MuData by keep_barcodes file")
     keep_bc = pd.read_csv(args.keep_barcodes,header=None)
     mdata = mdata[mdata.obs_names.isin(keep_bc[0]),:].copy()
     remove_unused_categories(mdata.obs)
     mdata.update()
-    L.info("Remaining cells %d" % mdata.n_obs)
+    L.info("Remaining cells: %d" % mdata.n_obs)
 
 
 
 # filter more than
 if filter_dict['run']:
     # this will go through the modalities one at a time,
     # then the categories max, min and bool
     for mod in mdata.mod.keys():
         L.info(mod)
         if mod in filter_dict.keys():
             for marg in filter_dict[mod].keys():
                 if marg == "obs":
                     if "max" in filter_dict[mod][marg].keys():
                         for col, n in filter_dict[mod][marg]['max'].items():
-                            L.info("filter %s %s to less than %s" % (mod, col, n))
+                            L.info("Filtering cells of modality '%s' by '%s' in .obs to less than %s" % (mod, col, n))
                             mu.pp.filter_obs(mdata.mod[mod], col, lambda x: x <= n)
-                            L.info("Remaining cells %d" % mdata[mod].n_obs)
-                            L.info("Remaining cells %d" % mdata[mod].shape[0])
+                            L.info("Remaining cells: %d" % mdata[mod].n_obs)
                     if "min" in filter_dict[mod][marg].keys():
                         for col, n in filter_dict[mod][marg]['min'].items():
-                            L.info("filter %s %s to more than %s" % (mod, col, n))
+                            L.info("Filtering cells of modality '%s' by '%s' in .obs to more than %s" % (mod, col, n))
                             mu.pp.filter_obs(mdata.mod[mod], col, lambda x: x >= n)
-                            L.info("Remaining cells %d" % mdata[mod].n_obs)
+                            L.info("Remaining cells: %d" % mdata[mod].n_obs)
                     if "bool" in filter_dict[mod][marg].keys():
                         for col, n in filter_dict[mod][marg]['bool'].items():
-                            L.info("filter %s %s marked %s" % (mod, col, n))
+                            L.info("Filtering cells of modality '%s' by '%s' in .obs marked %s" % (mod, col, n))
                             mu.pp.filter_obs(mdata.mod[mod], col, lambda x: x == n)
-                            L.info("Remaining cells %d" % mdata[mod].n_obs)
+                            L.info("Remaining cells: %d" % mdata[mod].n_obs)
                 if marg == "var":
                     if "max" in filter_dict[mod][marg].keys():
                         for col, n in filter_dict[mod][marg]['max'].items():
-                            L.info("filter %s %s to less than %s" % (mod, col, n))
+                            L.info("Filtering features of modality '%s' by '%s' in .var to less than %s" % (mod, col, n))
                             mu.pp.filter_var(mdata.mod[mod], col, lambda x: x <= n)
-                            L.info("Remaining cells %d" % mdata[mod].n_obs)
+                            L.info("Remaining features: %d" % mdata[mod].n_vars)
 
                     if "min" in filter_dict[mod][marg].keys():
                         for col, n in filter_dict[mod][marg]['min'].items():
-                            L.info("filter %s %s to more than %s" % (mod, col, n))
+                            L.info("Filtering features of modality '%s' by '%s' in .var to more than %s" % (mod, col, n))
                             mu.pp.filter_var(mdata.mod[mod], col, lambda x: x >= n)
-                            L.info("Remaining cells %d" % mdata[mod].n_obs)
+                            L.info("Remaining features: %d" % mdata[mod].n_vars)
 
                     if "bool" in filter_dict[mod][marg].keys():
                         for col, n in filter_dict[mod][marg]['bool'].items():
-                            L.info("filter %s %s marked %s" % (mod, col, n))
+                            L.info("Filtering features of modality '%s' by '%s' in .var marked %s" % (mod, col, n))
                             mu.pp.filter_var(mdata.mod[mod], col, lambda x: x == n)
-                            L.info("Remaining cells %d" % mdata[mod].n_obs)
+                            L.info("Remaining features: %d" % mdata[mod].n_vars)
                             
 
 mdata.update()
 
-# intersect specific modalities
-# we don't want to just use mu.pp.intersect_obs, 
-# because we don't want to necessarily filter by repertoire
-#if args.intersect_mods is not None:
-#    intersect_mods = args.intersect_mods.split(',')
-#    intersect_mods= [a.strip() for a in intersect_mods]
-#    L.info("intersecting barcodes in %s" % args.intersect_mods)
-#    intersect_obs_by_mod(mdata, mods = intersect_mods)
-#    L.info("Remaining cells %d" % mdata.n_obs)
-#    L.info(mdata.shape)
-
-
+L.info("After filtering: "+ str(mdata.n_obs) + " cells and " + str(mdata.n_vars) + " features")
 
 remove_unused_categories(mdata.obs)
 
 # run quick test before saving out.
 assert test_matching_df_ignore_cat(mdata.obs, orig_obs)  
 
 # write out obs
 output_prefix = re.sub(".h5mu", "", os.path.basename(args.output_mudata))
+
+L.info("Saving updated obs in a metadata tsv file to './tables/" + output_prefix + "_filtered_cell_metadata.tsv'")
 write_obs(mdata, output_prefix=os.path.join("tables/",output_prefix), output_suffix="_filtered_cell_metadata.tsv")
 
 # write out the per sample_id cell numbers 
 cell_counts_dict={}
 for mm in mdata.mod.keys():
     cell_counts_dict[mm] = mdata[mm].obs.sample_id.value_counts().to_frame('n_cells')
 
 cell_counts = pd.concat(cell_counts_dict).reset_index().rename(
     columns={"level_0": "modality", "level_1": "sample_id"})
 
-L.info("cell_counts\n%s" %cell_counts)
+L.info("cell_counts: \n%s" %cell_counts)
+L.info("Saving cell counts in a metadata csv file to './tables/" + output_prefix + "_cell_counts.csv'")
 cell_counts.to_csv("tables/" + output_prefix + "_cell_counts.csv", index=None)
 
-
 mdata.update()
-L.info("writing mdata h5mu")
-L.info(args.output_mudata)
+
+L.info("Saving updated MuData to '%s'" % args.output_mudata)
 mdata.write(args.output_mudata)
 
 L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/run_find_markers.py` & `panpipes-0.5.0/panpipes/python_scripts/run_find_markers.py`

 * *Files identical despite different names*

### Comparing `panpipes-0.4.1/panpipes/python_scripts/run_find_markers_multi.py` & `panpipes-0.5.0/panpipes/python_scripts/run_find_markers_multi.py`

 * *Files 12% similar despite different names*

```diff
@@ -58,36 +58,37 @@
     if 'log1p' in adata.uns.keys():
         if not adata.uns['log1p']:
             L.debug( "log1p dict is Empty, refilling dict")
             adata.uns['log1p'] = {'base': None}
 
 
 def load_and_merge_clusters(adata, cluster_file):
-    # load clusterss
+    # load clusters
     df = pd.read_csv(cluster_file, sep="\t", index_col=0)
     adata_shape = adata.shape
     # add clusters to adata.obs
     adata.obs = pd.merge(adata.obs, df, how="left", left_index=True, right_index=True)
     # check check we have not lost cells in merge
     if adata.shape != adata_shape:
-        L.info("some cells lost in merge, not all cells have a cluster?")
+        L.warning("Some cells lost in merge, not all cells have a cluster?")
     L.debug(adata.shape)
 
 
 def get_header():
     # write out the correct header before we start, need to werite it out before, because we use append mode for the multimodal find markers
     # and we don't wantto end up with a new header half
-    if sc.__version__ < "1.7.0":
+    if sc.__version__ < "1.07.0":
         markers_columns = ['cluster', 'scores', 'gene', 'avg_logFC', 'pvals', 'p.adj.bonferroni']
-    elif sc.__version__ >= "1.7.0":
+    elif sc.__version__ >= "1.07.0":
         markers_columns = ['cluster', 'gene', 'scores', 'avg_logFC', 'pvals', 'p.adj.bonferroni']
     return markers_columns
 
 
 def filter_zero_count_genes(adata, layer=None):
+    L.info("Removing zero count genes")
     if layer is None:
         if issparse(adata.X):
             bool_list = (adata.X.sum(axis=0) > 0).tolist()[0]
         else:
             bool_list = (adata.X.sum(axis=0) > 0).tolist()
     else:
         if issparse(adata.layers[layer]):
@@ -105,119 +106,124 @@
                    methoduse=None, 
                    pseudo_seurat=False):
     if type(cluster_groups) is list:
         # make sure the clusters are strings else rank_gene_groups crashes
         cluster_groups = [str(x) for x in cluster_groups]
     adata.obs[cluster_col] = adata.obs[cluster_col].astype('str').astype('category')
     if pseudo_seurat:
-        L.info('running rank gene groups with pseudo-seurat method')
+        L.info('Running rank gene groups with pseudo-seurat method')
         markers, filter_stats = find_all_markers_pseudo_seurat(adata,   
                                         groups=cluster_groups, 
                                         groupby=cluster_col, 
                                         method=methoduse,
                                         n_genes=float("inf"), 
                                         corr_method="bonferroni",
                                         layer=layer,
                                         arg_minpct=0.1,
                                         arg_mindiffpct=-float("inf"), 
                                         arg_logfcdiff=0.25)
         markers = markers.reset_index().drop(columns='level_1').rename(columns={'level_0':'gene'})
     else:
         # find markers
-        L.info('running rank gene groups with standard scanpy implementation')
+        L.info('Running rank gene groups with standard scanpy implementation')
         sc.tl.rank_genes_groups(adata, 
                                 groups=cluster_groups, 
                                 groupby=cluster_col, 
                                 method=methoduse,
                                 n_genes=float("inf"), 
                                 corr_method="bonferroni",
                                 layer=layer)
         markers = sc.get.rank_genes_groups_df(adata, group=None)
-        L.info("Rank gene groups complete")
         filter_stats = None
     return markers, filter_stats
 
 
 def main(adata, 
          cluster_file,
          mod, 
          mincells=None,
          layer=None,
          testuse=None,
          pseudo_seurat=False,
          output_file_prefix="markers") :
     # check the X slot actually contains data
     if adata.X.shape[1] == 0:
-        L.info("exiting because adata.X contains no values")
-        sys.exit("exiting because adata.X contains no values")
+        L.error(".X does not contain any values")
+        sys.exit(".X does not contain any values")
     # prevent log1p base error.
     check_log1p_dict(adata)
     # load clusters
     load_and_merge_clusters(adata, cluster_file)
     # filter out genes with zero counts
     filter_zero_count_genes(adata, layer=layer)
     # filter out clusters with less than min cells
     if mincells is not None:
         min_cell_df = adata.obs['clusters'].value_counts() 
         if any(min_cell_df < mincells):
             exclude = min_cell_df[min_cell_df < mincells].index
-            L.info('exluding clusters for haveing too few cells: %s' % str(list(exclude)))
+            L.info('Exluding clusters for having < %s cells: %s' % (mincells,str(list(exclude))))
             clust_vals = list(set(min_cell_df[min_cell_df >= mincells].index))
         else:
             clust_vals = list(set(adata.obs["clusters"]))
     all_markers, all_filter_stats = run_clustering(adata,
                                                    cluster_groups=clust_vals,
                                                    cluster_col="clusters",
                                         layer=layer, 
                                         methoduse=testuse, 
                                         pseudo_seurat=pseudo_seurat)
     # make sure all files have consitent headers
     all_markers.columns = get_header()
     all_markers['mod'] = mod
+    L.info("Saving all markers to " + output_file_prefix + ".txt")
     all_markers.to_csv(output_file_prefix + ".txt", index=False, sep='\t')
     # subset to significant markers
+    L.info("Subsetting to significant markers with Bonferroni < 0.05 and avg logFC > 0")
     signif_markers = all_markers[(all_markers["p.adj.bonferroni"] < 0.05) &( all_markers.avg_logFC > 0)]
     if signif_markers.shape[0] !=0:
+        L.info("Saving significant markers to " + output_file_prefix + mod + "_signif.txt")
         signif_markers.to_csv(output_file_prefix + mod + "_signif.txt", index=False, sep='\t')
         # write out to excel
+        L.info("Saving significant markers to excel file")
         excel_file_top = output_file_prefix + mod + "_signif.xlsx"
         with pd.ExcelWriter(excel_file_top) as writer:
             for xx in signif_markers.cluster.unique():
                 df_sub = signif_markers[signif_markers.cluster == xx]
                 if df_sub.shape[0] !=0:
                     df_sub.to_excel(writer, sheet_name="cluster" + str(xx), index=False)
+    else:
+        L.warning("No significant markers found!")
     #  when relevent write out filter stats
     if pseudo_seurat is True:
+        L.info("Saving filter statistics to " + output_file_prefix + "_filter_stats_" + mod + ".txt")
         all_filter_stats = all_filter_stats.reset_index().rename(columns={'index':'cluster'})
         all_filter_stats.to_csv(output_file_prefix + "_filter_stats_" + mod + ".txt", index=False, sep="\t")
 
 
-
-L.info("Running with options")
-L.info(args)
-L.info('\n')
+L.info("Running with params: %s", args)
 
 # read data
+L.info("Reading in MuData from '%s'" % args.infile)
 mdata = read(args.infile)
     
 
 if type(mdata) is AnnData:
     adata = mdata
     # main function only does rank_gene_groups on X, so 
 elif type(mdata) is MuData and args.modality is not None:
     adata = mdata[args.modality]    
 else:
-    sys.exit('if inputting a mudata object, you need to specify a modality')
+    L.error("If the input is a MuData object, a modality needs to be specified")
+    sys.exit('If the input is a MuData object, a modality needs to be specified')
     
 
-
 main(adata, 
      mod=args.modality,
      cluster_file=args.cluster_file,
     mincells=int(args.mincells),
     layer=args.layer,
     testuse=args.testuse,
     pseudo_seurat=args.pseudo_seurat,
     output_file_prefix=args.output_file_prefix)
 
-L.info("done")
+
+L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/run_find_neighbors.py` & `panpipes-0.5.0/panpipes/python_scripts/run_find_neighbors.py`

 * *Files identical despite different names*

### Comparing `panpipes-0.4.1/panpipes/python_scripts/run_lisi.py` & `panpipes-0.5.0/panpipes/python_scripts/run_lisi.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,22 +18,25 @@
 
 parser = argparse.ArgumentParser()
 parser.add_argument("--combined_umaps_df")
 parser.add_argument("--cell_meta_df")
 parser.add_argument("--integration_dict")
 parser.add_argument("--fig_dir")
 args = parser.parse_args()
-L.info(args)
+L.info("Running with params: %s", args)
 
 # load combined umaps and cellmtd file
 # load metadata
+L.info("Reading in cell metadata from '%s'" % args.cell_meta_df)
 cell_meta_df = pd.read_csv(args.cell_meta_df, index_col=0)
+L.info("Reading in batch dictionary from '%s" % args.integration_dict)
 batch_dict = read_yaml(args.integration_dict)
+L.info("Reading in UMAP coordinates from '%s'" % args.combined_umaps_df)
 umaps = pd.read_csv(args.combined_umaps_df, sep="\t", index_col=0)
-L.info("fixing the batch_keys dictionary")
+
 for k in batch_dict.keys():
     v=batch_dict[k]
     if k =="multimodal":
         mk = []
         exc = []
         for v2 in v:
             if v2 in cell_meta_df.columns:
@@ -51,36 +54,37 @@
    # else:
    #     v =[k + ":" +v1 if k!="multimodal" else v1 for v1 in v  ] #add the prepending modality
    #     batch_dict[k] = v
     if len(v) > 1:
         mod_meta_df= cell_meta_df[v].dropna()
         cell_meta_df[str(k)+ ":bc_batch"] = mod_meta_df.apply(lambda x: "|".join(str(x)), axis=1)
         batch_dict[k].append(k+ ":bc_batch")
-    L.info("batch keys %s" %(batch_dict[k]))
+    L.info("Batch keys %s" %(batch_dict[k]))
 
 
 for md in batch_dict.keys():
-    L.info("Running lisi on modality: %s" % md)
+    L.info("Running LISI on modality: %s" % md)
     # get one df per method for this modality
     splits = dict(list(umaps[umaps["mod"]==md].groupby("method")))
     lisi_results = []
     columns = batch_dict[md]
     for k, xx in splits.items():
-        L.info("computing lisi for correction %s" % k)
+        L.info("Computing LISI for correction %s" % k)
         # compute LISI for each batch
         umap_coords = xx.loc[:,["umap_1", "umap_2"]].to_numpy()
         # check it"s in the correct order
         batch_df = cell_meta_df.loc[xx.index,:]
         res = hm.compute_lisi(umap_coords, batch_df, columns)
         lisi_results.append(pd.DataFrame(res, index=batch_df.index, columns=columns))
     # put LISI scores into a pandas df
     lisi_df = pd.concat(lisi_results, keys=splits.keys()).reset_index().rename(columns={"level_0":"method", "level_1":"cellbarcode", "index":"cellbarcode"})
+    L.info("Saving LISI scores to csv file")
     lisi_df.to_csv(os.path.join(args.fig_dir, md, "LISI_scores.csv"), index=False)
     # # make a density  plot of LISI scores.
-    L.info("plotting lisi density")
+    L.info("Plotting LISI density")
     plot_df = lisi_df.melt(id_vars=['cellbarcode', 'method'], var_name="integration_variable", value_name="LISI score")
     plot_df["integration_variable"] = plot_df["integration_variable"].astype("category")
     plot_df = plot_df.rename(columns={"method": "Correction"})
     plot_df["Correction"] = plot_df["Correction"].astype('category')
     # # reorder categories to match other plots
     methods = plot_df["Correction"].unique().tolist()
     if "none" in methods:
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/run_preprocess_atac.py` & `panpipes-0.5.0/panpipes/python_scripts/run_preprocess_atac.py`

 * *Files 7% similar despite different names*

```diff
@@ -84,143 +84,164 @@
                     help="cutoff for Signac's HVF selection")
 parser.add_argument("--filter_by_hvf", default=False) 
 parser.add_argument("--color_by", default="batch") 
 
 
 args, opt = parser.parse_known_args()
 
-L.info("running with args:")
-L.info(args)
+L.info("Running with params: %s", args)
 
 figdir = args.figdir
 
 if not os.path.exists(figdir):
     os.mkdir(figdir)
 
 sc.settings.figdir = figdir
 sc.set_figure_params(scanpy=True, fontsize=14, dpi=300, facecolor='white', figsize=(5,5))
 
+L.info("Reading in MuData from '%s'" % args.input_mudata)
 mdata = mu.read(args.input_mudata)
 atac = mdata.mod['atac']
 
 # save raw counts
+L.info("Checking if raw data is available")
 if X_is_raw(atac):
+    L.info("Saving raw counts from .X to .layers['raw_counts']")
     atac.layers["raw_counts"] = atac.X.copy()
-elif "raw_counts" in atac.layers :
-    L.info("raw_counts layer already exists")
+elif "raw_counts" in atac.layers:
+    L.info(".layers['raw_counts'] already exists and copying it to .X")
+    atac.X = atac.layers['raw_counts'].copy()
 else:
     L.error("X is not raw data and raw_counts layer not found")
     sys.exit("X is not raw data and raw_counts layer not found")
 
 
 # NORMALIZE
 if X_is_raw(atac):
     if args.binarize is True:
-        L.info("binarizing peak count matrix")
+        L.info("Binarizing peak count matrix")
         ac.pp.binarize(atac)    
 
     if args.normalize is not None:
+        L.info("Normalizing data")
         if args.normalize == "log1p":
             if args.binarize:
                 L.warning("Careful, you have decided to binarize data but also to normalize per cell and log1p. Not sure this is meaningful")
             sc.pp.normalize_per_cell(atac,counts_per_cell_after=1e4)
             sc.pp.log1p(atac)
+            L.info("Saving normalized counts to layer 'logged_counts'")
             atac.layers["logged_counts"] = atac.X.copy()
         elif args.normalize == "TFIDF":
             if args.TFIDF_flavour=="signac":
                 ac.pp.tfidf(atac, scale_factor=1e4, log_tfidf=True, log_tf=False, log_idf=False)
+                L.info("Saving normalized counts to layer 'signac_norm'")
                 atac.layers["signac_norm"] = atac.X.copy()
             elif args.TFIDF_flavour=="logTF":
-                ac.pp.tfidf(atac, scale_factor=1e4, log_tfidf=False, log_tf=True, log_idf=False)    
+                ac.pp.tfidf(atac, scale_factor=1e4, log_tfidf=False, log_tf=True, log_idf=False)  
+                L.info("Saving normalized counts to layer 'logTF_norm'")  
                 atac.layers["logTF_norm"] = atac.X.copy()
             elif args.TFIDF_flavour=="logIDF":
                 ac.pp.tfidf(atac, scale_factor=1e4, log_tfidf=False, log_tf=False, log_idf=True)
+                L.info("Saving normalized counts to layer 'logIDF_norm'")
                 atac.layers["logIDF_norm"] = atac.X.copy()
     else: 
-        L.error("We Require a normalization strategy for ATAC")
-        sys.exit("Exiting because no normalization was specified. If None was intended, check your pipeline.yml file")
+        L.error("A normalization strategy is needed for ATAC. For that, please specify the 'normalize' parameter in the pipeline.yml")
+        sys.exit("A normalization strategy is needed for ATAC. For that, please specify the 'normalize' parameter in the pipeline.yml")
 
 
 #highly variable feature selection
 if "highly_variable" in atac.var: 
     L.warning( "You have %s Highly Variable Features", np.sum(atac.var.highly_variable))
 else:
-
     if args.feature_selection_flavour == "scanpy":
+        L.info("Running HVF selection")
         if args.n_top_features is None:
             sc.pp.highly_variable_genes(atac, min_mean=float(args.min_mean), 
             max_mean=float(args.max_mean), min_disp=float(args.min_disp))
         else:
             sc.pp.highly_variable_genes(atac, n_top_genes=int(args.n_top_features))
     elif args.feature_selection_flavour == "signac":
+        L.info("Running HVF selection")
         findTopFeatures_pseudo_signac(atac, args.min_cutoff)
     else:
         L.warning("No highly variable feature selection was performed!")
 
 if "highly_variable" in atac.var: 
     L.warning( "You have %s Highly Variable Features", np.sum(atac.var.highly_variable))
 
 # filter by hvgs
-filter_by_hvgs = args.filter_by_hvf
+if args.filter_by_hvf == "False": 
+    filter_by_hvgs = False
+elif args.filter_by_hvf == "True":
+    filter_by_hvgs = True
+else: 
+    filter_by_hvgs = args.filter_by_hvf
 
 if filter_by_hvgs:
-    L.info("filtering object to only include highly variable features")
+    L.info("Subsetting object to only include HVGs")
     mdata.mod["atac"] = atac[:, atac.var.highly_variable]
     if isinstance(mdata, mu.MuData):
         mdata.update()
     atac = mdata["atac"]
     genes = atac.var
     genes['gene_name'] = atac.var.index
     genes.to_csv("filtered_variable_features.tsv", sep="\t", index=True)
 
 # The combined steps of TF-IDF followed by SVD are known as latent semantic indexing (LSI), 
 # and were first introduced for the analysis of scATAC-seq data by Cusanovich et al. 2015.
 
 if args.dimred == "LSI" and args.normalize == "TFIDF":
+    L.info("Running LSI")
     lsi(adata=atac, num_components=int(args.n_comps))
-else:
+elif args.dimred == "LSI" and args.normalize == "log1p":
     L.info("Applying LSI on logged_counts is not recommended. Changing dimred to PCA")
     args.dimred = "PCA"
 if args.dimred == "PCA":
+    L.info("Scaling data")
     sc.pp.scale(atac)
+    L.info("Saving scaled counts to layer 'scaled_counts'")
     atac.layers["scaled_counts"] = atac.X.copy()
+    L.info("Running PCA")
     sc.tl.pca(atac, n_comps=int(args.n_comps), svd_solver=args.solver, 
     random_state=0)
 
 col_variables = args.color_by.split(",")
 col_variables = [a.strip() for a in col_variables]
 col_use = [var for var in col_variables if var in atac.obs.columns]
 
 #some plotting before removing the components
 
 if args.dimred =='PCA':
+    L.info("Plotting PCA")
     sc.pl.pca_variance_ratio(atac, log=True, n_pcs=int(args.n_comps), save=".png")
     sc.pl.pca(atac, color=col_use, save = "_vars.png")
     sc.pl.pca_loadings(atac, components="1,2,3,4,5,6", save = ".png")
     sc.pl.pca_overview(atac, save = ".png")
 if args.dimred =='LSI':
+    L.info("Plotting LSI")
     sc.pl.embedding(atac, color=col_use,basis="X_lsi", save = ".png")
     correlation_df = calc_tech_corr(extract_lsi(atac), 
         tech_covariates = ['n_genes_by_counts', 'total_counts'])
 
     correlation_df.to_csv(os.path.join(args.figdir,"tech_covariates_corr_LSI.tsv"), sep='\t')
 
     plot_lsi_corr(correlation_df, tech_covariates=['n_genes_by_counts', 'total_counts'],
         filename=os.path.join(args.figdir,"LSI_corr_plot.png"))
 
 
 if args.dim_remove is not None:
-    L.info("removing component from dimred")
+    L.info("Removing component %s from %s" % (args.dim_remove, args.dimred))
     dimrem=int(args.dim_remove)
     if args.dimred == "LSI":
         atac.obsm['X_lsi'] = atac.obsm['X_lsi'][:,dimrem:]
         atac.varm["LSI"] = atac.varm["LSI"][:,dimrem:]
         atac.uns["lsi"]["stdev"] = atac.uns["lsi"]["stdev"][dimrem:]
     if args.dimred == "PCA":
         atac.obsm['X_pca'] = atac.obsm['X_pca'][:,dimrem:]
         atac.varm["PCs"] = atac.varm["PCs"][:,dimrem:]
         
 mdata.update()
+L.info("Saving updated MuData to '%s'" % args.output_mudata)
 mdata.write(args.output_mudata)
 
 L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/run_preprocess_prot.py` & `panpipes-0.5.0/panpipes/python_scripts/run_preprocess_prot.py`

 * *Files 7% similar despite different names*

```diff
@@ -63,77 +63,81 @@
                     help="which PCA solver to use")
 parser.add_argument("--color_by",
                     default="sample_id",
                     help="which columns to fetch from the protein .obs slot")
 
 
 args, opt = parser.parse_known_args()
-# args = argparse.Namespace(filtered_mudata='test.h5mu', 
-# bg_mudata='/well/cartography/users/zsj686/non_cart_projects/005-multimodal_scpipelines/ingest/test_raw.h5mu', 
-# channel_col=None, normalisation_methods='clr,dsb', clr_margin='0', quantile_clipping='True', figpath='./figures/prot', save_mtx=False, save_mudata_path='test.h5mu')
 save_mtx=pnp.pp.check_for_bool(args.save_mtx)
 
 norm_methods = args.normalisation_methods.split(',')
 
 
-L.info(args)
+L.info("Running with params: %s", args)
 
 figdir = args.figpath
 if not os.path.exists(figdir):
     os.mkdir(figdir)
 
 sc.settings.figdir = figdir
 sc.set_figure_params(scanpy=True, fontsize=14, dpi=300, facecolor='white', figsize=(5,5))
 
 
-
 # load filtered data - if use_muon is True this will return a mudata object, else returns an mudata object
-
-L.info("reading filtered mudata object")
+L.info("Reading in MuData from '%s'" % args.filtered_mudata)
 try:
     all_mdata = mu.read(args.filtered_mudata)
 except FileNotFoundError:
+    L.error("filtered_mudata file not found")
     sys.exit("filtered_mudata file not found")
 
 # load bg data
 if 'dsb' in norm_methods:
     if args.bg_mudata is not None:
-        L.info("reading bg file object")
+        L.info("Reading in background MuData from " + args.bg_mudata)
         try:
             all_mdata_bg = mu.read(args.bg_mudata)
             # subset to just the channel 
         except FileNotFoundError:
-            sys.exit("bg_mudata object not found")
+            L.error("Background MuData object not found in " + args.bg_mudata)
+            sys.exit("Background MuData object not found in " + args.bg_mudata)
     else:
-        sys.exit("must specify a bg mudata to run dsb, containing both rna and prot")
+        L.error("You must specify a background MuData to run dsb, containing both rna and prot")
+        sys.exit("You must specify a background MuData to run dsb, containing both rna and prot")
     
-    # checking that the samne proteins are in foreground and background (since foreground might have been filtered)
+    # checking that the same proteins are in foreground and background (since foreground might have been filtered)
+    L.info("Checking that the same proteins are in foreground and background")
     if len(all_mdata['prot'].var_names) != len(all_mdata_bg['prot'].var_names):
         mu.pp.filter_var(all_mdata_bg['prot'], all_mdata['prot'].var_names)
         all_mdata_bg.update()
 
 
 # find isotypes columns 
+L.info("Looking for isotypes column in .var['isotype']")
 if "isotype" in all_mdata["prot"].var.columns:
     isotypes = list(all_mdata["prot"].var_names[all_mdata["prot"].var.isotype])
     # exclude isotypes from downstream analysis by setting them as the only not highly variable genes.
+    L.info("Excluding isotypes from downstream analysis by setting them as the only not HVGs")
     all_mdata['prot'].var['highly_variable'] = ~all_mdata['prot'].var['isotype'] 
 else:
+    L.info("No isotype column found in .var")
     isotypes = None
     
-L.info("isotypes found:")
+L.info("The following isotypes were found:")
 L.info(isotypes)
 
 
 # save raw counts
+L.info("Checking if raw data is available")
 if pnp.scmethods.X_is_raw(all_mdata["prot"]):
+    L.info("Saving raw counts from .X to .layers['raw_counts']")
     all_mdata["prot"].layers["raw_counts"] = all_mdata["prot"].X.copy()
 elif "raw_counts" in all_mdata["prot"].layers :
-    L.info("raw_counts layer already exists")
-    all_mdata.X = all_mdata["prot"].layers['raw_counts'].copy()
+    L.info(".layers['raw_counts'] already exists and copying it to .X")
+    all_mdata["prot"].X = all_mdata["prot"].layers['raw_counts'].copy()
 else:
     L.error("X is not raw data and raw_counts layer not found")
     sys.exit("X is not raw data and raw_counts layer not found")
 
 
 
 if args.channel_col is not None:
@@ -203,18 +207,20 @@
     plot_features.sort()
     plot_features = [x for x in plot_features if x not in isotypes]
     if 'clr' in norm_methods:
         # make sure to start from raw counts
         all_mdata["prot"].X = all_mdata["prot"].layers["raw_counts"].copy()
         # run normalise
         # this stores a layer named after the method as well as overwriting X
+        L.info("Normalizing data with CLR")
         pnp.scmethods.run_prot_normalise(mdata=all_mdata, 
                 mdata_bg=None,
                 method="clr",
                 clr_margin=int(args.clr_margin))
+        L.info("Plotting Ridgeplot")
         pnp.plotting.ridgeplot(all_mdata["prot"], features=plot_features, layer="clr",  splitplot=6)
         plt.savefig(os.path.join(args.figpath, "clr_ridgeplot.png"))
         if isotypes is not None:
             pnp.plotting.ridgeplot(all_mdata["prot"], features=isotypes, layer="clr",  splitplot=1)
             plt.savefig(os.path.join(args.figpath, "clr_ridgeplot_isotypes.png"))
         # save out the data in what format?
         if save_mtx:
@@ -224,23 +230,26 @@
         all_mdata["prot"].X = all_mdata["prot"].layers["raw_counts"].copy()
         # then run dsb
         # comput log 10 umi
         all_mdata_bg["rna"].obs["log10umi"] = np.array(np.log10(all_mdata_bg["rna"].X.sum(axis=1) + 1)).reshape(-1)
         mu.pl.histogram(all_mdata_bg["rna"], ["log10umi"], bins=50)
         plt.savefig(os.path.join(args.figpath, "all_log10umi.png"))
         # this stores a layer named after the method as well as overwriting X
+        L.info("Normalizing data with dsb")
         pnp.scmethods.run_prot_normalise(mdata=all_mdata, 
                 mdata_bg=all_mdata_bg, 
                 method="dsb",
                 isotypes=isotypes) 
         # apply quantile clipping # discussed in FAQs https://cran.r-project.org/web/packages/dsb/vignettes/dsb_normalizing_CITEseq_data.html
         if args.quantile_clipping:
+            L.info("Quantile clipping")
             all_mdata['prot'].layers['dsb'] = pnp.scmethods.quantile_clipping(all_mdata['prot'], layer="dsb", inplace=False)
             all_mdata['prot'].X = all_mdata['prot'].layers['dsb'].copy()
         # plot ridgeplot
+        L.info("Plotting Ridgeplot")
         pnp.plotting.ridgeplot(all_mdata["prot"], features=plot_features, layer="dsb",  splitplot=6)
         plt.savefig(os.path.join(args.figpath, "dsb_ridgeplot.png"))
         if isotypes is not None:
             pnp.plotting.ridgeplot(all_mdata["prot"], features=isotypes, layer="dsb",  splitplot=1)
             plt.savefig(os.path.join(args.figpath, "dsb_ridgeplot_isotypes.png"))
         # save out the data in what format?
         if save_mtx:
@@ -248,46 +257,41 @@
     
     if args.store_as_x is not None:
         all_mdata["prot"].X = all_mdata["prot"].layers[args.store_as_x]
         
     # run pca on X 
     # this basically makes no sense if you have a small panel of antibodies.
     if args.run_pca:
-        L.info("running pca")
+        L.info("Running PCA")
 
         if all_mdata['prot'].var.shape[0] < int(args.n_pcs):
-            L.info("You have less features than number of PCs you intend to calculate")
+            L.warning("You have less features (%s) than number of PCs (%t) you intend to calculate." % (all_mdata['prot'].var.shape[0], args.n_pcs))
             n_pcs = all_mdata['prot'].var.shape[0] - 1
-            L.info("Setting n PCS to %i" % int(n_pcs))
+            L.info("Setting number of PCS to %i" % int(n_pcs))
         else:
             n_pcs = int(args.n_pcs)
         sc.tl.pca(all_mdata['prot'], n_comps=n_pcs, 
                         svd_solver=args.pca_solver, 
                         random_state=0) 
 
         # do some plots!
+        L.info("Plotting PCA")
         sc.pl.pca_variance_ratio(all_mdata['prot'], log=True, n_pcs=n_pcs, save=".png")
         
-        L.info(args.color_by)
         
         col_variables = args.color_by.split(",")
-        L.info("col_variables")
-        L.info(col_variables)
         
         col_variables = [a.strip() for a in col_variables]
-
-        L.info("col_variables now")
-        L.info(col_variables)
         
         col_use = [var for var in col_variables if var in all_mdata['prot'].obs.columns]
-        L.info("col_use")
-        L.info(col_use)
+
         sc.pl.pca(all_mdata['prot'], color=col_use, save = "_vars.png")
         sc.pl.pca_loadings(all_mdata['prot'], components="1,2,3,4,5,6", save = ".png")
         sc.pl.pca_overview(all_mdata['prot'], save = ".png")
 
     if args.save_mudata_path is not None:
         all_mdata.update()
+        L.info("Saving updated MuData to '%s'" % args.save_mudata_path)
         all_mdata.write(args.save_mudata_path)
 
 
-L.info("done")
+L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/run_preprocess_rna.py` & `panpipes-0.5.0/panpipes/python_scripts/run_preprocess_rna.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,63 +67,66 @@
 # pca options
 parser.add_argument("--n_pcs", default=50)
 parser.add_argument("--pca_solver", default="arpack")
 parser.add_argument("--color_by", default="batch") 
 
 parser.set_defaults(verbose=True)
 args, opt = parser.parse_known_args()
-L.info(args)
+L.info("Running with params: %s", args)
 
 figdir = args.fig_dir
 if not os.path.exists(figdir):
     os.mkdir(figdir)
 
 sc.settings.figdir = figdir
 sc.set_figure_params(scanpy=True, fontsize=14, dpi=300, facecolor='white', figsize=(5,5))
 
+L.info("Reading in MuData from '%s'" % args.input_mudata)
 mdata = mu.read(args.input_mudata)
 
 # if we have actually loaded an anndata object, make into a mudata
 if isinstance(mdata, sc.AnnData):
     mdata =  mu.MuData({'rna': mdata})
 
 adata = mdata['rna']
 # resolve multi-column batch for hvg batch key
 if args.hvg_batch_key is not None:
     columns = [x.strip() for x in args.hvg_batch_key.split(",")]
     if len(columns) > 1: 
-        L.info("combining batch columns into one column 'hvg_batch_key'")
+        L.info("Combining batch columns into one column 'hvg_batch_key'")
         adata.obs["hvg_batch_key"] = adata.obs[columns].apply(lambda x: '|'.join(x), axis=1)
         # make sure that batch is a categorical
         adata.obs["hvg_batch_key"] = adata.obs["hvg_batch_key"].astype("category")
         hvg_batch_key="hvg_batch_key"
     else:
         hvg_batch_key=columns[0]
 else:
     hvg_batch_key=None
 
 # save raw counts as a layer
+L.info("Checking if raw data is available")
 if X_is_raw(adata):
+    L.info("Saving raw counts from .X to .layers['raw_counts']")
     adata.layers['raw_counts'] = adata.X.copy()
 elif "raw_counts" in adata.layers :
-    L.info("raw_counts layer already exists")
+    L.info(".layers['raw_counts'] already exists and copying it to .X")
     adata.X = adata.layers['raw_counts'].copy()
 else:
     L.error("X is not raw data and raw_counts layer not found")
     sys.exit("X is not raw data and raw_counts layer not found")
 
 
 # sc.pp.highly variable genes Expects logarithmized data, 
 # except when flavor='seurat_v3' in which count data is expected.
 # change the order accordingly
 if X_is_raw(adata):
-    L.info("normalise, log and calculate highly variable genes")
+    L.info("Normalize, log and calculate HVGs")
     if args.flavor == "seurat_v3":
         if args.n_top_genes is None:
-            raise ValueError("if seurat_v3 is used you must give a n_top_genes value")
+            raise ValueError("If seurat_v3 is used, you must give a n_top_genes value")
         else:
             sc.pp.highly_variable_genes(adata, flavor="seurat_v3", 
                                         n_top_genes=int(args.n_top_genes),
                                         batch_key=hvg_batch_key)
         sc.pp.normalize_total(adata, target_sum=1e4)
         sc.pp.log1p(adata)
     else:
@@ -132,113 +135,109 @@
         L.debug(adata.uns['log1p'])
         sc.pp.highly_variable_genes(adata, flavor=args.flavor,
                                     min_mean=float(args.min_mean), 
                                     max_mean=float(args.max_mean),
                                     min_disp=float(args.min_disp),
                                     batch_key=hvg_batch_key)
         L.debug(adata.uns['log1p'])
+
 if "highly_variable" in adata.var: 
-    L.warning( "You have %s Highly Variable Features", np.sum(adata.var.highly_variable))
+    L.info( "You have %s HVGs", np.sum(adata.var.highly_variable))
     sc.pl.highly_variable_genes(adata,show=False, save ="_genes_highlyvar.png")
-else:
-    sys.exit("I cannot find Highly Variable Features in your RNA")
 
 if isinstance(mdata, mu.MuData):
     mdata.update()
 
 # exclude hvgs if there is an exclude file
 if args.exclude_file is not None:
     if os.path.exists(args.exclude_file):
-        L.info("exclude genes from hvg")
+        L.info("Reading in exclude_file from '%s'" % args.exclude_file)
         customgenes = pd.read_csv(args.exclude_file) 
         custom_cat = list(set(customgenes['group'].tolist()))
         cat_dic = {}
         for cc in custom_cat:
             cat_dic[cc] = customgenes.loc[customgenes["group"] == cc,"feature"].tolist()
         exclude_action = str(args.exclude)
         excl = cat_dic[exclude_action]
-        L.info(len(excl))
-        L.info("number of hvgs prior to filtering")
-        L.info(adata.var.highly_variable.sum())
+        L.info("Number of HVGs prior to filtering: %s" % adata.var.highly_variable.sum())
         adata.var['hvg_exclude'] = [True if gg in excl else False for gg in adata.var.index]
-        L.debug("num to exclude %s" %  (adata.var['hvg_exclude'] & adata.var['highly_variable']).sum() )
-        L.debug(adata)
+        L.info("Number of genes to exclude %s" %  (adata.var['hvg_exclude'] & adata.var['highly_variable']).sum() )
+        L.info("Excluding genes from HVG")
         if any(adata.var['hvg_exclude'] & adata.var['highly_variable']):
             adata.var['highly_variable'].loc[adata.var.hvg_exclude] = False
             adata.var.loc[adata.var.hvg_exclude, 'highly_variable_rank'] = np.nan
             
-            L.info("number of hvgs after filtering")
-            L.info(adata.var.highly_variable.sum())
+            L.info("Number of HVGs after filtering: %s" % adata.var.highly_variable.sum())
             sc.pl.highly_variable_genes(adata,show=False, save ="_exclude_genes_highlyvar.png")
     else:
-        sys.exit("exclusion file %s not found, check the path and try again" % args.exclude_file)
+        L.error("Exclusion file %s not found" % args.exclude_file)
+        sys.exit("Exclusion file %s not found" % args.exclude_file)
 
 if isinstance(mdata, mu.MuData):
     mdata.update()
 
-L.debug(adata.uns['log1p'])
+
 # filter by hvgs
 filter_by_hvgs = args.filter_by_hvg
 
 if filter_by_hvgs is True:
-    L.info("filtering object to only include highly variable genes")
+    L.info("Subsetting object to only include HVGs")
     mdata.mod["rna"] = adata[:, adata.var.highly_variable]
     if isinstance(mdata, mu.MuData):
         mdata.update()
     adata = mdata.mod["rna"]
     genes = adata.var
     genes['gene_name'] = adata.var.index
     genes.to_csv("filtered_genes.tsv", sep="\t", index=True)
  
 
 adata.layers['logged_counts'] = adata.X.copy()
-L.debug(adata.uns['log1p'])
 # regress out
 if args.regress_out is not None:
+    L.info("Regressing out %s" % args.regress_out)
     regress_opts = args.regress_out.split(",")
-    L.info("regressing out %s" % regress_opts)
     sc.pp.regress_out(adata, regress_opts)
 
 
 if args.scale is True and args.scale_max_value is None:
-    L.info("scaling data with default parameters")
+    L.info("Scaling data with default parameters")
     sc.pp.scale(adata)
 elif args.scale is True:
-    L.info("scaling data to max value %i" % int(args.scale_max_value))
+    L.info("Scaling data to max value %i" % int(args.scale_max_value))
     sc.pp.scale(adata, max_value=int(args.scale_max_value))
 else:
-    L.info("not scaling data")
-    pass
+    L.info("Not scaling the data")
+    #pass
+
 
-L.debug(adata.uns['log1p'])
 # run pca
-L.info("running pca")
+L.info("Running PCA")
 
 if adata.var.shape[0] < int(args.n_pcs):
-    L.info("You have less features than number of PCs you intend to calculate")
+    L.warning("You have less features (%s) than number of PCs (%s) you intend to calculate." % (adata.var.shape[0], args.n_pcs))
     n_pcs = adata.var.shape[0] - 1
-    L.info("Setting n PCS to %i" % int(n_pcs))    
+    L.info("Setting number of PCS to %i" % int(n_pcs))    
 else:
     n_pcs = int(args.n_pcs)
 sc.tl.pca(adata, n_comps=n_pcs, 
                 svd_solver=args.pca_solver, 
                 random_state=0) 
 
-# do some plots!
+# pca plots
+L.info("Plotting PCA")
 sc.pl.pca_variance_ratio(adata, log=True, n_pcs=n_pcs, save=".png")
 
 col_variables = args.color_by.split(",")
 col_variables = [a.strip() for a in col_variables]
 
 col_use = [var for var in col_variables if var in adata.obs.columns]
 sc.pl.pca(adata, color=col_use, save = "_vars.png")
 sc.pl.pca_loadings(adata, components="1,2,3,4,5,6", save = ".png")
 sc.pl.pca_overview(adata, save = ".png")
 
 
 mdata.update()
 # save the scaled adata object
-
+L.info("Saving updated MuData to '%s'" % args.output_scaled_mudata)
 mdata.write(args.output_scaled_mudata)
-L.debug(adata.uns['log1p'])
 
-L.info("done")
+L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/run_preprocess_spatial.py` & `panpipes-0.5.0/panpipes/python_scripts/run_preprocess_spatial.py`

 * *Files 18% similar despite different names*

```diff
@@ -74,96 +74,106 @@
 parser.add_argument("--n_pcs",
                     default=50,
                     help="how many PCs to compute")
 
 
 args, opt = parser.parse_known_args()
 
-L.info("running with args:")
-L.info(args)
+L.info("Running with params: %s", args)
 
 figdir = args.figdir
 
 if not os.path.exists(figdir):
     os.mkdir(figdir)
 
 sc.settings.figdir = figdir
 sc.set_figure_params(scanpy=True, fontsize=14, dpi=300, facecolor='white', figsize=(5,5))
 
+L.info("Reading in MuData from '%s'" % args.input_mudata)
 mdata = mu.read(args.input_mudata)
 spatial = mdata.mod['spatial']
 
 input_data = os.path.basename(args.input_mudata)
 pattern = r"_filtered.h5(.*)"
 match = re.search(pattern, input_data)
 sprefix = input_data[:match.start()]
 
 
 # check if raw data is available
 #maybe layer of raw data as parameter
+L.info("Checking if raw data is available")
 if X_is_raw(spatial):
+    L.info("Saving raw counts from .X to .layers['raw_counts']")
     spatial.layers['raw_counts'] = spatial.X.copy()
 elif "raw_counts" in spatial.layers :
-    L.info("raw_counts layer already exists")
+    L.info(".layers['raw_counts'] already exists and copying it to .X")
     spatial.X = spatial.layers['raw_counts'].copy()
 else:
     L.error("X is not raw data and 'raw_counts' layer not found")
     sys.exit("X is not raw data and 'raw_counts' layer not found")
 
 
-
 # Normalization + HVG selection based on flavour
 if args.norm_hvg_flavour == "squidpy":
     if args.squidpy_hvg_flavour == "seurat_v3":
+        L.info("Running HVG selection with flavor seurat_v3")
         sc.pp.highly_variable_genes(spatial, flavor="seurat_v3", n_top_genes=int(args.n_top_genes), subset=args.filter_by_hvg,
                                     batch_key=args.hvg_batch_key)
+        L.info("Log-normalizing data")
         sc.pp.normalize_total(spatial)
         sc.pp.log1p(spatial)
     else:
+        L.info("Log-normalizing data")
         sc.pp.normalize_total(spatial)
         sc.pp.log1p(spatial)
+        L.info("Running HVG selection with flavor %s" % args.squidpy_hvg_flavour)
         sc.pp.highly_variable_genes(spatial, flavor=args.squidpy_hvg_flavour,
                                     min_mean=float(args.min_mean),
                                     max_mean=float(args.max_mean),
                                     min_disp=float(args.min_disp), subset=args.filter_by_hvg, batch_key=args.hvg_batch_key)
+    L.info("Saving log-normalized counts to .layers['lognorm']")
     spatial.layers["lognorm"] = spatial.X.copy()
     # plot HVGs:
     sc.pl.highly_variable_genes(spatial, show=False, save="_genes_highlyvar" + "."+ sprefix+ ".png")
 
 elif args.norm_hvg_flavour == "seurat":
     if args.clip is None:
         clip = args.clip
     elif args.clip == "None":
         clip = None
     elif args.clip == "np.Inf":
         clip = np.Inf
     else:
         clip = float(args.clip)
-
+    L.info("Running Pearson Residuals HVG selection")
     sce.pp.highly_variable_genes(spatial, theta=float(args.theta), clip=clip, n_top_genes=int(args.n_top_genes),
                                  batch_key=args.hvg_batch_key, flavor='pearson_residuals',
                                  layer="raw_counts", subset=args.filter_by_hvg)
-    
+    L.info("Running Pearson Residuals normalization")
     sce.pp.normalize_pearson_residuals(spatial, theta=float(args.theta), clip=clip, layer="raw_counts")
+    L.info("Saving log-normalized counts to .layers['norm_pearson_resid']")
     spatial.layers["norm_pearson_resid"] = spatial.X.copy()
 else:
     # error or warning?
     L.warning("No normalization and HVG selection was performed! To perform, please specify the 'norm_hvg_flavour' as either 'squidpy' or 'seurat'")
 
 
 if "highly_variable" in spatial.var:
-    L.warning( "You have %s Highly Variable Features", np.sum(spatial.var.highly_variable))
+    L.info("You have %s Highly Variable Features", np.sum(spatial.var.highly_variable))
 
 
 
 #PCA
+L.info("Running PCA")
 sc.pp.pca(spatial, n_comps=int(args.n_pcs), svd_solver='arpack', random_state=0)
+L.info("Plotting PCA")
 sc.pl.pca(spatial, save = "_vars" + "."+ sprefix+".png")
 sc.pl.pca_variance_ratio(spatial, log=True, n_pcs=int(args.n_pcs), save= "."+ sprefix+".png")
 
 
         
 mdata.update()
+L.info("Saving updated MuData to '%s'" % args.output_mudata)
 mdata.write(args.output_mudata)
 
 L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/run_scanpyQC_atac.py` & `panpipes-0.5.0/panpipes/python_scripts/run_scanpyQC_atac.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 import logging
 L = logging.getLogger()
 L.setLevel(logging.INFO)
 log_handler = logging.StreamHandler(sys.stdout)
 formatter = logging.Formatter('%(asctime)s: %(levelname)s - %(message)s')
 log_handler.setFormatter(formatter)
 L.addHandler(log_handler)
-L.debug("testing logger works")
 
 from panpipes.funcs.io import  write_obs
 from panpipes.funcs.processing import check_for_bool
 
 
 sc.settings.verbosity = 3
 
@@ -66,107 +65,120 @@
                     default="",
                     help="")
                 
 
 
 
 args, opt = parser.parse_known_args()
-
-L.info("running with args:")
-L.debug(args)
+L.info("Running with params: %s", args)
 
 figdir = args.figdir
 
 if not os.path.exists(figdir):
     os.mkdir(figdir)
 
 sc.settings.figdir = figdir
 sc.set_figure_params(scanpy=True, fontsize=14, dpi=300, facecolor='white', figsize=(5,5))
 args.is_paired= check_for_bool(args.is_paired)
 
 if args.is_paired:
     args.use_muon= True
     L.info("I'm working on a multiome experiment")
 else:
-    L.info("qc'ing an atac standalone assay")
+    L.info("QC'ing an atac standalone assay")
 
+L.info("Reading in MuData from '%s'" % args.input_anndata)
 mdata = mu.read(args.input_anndata)
 atac = mdata.mod['atac']
 
 
 # CALCULATE SOME GENERAL QC metrics
+L.info("Calculating QC metrics with scanpy.pp.calculate_qc_metrics()")
 sc.pp.calculate_qc_metrics(atac, percent_top=None, log1p=False, inplace=True)
 checkfiles = 'files' in list(atac.uns.keys()) 
 if checkfiles:
     if atac.uns["files"]["fragments"] is not None:
+        L.info("Computing nucleosome signal")
         ac.tl.nucleosome_signal(atac, n=1e6)
         atac.obs['NS']=np.where(atac.obs['nucleosome_signal'] >3, 'trinucleosome', 'mono_trinucleosome')
-        L.debug("added nucleosome signal to atac")
+        L.info("Plotting nucleosome signal as histogram")
         mu.pl.histogram(atac, "nucleosome_signal", groupby='NS')
         plt.savefig(os.path.join(figdir, "nucleosome.png"))
 
 
 if args.is_paired & checkfiles :
     if atac.uns["files"]["fragments"] is not None:
         #ac.tl.get_gene_annotation_from_rna(mdata['rna'])  # accepts MuData with 'rna' modality or mdata['rna'] AnnData directly if
+        L.info("Computing TSS enrichment")
         tss = ac.tl.tss_enrichment(mdata, n_tss=1000) # by default, features=ac.tl.get_gene_annotation_from_rna(mdata), but it could work with a custom annotation 
         tss.obs['tss_class'] = np.where(tss.obs["tss_score"]>2 , "High","Low") 
+        L.info("Plotting TSS enrichment")
         ac.pl.tss_enrichment(tss, color="tss_class")
         plt.savefig(os.path.join(figdir, "tss_enrichment.png"))
         mdata.mod["tss"] = tss # add the tss anndata to the mudata, no point in saving it outside
         
 else:
     #since we're here, change some names
     for col in atac.obs.columns:
         if "peak_region_fragments" in col:
+            L.info("Saving '%s' to column 'atac_peak_region_fragments'" % col)
             atac.obs["atac_peak_region_fragments"] = atac.obs[col]
         if col.endswith("mitochondrial"):
             if atac.obs["atac_mitochondrial_reads"] is not None:
+                L.info("Saving '%s' to column 'atac_mitochondrial_reads'" % col)
                 atac.obs["atac_mitochondrial_reads"] = atac.obs[col]
-        if col.endswith("passed_filters"):  
+        if col.endswith("passed_filters"): 
+            L.info("Saving '%s' to column 'atac_fragments'" % col) 
             atac.obs['atac_fragments']= atac.obs[col]
     
     if args.paired_rna is not None:
+        L.info("Reading in paired RNA data from '%s" % args.paired_rna)
         rna = mu.read(args.paired_rna)
+        L.info("Running muon.atac.tl.get_gene_annotation_from_rna()")
         tss_features = ac.tl.get_gene_annotation_from_rna(rna)
     elif args.tss_coordinates is not None:
+        L.info("Reading in TSS features from '%s'" % args.tss_coordinates)
         tss_features = pd.read_csv(args.tss_coordinates, index_col=0, sep="\t")
-    
+        L.info("Computing TSS enrichment with features from tsv file")
         tss_data = ac.tl.tss_enrichment(atac, features= tss_features, n_tss=1000)
+        L.info("Creating column 'tss_class' in .obs")
         tss_data.obs['tss_class'] = np.where(tss_data.obs["tss_score"]>2 , "High","Low") 
+        L.info("Plotting TSS enrichment")
         ac.pl.tss_enrichment(tss_data, color="tss_class")
         plt.savefig(os.path.join(figdir, "tss_enrichment.png"))
         mdata.mod["tss"] = tss_data
     
 if args.paired_rna is None :
     if args.tss_coordinates is None:
-        L.warning("""you didn't provide an rna anndata or the features coordinate files to
-        run the tss enrichment analysis, this will be skipped
+        L.warning("""No RNA AnnData and feature coordinate file was provided to
+        run the TSS enrichment analysis, this will be skipped
         """)
 
 # calc pct fragments in peaks 
 if "atac_fragments" in atac.obs.columns:
-    L.debug("adding percent fragments in peaks")
+    L.debug("Adding percent fragments in peaks")
     atac.obs['pct_fragments_in_peaks']=atac.obs['atac_peak_region_fragments']/atac.obs['atac_fragments'] *100          
 
 #PLOTS
 
+L.info("Plotting violin plots of QC vars")
 if args.atac_qc_metrics is not None:
     qc_vars=args.atac_qc_metrics.split(",")
     qc_vars= [a.strip() for a in qc_vars]
 else:
     qc_vars = ["n_genes_by_counts","total_counts","pct_fragments_in_peaks"]
 
 qc_vars_plot = [gg for gg in qc_vars if gg in atac.obs.columns]
 sc.pl.violin(atac, qc_vars_plot, 
              jitter=0.4, multi_panel=True, save = "atac_metrics_violin.png")
 
 mdata.update()
 
-L.info("saving mudata and obs in a metadata tsv file")
+L.info("Saving updated obs in a metadata tsv file to ./" + args.sampleprefix + "_cell_metadata.tsv")
 write_obs(mdata, output_prefix=args.sampleprefix, 
         output_suffix="_cell_metadata.tsv")
 
+L.info("Saving updated MuData to '%s'" % args.outfile)
 mdata.write(args.outfile)
 
 L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/run_scanpyQC_prot.py` & `panpipes-0.5.0/panpipes/python_scripts/run_scanpyQC_prot.py`

 * *Files 12% similar despite different names*

```diff
@@ -66,85 +66,88 @@
                     help="")
 parser.add_argument("--per_prot_metrics",
                     default=None,
                     help="")
 
 
 args, opt = parser.parse_known_args()
+L.info("Running with params: %s", args)
 
-L.info("Scanpy qc pipeline")
 sc.settings.verbosity = 3
-
-L.info("running with args:")
-L.info(args)
 figdir = args.figdir
 
 if not os.path.exists(figdir):
     os.mkdir(figdir)
 
 sc.settings.figdir = figdir
 sc.set_figure_params(scanpy=True, fontsize=14, dpi=300, facecolor='white', figsize=(5,5))
 
 
-
+L.info("Reading in MuData from '%s'" % args.input_anndata)
 mdata = mu.read(args.input_anndata)
 prot = mdata['prot']
 
 
 # determine what QC metrics we want
 if args.per_cell_metrics is not None:
     per_cell_metrics = args.per_cell_metrics.split(",")
     per_cell_metrics = [a.strip() for a in per_cell_metrics]
 
 
 
-
 # work out if we already have isotype column, if not try to infer from index.
+L.info("Looking for 'isotype' column in .var")
 if 'isotype' not in prot.var.columns:
     # this means that isotype column was not included in the protein conversion table 
     # so we are going to have a wwhack at identifying them
+    L.info("No 'isotype' column found in .var, adding 'isotype' column.")
     prot.var['isotype'] = prot.var_names.str.contains("isotype")
 else:
     # there is already an isotype column in var
-    L.info("isotype column already in var")
+    L.info("Isotype column found in var")
     pass
 
 # are there any actual isotypes though?
 isotypes = list(prot.var_names[prot.var.isotype].unique())
-L.info("n isotypes found in data %i" % len(isotypes))
+L.info("Number of isotypes found in data %i" % len(isotypes))
 if len(isotypes) > 0:
+    L.info("Including isotypes in QC metrics call")
     qc_vars=["isotype"]
 else:
+    L.info("Not including isotypes in QC metrics call")
     qc_vars=[]
 # if isotypes are found then include them in the caluclate qc metrics call.
 # this calculates standard metrics 
+
+L.info("Calculating QC metrics with scanpy.pp.calculate_qc_metrics()")
 sc.pp.calculate_qc_metrics(prot,
                         var_type="prot",  
                         qc_vars=qc_vars, 
                         percent_top=None,log1p=True, inplace=True)
 
 ## let's assess the isotype outlier cells. 
 #(Cells with an excessive amount of isotype indicating stickiness)
 if (len(isotypes) > 0) & check_for_bool(args.identify_isotype_outliers):
-    L.info("identifying isotype outliers")
+    L.info("Identifying isotype outliers")
     # this measn we found some isotypes earlier
     # we identify outliers on a per channel basis 
     # using the groupby argument
     identify_isotype_outliers(prot, isotypes, 
             quantile_val=float(args.isotype_upper_quantile),
             n_isotypes_pass=int(args.isotype_n_pass), 
             groupby=args.channel_col)
 
 mdata.update()
 
 # write out the cell_metadata
-logging.info("saving mudata and obs in a metadata tsv file")
+L.info("Saving updated obs in a metadata tsv file to ./" + args.sampleprefix + "_cell_metadata.tsv")
 write_obs(mdata, output_prefix=args.sampleprefix, 
         output_suffix="_cell_metadata.tsv")
 # write out whole object data.
+L.info("Saving updated MuData to '%s'" % args.outfile)
 mdata.write(args.outfile)
 
 
 
 
 # now run some per channel metrics - this is not stored in the final object.
 # the reason these are not run on the whole object is to get the "var_df" 
@@ -153,17 +156,18 @@
 
 # the rest of the script is concerned with Per PROT metrics instead of per cell. 
 # per cell metrics are plotted in plotqc.R
 
 
 channel_col = args.channel_col # TO DO why is this just not simply sample_id 
 
+L.info("Calculating per channel metrics for channel '%s'" % channel_col)
+
 out = {}
 for si in prot.obs[channel_col].unique():
-    L.info(si)
     obs_df, var_df = sc.pp.calculate_qc_metrics(prot[prot.obs[channel_col]==si],
                             var_type="prot", 
                             qc_vars=qc_vars, 
                             percent_top=None,log1p=True, inplace=False)
     # store the var df for the metrics we care about in the dictionary.
     out[si] = var_df.copy()
     # add an extra column t the var_df to indicate which channel the data came from
@@ -174,20 +178,22 @@
 prot_id_col=var_dat.columns[1]
 
 if args.per_prot_metrics is not None:
     per_prot_metrics = args.per_prot_metrics.split(",")
     per_prot_metrics = [a.strip() for a in per_prot_metrics]
 
     # let's make some boxplot figures.
+    L.info("Plotting per channel metrics in boxplots")
     for qcp in per_prot_metrics:
         fig, ax = plt.subplots(nrows=1,figsize=(24,6))
         sns.boxplot(data=var_dat, x=prot_id_col, y=qcp, ax=ax)
         adjust_x_axis(ax)
         fig.tight_layout()
         plt.savefig(os.path.join(figdir, "boxplot_" + channel_col + "_" + qcp + ".png"))
     plt.close()
 
     # write out the per channel metrics in a separate csv.
+    L.info("Saving per channel metrics to csv file '"+ args.sampleprefix + "_prot_qc_metrics_per_" + channel_col + ".csv'")
     var_dat.to_csv(args.sampleprefix + "_prot_qc_metrics_per_" + channel_col + ".csv")
 
 L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/run_scanpyQC_rep.py` & `panpipes-0.5.0/panpipes/python_scripts/run_scanpyQC_rep.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,45 +47,47 @@
                     help="what metrics to calculate sequence distance metric? \
                     any arguments from scirpy.pp.ir_dist as a dict in format'{arg: value}' ")
 parser.add_argument("--clonotype_metrics",
                     default=None,type=yaml.safe_load,
                     help="what metrics to calculate sequence distance metric? \
                     any arguments from scirpy.pp.define_clonotypes as a dict in format'{arg: value}' ")
 args, opt = parser.parse_known_args()
-L.info(args)
+L.info("Running with params: %s", args)
+
+L.info("Reading in MuData from '%s'" % args.input_mudata)
 mdata = mu.read(args.input_mudata)
 rep = mdata['rep']
 # chain qc
+L.info("Running scirpy.tl.chain_qc()")
 ir.tl.chain_qc(rep)
 
 # remove nones, so defaults are used
 if args.distance_metrics is not None:
     # remove nones, so defaults are used
     dist_args = {k: v for k, v in args.distance_metrics.items() if v != "None"}
     dist_args = {k: v for k, v in dist_args.items() if v}
 else:
     dist_args = {}
 
-L.info("distance args:")
-L.info(dist_args)
-
+L.info("Distance args: %s" % dist_args)
+L.info("Computing sequence-distance metric")
 ir.pp.ir_dist(rep, **dist_args)
 
 # pull function arguments from args. 
 if args.clonotype_metrics is not None:
     # remove nones, so defaults are used
     clonotype_args = {k: v for k, v in args.clonotype_metrics.items() if v != "None"}
     clonotype_args = {k: v for k, v in clonotype_args.items() if v}
 else:
     clonotype_args={}
 # define clonotypes
-L.info("clonotypes args:")
-L.info(clonotype_args)
-
+L.info("Clonotypes args: %s" % clonotype_args)
+L.info("Defining clonotypes")
 ir.tl.define_clonotypes(rep, **clonotype_args)
+L.info("Adding column to obs recording which clonotypes are expanded")
 ir.tl.clonal_expansion(rep)
 
     
 category_cols = ['has_ir']
 for cc in category_cols:
     if pd.api.types.infer_dtype(rep.obs[cc]) != "categorical":
         rep.obs[cc] = rep.obs[cc].astype('string').astype('category')
@@ -98,14 +100,15 @@
     
 if "TCR" in rep.obs.receptor_type.values:
     tcr = rep[rep.obs.receptor_type =="TCR", :].copy()
 else:
     tcr=None
 
 # plot group abundances
+L.info("Plotting group abundances")
 fig, ax = plt.subplots()
 ax = ir.pl.group_abundance(rep, groupby="receptor_type", ax=ax)
 fig.savefig(args.figdir +"/barplot_group_abundance_receptor_type.png", bbox_inches="tight")
 
 if bcr is not None:
     fig, ax = plt.subplots()
     ax = ir.pl.group_abundance(bcr, groupby="chain_pairing", ax=ax)
@@ -116,28 +119,31 @@
     fig, ax = plt.subplots()
     ax = ir.pl.group_abundance(tcr, groupby="chain_pairing",  ax=ax)
     fig.tight_layout()
     fig.savefig(args.figdir +"/barplot_group_abundance_tcr_receptor_subtype.png", bbox_inches="tight")
 
 # clonal expansion
 
+L.info("Plotting clonal expansion")
 clone_counts = rep.obs.groupby("receptor_type").clone_id.value_counts().to_frame("cell_counts").reset_index()
 
 if bcr is not None:
     ax = ir.pl.clonal_expansion(bcr, groupby="sample_id")
     ax.set_title("bcr clonal expansion")
     plt.savefig(args.figdir +"/barplot_clonal_expansion_bcr.png", bbox_inches="tight" )
 
 if tcr is not None:
     ax = ir.pl.clonal_expansion(tcr, groupby="sample_id")
     ax.set_title("tcr clonal expansion")
     plt.savefig(args.figdir +"/barplot_clonal_expansion_tcr.png", bbox_inches="tight")
 
 
-L.info("saving anndata and obs in a metadata tsv file")
+
 mdata.update()
+L.info("Saving updated obs in a metadata tsv file to ./" + args.sampleprefix + "_cell_metadata.tsv")
 write_obs(mdata, output_prefix=args.sampleprefix, 
     output_suffix="_cell_metadata.tsv")
+L.info("Saving updated MuData to '%s'" % args.output_mudata)
 mdata.write(args.output_mudata)
 
 L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/run_scanpyQC_rna.py` & `panpipes-0.5.0/panpipes/python_scripts/run_scanpyQC_rna.py`

 * *Files 13% similar despite different names*

```diff
@@ -57,41 +57,35 @@
                     default="mitochondrial,ribosomal",
                     help="which list of genes to use to calc proportion of mapped reads over total,per cell?")
 parser.add_argument("--score_genes",
                     default="MarkersNeutro",
                     help="which list of genes to use to scanpy.tl.score_genes per cell?")
 
 args, opt = parser.parse_known_args()
-
-L.info("Running scanpy rna qc pipeline")
+L.info("Running with params: %s", args)
 
 sc.settings.verbosity = 3
-
-
-L.info("running with args:")
-L.info(args)
 figdir = args.figdir
 
 if not os.path.exists(figdir):
     os.mkdir(figdir)
 
 sc.settings.figdir = figdir
 sc.set_figure_params(scanpy=True, fontsize=14, dpi=300, facecolor='white', figsize=(5,5))
 
 
-L.info("reading in data")
-
+L.info("Reading in MuData from '%s'" % args.input_anndata)
 mdata = mu.read(args.input_anndata)
 rna = mdata['rna']
 
 
-L.info("merge in the scrublet scores")
 # load the scrublet scores into the anndata (if they have been run)
 if args.scrubletdir is not None:
     scrub_dir = args.scrubletdir
+    L.info("Merging in the scrublet scores from directory '%s'" % args.scrubletdir)
     sample_ids = rna.obs[['sample_id']].drop_duplicates()
     [scrub_dir + '/' + ss + '_scrublet_scores.txt' for ss in sample_ids.sample_id]
     doubletscores = [pd.read_csv(scrub_dir + '/' + ss + '_scrublet_scores.txt', sep="\t", header=0) for ss in sample_ids.sample_id]
     doubletscores = pd.concat(doubletscores, keys=sample_ids.sample_id).reset_index(level="sample_id")
     # rename the barcodes to match up qwith what the rna.obs barcodes are
     if len(sample_ids) > 1:
         doubletscores['barcode'] = doubletscores['barcode'] + '-' + doubletscores['sample_id']
@@ -103,69 +97,80 @@
 # Cell-wise QC based on .var lists of genes 
 
 qc_vars = []
 
 if args.customgenesfile is not None:
     if os.path.exists(args.customgenesfile):
         cat_dic = {}
+        L.info("Reading in custom genes csv file from '%s'" % args.customgenesfile)
         customgenes = pd.read_csv(args.customgenesfile)
+        if not {'group', 'feature'}.issubset(customgenes.columns):
+            L.error("The custom genes file needs to have both columns, 'group' and 'feature'.")
+            sys.exit("The custom genes file needs to have both columns, 'group' and 'feature'.")
         custom_cat = list(set(customgenes['group'].tolist()))
         for cc in custom_cat:
             cat_dic[cc] = customgenes.loc[customgenes["group"] == cc,"feature"].tolist()
         if args.calc_proportions is not None:
             calc_proportions = args.calc_proportions.split(",")
             calc_proportions = [a.strip() for a in calc_proportions]
         else:
-            L.warn("I don't have genes to calc proportions for")
+            L.warning("No genes to calculate proportions for")
             
         if args.score_genes is not None:
             score_genes = args.score_genes.split(",")
             score_genes = [a.strip() for a in score_genes]
         else:
-            L.warn("I don't have genes to calc scores for")    
+            L.warning("No genes to calculate scores for")    
         
     else:
-
+        L.error("You have not provided a list of custom genes to use for QC purposes")
         sys.exit("You have not provided a list of custom genes to use for QC purposes")
 
 for kk in calc_proportions:
     xname= kk
     gene_list = cat_dic[kk]
     rna.var[xname] = [x in gene_list for x in rna.var_names] # annotate the group of hb genes as 'hb'
     qc_vars.append(xname)
 
+qc_info = ""
+if qc_vars != []:
+    qc_info = " and calculating proportions for '%s'" % qc_vars
+L.info("Calculating QC metrics with scanpy.pp.calculate_qc_metrics()" + qc_info)
 sc.pp.calculate_qc_metrics(rna, qc_vars=qc_vars, percent_top=None,log1p=True, inplace=True)
 
 if args.score_genes is not None:
     for kk in score_genes:
+        L.info("Computing gene scores for '%s'" % kk)
         xname= kk
         gene_list = cat_dic[kk]
         sc.tl.score_genes(rna, gene_list , 
                             ctrl_size=min(len(gene_list), 50), 
                             gene_pool=None, 
                             n_bins=25, 
                             score_name=kk + '_score', 
                             random_state=0, 
                             copy=False, 
                             use_raw=None)
 
 
 if args.ccgenes is not None:
+    L.info("Reading in cell cycle genes tsv file from '%s'" % args.ccgenes)
     ccgenes = pd.read_csv(args.ccgenes, sep='\t')
+    if not {'cc_phase', 'gene_name'}.issubset(ccgenes.columns):
+        L.error("The cell cycle genes file needs to have both columns, 'cc_phase' and 'gene_name'.")
+        sys.exit("The cell cycle genes file needs to have both columns, 'cc_phase' and 'gene_name'.")
     sgenes = ccgenes[ccgenes["cc_phase"] == "s"]["gene_name"].tolist()
     g2mgenes = ccgenes[ccgenes["cc_phase"] == "g2m"]["gene_name"].tolist()
+    L.info("Calculating cell cycle scores")
     sc.tl.score_genes_cell_cycle(rna, s_genes=sgenes, g2m_genes=g2mgenes)
 
 
-
-L.info("calculated scores and metrics")
-
 mdata.update()
 
-L.info("saving anndata and obs in a metadata tsv file")
+L.info("Saving updated obs in a metadata tsv file to ./" + args.sampleprefix + "_cell_metadata.tsv")
 write_obs(mdata, output_prefix=args.sampleprefix, 
         output_suffix="_cell_metadata.tsv")
-
+L.info("Saving updated MuData to '%s'" % args.outfile)
 mdata.write(args.outfile)
 
-L.info("done")
+L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/run_scanpyQC_spatial.py` & `panpipes-0.5.0/panpipes/python_scripts/run_scanpyQC_spatial.py`

 * *Files 24% similar despite different names*

```diff
@@ -47,115 +47,121 @@
                     help="which list of genes to use to calc proportion of mapped reads over total,per cell?")
 parser.add_argument("--score_genes",
                     default=None,
                     help="which list of genes to use to scanpy.tl.score_genes per cell?")
 
 args, opt = parser.parse_known_args()
 
-L.info("running scanpy spatial qc pipeline")
-
 sc.settings.verbosity = 3
 
 
-L.info("running with args:")
-L.info(args)
+L.info("Running with params: %s", args)
 figdir = args.figdir
 
 if not os.path.exists(figdir):
     os.mkdir(figdir)
 
 sc.settings.figdir = figdir
 sc.set_figure_params(scanpy=True, fontsize=14, dpi=300, facecolor='white', figsize=(5,5))
 
 
-L.info("reading in data")
+L.info("Reading in MuData from '%s'" % args.input_anndata)
 
 mdata = mu.read(args.input_anndata)
 spatial = mdata['spatial']
 
-L.info("spatial data is")
+L.info("Spatial data is:")
 print(spatial)
-L.info("sample id")
-print(spatial.obs["sample_id"])
+L.info("With sample id '%s'" % spatial.obs["sample_id"].unique()[0])
 
 qc_vars = []
 
 if args.customgenesfile is not None:
     if os.path.exists(args.customgenesfile):
+        L.info("Reading in custom genes file from '%s'" % args.customgenesfile)
         cat_dic = {}
         customgenes = pd.read_csv(args.customgenesfile)
+        if not {'group', 'feature'}.issubset(customgenes.columns):
+            L.error("The custom genes file needs to have both columns, 'group' and 'feature'.")
+            sys.exit("The custom genes file needs to have both columns, 'group' and 'feature'.")
         custom_cat = list(set(customgenes['group'].tolist()))
         for cc in custom_cat:
             cat_dic[cc] = customgenes.loc[customgenes["group"] == cc,"feature"].tolist()
             
         # define qc_vars 
         if args.calc_proportions is not None:
             calc_proportions = args.calc_proportions.split(",")
             calc_proportions = [a.strip() for a in calc_proportions]
             for kk in calc_proportions:
                 xname= kk
                 gene_list = cat_dic[kk]
                 spatial.var[xname] = [x in gene_list for x in spatial.var_names] 
                 qc_vars.append(xname)
-        else:
-            L.info("no genes to calc proportions for")
            
         # Score genes 
         if args.score_genes is not None:
             score_genes = args.score_genes.split(",")
             score_genes = [a.strip() for a in score_genes]
             for kk in score_genes:
+                L.info("Computing gene scores for '%s'" % kk)
                 xname= kk
                 gene_list = cat_dic[kk]
                 sc.tl.score_genes(spatial, gene_list , 
                                     ctrl_size=min(len(gene_list), 50), 
                                     gene_pool=None, 
                                     n_bins=25, 
                                     score_name=kk + '_score', 
                                     random_state=0, 
                                     copy=False, 
                                     use_raw=None)
-        else:
-            L.info("no genes to calc scores for")    
         
     else:
-        sys.exit("the path of the custom genes file does not exist")
+        L.error("The path of the custom genes file '%s' could not be found" % args.customgenesfile)
+        sys.exit("The path of the custom genes file '%s' could not be found" % args.customgenesfile)
 
         
         
         
 # Calculate QC metrics 
-L.info("calculating QC metrics")
+qc_info = ""
+if qc_vars != []:
+    qc_info = " and calculating proportions for '%s'" % qc_vars
+L.info("Calculating QC metrics with scanpy.pp.calculate_qc_metrics()" + qc_info)
 percent_top = [50, 100, 200, 500] #default
 percent_top = [x for x in percent_top if x <= spatial.n_vars]
 sc.pp.calculate_qc_metrics(spatial, qc_vars=qc_vars, percent_top=percent_top, inplace=True)
 
-if args.spatial_filetype == "vizgen":
+if (args.spatial_filetype == "vizgen") and ("blank_genes" in spatial.obsm):    
     spatial.obsm["blank_genes"].to_numpy().sum() / spatial.var["total_counts"].sum() * 100
 
 # Calculate cc scores 
 if args.ccgenes is not None:
-    ccgenes = pd.read_csv(args.ccgenes, sep='\t')
-    sgenes = ccgenes[ccgenes["cc_phase"] == "s"]["gene_name"].tolist()
-    g2mgenes = ccgenes[ccgenes["cc_phase"] == "g2m"]["gene_name"].tolist()
-    L.info("calculating CC scores")
-    sc.tl.score_genes_cell_cycle(spatial, s_genes=sgenes, g2m_genes=g2mgenes)
+    if os.path.exists(args.ccgenes):
+        L.info("Reading in cell cycle genes tsv file from '%s'" % args.ccgenes)
+        ccgenes = pd.read_csv(args.ccgenes, sep='\t')
+        if not {'cc_phase', 'gene_name'}.issubset(ccgenes.columns):
+            L.error("The cell cycle genes file needs to have both columns, 'cc_phase' and 'gene_name'.")
+            sys.exit("The cell cycle genes file needs to have both columns, 'cc_phase' and 'gene_name'.")
+        sgenes = ccgenes[ccgenes["cc_phase"] == "s"]["gene_name"].tolist()
+        g2mgenes = ccgenes[ccgenes["cc_phase"] == "g2m"]["gene_name"].tolist()
+        L.info("Calculating cell cycle scores")
+        sc.tl.score_genes_cell_cycle(spatial, s_genes=sgenes, g2m_genes=g2mgenes)
+    else: 
+        L.error("The path of the  cell cycle genes tsv file '%s' could not be found" % args.ccgenes)
+        sys.exit("The path of the  cell cycle genes tsv file '%s' could not be found" % args.ccgenes)
+
 
-# Aug 2023: we now need to update the mdata object to pick the calc proportion outputs made on 
+#TODO: we now need to update the mdata object to pick the calc proportion outputs made on 
 # spatial = mdata['spatial']
-print(spatial.obs.columns)
-print(mdata.obs.columns)
 
 mdata.update()
 
 single_id = os.path.basename(str(args.input_anndata))
 single_id = single_id.replace("_raw.h5mu","")
-L.info("updated metadata")
-print(mdata.obs.columns)
 
-L.info("saving obs in a metadata tsv file")
+L.info("Saving updated obs in a metadata tsv file to ./" + single_id + "_cell_metadata.tsv")
 write_obs(mdata, output_prefix=single_id, output_suffix="_cell_metadata.tsv")
-L.info("saving mudata")
+L.info("Saving updated MuData to '%s'" % args.outfile)
 mdata.write(args.outfile)
 
-L.info("done")
+L.info("Done")
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/run_scib_metrics.py` & `panpipes-0.5.0/panpipes/python_scripts/run_scib_metrics.py`

 * *Files identical despite different names*

### Comparing `panpipes-0.4.1/panpipes/python_scripts/run_scrublet_scores.py` & `panpipes-0.5.0/panpipes/python_scripts/run_scrublet_scores.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,18 +7,14 @@
 import os
 import argparse
 import muon as mu
 
 import sys
 import logging
 
-
-
-
-
 import matplotlib
 matplotlib.use('Agg')
 matplotlib.pyplot.ioff()
 
 L = logging.getLogger()
 L.setLevel(logging.INFO)
 log_handler = logging.StreamHandler(sys.stdout)
@@ -59,31 +55,34 @@
                     help="Number of principal components used to embed the transcriptomes prior to k-nearest-neighbor graph construction")
 parser.add_argument("--use_thr",
                     default=True,
                     help="use a user defined thr to define min doublet score to split true from false doublets? if false just use what the software produces")
 parser.add_argument("--call_doublets_thr",
                     default=0.25,
                     help="if use_thr is True, this thr will be used to define doublets")
+
 args, opt = parser.parse_known_args()
+L.info("Running with params: %s", args)
 
 # loading data
+input = args.inputpath + "/rna"
+L.info("Reading in data from '%s'" % input)
 adata = mu.read(args.inputpath + "/rna")
 
 
-    
+
 counts_matrix = adata.X
 L.info('Counts matrix shape: {} rows, {} columns'.format(counts_matrix.shape[0], counts_matrix.shape[1]))
 L.info('Number of genes in gene list: {}'.format(len(adata.var_names)))
 
-L.info("now initializing the scrublet object with expected_doublet_rate:\n")
-L.info(args.expected_doublet_rate)
+L.info("Initializing the scrublet object with expected_doublet_rate: %s" % args.expected_doublet_rate)
 
 scrub = scr.Scrublet(counts_matrix, expected_doublet_rate=float(args.expected_doublet_rate))
-L.info("predicting doublets with params: \nmincells: %s \nmingenes: %s \nmin_gene_variabilty_pctl: %s\nn_prin_comps: %s\n" % (args.min_counts, args.min_cells, args.min_gene_variability_pctl, args.n_prin_comps))
-L.info("predicting using:\n")
+L.info("Predicting doublets with params: \nmincells: %s \nmingenes: %s \nmin_gene_variabilty_pctl: %s\nn_prin_comps: %s\n" % (args.min_counts, args.min_cells, args.min_gene_variability_pctl, args.n_prin_comps))
+L.info("Predicting using:\n")
 
 doublet_scores, predicted_doublets = scrub.scrub_doublets(min_counts=int(args.min_counts),
                                                           min_cells=int(args.min_cells),
                                                           min_gene_variability_pctl=float(args.min_gene_variability_pctl),
                                                           n_prin_comps=int(args.n_prin_comps))
 
 # cgat pipelines will probably parse a string
@@ -91,38 +90,38 @@
     use_thr = True
 else:
     use_thr = False
 
 
 
 if use_thr:
-    L.info("using provided or default threshold  %s to call doublets, instead of predicted" % args.call_doublets_thr)
+    L.info("Using provided or default threshold %s to call doublets, instead of predicted" % args.call_doublets_thr)
     predicted_doublets = scrub.call_doublets(threshold=float(args.call_doublets_thr))
 else:
 
-    L.info("attempting to use predicted threshold for doublet prediction")
+    L.info("Attempting to use predicted threshold for doublet prediction")
     try:
         use_threshold=round(scrub.threshold_, 2)
-        L.info("using predicted threshold %s" % use_threshold)
+        L.info("Using predicted threshold %s" % use_threshold)
     except AttributeError:
         use_threshold=float(args.call_doublets_thr)
-        L.info("scrublet couldn't predict a threshold falling back on provided or default threshold %s" % use_threshold)
+        L.info("Scrublet couldn't predict a threshold falling back on provided or default threshold %s" % use_threshold)
 
     predicted_doublets = scrub.call_doublets(threshold=float(use_threshold))
-L.info("saving plots to outdir")
 
+L.info("Saving plots to directory '%s'" % args.outdir)
 fig = scrub.plot_histogram()
 fig[0].savefig(args.outdir + '/' + args.sample_id + '_' + "doubletScore_histogram.png",
                bbox_inches='tight', dpi=120)
 
-L.info("cellnames and doublet scores and prediction")
+L.info("Saving cell names, doublet scores, and prediction to txt file in directory '%s'" % args.outdir)
 
 data = pd.DataFrame({'doublet_scores': doublet_scores,
                      'predicted_doublets': predicted_doublets})
-
 data['barcode'] = adata.obs_names
 data.to_csv(os.path.join(args.outdir + "/" + args.sample_id + "_scrublet_scores.txt"),
             sep="\t", index=False)
-L.info('done')
+
+L.info('Done')
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/run_umap.py` & `panpipes-0.5.0/panpipes/python_scripts/run_umap.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,20 +29,21 @@
 parser.add_argument("--outfile", 
                     default="umap.txt.gz", 
                     help="file name, format: .h5ad")
 parser.add_argument("--min_dist", 
                     default=0.1, 
                     help="no. neighbours parameters for sc.pp.neighbors()")
 parser.add_argument("--neighbors_key", 
-                    default="neighbors", help="algortihm choice from louvain and leiden")
+                    default="neighbors", help="name of the saved knn neighbors")
 
 args, opt = parser.parse_known_args()
-L.info(args)
+L.info("Running with params: %s", args)
 
 # read data
+L.info("Reading in data from '%s'" % args.infile)
 mdata = mu.read(args.infile)
 if type(mdata) is AnnData:
     adata = mdata
 elif args.modality is not None:
     adata = mdata[args.modality]
 else:
     adata = mdata
@@ -51,34 +52,37 @@
 # set seed
 # seed = int(200612)
 
 uns_key=args.neighbors_key
 # check sc.pp.neihgbours has been run
 if uns_key not in adata.uns.keys():
     # sys.exit("Error: sc.pp.neighbours has not been run on this object")
-    L.warning("running neighbors with default parameters since no neighbors graph found in this data object")
+    L.warning("Running neighbors for modality %s with default parameters since no neighbors graph found in this data object" % args.modality)
     sc.pp.neighbors(adata)
     uns_key="neighbors"
 
 # code to run multiple umaps in one script, currently not used
 # manipulate min dist to list of floats
 # if type(args.min_dist) is str:
 #     min_dist = [float(md) for md in args.min_dist.split(',')]
 # elif type(args.min_dist) is float:
 #     min_dist = [args.min_dist]
 
 
 # what parameters?
+if args.modality is not None:
+    L.info("Running UMAP for modality %s on neighbors_key %s and mindist %s" % (args.modality,uns_key,args.min_dist))
 if uns_key =="wnn":
     mu.tl.umap(adata, min_dist=float(args.min_dist), neighbors_key=uns_key)
 else:
     sc.tl.umap(adata, min_dist=float(args.min_dist), neighbors_key=uns_key)
 
 # extract umap coordinates for plotting (in R??)
 umap_coords = pd.DataFrame(adata.obsm['X_umap'])
 
 # add in the rownames 
 umap_coords.index = adata.obs_names
 
 # save coordinates to file
 # (note this saves values values up to 6 significant figures, because why save 20 for a plot
+L.info("Saving UMAP coordinates to csv file '%s'" % args.outfile)
 umap_coords.to_csv(args.outfile, sep = '\t')
```

### Comparing `panpipes-0.4.1/panpipes/python_scripts/subtract_scrublet.py` & `panpipes-0.5.0/panpipes/python_scripts/subtract_scrublet.py`

 * *Files identical despite different names*

### Comparing `panpipes-0.4.1/panpipes/python_scripts/write_metadata.py` & `panpipes-0.5.0/panpipes/python_scripts/write_metadata.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,13 +16,16 @@
 parser = argparse.ArgumentParser()
 parser.add_argument('--infile',
                     default="./mdata.h5mu",
                     help="mudata object ")
 parser.add_argument('--outfile', default='sc_preprocess.txt',
                     help="path for text file output")
 args = parser.parse_args()
-
 args, opt = parser.parse_known_args()
+L.info("Running with params: %s", args)
 
 # read file
+L.info("Reading in MuData from '%s'" % args.infile)
 mdata = read(args.infile)
+
+L.info("Writing obs to '%s'" % args.outfile)
 mdata.obs.to_csv(args.outfile, sep='\t')
```

### Comparing `panpipes-0.4.1/panpipes/resources/cell_cycle_genes.tsv` & `panpipes-0.5.0/panpipes/resources/cell_cycle_genes.tsv`

 * *Files identical despite different names*

### Comparing `panpipes-0.4.1/panpipes/resources/metrics_summary_col_conversion.tsv` & `panpipes-0.5.0/panpipes/resources/metrics_summary_col_conversion.tsv`

 * *Files identical despite different names*

### Comparing `panpipes-0.4.1/panpipes/resources/qc_genelist_1.0.csv` & `panpipes-0.5.0/panpipes/resources/qc_genelist_1.0.csv`

 * *Files identical despite different names*

### Comparing `panpipes-0.4.1/panpipes/resources/sample_file_qc_spatial.txt` & `panpipes-0.5.0/panpipes/resources/sample_file_qc_spatial.txt`

 * *Files identical despite different names*

### Comparing `panpipes-0.4.1/panpipes.egg-info/SOURCES.txt` & `panpipes-0.5.0/panpipes.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -96,22 +96,26 @@
 panpipes/python_scripts/run_preprocess_rna.py
 panpipes/python_scripts/run_preprocess_spatial.py
 panpipes/python_scripts/run_scanpyQC_atac.py
 panpipes/python_scripts/run_scanpyQC_prot.py
 panpipes/python_scripts/run_scanpyQC_rep.py
 panpipes/python_scripts/run_scanpyQC_rna.py
 panpipes/python_scripts/run_scanpyQC_spatial.py
+panpipes/python_scripts/run_scib.py
 panpipes/python_scripts/run_scib_metrics.py
 panpipes/python_scripts/run_scrublet_scores.py
+panpipes/python_scripts/run_tangram.py
 panpipes/python_scripts/run_umap.py
 panpipes/python_scripts/subtract_scrublet.py
 panpipes/python_scripts/write_metadata.py
 panpipes/resources/__init__.py
 panpipes/resources/cell_cycle_genes.tsv
 panpipes/resources/metrics_summary_col_conversion.tsv
+panpipes/resources/mouse_cell_cycle_genes.tsv
+panpipes/resources/qc_gene_list_mouse.csv
 panpipes/resources/qc_genelist_1.0.csv
 panpipes/resources/sample_file_inc_demultiplexing.txt
 panpipes/resources/sample_file_qc_atac.txt
 panpipes/resources/sample_file_qc_mm.txt
 panpipes/resources/sample_file_qc_mm_gex_only.txt
 panpipes/resources/sample_file_qc_multiome.txt
 panpipes/resources/sample_file_qc_multiome_cellranger.txt
```

### Comparing `panpipes-0.4.1/tests/test_anndata.py` & `panpipes-0.5.0/tests/test_anndata.py`

 * *Files identical despite different names*

### Comparing `panpipes-0.4.1/tests/test_ingest_funcs.py` & `panpipes-0.5.0/tests/test_ingest_funcs.py`

 * *Files identical despite different names*

### Comparing `panpipes-0.4.1/tests/test_processing.py` & `panpipes-0.5.0/tests/test_processing.py`

 * *Files identical despite different names*

