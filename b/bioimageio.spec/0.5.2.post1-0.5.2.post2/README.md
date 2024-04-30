# Comparing `tmp/bioimageio.spec-0.5.2.post1.tar.gz` & `tmp/bioimageio.spec-0.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioimageio.spec-0.5.2.post1.tar", last modified: Mon Apr 22 20:14:44 2024, max compression
+gzip compressed data, was "bioimageio.spec-0.5.2.post2.tar", last modified: Tue Apr 30 11:45:16 2024, max compression
```

## Comparing `bioimageio.spec-0.5.2.post1.tar` & `bioimageio.spec-0.5.2.post2.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:14:44.833174 bioimageio.spec-0.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    19029 2024-04-22 20:14:44.833174 bioimageio.spec-0.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18200 2024-04-22 20:14:43.000000 bioimageio.spec-0.5.2.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:14:44.813174 bioimageio.spec-0.5.2.post1/bioimageio/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:14:44.821174 bioimageio.spec-0.5.2.post1/bioimageio/spec/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-22 20:14:43.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/_build_description.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/_description.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:14:44.821174 bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10694 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/_generated_spdx_license_literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16162 2024-04-22 20:14:43.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/common_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/docs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/field_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/field_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)    20499 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/io_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/license_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-22 20:14:43.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/packaging_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/root_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/url.py
--rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/validated_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/validation_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/validator_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/version_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/warning_levels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     9712 2024-04-22 20:14:43.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/_package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:14:44.825174 bioimageio.spec-0.5.2.post1/bioimageio/spec/application/
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/application/v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/application/v0_3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:14:44.825174 bioimageio.spec-0.5.2.post1/bioimageio/spec/collection/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11116 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/collection/v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12553 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/collection/v0_3.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:14:44.825174 bioimageio.spec-0.5.2.post1/bioimageio/spec/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/dataset/v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/dataset/v0_3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:14:44.825174 bioimageio.spec-0.5.2.post1/bioimageio/spec/generic/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/generic/_v0_2_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/generic/_v0_3_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    15487 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/generic/v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/generic/v0_3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:14:44.825174 bioimageio.spec-0.5.2.post1/bioimageio/spec/model/
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/model/_v0_3_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/model/_v0_4_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    41548 2024-04-22 20:14:43.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/model/v0_4.py
--rw-r--r--   0 runner    (1001) docker     (127)   101035 2024-04-22 20:14:43.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/model/v0_5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:14:44.825174 bioimageio.spec-0.5.2.post1/bioimageio/spec/notebook/
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/notebook/v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/notebook/v0_3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:14:44.825174 bioimageio.spec-0.5.2.post1/bioimageio/spec/partner_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/partner_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:14:44.825174 bioimageio.spec-0.5.2.post1/bioimageio/spec/partner_utils/imjoy/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/partner_utils/imjoy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/partner_utils/imjoy/_plugin_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/pretty_validation_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:14:44.829174 bioimageio.spec-0.5.2.post1/bioimageio/spec/static/
--rw-r--r--   0 runner    (1001) docker     (127)   258617 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/static/spdx_licenses.json
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/static/tag_categories.json
--rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/bioimageio/spec/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:14:44.817174 bioimageio.spec-0.5.2.post1/bioimageio.spec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19029 2024-04-22 20:14:44.000000 bioimageio.spec-0.5.2.post1/bioimageio.spec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-22 20:14:44.000000 bioimageio.spec-0.5.2.post1/bioimageio.spec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 20:14:44.000000 bioimageio.spec-0.5.2.post1/bioimageio.spec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-22 20:14:44.000000 bioimageio.spec-0.5.2.post1/bioimageio.spec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-22 20:14:44.000000 bioimageio.spec-0.5.2.post1/bioimageio.spec.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:14:44.817174 bioimageio.spec-0.5.2.post1/example_descriptions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:14:44.817174 bioimageio.spec-0.5.2.post1/example_descriptions/collections/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:14:44.829174 bioimageio.spec-0.5.2.post1/example_descriptions/collections/unet2d_nuclei_broad_coll/
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/example_descriptions/collections/unet2d_nuclei_broad_coll/unet2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:14:44.817174 bioimageio.spec-0.5.2.post1/example_descriptions/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:14:44.829174 bioimageio.spec-0.5.2.post1/example_descriptions/models/unet2d_diff_output_shape/
--rw-r--r--   0 runner    (1001) docker     (127)    12778 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/example_descriptions/models/unet2d_diff_output_shape/resize_unet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:14:44.829174 bioimageio.spec-0.5.2.post1/example_descriptions/models/unet2d_fixed_shape/
--rw-r--r--   0 runner    (1001) docker     (127)    21841 2024-04-22 20:12:27.000000 bioimageio.spec-0.5.2.post1/example_descriptions/models/unet2d_fixed_shape/unet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:14:44.829174 bioimageio.spec-0.5.2.post1/example_descriptions/models/unet2d_multi_tensor/
--rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/example_descriptions/models/unet2d_multi_tensor/multi_tensor_unet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:14:44.829174 bioimageio.spec-0.5.2.post1/example_descriptions/models/unet2d_nuclei_broad/
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/example_descriptions/models/unet2d_nuclei_broad/unet2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/example_descriptions/models/unet2d_nuclei_broad/unet2d_expand_output_shape.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:14:44.829174 bioimageio.spec-0.5.2.post1/example_descriptions/models/upsample_test_model/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/example_descriptions/models/upsample_test_model/upsample_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:14:44.829174 bioimageio.spec-0.5.2.post1/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/scripts/compare_yaml_syntax.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/scripts/generate_dtype_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/scripts/generate_json_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    17796 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/scripts/generate_spec_documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/scripts/generate_version_submodule_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)    12159 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/scripts/report_invalid_rdfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/scripts/update_spdx_licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 20:14:44.833174 bioimageio.spec-0.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:14:44.829174 bioimageio.spec-0.5.2.post1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/tests/test_bioimageio_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/tests/test_description.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/tests/test_example_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:14:44.829174 bioimageio.spec-0.5.2.post1/tests/test_generic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/tests/test_generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/tests/test_generic/test_v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/tests/test_generic/test_v0_3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:14:44.833174 bioimageio.spec-0.5.2.post1/tests/test_internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/tests/test_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/tests/test_internal/test_base_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/tests/test_internal/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/tests/test_internal/test_file_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/tests/test_internal/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/tests/test_internal/test_license_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/tests/test_internal/test_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/tests/test_internal/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/tests/test_internal/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/tests/test_internal/test_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/tests/test_internal/test_validated_string.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/tests/test_internal/test_version_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/tests/test_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:14:44.833174 bioimageio.spec-0.5.2.post1/tests/test_model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/tests/test_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16073 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/tests/test_model/test_v0_4.py
--rw-r--r--   0 runner    (1001) docker     (127)    15505 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/tests/test_model/test_v0_5.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-22 20:12:28.000000 bioimageio.spec-0.5.2.post1/tests/test_specific_reexports_generics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:45:16.256175 bioimageio.spec-0.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    19190 2024-04-30 11:45:16.256175 bioimageio.spec-0.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18361 2024-04-30 11:45:14.000000 bioimageio.spec-0.5.2.post2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:45:16.236175 bioimageio.spec-0.5.2.post2/bioimageio/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:45:16.244175 bioimageio.spec-0.5.2.post2/bioimageio/spec/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-30 11:45:14.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/_build_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/_description.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:45:16.244175 bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10694 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/_generated_spdx_license_literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-30 11:45:14.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16162 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/common_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/docs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/field_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/field_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20589 2024-04-30 11:45:14.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/io_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9853 2024-04-30 11:45:14.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/license_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/packaging_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/root_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/validated_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/validation_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/validator_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/version_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/warning_levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9712 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/_package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:45:16.248175 bioimageio.spec-0.5.2.post2/bioimageio/spec/application/
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/application/v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/application/v0_3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:45:16.248175 bioimageio.spec-0.5.2.post2/bioimageio/spec/collection/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11116 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/collection/v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12926 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/collection/v0_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:45:16.248175 bioimageio.spec-0.5.2.post2/bioimageio/spec/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/dataset/v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/dataset/v0_3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:45:16.248175 bioimageio.spec-0.5.2.post2/bioimageio/spec/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/generic/_v0_2_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/generic/_v0_3_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15487 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/generic/v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/generic/v0_3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:45:16.248175 bioimageio.spec-0.5.2.post2/bioimageio/spec/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/model/_v0_3_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/model/_v0_4_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41548 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/model/v0_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101035 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/model/v0_5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:45:16.248175 bioimageio.spec-0.5.2.post2/bioimageio/spec/notebook/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/notebook/v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/notebook/v0_3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:45:16.248175 bioimageio.spec-0.5.2.post2/bioimageio/spec/partner_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/partner_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:45:16.248175 bioimageio.spec-0.5.2.post2/bioimageio/spec/partner_utils/imjoy/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/partner_utils/imjoy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/partner_utils/imjoy/_plugin_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/pretty_validation_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:45:16.252175 bioimageio.spec-0.5.2.post2/bioimageio/spec/static/
+-rw-r--r--   0 runner    (1001) docker     (127)   258617 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/static/spdx_licenses.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/static/tag_categories.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-30 11:45:14.000000 bioimageio.spec-0.5.2.post2/bioimageio/spec/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:45:16.240175 bioimageio.spec-0.5.2.post2/bioimageio.spec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19190 2024-04-30 11:45:16.000000 bioimageio.spec-0.5.2.post2/bioimageio.spec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-30 11:45:16.000000 bioimageio.spec-0.5.2.post2/bioimageio.spec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 11:45:16.000000 bioimageio.spec-0.5.2.post2/bioimageio.spec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-30 11:45:16.000000 bioimageio.spec-0.5.2.post2/bioimageio.spec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-30 11:45:16.000000 bioimageio.spec-0.5.2.post2/bioimageio.spec.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:45:16.240175 bioimageio.spec-0.5.2.post2/example_descriptions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:45:16.240175 bioimageio.spec-0.5.2.post2/example_descriptions/collections/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:45:16.252175 bioimageio.spec-0.5.2.post2/example_descriptions/collections/unet2d_nuclei_broad_coll/
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-30 11:42:46.000000 bioimageio.spec-0.5.2.post2/example_descriptions/collections/unet2d_nuclei_broad_coll/unet2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:45:16.240175 bioimageio.spec-0.5.2.post2/example_descriptions/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:45:16.252175 bioimageio.spec-0.5.2.post2/example_descriptions/models/unet2d_diff_output_shape/
+-rw-r--r--   0 runner    (1001) docker     (127)    12778 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/example_descriptions/models/unet2d_diff_output_shape/resize_unet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:45:16.252175 bioimageio.spec-0.5.2.post2/example_descriptions/models/unet2d_fixed_shape/
+-rw-r--r--   0 runner    (1001) docker     (127)    21841 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/example_descriptions/models/unet2d_fixed_shape/unet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:45:16.252175 bioimageio.spec-0.5.2.post2/example_descriptions/models/unet2d_multi_tensor/
+-rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/example_descriptions/models/unet2d_multi_tensor/multi_tensor_unet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:45:16.252175 bioimageio.spec-0.5.2.post2/example_descriptions/models/unet2d_nuclei_broad/
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/example_descriptions/models/unet2d_nuclei_broad/unet2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/example_descriptions/models/unet2d_nuclei_broad/unet2d_expand_output_shape.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:45:16.252175 bioimageio.spec-0.5.2.post2/example_descriptions/models/upsample_test_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/example_descriptions/models/upsample_test_model/upsample_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:45:16.252175 bioimageio.spec-0.5.2.post2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/scripts/compare_yaml_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/scripts/generate_dtype_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/scripts/generate_json_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17796 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/scripts/generate_spec_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/scripts/generate_version_submodule_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12159 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/scripts/report_invalid_rdfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/scripts/update_spdx_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 11:45:16.256175 bioimageio.spec-0.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-30 11:45:14.000000 bioimageio.spec-0.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:45:16.252175 bioimageio.spec-0.5.2.post2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/tests/test_bioimageio_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/tests/test_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/tests/test_example_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:45:16.256175 bioimageio.spec-0.5.2.post2/tests/test_generic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/tests/test_generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/tests/test_generic/test_v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/tests/test_generic/test_v0_3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:45:16.256175 bioimageio.spec-0.5.2.post2/tests/test_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/tests/test_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/tests/test_internal/test_base_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/tests/test_internal/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/tests/test_internal/test_file_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/tests/test_internal/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/tests/test_internal/test_license_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/tests/test_internal/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/tests/test_internal/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/tests/test_internal/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/tests/test_internal/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/tests/test_internal/test_validated_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/tests/test_internal/test_version_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-30 11:45:14.000000 bioimageio.spec-0.5.2.post2/tests/test_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:45:16.256175 bioimageio.spec-0.5.2.post2/tests/test_model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/tests/test_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16073 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/tests/test_model/test_v0_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15505 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/tests/test_model/test_v0_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-30 11:42:47.000000 bioimageio.spec-0.5.2.post2/tests/test_specific_reexports_generics.py
```

### Comparing `bioimageio.spec-0.5.2.post1/LICENSE` & `bioimageio.spec-0.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/PKG-INFO` & `bioimageio.spec-0.5.2.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioimageio.spec
-Version: 0.5.2.post1
+Version: 0.5.2.post2
 Summary: Parser and validator library for bioimage.io specifications
 Home-page: https://github.com/bioimage-io/spec-bioimage-io
 Author: bioimage.io Team
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bioimage-io/spec-bioimage-io/issues
 Project-URL: Source, https://github.com/bioimage-io/spec-bioimage-io
 Platform: UNKNOWN
