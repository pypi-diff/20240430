# Comparing `tmp/dkist-processing-common-6.2.0rc1.tar.gz` & `tmp/dkist-processing-common-6.2.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-common-6.2.0rc1.tar", last modified: Thu Apr 25 21:54:19 2024, max compression
+gzip compressed data, was "dkist-processing-common-6.2.1rc2.tar", last modified: Tue Apr 30 16:44:53 2024, max compression
```

## Comparing `dkist-processing-common-6.2.0rc1.tar` & `dkist-processing-common-6.2.1rc2.tar`

### file list

```diff
@@ -1,139 +1,138 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-25 21:54:19.727801 dkist-processing-common-6.2.0rc1/
--rw-rw-rw-   0 root         (0) root         (0)     2481 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      844 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      429 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    24493 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     4394 2024-04-25 21:54:19.727801 dkist-processing-common-6.2.0rc1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3730 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     3271 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-25 21:54:19.719801 dkist-processing-common-6.2.0rc1/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)       66 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/changelog/185.feature.rst
--rw-rw-rw-   0 root         (0) root         (0)       66 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/changelog/187.misc.rst
--rw-rw-rw-   0 root         (0) root         (0)       28 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/changelog/188.misc.rst
--rwxrwxrwx   0 root         (0) root         (0)      642 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-25 21:54:19.719801 dkist-processing-common-6.2.0rc1/dkist_processing_common/
--rw-rw-rw-   0 root         (0) root         (0)      317 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-25 21:54:19.719801 dkist-processing-common-6.2.0rc1/dkist_processing_common/_util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/_util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2931 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/_util/config.py
--rw-rw-rw-   0 root         (0) root         (0)     3244 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/_util/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1178 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/_util/dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     3426 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/_util/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)    10378 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/_util/scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     6226 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/_util/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-25 21:54:19.719801 dkist-processing-common-6.2.0rc1/dkist_processing_common/codecs/
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/codecs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/codecs/asdf.py
--rw-rw-rw-   0 root         (0) root         (0)      495 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/codecs/bytes.py
--rw-rw-rw-   0 root         (0) root         (0)     2331 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/codecs/fits.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/codecs/iobase.py
--rw-rw-rw-   0 root         (0) root         (0)      939 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/codecs/json.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/codecs/path.py
--rw-rw-rw-   0 root         (0) root         (0)     3090 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/codecs/quality.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/codecs/str.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-25 21:54:19.719801 dkist-processing-common-6.2.0rc1/dkist_processing_common/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/fonts/Lato-Regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/fonts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7037 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/manual.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-25 21:54:19.723801 dkist-processing-common-6.2.0rc1/dkist_processing_common/models/
--rw-rw-rw-   0 root         (0) root         (0)       74 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5409 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     4113 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/models/fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     5128 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/models/flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)     3681 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/models/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     1109 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)     6532 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2225 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/models/quality.py
--rw-rw-rw-   0 root         (0) root         (0)    11949 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/models/tags.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/models/task_name.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/models/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-25 21:54:19.723801 dkist-processing-common-6.2.0rc1/dkist_processing_common/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       67 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6461 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/parsers/cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1571 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/parsers/dsps_repeat.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/parsers/experiment_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1536 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/parsers/id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/parsers/l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     2595 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/parsers/l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/parsers/proposal_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/parsers/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/parsers/single_value_single_key_flower.py
--rw-rw-rw-   0 root         (0) root         (0)     3938 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/parsers/task.py
--rw-rw-rw-   0 root         (0) root         (0)     7839 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     3041 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/parsers/unique_bud.py
--rw-rw-rw-   0 root         (0) root         (0)      545 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/parsers/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-25 21:54:19.723801 dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      562 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12488 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    13198 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/base.py
--rw-rw-rw-   0 root         (0) root         (0)     9876 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/l1_output_data.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-25 21:54:19.723801 dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6598 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/mixin/globus.py
--rw-rw-rw-   0 root         (0) root         (0)     6813 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/mixin/input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     2077 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/mixin/interservice_bus.py
--rw-rw-rw-   0 root         (0) root         (0)    14466 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/mixin/metadata_store.py
--rw-rw-rw-   0 root         (0) root         (0)     3242 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/mixin/object_store.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-25 21:54:19.723801 dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/mixin/quality/
--rw-rw-rw-   0 root         (0) root         (0)      383 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/mixin/quality/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8094 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/mixin/quality/_base.py
--rw-rw-rw-   0 root         (0) root         (0)    47664 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/mixin/quality/_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     3699 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     7986 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     8917 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     2270 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     5215 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     7979 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/trial_catalog.py
--rw-rw-rw-   0 root         (0) root         (0)     9483 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    19478 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-25 21:54:19.727801 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    27099 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     4165 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    16866 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_assemble_quality.py
--rw-rw-rw-   0 root         (0) root         (0)     7048 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)    20569 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_codecs.py
--rw-rw-rw-   0 root         (0) root         (0)     5903 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2408 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)    10946 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     3151 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)    19450 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     3120 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     8346 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    10629 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_publish_catalog_messages.py
--rw-rw-rw-   0 root         (0) root         (0)     9156 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    36296 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_quality_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    16481 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_scratch.py
--rw-rw-rw-   0 root         (0) root         (0)    24306 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_stems.py
--rw-rw-rw-   0 root         (0) root         (0)     3778 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_submit_dataset_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     5023 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     1234 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_task_name.py
--rw-rw-rw-   0 root         (0) root         (0)     4027 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_task_parsing.py
--rw-rw-rw-   0 root         (0) root         (0)     5494 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     6658 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2109 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_transfer_l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)     6453 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_trial_catalog.py
--rw-rw-rw-   0 root         (0) root         (0)    20114 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    10488 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_workflow_task_base.py
--rw-rw-rw-   0 root         (0) root         (0)    17411 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-25 21:54:19.719801 dkist-processing-common-6.2.0rc1/dkist_processing_common.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4394 2024-04-25 21:54:19.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5166 2024-04-25 21:54:19.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-25 21:54:19.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      823 2024-04-25 21:54:19.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-25 21:54:19.000000 dkist-processing-common-6.2.0rc1/dkist_processing_common.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-25 21:54:19.727801 dkist-processing-common-6.2.0rc1/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      120 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1890 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/docs/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-25 21:54:19.727801 dkist-processing-common-6.2.0rc1/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      780 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1887 2024-04-25 21:54:19.727801 dkist-processing-common-6.2.0rc1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2024-04-25 21:54:13.000000 dkist-processing-common-6.2.0rc1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:44:53.947109 dkist-processing-common-6.2.1rc2/
+-rw-rw-rw-   0 root         (0) root         (0)     2481 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      844 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      429 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    24493 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4370 2024-04-30 16:44:53.947109 dkist-processing-common-6.2.1rc2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3730 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3271 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:44:53.935109 dkist-processing-common-6.2.1rc2/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)       97 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/changelog/124.misc.rst
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/changelog/186.misc.rst
+-rw-rw-rw-   0 root         (0) root         (0)       66 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/changelog/187.misc.rst
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/changelog/188.misc.rst
+-rwxrwxrwx   0 root         (0) root         (0)      642 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:44:53.935109 dkist-processing-common-6.2.1rc2/dkist_processing_common/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:44:53.935109 dkist-processing-common-6.2.1rc2/dkist_processing_common/_util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/_util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2931 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/_util/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3244 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/_util/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1178 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/_util/dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     3426 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/_util/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)    10378 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/_util/scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     6226 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/_util/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:44:53.935109 dkist-processing-common-6.2.1rc2/dkist_processing_common/codecs/
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/codecs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/codecs/asdf.py
+-rw-rw-rw-   0 root         (0) root         (0)      495 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/codecs/bytes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2331 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/codecs/fits.py
+-rw-rw-rw-   0 root         (0) root         (0)      977 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/codecs/iobase.py
+-rw-rw-rw-   0 root         (0) root         (0)      939 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/codecs/json.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/codecs/path.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/codecs/str.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:44:53.939109 dkist-processing-common-6.2.1rc2/dkist_processing_common/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/fonts/Lato-Regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/fonts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7037 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/manual.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:44:53.939109 dkist-processing-common-6.2.1rc2/dkist_processing_common/models/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5409 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     4113 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/models/fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     5128 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/models/flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)     3681 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/models/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     1109 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     6532 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2225 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/models/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/models/quality_json_encoders.py
+-rw-rw-rw-   0 root         (0) root         (0)    11331 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/models/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      565 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/models/task_name.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/models/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:44:53.939109 dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6461 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/dsps_repeat.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/experiment_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     2595 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/proposal_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/single_value_single_key_flower.py
+-rw-rw-rw-   0 root         (0) root         (0)     3938 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     7839 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     3041 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/unique_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)      545 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:44:53.943109 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      562 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12507 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    13069 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8882 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/l1_output_data.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:44:53.943109 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6598 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/globus.py
+-rw-rw-rw-   0 root         (0) root         (0)     6813 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2077 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/interservice_bus.py
+-rw-rw-rw-   0 root         (0) root         (0)    14513 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/metadata_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     3242 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/object_store.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:44:53.943109 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/quality/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/quality/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8115 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/quality/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    47664 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/quality/_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3699 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7986 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     8852 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     2270 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     5215 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     6120 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/trial_catalog.py
+-rw-rw-rw-   0 root         (0) root         (0)     8200 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    19478 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:44:53.947109 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    27198 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4165 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     7048 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    11068 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_codecs.py
+-rw-rw-rw-   0 root         (0) root         (0)     5903 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2408 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)    10946 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     3151 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)    19450 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3120 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8346 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    10629 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_publish_catalog_messages.py
+-rw-rw-rw-   0 root         (0) root         (0)     9356 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    36297 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_quality_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    16481 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)    24306 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_stems.py
+-rw-rw-rw-   0 root         (0) root         (0)     5023 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     1234 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_task_name.py
+-rw-rw-rw-   0 root         (0) root         (0)     4027 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_task_parsing.py
+-rw-rw-rw-   0 root         (0) root         (0)     5494 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     6658 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2109 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_transfer_l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     4614 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_trial_catalog.py
+-rw-rw-rw-   0 root         (0) root         (0)    15740 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    10488 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_workflow_task_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    17411 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:44:53.935109 dkist-processing-common-6.2.1rc2/dkist_processing_common.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4370 2024-04-30 16:44:53.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5083 2024-04-30 16:44:53.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-30 16:44:53.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      770 2024-04-30 16:44:53.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-30 16:44:53.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:44:53.947109 dkist-processing-common-6.2.1rc2/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/docs/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:44:53.947109 dkist-processing-common-6.2.1rc2/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      780 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1839 2024-04-30 16:44:53.947109 dkist-processing-common-6.2.1rc2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/setup.py
```

### Comparing `dkist-processing-common-6.2.0rc1/.gitignore` & `dkist-processing-common-6.2.1rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/.pre-commit-config.yaml` & `dkist-processing-common-6.2.1rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/CHANGELOG.rst` & `dkist-processing-common-6.2.1rc2/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/PKG-INFO` & `dkist-processing-common-6.2.1rc2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 6.2.0rc1
+Version: 6.2.1rc2
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Provides-Extra: test
 Provides-Extra: docs
 Provides-Extra: inventory
 Provides-Extra: asdf
