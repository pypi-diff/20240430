# Comparing `tmp/fractal_tasks_core-1.0.0a3.tar.gz` & `tmp/fractal_tasks_core-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_tasks_core-1.0.0a3.tar", max compression
+gzip compressed data, was "fractal_tasks_core-1.0.1.tar", max compression
```

## Comparing `fractal_tasks_core-1.0.0a3.tar` & `fractal_tasks_core-1.0.1.tar`

### file list

```diff
@@ -1,59 +1,60 @@
--rw-r--r--   0        0        0     1584 2024-04-19 12:17:10.268485 fractal_tasks_core-1.0.0a3/LICENSE
--rw-r--r--   0        0        0     3743 2024-04-19 12:17:10.268485 fractal_tasks_core-1.0.0a3/README.md
--rw-r--r--   0        0        0       32 2024-04-19 12:17:10.272485 fractal_tasks_core-1.0.0a3/fractal_tasks_core/.gitignore
--rw-r--r--   0        0        0    64035 2024-04-19 12:17:10.272485 fractal_tasks_core-1.0.0a3/fractal_tasks_core/__FRACTAL_MANIFEST__.json
--rw-r--r--   0        0        0      200 2024-04-19 12:17:10.272485 fractal_tasks_core-1.0.0a3/fractal_tasks_core/__init__.py
--rw-r--r--   0        0        0       87 2024-04-19 12:17:10.272485 fractal_tasks_core-1.0.0a3/fractal_tasks_core/cellvoyager/__init__.py
--rw-r--r--   0        0        0     4552 2024-04-19 12:17:10.272485 fractal_tasks_core-1.0.0a3/fractal_tasks_core/cellvoyager/filenames.py
--rw-r--r--   0        0        0    12515 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/cellvoyager/metadata.py
--rw-r--r--   0        0        0    16707 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/channels.py
--rw-r--r--   0        0        0      108 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/README.md
--rw-r--r--   0        0        0       98 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/__init__.py
--rw-r--r--   0        0        0     4607 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/check_manifest.py
--rw-r--r--   0        0        0     5368 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/create_manifest.py
--rw-r--r--   0        0        0     8166 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/lib_args_schemas.py
--rw-r--r--   0        0        0     6406 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/lib_descriptions.py
--rw-r--r--   0        0        0     3260 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/lib_signature_constraints.py
--rw-r--r--   0        0        0     2827 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/lib_task_docs.py
--rw-r--r--   0        0        0     2273 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/lib_titles.py
--rw-r--r--   0        0        0     3624 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/task_list.py
--rw-r--r--   0        0        0     2660 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/task_models.py
--rw-r--r--   0        0        0     5189 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/labels.py
--rw-r--r--   0        0        0     9005 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/masked_loading.py
--rw-r--r--   0        0        0      508 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/ngff/__init__.py
--rw-r--r--   0        0        0    13113 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/ngff/specs.py
--rw-r--r--   0        0        0     3974 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/ngff/zarr_utils.py
--rw-r--r--   0        0        0     3788 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/pyramids.py
--rw-r--r--   0        0        0      185 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/roi/__init__.py
--rw-r--r--   0        0        0     4501 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/roi/_overlaps_common.py
--rw-r--r--   0        0        0     1327 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/roi/load_region.py
--rw-r--r--   0        0        0    18609 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/roi/v1.py
--rw-r--r--   0        0        0     4910 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/roi/v1_checks.py
--rw-r--r--   0        0        0    13273 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/roi/v1_overlaps.py
--rw-r--r--   0        0        0     3394 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tables/__init__.py
--rw-r--r--   0        0        0    11579 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tables/v1.py
--rw-r--r--   0        0        0       72 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/__init__.py
--rw-r--r--   0        0        0     8166 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/_registration_utils.py
--rw-r--r--   0        0        0     2407 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/_utils.py
--rw-r--r--   0        0        0     3839 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/_zarr_utils.py
--rw-r--r--   0        0        0    13819 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/apply_registration_to_image.py
--rw-r--r--   0        0        0     9363 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/calculate_registration_image_based.py
--rw-r--r--   0        0        0    27516 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/cellpose_segmentation.py
--rw-r--r--   0        0        0     8458 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/cellpose_transforms.py
--rw-r--r--   0        0        0     7779 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_compute.py
--rw-r--r--   0        0        0    18431 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init.py
--rw-r--r--   0        0        0    21103 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init_multiplex.py
--rw-r--r--   0        0        0    11258 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/copy_ome_zarr_hcs_plate.py
--rw-r--r--   0        0        0     6403 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/find_registration_consensus.py
--rw-r--r--   0        0        0    10480 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/illumination_correction.py
--rw-r--r--   0        0        0     3596 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/image_based_registration_hcs_init.py
--rw-r--r--   0        0        0    11764 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/import_ome_zarr.py
--rw-r--r--   0        0        0     2998 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/init_group_by_well_for_multiplexing.py
--rw-r--r--   0        0        0     4903 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/io_models.py
--rw-r--r--   0        0        0     6239 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/maximum_intensity_projection.py
--rw-r--r--   0        0        0    24816 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/napari_workflows_wrapper.py
--rw-r--r--   0        0        0     7136 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/upscale_array.py
--rw-r--r--   0        0        0     6101 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/utils.py
--rw-r--r--   0        0        0     3890 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/zarr_utils.py
--rw-r--r--   0        0        0     3387 2024-04-19 12:17:10.280485 fractal_tasks_core-1.0.0a3/pyproject.toml
--rw-r--r--   0        0        0     5764 1970-01-01 00:00:00.000000 fractal_tasks_core-1.0.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1584 2024-04-30 10:58:01.120479 fractal_tasks_core-1.0.1/LICENSE
+-rw-r--r--   0        0        0     6042 2024-04-30 10:58:01.120479 fractal_tasks_core-1.0.1/README.md
+-rw-r--r--   0        0        0       32 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/.gitignore
+-rw-r--r--   0        0        0    64149 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/__FRACTAL_MANIFEST__.json
+-rw-r--r--   0        0        0      198 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/__init__.py
+-rw-r--r--   0        0        0       87 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/cellvoyager/__init__.py
+-rw-r--r--   0        0        0     4552 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/cellvoyager/filenames.py
+-rw-r--r--   0        0        0    15388 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/cellvoyager/metadata.py
+-rw-r--r--   0        0        0     3289 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/cellvoyager/wells.py
+-rw-r--r--   0        0        0    16713 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/channels.py
+-rw-r--r--   0        0        0      108 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/dev/README.md
+-rw-r--r--   0        0        0       98 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/dev/__init__.py
+-rw-r--r--   0        0        0     4607 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/dev/check_manifest.py
+-rw-r--r--   0        0        0     5368 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/dev/create_manifest.py
+-rw-r--r--   0        0        0     8166 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/dev/lib_args_schemas.py
+-rw-r--r--   0        0        0     6406 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/dev/lib_descriptions.py
+-rw-r--r--   0        0        0     3260 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/dev/lib_signature_constraints.py
+-rw-r--r--   0        0        0     2827 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/dev/lib_task_docs.py
+-rw-r--r--   0        0        0     2273 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/dev/lib_titles.py
+-rw-r--r--   0        0        0     3624 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/dev/task_list.py
+-rw-r--r--   0        0        0     2660 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/dev/task_models.py
+-rw-r--r--   0        0        0     5189 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/labels.py
+-rw-r--r--   0        0        0     9005 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/masked_loading.py
+-rw-r--r--   0        0        0      508 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/ngff/__init__.py
+-rw-r--r--   0        0        0    12849 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/ngff/specs.py
+-rw-r--r--   0        0        0     3974 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/ngff/zarr_utils.py
+-rw-r--r--   0        0        0     3788 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/pyramids.py
+-rw-r--r--   0        0        0      185 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/roi/__init__.py
+-rw-r--r--   0        0        0     4501 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/roi/_overlaps_common.py
+-rw-r--r--   0        0        0     1327 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/roi/load_region.py
+-rw-r--r--   0        0        0    18609 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/roi/v1.py
+-rw-r--r--   0        0        0     4910 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/roi/v1_checks.py
+-rw-r--r--   0        0        0    13273 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/roi/v1_overlaps.py
+-rw-r--r--   0        0        0     3394 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tables/__init__.py
+-rw-r--r--   0        0        0    11579 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tables/v1.py
+-rw-r--r--   0        0        0       72 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/__init__.py
+-rw-r--r--   0        0        0     8178 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/_registration_utils.py
+-rw-r--r--   0        0        0     2407 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/_utils.py
+-rw-r--r--   0        0        0     7545 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/_zarr_utils.py
+-rw-r--r--   0        0        0    14906 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/apply_registration_to_image.py
+-rw-r--r--   0        0        0     9394 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/calculate_registration_image_based.py
+-rw-r--r--   0        0        0    27516 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/cellpose_segmentation.py
+-rw-r--r--   0        0        0     8458 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/cellpose_transforms.py
+-rw-r--r--   0        0        0     7384 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_compute.py
+-rw-r--r--   0        0        0    18564 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init.py
+-rw-r--r--   0        0        0    21248 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init_multiplex.py
+-rw-r--r--   0        0        0    11258 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/copy_ome_zarr_hcs_plate.py
+-rw-r--r--   0        0        0     6421 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/find_registration_consensus.py
+-rw-r--r--   0        0        0    10735 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/illumination_correction.py
+-rw-r--r--   0        0        0     3686 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/image_based_registration_hcs_init.py
+-rw-r--r--   0        0        0    11752 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/import_ome_zarr.py
+-rw-r--r--   0        0        0     3066 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/init_group_by_well_for_multiplexing.py
+-rw-r--r--   0        0        0     4903 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/io_models.py
+-rw-r--r--   0        0        0     6239 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/maximum_intensity_projection.py
+-rw-r--r--   0        0        0    24816 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/napari_workflows_wrapper.py
+-rw-r--r--   0        0        0     7136 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/upscale_array.py
+-rw-r--r--   0        0        0     6101 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/utils.py
+-rw-r--r--   0        0        0     3890 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/zarr_utils.py
+-rw-r--r--   0        0        0     3403 2024-04-30 10:58:01.132479 fractal_tasks_core-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     8096 1970-01-01 00:00:00.000000 fractal_tasks_core-1.0.1/PKG-INFO
```

### Comparing `fractal_tasks_core-1.0.0a3/LICENSE` & `fractal_tasks_core-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/__FRACTAL_MANIFEST__.json` & `fractal_tasks_core-1.0.1/fractal_tasks_core/__FRACTAL_MANIFEST__.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9962992862654321%*

 * *Differences: {"'task_list'": "{0: {'args_schema_parallel': {'properties': {delete: ['overwrite']}}, "*

 * *                "'docs_info': '## cellvoyager_to_ome_zarr_init\\nCreate a OME-NGFF zarr folder, "*

 * *                'without reading/writing image data.\\n\\nFind plates (for each folder in '*

 * *                'input_paths):\\n\\n- glob image files,\\n- parse metadata from image filename to '*

 * *                'identify plates,\\n- identify populated channels.\\n\\nCreate a zarr folder (for '*

 * *                'each plate):\\n\ […]*

```diff
@@ -215,34 +215,28 @@
                 },
                 "properties": {
                     "init_args": {
                         "$ref": "#/definitions/InitArgsCellVoyager",
                         "description": "Intialization arguments provided by `create_cellvoyager_ome_zarr_init`.",
                         "title": "Init_Args"
                     },
-                    "overwrite": {
-                        "default": false,
-                        "description": "If `True`, overwrite the task output.",
-                        "title": "Overwrite",
-                        "type": "boolean"
-                    },
                     "zarr_url": {
                         "description": "Path or url to the individual OME-Zarr image to be processed. (standard argument for Fractal tasks, managed by Fractal server).",
                         "title": "Zarr Url",
                         "type": "string"
                     }
                 },
                 "required": [
                     "zarr_url",
                     "init_args"
                 ],
                 "title": "CellvoyagerToOmeZarrCompute",
                 "type": "object"
             },
-            "docs_info": "## cellvoyager_to_ome_zarr_init\nCreate a OME-NGFF zarr folder, without reading/writing image data.\n\nFind plates (for each folder in input_paths):\n\n- glob image files,\n- parse metadata from image filename to identify plates,\n- identify populated channels.\n\nCreate a zarr folder (for each plate):\n\n- parse mlf metadata,\n- identify wells and field of view (FOV),\n- create FOV ZARR,\n- verify that channels are uniform (i.e., same channels).\n## cellvoyager_to_ome_zarr_compute\nConvert Yokogawa output (png, tif) to zarr file.\n\nThis task is typically run after Create OME-Zarr or\nCreate OME-Zarr Multiplexing and populates the empty OME-Zarr files that\nwere prepared.\n",
+            "docs_info": "## cellvoyager_to_ome_zarr_init\nCreate a OME-NGFF zarr folder, without reading/writing image data.\n\nFind plates (for each folder in input_paths):\n\n- glob image files,\n- parse metadata from image filename to identify plates,\n- identify populated channels.\n\nCreate a zarr folder (for each plate):\n\n- parse mlf metadata,\n- identify wells and field of view (FOV),\n- create FOV ZARR,\n- verify that channels are uniform (i.e., same channels).\n## cellvoyager_to_ome_zarr_compute\nConvert Yokogawa output (png, tif) to zarr file.\n\nThis task is run after an init task (typically\n`cellvoyager_to_ome_zarr_init` or\n`cellvoyager_to_ome_zarr_init_multiplex`), and it populates the empty\nOME-Zarr files that were prepared.\n\nNote that the current task always overwrites existing data. To avoid this\nbehavior, set the `overwrite` argument of the init task to `False`.\n",
             "docs_link": "https://fractal-analytics-platform.github.io/fractal-tasks-core",
             "executable_non_parallel": "tasks/cellvoyager_to_ome_zarr_init.py",
             "executable_parallel": "tasks/cellvoyager_to_ome_zarr_compute.py",
             "meta_non_parallel": {
                 "cpus_per_task": 1,
                 "mem": 4000
             },
@@ -482,34 +476,28 @@
                 },
                 "properties": {
                     "init_args": {
                         "$ref": "#/definitions/InitArgsCellVoyager",
                         "description": "Intialization arguments provided by `create_cellvoyager_ome_zarr_init`.",
                         "title": "Init_Args"
                     },
-                    "overwrite": {
-                        "default": false,
-                        "description": "If `True`, overwrite the task output.",
-                        "title": "Overwrite",
-                        "type": "boolean"
-                    },
                     "zarr_url": {
                         "description": "Path or url to the individual OME-Zarr image to be processed. (standard argument for Fractal tasks, managed by Fractal server).",
                         "title": "Zarr Url",
                         "type": "string"
                     }
                 },
                 "required": [
                     "zarr_url",
                     "init_args"
                 ],
                 "title": "CellvoyagerToOmeZarrCompute",
                 "type": "object"
             },
-            "docs_info": "## cellvoyager_to_ome_zarr_init_multiplex\nCreate OME-NGFF structure and metadata to host a multiplexing dataset.\n\nThis task takes a set of image folders (i.e. different acquisition cycles)\nand build the internal structure and metadata of a OME-NGFF zarr group,\nwithout actually loading/writing the image data.\n\nEach element in input_paths should be treated as a different acquisition.\n## cellvoyager_to_ome_zarr_compute\nConvert Yokogawa output (png, tif) to zarr file.\n\nThis task is typically run after Create OME-Zarr or\nCreate OME-Zarr Multiplexing and populates the empty OME-Zarr files that\nwere prepared.\n",
+            "docs_info": "## cellvoyager_to_ome_zarr_init_multiplex\nCreate OME-NGFF structure and metadata to host a multiplexing dataset.\n\nThis task takes a set of image folders (i.e. different multiplexing\nacquisitions) and build the internal structure and metadata of a OME-NGFF\nzarr group, without actually loading/writing the image data.\n\nEach element in input_paths should be treated as a different acquisition.\n## cellvoyager_to_ome_zarr_compute\nConvert Yokogawa output (png, tif) to zarr file.\n\nThis task is run after an init task (typically\n`cellvoyager_to_ome_zarr_init` or\n`cellvoyager_to_ome_zarr_init_multiplex`), and it populates the empty\nOME-Zarr files that were prepared.\n\nNote that the current task always overwrites existing data. To avoid this\nbehavior, set the `overwrite` argument of the init task to `False`.\n",
             "docs_link": "https://fractal-analytics-platform.github.io/fractal-tasks-core",
             "executable_non_parallel": "tasks/cellvoyager_to_ome_zarr_init_multiplex.py",
             "executable_parallel": "tasks/cellvoyager_to_ome_zarr_compute.py",
             "meta_non_parallel": {
                 "cpus_per_task": 1,
                 "mem": 4000
             },
@@ -960,18 +948,18 @@
             },
             "name": "Cellpose Segmentation"
         },
         {
             "args_schema_non_parallel": {
                 "additionalProperties": false,
                 "properties": {
-                    "reference_cycle": {
+                    "reference_acquisition": {
                         "default": 0,
-                        "description": "Which cycle to register against. Needs to match the acquisition metadata in the OME-Zarr image.",
-                        "title": "Reference Cycle",
+                        "description": "Which acquisition to register against. Needs to match the acquisition metadata in the OME-Zarr image.",
+                        "title": "Reference Acquisition",
                         "type": "integer"
                     },
                     "zarr_dir": {
                         "description": "path of the directory where the new OME-Zarrs will be created. Not used by this task. (standard argument for Fractal tasks, managed by Fractal server).",
                         "title": "Zarr Dir",
                         "type": "string"
                     },
@@ -1042,15 +1030,15 @@
                     "zarr_url",
                     "init_args",
                     "wavelength_id"
                 ],
                 "title": "CalculateRegistrationImageBased",
                 "type": "object"
             },
-            "docs_info": "## image_based_registration_hcs_init\nInitialized calculate registration task\n\nThis task prepares a parallelization list of all zarr_urls that need to be\nused to calculate the registration between cycles (all zarr_urls except\nthe reference cycle vs. the reference cycle).\nThis task only works for HCS OME-Zarrs for 2 reasons: Only HCS OME-Zarrs\ncurrently have defined acquisition metadata to determine reference cycles.\nAnd we have only implemented the grouping of images for HCS OME-Zarrs by\nwell (with the assumption that every well just has 1 image per acqusition).\n## calculate_registration_image_based\nCalculate registration based on images\n\nThis task consists of 3 parts:\n\n1. Loading the images of a given ROI (=> loop over ROIs)\n2. Calculating the transformation for that ROI\n3. Storing the calculated transformation in the ROI table\n",
+            "docs_info": "## image_based_registration_hcs_init\nInitialized calculate registration task\n\nThis task prepares a parallelization list of all zarr_urls that need to be\nused to calculate the registration between acquisitions (all zarr_urls\nexcept the reference acquisition vs. the reference acquisition).\nThis task only works for HCS OME-Zarrs for 2 reasons: Only HCS OME-Zarrs\ncurrently have defined acquisition metadata to determine reference\nacquisitions. And we have only implemented the grouping of images for\nHCS OME-Zarrs by well (with the assumption that every well just has 1\nimage per acqusition).\n## calculate_registration_image_based\nCalculate registration based on images\n\nThis task consists of 3 parts:\n\n1. Loading the images of a given ROI (=> loop over ROIs)\n2. Calculating the transformation for that ROI\n3. Storing the calculated transformation in the ROI table\n",
             "docs_link": "https://fractal-analytics-platform.github.io/fractal-tasks-core",
             "executable_non_parallel": "tasks/image_based_registration_hcs_init.py",
             "executable_parallel": "tasks/calculate_registration_image_based.py",
             "meta_non_parallel": {
                 "cpus_per_task": 1,
                 "mem": 1000
             },
@@ -1060,18 +1048,18 @@
             },
             "name": "Calculate Registration (image-based)"
         },
         {
             "args_schema_non_parallel": {
                 "additionalProperties": false,
                 "properties": {
-                    "reference_cycle": {
+                    "reference_acquisition": {
                         "default": 0,
-                        "description": "Which cycle to register against. Uses the OME-NGFF HCS well metadata acquisition keys to find the reference cycle.",
-                        "title": "Reference Cycle",
+                        "description": "Which acquisition to register against. Uses the OME-NGFF HCS well metadata acquisition keys to find the reference acquisition.",
+                        "title": "Reference Acquisition",
                         "type": "integer"
                     },
                     "zarr_dir": {
                         "description": "path of the directory where the new OME-Zarrs will be created. Not used by this task. (standard argument for Fractal tasks, managed by Fractal server).",
                         "title": "Zarr Dir",
                         "type": "string"
                     },
@@ -1111,42 +1099,42 @@
                         "title": "InitArgsRegistrationConsensus",
                         "type": "object"
                     }
                 },
                 "properties": {
                     "init_args": {
                         "$ref": "#/definitions/InitArgsRegistrationConsensus",
-                        "description": "Intialization arguments provided by `init_group_by_well_for_multiplexing`. It contains the zarr_url_list listing all the zarr_urls in the same well as the zarr_url of the reference cycle that are being processed. (standard argument for Fractal tasks, managed by Fractal server).",
+                        "description": "Intialization arguments provided by `init_group_by_well_for_multiplexing`. It contains the zarr_url_list listing all the zarr_urls in the same well as the zarr_url of the reference acquisition that are being processed. (standard argument for Fractal tasks, managed by Fractal server).",
                         "title": "Init_Args"
                     },
                     "new_roi_table": {
                         "description": "Optional name for the new, registered ROI table. If no name is given, it will default to \"registered_\" + `roi_table`",
                         "title": "New Roi Table",
                         "type": "string"
                     },
                     "roi_table": {
                         "default": "FOV_ROI_table",
                         "description": "Name of the ROI table over which the task loops to calculate the registration. Examples: `FOV_ROI_table` => loop over the field of views, `well_ROI_table` => process the whole well as one image.",
                         "title": "Roi Table",
                         "type": "string"
                     },
                     "zarr_url": {
-                        "description": "Path or url to the individual OME-Zarr image to be processed. Refers to the zarr_url of the reference cycle. (standard argument for Fractal tasks, managed by Fractal server).",
+                        "description": "Path or url to the individual OME-Zarr image to be processed. Refers to the zarr_url of the reference acquisition. (standard argument for Fractal tasks, managed by Fractal server).",
                         "title": "Zarr Url",
                         "type": "string"
                     }
                 },
                 "required": [
                     "zarr_url",
                     "init_args"
                 ],
                 "title": "FindRegistrationConsensus",
                 "type": "object"
             },
-            "docs_info": "## init_group_by_well_for_multiplexing\nFinds images for all acquisitions per well.\n\nReturns the parallelization_list to run `find_registration_consensus`.\n## find_registration_consensus\nApplies pre-calculated registration to ROI tables.\n\nApply pre-calculated registration such that resulting ROIs contain\nthe consensus align region between all cycles.\n\nParallelization level: well\n",
+            "docs_info": "## init_group_by_well_for_multiplexing\nFinds images for all acquisitions per well.\n\nReturns the parallelization_list to run `find_registration_consensus`.\n## find_registration_consensus\nApplies pre-calculated registration to ROI tables.\n\nApply pre-calculated registration such that resulting ROIs contain\nthe consensus align region between all acquisitions.\n\nParallelization level: well\n",
             "docs_link": "https://fractal-analytics-platform.github.io/fractal-tasks-core",
             "executable_non_parallel": "tasks/init_group_by_well_for_multiplexing.py",
             "executable_parallel": "tasks/find_registration_consensus.py",
             "meta_non_parallel": {
                 "cpus_per_task": 1,
                 "mem": 1000
             },
@@ -1162,18 +1150,18 @@
                 "properties": {
                     "overwrite_input": {
                         "default": true,
                         "description": "Whether the old image data should be replaced with the newly registered image data. Currently only implemented for `overwrite_input=True`.",
                         "title": "Overwrite Input",
                         "type": "boolean"
                     },
-                    "reference_cycle": {
+                    "reference_acquisition": {
                         "default": 0,
-                        "description": "Which cycle to register against. Uses the OME-NGFF HCS well metadata acquisition keys to find the reference cycle.",
-                        "title": "Reference Cycle",
+                        "description": "Which acquisition to register against. Uses the OME-NGFF HCS well metadata acquisition keys to find the reference acquisition.",
+                        "title": "Reference Acquisition",
                         "type": "integer"
                     },
                     "registered_roi_table": {
                         "description": "Name of the ROI table which has been registered and will be applied to mask and shift the images. Examples: `registered_FOV_ROI_table` => loop over the field of views, `registered_well_ROI_table` => process the whole well as one image.",
                         "title": "Registered Roi Table",
                         "type": "string"
                     },
@@ -1186,15 +1174,15 @@
                 "required": [
                     "zarr_url",
                     "registered_roi_table"
                 ],
                 "title": "ApplyRegistrationToImage",
                 "type": "object"
             },
-            "docs_info": "## apply_registration_to_image\nApply registration to images by using a registered ROI table\n\nThis task consists of 4 parts:\n\n1. Mask all regions in images that are not available in the\nregistered ROI table and store each cycle aligned to the\nreference_cycle (by looping over ROIs).\n2. Do the same for all label images.\n3. Copy all tables from the non-aligned image to the aligned image\n(currently only works well if the only tables are well & FOV ROI tables\n(registered and original). Not implemented for measurement tables and\nother ROI tables).\n4. Clean up: Delete the old, non-aligned image and rename the new,\naligned image to take over its place.\n",
+            "docs_info": "## apply_registration_to_image\nApply registration to images by using a registered ROI table\n\nThis task consists of 4 parts:\n\n1. Mask all regions in images that are not available in the\nregistered ROI table and store each acquisition aligned to the\nreference_acquisition (by looping over ROIs).\n2. Do the same for all label images.\n3. Copy all tables from the non-aligned image to the aligned image\n(currently only works well if the only tables are well & FOV ROI tables\n(registered and original). Not implemented for measurement tables and\nother ROI tables).\n4. Clean up: Delete the old, non-aligned image and rename the new,\naligned image to take over its place.\n",
             "docs_link": "https://fractal-analytics-platform.github.io/fractal-tasks-core",
             "executable_parallel": "tasks/apply_registration_to_image.py",
             "input_types": {
                 "registered": false
             },
             "meta_parallel": {
                 "cpus_per_task": 1,
```

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/cellvoyager/filenames.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/cellvoyager/filenames.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/channels.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/channels.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
     First identify the channel-labels list for each image in the well, then
     compare lists and verify their intersection is empty.
 
     Args:
         well_zarr_path: path to an OME-NGFF well zarr group.
     """
 
-    # Iterate over all images (multiplexing cycles, multi-FOVs, ...)
+    # Iterate over all images (multiplexing acquisitions, multi-FOVs, ...)
     group = zarr.open_group(well_zarr_path, mode="r+")
     image_paths = [image["path"] for image in group.attrs["well"]["images"]]
     list_of_channel_lists = []
     for image_path in image_paths:
         channels = get_omero_channel_list(
             image_zarr_path=f"{well_zarr_path}/{image_path}"
         )
```

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/check_manifest.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/dev/check_manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/create_manifest.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/dev/create_manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/lib_args_schemas.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/dev/lib_args_schemas.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/lib_descriptions.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/dev/lib_descriptions.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/lib_signature_constraints.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/dev/lib_signature_constraints.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/lib_task_docs.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/dev/lib_task_docs.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/lib_titles.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/dev/lib_titles.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/task_list.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/dev/task_list.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/task_models.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/dev/task_models.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/labels.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/labels.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/masked_loading.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/masked_loading.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/ngff/specs.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/ngff/specs.py`

 * *Files 4% similar despite different names*

```diff
@@ -340,45 +340,40 @@
     Model for the metadata of a NGFF well.
 
     See https://ngff.openmicroscopy.org/0.4/#well-md.
     """
 
     well: Optional[Well] = None
 
-    def get_acquisition_paths(self) -> dict[int, str]:
+    def get_acquisition_paths(self) -> dict[int, list[str]]:
         """
         Create mapping from acquisition indices to corresponding paths.
 
         Runs on the well zarr attributes and loads the relative paths in the
         well.
 
         Returns:
-            Dictionary with `(acquisition index: image path)` key/value pairs.
+            Dictionary with `(acquisition index: [image_path])` key/value
+            pairs.
 
         Raises:
             ValueError:
                 If an element of `self.well.images` has no `acquisition`
                     attribute.
-            NotImplementedError:
-                If acquisitions are not unique.
         """
         acquisition_dict = {}
         for image in self.well.images:
             if image.acquisition is None:
                 raise ValueError(
                     "Cannot get acquisition paths for Zarr files without "
                     "'acquisition' metadata at the well level"
                 )
-            if image.acquisition in acquisition_dict:
-                raise NotImplementedError(
-                    "The `NgffWellMeta.get_acquisition_paths` method (in "
-                    "fractal-tasks-core) does not support wells with "
-                    "multiple images of the same acquisition."
-                )
-            acquisition_dict[image.acquisition] = image.path
+            if image.acquisition not in acquisition_dict:
+                acquisition_dict[image.acquisition] = []
+            acquisition_dict[image.acquisition].append(image.path)
         return acquisition_dict
 
 
 ######################
 # Plate models
 ######################
```

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/ngff/zarr_utils.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/ngff/zarr_utils.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/pyramids.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/pyramids.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/roi/_overlaps_common.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/roi/_overlaps_common.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/roi/load_region.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/roi/load_region.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/roi/v1.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/roi/v1.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/roi/v1_checks.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/roi/v1_checks.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/roi/v1_overlaps.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/roi/v1_overlaps.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tables/__init__.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tables/v1.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/tables/v1.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/_registration_utils.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/_registration_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     """
     Add three zero-filled columns (`translation_{x,y,z}`) to an AnnData table.
     """
     columns = ["translation_z", "translation_y", "translation_x"]
     if ad_table.var.index.isin(columns).any().any():
         raise ValueError(
             "The roi table already contains translation columns. Did you "
-            "enter a wrong reference cycle?"
+            "enter a wrong reference acquisition?"
         )
     df = pd.DataFrame(np.zeros([len(ad_table), 3]), columns=columns)
     df.index = ad_table.obs.index
     ad_new = ad.concat([ad_table, ad.AnnData(df)], axis=1)
     return ad_new
 
 
@@ -188,15 +188,15 @@
             Rows are ROIs
         max_df: Max translation shift in z, y, x for each ROI. Rows are ROIs,
             columns are translation_z, translation_y, translation_x
         min_df: Min translation shift in z, y, x for each ROI. Rows are ROIs,
             columns are translation_z, translation_y, translation_x
     Returns:
         ROI table where all ROIs are registered to the smallest common area
-        across all cycles.
+        across all acquisitions.
     """
     roi_table = copy.deepcopy(roi_table)
     rois = roi_table.obs.index
     if (rois != max_df.index).all() or (rois != min_df.index).all():
         raise ValueError(
             "ROI table and max & min translation need to contain the same "
             f"ROIS, but they were {rois=}, {max_df.index=}, {min_df.index=}"
```

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/_utils.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/_utils.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/apply_registration_to_image.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/apply_registration_to_image.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,39 +32,43 @@
 from fractal_tasks_core.roi import (
     convert_ROI_table_to_indices,
 )
 from fractal_tasks_core.roi import is_standard_roi_table
 from fractal_tasks_core.roi import load_region
 from fractal_tasks_core.tables import write_table
 from fractal_tasks_core.tasks._zarr_utils import (
+    _get_matching_ref_acquisition_path_heuristic,
+)
+from fractal_tasks_core.tasks._zarr_utils import (
     _split_well_path_image_path,
 )
+from fractal_tasks_core.tasks._zarr_utils import _update_well_metadata
 from fractal_tasks_core.utils import _get_table_path_dict
 
 logger = logging.getLogger(__name__)
 
 
 @validate_arguments
 def apply_registration_to_image(
     *,
     # Fractal parameters
     zarr_url: str,
     # Core parameters
     registered_roi_table: str,
-    reference_cycle: int = 0,
+    reference_acquisition: int = 0,
     overwrite_input: bool = True,
 ):
     """
     Apply registration to images by using a registered ROI table
 
     This task consists of 4 parts:
 
     1. Mask all regions in images that are not available in the
-    registered ROI table and store each cycle aligned to the
-    reference_cycle (by looping over ROIs).
+    registered ROI table and store each acquisition aligned to the
+    reference_acquisition (by looping over ROIs).
     2. Do the same for all label images.
     3. Copy all tables from the non-aligned image to the aligned image
     (currently only works well if the only tables are well & FOV ROI tables
     (registered and original). Not implemented for measurement tables and
     other ROI tables).
     4. Clean up: Delete the old, non-aligned image and rename the new,
     aligned image to take over its place.
@@ -73,56 +77,68 @@
         zarr_url: Path or url to the individual OME-Zarr image to be processed.
             (standard argument for Fractal tasks, managed by Fractal server).
         registered_roi_table: Name of the ROI table which has been registered
             and will be applied to mask and shift the images.
             Examples: `registered_FOV_ROI_table` => loop over the field of
             views, `registered_well_ROI_table` => process the whole well as
             one image.
-        reference_cycle: Which cycle to register against. Uses the OME-NGFF
-            HCS well metadata acquisition keys to find the reference cycle.
+        reference_acquisition: Which acquisition to register against. Uses the
+            OME-NGFF HCS well metadata acquisition keys to find the reference
+            acquisition.
         overwrite_input: Whether the old image data should be replaced with the
             newly registered image data. Currently only implemented for
             `overwrite_input=True`.
 
     """
     logger.info(zarr_url)
     logger.info(
         f"Running `apply_registration_to_image` on {zarr_url=}, "
-        f"{registered_roi_table=} and {reference_cycle=}. "
+        f"{registered_roi_table=} and {reference_acquisition=}. "
         f"Using {overwrite_input=}"
     )
 
-    well_url, _ = _split_well_path_image_path(zarr_url)
+    well_url, old_img_path = _split_well_path_image_path(zarr_url)
     new_zarr_url = f"{well_url}/{zarr_url.split('/')[-1]}_registered"
-    # Get the zarr_url for the reference cycle
+    # Get the zarr_url for the reference acquisition
     acq_dict = load_NgffWellMeta(well_url).get_acquisition_paths()
-    if reference_cycle not in acq_dict:
+    if reference_acquisition not in acq_dict:
         raise ValueError(
-            f"{reference_cycle=} was not one of the available acquisitions in "
-            f"{acq_dict=} for well {well_url}"
+            f"{reference_acquisition=} was not one of the available "
+            f"acquisitions in {acq_dict=} for well {well_url}"
+        )
+    elif len(acq_dict[reference_acquisition]) > 1:
+        ref_path = _get_matching_ref_acquisition_path_heuristic(
+            acq_dict[reference_acquisition], old_img_path
         )
-    reference_zarr_url = f"{well_url}/{acq_dict[reference_cycle]}"
+        logger.warning(
+            "Running registration when there are multiple images of the same "
+            "acquisition in a well. Using a heuristic to match the reference "
+            f"acquisition. Using {ref_path} as the reference image."
+        )
+    else:
+        ref_path = acq_dict[reference_acquisition][0]
+    reference_zarr_url = f"{well_url}/{ref_path}"
 
     ROI_table_ref = ad.read_zarr(
         f"{reference_zarr_url}/tables/{registered_roi_table}"
     )
-    ROI_table_cycle = ad.read_zarr(f"{zarr_url}/tables/{registered_roi_table}")
+    ROI_table_acq = ad.read_zarr(f"{zarr_url}/tables/{registered_roi_table}")
 
     ngff_image_meta = load_NgffImageMeta(zarr_url)
     coarsening_xy = ngff_image_meta.coarsening_xy
     num_levels = ngff_image_meta.num_levels
 
     ####################
     # Process images
     ####################
     logger.info("Write the registered Zarr image to disk")
     write_registered_zarr(
         zarr_url=zarr_url,
         new_zarr_url=new_zarr_url,
-        ROI_table=ROI_table_cycle,
+        ROI_table=ROI_table_acq,
         ROI_table_ref=ROI_table_ref,
         num_levels=num_levels,
         coarsening_xy=coarsening_xy,
         aggregation_function=np.mean,
     )
 
     ####################
@@ -139,25 +155,26 @@
         labels_group = zarr.group(f"{new_zarr_url}/labels")
         labels_group.attrs["labels"] = label_list
 
         for label in label_list:
             write_registered_zarr(
                 zarr_url=f"{zarr_url}/labels/{label}",
                 new_zarr_url=f"{new_zarr_url}/labels/{label}",
-                ROI_table=ROI_table_cycle,
+                ROI_table=ROI_table_acq,
                 ROI_table_ref=ROI_table_ref,
                 num_levels=num_levels,
                 coarsening_xy=coarsening_xy,
                 aggregation_function=np.max,
             )
 
     ####################
     # Copy tables
-    # 1. Copy all standard ROI tables from cycle 0.
-    # 2. Copy all tables that aren't standard ROI tables from the given cycle
+    # 1. Copy all standard ROI tables from the reference acquisition.
+    # 2. Copy all tables that aren't standard ROI tables from the given
+    # acquisition.
     ####################
     table_dict_reference = _get_table_path_dict(reference_zarr_url)
     table_dict_component = _get_table_path_dict(zarr_url)
 
     table_dict = {}
     # Define which table should get copied:
     for table in table_dict_reference:
@@ -166,20 +183,20 @@
     for table in table_dict_component:
         if not is_standard_roi_table(table):
             if reference_zarr_url != zarr_url:
                 logger.warning(
                     f"{zarr_url} contained a table that is not a standard "
                     "ROI table. The `Apply Registration To Image task` is "
                     "best used before additional tables are generated. It "
-                    f"will copy the {table} from this cycle without applying "
-                    f"any transformations. This will work well if {table} "
-                    f"contains measurements. But if {table} is a custom ROI "
-                    "table coming from another task, the transformation is "
-                    "not applied and it will not match with the registered "
-                    "image anymore"
+                    f"will copy the {table} from this acquisition without "
+                    "applying any transformations. This will work well if "
+                    f"{table} contains measurements. But if {table} is a "
+                    "custom ROI table coming from another task, the "
+                    "transformation is not applied and it will not match "
+                    "with the registered image anymore."
                 )
             table_dict[table] = table_dict_component[table]
 
     if table_dict:
         logger.info(f"Processing the tables: {table_dict}")
         new_image_group = zarr.group(new_zarr_url)
 
@@ -216,25 +233,33 @@
     ####################
     # Clean up Zarr file
     ####################
     if overwrite_input:
         logger.info(
             "Replace original zarr image with the newly created Zarr image"
         )
-        # Potential for race conditions: Every cycle reads the
-        # reference cycle, but the reference cycle also gets modified
+        # Potential for race conditions: Every acquisition reads the
+        # reference acquisition, but the reference acquisition also gets
+        # modified
         # See issue #516 for the details
         os.rename(zarr_url, f"{zarr_url}_tmp")
         os.rename(new_zarr_url, zarr_url)
         shutil.rmtree(f"{zarr_url}_tmp")
         image_list_updates = dict(image_list_updates=[dict(zarr_url=zarr_url)])
     else:
         image_list_updates = dict(
             image_list_updates=[dict(zarr_url=new_zarr_url, origin=zarr_url)]
         )
+        # Update the metadata of the the well
+        well_url, new_img_path = _split_well_path_image_path(new_zarr_url)
+        _update_well_metadata(
+            well_url=well_url,
+            old_image_path=old_img_path,
+            new_image_path=new_img_path,
+        )
 
     return image_list_updates
 
 
 def write_registered_zarr(
     zarr_url: str,
     new_zarr_url: str,
@@ -256,15 +281,15 @@
     the two lists of ROI indices vary.
 
     Args:
         zarr_url: Path or url to the individual OME-Zarr image to be used as
             the basis for the new OME-Zarr image.
         new_zarr_url: Path or url to the new OME-Zarr image to be written
         ROI_table: Fractal ROI table for the component
-        ROI_table_ref: Fractal ROI table for the reference cycle
+        ROI_table_ref: Fractal ROI table for the reference acquisition
         num_levels: Number of pyramid layers to be created (argument of
             `build_pyramid`).
         coarsening_xy: Coarsening factor between pyramid levels
         aggregation_function: Function to be used when downsampling (argument
             of `build_pyramid`).
 
     """
@@ -296,15 +321,15 @@
     # Create dask array with 0s of same shape
     new_array = da.zeros_like(data_array)
 
     # TODO: Add sanity checks on the 2 ROI tables:
     # 1. The number of ROIs need to match
     # 2. The size of the ROIs need to match
     # (otherwise, we can't assign them to the reference regions)
-    # ROI_table_ref vs ROI_table_cycle
+    # ROI_table_ref vs ROI_table_acq
     for i, roi_indices in enumerate(list_indices):
         reference_region = convert_indices_to_regions(list_indices_ref[i])
         region = convert_indices_to_regions(roi_indices)
 
         axes_list = old_ngff_image_meta.axes_names
 
         if axes_list == ["c", "z", "y", "x"]:
```

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/calculate_registration_image_based.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/calculate_registration_image_based.py`

 * *Files 8% similar despite different names*

```diff
@@ -142,92 +142,92 @@
         raise ValueError(
             (
                 f"Table '{roi_table}' (with type '{ref_table_type}') is "
                 "not a valid ROI table."
             )
         )
 
-    # For each cycle, get the relevant info
+    # For each acquisition, get the relevant info
     # TODO: Add additional checks on ROIs?
     if (ROI_table_ref.obs.index != ROI_table_x.obs.index).all():
         raise ValueError(
             "Registration is only implemented for ROIs that match between the "
-            "cycles (e.g. well, FOV ROIs). Here, the ROIs in the reference "
-            "cycles were {ROI_table_ref.obs.index}, but the ROIs in the "
-            "alignment cycle were {ROI_table_x.obs.index}"
+            "acquisitions (e.g. well, FOV ROIs). Here, the ROIs in the "
+            f"reference acquisitions were {ROI_table_ref.obs.index}, but the "
+            f"ROIs in the alignment acquisition were {ROI_table_x.obs.index}"
         )
     # TODO: Make this less restrictive? i.e. could we also run it if different
-    # cycles have different FOVs? But then how do we know which FOVs to match?
+    # acquisitions have different FOVs? But then how do we know which FOVs to
+    # match?
     # If we relax this, downstream assumptions on matching based on order
     # in the list will break.
 
     # Read pixel sizes from zarr attributes
-    ngff_image_meta_cycle_x = load_NgffImageMeta(zarr_url)
+    ngff_image_meta_acq_x = load_NgffImageMeta(zarr_url)
     pxl_sizes_zyx = ngff_image_meta.get_pixel_sizes_zyx(level=0)
-    pxl_sizes_zyx_cycle_x = ngff_image_meta_cycle_x.get_pixel_sizes_zyx(
-        level=0
-    )
+    pxl_sizes_zyx_acq_x = ngff_image_meta_acq_x.get_pixel_sizes_zyx(level=0)
 
-    if pxl_sizes_zyx != pxl_sizes_zyx_cycle_x:
+    if pxl_sizes_zyx != pxl_sizes_zyx_acq_x:
         raise ValueError(
-            "Pixel sizes need to be equal between cycles for registration"
+            "Pixel sizes need to be equal between acquisitions for "
+            "registration."
         )
 
     # Create list of indices for 3D ROIs spanning the entire Z direction
     list_indices_ref = convert_ROI_table_to_indices(
         ROI_table_ref,
         level=level,
         coarsening_xy=coarsening_xy,
         full_res_pxl_sizes_zyx=pxl_sizes_zyx,
     )
     check_valid_ROI_indices(list_indices_ref, roi_table)
 
-    list_indices_cycle_x = convert_ROI_table_to_indices(
+    list_indices_acq_x = convert_ROI_table_to_indices(
         ROI_table_x,
         level=level,
         coarsening_xy=coarsening_xy,
         full_res_pxl_sizes_zyx=pxl_sizes_zyx,
     )
-    check_valid_ROI_indices(list_indices_cycle_x, roi_table)
+    check_valid_ROI_indices(list_indices_acq_x, roi_table)
 
     num_ROIs = len(list_indices_ref)
     compute = True
     new_shifts = {}
     for i_ROI in range(num_ROIs):
         logger.info(
             f"Now processing ROI {i_ROI+1}/{num_ROIs} "
             f"for channel {channel_align}."
         )
         img_ref = load_region(
             data_zyx=data_reference_zyx,
             region=convert_indices_to_regions(list_indices_ref[i_ROI]),
             compute=compute,
         )
-        img_cycle_x = load_region(
+        img_acq_x = load_region(
             data_zyx=data_alignment_zyx,
-            region=convert_indices_to_regions(list_indices_cycle_x[i_ROI]),
+            region=convert_indices_to_regions(list_indices_acq_x[i_ROI]),
             compute=compute,
         )
 
         ##############
         #  Calculate the transformation
         ##############
         # Basic version (no padding, no internal binning)
-        if img_ref.shape != img_cycle_x.shape:
+        if img_ref.shape != img_acq_x.shape:
             raise NotImplementedError(
                 "This registration is not implemented for ROIs with "
-                "different shapes between cycles"
+                "different shapes between acquisitions."
             )
         shifts = phase_cross_correlation(
-            np.squeeze(img_ref), np.squeeze(img_cycle_x)
+            np.squeeze(img_ref), np.squeeze(img_acq_x)
         )[0]
 
         # Registration based on scmultiplex, image-based
         # shifts, _, _ = calculate_shift(np.squeeze(img_ref),
-        #           np.squeeze(img_cycle_x), bin=binning, binarize=False)
+        #           np.squeeze(img_acq_x), bin=binning, binarize=False)
 
         # TODO: Make this work on label images
         # (=> different loading) etc.
 
         ##############
         # Storing the calculated transformation ###
         ##############
```

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/cellpose_segmentation.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/cellpose_segmentation.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/cellpose_transforms.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/cellpose_transforms.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_compute.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_compute.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,30 +15,28 @@
 import logging
 
 import dask.array as da
 import zarr
 from anndata import read_zarr
 from dask.array.image import imread
 from pydantic.decorator import validate_arguments
-from zarr.errors import ContainsArrayError
 
 from fractal_tasks_core.cellvoyager.filenames import (
     glob_with_multiple_patterns,
 )
 from fractal_tasks_core.cellvoyager.filenames import parse_filename
 from fractal_tasks_core.channels import get_omero_channel_list
 from fractal_tasks_core.channels import OmeroChannel
 from fractal_tasks_core.ngff import load_NgffImageMeta
 from fractal_tasks_core.pyramids import build_pyramid
 from fractal_tasks_core.roi import check_valid_ROI_indices
 from fractal_tasks_core.roi import (
     convert_ROI_table_to_indices,
 )
 from fractal_tasks_core.tasks.io_models import InitArgsCellVoyager
-from fractal_tasks_core.zarr_utils import OverwriteNotAllowedError
 
 
 logger = logging.getLogger(__name__)
 
 
 def sort_fun(filename: str) -> list[int]:
     """
@@ -57,30 +55,31 @@
 
 @validate_arguments
 def cellvoyager_to_ome_zarr_compute(
     *,
     # Fractal parameters
     zarr_url: str,
     init_args: InitArgsCellVoyager,
-    # Advanced parameters
-    overwrite: bool = False,
 ):
     """
     Convert Yokogawa output (png, tif) to zarr file.
 
-    This task is typically run after Create OME-Zarr or
-    Create OME-Zarr Multiplexing and populates the empty OME-Zarr files that
-    were prepared.
+    This task is run after an init task (typically
+    `cellvoyager_to_ome_zarr_init` or
+    `cellvoyager_to_ome_zarr_init_multiplex`), and it populates the empty
+    OME-Zarr files that were prepared.
+
+    Note that the current task always overwrites existing data. To avoid this
+    behavior, set the `overwrite` argument of the init task to `False`.
 
     Args:
         zarr_url: Path or url to the individual OME-Zarr image to be processed.
             (standard argument for Fractal tasks, managed by Fractal server).
         init_args: Intialization arguments provided by
             `create_cellvoyager_ome_zarr_init`.
-        overwrite: If `True`, overwrite the task output.
     """
 
     # Read attributes from NGFF metadata
     ngff_image_meta = load_NgffImageMeta(zarr_url)
     num_levels = ngff_image_meta.num_levels
     coarsening_xy = ngff_image_meta.coarsening_xy
     full_res_pxl_sizes_zyx = ngff_image_meta.get_pixel_sizes_zyx(level=0)
@@ -127,31 +126,22 @@
         folder=init_args.image_dir,
         patterns=patterns,
     )
     sample = imread(tmp_images.pop())
 
     # Initialize zarr
     chunksize = (1, 1, sample.shape[1], sample.shape[2])
-    try:
-        canvas_zarr = zarr.create(
-            shape=(len(wavelength_ids), max_z, max_y, max_x),
-            chunks=chunksize,
-            dtype=sample.dtype,
-            store=zarr.storage.FSStore(zarr_url + "/0"),
-            overwrite=overwrite,
-            dimension_separator="/",
-        )
-    except ContainsArrayError as e:
-        error_msg = (
-            f"Cannot create a zarr group at '{zarr_url}/0', "
-            f"with {overwrite=} (original error: {str(e)}).\n"
-            "Hint: try setting overwrite=True."
-        )
-        logger.error(error_msg)
-        raise OverwriteNotAllowedError(error_msg)
+    canvas_zarr = zarr.create(
+        shape=(len(wavelength_ids), max_z, max_y, max_x),
+        chunks=chunksize,
+        dtype=sample.dtype,
+        store=zarr.storage.FSStore(zarr_url + "/0"),
+        overwrite=True,
+        dimension_separator="/",
+    )
 
     # Loop over channels
     for i_c, wavelength_id in enumerate(wavelength_ids):
         A, C = wavelength_id.split("_")
 
         patterns = [
             f"{init_args.plate_prefix}_{init_args.well_ID}_*{A}*{C}*."
@@ -191,15 +181,15 @@
                 compute=True,
             )
 
     # Starting from on-disk highest-resolution data, build and write to disk a
     # pyramid of coarser levels
     build_pyramid(
         zarrurl=zarr_url,
-        overwrite=overwrite,
+        overwrite=True,
         num_levels=num_levels,
         coarsening_xy=coarsening_xy,
         chunksize=chunksize,
     )
 
     # Generate image list updates
     # TODO: Can we check for dimensionality more robustly? Just checks for the
```

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 from fractal_tasks_core.cellvoyager.filenames import (
     glob_with_multiple_patterns,
 )
 from fractal_tasks_core.cellvoyager.filenames import parse_filename
 from fractal_tasks_core.cellvoyager.metadata import (
     parse_yokogawa_metadata,
 )
+from fractal_tasks_core.cellvoyager.wells import generate_row_col_split
+from fractal_tasks_core.cellvoyager.wells import get_filename_well_id
 from fractal_tasks_core.channels import check_unique_wavelength_ids
 from fractal_tasks_core.channels import define_omero_channels
 from fractal_tasks_core.channels import OmeroChannel
 from fractal_tasks_core.ngff.specs import NgffImageMeta
 from fractal_tasks_core.ngff.specs import Plate
 from fractal_tasks_core.ngff.specs import Well
 from fractal_tasks_core.roi import prepare_FOV_ROI_table
@@ -324,17 +326,16 @@
                 raise ValueError(
                     f"ERROR: well {well} in plate {plate} (prefix: "
                     f"{plate_prefix}) has missing channels.\n"
                     f"Expected: {actual_channels}\n"
                     f"Found: {well_wavelength_ids}.\n"
                 )
 
-        well_rows_columns = [
-            ind for ind in sorted([(n[0], n[1:]) for n in wells])
-        ]
+        well_rows_columns = generate_row_col_split(wells)
+
         row_list = [
             well_row_column[0] for well_row_column in well_rows_columns
         ]
         col_list = [
             well_row_column[1] for well_row_column in well_rows_columns
         ]
         row_list = sorted(list(set(row_list)))
@@ -363,15 +364,15 @@
         for row, column in well_rows_columns:
             parallelization_list.append(
                 {
                     "zarr_url": f"{zarr_dir}/{plate}.zarr/{row}/{column}/0/",
                     "init_args": InitArgsCellVoyager(
                         image_dir=in_path,
                         plate_prefix=plate_prefix,
-                        well_ID=f"{row}{column}",
+                        well_ID=get_filename_well_id(row, column),
                         image_extension=image_extension,
                         image_glob_patterns=image_glob_patterns,
                     ).dict(),
                 }
             )
             group_well = group_plate.create_group(f"{row}/{column}/")
 
@@ -437,15 +438,15 @@
                 ),
             }
 
             # Validate Image attrs
             NgffImageMeta(**group_image.attrs)
 
             # Prepare AnnData tables for FOV/well ROIs
-            well_id = row + column
+            well_id = get_filename_well_id(row, column)
             FOV_ROIs_table = prepare_FOV_ROI_table(site_metadata.loc[well_id])
             well_ROIs_table = prepare_well_ROI_table(
                 site_metadata.loc[well_id]
             )
 
             # Write AnnData tables into the `tables` zarr group
             write_table(
```

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init_multiplex.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init_multiplex.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 from fractal_tasks_core.cellvoyager.filenames import (
     glob_with_multiple_patterns,
 )
 from fractal_tasks_core.cellvoyager.filenames import parse_filename
 from fractal_tasks_core.cellvoyager.metadata import (
     parse_yokogawa_metadata,
 )
+from fractal_tasks_core.cellvoyager.wells import generate_row_col_split
+from fractal_tasks_core.cellvoyager.wells import get_filename_well_id
 from fractal_tasks_core.channels import check_unique_wavelength_ids
 from fractal_tasks_core.channels import check_well_channel_labels
 from fractal_tasks_core.channels import define_omero_channels
 from fractal_tasks_core.ngff.specs import NgffImageMeta
 from fractal_tasks_core.ngff.specs import Plate
 from fractal_tasks_core.ngff.specs import Well
 from fractal_tasks_core.roi import prepare_FOV_ROI_table
@@ -65,17 +67,17 @@
     image_extension: str = "tif",
     metadata_table_files: Optional[dict[str, str]] = None,
     overwrite: bool = False,
 ) -> dict[str, Any]:
     """
     Create OME-NGFF structure and metadata to host a multiplexing dataset.
 
-    This task takes a set of image folders (i.e. different acquisition cycles)
-    and build the internal structure and metadata of a OME-NGFF zarr group,
-    without actually loading/writing the image data.
+    This task takes a set of image folders (i.e. different multiplexing
+    acquisitions) and build the internal structure and metadata of a OME-NGFF
+    zarr group, without actually loading/writing the image data.
 
     Each element in input_paths should be treated as a different acquisition.
 
     Args:
         zarr_urls: List of paths or urls to the individual OME-Zarr image to
             be processed. Not used by the converter task.
             (standard argument for Fractal tasks, managed by Fractal server).
@@ -336,17 +338,15 @@
                 raise ValueError(
                     f"ERROR: well {well} in plate {plate} (prefix: "
                     f"{plate_prefix}) has missing channels.\n"
                     f"Expected: {actual_wavelength_ids}\n"
                     f"Found: {well_wavelength_ids}.\n"
                 )
 
-        well_rows_columns = [
-            ind for ind in sorted([(n[0], n[1:]) for n in wells])
-        ]
+        well_rows_columns = generate_row_col_split(wells)
         row_list = [
             well_row_column[0] for well_row_column in well_rows_columns
         ]
         col_list = [
             well_row_column[1] for well_row_column in well_rows_columns
         ]
         row_list = sorted(list(set(row_list)))
@@ -374,15 +374,15 @@
                     "zarr_url": (
                         f"{zarr_dir}/{plate}.zarr/{row}/{column}/"
                         f"{acquisition}/"
                     ),
                     "init_args": InitArgsCellVoyager(
                         image_dir=acquisitions[acquisition].image_dir,
                         plate_prefix=plate_prefix,
-                        well_ID=f"{row}{column}",
+                        well_ID=get_filename_well_id(row, column),
                         image_extension=image_extension,
                         image_glob_patterns=image_glob_patterns,
                         acquisition=acquisition,
                     ).dict(),
                 }
             )
             try:
@@ -479,15 +479,15 @@
                     label_prefix=acquisition,
                 ),
             }
             # Validate Image attrs
             NgffImageMeta(**group_image.attrs)
 
             # Prepare AnnData tables for FOV/well ROIs
-            well_id = row + column
+            well_id = get_filename_well_id(row, column)
             FOV_ROIs_table = prepare_FOV_ROI_table(site_metadata.loc[well_id])
             well_ROIs_table = prepare_well_ROI_table(
                 site_metadata.loc[well_id]
             )
 
             # Write AnnData tables into the `tables` zarr group
             write_table(
@@ -501,16 +501,16 @@
                 group_image,
                 "well_ROI_table",
                 well_ROIs_table,
                 overwrite=overwrite,
                 table_attrs={"type": "roi_table"},
             )
 
-    # Check that the different images (e.g. different cycles) in the each well
-    # have unique labels
+    # Check that the different images (e.g. different acquisitions) in the each
+    # well have unique labels
     for well_path in zarrurls["well"]:
         check_well_channel_labels(
             well_zarr_path=str(Path(zarr_dir) / well_path)
         )
 
     return dict(parallelization_list=parallelization_list)
```

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/copy_ome_zarr_hcs_plate.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/copy_ome_zarr_hcs_plate.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/find_registration_consensus.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/find_registration_consensus.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,26 +49,26 @@
     # Advanced parameters
     new_roi_table: Optional[str] = None,
 ):
     """
     Applies pre-calculated registration to ROI tables.
 
     Apply pre-calculated registration such that resulting ROIs contain
