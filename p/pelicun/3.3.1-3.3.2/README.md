# Comparing `tmp/pelicun-3.3.1.tar.gz` & `tmp/pelicun-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelicun-3.3.1.tar", last modified: Wed Apr 17 00:41:14 2024, max compression
+gzip compressed data, was "pelicun-3.3.2.tar", last modified: Tue Apr 30 01:37:31 2024, max compression
```

## Comparing `pelicun-3.3.1.tar` & `pelicun-3.3.2.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.285605 pelicun-3.3.1/
--rw-r--r--   0 adamzs     (504) staff       (20)     1661 2022-12-05 20:30:08.000000 pelicun-3.3.1/LICENSE
--rw-r--r--   0 adamzs     (504) staff       (20)      486 2024-04-04 20:31:52.000000 pelicun-3.3.1/MANIFEST.in
--rw-r--r--   0 adamzs     (504) staff       (20)    21993 2024-04-17 00:41:14.285296 pelicun-3.3.1/PKG-INFO
--rw-r--r--   0 adamzs     (504) staff       (20)    20703 2024-04-04 20:38:24.000000 pelicun-3.3.1/README.md
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.229905 pelicun-3.3.1/pelicun/
--rw-r--r--   0 adamzs     (504) staff       (20)     2012 2024-04-17 00:38:15.000000 pelicun-3.3.1/pelicun/__init__.py
--rw-r--r--   0 adamzs     (504) staff       (20)     7284 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/assessment.py
--rw-r--r--   0 adamzs     (504) staff       (20)     3684 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/auto.py
--rw-r--r--   0 adamzs     (504) staff       (20)    38835 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/base.py
--rw-r--r--   0 adamzs     (504) staff       (20)   104242 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/db.py
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.222517 pelicun-3.3.1/pelicun/examples/
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.233106 pelicun-3.3.1/pelicun/examples/001/
--rw-r--r--   0 adamzs     (504) staff       (20)     5011 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/examples/001/CMP_QNT.csv
--rw-r--r--   0 adamzs     (504) staff       (20)    11827 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/examples/001/demands_s4.csv
--rw-r--r--   0 adamzs     (504) staff       (20)     2149 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/examples/001/input.json
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.234636 pelicun-3.3.1/pelicun/examples/002/
--rw-r--r--   0 adamzs     (504) staff       (20)      211 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/examples/002/CMP_QNT.csv
--rw-r--r--   0 adamzs     (504) staff       (20)      902 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/examples/002/input.json
--rw-r--r--   0 adamzs     (504) staff       (20)     4139 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/examples/002/response.csv
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.236681 pelicun-3.3.1/pelicun/examples/0_tmp/
--rw-r--r--   0 adamzs     (504) staff       (20)      652 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/examples/0_tmp/CMP_marginals.csv
--rw-r--r--   0 adamzs     (504) staff       (20)       52 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/examples/0_tmp/DMG_process_P58.json
--rw-r--r--   0 adamzs     (504) staff       (20)      347 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/examples/0_tmp/LOSS_map.csv
--rw-r--r--   0 adamzs     (504) staff       (20)     2782 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/examples/0_tmp/config.json
--rw-r--r--   0 adamzs     (504) staff       (20)     3892 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/examples/0_tmp/demands.csv
--rw-r--r--   0 adamzs     (504) staff       (20)      890 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/examples/0_tmp/fragility_Additional.csv
--rw-r--r--   0 adamzs     (504) staff       (20)      158 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/examples/0_tmp/repair_Additional.csv
--rw-r--r--   0 adamzs     (504) staff       (20)    16427 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/file_io.py
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.239279 pelicun-3.3.1/pelicun/model/
--rw-r--r--   0 adamzs     (504) staff       (20)     2010 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/model/__init__.py
--rw-r--r--   0 adamzs     (504) staff       (20)    15084 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/model/asset_model.py
--rw-r--r--   0 adamzs     (504) staff       (20)    60323 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/model/damage_model.py
--rw-r--r--   0 adamzs     (504) staff       (20)    33061 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/model/demand_model.py
--rw-r--r--   0 adamzs     (504) staff       (20)    40848 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/model/loss_model.py
--rw-r--r--   0 adamzs     (504) staff       (20)     8855 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/model/pelicun_model.py
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.222892 pelicun-3.3.1/pelicun/resources/
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.264690 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/
--rw-r--r--   0 adamzs     (504) staff       (20)    80663 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_FEMA_P58_2nd.csv
--rw-r--r--   0 adamzs     (504) staff       (20)  1167069 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_FEMA_P58_2nd.json
--rw-r--r--   0 adamzs     (504) staff       (20)    36386 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_bldg.csv
--rw-r--r--   0 adamzs     (504) staff       (20)   881431 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_bldg.json
--rw-r--r--   0 adamzs     (504) staff       (20)     9616 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_story.csv
--rw-r--r--   0 adamzs     (504) staff       (20)   183256 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_story.json
--rw-r--r--   0 adamzs     (504) staff       (20)     4297 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_trnsp.csv
--rw-r--r--   0 adamzs     (504) staff       (20)    52505 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_trnsp.json
--rw-r--r--   0 adamzs     (504) staff       (20)     2203 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_water.csv
--rw-r--r--   0 adamzs     (504) staff       (20)     3921 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_HU.csv
--rw-r--r--   0 adamzs     (504) staff       (20)    18199 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_HU.json
--rw-r--r--   0 adamzs     (504) staff       (20)  3714342 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_Hazus_HU_bldg.csv
--rw-r--r--   0 adamzs     (504) staff       (20)   521287 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_FEMA_P58_2nd.csv
--rw-r--r--   0 adamzs     (504) staff       (20)  1132502 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_FEMA_P58_2nd.json
--rw-r--r--   0 adamzs     (504) staff       (20)     8934 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_bldg.csv
--rw-r--r--   0 adamzs     (504) staff       (20)   262248 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_bldg.json
--rw-r--r--   0 adamzs     (504) staff       (20)     5912 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_story.csv
--rw-r--r--   0 adamzs     (504) staff       (20)   204054 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_story.json
--rw-r--r--   0 adamzs     (504) staff       (20)      302 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_trnsp.csv
--rw-r--r--   0 adamzs     (504) staff       (20)     3873 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_trnsp.json
--rw-r--r--   0 adamzs     (504) staff       (20)  2118028 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_SimCenter_Hazus_HU_bldg.csv
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.269271 pelicun-3.3.1/pelicun/resources/auto/
--rw-r--r--   0 adamzs     (504) staff       (20)    30421 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/auto/Hazus_Earthquake_IM.py
--rw-r--r--   0 adamzs     (504) staff       (20)     9084 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/auto/Hazus_Earthquake_Story.py
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.271753 pelicun-3.3.1/pelicun/settings/
--rw-r--r--   0 adamzs     (504) staff       (20)      661 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/settings/default_config.json
--rw-r--r--   0 adamzs     (504) staff       (20)     1610 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/settings/default_units.json
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.275332 pelicun-3.3.1/pelicun/tests/
--rw-r--r--   0 adamzs     (504) staff       (20)     3113 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/code_repetition_checker.py
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.223707 pelicun-3.3.1/pelicun/tests/data/
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.223307 pelicun-3.3.1/pelicun/tests/data/assessment/
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.275686 pelicun-3.3.1/pelicun/tests/data/assessment/test_assessment_calc_unit_scale_factor/
--rw-r--r--   0 adamzs     (504) staff       (20)       55 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/assessment/test_assessment_calc_unit_scale_factor/custom_units.json
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.223464 pelicun-3.3.1/pelicun/tests/data/base/
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.277291 pelicun-3.3.1/pelicun/tests/data/base/test_parse_units/
--rw-r--r--   0 adamzs     (504) staff       (20)       38 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/base/test_parse_units/additional_units_a.json
--rw-r--r--   0 adamzs     (504) staff       (20)     1547 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/base/test_parse_units/duplicate.json
--rw-r--r--   0 adamzs     (504) staff       (20)     1531 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/base/test_parse_units/duplicate2.json
--rw-r--r--   0 adamzs     (504) staff       (20)       43 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/base/test_parse_units/invalid.json
--rw-r--r--   0 adamzs     (504) staff       (20)       26 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/base/test_parse_units/not_dict.json
--rw-r--r--   0 adamzs     (504) staff       (20)       38 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/base/test_parse_units/not_float.json
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.223618 pelicun-3.3.1/pelicun/tests/data/file_io/
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.278427 pelicun-3.3.1/pelicun/tests/data/file_io/test_load_data/
--rw-r--r--   0 adamzs     (504) staff       (20)     1537 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/file_io/test_load_data/no_units.csv
--rwxr-xr-x   0 adamzs     (504) staff       (20)      372 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/file_io/test_load_data/orient_1.csv
--rwxr-xr-x   0 adamzs     (504) staff       (20)      445 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/file_io/test_load_data/orient_1_units.csv
--rw-r--r--   0 adamzs     (504) staff       (20)     1641 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/file_io/test_load_data/units.csv
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.224472 pelicun-3.3.1/pelicun/tests/data/model/
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.279481 pelicun-3.3.1/pelicun/tests/data/model/test_AssetModel/
--rwxr-xr-x   0 adamzs     (504) staff       (20)      108 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_AssetModel/CMP_marginals.csv
--rwxr-xr-x   0 adamzs     (504) staff       (20)      317 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_AssetModel/CMP_marginals_2.csv
--rwxr-xr-x   0 adamzs     (504) staff       (20)      125 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_AssetModel/CMP_marginals_block_weights.csv
--rwxr-xr-x   0 adamzs     (504) staff       (20)      116 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_AssetModel/CMP_marginals_invalid_dir.csv
--rwxr-xr-x   0 adamzs     (504) staff       (20)      111 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_AssetModel/CMP_marginals_invalid_loc.csv
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.279765 pelicun-3.3.1/pelicun/tests/data/model/test_DamageModel__evaluate_damage_state_and_prepare_dmg_quantities/
--rw-r--r--   0 adamzs     (504) staff       (20)      229 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_DamageModel__evaluate_damage_state_and_prepare_dmg_quantities/demand_sample.csv
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.280000 pelicun-3.3.1/pelicun/tests/data/model/test_DamageModel_assemble_required_demand_data/
--rw-r--r--   0 adamzs     (504) staff       (20)      208 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_DamageModel_assemble_required_demand_data/demand_sample.csv
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.280215 pelicun-3.3.1/pelicun/tests/data/model/test_DamageModel_calculate_multilinear_CDF/
--rw-r--r--   0 adamzs     (504) staff       (20)      237 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_DamageModel_calculate_multilinear_CDF/damage_model.csv
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.281085 pelicun-3.3.1/pelicun/tests/data/model/test_DamageModel_perform_dmg_task/
--rwxr-xr-x   0 adamzs     (504) staff       (20)       75 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_DamageModel_perform_dmg_task/CMP_marginals.csv
--rwxr-xr-x   0 adamzs     (504) staff       (20)      109 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_DamageModel_perform_dmg_task/CMP_marginals_2.csv
--rw-r--r--   0 adamzs     (504) staff       (20)      249 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_DamageModel_perform_dmg_task/fragility_DB_test.csv
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.281313 pelicun-3.3.1/pelicun/tests/data/model/test_DemandModel_estimate_RID/
--rw-r--r--   0 adamzs     (504) staff       (20)       51 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_DemandModel_estimate_RID/demand_sample_A.csv
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.281559 pelicun-3.3.1/pelicun/tests/data/model/test_DemandModel_generate_sample_with_demand_cloning/
--rw-r--r--   0 adamzs     (504) staff       (20)      138 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_DemandModel_generate_sample_with_demand_cloning/sample.csv
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.282509 pelicun-3.3.1/pelicun/tests/data/model/test_DemandModel_load_sample/
--rw-r--r--   0 adamzs     (504) staff       (20)      162 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_DemandModel_load_sample/demand_sample_A.csv
--rw-r--r--   0 adamzs     (504) staff       (20)      152 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_DemandModel_load_sample/demand_sample_B.csv
--rw-r--r--   0 adamzs     (504) staff       (20)      152 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_DemandModel_load_sample/demand_sample_C.csv
--rw-r--r--   0 adamzs     (504) staff       (20)      152 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_DemandModel_load_sample/demand_sample_D.csv
--rw-r--r--   0 adamzs     (504) staff       (20)     5729 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/reset_tests.py
--rw-r--r--   0 adamzs     (504) staff       (20)     5155 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/test_assessment.py
--rw-r--r--   0 adamzs     (504) staff       (20)     4416 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/test_auto.py
--rw-r--r--   0 adamzs     (504) staff       (20)    26202 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/test_base.py
--rw-r--r--   0 adamzs     (504) staff       (20)     7915 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/test_file_io.py
--rw-r--r--   0 adamzs     (504) staff       (20)    76806 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/test_model.py
--rw-r--r--   0 adamzs     (504) staff       (20)    46929 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/test_uq.py
--rw-r--r--   0 adamzs     (504) staff       (20)     3298 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/util.py
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.284158 pelicun-3.3.1/pelicun/tools/
--rw-r--r--   0 adamzs     (504) staff       (20)    70920 2024-04-10 18:14:45.000000 pelicun-3.3.1/pelicun/tools/DL_calculation.py
--rw-r--r--   0 adamzs     (504) staff       (20)     2411 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tools/HDF_to_CSV.py
--rw-r--r--   0 adamzs     (504) staff       (20)     3256 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tools/export_DB.py
--rw-r--r--   0 adamzs     (504) staff       (20)    75896 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/uq.py
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.284778 pelicun-3.3.1/pelicun.egg-info/
--rw-r--r--   0 adamzs     (504) staff       (20)    21993 2024-04-17 00:41:14.000000 pelicun-3.3.1/pelicun.egg-info/PKG-INFO
--rw-r--r--   0 adamzs     (504) staff       (20)     4829 2024-04-17 00:41:14.000000 pelicun-3.3.1/pelicun.egg-info/SOURCES.txt
--rw-r--r--   0 adamzs     (504) staff       (20)        1 2024-04-17 00:41:14.000000 pelicun-3.3.1/pelicun.egg-info/dependency_links.txt
--rw-r--r--   0 adamzs     (504) staff       (20)       62 2024-04-17 00:41:14.000000 pelicun-3.3.1/pelicun.egg-info/entry_points.txt
--rw-r--r--   0 adamzs     (504) staff       (20)       88 2024-04-17 00:41:14.000000 pelicun-3.3.1/pelicun.egg-info/requires.txt
--rw-r--r--   0 adamzs     (504) staff       (20)        8 2024-04-17 00:41:14.000000 pelicun-3.3.1/pelicun.egg-info/top_level.txt
--rw-r--r--   0 adamzs     (504) staff       (20)       38 2024-04-17 00:41:14.285674 pelicun-3.3.1/setup.cfg
--rw-r--r--   0 adamzs     (504) staff       (20)     2161 2024-04-04 20:31:52.000000 pelicun-3.3.1/setup.py
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.106868 pelicun-3.3.2/
+-rw-r--r--   0 adamzs     (504) staff       (20)     1661 2022-12-05 20:30:08.000000 pelicun-3.3.2/LICENSE
+-rw-r--r--   0 adamzs     (504) staff       (20)      486 2024-04-04 20:31:52.000000 pelicun-3.3.2/MANIFEST.in
+-rw-r--r--   0 adamzs     (504) staff       (20)    21964 2024-04-30 01:37:31.106529 pelicun-3.3.2/PKG-INFO
+-rw-r--r--   0 adamzs     (504) staff       (20)    20703 2024-04-04 20:38:24.000000 pelicun-3.3.2/README.md
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.053395 pelicun-3.3.2/pelicun/
+-rw-r--r--   0 adamzs     (504) staff       (20)     2012 2024-04-30 01:07:33.000000 pelicun-3.3.2/pelicun/__init__.py
+-rw-r--r--   0 adamzs     (504) staff       (20)     7284 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/assessment.py
+-rw-r--r--   0 adamzs     (504) staff       (20)     3684 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/auto.py
+-rw-r--r--   0 adamzs     (504) staff       (20)    38835 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/base.py
+-rw-r--r--   0 adamzs     (504) staff       (20)   104242 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/db.py
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.047481 pelicun-3.3.2/pelicun/examples/
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.055884 pelicun-3.3.2/pelicun/examples/001/
+-rw-r--r--   0 adamzs     (504) staff       (20)     5011 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/examples/001/CMP_QNT.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)    11827 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/examples/001/demands_s4.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)     2149 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/examples/001/input.json
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.057178 pelicun-3.3.2/pelicun/examples/002/
+-rw-r--r--   0 adamzs     (504) staff       (20)      211 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/examples/002/CMP_QNT.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)      902 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/examples/002/input.json
+-rw-r--r--   0 adamzs     (504) staff       (20)     4139 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/examples/002/response.csv
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.059019 pelicun-3.3.2/pelicun/examples/0_tmp/
+-rw-r--r--   0 adamzs     (504) staff       (20)      652 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/examples/0_tmp/CMP_marginals.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)       52 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/examples/0_tmp/DMG_process_P58.json
+-rw-r--r--   0 adamzs     (504) staff       (20)      347 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/examples/0_tmp/LOSS_map.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)     2782 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/examples/0_tmp/config.json
+-rw-r--r--   0 adamzs     (504) staff       (20)     3892 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/examples/0_tmp/demands.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)      890 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/examples/0_tmp/fragility_Additional.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)      158 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/examples/0_tmp/repair_Additional.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)    16427 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/file_io.py
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.061578 pelicun-3.3.2/pelicun/model/
+-rw-r--r--   0 adamzs     (504) staff       (20)     2010 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/model/__init__.py
+-rw-r--r--   0 adamzs     (504) staff       (20)    15084 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/model/asset_model.py
+-rw-r--r--   0 adamzs     (504) staff       (20)    60323 2024-04-30 01:02:56.000000 pelicun-3.3.2/pelicun/model/damage_model.py
+-rw-r--r--   0 adamzs     (504) staff       (20)    33061 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/model/demand_model.py
+-rw-r--r--   0 adamzs     (504) staff       (20)    40848 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/model/loss_model.py
+-rw-r--r--   0 adamzs     (504) staff       (20)     8855 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/model/pelicun_model.py
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.048043 pelicun-3.3.2/pelicun/resources/
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.084927 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/
+-rw-r--r--   0 adamzs     (504) staff       (20)    80663 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_FEMA_P58_2nd.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)  1167069 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_FEMA_P58_2nd.json
+-rw-r--r--   0 adamzs     (504) staff       (20)    36386 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_bldg.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)   881431 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_bldg.json
+-rw-r--r--   0 adamzs     (504) staff       (20)     9616 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_story.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)   183256 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_story.json
+-rw-r--r--   0 adamzs     (504) staff       (20)     4297 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_trnsp.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)    52505 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_trnsp.json
+-rw-r--r--   0 adamzs     (504) staff       (20)     2203 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_water.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)     3921 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_HU.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)    18199 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_HU.json
+-rw-r--r--   0 adamzs     (504) staff       (20)  3714342 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_Hazus_HU_bldg.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)   521287 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_FEMA_P58_2nd.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)  1132502 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_FEMA_P58_2nd.json
+-rw-r--r--   0 adamzs     (504) staff       (20)     8934 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_bldg.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)   262248 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_bldg.json
+-rw-r--r--   0 adamzs     (504) staff       (20)     5912 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_story.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)   204054 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_story.json
+-rw-r--r--   0 adamzs     (504) staff       (20)      302 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_trnsp.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)     3873 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_trnsp.json
+-rw-r--r--   0 adamzs     (504) staff       (20)  2118028 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_SimCenter_Hazus_HU_bldg.csv
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.089131 pelicun-3.3.2/pelicun/resources/auto/
+-rw-r--r--   0 adamzs     (504) staff       (20)    31025 2024-04-30 01:01:03.000000 pelicun-3.3.2/pelicun/resources/auto/Hazus_Earthquake_IM.py
+-rw-r--r--   0 adamzs     (504) staff       (20)     9220 2024-04-30 01:01:14.000000 pelicun-3.3.2/pelicun/resources/auto/Hazus_Earthquake_Story.py
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.091216 pelicun-3.3.2/pelicun/settings/
+-rw-r--r--   0 adamzs     (504) staff       (20)      661 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/settings/default_config.json
+-rw-r--r--   0 adamzs     (504) staff       (20)     1610 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/settings/default_units.json
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.094348 pelicun-3.3.2/pelicun/tests/
+-rw-r--r--   0 adamzs     (504) staff       (20)     3113 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/code_repetition_checker.py
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.049053 pelicun-3.3.2/pelicun/tests/data/
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.048627 pelicun-3.3.2/pelicun/tests/data/assessment/
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.094674 pelicun-3.3.2/pelicun/tests/data/assessment/test_assessment_calc_unit_scale_factor/
+-rw-r--r--   0 adamzs     (504) staff       (20)       55 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/assessment/test_assessment_calc_unit_scale_factor/custom_units.json
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.048801 pelicun-3.3.2/pelicun/tests/data/base/
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.098077 pelicun-3.3.2/pelicun/tests/data/base/test_parse_units/
+-rw-r--r--   0 adamzs     (504) staff       (20)       38 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/base/test_parse_units/additional_units_a.json
+-rw-r--r--   0 adamzs     (504) staff       (20)     1547 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/base/test_parse_units/duplicate.json
+-rw-r--r--   0 adamzs     (504) staff       (20)     1531 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/base/test_parse_units/duplicate2.json
+-rw-r--r--   0 adamzs     (504) staff       (20)       43 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/base/test_parse_units/invalid.json
+-rw-r--r--   0 adamzs     (504) staff       (20)       26 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/base/test_parse_units/not_dict.json
+-rw-r--r--   0 adamzs     (504) staff       (20)       38 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/base/test_parse_units/not_float.json
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.048968 pelicun-3.3.2/pelicun/tests/data/file_io/
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.099417 pelicun-3.3.2/pelicun/tests/data/file_io/test_load_data/
+-rw-r--r--   0 adamzs     (504) staff       (20)     1537 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/file_io/test_load_data/no_units.csv
+-rwxr-xr-x   0 adamzs     (504) staff       (20)      372 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/file_io/test_load_data/orient_1.csv
+-rwxr-xr-x   0 adamzs     (504) staff       (20)      445 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/file_io/test_load_data/orient_1_units.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)     1641 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/file_io/test_load_data/units.csv
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.049966 pelicun-3.3.2/pelicun/tests/data/model/
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.100894 pelicun-3.3.2/pelicun/tests/data/model/test_AssetModel/
+-rwxr-xr-x   0 adamzs     (504) staff       (20)      108 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_AssetModel/CMP_marginals.csv
+-rwxr-xr-x   0 adamzs     (504) staff       (20)      317 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_AssetModel/CMP_marginals_2.csv
+-rwxr-xr-x   0 adamzs     (504) staff       (20)      125 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_AssetModel/CMP_marginals_block_weights.csv
+-rwxr-xr-x   0 adamzs     (504) staff       (20)      116 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_AssetModel/CMP_marginals_invalid_dir.csv
+-rwxr-xr-x   0 adamzs     (504) staff       (20)      111 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_AssetModel/CMP_marginals_invalid_loc.csv
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.101129 pelicun-3.3.2/pelicun/tests/data/model/test_DamageModel__evaluate_damage_state_and_prepare_dmg_quantities/
+-rw-r--r--   0 adamzs     (504) staff       (20)      229 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_DamageModel__evaluate_damage_state_and_prepare_dmg_quantities/demand_sample.csv
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.101616 pelicun-3.3.2/pelicun/tests/data/model/test_DamageModel_assemble_required_demand_data/
+-rw-r--r--   0 adamzs     (504) staff       (20)      208 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_DamageModel_assemble_required_demand_data/demand_sample.csv
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.102032 pelicun-3.3.2/pelicun/tests/data/model/test_DamageModel_calculate_multilinear_CDF/
+-rw-r--r--   0 adamzs     (504) staff       (20)      237 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_DamageModel_calculate_multilinear_CDF/damage_model.csv
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.102746 pelicun-3.3.2/pelicun/tests/data/model/test_DamageModel_perform_dmg_task/
+-rwxr-xr-x   0 adamzs     (504) staff       (20)       75 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_DamageModel_perform_dmg_task/CMP_marginals.csv
+-rwxr-xr-x   0 adamzs     (504) staff       (20)      109 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_DamageModel_perform_dmg_task/CMP_marginals_2.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)      249 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_DamageModel_perform_dmg_task/fragility_DB_test.csv
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.102975 pelicun-3.3.2/pelicun/tests/data/model/test_DemandModel_estimate_RID/
+-rw-r--r--   0 adamzs     (504) staff       (20)       51 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_DemandModel_estimate_RID/demand_sample_A.csv
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.103185 pelicun-3.3.2/pelicun/tests/data/model/test_DemandModel_generate_sample_with_demand_cloning/
+-rw-r--r--   0 adamzs     (504) staff       (20)      138 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_DemandModel_generate_sample_with_demand_cloning/sample.csv
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.104055 pelicun-3.3.2/pelicun/tests/data/model/test_DemandModel_load_sample/
+-rw-r--r--   0 adamzs     (504) staff       (20)      162 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_DemandModel_load_sample/demand_sample_A.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)      152 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_DemandModel_load_sample/demand_sample_B.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)      152 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_DemandModel_load_sample/demand_sample_C.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)      152 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/data/model/test_DemandModel_load_sample/demand_sample_D.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)     5729 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/reset_tests.py
+-rw-r--r--   0 adamzs     (504) staff       (20)     5155 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/test_assessment.py
+-rw-r--r--   0 adamzs     (504) staff       (20)     4416 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/test_auto.py
+-rw-r--r--   0 adamzs     (504) staff       (20)    26202 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/test_base.py
+-rw-r--r--   0 adamzs     (504) staff       (20)     7915 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/test_file_io.py
+-rw-r--r--   0 adamzs     (504) staff       (20)    76806 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/test_model.py
+-rw-r--r--   0 adamzs     (504) staff       (20)    46929 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/test_uq.py
+-rw-r--r--   0 adamzs     (504) staff       (20)     3298 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tests/util.py
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.105387 pelicun-3.3.2/pelicun/tools/
+-rw-r--r--   0 adamzs     (504) staff       (20)    70920 2024-04-30 01:07:19.000000 pelicun-3.3.2/pelicun/tools/DL_calculation.py
+-rw-r--r--   0 adamzs     (504) staff       (20)     2411 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tools/HDF_to_CSV.py
+-rw-r--r--   0 adamzs     (504) staff       (20)     3256 2024-04-04 20:31:52.000000 pelicun-3.3.2/pelicun/tools/export_DB.py
+-rw-r--r--   0 adamzs     (504) staff       (20)    76038 2024-04-30 01:15:29.000000 pelicun-3.3.2/pelicun/uq.py
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-30 01:37:31.105849 pelicun-3.3.2/pelicun.egg-info/
+-rw-r--r--   0 adamzs     (504) staff       (20)    21964 2024-04-30 01:37:31.000000 pelicun-3.3.2/pelicun.egg-info/PKG-INFO
+-rw-r--r--   0 adamzs     (504) staff       (20)     4829 2024-04-30 01:37:31.000000 pelicun-3.3.2/pelicun.egg-info/SOURCES.txt
+-rw-r--r--   0 adamzs     (504) staff       (20)        1 2024-04-30 01:37:31.000000 pelicun-3.3.2/pelicun.egg-info/dependency_links.txt
+-rw-r--r--   0 adamzs     (504) staff       (20)       62 2024-04-30 01:37:31.000000 pelicun-3.3.2/pelicun.egg-info/entry_points.txt
+-rw-r--r--   0 adamzs     (504) staff       (20)       74 2024-04-30 01:37:31.000000 pelicun-3.3.2/pelicun.egg-info/requires.txt
+-rw-r--r--   0 adamzs     (504) staff       (20)        8 2024-04-30 01:37:31.000000 pelicun-3.3.2/pelicun.egg-info/top_level.txt
+-rw-r--r--   0 adamzs     (504) staff       (20)       38 2024-04-30 01:37:31.106938 pelicun-3.3.2/setup.cfg
+-rw-r--r--   0 adamzs     (504) staff       (20)     2162 2024-04-30 01:27:58.000000 pelicun-3.3.2/setup.py
```

### Comparing `pelicun-3.3.1/LICENSE` & `pelicun-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/PKG-INFO` & `pelicun-3.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pelicun
-Version: 3.3.1
+Version: 3.3.2
 Summary: Probabilistic Estimation of Losses, Injuries, and Community resilience Under Natural hazard events
 Home-page: http://nheri-simcenter.github.io/pelicun/
 Author: Adam Zsarnóczay
 Author-email: adamzs@stanford.edu
 License: BSD License
 Platform: any
 Classifier: Programming Language :: Python