-Provides-Extra: quality
 
 dkist-processing-common
 =======================
 
 This repository works in concert with `dkist-processing-core <https://pypi.org/project/dkist-processing-core/>`_ and `dkist-processing-*instrument*` to
 form the DKIST calibration processing stack.
```

### Comparing `dkist-processing-common-6.2.0rc1/README.rst` & `dkist-processing-common-6.2.1rc2/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/bitbucket-pipelines.yml` & `dkist-processing-common-6.2.1rc2/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/check_changelog_updated.sh` & `dkist-processing-common-6.2.1rc2/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/_util/config.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/_util/config.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/_util/constants.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/_util/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/_util/dkist_location.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/_util/dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/_util/graphql.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/_util/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/_util/scratch.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/_util/scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/_util/tags.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/_util/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/codecs/asdf.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/codecs/asdf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/codecs/fits.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/codecs/fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/codecs/iobase.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/codecs/iobase.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/codecs/json.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/codecs/json.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/codecs/str.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/codecs/str.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/fonts/Lato-Regular.ttf` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/manual.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/manual.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/models/constants.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/models/fits_access.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/models/fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/models/flower_pot.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/models/flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/models/graphql.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/models/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/models/message.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/models/message.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/models/parameters.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/models/quality.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/models/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/models/tags.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/models/tags.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,20 +26,16 @@
     quality = "QUALITY"
     exposure_time = "EXP_TIME"
     readout_exp_time = "READOUT_EXP_TIME"
     quality_task = "QUALITY_TASK"
     parameter = "PARAMETER"
     workflow_task = "WORKFLOW_TASK"
     debug = "DEBUG"
-    # The QUALITY_DATA is the json data that normally gets stored to the remote (metadata store) database.
-    quality_data = "QUALITY_DATA"
-    # For trial workflows.
     dataset_inventory = "DATASET_INVENTORY"
     asdf = "ASDF"
-    quality_report = "QUALITY_REPORT"
 
 
 class Tag:
     """Controlled methods for creating tags from stems + optional suffixes."""
 
     @staticmethod
     def format_tag(stem: StemName | str, *parts):
@@ -173,24 +169,14 @@
         return cls.format_tag(StemName.movie)
 
     @classmethod
     def debug(cls) -> str:
         """Return a debug tag."""
         return cls.format_tag(StemName.debug)
 
-    @classmethod
-    def quality_data(cls) -> str:
-        """Tags the quality data that normally gets stored to the remote database."""
-        return cls.format_tag(StemName.quality_data.value)
-
-    @classmethod
-    def quality_report(cls) -> str:
-        """Tags the quality report .pdf that gets stored to the file system for trial workflows."""
-        return cls.format_tag(StemName.quality_report.value)
-
     # Task type tags
     @classmethod
     def task_observe(cls) -> str:
         """Tags input observe objects."""
         return cls.task(TaskName.observe.value)
 
     @classmethod
```

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/models/task_name.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/models/task_name.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/models/wavelength.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/models/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/parsers/cs_step.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/parsers/dsps_repeat.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/dsps_repeat.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/parsers/experiment_id_bud.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/experiment_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/parsers/id_bud.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/parsers/l0_fits_access.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/parsers/l1_fits_access.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/parsers/proposal_id_bud.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/proposal_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/parsers/quality.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/parsers/single_value_single_key_flower.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/single_value_single_key_flower.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/parsers/task.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/task.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/parsers/time.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/time.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/parsers/unique_bud.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/unique_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/parsers/wavelength.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/__init__.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/assemble_movie.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/assemble_movie.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """Task(s) for assembling a browse movie."""
+import logging
 from abc import ABC
 from abc import abstractmethod
 from typing import Literal
 
 import moviepy.editor as mpy
 import numpy as np
 import pkg_resources
-from dkist_service_configuration import logger
 from matplotlib import colormaps
 from PIL import Image
 from PIL import ImageDraw
 from PIL import ImageFont
 
 from dkist_processing_common.codecs.fits import fits_access_decoder
 from dkist_processing_common.models.fits_access import FitsAccessBase
 from dkist_processing_common.models.tags import Tag
 from dkist_processing_common.parsers.l0_fits_access import L1FitsAccess
 from dkist_processing_common.tasks import WorkflowTaskBase
 
 __all__ = ["AssembleMovie"]
 