-    the consensus align region between all cycles.
+    the consensus align region between all acquisitions.
 
     Parallelization level: well
 
     Args:
         zarr_url: Path or url to the individual OME-Zarr image to be processed.
-            Refers to the zarr_url of the reference cycle.
+            Refers to the zarr_url of the reference acquisition.
             (standard argument for Fractal tasks, managed by Fractal server).
         init_args: Intialization arguments provided by
             `init_group_by_well_for_multiplexing`. It contains the
             zarr_url_list listing all the zarr_urls in the same well as the
-            zarr_url of the reference cycle that are being processed.
+            zarr_url of the reference acquisition that are being processed.
             (standard argument for Fractal tasks, managed by Fractal server).
         roi_table: Name of the ROI table over which the task loops to
             calculate the registration. Examples: `FOV_ROI_table` => loop over
             the field of views, `well_ROI_table` => process the whole well as
             one image.
         new_roi_table: Optional name for the new, registered ROI table. If no
             name is given, it will default to "registered_" + `roi_table`
@@ -88,15 +88,15 @@
     for acq_zarr_url in init_args.zarr_url_list:
         curr_ROI_table = ad.read_zarr(f"{acq_zarr_url}/tables/{roi_table}")
         curr_ROI_table_group = zarr.open_group(
             f"{acq_zarr_url}/tables/{roi_table}", mode="r"
         )
         curr_ROI_table_attrs = curr_ROI_table_group.attrs.asdict()
 