@@ -24,15 +24,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy<2.0,>=1.22.0
 Requires-Dist: scipy<2.0,>=1.7.0
 Requires-Dist: pandas<3.0,>=1.4.0
-Requires-Dist: tables>=3.7.0
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 
 <p align="center">
 	<img src="https://raw.githubusercontent.com/NHERI-SimCenter/pelicun/gh-pages/doc_src/common/figures/pelicun-Logo-white.png"
 		alt="pelicun" align="middle" height="200"/>
 </p>
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: pelicun Version: 3.3.1 Summary: Probabilistic
+Metadata-Version: 2.1 Name: pelicun Version: 3.3.2 Summary: Probabilistic
 Estimation of Losses, Injuries, and Community resilience Under Natural hazard
 events Home-page: http://nheri-simcenter.github.io/pelicun/ Author: Adam
 ZsarnÃ³czay Author-email: adamzs@stanford.edu License: BSD License Platform:
 any Classifier: Programming Language :: Python Classifier: Development Status
 :: 5 - Production/Stable Classifier: Natural Language :: English Classifier:
 Environment :: Console Classifier: Framework :: Jupyter Classifier: Intended
 Audience :: Education Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License Classifier: Natural Language
 :: English Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: numpy<2.0,>=1.22.0 Requires-Dist:
-scipy<2.0,>=1.7.0 Requires-Dist: pandas<3.0,>=1.4.0 Requires-Dist:
-tables>=3.7.0 Provides-Extra: testing Requires-Dist: pytest; extra == "testing"
+scipy<2.0,>=1.7.0 Requires-Dist: pandas<3.0,>=1.4.0 Provides-Extra: testing
+Requires-Dist: pytest; extra == "testing"
                                    [pelicun]
       alt="DOI">[https://zenodo.org/badge/DOI/10.5281/zenodo.2558558.svg]
  PPrroobbaabbiilliissttiicc EEssttiimmaattiioonn ooff LLoosssseess,, IInnjjuurriieess,, aanndd CCoommmmuunniittyy rreessiilliieennccee UUnnddeerr
                              NNaattuurraall hhaazzaarrdd eevveennttss
 ![Tests](https://github.com/NHERI-SimCenter/pelicun/actions/workflows/
 tests.yml/badge.svg) [![codecov](https://codecov.io/github/NHERI-SimCenter/
 pelicun/branch/master/graph/badge.svg?token=W79M5FGOCG)](https://codecov.io/
```

### Comparing `pelicun-3.3.1/README.md` & `pelicun-3.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/__init__.py` & `pelicun-3.3.2/pelicun/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,14 @@
 
 Contributors:
 Adam Zsarnóczay
 """
 
 name = "pelicun"
 
-__version__ = '3.3.1'
+__version__ = '3.3.2'
 
 __copyright__ = ("Copyright (c) 2018 Leland Stanford "
                  "Junior University and The Regents "
                  "of the University of California")
 
 __license__ = "BSD 3-Clause License"
```

### Comparing `pelicun-3.3.1/pelicun/assessment.py` & `pelicun-3.3.2/pelicun/assessment.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/auto.py` & `pelicun-3.3.2/pelicun/auto.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/base.py` & `pelicun-3.3.2/pelicun/base.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/db.py` & `pelicun-3.3.2/pelicun/db.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/examples/001/CMP_QNT.csv` & `pelicun-3.3.2/pelicun/examples/001/CMP_QNT.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/examples/001/demands_s4.csv` & `pelicun-3.3.2/pelicun/examples/001/demands_s4.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/examples/001/input.json` & `pelicun-3.3.2/pelicun/examples/001/input.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/examples/002/input.json` & `pelicun-3.3.2/pelicun/examples/002/input.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/examples/002/response.csv` & `pelicun-3.3.2/pelicun/examples/002/response.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/examples/0_tmp/CMP_marginals.csv` & `pelicun-3.3.2/pelicun/examples/0_tmp/CMP_marginals.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/examples/0_tmp/config.json` & `pelicun-3.3.2/pelicun/examples/0_tmp/config.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/examples/0_tmp/demands.csv` & `pelicun-3.3.2/pelicun/examples/0_tmp/demands.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/examples/0_tmp/fragility_Additional.csv` & `pelicun-3.3.2/pelicun/examples/0_tmp/fragility_Additional.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/file_io.py` & `pelicun-3.3.2/pelicun/file_io.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/model/__init__.py` & `pelicun-3.3.2/pelicun/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/model/asset_model.py` & `pelicun-3.3.2/pelicun/model/asset_model.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/model/damage_model.py` & `pelicun-3.3.2/pelicun/model/damage_model.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/model/demand_model.py` & `pelicun-3.3.2/pelicun/model/demand_model.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/model/loss_model.py` & `pelicun-3.3.2/pelicun/model/loss_model.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/model/pelicun_model.py` & `pelicun-3.3.2/pelicun/model/pelicun_model.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_FEMA_P58_2nd.csv` & `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_FEMA_P58_2nd.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_FEMA_P58_2nd.json` & `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_FEMA_P58_2nd.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_bldg.csv` & `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_bldg.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_bldg.json` & `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_bldg.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_story.csv` & `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_story.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_story.json` & `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_story.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_trnsp.csv` & `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_trnsp.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_trnsp.json` & `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_trnsp.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_water.csv` & `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_water.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_HU.csv` & `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_HU.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_HU.json` & `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_HU.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_Hazus_HU_bldg.csv` & `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_Hazus_HU_bldg.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_FEMA_P58_2nd.csv` & `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_FEMA_P58_2nd.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_FEMA_P58_2nd.json` & `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_FEMA_P58_2nd.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_bldg.csv` & `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_bldg.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_bldg.json` & `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_bldg.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_story.csv` & `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_story.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_story.json` & `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_story.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_trnsp.json` & `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_trnsp.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_SimCenter_Hazus_HU_bldg.csv` & `pelicun-3.3.2/pelicun/resources/SimCenterDBDL/loss_repair_DB_SimCenter_Hazus_HU_bldg.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/resources/auto/Hazus_Earthquake_IM.py` & `pelicun-3.3.2/pelicun/resources/auto/Hazus_Earthquake_IM.py`

 * *Files 2% similar despite different names*

```diff
@@ -404,14 +404,19 @@
             "Demands": {},
             "Losses": {
                 "Repair": {
                     "ConsequenceDatabase": "Hazus Earthquake - Buildings",
                     "MapApproach": "Automatic",
                 }
             },
+            "Options": {
+                "NonDirectionalMultipliers": {
+                    "ALL": 1.0
+                },
+            }
         }
 
     elif assetType == "TransportationNetwork":
         inf_type = GI["assetSubtype"]
 
         if inf_type == "HwyBridge":
             # get the bridge class
@@ -437,14 +442,19 @@
                 "Demands": {},
                 "Losses": {
                     "Repair": {
                         "ConsequenceDatabase": "Hazus Earthquake - Transportation",
                         "MapApproach": "Automatic",
                     }
                 },
+                "Options": {
+                    "NonDirectionalMultipliers": {
+                        "ALL": 1.0
+                    },
+                }
             }
 
         elif inf_type == "HwyTunnel":
             # get the tunnel class
             tt = convertTunnelToHAZUSclass(GI)
             GI_ap['TunnelHazusClass'] = tt
 
@@ -467,14 +477,19 @@
                 "Demands": {},
                 "Losses": {
                     "Repair": {
                         "ConsequenceDatabase": "Hazus Earthquake - Transportation",
                         "MapApproach": "Automatic",
                     }
                 },
+                "Options": {
+                    "NonDirectionalMultipliers": {
+                        "ALL": 1.0
+                    },
+                }
             }
         elif inf_type == "Roadway":
             # get the road class
             rt = convertRoadToHAZUSclass(GI)
             GI_ap['RoadHazusClass'] = rt
 
             # fmt: off
@@ -495,14 +510,19 @@
                 "Demands": {},
                 "Losses": {
                     "Repair": {
                         "ConsequenceDatabase": "Hazus Earthquake - Transportation",
                         "MapApproach": "Automatic",
                     }
                 },
+                "Options": {
+                    "NonDirectionalMultipliers": {
+                        "ALL": 1.0
+                    },
+                }
             }
         else:
             print("subtype not supported in HWY")
 
     elif assetType == "WaterDistributionNetwork":
 
         pipe_material_map = {
```

### Comparing `pelicun-3.3.1/pelicun/resources/auto/Hazus_Earthquake_Story.py` & `pelicun-3.3.2/pelicun/resources/auto/Hazus_Earthquake_Story.py`

 * *Files 4% similar despite different names*

```diff
@@ -260,14 +260,19 @@
                 "NumberOfStories": f"{stories}",
                 "OccupancyType": f"{ot}",
                 "PlanArea": str(plan_area),
             },
             "Damage": {"DamageProcess": "Hazus Earthquake"},
             "Demands": {},
             "Losses": {"Repair": repair_config},
+            "Options": {
+                "NonDirectionalMultipliers": {
+                    "ALL": 1.0
+                },
+            }
         }
 
     else:
         print(
             f"AssetType: {assetType} is not supported "
             f"in Hazus Earthquake Story-based DL method"
         )
```

### Comparing `pelicun-3.3.1/pelicun/settings/default_config.json` & `pelicun-3.3.2/pelicun/settings/default_config.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/settings/default_units.json` & `pelicun-3.3.2/pelicun/settings/default_units.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/tests/code_repetition_checker.py` & `pelicun-3.3.2/pelicun/tests/code_repetition_checker.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/tests/data/base/test_parse_units/duplicate.json` & `pelicun-3.3.2/pelicun/tests/data/base/test_parse_units/duplicate.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/tests/data/base/test_parse_units/duplicate2.json` & `pelicun-3.3.2/pelicun/tests/data/base/test_parse_units/duplicate2.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/tests/data/file_io/test_load_data/no_units.csv` & `pelicun-3.3.2/pelicun/tests/data/file_io/test_load_data/no_units.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/tests/data/file_io/test_load_data/units.csv` & `pelicun-3.3.2/pelicun/tests/data/file_io/test_load_data/units.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/tests/reset_tests.py` & `pelicun-3.3.2/pelicun/tests/reset_tests.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/tests/test_assessment.py` & `pelicun-3.3.2/pelicun/tests/test_assessment.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/tests/test_auto.py` & `pelicun-3.3.2/pelicun/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/tests/test_base.py` & `pelicun-3.3.2/pelicun/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/tests/test_file_io.py` & `pelicun-3.3.2/pelicun/tests/test_file_io.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/tests/test_model.py` & `pelicun-3.3.2/pelicun/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/tests/test_uq.py` & `pelicun-3.3.2/pelicun/tests/test_uq.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/tests/util.py` & `pelicun-3.3.2/pelicun/tests/util.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/tools/DL_calculation.py` & `pelicun-3.3.2/pelicun/tools/DL_calculation.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/tools/HDF_to_CSV.py` & `pelicun-3.3.2/pelicun/tools/HDF_to_CSV.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/tools/export_DB.py` & `pelicun-3.3.2/pelicun/tools/export_DB.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/pelicun/uq.py` & `pelicun-3.3.2/pelicun/uq.py`

 * *Files 2% similar despite different names*

```diff
@@ -1241,17 +1241,17 @@
             Anchors this to another variable. If the anchor is not None, this
             variable will be perfectly correlated with its anchor. Note that
             the attributes of this variable and its anchor do not have to be
             identical.
 
         """
         super().__init__(
-            name,
-            f_map,
-            anchor,
+            name=name,
+            f_map=f_map,
+            anchor=anchor,
         )
 
     @abstractmethod
     def inverse_transform(self, values):
         """
         Uses inverse probability integral transformation on the
         provided values.
@@ -1277,49 +1277,39 @@
     """
     Random variable that needs `sample_size` in `inverse_transform`
     """
 
     @abstractmethod
     def __init__(
         self,
-        name,
-        theta,
-        truncation_limits=np.array((np.nan, np.nan)),
+        name,        
         f_map=None,
         anchor=None,
     ):
         """
         Instantiates a normal random variable.
 
         Parameters
         ----------
         name: string
-            A unique string that identifies the random variable.
-        theta: 2-element float ndarray
-          Set of parameters that define the Cumulative Distribution
-          Function (CDF) of the variable: Mean, coefficient of
-          variation.
-        truncation_limits: float ndarray, optional
-          Defines the np.array((a, b)) truncation limits for the
-          distribution. Use np.nan to assign no limit in one direction,
-          like so: np.array((a, np.nan)), or np.array((np.nan, b)).
+            A unique string that identifies the random variable.        
         f_map: function, optional
             A user-defined function that is applied on the realizations before
             returning a sample.
         anchor: RandomVariable, optional
             Anchors this to another variable. If the anchor is not None, this
             variable will be perfectly correlated with its anchor. Note that
             the attributes of this variable and its anchor do not have to be
             identical.
 
         """
         super().__init__(
-            name,
-            f_map,
-            anchor,
+            name=name,
+            f_map=f_map,
+            anchor=anchor,
         )
 
     @abstractmethod
     def inverse_transform(self, sample_size):
         """
         Uses inverse probability integral transformation on the
         provided values.
@@ -1345,17 +1335,19 @@
         name,
         theta,
         truncation_limits=np.array((np.nan, np.nan)),
         f_map=None,
         anchor=None,
     ):
         super().__init__(
-            name,
-            f_map,
-            anchor,
+            name=name,
+            theta=theta,
+            truncation_limits=truncation_limits,
+            f_map=f_map,
+            anchor=anchor,
         )
         self.distribution = 'normal'
         self.theta = np.atleast_1d(theta)
         self.truncation_limits = truncation_limits
 
     def cdf(self, values):
         """
@@ -1465,17 +1457,19 @@
         name,
         theta,
         truncation_limits=np.array((np.nan, np.nan)),
         f_map=None,
         anchor=None,
     ):
         super().__init__(
-            name,
-            f_map,
-            anchor,
+            name=name,
+            theta=theta,
+            truncation_limits=truncation_limits,
+            f_map=f_map,
+            anchor=anchor,
         )
         self.distribution = 'lognormal'
         self.theta = np.atleast_1d(theta)
         self.truncation_limits = truncation_limits
 
     def cdf(self, values):
         """
@@ -1579,17 +1573,19 @@
         name,
         theta,
         truncation_limits=np.array((np.nan, np.nan)),
         f_map=None,
         anchor=None,
     ):
         super().__init__(
-            name,
-            f_map,
-            anchor,
+            name=name,
+            theta=theta,
+            truncation_limits=truncation_limits,
+            f_map=f_map,
+            anchor=anchor,
         )
         self.distribution = 'uniform'
         self.theta = np.atleast_1d(theta)
         self.truncation_limits = truncation_limits
 
     def cdf(self, values):
         """
@@ -1666,17 +1662,19 @@
         name,
         theta,
         truncation_limits=np.array((np.nan, np.nan)),
         f_map=None,
         anchor=None,
     ):
         super().__init__(
-            name,
-            f_map,
-            anchor,
+            name=name,
+            theta=theta,
+            truncation_limits=truncation_limits,
+            f_map=f_map,
+            anchor=anchor,
         )
         self.distribution = 'multilinear_CDF'
 
         if not np.all(np.isnan(truncation_limits)):
             raise NotImplementedError(
                 f'{self.distribution} RVs do not support truncation'
             )
@@ -1787,17 +1785,19 @@
         name,
         raw_samples,
         truncation_limits=np.array((np.nan, np.nan)),
         f_map=None,
         anchor=None,
     ):
         super().__init__(
-            name,
-            f_map,
-            anchor,
+            name=name, 
+            theta=raw_samples,
+            truncation_limits=truncation_limits,           
+            f_map=f_map,
+            anchor=anchor,
         )
         self.distribution = 'empirical'
         if not np.all(np.isnan(truncation_limits)):
             raise NotImplementedError(
                 f'{self.distribution} RVs do not support truncation'
             )
 
@@ -1867,17 +1867,17 @@
         Raises
         ------
         NotImplementedError
           When truncation limits are provided
 
         """
         super().__init__(
-            name,
-            f_map,
-            anchor,
+            name=name,
+            f_map=f_map,
+            anchor=anchor,
         )
         self.distribution = 'coupled_empirical'
         if not np.all(np.isnan(truncation_limits)):
             raise NotImplementedError(
                 f'{self.distribution} RVs do not support truncation'
             )
 