+logger = logging.getLogger(__name__)
+
 
 class AssembleMovie(WorkflowTaskBase, ABC):
     """
 
     Assemble all movie frames (tagged with Tag.movie_frame()) into an mp4 movie file.
 
     It is intended to be subclassed so, e.g., instrument-specific overlays can be added.
@@ -148,15 +150,15 @@
         "{dataset_id}.mp4"
         """
         # This is here in `run` instead of `pre_run` because instruments may define their own `pre_run` that calls
         # `super().pre_run` and THEN updates the movie shape. No instrument should *ever* define its own `run` method.
         self.MOVIE_FRAME_SHAPE = self._ensure_movie_shape_is_even()
         clip = mpy.VideoClip(self.make_frame, duration=self.duration)
 
-        relative_movie_path = f"{self.constants.dataset_id}.mp4"
+        relative_movie_path = f"{self.constants.dataset_id}_browse_movie.mp4"
         absolute_movie_path = str(self.scratch.absolute_path(relative_movie_path))
 
         with self.apm_processing_step("Assembling movie frames"):
             clip.write_videofile(absolute_movie_path, fps=self.FPS, codec="libx264", audio=False)
 
         self.tag(path=absolute_movie_path, tags=[Tag.movie(), Tag.output()])
```

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/base.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Wrappers for all workflow tasks."""
 import json
 import logging
-import re
 from abc import ABC
 from pathlib import Path
 from typing import Any
 from typing import Generator
 from typing import Iterable
 from typing import Type
 
@@ -276,16 +275,15 @@
             for tag in tags_with_stem:
                 filename_parts.append(tag)
                 copied_tags.remove(tag)
 
         sorted_remaining_tags = sorted(copied_tags)
         filename_parts += sorted_remaining_tags
 
-        # replace spaces and underscores with dashes - dynamic part (e.g. polcal `Beam 1` label) may include spaces
-        dash_separated_parts = [re.sub("[ _]", "-", t) for t in filename_parts]
+        dash_separated_parts = [t.replace("_", "-") for t in filename_parts]
 
         base_filename = "_".join(dash_separated_parts)
         base_filename_counter = str(self.filename_counter.increment(base_filename))
         return base_filename + "_" + base_filename_counter + ".dat"
 
     def count(self, tags: tag_type_hint) -> int:
         """
```

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/l1_output_data.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/l1_output_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 """Task(s) for the transfer and publishing of L1 data from a production run of a processing pipeline."""
 import logging
-from abc import ABC
-from itertools import chain
 from pathlib import Path
 from typing import Iterable
 
-from dkist_processing_common.codecs.quality import quality_data_decoder
-from dkist_processing_common.codecs.quality import quality_data_encoder
 from dkist_processing_common.models.message import CatalogFrameMessage
 from dkist_processing_common.models.message import CatalogObjectMessage
 from dkist_processing_common.models.message import CreateQualityReportMessage
 from dkist_processing_common.models.tags import Tag
 from dkist_processing_common.tasks.mixin.globus import GlobusMixin
 from dkist_processing_common.tasks.mixin.interservice_bus import InterserviceBusMixin
-from dkist_processing_common.tasks.mixin.quality import QualityMixin
-from dkist_processing_common.tasks.output_data_base import OutputDataBase
-from dkist_processing_common.tasks.output_data_base import TransferDataBase
 
 
 __all__ = [
-    "L1OutputDataBase",
-    "TransferL1Data",
-    "AssembleQualityData",
-    "SubmitDatasetMetadata",
+    "AddDatasetReceiptAccount",
     "PublishCatalogAndQualityMessages",
+    "TransferL1Data",
+    "L1OutputDataBase",
+    "SubmitQuality",
 ]
 
+from dkist_processing_common.tasks.mixin.quality import QualityMixin
+from dkist_processing_common.tasks.output_data_base import OutputDataBase, TransferDataBase
 
 logger = logging.getLogger(__name__)
 
 
-class L1OutputDataBase(OutputDataBase, ABC):
+class L1OutputDataBase(OutputDataBase, QualityMixin):
     """Subclass of OutputDataBase which encapsulates common level 1 output data methods."""
 
     @property
     def dataset_has_quality_report(self) -> bool:
         """Return True if a quality report has been submitted to the metadata-store."""
         return self.metadata_store_quality_report_exists(dataset_id=self.constants.dataset_id)
 
@@ -95,80 +90,14 @@
             movie=movie,
             bucket=self.destination_bucket,
             object_key=movie_object_key,
             content_type="video/mp4",
         )
 
 
-class AssembleQualityData(L1OutputDataBase, QualityMixin):
-    """Assemble quality data from the various quality metrics."""
-
-    @property
-    def polcal_label_list(self) -> list[str] | None:
-        """Return the list of labels to look for when building polcal metrics.
-
-        If no labels are specified then no polcal metrics will be built.
-        """
-        return None
-
-    def run(self):
-        """Run method for the task."""
-        with self.apm_processing_step("Assembling quality data"):
-            quality_data = self.quality_assemble_data(polcal_label_list=self.polcal_label_list)
-
-        with self.apm_writing_step(
-            f"Saving quality data with {len(quality_data)} metrics to the file system"
-        ):
-            self.write(
-                quality_data,
-                tags=Tag.quality_data(),
-                encoder=quality_data_encoder,
-                relative_path=f"{self.constants.dataset_id}_quality_data.json",
-            )
-
-
-class SubmitDatasetMetadata(L1OutputDataBase):
-    """
-    Add quality data and receipt account to the metadata store.
-
-    Add the quality data to the Quality database.
-    Add a Dataset Receipt Account record to Processing Support for use by the Dataset Catalog Locker.
-    Adds the number of files created during the calibration processing to the Processing Support table
-    for use by the Dataset Catalog Locker.
-    """
-
-    def run(self) -> None:
-        """Run method for this task."""
-        with self.apm_writing_step(f"Storing quality data to metadata store"):
-            # each quality_data file is a list - this will combine the elements of multiple lists into a single list
-            quality_data = list(
-                chain.from_iterable(
-                    self.read(tags=Tag.quality_data(), decoder=quality_data_decoder)
-                )
-            )
-            self.metadata_store_add_quality_data(
-                dataset_id=self.constants.dataset_id, quality_data=quality_data
-            )
-        with self.apm_processing_step("Count Expected Outputs"):
-            dataset_id = self.constants.dataset_id
-            expected_object_count = self.count(tags=Tag.output())
-            if self.dataset_has_quality_report:
-                expected_object_count += 1
-        logger.info(
-            f"Adding Dataset Receipt Account: "
-            f"{dataset_id=}, {expected_object_count=}, recipe_run_id={self.recipe_run_id}"
-        )
-        with self.apm_task_step(
-            f"Add Dataset Receipt Account: {dataset_id = }, {expected_object_count = }"
-        ):
-            self.metadata_store_add_dataset_receipt_account(
-                dataset_id=dataset_id, expected_object_count=expected_object_count
-            )
-
-
 class PublishCatalogAndQualityMessages(L1OutputDataBase, InterserviceBusMixin):
     """Task class for publishing Catalog and Quality Messages."""
 
     def frame_messages(self, paths: Iterable[Path]) -> list[CatalogFrameMessage]:
         """
         Create the frame messages.
 
@@ -219,25 +148,25 @@
             for p in paths
         ]
         return messages
 
     @property
     def quality_report_message(self) -> CreateQualityReportMessage:
         """Create the Quality Report Message."""
-        file_name = Path(f"{self.constants.dataset_id}.pdf")
+        file_name = Path(f"{self.constants.dataset_id}_quality_report.pdf")
         return CreateQualityReportMessage(
             bucket=self.destination_bucket,
             objectName=self.format_object_key(file_name),
             conversationId=str(self.recipe_run_id),
             datasetId=self.constants.dataset_id,
             incrementDatasetCatalogReceiptCount=True,
         )
 
     def run(self) -> None:
-        """Run method for this task."""
+        """Run method for this trask."""
         with self.apm_task_step("Gather output data"):
             frames = self.read(tags=self.output_frame_tags)
             movies = self.read(tags=[Tag.output(), Tag.movie()])
         with self.apm_task_step("Create message objects"):
             messages = []
             messages += self.frame_messages(paths=frames)
             frame_message_count = len(messages)
@@ -246,7 +175,55 @@
             dataset_has_quality_report = self.dataset_has_quality_report
             if dataset_has_quality_report:
                 messages.append(self.quality_report_message)
         with self.apm_task_step(
             f"Publish messages: {frame_message_count = }, {object_message_count = }, {dataset_has_quality_report = }"
         ):
             self.interservice_bus_publish(messages=messages)
+
+
+class AddDatasetReceiptAccount(L1OutputDataBase):
+    """
+    Add a Dataset Receipt Account record to Processing Support for use by the Dataset Catalog Locker.
+
+    Adds the number of files created during the calibration processing to the Processing Support table
+    for use by the Dataset Catalog Locker.
+    """
+
+    def run(self) -> None:
+        """Run method for this task."""
+        with self.apm_processing_step("Count Expected Outputs"):
+            dataset_id = self.constants.dataset_id
+            expected_object_count = self.count(tags=Tag.output())
+            if self.dataset_has_quality_report:
+                expected_object_count += 1
+        logger.info(
+            f"Adding Dataset Receipt Account: "
+            f"{dataset_id=}, {expected_object_count=}, recipe_run_id={self.recipe_run_id}"
+        )
+        with self.apm_task_step(
+            f"Add Dataset Receipt Account: {dataset_id = }, {expected_object_count = }"
+        ):
+            self.metadata_store_add_dataset_receipt_account(
+                dataset_id=dataset_id, expected_object_count=expected_object_count
+            )
+
+
+class SubmitQuality(L1OutputDataBase, QualityMixin):
+    """Task class for submitting the quality report to the metadata store."""
+
+    @property
+    def polcal_label_list(self) -> list[str] | None:
+        """Return the list of labels to look for when building polcal metrics.
+
+        If no labels are specified then no polcal metrics will be built.
+        """
+        return None
+
+    def run(self):
+        """Run method for the task."""
+        with self.apm_processing_step("Building quality report"):
+            report = self.quality_build_report(polcal_label_list=self.polcal_label_list)
+        with self.apm_task_step(f"Submitting quality report: report section count = {len(report)}"):
+            self.metadata_store_add_quality_report(
+                dataset_id=self.constants.dataset_id, quality_report=report
+            )
```

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/mixin/globus.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/globus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/mixin/input_dataset.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/mixin/interservice_bus.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/interservice_bus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/mixin/metadata_store.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/metadata_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Mixin for a WorkflowDataTaskBase subclass which implements Metadata Store data access functionality."""
 import json
 import logging
 from functools import cached_property
 
 from dkist_processing_common._util.config import service_configuration
 from dkist_processing_common._util.graphql import GraphQLClient