-        # For reference_cycle acquisition, handle the fact that it doesn't
+        # For reference_acquisition, handle the fact that it doesn't
         # have the shifts
         if acq_zarr_url == zarr_url:
             curr_ROI_table = add_zero_translation_columns(curr_ROI_table)
         # Check for valid ROI tables
         are_ROI_table_columns_valid(table=curr_ROI_table)
         translation_columns = [
             "translation_z",
@@ -123,15 +123,15 @@
                 f"{zarr_url}: {rois}"
             )
 
     roi_table_dfs = [
         roi_table.to_df().loc[:, translation_columns]
         for roi_table in roi_tables.values()
     ]
-    logger.info("Calculating min & max translation across cycles.")
+    logger.info("Calculating min & max translation across acquisitions.")
     max_df, min_df = calculate_min_max_across_dfs(roi_table_dfs)
     shifted_rois = {}
 
     # Loop over acquisitions
     for acq_zarr_url in init_args.zarr_url_list:
         shifted_rois[acq_zarr_url] = apply_registration_to_single_ROI_table(
             roi_tables[acq_zarr_url], max_df, min_df
```

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/illumination_correction.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/illumination_correction.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from fractal_tasks_core.ngff import load_NgffImageMeta
 from fractal_tasks_core.pyramids import build_pyramid
 from fractal_tasks_core.roi import check_valid_ROI_indices
 from fractal_tasks_core.roi import (
     convert_ROI_table_to_indices,
 )
 from fractal_tasks_core.tasks._zarr_utils import _copy_hcs_ome_zarr_metadata
+from fractal_tasks_core.tasks._zarr_utils import _copy_tables_from_zarr_url
 
 logger = logging.getLogger(__name__)
 
 
 def correct(
     img_stack: np.ndarray,
     corr_img: np.ndarray,
@@ -224,14 +225,17 @@
             chunks=data_czyx.chunksize,
             dtype=data_czyx.dtype,
             store=zarr.storage.FSStore(f"{zarr_url_new}/0"),
             overwrite=False,
             dimension_separator="/",
         )
         _copy_hcs_ome_zarr_metadata(zarr_url, zarr_url_new)
+        # Copy ROI tables from the old zarr_url to keep ROI tables and other
+        # tables available in the new Zarr
+        _copy_tables_from_zarr_url(zarr_url, zarr_url_new)
 
     # Iterate over FOV ROIs
     num_ROIs = len(list_indices)
     for i_c, channel in enumerate(channels):
         for i_ROI, indices in enumerate(list_indices):
             # Define region
             s_z, e_z, s_y, e_y, s_x, e_x = indices[:]
```

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/image_based_registration_hcs_init.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/image_based_registration_hcs_init.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,61 +27,62 @@
 @validate_arguments
 def image_based_registration_hcs_init(
     *,
     # Fractal parameters
     zarr_urls: list[str],
     zarr_dir: str,
     # Core parameters
-    reference_cycle: int = 0,
+    reference_acquisition: int = 0,
 ) -> dict[str, list[dict[str, Any]]]:
     """
     Initialized calculate registration task
 
     This task prepares a parallelization list of all zarr_urls that need to be
-    used to calculate the registration between cycles (all zarr_urls except
-    the reference cycle vs. the reference cycle).
+    used to calculate the registration between acquisitions (all zarr_urls
+    except the reference acquisition vs. the reference acquisition).
     This task only works for HCS OME-Zarrs for 2 reasons: Only HCS OME-Zarrs
-    currently have defined acquisition metadata to determine reference cycles.
-    And we have only implemented the grouping of images for HCS OME-Zarrs by
-    well (with the assumption that every well just has 1 image per acqusition).
+    currently have defined acquisition metadata to determine reference
+    acquisitions. And we have only implemented the grouping of images for
+    HCS OME-Zarrs by well (with the assumption that every well just has 1
+    image per acqusition).
 
     Args:
         zarr_urls: List of paths or urls to the individual OME-Zarr image to
             be processed.
             (standard argument for Fractal tasks, managed by Fractal server).
         zarr_dir: path of the directory where the new OME-Zarrs will be
             created. Not used by this task.
             (standard argument for Fractal tasks, managed by Fractal server).
-        reference_cycle: Which cycle to register against. Needs to match the
-            acquisition metadata in the OME-Zarr image.
+        reference_acquisition: Which acquisition to register against. Needs to
+            match the acquisition metadata in the OME-Zarr image.
 
     Returns:
         task_output: Dictionary for Fractal server that contains a
             parallelization list.
     """
     logger.info(
         f"Running `image_based_registration_hcs_init` for {zarr_urls=}"
     )
     image_groups = create_well_acquisition_dict(zarr_urls)
 
     # Create the parallelization list
     parallelization_list = []
     for key, image_group in image_groups.items():
-        # Assert that all image groups have the reference cycle present
-        if reference_cycle not in image_group.keys():
+        # Assert that all image groups have the reference acquisition present
+        if reference_acquisition not in image_group.keys():
             raise ValueError(
-                f"Registration with {reference_cycle=} can only work if all"
-                "wells have the reference cycle present. It was not found"
-                f"for well {key}."
+                f"Registration with {reference_acquisition=} can only work if "
+                "all wells have the reference acquisition present. It was not "
+                f"found for well {key}."
             )
-        # Add all zarr_urls except the reference cycle to the
+        # Add all zarr_urls except the reference acquisition to the
         # parallelization list
         for acquisition, zarr_url in image_group.items():
-            if acquisition != reference_cycle:
-                reference_zarr_url = image_group[reference_cycle]
+            if acquisition != reference_acquisition:
+                reference_zarr_url = image_group[reference_acquisition]
                 parallelization_list.append(
                     dict(
                         zarr_url=zarr_url,
                         init_args=dict(reference_zarr_url=reference_zarr_url),
                     )
                 )
```

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/import_ome_zarr.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/import_ome_zarr.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,16 +61,14 @@
     """
 
     # Note from zarr docs: `r+` means read/write (must exist)
     image_group = zarr.open_group(image_path, mode="r+")
     image_meta = NgffImageMeta(**image_group.attrs.asdict())
 
     # Preliminary checks
-    if not (add_image_ROI_table or add_grid_ROI_table):
-        return
     if add_grid_ROI_table and (grid_YX_shape is None):
         raise ValueError(
             f"_process_single_image called with {add_grid_ROI_table=}, "
             f"but {grid_YX_shape=}."
         )
 
     pixels_ZYX = image_meta.get_pixel_sizes_zyx(level=0)
@@ -259,27 +257,28 @@
             "Only OME-Zarr for plates are fully supported in Fractal; "
             f"e.g. the current one ({ngff_type=}) cannot be "
             "processed via the `maximum_intensity_projection` task."
         )
         for image in root_group.attrs["well"]["images"]:
             image_path = image["path"]
             zarr_url = f"{zarr_path}/{image_path}"
+            well_name = "".join(zarr_path.split("/")[-2:])
             types = _process_single_image(
                 zarr_url,
                 add_image_ROI_table,
                 add_grid_ROI_table,
                 update_omero_metadata,
                 grid_YX_shape=grid_YX_shape,
                 overwrite=overwrite,
             )
             image_list_updates.append(
                 dict(
                     zarr_url=zarr_url,
                     attributes=dict(
-                        well=zarr_name,
+                        well=well_name,
                     ),
                     types=types,
                 )
             )
     elif ngff_type == "image":
         logger.warning(
             "Only OME-Zarr for plates are fully supported in Fractal; "
```

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/init_group_by_well_for_multiplexing.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/init_group_by_well_for_multiplexing.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,51 +26,52 @@
 @validate_arguments
 def init_group_by_well_for_multiplexing(
     *,
     # Fractal parameters
     zarr_urls: list[str],
     zarr_dir: str,
     # Core parameters
-    reference_cycle: int = 0,
+    reference_acquisition: int = 0,
 ) -> dict[str, list[str]]:
     """
     Finds images for all acquisitions per well.
 
     Returns the parallelization_list to run `find_registration_consensus`.
 
     Args:
         zarr_urls: List of paths or urls to the individual OME-Zarr image to
             be processed.
             (standard argument for Fractal tasks, managed by Fractal server).
         zarr_dir: path of the directory where the new OME-Zarrs will be
             created. Not used by this task.
             (standard argument for Fractal tasks, managed by Fractal server).
-        reference_cycle: Which cycle to register against. Uses the OME-NGFF
-            HCS well metadata acquisition keys to find the reference cycle.
+        reference_acquisition: Which acquisition to register against. Uses the
+            OME-NGFF HCS well metadata acquisition keys to find the reference
+            acquisition.
     """
     logger.info(
         f"Running `init_group_by_well_for_multiplexing` for {zarr_urls=}"
     )
     image_groups = create_well_acquisition_dict(zarr_urls)
 
     # Create the parallelization list
     parallelization_list = []
     for key, image_group in image_groups.items():
-        # Assert that all image groups have the reference cycle present
-        if reference_cycle not in image_group.keys():
+        # Assert that all image groups have the reference acquisition present
+        if reference_acquisition not in image_group.keys():
             raise ValueError(
-                f"Registration with {reference_cycle=} can only work if all"
-                "wells have the reference cycle present. It was not found"
-                f"for well {key}."
+                f"Registration with {reference_acquisition=} can only work if "
+                "all wells have the reference acquisition present. It was not "
+                f"found for well {key}."
             )
 
         # Create a parallelization list entry for each image group
         zarr_url_list = []
         for acquisition, zarr_url in image_group.items():
-            if acquisition == reference_cycle:
+            if acquisition == reference_acquisition:
                 reference_zarr_url = zarr_url
 
             zarr_url_list.append(zarr_url)
 
         parallelization_list.append(
             dict(
                 zarr_url=reference_zarr_url,
```

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/io_models.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/io_models.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/maximum_intensity_projection.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/maximum_intensity_projection.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/napari_workflows_wrapper.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/napari_workflows_wrapper.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/upscale_array.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/upscale_array.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/utils.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/fractal_tasks_core/zarr_utils.py` & `fractal_tasks_core-1.0.1/fractal_tasks_core/zarr_utils.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a3/pyproject.toml` & `fractal_tasks_core-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-tasks-core"
-version = "1.0.0a3"
+version = "1.0.1"
 description = "Core bioimage-analysis library and tasks of the Fractal analytics platform"
 authors = [
     "Joel Lüthi  <joel.luethi@fmi.ch>",
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
 ]
@@ -30,14 +30,15 @@
 numpy = "<2"
 pandas = ">=1.2.0,<2"
 defusedxml = "^0.7.1"
 lxml = "^4.9.1"
 pydantic = "<2"
 docstring-parser = "^0.15"
 anndata = ">=0.8.0,<0.11.0"
+filelock = "3.13.*"
 
 # Optional dependencies (used in extras)
 Pillow = { version = ">=9.1.1", optional = true }
 imageio-ffmpeg = { version = "^0.4.7", optional = true }
 scikit-image = { version = ">=0.19", optional = true }
 napari-segment-blobs-and-things-with-membranes = { version = "^0.3.3", optional = true }
 napari-workflows = { version = "^0.2.8", optional = true }
@@ -85,15 +86,15 @@
 branch = true
 parallel = true
 relative_files = true
 source = ["fractal_tasks_core"]
 omit = ["tests/*", "examples/*", "fractal_tasks_core/dev/*"]
 
 [tool.bumpver]
-current_version = "1.0.0a3"
+current_version = "1.0.1"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