@@ -1953,17 +1953,17 @@
         Raises
         ------
         NotImplementedError
           When truncation limits are provided
 
         """
         super().__init__(
-            name,
-            f_map,
-            anchor,
+            name=name,
+            f_map=f_map,
+            anchor=anchor,
         )
         self.distribution = 'deterministic'
         if not np.all(np.isnan(truncation_limits)):
             raise NotImplementedError(
                 f'{self.distribution} RVs do not support truncation'
             )
 
@@ -2000,17 +2000,19 @@
         name,
         theta,
         truncation_limits=np.array((np.nan, np.nan)),
         f_map=None,
         anchor=None,
     ):
         super().__init__(
-            name,
-            f_map,
-            anchor,
+            name=name,
+            theta=theta,
+            truncation_limits=truncation_limits,
+            f_map=f_map,
+            anchor=anchor,
         )
         if not np.all(np.isnan(truncation_limits)):
             raise NotImplementedError(
                 f'{self.distribution} RVs do not support truncation'
             )
         self.distribution = 'multinomial'
         if np.sum(theta) > 1.00:
```

### Comparing `pelicun-3.3.1/pelicun.egg-info/PKG-INFO` & `pelicun-3.3.2/pelicun.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pelicun
-Version: 3.3.1
+Version: 3.3.2
 Summary: Probabilistic Estimation of Losses, Injuries, and Community resilience Under Natural hazard events
 Home-page: http://nheri-simcenter.github.io/pelicun/
 Author: Adam Zsarnóczay
 Author-email: adamzs@stanford.edu
 License: BSD License
 Platform: any
 Classifier: Programming Language :: Python
@@ -24,15 +24,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy<2.0,>=1.22.0
 Requires-Dist: scipy<2.0,>=1.7.0
 Requires-Dist: pandas<3.0,>=1.4.0
-Requires-Dist: tables>=3.7.0
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 
 <p align="center">
 	<img src="https://raw.githubusercontent.com/NHERI-SimCenter/pelicun/gh-pages/doc_src/common/figures/pelicun-Logo-white.png"
 		alt="pelicun" align="middle" height="200"/>
 </p>
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: pelicun Version: 3.3.1 Summary: Probabilistic
+Metadata-Version: 2.1 Name: pelicun Version: 3.3.2 Summary: Probabilistic
 Estimation of Losses, Injuries, and Community resilience Under Natural hazard
 events Home-page: http://nheri-simcenter.github.io/pelicun/ Author: Adam
 ZsarnÃ³czay Author-email: adamzs@stanford.edu License: BSD License Platform:
 any Classifier: Programming Language :: Python Classifier: Development Status
 :: 5 - Production/Stable Classifier: Natural Language :: English Classifier:
 Environment :: Console Classifier: Framework :: Jupyter Classifier: Intended
 Audience :: Education Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License Classifier: Natural Language
 :: English Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: numpy<2.0,>=1.22.0 Requires-Dist:
-scipy<2.0,>=1.7.0 Requires-Dist: pandas<3.0,>=1.4.0 Requires-Dist:
-tables>=3.7.0 Provides-Extra: testing Requires-Dist: pytest; extra == "testing"
+scipy<2.0,>=1.7.0 Requires-Dist: pandas<3.0,>=1.4.0 Provides-Extra: testing
+Requires-Dist: pytest; extra == "testing"
                                    [pelicun]
       alt="DOI">[https://zenodo.org/badge/DOI/10.5281/zenodo.2558558.svg]
  PPrroobbaabbiilliissttiicc EEssttiimmaattiioonn ooff LLoosssseess,, IInnjjuurriieess,, aanndd CCoommmmuunniittyy rreessiilliieennccee UUnnddeerr
                              NNaattuurraall hhaazzaarrdd eevveennttss
 ![Tests](https://github.com/NHERI-SimCenter/pelicun/actions/workflows/
 tests.yml/badge.svg) [![codecov](https://codecov.io/github/NHERI-SimCenter/
 pelicun/branch/master/graph/badge.svg?token=W79M5FGOCG)](https://codecov.io/
```

### Comparing `pelicun-3.3.1/pelicun.egg-info/SOURCES.txt` & `pelicun-3.3.2/pelicun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pelicun-3.3.1/setup.py` & `pelicun-3.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     packages=find_packages(),
     include_package_data=True,
     platforms='any',
     install_requires=[
         'numpy>=1.22.0, <2.0',
         'scipy>=1.7.0, <2.0',
         'pandas>=1.4.0, <3.0',
-        'tables>=3.7.0',
+        #'tables>=3.7.0',
     ],
     classifiers=[
         'Programming Language :: Python',
         'Development Status :: 5 - Production/Stable',
         'Natural Language :: English',
         'Environment :: Console',
         'Framework :: Jupyter',
```