-from dkist_processing_common.codecs.quality import QualityDataEncoder
 from dkist_processing_common.models.graphql import DatasetCatalogReceiptAccountMutation
 from dkist_processing_common.models.graphql import DatasetCatalogReceiptAccountResponse
 from dkist_processing_common.models.graphql import InputDatasetPartResponse
 from dkist_processing_common.models.graphql import InputDatasetRecipeRunResponse
 from dkist_processing_common.models.graphql import QualityReportMutation
 from dkist_processing_common.models.graphql import QualityReportQuery
 from dkist_processing_common.models.graphql import QualityReportResponse
@@ -18,14 +17,15 @@
 from dkist_processing_common.models.graphql import RecipeRunProvenanceMutation
 from dkist_processing_common.models.graphql import RecipeRunProvenanceResponse
 from dkist_processing_common.models.graphql import RecipeRunQuery
 from dkist_processing_common.models.graphql import RecipeRunResponse
 from dkist_processing_common.models.graphql import RecipeRunStatusMutation
 from dkist_processing_common.models.graphql import RecipeRunStatusQuery
 from dkist_processing_common.models.graphql import RecipeRunStatusResponse
+from dkist_processing_common.models.quality_json_encoders import QualityReportEncoder
 
 
 logger = logging.getLogger(__name__)
 
 input_dataset_part_document_type_hint = list | dict | str | int | float | None
 
 
@@ -74,18 +74,18 @@
         )
         self.metadata_store_client.execute_gql_mutation(
             mutation_base="createRecipeRunProvenance",
             mutation_parameters=params,
             mutation_response_cls=RecipeRunProvenanceResponse,
         )
 
-    def metadata_store_add_quality_data(self, dataset_id: str, quality_data: list[dict]):
-        """Add the quality data to the metadata-store."""
-        quality_data_json = json.dumps(quality_data, cls=QualityDataEncoder)
-        params = QualityReportMutation(datasetId=dataset_id, qualityReport=quality_data_json)
+    def metadata_store_add_quality_report(self, dataset_id: str, quality_report: list[dict]):
+        """Add the quality report to the metadata-store."""
+        quality_report_json = json.dumps(quality_report, cls=QualityReportEncoder, allow_nan=False)
+        params = QualityReportMutation(datasetId=dataset_id, qualityReport=quality_report_json)
         self.metadata_store_client.execute_gql_mutation(
             mutation_base="createQualityReport",
             mutation_parameters=params,
             mutation_response_cls=QualityReportResponse,
         )
 
     def metadata_store_quality_report_exists(self, dataset_id: str) -> bool:
```

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/mixin/object_store.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/object_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/mixin/quality/_base.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/quality/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """Base QualityMixin class that contains machinery common to all metric types."""
 from typing import Iterable
 
 import numpy as np
 
 from dkist_processing_common.codecs.json import json_encoder
-from dkist_processing_common.codecs.quality import QualityValueEncoder
+from dkist_processing_common.models.quality_json_encoders import QualityValueEncoder
 from dkist_processing_common.models.tags import Tag
 from dkist_processing_common.tasks.mixin.quality._metrics import _PolcalQualityMixin
 from dkist_processing_common.tasks.mixin.quality._metrics import _SimplePlotQualityMixin
 from dkist_processing_common.tasks.mixin.quality._metrics import _SimpleQualityMixin
 from dkist_processing_common.tasks.mixin.quality._metrics import _TableQualityMixin
 
 
 class QualityMixin(
     _SimpleQualityMixin, _SimplePlotQualityMixin, _TableQualityMixin, _PolcalQualityMixin
 ):
     """Mixin class supporting the generation of the quality reports."""
 
-    def quality_assemble_data(self, polcal_label_list: list[str] | None = None) -> list[dict]:
-        """Assemble the quality data by checking for the existence of each metric."""
+    def quality_build_report(self, polcal_label_list: list[str] | None = None) -> list[dict]:
+        """Build the quality report by checking for the existence of data for each metric."""
         report = []
         report += self.quality_task_independent_metrics()
         report += self.quality_task_dependent_metrics()
 
         polcal_labels = polcal_label_list or []
         report += self.quality_polcal_metrics(polcal_labels)
```

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/mixin/quality/_metrics.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/quality/_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/output_data_base.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/parse_l0_input_data.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/quality_metrics.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/quality_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,17 +80,15 @@
                     f"Calculating L0 metrics for task {quality_task_type_datum.quality_task_type}"
                 ):
                     for path in paths:
 
                         # We grab the task name
                         tags = self.tags(path)
                         task_type = [
-                            t.replace(f"{StemName.task.value}_", "")
-                            for t in tags
-                            if t.startswith("TASK")
+                            t.replace(f"{StemName.task.value}_", "") for t in tags if "TASK" in t
                         ][0]
 
                         if (
                             task_type.casefold()
                             == quality_task_type_datum.quality_task_type.casefold()
                         ):
                             frame = access_class.from_path(path)