@@ -106,14 +106,18 @@
 
 Made with [contrib.rocks](https://contrib.rocks).
 
 ## Δ Changelog
 
 ### bioimageio.spec Python package
 
+#### bioimageio.spec 0.5.2post2
+
+* resolve version (un)specific collection IDs, e.g. `load_description('affable-shark')`, `load_description('affable-shark/1')`
+
 #### bioimageio.spec 0.5.2post1
 
 * fix model packaging with weights format priority
 
 #### bioimageio.spec 0.5.2
 
 * new patch version model 0.5.2
```

### Comparing `bioimageio.spec-0.5.2.post1/README.md` & `bioimageio.spec-0.5.2.post2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,18 @@
 
 Made with [contrib.rocks](https://contrib.rocks).
 
 ## Δ Changelog
 
 ### bioimageio.spec Python package
 
+#### bioimageio.spec 0.5.2post2
+
+* resolve version (un)specific collection IDs, e.g. `load_description('affable-shark')`, `load_description('affable-shark/1')`
+
 #### bioimageio.spec 0.5.2post1
 
 * fix model packaging with weights format priority
 
 #### bioimageio.spec 0.5.2
 
 * new patch version model 0.5.2
```

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/__init__.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/_build_description.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/_build_description.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/_description.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/_description.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/_generated_spdx_license_literals.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/_generated_spdx_license_literals.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/common_nodes.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/common_nodes.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/constants.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/constants.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/docs_utils.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/docs_utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/field_validation.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/field_validation.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/field_warning.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/field_warning.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/io.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/io.py`

 * *Files identical despite different names*

```diff
@@ -564,14 +564,16 @@
         return source.download()
 
     strict_source = interprete_file_source(source)
     if isinstance(strict_source, RelativeFilePath):
         strict_source = strict_source.absolute
 
     if isinstance(strict_source, PurePath):
+        if not strict_source.exists():
+            raise FileNotFoundError(strict_source)
         local_source = strict_source
         root: Union[RootHttpUrl, DirectoryPath] = strict_source.parent
     else:
         if strict_source.scheme not in ("http", "https"):
             raise NotImplementedError(strict_source.scheme)
 
         if settings.CI:
```

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/license_id.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/license_id.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/node.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/node.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/packaging_context.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/packaging_context.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/root_url.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/root_url.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/types.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/types.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/url.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/url.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/utils.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/validated_string.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/validated_string.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/validation_context.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/validation_context.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/validator_annotations.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/validator_annotations.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/version_type.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/version_type.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/_internal/warning_levels.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/_internal/warning_levels.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/_io.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/_io.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/_package.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/_package.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/application/__init__.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/application/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/application/v0_2.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/application/v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/application/v0_3.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/application/v0_3.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/collection/__init__.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/collection/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/collection/v0_2.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/collection/v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/collection/v0_3.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/collection/v0_3.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,17 @@
     The final `id` for each collection entry is composed of the collection's `id`
     and the entry's 'sub-'`id`, specified externally in `descr_source` or superseeded in-place,
     such that the `final_entry_id = <collection_id>/<entry_id>`"""
 
     entry_source: Optional[FileSource] = None
     """an external source this entry description is based on"""
 
+    entry_sha256: Optional[Sha256] = None
+    """SHA256 of `entry_source`"""
+
     id: Optional[ResourceId] = None
     """Collection entry sub id overwriting `rdf_source.id`.
     The full collection entry's id is the collection's base id, followed by this sub id and separated by a slash '/'."""
 
     _descr: Optional[EntryDescr] = PrivateAttr(None)
 
     @property
@@ -192,24 +195,31 @@
 
         for i, entry in enumerate(self.collection):
             entry_data: Dict[str, Any] = dict(common_entry_content)
             # set entry specific root as it might be adapted in the presence of an external entry source
             entry_root = context.root
             entry_file_name = context.file_name
 
-            if entry.entry_source is not None:
+            if entry.entry_source is None:
+                if entry.entry_sha256 is None:
+                    raise ValueError(
+                        f"Got unexpected `entry_sha256` {entry.entry_sha256} for unspecified `entry_source`"
+                    )
+            else:
                 if not context.perform_io_checks:
                     issue_warning(
                         "Skipping IO relying validation for collection[{i}]",
                         value=entry.entry_source,
                         msg_context=dict(i=i),
                     )
                     continue
 
-                external_data = open_bioimageio_yaml(entry.entry_source)
+                external_data = open_bioimageio_yaml(
+                    entry.entry_source, sha256=entry.entry_sha256
+                )
                 # add/overwrite common collection entry content with external source
                 entry_data.update(external_data.content)
                 entry_root = external_data.original_root
                 entry_file_name = external_data.original_file_name
 
             # add/overwrite common+external entry content with in-place entry update
             entry_data.update(entry.entry_update)
```

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/common.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/common.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/dataset/__init__.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/dataset/v0_2.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/dataset/v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/dataset/v0_3.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/dataset/v0_3.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/generic/__init__.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/generic/_v0_2_converter.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/generic/_v0_2_converter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/generic/_v0_3_converter.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/generic/_v0_3_converter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/generic/v0_2.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/generic/v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/generic/v0_3.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/generic/v0_3.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/model/__init__.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/model/_v0_3_converter.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/model/_v0_3_converter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/model/_v0_4_converter.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/model/_v0_4_converter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/model/v0_4.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/model/v0_4.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/model/v0_5.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/model/v0_5.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/notebook/__init__.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/notebook/v0_2.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/notebook/v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/notebook/v0_3.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/notebook/v0_3.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/partner_utils/imjoy/_plugin_parser.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/partner_utils/imjoy/_plugin_parser.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/pretty_validation_errors.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/pretty_validation_errors.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/static/spdx_licenses.json` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/static/spdx_licenses.json`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/static/tag_categories.json` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/static/tag_categories.json`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio/spec/summary.py` & `bioimageio.spec-0.5.2.post2/bioimageio/spec/summary.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio.spec.egg-info/PKG-INFO` & `bioimageio.spec-0.5.2.post2/bioimageio.spec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioimageio.spec
-Version: 0.5.2.post1
+Version: 0.5.2.post2
 Summary: Parser and validator library for bioimage.io specifications
 Home-page: https://github.com/bioimage-io/spec-bioimage-io
 Author: bioimage.io Team
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bioimage-io/spec-bioimage-io/issues
 Project-URL: Source, https://github.com/bioimage-io/spec-bioimage-io
 Platform: UNKNOWN
@@ -106,14 +106,18 @@
 
 Made with [contrib.rocks](https://contrib.rocks).
 
 ## Δ Changelog
 
 ### bioimageio.spec Python package
 
+#### bioimageio.spec 0.5.2post2
+
+* resolve version (un)specific collection IDs, e.g. `load_description('affable-shark')`, `load_description('affable-shark/1')`
+
 #### bioimageio.spec 0.5.2post1
 
 * fix model packaging with weights format priority
 
 #### bioimageio.spec 0.5.2
 
 * new patch version model 0.5.2
```

### Comparing `bioimageio.spec-0.5.2.post1/bioimageio.spec.egg-info/SOURCES.txt` & `bioimageio.spec-0.5.2.post2/bioimageio.spec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/example_descriptions/collections/unet2d_nuclei_broad_coll/unet2d.py` & `bioimageio.spec-0.5.2.post2/example_descriptions/collections/unet2d_nuclei_broad_coll/unet2d.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/example_descriptions/models/unet2d_diff_output_shape/resize_unet.py` & `bioimageio.spec-0.5.2.post2/example_descriptions/models/unet2d_diff_output_shape/resize_unet.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/example_descriptions/models/unet2d_fixed_shape/unet.py` & `bioimageio.spec-0.5.2.post2/example_descriptions/models/unet2d_fixed_shape/unet.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/example_descriptions/models/unet2d_multi_tensor/multi_tensor_unet.py` & `bioimageio.spec-0.5.2.post2/example_descriptions/models/unet2d_multi_tensor/multi_tensor_unet.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/example_descriptions/models/unet2d_nuclei_broad/unet2d.py` & `bioimageio.spec-0.5.2.post2/example_descriptions/models/unet2d_nuclei_broad/unet2d.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/example_descriptions/models/unet2d_nuclei_broad/unet2d_expand_output_shape.py` & `bioimageio.spec-0.5.2.post2/example_descriptions/models/unet2d_nuclei_broad/unet2d_expand_output_shape.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/pyproject.toml` & `bioimageio.spec-0.5.2.post2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/scripts/compare_yaml_syntax.py` & `bioimageio.spec-0.5.2.post2/scripts/compare_yaml_syntax.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/scripts/generate_json_schemas.py` & `bioimageio.spec-0.5.2.post2/scripts/generate_json_schemas.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/scripts/generate_spec_documentation.py` & `bioimageio.spec-0.5.2.post2/scripts/generate_spec_documentation.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/scripts/generate_version_submodule_imports.py` & `bioimageio.spec-0.5.2.post2/scripts/generate_version_submodule_imports.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/scripts/report_invalid_rdfs.py` & `bioimageio.spec-0.5.2.post2/scripts/report_invalid_rdfs.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/scripts/update_spdx_licenses.py` & `bioimageio.spec-0.5.2.post2/scripts/update_spdx_licenses.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/setup.py` & `bioimageio.spec-0.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         "numpy>=1.21",
         "packaging>=17.0",
         "pooch",
         "pydantic-settings",
         "pydantic>=2.6.3",
         "python-dateutil",
         "python-dotenv",
+        "requests",
         "rich",
         "ruyaml",
         "tqdm",
         "typing-extensions",
     ],
     extras_require={
         "dev": [
```

### Comparing `bioimageio.spec-0.5.2.post1/tests/test_bioimageio_collection.py` & `bioimageio.spec-0.5.2.post2/tests/test_bioimageio_collection.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/tests/test_description.py` & `bioimageio.spec-0.5.2.post2/tests/test_description.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/tests/test_example_specs.py` & `bioimageio.spec-0.5.2.post2/tests/test_example_specs.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/tests/test_generic/test_v0_2.py` & `bioimageio.spec-0.5.2.post2/tests/test_generic/test_v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/tests/test_generic/test_v0_3.py` & `bioimageio.spec-0.5.2.post2/tests/test_generic/test_v0_3.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/tests/test_internal/test_constants.py` & `bioimageio.spec-0.5.2.post2/tests/test_internal/test_constants.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/tests/test_internal/test_file_source.py` & `bioimageio.spec-0.5.2.post2/tests/test_internal/test_file_source.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/tests/test_internal/test_io.py` & `bioimageio.spec-0.5.2.post2/tests/test_internal/test_io.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/tests/test_internal/test_license_id.py` & `bioimageio.spec-0.5.2.post2/tests/test_internal/test_license_id.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/tests/test_internal/test_node.py` & `bioimageio.spec-0.5.2.post2/tests/test_internal/test_node.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/tests/test_internal/test_types.py` & `bioimageio.spec-0.5.2.post2/tests/test_internal/test_types.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/tests/test_internal/test_utils.py` & `bioimageio.spec-0.5.2.post2/tests/test_internal/test_utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/tests/test_internal/test_validate.py` & `bioimageio.spec-0.5.2.post2/tests/test_internal/test_validate.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/tests/test_internal/test_validated_string.py` & `bioimageio.spec-0.5.2.post2/tests/test_internal/test_validated_string.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/tests/test_model/test_v0_4.py` & `bioimageio.spec-0.5.2.post2/tests/test_model/test_v0_4.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/tests/test_model/test_v0_5.py` & `bioimageio.spec-0.5.2.post2/tests/test_model/test_v0_5.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/tests/test_package.py` & `bioimageio.spec-0.5.2.post2/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post1/tests/test_specific_reexports_generics.py` & `bioimageio.spec-0.5.2.post2/tests/test_specific_reexports_generics.py`

 * *Files identical despite different names*