```

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/teardown.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/transfer_input_data.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/trial_catalog.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/trial_catalog.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 """Tasks to support the generation of downstream artifacts in a trial workflow that wouldn't otherwise produce them."""
 import logging
 from datetime import datetime
 from importlib import resources
-from itertools import chain
 from pathlib import Path
 from typing import Generator
 from uuid import uuid4
 
 from dkist_processing_common.codecs.asdf import asdf_encoder
 from dkist_processing_common.codecs.fits import fits_access_decoder
 from dkist_processing_common.codecs.json import json_encoder
 from dkist_processing_common.codecs.path import path_decoder
-from dkist_processing_common.codecs.quality import quality_data_decoder
 from dkist_processing_common.models.fits_access import FitsAccessBase
 from dkist_processing_common.models.tags import Tag
 from dkist_processing_common.tasks.output_data_base import OutputDataBase
 
 logger = logging.getLogger(__name__)
 
-__all__ = ["CreateTrialDatasetInventory", "CreateTrialAsdf", "CreateTrialQualityReport"]
+__all__ = ["CreateTrialDatasetInventory", "CreateTrialAsdf"]
 
 
 # Capture condition of dkist-processing-common[inventory] install
 INVENTORY_EXTRA_INSTALLED = False
 try:
     from dkist_inventory.inventory import generate_inventory_from_frame_inventory
+    from dkist_inventory.inventory import generate_asdf_filename
 
     INVENTORY_EXTRA_INSTALLED = True
 except ModuleNotFoundError:
     pass
 
 # Capture condition of dkist-processing-common[asdf] install
 ASDF_EXTRA_INSTALLED = False
@@ -36,24 +35,14 @@
     import asdf
     from dkist_inventory.asdf_generator import asdf_tree_from_filenames
 
     ASDF_EXTRA_INSTALLED = True
 except ModuleNotFoundError:
     pass
 
-# Verify dkist-quality is installed
-QUALITY_EXTRA_INSTALLED = False
-try:
-    from dkist_quality.report import format_report
-    from dkist_quality.report import ReportFormattingException
-
-    QUALITY_EXTRA_INSTALLED = True
-except ModuleNotFoundError:
-    pass
-
 
 class CreateTrialDatasetInventory(OutputDataBase):
     """
     Task for use in Trial workflows that can simulate the generation of dataset inventory for the dataset.
 
     Warning: This task requires the dkist-inventory package.
     """
@@ -143,51 +132,14 @@
             )
         with self.apm_writing_step("Save ASDF file"):
             with resources.path("dkist.io", "level_1_dataset_schema.yaml") as schema_path:
                 self.write(
                     tree,
                     tags=[Tag.output(), Tag.asdf()],
                     encoder=asdf_encoder,
-                    relative_path=f"{self.constants.dataset_id}_asdf.asdf",
+                    relative_path=generate_asdf_filename(
+                        instrument=self.constants.instrument,
+                        start_time=datetime.fromisoformat(self.constants.obs_ip_start_time),
+                        dataset_id=self.constants.dataset_id,
+                    ),
                     custom_schema=schema_path.as_posix(),
                 )
-
-
-class CreateTrialQualityReport(OutputDataBase):
-    """
-    Task for use in Trial workflows to generate the quality report for the dataset.
-
-    Warning: This task requires the dkist-quality package.
-    """
-
-    def pre_run(self) -> None:
-        """Require the dkist-quality package be installed."""
-        if not QUALITY_EXTRA_INSTALLED:
-            raise ModuleNotFoundError(
-                f"{self.__class__.__name__} Task requires the dkist-quality package "
-                f"(e.g. via a 'quality' pip_extra on dkist_processing_core.Workflow().add_node())"
-                f" but the required dependencies were not found."
-            )
-
-    def run(self) -> None:
-        """Generate the quality report for the dataset."""
-        self.create_trial_quality_report()
-
-    def create_trial_quality_report(self) -> None:
-        """Generate a trial quality report in pdf format and save to the file system for future upload."""
-        with self.apm_processing_step(f"Building the trial quality report"):
-            # each quality_data file is a list - this will combine the elements of multiple lists into a single list
-            quality_data = list(
-                chain.from_iterable(
-                    self.read(tags=Tag.quality_data(), decoder=quality_data_decoder)
-                )
-            )
-            quality_report = format_report(
-                report_data=quality_data, dataset_id=self.constants.dataset_id
-            )
-
-        with self.apm_writing_step(f"Saving the trial quality report to the file system"):
-            self.write(
-                quality_report,
-                tags=[Tag.output(), Tag.quality_report()],
-                relative_path=f"{self.constants.dataset_id}_quality_report.pdf",
-            )
```

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/trial_output_data.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/trial_output_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,28 +90,14 @@
     def output_asdf_switch(self) -> bool:
         """Switch to turn on/off the transfer of the asdf file to the trial location."""
         return self.metadata_store_recipe_run_configuration().get(
             "trial_transfer_output_asdf", True
         )
 
     @property
-    def output_quality_data_switch(self) -> bool:
-        """Switch to turn on/off the transfer of the quality data to the trial location."""
-        return self.metadata_store_recipe_run_configuration().get(
-            "trial_transfer_output_quality_data", True
-        )
-
-    @property
-    def output_quality_report_switch(self) -> bool:
-        """Switch to turn on/off the transfer of the quality report to the trial location."""
-        return self.metadata_store_recipe_run_configuration().get(
-            "trial_transfer_output_quality_report", True
-        )
-
-    @property
     def specific_frame_tag_lists(self) -> list:
         """Return list of tag lists that define specific files we want to transfer to the trial location."""
         return self.metadata_store_recipe_run_configuration().get("trial_transfer_tag_lists", [])
 
     @abstractmethod
     def build_transfer_list(self) -> list[GlobusTransferItem]:
         """Build a list of all items on scratch to transfer to the trial location."""
@@ -171,27 +157,14 @@
     def build_output_asdf_transfer_list(self) -> list[GlobusTransferItem]:
         """Build a transfer list containing all frames tagged with OUTPUT and ASDF."""
         transfer_items = self.build_transfer_list_from_tag_lists(
             tag_lists=[Tag.output(), Tag.asdf()]
         )
         return transfer_items
 
-    def build_output_quality_data_transfer_list(self) -> list[GlobusTransferItem]:
-        """Build a transfer list containing all files tagged with OUTPUT and QUALITY_DATA."""
-        # quality data is not tagged as OUTPUT
-        transfer_items = self.build_transfer_list_from_tag_lists(tag_lists=[Tag.quality_data()])
-        return transfer_items
-
-    def build_output_quality_report_transfer_list(self) -> list[GlobusTransferItem]:
-        """Build a transfer list containing all files tagged with OUTPUT and QUALITY_REPORT."""
-        transfer_items = self.build_transfer_list_from_tag_lists(
-            tag_lists=[Tag.output(), Tag.quality_report()]
-        )
-        return transfer_items
-
     @property
     def intermediate_task_names(self) -> list[str]:
         """List specifying which TASK types to build when selecting INTERMEDIATE frames."""
         return []
 
     def build_intermediate_frame_transfer_list(self) -> list[GlobusTransferItem]:
         """
```

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tasks/write_l1.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/conftest.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -758,9 +758,13 @@
 @pytest.fixture()
 def fake_constants_db() -> dict:
     """
     A fake constants DB to prevent key errors.
 
     Usage on a task: task.constants._update(fake_constants_db)
     """
-    db = {"PROPOSAL_ID": "PROPID"}
+    db = {
+        "PROPOSAL_ID": "PROPID",
+        "INSTRUMENT": "INSTRUMENT",
+        "OBS_IP_START_TIME": "20240416T160000",
+    }
     return db
```

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_assemble_movie.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_base.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_constants.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_cs_step.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_dkist_location.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_fits_access.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_flower_pot.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_input_dataset.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_output_data_base.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_parameters.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_parse_l0_input_data.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_publish_catalog_messages.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_publish_catalog_messages.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_quality.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_quality.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import numpy as np
 import pytest
 from astropy.io import fits
 from astropy.wcs import WCS
 from dkist_data_simulator.spec122 import Spec122Dataset
 from dkist_data_simulator.spec214 import Spec214Dataset
 
+from dkist_processing_common.codecs.fits import fits_access_decoder
 from dkist_processing_common.codecs.fits import fits_hdulist_encoder
 from dkist_processing_common.models.tags import Tag
 from dkist_processing_common.parsers.l0_fits_access import L0FitsAccess
 from dkist_processing_common.tasks.quality_metrics import QualityL0Metrics
 from dkist_processing_common.tasks.quality_metrics import QualityL1Metrics
 
 
@@ -80,16 +81,18 @@
     return factory
 
 
 class QualityL0Task(QualityL0Metrics):
     def run(self) -> None:
         frames: Generator[L0FitsAccess, None, None] = self.read(
             tags=[Tag.input()],
+            decoder=fits_access_decoder,
+            fits_access_class=L0FitsAccess,
         )
-        self.calculate_l0_metrics(frames)
+        self.calculate_l0_metrics(frames=frames)
 
 
 @pytest.fixture
 def quality_l0_task(recipe_run_id):
     with QualityL0Task(
         recipe_run_id=recipe_run_id,
         workflow_name="workflow_name",
@@ -131,14 +134,15 @@
         )
         for hdul in hduls
         for t in task_types
     ]
     return quality_l0_task
 
 
+@pytest.mark.skip()
 @pytest.mark.parametrize("metric_name", ["FRAME_RMS", "FRAME_AVERAGE"])
 def test_l0_quality_metrics(
     quality_l0_task_with_quality_task_types, metric_name, quality_task_type
 ):
     """
     Given: a task with the QualityL0Metrics class
     When: checking that the task metric combination was created and stored correctly
@@ -157,14 +161,15 @@
             assert data["x_values"]
             assert data["y_values"]
             assert all(isinstance(item, str) for item in data["x_values"])
             assert all(isinstance(item, float) for item in data["y_values"])
             assert len(data["x_values"]) == len(data["y_values"])
 
 
+@pytest.mark.skip()
 @pytest.mark.parametrize("metric_name", ["FRAME_RMS", "FRAME_AVERAGE"])
 def test_l0_quality_metrics_missing_quality_task_types(
     quality_l0_task_without_quality_task_types, metric_name, quality_task_type
 ):
     """
     Given: a task with the QualityL0Metrics class
     When: checking that the task metric combination was created and stored correctly
```

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_quality_mixin.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_quality_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import numpy as np
 import pandas
 import pytest
 
 from dkist_processing_common._util.scratch import WorkflowFileSystem
 from dkist_processing_common.codecs.json import json_encoder
-from dkist_processing_common.codecs.quality import QualityValueEncoder
+from dkist_processing_common.models.quality_json_encoders import QualityValueEncoder
 from dkist_processing_common.models.tags import Tag
 from dkist_processing_common.tasks import WorkflowTaskBase
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
 
 
 class Task(WorkflowTaskBase, QualityMixin):
     def run(self):
@@ -609,16 +609,16 @@
     task.quality_store_sensitivity(datetimes=datetimes, values=values, stokes="V")
     task.quality_store_historical(name="hist 1", value=7)
     task.quality_store_historical(name="hist 2", value="abc")
     task.quality_store_historical(
         name="hist 3", value=9.35, warning="warning for historical metric 3"
     )
 
-    quality_data = task.quality_assemble_data()
-    assert len(quality_data) == 15
+    report = task.quality_build_report()
+    assert len(report) == 15
 
 
 def test_polcal_store_results(quality_task, initialized_polcal_fitter):
     """
     Given: A task with the QualityMixin and a realistic PolcalFitter
     When: Storing all polcal metrics
     Then: The correct metric json files are written and their contents contain the correct types of data
```

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_scratch.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_stems.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_stems.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_tags.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_task_name.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_task_name.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_task_parsing.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_task_parsing.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_teardown.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_transfer_input_data.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_transfer_l1_output_data.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_transfer_l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_trial_output_data.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_trial_output_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 from pathlib import Path
 from uuid import uuid4
 
 import pytest
-from pydantic.dataclasses import dataclass as validating_dataclass
 
 from dkist_processing_common._util.scratch import WorkflowFileSystem
 from dkist_processing_common.models.graphql import RecipeRunResponse
 from dkist_processing_common.models.tags import Tag
 from dkist_processing_common.tasks.mixin.globus import GlobusTransferItem
 from dkist_processing_common.tasks.trial_output_data import TransferTrialDataBase
 from dkist_processing_common.tests.conftest import FakeGQLClient
@@ -39,15 +38,15 @@
 
 @pytest.fixture
 def dummy_globus_transfer_item() -> GlobusTransferItem:
     return GlobusTransferItem(source_path="foo", destination_path="bar", recursive=True)
 
 
 @pytest.fixture
-def trial_output_task(dummy_globus_transfer_item) -> type[TransferTrialDataBase]:
+def trial_output_task(dummy_globus_transfer_item):
     class TransferTrialData(TransferTrialDataBase):
         def build_transfer_list(self) -> list[GlobusTransferItem]:
 
             transfer_list = [dummy_globus_transfer_item]
             return transfer_list
 
         @property
@@ -76,32 +75,18 @@
             scratch_base_path=tmp_path,
         )
         task.constants._update({"PROPOSAL_ID": proposal_id})
         yield task, proposal_id
         task._purge()
 
 
-@validating_dataclass
-class OutputFileObjects:
-    """File objects returned by complete_trial_output_task"""
-
-    debug_file_obj: bytes
-    intermediate_keep_file_obj: bytes
-    intermediate_discard_file_obj: bytes
-    dataset_inv_file_obj: bytes
-    asdf_file_obj: bytes
-    quality_data_obj: bytes
-    quality_report_file_obj: bytes
-    movie_file_obj: bytes
-
-
 @pytest.fixture
 def complete_trial_output_task(
     recipe_run_id, recipe_run_configuration, trial_output_task, tmp_path, mocker
-) -> tuple[TransferTrialDataBase, str, OutputFileObjects]:
+):
     mocker.patch(
         "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient",
         new=recipe_run_configuration,
     )
     proposal_id = "test_proposal_id"
     with trial_output_task(
         recipe_run_id=recipe_run_id,
@@ -114,47 +99,30 @@
         )
         task.constants._update({"PROPOSAL_ID": proposal_id})
 
         # Write a debug frame
         debug_file_obj = uuid4().hex.encode("utf8")
         task.write(debug_file_obj, relative_path="debug.ext", tags=[Tag.debug(), Tag.frame()])
 
-        # Write a dataset inventory file
-        dataset_inv_file_obj = uuid4().hex.encode("utf8")
-        task.write(
-            dataset_inv_file_obj,
-            relative_path="dataset_inv.ext",
-            tags=[Tag.output(), Tag.dataset_inventory()],
-        )
-
         # Write an asdf file
         asdf_file_obj = uuid4().hex.encode("utf8")
         task.write(asdf_file_obj, relative_path="asdf.ext", tags=[Tag.output(), Tag.asdf()])
 
-        # Write quality data
-        # quality data is not tagged as OUTPUT
-        quality_data_obj = uuid4().hex.encode("utf8")
-        task.write(
-            quality_data_obj,
-            relative_path="quality_data.json",
-            tags=Tag.quality_data(),
-        )
-
-        # Write a quality report file
-        quality_report_file_obj = uuid4().hex.encode("utf8")
-        task.write(
-            quality_report_file_obj,
-            relative_path="quality_report.pdf",
-            tags=[Tag.output(), Tag.quality_report()],
-        )
-
         # Write a movie file
         movie_file_obj = uuid4().hex.encode("utf8")
         task.write(movie_file_obj, relative_path="movie.mp4", tags=[Tag.output(), Tag.movie()])
 
+        # Write a dataset inventory file
+        dataset_inv_file_obj = uuid4().hex.encode("utf8")
+        task.write(
+            dataset_inv_file_obj,
+            relative_path="dataset_inv.ext",
+            tags=[Tag.output(), Tag.dataset_inventory()],
+        )
+
         # Write an intermediate frame that we want to transfer
         intermediate_keep_file_obj = uuid4().hex.encode("utf8")
         task.write(
             intermediate_keep_file_obj,
             relative_path="intermediate.ext",
             tags=[Tag.intermediate(), Tag.frame(), Tag.task("FOO")],
         )
@@ -163,26 +131,15 @@
         intermediate_discard_file_obj = uuid4().hex.encode("utf8")
         task.write(
             intermediate_discard_file_obj,
             relative_path="something_else.ext",
             tags=[Tag.intermediate(), Tag.frame(), Tag.task("WHO_CARES")],
         )
 
-        output_file_objects = OutputFileObjects(
-            debug_file_obj=debug_file_obj,
-            intermediate_keep_file_obj=intermediate_keep_file_obj,
-            intermediate_discard_file_obj=intermediate_discard_file_obj,
-            dataset_inv_file_obj=dataset_inv_file_obj,
-            asdf_file_obj=asdf_file_obj,
-            quality_data_obj=quality_data_obj,
-            quality_report_file_obj=quality_report_file_obj,
-            movie_file_obj=movie_file_obj,
-        )
-
-        yield task, proposal_id, output_file_objects
+        yield task, proposal_id, debug_file_obj, intermediate_keep_file_obj, intermediate_discard_file_obj, asdf_file_obj, dataset_inv_file_obj, movie_file_obj
         task._purge()
 
 
 @pytest.mark.parametrize(
     "custom_root_name, custom_dir_name",
     [
         pytest.param("roor", "foo", id="Custom trial dir name"),
@@ -226,16 +183,15 @@
 )
 def test_build_debug_transfer_list(complete_trial_output_task, destination_bucket, custom_dir_name):
     """
     Given: A Task based on TransferTrialDataBase with a tagged DEBUG frame
     When: Building the debug transfer list
     Then: The resulting transfer list has the correct source and destination paths and references the correct frames
     """
-    task, proposal_id, output_file_objects = complete_trial_output_task
-    debug_file_obj = output_file_objects.debug_file_obj
+    task, proposal_id, debug_file_obj, *_ = complete_trial_output_task
 
     transfer_list = task.build_debug_frame_transfer_list()
 
     assert len(transfer_list) == 1
     transfer_item = transfer_list[0]
     assert transfer_item.source_path == task.scratch.workflow_base_path / "debug.ext"
     expected_destination = Path(
@@ -253,16 +209,15 @@
     complete_trial_output_task, destination_bucket, custom_dir_name
 ):
     """
     Given: A Task based on TransferTrialDataBase with a tagged output asdf file
     When: Building the output asdf transfer list
     Then: The resulting transfer list has the correct source and destination paths and references the correct frames
     """
-    task, proposal_id, output_file_objects = complete_trial_output_task
-    asdf_file_obj = output_file_objects.asdf_file_obj
+    task, proposal_id, _, _, _, asdf_file_obj, *_ = complete_trial_output_task
 
     transfer_list = task.build_output_asdf_transfer_list()
 
     assert len(transfer_list) == 1
     transfer_item = transfer_list[0]
     assert transfer_item.source_path == task.scratch.workflow_base_path / "asdf.ext"
     expected_destination = Path(
@@ -272,84 +227,23 @@
     with transfer_item.source_path.open(mode="rb") as f:
         assert asdf_file_obj == f.read()
 
 
 @pytest.mark.parametrize(
     "custom_root_name, custom_dir_name", [pytest.param(None, "foo", id="Custom trial dir name")]
 )
-def test_build_output_quality_data_transfer_list(
-    complete_trial_output_task, destination_bucket, custom_dir_name
-):
-    """
-    Given: A Task based on TransferTrialDataBase with tagged output quality data
-    When: Building the output quality data transfer list
-    Then: The resulting transfer list has the correct source and destination paths and references the correct file
-    """
-    task, proposal_id, output_file_objects = complete_trial_output_task
-    quality_data_obj = output_file_objects.quality_data_obj
-
-    transfer_list = task.build_output_quality_data_transfer_list()
-
-    assert len(transfer_list) == 1
-    transfer_item = transfer_list[0]
-    assert transfer_item.source_path == task.scratch.workflow_base_path / "quality_data.json"
-    expected_destination = Path(
-        destination_bucket,
-        proposal_id,
-        custom_dir_name or task.constants.dataset_id,
-        "quality_data.json",
-    )
-    assert transfer_item.destination_path == expected_destination
-    with transfer_item.source_path.open(mode="rb") as f:
-        assert quality_data_obj == f.read()
-
-
-@pytest.mark.parametrize(
-    "custom_root_name, custom_dir_name", [pytest.param(None, "foo", id="Custom trial dir name")]
-)
-def test_build_output_quality_report_transfer_list(
-    complete_trial_output_task, destination_bucket, custom_dir_name
-):
-    """
-    Given: A Task based on TransferTrialDataBase with a tagged output quality report file
-    When: Building the output quality report transfer list
-    Then: The resulting transfer list has the correct source and destination paths and references the correct file
-    """
-    task, proposal_id, output_file_objects = complete_trial_output_task
-    quality_report_file_obj = output_file_objects.quality_report_file_obj
-
-    transfer_list = task.build_output_quality_report_transfer_list()
-
-    assert len(transfer_list) == 1
-    transfer_item = transfer_list[0]
-    assert transfer_item.source_path == task.scratch.workflow_base_path / "quality_report.pdf"
-    expected_destination = Path(
-        destination_bucket,
-        proposal_id,
-        custom_dir_name or task.constants.dataset_id,
-        "quality_report.pdf",
-    )
-    assert transfer_item.destination_path == expected_destination
-    with transfer_item.source_path.open(mode="rb") as f:
-        assert quality_report_file_obj == f.read()
-
-
-@pytest.mark.parametrize(
-    "custom_root_name, custom_dir_name", [pytest.param(None, "foo", id="Custom trial dir name")]
-)
 def test_build_output_dataset_inventory_transfer_list(
     complete_trial_output_task, destination_bucket, custom_dir_name
 ):
     """
     Given: A Task based on TransferTrialDataBase with a tagged output dataset inventory file
     When: Building the output dataset inventory transfer list
     Then: The resulting transfer list has the correct source and destination paths and references the correct frames
     """
-    task, proposal_id, output_file_objects = complete_trial_output_task
-    dataset_inv_file_obj = output_file_objects.dataset_inv_file_obj
+    task, proposal_id, _, _, _, _, dataset_inv_file_obj, *_ = complete_trial_output_task
 
     transfer_list = task.build_output_dataset_inventory_transfer_list()
 
     assert len(transfer_list) == 1
     transfer_item = transfer_list[0]
     assert transfer_item.source_path == task.scratch.workflow_base_path / "dataset_inv.ext"
     expected_destination = Path(
@@ -370,16 +264,15 @@
     complete_trial_output_task, destination_bucket, custom_dir_name
 ):
     """
     Given: A Task based on TransferTrialDataBase with a tagged output movie file
     When: Building the output movie transfer list
     Then: The resulting transfer list has the correct source and destination paths and references the correct files
     """
-    task, proposal_id, output_file_objects = complete_trial_output_task
-    movie_file_obj = output_file_objects.movie_file_obj
+    task, proposal_id, _, _, _, _, _, movie_file_obj, *_ = complete_trial_output_task
 
     transfer_list = task.build_output_movie_transfer_list()
 
     assert len(transfer_list) == 1
     transfer_item = transfer_list[0]
     assert transfer_item.source_path == task.scratch.workflow_base_path / "movie.mp4"
     expected_destination = Path(
@@ -397,16 +290,15 @@
     complete_trial_output_task, destination_bucket, custom_root_name
 ):
     """
     Given: A Task based on TransferTrialDataBase with tagged INTERMEDIATE frames
     When: Building the intermediate transfer list
     Then: The resulting transfer list has the correct source and destination paths and references the correct frames
     """
-    task, proposal_id, output_file_objects = complete_trial_output_task
-    intermediate_file_obj = output_file_objects.intermediate_keep_file_obj
+    task, proposal_id, _, intermediate_file_obj, *_ = complete_trial_output_task
 
     transfer_list = task.build_intermediate_frame_transfer_list()
     expected_destination_name = "intermediate.ext"
     expected_destination_path = Path(
         destination_bucket, task.format_object_key(Path(expected_destination_name))
     )
 
@@ -423,18 +315,22 @@
 )
 def test_build_transfer_list_from_tag_list(complete_trial_output_task, destination_bucket):
     """
     Given: A Task based on TransferTrialDataBase with tagged frames
     When: Building a transfer list from lists of tags
     Then: The transfer list is built with correct source and destination paths
     """
-    task, proposal_id, output_file_objects = complete_trial_output_task
-    debug_file_obj = output_file_objects.debug_file_obj
-    intermediate_file_obj = output_file_objects.intermediate_keep_file_obj
-    intermediate_file_obj_2 = output_file_objects.intermediate_discard_file_obj
+    (
+        task,
+        _,
+        debug_file_obj,
+        intermediate_file_obj,
+        intermediate_file_obj_2,
+        *_,
+    ) = complete_trial_output_task
 
     tag_list_1 = [Tag.frame(), Tag.task("WHO_CARES")]
     tag_list_2 = [Tag.debug()]
     tag_list_3 = [Tag.intermediate()]
     tag_list = [tag_list_1, tag_list_2, tag_list_3]
 
     transfer_list = task.build_transfer_list_from_tag_lists(tag_list)
@@ -484,16 +380,15 @@
     complete_trial_output_task, destination_bucket
 ):
     """
     Given: A Task based on TransferTrialDataBase with tagged frames
     When: Building a transfer list from a single list of tags
     Then: The transfer list is built with correct source and destination paths
     """
-    task, proposal_id, output_file_objects = complete_trial_output_task
-    debug_file_obj = output_file_objects.debug_file_obj
+    task, _, debug_file_obj, *_ = complete_trial_output_task
 
     tag_list = [Tag.debug()]
 
     transfer_list = task.build_transfer_list_from_tag_lists(tag_list)
 
     assert len(transfer_list) == 1
     transfer_item = transfer_list[0]
```

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_workflow_task_base.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_workflow_task_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common/tests/test_write_l1.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common.egg-info/PKG-INFO` & `dkist-processing-common-6.2.1rc2/dkist_processing_common.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 6.2.0rc1
+Version: 6.2.1rc2
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Provides-Extra: test
 Provides-Extra: docs
 Provides-Extra: inventory
 Provides-Extra: asdf
-Provides-Extra: quality
 
 dkist-processing-common
 =======================
 
 This repository works in concert with `dkist-processing-core <https://pypi.org/project/dkist-processing-core/>`_ and `dkist-processing-*instrument*` to
 form the DKIST calibration processing stack.
```

### Comparing `dkist-processing-common-6.2.0rc1/dkist_processing_common.egg-info/SOURCES.txt` & `dkist-processing-common-6.2.1rc2/dkist_processing_common.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 README.rst
 bitbucket-pipelines.yml
 check_changelog_updated.sh
 pyproject.toml
 setup.cfg
 setup.py
 changelog/.gitempty
-changelog/185.feature.rst
+changelog/124.misc.rst
+changelog/186.misc.rst
 changelog/187.misc.rst
 changelog/188.misc.rst
 dkist_processing_common/__init__.py
 dkist_processing_common/manual.py
 dkist_processing_common.egg-info/PKG-INFO
 dkist_processing_common.egg-info/SOURCES.txt
 dkist_processing_common.egg-info/dependency_links.txt
@@ -29,26 +30,26 @@
 dkist_processing_common/codecs/__init__.py
 dkist_processing_common/codecs/asdf.py
 dkist_processing_common/codecs/bytes.py
 dkist_processing_common/codecs/fits.py
 dkist_processing_common/codecs/iobase.py
 dkist_processing_common/codecs/json.py
 dkist_processing_common/codecs/path.py
-dkist_processing_common/codecs/quality.py
 dkist_processing_common/codecs/str.py
 dkist_processing_common/fonts/Lato-Regular.ttf
 dkist_processing_common/fonts/__init__.py
 dkist_processing_common/models/__init__.py
 dkist_processing_common/models/constants.py
 dkist_processing_common/models/fits_access.py
 dkist_processing_common/models/flower_pot.py
 dkist_processing_common/models/graphql.py
 dkist_processing_common/models/message.py
 dkist_processing_common/models/parameters.py
 dkist_processing_common/models/quality.py
+dkist_processing_common/models/quality_json_encoders.py
 dkist_processing_common/models/tags.py
 dkist_processing_common/models/task_name.py
 dkist_processing_common/models/wavelength.py
 dkist_processing_common/parsers/__init__.py
 dkist_processing_common/parsers/cs_step.py
 dkist_processing_common/parsers/dsps_repeat.py
 dkist_processing_common/parsers/experiment_id_bud.py
@@ -82,15 +83,14 @@
 dkist_processing_common/tasks/mixin/object_store.py
 dkist_processing_common/tasks/mixin/quality/__init__.py
 dkist_processing_common/tasks/mixin/quality/_base.py
 dkist_processing_common/tasks/mixin/quality/_metrics.py
 dkist_processing_common/tests/__init__.py
 dkist_processing_common/tests/conftest.py
 dkist_processing_common/tests/test_assemble_movie.py
-dkist_processing_common/tests/test_assemble_quality.py
 dkist_processing_common/tests/test_base.py
 dkist_processing_common/tests/test_codecs.py
 dkist_processing_common/tests/test_constants.py
 dkist_processing_common/tests/test_cs_step.py
 dkist_processing_common/tests/test_dkist_location.py
 dkist_processing_common/tests/test_fits_access.py
 dkist_processing_common/tests/test_flower_pot.py
@@ -99,15 +99,14 @@
 dkist_processing_common/tests/test_parameters.py
 dkist_processing_common/tests/test_parse_l0_input_data.py
 dkist_processing_common/tests/test_publish_catalog_messages.py
 dkist_processing_common/tests/test_quality.py
 dkist_processing_common/tests/test_quality_mixin.py
 dkist_processing_common/tests/test_scratch.py
 dkist_processing_common/tests/test_stems.py
-dkist_processing_common/tests/test_submit_dataset_metadata.py
 dkist_processing_common/tests/test_tags.py
 dkist_processing_common/tests/test_task_name.py
 dkist_processing_common/tests/test_task_parsing.py
 dkist_processing_common/tests/test_teardown.py
 dkist_processing_common/tests/test_transfer_input_data.py
 dkist_processing_common/tests/test_transfer_l1_output_data.py
 dkist_processing_common/tests/test_trial_catalog.py
```

### Comparing `dkist-processing-common-6.2.0rc1/docs/Makefile` & `dkist-processing-common-6.2.1rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/docs/conf.py` & `dkist-processing-common-6.2.1rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/docs/make.bat` & `dkist-processing-common-6.2.1rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/licenses/LICENSE.rst` & `dkist-processing-common-6.2.1rc2/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/pyproject.toml` & `dkist-processing-common-6.2.1rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.0rc1/setup.cfg` & `dkist-processing-common-6.2.1rc2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -50,29 +50,26 @@
 	pytest-cov
 	pytest-mock
 	hypothesis
 	towncrier
 	dkist-data-simulator >= 5.0.0
 	%(inventory)s
 	%(asdf)s
-	%(quality)s
 docs = 
 	sphinx
 	sphinx-astropy
 	sphinx-changelog
 	sphinx-autoapi
 	pytest
 	towncrier < 22.12.0
 	dkist-sphinx-theme
 inventory = 
-	dkist-inventory >= 1.2.1
+	dkist-inventory >= 1.3.1
 asdf = 
-	dkist-inventory[asdf] >= 1.2.1
-quality = 
-	dkist-quality >= 1.0.1
+	dkist-inventory[asdf] >= 1.3.1
 
 [build_docs]
 source-dir = docs
 build-dir = docs/_build
 all_files = 1
 
 [upload_docs]
```

