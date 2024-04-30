# Comparing `tmp/spikeinterface-0.99.0.tar.gz` & `tmp/spikeinterface-0.99.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spikeinterface-0.99.0.tar", last modified: Fri Nov  3 09:17:33 2023, max compression
+gzip compressed data, was "spikeinterface-0.99.1.tar", last modified: Mon Nov 13 14:48:38 2023, max compression
```

## Comparing `spikeinterface-0.99.0.tar` & `spikeinterface-0.99.1.tar`

### file list

```diff
@@ -1,325 +1,325 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 09:17:33.798447 spikeinterface-0.99.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8586 2023-11-03 09:17:33.798447 spikeinterface-0.99.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4324 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-03 09:17:33.798447 spikeinterface-0.99.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      225 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 09:17:33.722447 spikeinterface-0.99.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 09:17:33.726447 spikeinterface-0.99.0/src/spikeinterface/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 09:17:33.730448 spikeinterface-0.99.0/src/spikeinterface/comparison/
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/comparison/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11506 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/comparison/basecomparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     8560 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/comparison/collision.py
--rw-r--r--   0 runner    (1001) docker     (127)    30758 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/comparison/comparisontools.py
--rw-r--r--   0 runner    (1001) docker     (127)     6353 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/comparison/correlogram.py
--rw-r--r--   0 runner    (1001) docker     (127)    16352 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/comparison/groundtruthstudy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10485 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/comparison/hybrid.py
--rw-r--r--   0 runner    (1001) docker     (127)    15091 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/comparison/multicomparisons.py
--rw-r--r--   0 runner    (1001) docker     (127)    25915 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/comparison/paircomparisons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 09:17:33.738448 spikeinterface-0.99.0/src/spikeinterface/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42763 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4876 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/baseevent.py
--rw-r--r--   0 runner    (1001) docker     (127)    29795 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/baserecording.py
--rw-r--r--   0 runner    (1001) docker     (127)    20161 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/baserecordingsnippets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9357 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/basesnippets.py
--rw-r--r--   0 runner    (1001) docker     (127)    22622 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/basesorting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/binaryfolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7850 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/binaryrecordingextractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7584 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/channelsaggregationrecording.py
--rw-r--r--   0 runner    (1001) docker     (127)     7730 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/channelslice.py
--rw-r--r--   0 runner    (1001) docker     (127)    31373 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/core_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/frameslicerecording.py
--rw-r--r--   0 runner    (1001) docker     (127)     4935 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/frameslicesorting.py
--rw-r--r--   0 runner    (1001) docker     (127)    57256 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)    16774 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/job_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    24618 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/node_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/npyfoldersnippets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5460 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/npysnippetsextractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/npzfolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/npzsortingextractor.py
--rw-r--r--   0 runner    (1001) docker     (127)    21499 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/numpyextractors.py
--rw-r--r--   0 runner    (1001) docker     (127)    13580 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/old_api_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13558 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/recording_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    25530 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/segmentutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/snippets_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4681 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/sortingfolder.py
--rw-r--r--   0 runner    (1001) docker     (127)    17436 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/sparsity.py
--rw-r--r--   0 runner    (1001) docker     (127)     8246 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/template_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/testing_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5576 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/unitsaggregationsorting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/unitsselectionsorting.py
--rw-r--r--   0 runner    (1001) docker     (127)    83925 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/waveform_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)    24204 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/waveform_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/core/zarrrecordingextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 09:17:33.742447 spikeinterface-0.99.0/src/spikeinterface/curation/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/curation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18978 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/curation/auto_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5144 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/curation/curation_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7996 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/curation/curationsorting.py
--rw-r--r--   0 runner    (1001) docker     (127)     8638 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/curation/mergeunitssorting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/curation/remove_duplicated_spikes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/curation/remove_excess_spikes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7225 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/curation/remove_redundant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5007 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/curation/sortingview_curation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/curation/splitunitsorting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 09:17:33.742447 spikeinterface-0.99.0/src/spikeinterface/exporters/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/exporters/report.py
--rw-r--r--   0 runner    (1001) docker     (127)    12385 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/exporters/to_phy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 09:17:33.746447 spikeinterface-0.99.0/src/spikeinterface/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6815 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/alfsortingextractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/bids.py
--rw-r--r--   0 runner    (1001) docker     (127)     4774 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/cbin_ibl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9574 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/cellexplorersortingextractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4348 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/combinatoextractors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/extractorlist.py
--rw-r--r--   0 runner    (1001) docker     (127)    10124 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/hdsortextractors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5788 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/herdingspikesextractors.py
--rw-r--r--   0 runner    (1001) docker     (127)    10567 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/iblstreamingrecording.py
--rw-r--r--   0 runner    (1001) docker     (127)     6161 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/klustaextractors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/matlabhelpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/mclustextractors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/mcsh5extractors.py
--rw-r--r--   0 runner    (1001) docker     (127)    25541 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/mdaextractors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 09:17:33.750448 spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/alphaomega.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/axona.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/biocam.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/blackrock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/ced.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/edf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/intan.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/maxwell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/mcsraw.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/mearec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/neo_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    27753 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/neobaseextractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/neuralynx.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/neuroexplorer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13914 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/neuroscope.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/nix.py
--rw-r--r--   0 runner    (1001) docker     (127)    14480 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/openephys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/plexon.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/plexon2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/spike2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/spikegadgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4445 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/spikeglx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/tdt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/neuropixels_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25159 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/nwbextractors.py
--rw-r--r--   0 runner    (1001) docker     (127)    10881 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/phykilosortextractors.py
--rw-r--r--   0 runner    (1001) docker     (127)     8917 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/shybridextractors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/spykingcircusextractors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/toy_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/tridesclousextractors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5687 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/waveclussnippetstextractors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/waveclustextractors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/extractors/yassextractors.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/full.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 09:17:33.754448 spikeinterface-0.99.0/src/spikeinterface/postprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/postprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/postprocessing/alignsorting.py
--rw-r--r--   0 runner    (1001) docker     (127)    28897 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/postprocessing/amplitude_scalings.py
--rw-r--r--   0 runner    (1001) docker     (127)    13802 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/postprocessing/correlograms.py
--rw-r--r--   0 runner    (1001) docker     (127)     7347 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/postprocessing/isi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/postprocessing/noise_level.py
--rw-r--r--   0 runner    (1001) docker     (127)    29949 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/postprocessing/principal_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     9477 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/postprocessing/spike_amplitudes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7292 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/postprocessing/spike_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)    38395 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/postprocessing/template_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6808 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/postprocessing/template_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)    23003 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/postprocessing/unit_localization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 09:17:33.762447 spikeinterface-0.99.0/src/spikeinterface/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/align_snippets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/astype.py
--rw-r--r--   0 runner    (1001) docker     (127)     5516 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/average_across_direction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/basepreprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6672 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     8634 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/common_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     3126 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/correct_lsb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 09:17:33.762447 spikeinterface-0.99.0/src/spikeinterface/preprocessing/deepinterpolation/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/deepinterpolation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7556 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/deepinterpolation/deepinterpolation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13959 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/deepinterpolation/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/deepinterpolation/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11069 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/deepinterpolation/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/depth_order.py
--rw-r--r--   0 runner    (1001) docker     (127)    16030 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/detect_bad_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     5523 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/directional_derivative.py
--rw-r--r--   0 runner    (1001) docker     (127)     9851 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/filter_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     9280 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/filter_opencl.py
--rw-r--r--   0 runner    (1001) docker     (127)    11119 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/highpass_spatial_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/interpolate_bad_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)    14167 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/motion.py
--rw-r--r--   0 runner    (1001) docker     (127)    11315 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/normalize_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)     6691 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/phase_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/preprocessing_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/preprocessinglist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/rectify.py
--rw-r--r--   0 runner    (1001) docker     (127)    20984 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/remove_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     7369 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/resample.py
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/silence_periods.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/unsigned_to_signed.py
--rw-r--r--   0 runner    (1001) docker     (127)     7643 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/whiten.py
--rw-r--r--   0 runner    (1001) docker     (127)     9669 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/preprocessing/zero_channel_pad.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 09:17:33.762447 spikeinterface-0.99.0/src/spikeinterface/qualitymetrics/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/qualitymetrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51942 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/qualitymetrics/misc_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    37907 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/qualitymetrics/pca_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9260 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/qualitymetrics/quality_metric_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/qualitymetrics/quality_metric_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/qualitymetrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 09:17:33.766447 spikeinterface-0.99.0/src/spikeinterface/sorters/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16663 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/basesorter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 09:17:33.770447 spikeinterface-0.99.0/src/spikeinterface/sorters/external/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7937 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/external/combinato.py
--rw-r--r--   0 runner    (1001) docker     (127)    12446 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/external/hdsort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/external/hdsort_master.m
--rw-r--r--   0 runner    (1001) docker     (127)     9055 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/external/herdingspikes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12045 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/external/ironclust.py
--rw-r--r--   0 runner    (1001) docker     (127)     9407 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/external/kilosort.py
--rw-r--r--   0 runner    (1001) docker     (127)     9189 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/external/kilosort2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10570 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/external/kilosort2_5.py
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/external/kilosort2_5_master.m
--rw-r--r--   0 runner    (1001) docker     (127)     4460 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/external/kilosort2_master.m
--rw-r--r--   0 runner    (1001) docker     (127)    10356 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/external/kilosort3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4809 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/external/kilosort3_master.m
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/external/kilosort_master.m
--rw-r--r--   0 runner    (1001) docker     (127)    10767 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/external/kilosortbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     6053 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/external/klusta.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      533 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/external/klusta_config_default.prm
--rw-r--r--   0 runner    (1001) docker     (127)     5818 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/external/mountainsort4.py
--rw-r--r--   0 runner    (1001) docker     (127)     8275 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/external/mountainsort5.py
--rw-r--r--   0 runner    (1001) docker     (127)     8723 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/external/pykilosort.py
--rw-r--r--   0 runner    (1001) docker     (127)     7564 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/external/sc_config_default.params
--rw-r--r--   0 runner    (1001) docker     (127)     6625 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/external/spyking_circus.py
--rw-r--r--   0 runner    (1001) docker     (127)     6812 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/external/tridesclous.py
--rw-r--r--   0 runner    (1001) docker     (127)    12251 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/external/waveclus.py
--rw-r--r--   0 runner    (1001) docker     (127)     6560 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/external/waveclus_master.m
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/external/waveclus_snippets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3707 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/external/waveclus_snippets_master.m
--rw-r--r--   0 runner    (1001) docker     (127)    14413 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/external/yass.py
--rw-r--r--   0 runner    (1001) docker     (127)     6034 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/external/yass_config_default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 09:17:33.770447 spikeinterface-0.99.0/src/spikeinterface/sorters/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/internal/si_based.py
--rw-r--r--   0 runner    (1001) docker     (127)     7051 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/internal/spyking_circus2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12918 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/internal/tridesclous2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15338 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    30487 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/runsorter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/sorterlist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 09:17:33.774448 spikeinterface-0.99.0/src/spikeinterface/sorters/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/utils/constructNPYheader.m
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7279 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/utils/shellscript.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sorters/utils/writeNPY.m
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 09:17:33.774448 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 09:17:33.778447 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21605 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/benchmark/benchmark_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)    29219 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/benchmark/benchmark_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)    22159 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/benchmark/benchmark_motion_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)    25787 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/benchmark/benchmark_motion_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (127)    18606 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/benchmark/benchmark_peak_localization.py
--rw-r--r--   0 runner    (1001) docker     (127)    25129 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/benchmark/benchmark_peak_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/benchmark/benchmark_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 09:17:33.782447 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10692 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/circus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)    28055 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/clustering_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7307 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/isocut5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    22761 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/method_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/position.py
--rw-r--r--   0 runner    (1001) docker     (127)     7041 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/position_and_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     9208 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/position_and_pca.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/position_ptp_scaled.py
--rw-r--r--   0 runner    (1001) docker     (127)     9293 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/random_projections.py
--rw-r--r--   0 runner    (1001) docker     (127)    21202 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/sliding_hdbscan.py
--rw-r--r--   0 runner    (1001) docker     (127)    24935 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/sliding_nn.py
--rw-r--r--   0 runner    (1001) docker     (127)     9467 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/split.py
--rw-r--r--   0 runner    (1001) docker     (127)     5496 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/triage.py
--rw-r--r--   0 runner    (1001) docker     (127)    15007 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/features_from_peaks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 09:17:33.782447 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/matching/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/matching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46518 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/matching/circus.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/matching/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/matching/method_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/matching/naive.py
--rw-r--r--   0 runner    (1001) docker     (127)    13795 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/matching/tdc.py
--rw-r--r--   0 runner    (1001) docker     (127)    44820 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/matching/wobble.py
--rw-r--r--   0 runner    (1001) docker     (127)    59836 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/motion_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)    15952 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/motion_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (127)    40441 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/peak_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)    17492 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/peak_localization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/peak_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    13570 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/peak_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 09:17:33.782447 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/waveforms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/waveforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5426 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/waveforms/neural_network_denoiser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/waveforms/savgol_denoiser.py
--rw-r--r--   0 runner    (1001) docker     (127)    11502 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/waveforms/temporal_pca.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/waveforms/waveform_thresholder.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/waveforms/waveform_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 09:17:33.790447 spikeinterface-0.99.0/src/spikeinterface/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/all_amplitudes_distributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10070 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/amplitudes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/autocorrelograms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9297 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/collision.py
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/crosscorrelograms.py
--rw-r--r--   0 runner    (1001) docker     (127)    10639 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/gtstudy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/isi_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     9421 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6405 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/motion.py
--rw-r--r--   0 runner    (1001) docker     (127)     9800 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/multicomparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     5089 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/peak_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/probe_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/rasters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/sorting_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)    10907 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/spike_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)    12356 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/spikes_on_traces.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/template_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/template_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)    20901 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/traces.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/unit_depths.py
--rw-r--r--   0 runner    (1001) docker     (127)     8801 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/unit_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/unit_presence.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/unit_probe_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/unit_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/unit_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    16028 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/unit_waveforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     8389 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/unit_waveforms_density_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     7179 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13304 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/utils_ipywidgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/utils_matplotlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/utils_sortingview.py
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2023-11-03 09:16:33.000000 spikeinterface-0.99.0/src/spikeinterface/widgets/widget_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 09:17:33.726447 spikeinterface-0.99.0/src/spikeinterface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8586 2023-11-03 09:17:33.000000 spikeinterface-0.99.0/src/spikeinterface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14974 2023-11-03 09:17:33.000000 spikeinterface-0.99.0/src/spikeinterface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-03 09:17:33.000000 spikeinterface-0.99.0/src/spikeinterface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      932 2023-11-03 09:17:33.000000 spikeinterface-0.99.0/src/spikeinterface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-11-03 09:17:33.000000 spikeinterface-0.99.0/src/spikeinterface.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 14:48:38.802067 spikeinterface-0.99.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8586 2023-11-13 14:48:38.802067 spikeinterface-0.99.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4324 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4802 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-13 14:48:38.802067 spikeinterface-0.99.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 14:48:38.758068 spikeinterface-0.99.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 14:48:38.758068 spikeinterface-0.99.1/src/spikeinterface/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 14:48:38.758068 spikeinterface-0.99.1/src/spikeinterface/comparison/
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/comparison/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11506 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/comparison/basecomparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8560 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/comparison/collision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33483 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/comparison/comparisontools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6353 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/comparison/correlogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16352 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/comparison/groundtruthstudy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10485 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/comparison/hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15091 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/comparison/multicomparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26081 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/comparison/paircomparisons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 14:48:38.766068 spikeinterface-0.99.1/src/spikeinterface/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43010 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4876 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/baseevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29795 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/baserecording.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20161 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/baserecordingsnippets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9357 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/basesnippets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22622 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/basesorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/binaryfolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7850 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/binaryrecordingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7584 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/channelsaggregationrecording.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7730 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/channelslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31373 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/core_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/frameslicerecording.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4935 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/frameslicesorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57256 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16774 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/job_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24618 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/node_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/npyfoldersnippets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/npysnippetsextractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/npzfolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/npzsortingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21499 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/numpyextractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13580 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/old_api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13558 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/recording_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25530 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/segmentutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/snippets_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4681 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/sortingfolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17436 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/sparsity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8246 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/template_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5576 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/unitsaggregationsorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/unitsselectionsorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83925 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/waveform_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24204 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/waveform_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/core/zarrrecordingextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 14:48:38.766068 spikeinterface-0.99.1/src/spikeinterface/curation/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/curation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18978 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/curation/auto_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/curation/curation_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7996 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/curation/curationsorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8638 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/curation/mergeunitssorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/curation/remove_duplicated_spikes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/curation/remove_excess_spikes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7225 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/curation/remove_redundant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5007 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/curation/sortingview_curation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/curation/splitunitsorting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 14:48:38.766068 spikeinterface-0.99.1/src/spikeinterface/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5508 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/exporters/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12385 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/exporters/to_phy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 14:48:38.770067 spikeinterface-0.99.1/src/spikeinterface/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/alfsortingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/bids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/cbin_ibl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9574 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/cellexplorersortingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4348 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/combinatoextractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/extractorlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10124 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/hdsortextractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/herdingspikesextractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/iblstreamingrecording.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6161 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/klustaextractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/matlabhelpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/mclustextractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/mcsh5extractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25541 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/mdaextractors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 14:48:38.770067 spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/alphaomega.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/axona.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/biocam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/blackrock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/ced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/edf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/intan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/maxwell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/mcsraw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/mearec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/neo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27753 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/neobaseextractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/neuralynx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/neuroexplorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13914 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/neuroscope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/nix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14480 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/openephys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/plexon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/plexon2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/spike2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/spikegadgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4445 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/spikeglx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/tdt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4355 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/neuropixels_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25159 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/nwbextractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10881 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/phykilosortextractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8917 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/shybridextractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/spykingcircusextractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/toy_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/tridesclousextractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5687 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/waveclussnippetstextractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/waveclustextractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/extractors/yassextractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/full.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 14:48:38.774067 spikeinterface-0.99.1/src/spikeinterface/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/postprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/postprocessing/alignsorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28897 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/postprocessing/amplitude_scalings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13802 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/postprocessing/correlograms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7347 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/postprocessing/isi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/postprocessing/noise_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29949 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/postprocessing/principal_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9477 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/postprocessing/spike_amplitudes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7292 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/postprocessing/spike_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38395 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/postprocessing/template_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6808 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/postprocessing/template_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23003 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/postprocessing/unit_localization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 14:48:38.778067 spikeinterface-0.99.1/src/spikeinterface/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/align_snippets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/astype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5516 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/average_across_direction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/basepreprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6672 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8634 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/common_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/correct_lsb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 14:48:38.778067 spikeinterface-0.99.1/src/spikeinterface/preprocessing/deepinterpolation/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/deepinterpolation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7556 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/deepinterpolation/deepinterpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13959 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/deepinterpolation/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/deepinterpolation/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11069 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/deepinterpolation/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/depth_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16030 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/detect_bad_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5523 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/directional_derivative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9851 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/filter_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9280 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/filter_opencl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11119 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/highpass_spatial_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/interpolate_bad_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14167 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/motion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11315 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/normalize_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6691 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/phase_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/preprocessing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/preprocessinglist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/rectify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20984 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/remove_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7369 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/resample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/silence_periods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/unsigned_to_signed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7643 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/whiten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9669 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/preprocessing/zero_channel_pad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 14:48:38.778067 spikeinterface-0.99.1/src/spikeinterface/qualitymetrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/qualitymetrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51942 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/qualitymetrics/misc_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37907 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/qualitymetrics/pca_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9260 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/qualitymetrics/quality_metric_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/qualitymetrics/quality_metric_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/qualitymetrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 14:48:38.778067 spikeinterface-0.99.1/src/spikeinterface/sorters/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16663 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/basesorter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 14:48:38.782067 spikeinterface-0.99.1/src/spikeinterface/sorters/external/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7937 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/external/combinato.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12446 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/external/hdsort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/external/hdsort_master.m
+-rw-r--r--   0 runner    (1001) docker     (127)     9055 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/external/herdingspikes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12045 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/external/ironclust.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9407 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/external/kilosort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9189 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/external/kilosort2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10570 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/external/kilosort2_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/external/kilosort2_5_master.m
+-rw-r--r--   0 runner    (1001) docker     (127)     4460 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/external/kilosort2_master.m
+-rw-r--r--   0 runner    (1001) docker     (127)    10356 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/external/kilosort3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/external/kilosort3_master.m
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/external/kilosort_master.m
+-rw-r--r--   0 runner    (1001) docker     (127)    10767 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/external/kilosortbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6053 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/external/klusta.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      533 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/external/klusta_config_default.prm
+-rw-r--r--   0 runner    (1001) docker     (127)     5818 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/external/mountainsort4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8275 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/external/mountainsort5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/external/pykilosort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7564 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/external/sc_config_default.params
+-rw-r--r--   0 runner    (1001) docker     (127)     6625 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/external/spyking_circus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6812 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/external/tridesclous.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12251 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/external/waveclus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6560 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/external/waveclus_master.m
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/external/waveclus_snippets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/external/waveclus_snippets_master.m
+-rw-r--r--   0 runner    (1001) docker     (127)    14413 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/external/yass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6034 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/external/yass_config_default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 14:48:38.782067 spikeinterface-0.99.1/src/spikeinterface/sorters/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/internal/si_based.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7051 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/internal/spyking_circus2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12918 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/internal/tridesclous2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15338 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30487 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/runsorter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/sorterlist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 14:48:38.782067 spikeinterface-0.99.1/src/spikeinterface/sorters/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/utils/constructNPYheader.m
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7279 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/utils/shellscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sorters/utils/writeNPY.m
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 14:48:38.782067 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 14:48:38.786067 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21605 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29219 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22159 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_motion_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25787 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_motion_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18606 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_peak_localization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25129 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_peak_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 14:48:38.786067 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/circus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28055 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/clustering_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7307 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/isocut5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22761 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/method_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/position.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7041 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/position_and_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9208 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/position_and_pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/position_ptp_scaled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9293 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/random_projections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21202 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/sliding_hdbscan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24935 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/sliding_nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9467 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5496 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/triage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15007 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/features_from_peaks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 14:48:38.786067 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/matching/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46518 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/matching/circus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/matching/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/matching/method_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/matching/naive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13795 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/matching/tdc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44820 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/matching/wobble.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59836 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/motion_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16018 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/motion_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40441 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/peak_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17492 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/peak_localization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/peak_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13570 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/peak_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 14:48:38.790067 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/waveforms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/waveforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5426 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/waveforms/neural_network_denoiser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/waveforms/savgol_denoiser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11502 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/waveforms/temporal_pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/waveforms/waveform_thresholder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/waveforms/waveform_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 14:48:38.794067 spikeinterface-0.99.1/src/spikeinterface/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/all_amplitudes_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10070 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/amplitudes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/autocorrelograms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9297 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/collision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/crosscorrelograms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10639 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/gtstudy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/isi_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9421 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6405 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/motion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9800 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/multicomparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5089 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/peak_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/probe_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/rasters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/sorting_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10907 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/spike_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12356 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/spikes_on_traces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/template_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/template_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20901 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/traces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/unit_depths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8801 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/unit_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/unit_presence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/unit_probe_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/unit_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/unit_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16028 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/unit_waveforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8389 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/unit_waveforms_density_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7179 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13304 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/utils_ipywidgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/utils_matplotlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/utils_sortingview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2023-11-13 14:47:44.000000 spikeinterface-0.99.1/src/spikeinterface/widgets/widget_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 14:48:38.758068 spikeinterface-0.99.1/src/spikeinterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8586 2023-11-13 14:48:38.000000 spikeinterface-0.99.1/src/spikeinterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14974 2023-11-13 14:48:38.000000 spikeinterface-0.99.1/src/spikeinterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-13 14:48:38.000000 spikeinterface-0.99.1/src/spikeinterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2023-11-13 14:48:38.000000 spikeinterface-0.99.1/src/spikeinterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2023-11-13 14:48:38.000000 spikeinterface-0.99.1/src/spikeinterface.egg-info/top_level.txt
```

### Comparing `spikeinterface-0.99.0/LICENSE` & `spikeinterface-0.99.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/PKG-INFO` & `spikeinterface-0.99.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spikeinterface
-Version: 0.99.0
+Version: 0.99.1
 Summary: Python toolkit for analysis, visualization, and comparison of spike sorting output
 Author-email: Alessio Buccino <alessiop.buccino@gmail.com>, Samuel Garcia <sam.garcia.die@gmail.com>
 Project-URL: homepage, https://github.com/SpikeInterface/spikeinterface
 Project-URL: repository, https://github.com/SpikeInterface/spikeinterface
 Project-URL: documentation, https://spikeinterface.readthedocs.io/
 Project-URL: changelog, https://spikeinterface.readthedocs.io/en/latest/whatisnew.html
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -158,15 +158,15 @@
 - export a report and/or export to phy
 - offer a powerful Qt-based viewer in a separate package [spikeinterface-gui](https://github.com/SpikeInterface/spikeinterface-gui)
 - have powerful sorting components to build your own sorter.
 
 
 ## Documentation
 
-Detailed documentation of the latest PyPI release of SpikeInterface can be found [here](https://spikeinterface.readthedocs.io/en/0.98.2).
+Detailed documentation of the latest PyPI release of SpikeInterface can be found [here](https://spikeinterface.readthedocs.io/en/0.99.1).
 
 Detailed documentation of the development version of SpikeInterface can be found [here](https://spikeinterface.readthedocs.io/en/latest).
 
 Several tutorials to get started can be found in [spiketutorials](https://github.com/SpikeInterface/spiketutorials).
 
 There are also some useful notebooks [on our blog](https://spikeinterface.github.io) that cover advanced benchmarking
 and sorting components.
```

### Comparing `spikeinterface-0.99.0/README.md` & `spikeinterface-0.99.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 - export a report and/or export to phy
 - offer a powerful Qt-based viewer in a separate package [spikeinterface-gui](https://github.com/SpikeInterface/spikeinterface-gui)
 - have powerful sorting components to build your own sorter.
 
 
 ## Documentation
 
-Detailed documentation of the latest PyPI release of SpikeInterface can be found [here](https://spikeinterface.readthedocs.io/en/0.98.2).
+Detailed documentation of the latest PyPI release of SpikeInterface can be found [here](https://spikeinterface.readthedocs.io/en/0.99.1).
 
 Detailed documentation of the development version of SpikeInterface can be found [here](https://spikeinterface.readthedocs.io/en/latest).
 
 Several tutorials to get started can be found in [spiketutorials](https://github.com/SpikeInterface/spiketutorials).
 
 There are also some useful notebooks [on our blog](https://spikeinterface.github.io) that cover advanced benchmarking
 and sorting components.
```

#### html2text {}

```diff
@@ -20,15 +20,15 @@
 metrics to validate and curate spike sorting outputs. - visualize recordings
 and spike sorting outputs in several ways (matplotlib, sortingview, jupyter,
 ephyviewer) - export a report and/or export to phy - offer a powerful Qt-based
 viewer in a separate package [spikeinterface-gui](https://github.com/
 SpikeInterface/spikeinterface-gui) - have powerful sorting components to build
 your own sorter. ## Documentation Detailed documentation of the latest PyPI
 release of SpikeInterface can be found [here](https://
-spikeinterface.readthedocs.io/en/0.98.2). Detailed documentation of the
+spikeinterface.readthedocs.io/en/0.99.1). Detailed documentation of the
 development version of SpikeInterface can be found [here](https://
 spikeinterface.readthedocs.io/en/latest). Several tutorials to get started can
 be found in [spiketutorials](https://github.com/SpikeInterface/spiketutorials).
 There are also some useful notebooks [on our blog](https://
 spikeinterface.github.io) that cover advanced benchmarking and sorting
 components. You can also have a look at the [spikeinterface-gui](https://
 github.com/SpikeInterface/spikeinterface-gui). ## How to install spikeinterface
```

### Comparing `spikeinterface-0.99.0/pyproject.toml` & `spikeinterface-0.99.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "spikeinterface"
-version = "0.99.0"
+version = "0.99.1"
 authors = [
   { name="Alessio Buccino", email="alessiop.buccino@gmail.com" },
   { name="Samuel Garcia", email="sam.garcia.die@gmail.com" },
 ]
 description = "Python toolkit for analysis, visualization, and comparison of spike sorting output"
 readme = "README.md"
 requires-python = ">=3.8,<4.0"
```

### Comparing `spikeinterface-0.99.0/src/spikeinterface/__init__.py` & `spikeinterface-0.99.1/src/spikeinterface/__init__.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/comparison/__init__.py` & `spikeinterface-0.99.1/src/spikeinterface/comparison/__init__.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/comparison/basecomparison.py` & `spikeinterface-0.99.1/src/spikeinterface/comparison/basecomparison.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/comparison/collision.py` & `spikeinterface-0.99.1/src/spikeinterface/comparison/collision.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/comparison/comparisontools.py` & `spikeinterface-0.99.1/src/spikeinterface/comparison/comparisontools.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,34 +59,30 @@
         return 0
     return num_matches / denom
 
 
 def do_count_event(sorting):
     """
     Count event for each units in a sorting.
+
+    Kept for backward compatibility sorting.count_num_spikes_per_unit() is doing the same.
+
     Parameters
     ----------
     sorting: SortingExtractor
         A sorting extractor
 
     Returns
     -------
     event_count: pd.Series
         Nb of spike by units.
     """
     import pandas as pd
 
-    unit_ids = sorting.get_unit_ids()
-    ev_counts = np.zeros(len(unit_ids), dtype="int64")
-    for segment_index in range(sorting.get_num_segments()):
-        ev_counts += np.array(
-            [len(sorting.get_unit_spike_train(u, segment_index=segment_index)) for u in unit_ids], dtype="int64"
-        )
-    event_counts = pd.Series(ev_counts, index=unit_ids)
-    return event_counts
+    return pd.Series(sorting.count_num_spikes_per_unit())
 
 
 def count_match_spikes(times1, all_times2, delta_frames):  # , event_counts1, event_counts2  unit2_ids,
     """
     Computes matching spikes between one spike train and a list of others.
 
     Parameters
@@ -120,124 +116,157 @@
     if hasattr(get_optimized_compute_matching_matrix, "_cached_function"):
         return get_optimized_compute_matching_matrix._cached_function
 
     import numba
 
     @numba.jit(nopython=True, nogil=True)
     def compute_matching_matrix(
-        frames_spike_train1,
-        frames_spike_train2,
+        spike_frames_train1,
+        spike_frames_train2,
         unit_indices1,
         unit_indices2,
-        num_units_sorting1,
-        num_units_sorting2,
+        num_units_train1,
+        num_units_train2,
         delta_frames,
     ):
         """
-        Compute a matrix representing the matches between two spike trains.
-
-        Given two spike trains, this function finds matching spikes based on a temporal proximity criterion
-        defined by `delta_frames`. The resulting matrix indicates the number of matches between units
-        in `frames_spike_train1` and `frames_spike_train2`.
+        Internal function used by `make_match_count_matrix()`.
+        This function is for one segment only.
+        The loop over segment is done in `make_match_count_matrix()`
 
         Parameters
         ----------
-        frames_spike_train1 : ndarray
-            Array of frames for the first spike train. Should be ordered in ascending order.
-        frames_spike_train2 : ndarray
-            Array of frames for the second spike train. Should be ordered in ascending order.
+        spike_frames_train1 : ndarray
+            An array of integer frame numbers corresponding to spike times for the first train. Must be in ascending order.
+        spike_frames_train2 : ndarray
+            An array of integer frame numbers corresponding to spike times for the second train. Must be in ascending order.
         unit_indices1 : ndarray
-            Array indicating the unit indices corresponding to each spike in `frames_spike_train1`.
+            An array of integers where `unit_indices1[i]` gives the unit index associated with the spike at `spike_frames_train1[i]`.
         unit_indices2 : ndarray
-            Array indicating the unit indices corresponding to each spike in `frames_spike_train2`.
-        num_units_sorting1 : int
-            Total number of units in the first spike train.
-        num_units_sorting2 : int
-            Total number of units in the second spike train.
+            An array of integers where `unit_indices2[i]` gives the unit index associated with the spike at `spike_frames_train2[i]`.
+        num_units_train1 : int
+            The total count of unique units in the first spike train.
+        num_units_train2 : int
+            The total count of unique units in the second spike train.
         delta_frames : int
-            Maximum difference in frames between two spikes to consider them as a match.
+            The inclusive upper limit on the frame difference for which two spikes are considered matching. That is
+            if `abs(spike_frames_train1[i] - spike_frames_train2[j]) <= delta_frames` then the spikes at `spike_frames_train1[i]`
+            and `spike_frames_train2[j]` are considered matching.
 
         Returns
         -------
         matching_matrix : ndarray
-            A matrix of shape (num_units_sorting1, num_units_sorting2) where each entry [i, j] represents
-            the number of matching spikes between unit i of `frames_spike_train1` and unit j of `frames_spike_train2`.
-
-        Notes
-        -----
-        This algorithm identifies matching spikes between two ordered spike trains.
-        By iterating through each spike in the first train, it compares them against spikes in the second train,
-        determining matches based on the two spikes frames being within `delta_frames` of each other.
-
-        To avoid redundant comparisons the algorithm maintains a reference, `lower_search_limit_in_second_train`,
-        which signifies the minimal index in the second spike train that might match the upcoming spike
-        in the first train. This means that the start of the search moves forward in the second train as the
-        matches between the two trains are found decreasing the number of comparisons needed.
-
-        An important condition here is thatthe same spike is not matched twice. This is managed by keeping track
-        of the last matched frame for each unit pair in `previous_frame1_match` and `previous_frame2_match`
+            A 2D numpy array of shape `(num_units_train1, num_units_train2)`. Each element `[i, j]` represents
+            the count of matching spike pairs between unit `i` from `spike_frames_train1` and unit `j` from `spike_frames_train2`.
 
-        For more details on the rationale behind this approach, refer to the documentation of this module and/or
-        the  metrics section in SpikeForest documentation.
         """
 
-        matching_matrix = np.zeros((num_units_sorting1, num_units_sorting2), dtype=np.uint16)
+        matching_matrix = np.zeros((num_units_train1, num_units_train2), dtype=np.uint64)
 
         # Used to avoid the same spike matching twice
-        previous_frame1_match = -np.ones_like(matching_matrix, dtype=np.int64)
-        previous_frame2_match = -np.ones_like(matching_matrix, dtype=np.int64)
+        last_match_frame1 = -np.ones_like(matching_matrix, dtype=np.int64)
+        last_match_frame2 = -np.ones_like(matching_matrix, dtype=np.int64)
 
-        lower_search_limit_in_second_train = 0
+        num_spike_frames_train1 = len(spike_frames_train1)
+        num_spike_frames_train2 = len(spike_frames_train2)
 
-        for index1 in range(len(frames_spike_train1)):
-            # Keeps track of which frame in the second spike train should be used as a search start for matches
-            index2 = lower_search_limit_in_second_train
-            frame1 = frames_spike_train1[index1]
-
-            # Determine next_frame1 if current frame is not the last frame
-            not_in_the_last_loop = index1 < len(frames_spike_train1) - 1
-            if not_in_the_last_loop:
-                next_frame1 = frames_spike_train1[index1 + 1]
-
-            while index2 < len(frames_spike_train2):
-                frame2 = frames_spike_train2[index2]
-                not_a_match = abs(frame1 - frame2) > delta_frames
-                if not_a_match:
-                    # Go to the next frame in the first train
+        # Keeps track of which frame in the second spike train should be used as a search start for matches
+        second_train_search_start = 0
+        for index1 in range(num_spike_frames_train1):
+            frame1 = spike_frames_train1[index1]
+
+            for index2 in range(second_train_search_start, num_spike_frames_train2):
+                frame2 = spike_frames_train2[index2]
+                if frame2 < frame1 - delta_frames:
+                    # no match move the left limit for the next loop
+                    second_train_search_start += 1
+                    continue
+                elif frame2 > frame1 + delta_frames:
+                    # no match stop search in train2 and continue increment in train1
                     break
+                else:
+                    # match
+                    unit_index1, unit_index2 = unit_indices1[index1], unit_indices2[index2]
+
+                    if (
+                        index1 != last_match_frame1[unit_index1, unit_index2]
+                        and index2 != last_match_frame2[unit_index1, unit_index2]
+                    ):
+                        last_match_frame1[unit_index1, unit_index2] = index1
+                        last_match_frame2[unit_index1, unit_index2] = index2
 
-                # Map the match to a matrix
-                row, column = unit_indices1[index1], unit_indices2[index2]
-
-                # The same spike cannot be matched twice see the notes in the docstring for more info on this constraint
-                if frame1 != previous_frame1_match[row, column] and frame2 != previous_frame2_match[row, column]:
-                    previous_frame1_match[row, column] = frame1
-                    previous_frame2_match[row, column] = frame2
-
-                    matching_matrix[row, column] += 1
-
-                index2 += 1
-
-                # Advance the lower_search_limit_in_second_train if the next frame in the first train does not match
-                not_a_match_with_next = abs(next_frame1 - frame2) > delta_frames
-                if not_a_match_with_next:
-                    lower_search_limit_in_second_train = index2
+                        matching_matrix[unit_index1, unit_index2] += 1
 
         return matching_matrix
 
     # Cache the compiled function
     get_optimized_compute_matching_matrix._cached_function = compute_matching_matrix
 
     return compute_matching_matrix
 
 
-def make_match_count_matrix(sorting1, sorting2, delta_frames, n_jobs=None):
+def make_match_count_matrix(sorting1, sorting2, delta_frames, ensure_symmetry=False):
+    """
+    Computes a matrix representing the matches between two Sorting objects.
+
+    Given two spike trains, this function finds matching spikes based on a temporal proximity criterion
+    defined by `delta_frames`. The resulting matrix indicates the number of matches between units
+    in `spike_frames_train1` and `spike_frames_train2` for each pair of units.
+
+    Note that this algo is not symmetric and is biased with `sorting1` representing ground truth for the comparison
+
+    Parameters
+    ----------
+    sorting1 : Sorting
+        An array of integer frame numbers corresponding to spike times for the first train. Must be in ascending order.
+    sorting2 : Sorting
+        An array of integer frame numbers corresponding to spike times for the second train. Must be in ascending order.
+    delta_frames : int
+        The inclusive upper limit on the frame difference for which two spikes are considered matching. That is
+        if `abs(spike_frames_train1[i] - spike_frames_train2[j]) <= delta_frames` then the spikes at
+        `spike_frames_train1[i]` and `spike_frames_train2[j]` are considered matching.
+    ensure_symmetry: bool, default False
+        If ensure_symmetry=True, then the algo is run two times by switching sorting1 and sorting2.
+        And the minimum of the two results is taken.
+    Returns
+    -------
+    matching_matrix : ndarray
+        A 2D numpy array of shape `(num_units_train1, num_units_train2)`. Each element `[i, j]` represents
+        the count of matching spike pairs between unit `i` from `spike_frames_train1` and unit `j` from `spike_frames_train2`.
+
+    Notes
+    -----
+    This algorithm identifies matching spikes between two ordered spike trains.
+    By iterating through each spike in the first train, it compares them against spikes in the second train,
+    determining matches based on the two spikes frames being within `delta_frames` of each other.
+
+    To avoid redundant comparisons the algorithm maintains a reference, `second_train_search_start `,
+    which signifies the minimal index in the second spike train that might match the upcoming spike
+    in the first train.
+
+    The logic can be summarized as follows:
+    1. Iterate through each spike in the first train
+    2. For each spike, find the first match in the second train.
+    3. Save the index of the first match as the new `second_train_search_start `
+    3. For each match, find as many matches as possible from the first match onwards.
+
+    An important condition here is that the same spike is not matched twice. This is managed by keeping track
+    of the last matched frame for each unit pair in `last_match_frame1` and `last_match_frame2`
+    There are corner cases where a spike can be counted twice in the spiketrain 2 if there are bouts of bursting activity
+    (below delta_frames) in the spiketrain 1. To ensure that the number of matches does not exceed the number of spikes,
+    we apply a final clip.
+
+
+    For more details on the rationale behind this approach, refer to the documentation of this module and/or
+    the metrics section in SpikeForest documentation.
+    """
+
     num_units_sorting1 = sorting1.get_num_units()
     num_units_sorting2 = sorting2.get_num_units()
-    matching_matrix = np.zeros((num_units_sorting1, num_units_sorting2), dtype=np.uint16)
+    matching_matrix = np.zeros((num_units_sorting1, num_units_sorting2), dtype=np.uint64)
 
     spike_vector1_segments = sorting1.to_spike_vector(concatenated=False)
     spike_vector2_segments = sorting2.to_spike_vector(concatenated=False)
 
     num_segments_sorting1 = sorting1.get_num_segments()
     num_segments_sorting2 = sorting2.get_num_segments()
     assert (
@@ -251,53 +280,73 @@
 
         sample_frames1_sorted = spike_vector1["sample_index"]
         sample_frames2_sorted = spike_vector2["sample_index"]
 
         unit_indices1_sorted = spike_vector1["unit_index"]
         unit_indices2_sorted = spike_vector2["unit_index"]
 
-        matching_matrix += get_optimized_compute_matching_matrix()(
+        matching_matrix_seg = get_optimized_compute_matching_matrix()(
             sample_frames1_sorted,
             sample_frames2_sorted,
             unit_indices1_sorted,
             unit_indices2_sorted,
             num_units_sorting1,
             num_units_sorting2,
             delta_frames,
         )
 
+        if ensure_symmetry:
+            matching_matrix_seg_switch = get_optimized_compute_matching_matrix()(
+                sample_frames2_sorted,
+                sample_frames1_sorted,
+                unit_indices2_sorted,
+                unit_indices1_sorted,
+                num_units_sorting2,
+                num_units_sorting1,
+                delta_frames,
+            )
+            matching_matrix_seg = np.maximum(matching_matrix_seg, matching_matrix_seg_switch.T)
+
+        matching_matrix += matching_matrix_seg
+
+    # ensure the number of match do not exceed the number of spike in train 2
+    # this is a simple way to handle corner cases for bursting in sorting1
+    spike_count2 = np.array(list(sorting2.count_num_spikes_per_unit().values()))
+    spike_count2 = spike_count2[np.newaxis, :]
+    matching_matrix = np.clip(matching_matrix, None, spike_count2)
+
     # Build a data frame from the matching matrix
     import pandas as pd
 
     unit_ids_of_sorting1 = sorting1.get_unit_ids()
     unit_ids_of_sorting2 = sorting2.get_unit_ids()
     match_event_counts_df = pd.DataFrame(matching_matrix, index=unit_ids_of_sorting1, columns=unit_ids_of_sorting2)
 
     return match_event_counts_df
 
 
-def make_agreement_scores(sorting1, sorting2, delta_frames, n_jobs=1):
+def make_agreement_scores(sorting1, sorting2, delta_frames, ensure_symmetry=True):
     """
     Make the agreement matrix.
     No threshold (min_score) is applied at this step.
 
-    Note : this computation is symmetric.
+    Note : this computation is symmetric by default.
     Inverting sorting1 and sorting2 give the transposed matrix.
 
     Parameters
     ----------
     sorting1: SortingExtractor
         The first sorting extractor
     sorting2: SortingExtractor
         The second sorting extractor
     delta_frames: int
         Number of frames to consider spikes coincident
-    n_jobs: int
-        Number of jobs to run in parallel
-
+    ensure_symmetry: bool, default: True
+        If ensure_symmetry is True, then the algo is run two times by switching sorting1 and sorting2.
+        And the minimum of the two results is taken.
     Returns
     -------
     agreement_scores: array (float)
         The agreement score matrix.
     """
     import pandas as pd
 
@@ -305,15 +354,15 @@
     unit2_ids = np.array(sorting2.get_unit_ids())
 
     ev_counts1 = np.array(list(sorting1.count_num_spikes_per_unit().values()))
     ev_counts2 = np.array(list(sorting2.count_num_spikes_per_unit().values()))
     event_counts1 = pd.Series(ev_counts1, index=unit1_ids)
     event_counts2 = pd.Series(ev_counts2, index=unit2_ids)
 
-    match_event_count = make_match_count_matrix(sorting1, sorting2, delta_frames, n_jobs=n_jobs)
+    match_event_count = make_match_count_matrix(sorting1, sorting2, delta_frames, ensure_symmetry=ensure_symmetry)
 
     agreement_scores = make_agreement_scores_from_count(match_event_count, event_counts1, event_counts2)
 
     return agreement_scores
 
 
 def make_agreement_scores_from_count(match_event_count, event_counts1, event_counts2):
```

### Comparing `spikeinterface-0.99.0/src/spikeinterface/comparison/correlogram.py` & `spikeinterface-0.99.1/src/spikeinterface/comparison/correlogram.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/comparison/groundtruthstudy.py` & `spikeinterface-0.99.1/src/spikeinterface/comparison/groundtruthstudy.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/comparison/hybrid.py` & `spikeinterface-0.99.1/src/spikeinterface/comparison/hybrid.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/comparison/multicomparisons.py` & `spikeinterface-0.99.1/src/spikeinterface/comparison/multicomparisons.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/comparison/paircomparisons.py` & `spikeinterface-0.99.1/src/spikeinterface/comparison/paircomparisons.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         sorting1,
         sorting2,
         sorting1_name=None,
         sorting2_name=None,
         delta_time=0.4,
         match_score=0.5,
         chance_score=0.1,
+        ensure_symmetry=False,
         n_jobs=1,
         verbose=False,
     ):
         if sorting1_name is None:
             sorting1_name = "sorting1"
         if sorting2_name is None:
             sorting2_name = "sorting2"
@@ -51,14 +52,16 @@
         )
         MixinSpikeTrainComparison.__init__(self, delta_time=delta_time, n_jobs=n_jobs)
         self.set_frames_and_frequency(self.object_list)
 
         self.unit1_ids = self.sorting1.get_unit_ids()
         self.unit2_ids = self.sorting2.get_unit_ids()
 
+        self.ensure_symmetry = ensure_symmetry
+
         self._do_agreement()
         self._do_matching()
 
     @property
     def sorting1(self):
         return self.object_list[0]
 
@@ -81,15 +84,15 @@
         # common to GroundTruthComparison and SymmetricSortingComparison
         # spike count for each spike train
         self.event_counts1 = do_count_event(self.sorting1)
         self.event_counts2 = do_count_event(self.sorting2)
 
         # matrix of  event match count for each pair
         self.match_event_count = make_match_count_matrix(
-            self.sorting1, self.sorting2, self.delta_frames, n_jobs=self.n_jobs
+            self.sorting1, self.sorting2, self.delta_frames, ensure_symmetry=self.ensure_symmetry
         )
 
         # agreement matrix score for each pair
         self.agreement_scores = make_agreement_scores_from_count(
             self.match_event_count, self.event_counts1, self.event_counts2
         )
 
@@ -149,14 +152,15 @@
             sorting1,
             sorting2,
             sorting1_name=sorting1_name,
             sorting2_name=sorting2_name,
             delta_time=delta_time,
             match_score=match_score,
             chance_score=chance_score,
+            ensure_symmetry=True,
             n_jobs=n_jobs,
             verbose=verbose,
         )
 
     def get_matching(self):
         return self.hungarian_match_12, self.hungarian_match_21
 
@@ -281,14 +285,15 @@
             gt_sorting,
             tested_sorting,
             sorting1_name=gt_name,
             sorting2_name=tested_name,
             delta_time=delta_time,
             match_score=match_score,
             chance_score=chance_score,
+            ensure_symmetry=False,
             n_jobs=n_jobs,
             verbose=verbose,
         )
         self.exhaustive_gt = exhaustive_gt
 
         self._compute_misclassifications = compute_misclassifications
         self.redundant_score = redundant_score
```

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/__init__.py` & `spikeinterface-0.99.1/src/spikeinterface/core/__init__.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/base.py` & `spikeinterface-0.99.1/src/spikeinterface/core/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -784,15 +784,15 @@
     def save_to_memory(self, **kwargs) -> "BaseExtractor":
         # used only by recording at the moment
         cached = self._save(**kwargs)
         self.copy_metadata(cached)
         return cached
 
     # TODO rename to saveto_binary_folder
-    def save_to_folder(self, name=None, folder=None, verbose=True, **save_kwargs):
+    def save_to_folder(self, name=None, folder=None, overwrite=False, verbose=True, **save_kwargs):
         """
         Save extractor to folder.
 
         The save consist of:
           * extracting traces by calling get_trace() method in chunks
           * saving data into file (memmap with BinaryRecordingExtractor)
           * dumping to json/pickle the original extractor for provenance
@@ -815,14 +815,16 @@
         ----------
         name: None str or Path
             Name of the subfolder in get_global_tmp_folder()
             If "name" is given, "folder" must be None.
         folder: None str or Path
             Name of the folder.
             If "folder" is given, "name" must be None.
+        overwrite: bool, default: False
+            If True, the folder is removed if it already exists
 
         Returns
         -------
         cached: saved copy of the extractor.
         """
 
         if folder is None:
@@ -835,15 +837,20 @@
             else:
                 folder = cache_folder / name
                 if not is_set_global_tmp_folder():
                     if verbose:
                         print(f"Use cache_folder={folder}")
         else:
             folder = Path(folder)
-        assert not folder.exists(), f"folder {folder} already exists, choose another name"
+        if overwrite and folder.is_dir():
+            import shutil
+
+            shutil.rmtree(folder)
+
+        assert not folder.exists(), f"folder {folder} already exists, choose another name or use overwrite=True"
         folder.mkdir(parents=True, exist_ok=False)
 
         # dump provenance
         provenance_file = folder / f"provenance.json"
         if self.check_serializablility("json"):
             self.dump(provenance_file)
         else:
```

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/baseevent.py` & `spikeinterface-0.99.1/src/spikeinterface/core/baseevent.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/baserecording.py` & `spikeinterface-0.99.1/src/spikeinterface/core/baserecording.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/baserecordingsnippets.py` & `spikeinterface-0.99.1/src/spikeinterface/core/baserecordingsnippets.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/basesnippets.py` & `spikeinterface-0.99.1/src/spikeinterface/core/basesnippets.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/basesorting.py` & `spikeinterface-0.99.1/src/spikeinterface/core/basesorting.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/binaryfolder.py` & `spikeinterface-0.99.1/src/spikeinterface/core/binaryfolder.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/binaryrecordingextractor.py` & `spikeinterface-0.99.1/src/spikeinterface/core/binaryrecordingextractor.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/channelsaggregationrecording.py` & `spikeinterface-0.99.1/src/spikeinterface/core/channelsaggregationrecording.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/channelslice.py` & `spikeinterface-0.99.1/src/spikeinterface/core/channelslice.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/core_tools.py` & `spikeinterface-0.99.1/src/spikeinterface/core/core_tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/datasets.py` & `spikeinterface-0.99.1/src/spikeinterface/core/datasets.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/frameslicerecording.py` & `spikeinterface-0.99.1/src/spikeinterface/core/frameslicerecording.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/frameslicesorting.py` & `spikeinterface-0.99.1/src/spikeinterface/core/frameslicesorting.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/generate.py` & `spikeinterface-0.99.1/src/spikeinterface/core/generate.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/globals.py` & `spikeinterface-0.99.1/src/spikeinterface/core/globals.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/job_tools.py` & `spikeinterface-0.99.1/src/spikeinterface/core/job_tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/node_pipeline.py` & `spikeinterface-0.99.1/src/spikeinterface/core/node_pipeline.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/npyfoldersnippets.py` & `spikeinterface-0.99.1/src/spikeinterface/core/npyfoldersnippets.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/npysnippetsextractor.py` & `spikeinterface-0.99.1/src/spikeinterface/core/npysnippetsextractor.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/npzsortingextractor.py` & `spikeinterface-0.99.1/src/spikeinterface/core/npzsortingextractor.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/numpyextractors.py` & `spikeinterface-0.99.1/src/spikeinterface/core/numpyextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/old_api_utils.py` & `spikeinterface-0.99.1/src/spikeinterface/core/old_api_utils.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/recording_tools.py` & `spikeinterface-0.99.1/src/spikeinterface/core/recording_tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/segmentutils.py` & `spikeinterface-0.99.1/src/spikeinterface/core/segmentutils.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/snippets_tools.py` & `spikeinterface-0.99.1/src/spikeinterface/core/snippets_tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/sortingfolder.py` & `spikeinterface-0.99.1/src/spikeinterface/core/sortingfolder.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/sparsity.py` & `spikeinterface-0.99.1/src/spikeinterface/core/sparsity.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/template_tools.py` & `spikeinterface-0.99.1/src/spikeinterface/core/template_tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/testing.py` & `spikeinterface-0.99.1/src/spikeinterface/core/testing.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/unitsaggregationsorting.py` & `spikeinterface-0.99.1/src/spikeinterface/core/unitsaggregationsorting.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/unitsselectionsorting.py` & `spikeinterface-0.99.1/src/spikeinterface/core/unitsselectionsorting.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/waveform_extractor.py` & `spikeinterface-0.99.1/src/spikeinterface/core/waveform_extractor.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/waveform_tools.py` & `spikeinterface-0.99.1/src/spikeinterface/core/waveform_tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/core/zarrrecordingextractor.py` & `spikeinterface-0.99.1/src/spikeinterface/core/zarrrecordingextractor.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/curation/__init__.py` & `spikeinterface-0.99.1/src/spikeinterface/curation/__init__.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/curation/auto_merge.py` & `spikeinterface-0.99.1/src/spikeinterface/curation/auto_merge.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/curation/curation_tools.py` & `spikeinterface-0.99.1/src/spikeinterface/curation/curation_tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/curation/curationsorting.py` & `spikeinterface-0.99.1/src/spikeinterface/curation/curationsorting.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/curation/mergeunitssorting.py` & `spikeinterface-0.99.1/src/spikeinterface/curation/mergeunitssorting.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/curation/remove_duplicated_spikes.py` & `spikeinterface-0.99.1/src/spikeinterface/curation/remove_duplicated_spikes.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/curation/remove_excess_spikes.py` & `spikeinterface-0.99.1/src/spikeinterface/curation/remove_excess_spikes.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/curation/remove_redundant.py` & `spikeinterface-0.99.1/src/spikeinterface/curation/remove_redundant.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/curation/sortingview_curation.py` & `spikeinterface-0.99.1/src/spikeinterface/curation/sortingview_curation.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/curation/splitunitsorting.py` & `spikeinterface-0.99.1/src/spikeinterface/curation/splitunitsorting.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/exporters/report.py` & `spikeinterface-0.99.1/src/spikeinterface/exporters/report.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/exporters/to_phy.py` & `spikeinterface-0.99.1/src/spikeinterface/exporters/to_phy.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/alfsortingextractor.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/alfsortingextractor.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/bids.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/bids.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/cbin_ibl.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/cbin_ibl.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/cellexplorersortingextractor.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/cellexplorersortingextractor.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/combinatoextractors.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/combinatoextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/extractorlist.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/extractorlist.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     NumpyRecording,
     NpzSortingExtractor,
     NumpySorting,
     NpySnippetsExtractor,
     ZarrRecordingExtractor,
     read_binary,
     read_zarr,
+    read_npz_sorting,
 )
 
 # sorting/recording/event from neo
 from .neoextractors import *
 
 # non-NEO objects implemented in neo folder
 from .neoextractors import NeuroScopeSortingExtractor, MaxwellEventExtractor
```

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/hdsortextractors.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/hdsortextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/herdingspikesextractors.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/herdingspikesextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/iblstreamingrecording.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/iblstreamingrecording.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/klustaextractors.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/klustaextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/matlabhelpers.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/matlabhelpers.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/mclustextractors.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/mclustextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/mcsh5extractors.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/mcsh5extractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/mdaextractors.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/mdaextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/__init__.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/__init__.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/alphaomega.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/alphaomega.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/axona.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/axona.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/biocam.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/biocam.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/blackrock.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/blackrock.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/ced.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/ced.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/edf.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/edf.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/intan.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/intan.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/maxwell.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/maxwell.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/mcsraw.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/mcsraw.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/mearec.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/mearec.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/neo_utils.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/neo_utils.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/neobaseextractor.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/neobaseextractor.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/neuralynx.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/neuralynx.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/neuroexplorer.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/neuroexplorer.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/neuroscope.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/neuroscope.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/nix.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/nix.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/openephys.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/openephys.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/plexon.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/plexon.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/plexon2.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/plexon2.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/spike2.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/spike2.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/spikegadgets.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/spikegadgets.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/spikeglx.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/spikeglx.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/neoextractors/tdt.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/neoextractors/tdt.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/neuropixels_utils.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/neuropixels_utils.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/nwbextractors.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/nwbextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/phykilosortextractors.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/phykilosortextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/shybridextractors.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/shybridextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/spykingcircusextractors.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/spykingcircusextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/toy_example.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/toy_example.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/tridesclousextractors.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/tridesclousextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/waveclussnippetstextractors.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/waveclussnippetstextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/waveclustextractors.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/waveclustextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/extractors/yassextractors.py` & `spikeinterface-0.99.1/src/spikeinterface/extractors/yassextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/full.py` & `spikeinterface-0.99.1/src/spikeinterface/full.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/postprocessing/__init__.py` & `spikeinterface-0.99.1/src/spikeinterface/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/postprocessing/alignsorting.py` & `spikeinterface-0.99.1/src/spikeinterface/postprocessing/alignsorting.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/postprocessing/amplitude_scalings.py` & `spikeinterface-0.99.1/src/spikeinterface/postprocessing/amplitude_scalings.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/postprocessing/correlograms.py` & `spikeinterface-0.99.1/src/spikeinterface/postprocessing/correlograms.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/postprocessing/isi.py` & `spikeinterface-0.99.1/src/spikeinterface/postprocessing/isi.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/postprocessing/noise_level.py` & `spikeinterface-0.99.1/src/spikeinterface/postprocessing/noise_level.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/postprocessing/principal_component.py` & `spikeinterface-0.99.1/src/spikeinterface/postprocessing/principal_component.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/postprocessing/spike_amplitudes.py` & `spikeinterface-0.99.1/src/spikeinterface/postprocessing/spike_amplitudes.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/postprocessing/spike_locations.py` & `spikeinterface-0.99.1/src/spikeinterface/postprocessing/spike_locations.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/postprocessing/template_metrics.py` & `spikeinterface-0.99.1/src/spikeinterface/postprocessing/template_metrics.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/postprocessing/template_similarity.py` & `spikeinterface-0.99.1/src/spikeinterface/postprocessing/template_similarity.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/postprocessing/unit_localization.py` & `spikeinterface-0.99.1/src/spikeinterface/postprocessing/unit_localization.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/preprocessing/align_snippets.py` & `spikeinterface-0.99.1/src/spikeinterface/preprocessing/align_snippets.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/preprocessing/astype.py` & `spikeinterface-0.99.1/src/spikeinterface/preprocessing/astype.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/preprocessing/average_across_direction.py` & `spikeinterface-0.99.1/src/spikeinterface/preprocessing/average_across_direction.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/preprocessing/basepreprocessor.py` & `spikeinterface-0.99.1/src/spikeinterface/preprocessing/basepreprocessor.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/preprocessing/clip.py` & `spikeinterface-0.99.1/src/spikeinterface/preprocessing/clip.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/preprocessing/common_reference.py` & `spikeinterface-0.99.1/src/spikeinterface/preprocessing/common_reference.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/preprocessing/correct_lsb.py` & `spikeinterface-0.99.1/src/spikeinterface/preprocessing/correct_lsb.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/preprocessing/deepinterpolation/deepinterpolation.py` & `spikeinterface-0.99.1/src/spikeinterface/preprocessing/deepinterpolation/deepinterpolation.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/preprocessing/deepinterpolation/generators.py` & `spikeinterface-0.99.1/src/spikeinterface/preprocessing/deepinterpolation/generators.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/preprocessing/deepinterpolation/tf_utils.py` & `spikeinterface-0.99.1/src/spikeinterface/preprocessing/deepinterpolation/tf_utils.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/preprocessing/deepinterpolation/train.py` & `spikeinterface-0.99.1/src/spikeinterface/preprocessing/deepinterpolation/train.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/preprocessing/depth_order.py` & `spikeinterface-0.99.1/src/spikeinterface/preprocessing/depth_order.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/preprocessing/detect_bad_channels.py` & `spikeinterface-0.99.1/src/spikeinterface/preprocessing/detect_bad_channels.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/preprocessing/directional_derivative.py` & `spikeinterface-0.99.1/src/spikeinterface/preprocessing/directional_derivative.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/preprocessing/filter.py` & `spikeinterface-0.99.1/src/spikeinterface/preprocessing/filter.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/preprocessing/filter_gaussian.py` & `spikeinterface-0.99.1/src/spikeinterface/preprocessing/filter_gaussian.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/preprocessing/filter_opencl.py` & `spikeinterface-0.99.1/src/spikeinterface/preprocessing/filter_opencl.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/preprocessing/highpass_spatial_filter.py` & `spikeinterface-0.99.1/src/spikeinterface/preprocessing/highpass_spatial_filter.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/preprocessing/interpolate_bad_channels.py` & `spikeinterface-0.99.1/src/spikeinterface/preprocessing/interpolate_bad_channels.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/preprocessing/motion.py` & `spikeinterface-0.99.1/src/spikeinterface/preprocessing/motion.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/preprocessing/normalize_scale.py` & `spikeinterface-0.99.1/src/spikeinterface/preprocessing/normalize_scale.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/preprocessing/phase_shift.py` & `spikeinterface-0.99.1/src/spikeinterface/preprocessing/phase_shift.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/preprocessing/preprocessing_tools.py` & `spikeinterface-0.99.1/src/spikeinterface/preprocessing/preprocessing_tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/preprocessing/preprocessinglist.py` & `spikeinterface-0.99.1/src/spikeinterface/preprocessing/preprocessinglist.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/preprocessing/rectify.py` & `spikeinterface-0.99.1/src/spikeinterface/preprocessing/rectify.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/preprocessing/remove_artifacts.py` & `spikeinterface-0.99.1/src/spikeinterface/preprocessing/remove_artifacts.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/preprocessing/resample.py` & `spikeinterface-0.99.1/src/spikeinterface/preprocessing/resample.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/preprocessing/silence_periods.py` & `spikeinterface-0.99.1/src/spikeinterface/preprocessing/silence_periods.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/preprocessing/unsigned_to_signed.py` & `spikeinterface-0.99.1/src/spikeinterface/preprocessing/unsigned_to_signed.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/preprocessing/whiten.py` & `spikeinterface-0.99.1/src/spikeinterface/preprocessing/whiten.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/preprocessing/zero_channel_pad.py` & `spikeinterface-0.99.1/src/spikeinterface/preprocessing/zero_channel_pad.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/qualitymetrics/misc_metrics.py` & `spikeinterface-0.99.1/src/spikeinterface/qualitymetrics/misc_metrics.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/qualitymetrics/pca_metrics.py` & `spikeinterface-0.99.1/src/spikeinterface/qualitymetrics/pca_metrics.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/qualitymetrics/quality_metric_calculator.py` & `spikeinterface-0.99.1/src/spikeinterface/qualitymetrics/quality_metric_calculator.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/qualitymetrics/quality_metric_list.py` & `spikeinterface-0.99.1/src/spikeinterface/qualitymetrics/quality_metric_list.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/qualitymetrics/utils.py` & `spikeinterface-0.99.1/src/spikeinterface/qualitymetrics/utils.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/basesorter.py` & `spikeinterface-0.99.1/src/spikeinterface/sorters/basesorter.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/external/combinato.py` & `spikeinterface-0.99.1/src/spikeinterface/sorters/external/combinato.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/external/hdsort.py` & `spikeinterface-0.99.1/src/spikeinterface/sorters/external/hdsort.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/external/hdsort_master.m` & `spikeinterface-0.99.1/src/spikeinterface/sorters/external/hdsort_master.m`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/external/herdingspikes.py` & `spikeinterface-0.99.1/src/spikeinterface/sorters/external/herdingspikes.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/external/ironclust.py` & `spikeinterface-0.99.1/src/spikeinterface/sorters/external/ironclust.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/external/kilosort.py` & `spikeinterface-0.99.1/src/spikeinterface/sorters/external/kilosort.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/external/kilosort2.py` & `spikeinterface-0.99.1/src/spikeinterface/sorters/external/kilosort2.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/external/kilosort2_5.py` & `spikeinterface-0.99.1/src/spikeinterface/sorters/external/kilosort2_5.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/external/kilosort2_5_master.m` & `spikeinterface-0.99.1/src/spikeinterface/sorters/external/kilosort2_5_master.m`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/external/kilosort2_master.m` & `spikeinterface-0.99.1/src/spikeinterface/sorters/external/kilosort2_master.m`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/external/kilosort3.py` & `spikeinterface-0.99.1/src/spikeinterface/sorters/external/kilosort3.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/external/kilosort3_master.m` & `spikeinterface-0.99.1/src/spikeinterface/sorters/external/kilosort3_master.m`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/external/kilosort_master.m` & `spikeinterface-0.99.1/src/spikeinterface/sorters/external/kilosort_master.m`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/external/kilosortbase.py` & `spikeinterface-0.99.1/src/spikeinterface/sorters/external/kilosortbase.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/external/klusta.py` & `spikeinterface-0.99.1/src/spikeinterface/sorters/external/klusta.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/external/klusta_config_default.prm` & `spikeinterface-0.99.1/src/spikeinterface/sorters/external/klusta_config_default.prm`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/external/mountainsort4.py` & `spikeinterface-0.99.1/src/spikeinterface/sorters/external/mountainsort4.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/external/mountainsort5.py` & `spikeinterface-0.99.1/src/spikeinterface/sorters/external/mountainsort5.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/external/pykilosort.py` & `spikeinterface-0.99.1/src/spikeinterface/sorters/external/pykilosort.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/external/sc_config_default.params` & `spikeinterface-0.99.1/src/spikeinterface/sorters/external/sc_config_default.params`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/external/spyking_circus.py` & `spikeinterface-0.99.1/src/spikeinterface/sorters/external/spyking_circus.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/external/tridesclous.py` & `spikeinterface-0.99.1/src/spikeinterface/sorters/external/tridesclous.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/external/waveclus.py` & `spikeinterface-0.99.1/src/spikeinterface/sorters/external/waveclus.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/external/waveclus_master.m` & `spikeinterface-0.99.1/src/spikeinterface/sorters/external/waveclus_master.m`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/external/waveclus_snippets.py` & `spikeinterface-0.99.1/src/spikeinterface/sorters/external/waveclus_snippets.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/external/waveclus_snippets_master.m` & `spikeinterface-0.99.1/src/spikeinterface/sorters/external/waveclus_snippets_master.m`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/external/yass.py` & `spikeinterface-0.99.1/src/spikeinterface/sorters/external/yass.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/external/yass_config_default.yaml` & `spikeinterface-0.99.1/src/spikeinterface/sorters/external/yass_config_default.yaml`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/internal/si_based.py` & `spikeinterface-0.99.1/src/spikeinterface/sorters/internal/si_based.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/internal/spyking_circus2.py` & `spikeinterface-0.99.1/src/spikeinterface/sorters/internal/spyking_circus2.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/internal/tridesclous2.py` & `spikeinterface-0.99.1/src/spikeinterface/sorters/internal/tridesclous2.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/launcher.py` & `spikeinterface-0.99.1/src/spikeinterface/sorters/launcher.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/runsorter.py` & `spikeinterface-0.99.1/src/spikeinterface/sorters/runsorter.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/sorterlist.py` & `spikeinterface-0.99.1/src/spikeinterface/sorters/sorterlist.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/utils/constructNPYheader.m` & `spikeinterface-0.99.1/src/spikeinterface/sorters/utils/constructNPYheader.m`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/utils/misc.py` & `spikeinterface-0.99.1/src/spikeinterface/sorters/utils/misc.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/utils/shellscript.py` & `spikeinterface-0.99.1/src/spikeinterface/sorters/utils/shellscript.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sorters/utils/writeNPY.m` & `spikeinterface-0.99.1/src/spikeinterface/sorters/utils/writeNPY.m`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/benchmark/benchmark_clustering.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_clustering.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/benchmark/benchmark_matching.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_matching.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/benchmark/benchmark_motion_estimation.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_motion_estimation.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/benchmark/benchmark_motion_interpolation.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_motion_interpolation.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/benchmark/benchmark_peak_localization.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_peak_localization.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/benchmark/benchmark_peak_selection.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_peak_selection.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/benchmark/benchmark_tools.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/circus.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/circus.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/clean.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/clean.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/clustering_tools.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/clustering_tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/isocut5.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/isocut5.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/main.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/main.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/merge.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/merge.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/method_list.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/method_list.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/position.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/position.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/position_and_features.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/position_and_features.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/position_and_pca.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/position_and_pca.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/position_ptp_scaled.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/position_ptp_scaled.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/random_projections.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/random_projections.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/sliding_hdbscan.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/sliding_hdbscan.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/sliding_nn.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/sliding_nn.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/split.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/split.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/tools.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/clustering/triage.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/clustering/triage.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/features_from_peaks.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/features_from_peaks.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/matching/circus.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/matching/circus.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/matching/main.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/matching/main.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/matching/naive.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/matching/naive.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/matching/tdc.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/matching/tdc.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/matching/wobble.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/matching/wobble.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/motion_estimation.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/motion_estimation.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/motion_interpolation.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/motion_interpolation.py`

 * *Files 1% similar despite different names*

```diff
@@ -382,21 +382,26 @@
 
     def get_traces(self, start_frame, end_frame, channel_indices):
         if self.time_vector is not None:
             raise NotImplementedError(
                 "time_vector for InterpolateMotionRecording do not work because temporal_bins start from 0"
             )
             # times = np.asarray(self.time_vector[start_frame:end_frame])
-        else:
-            times = np.arange((end_frame or self.get_num_samples()) - (start_frame or 0), dtype="float64")
-            times /= self.sampling_frequency
-            t0 = start_frame / self.sampling_frequency
-            # if self.t_start is not None:
-            #     t0 = t0 + self.t_start
-            times += t0
+
+        if start_frame is None:
+            start_frame = 0
+        if end_frame is None:
+            end_frame = self.get_num_samples()
+
+        times = np.arange(end_frame - start_frame, dtype="float64")
+        times /= self.sampling_frequency
+        t0 = start_frame / self.sampling_frequency
+        # if self.t_start is not None:
+        #     t0 = t0 + self.t_start
+        times += t0
 
         traces = self.parent_recording_segment.get_traces(start_frame, end_frame, channel_indices=slice(None))
 
         trace2 = interpolate_motion_on_traces(
             traces,
             times,
             self.channel_locations,
```

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/peak_detection.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/peak_detection.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/peak_localization.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/peak_localization.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/peak_pipeline.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/peak_pipeline.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/peak_selection.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/peak_selection.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/tools.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/waveforms/neural_network_denoiser.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/waveforms/neural_network_denoiser.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/waveforms/savgol_denoiser.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/waveforms/savgol_denoiser.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/waveforms/temporal_pca.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/waveforms/temporal_pca.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/waveforms/waveform_thresholder.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/waveforms/waveform_thresholder.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/sortingcomponents/waveforms/waveform_utils.py` & `spikeinterface-0.99.1/src/spikeinterface/sortingcomponents/waveforms/waveform_utils.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/all_amplitudes_distributions.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/all_amplitudes_distributions.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/amplitudes.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/amplitudes.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/autocorrelograms.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/autocorrelograms.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/base.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/base.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/collision.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/collision.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/comparison.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/comparison.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/crosscorrelograms.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/crosscorrelograms.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/gtstudy.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/gtstudy.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/isi_distribution.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/isi_distribution.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/metrics.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/metrics.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/motion.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/motion.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/multicomparison.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/multicomparison.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/peak_activity.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/peak_activity.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/probe_map.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/probe_map.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/quality_metrics.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/rasters.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/rasters.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/sorting_summary.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/sorting_summary.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/spike_locations.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/spike_locations.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/spikes_on_traces.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/spikes_on_traces.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/template_metrics.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/template_metrics.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/template_similarity.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/template_similarity.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/traces.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/traces.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/unit_depths.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/unit_depths.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/unit_locations.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/unit_locations.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/unit_presence.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/unit_presence.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/unit_probe_map.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/unit_probe_map.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/unit_summary.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/unit_summary.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/unit_templates.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/unit_templates.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/unit_waveforms.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/unit_waveforms.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/unit_waveforms_density_map.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/unit_waveforms_density_map.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/utils.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/utils_ipywidgets.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/utils_ipywidgets.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/utils_matplotlib.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/utils_matplotlib.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/utils_sortingview.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/utils_sortingview.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface/widgets/widget_list.py` & `spikeinterface-0.99.1/src/spikeinterface/widgets/widget_list.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface.egg-info/PKG-INFO` & `spikeinterface-0.99.1/src/spikeinterface.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spikeinterface
-Version: 0.99.0
+Version: 0.99.1
 Summary: Python toolkit for analysis, visualization, and comparison of spike sorting output
 Author-email: Alessio Buccino <alessiop.buccino@gmail.com>, Samuel Garcia <sam.garcia.die@gmail.com>
 Project-URL: homepage, https://github.com/SpikeInterface/spikeinterface
 Project-URL: repository, https://github.com/SpikeInterface/spikeinterface
 Project-URL: documentation, https://spikeinterface.readthedocs.io/
 Project-URL: changelog, https://spikeinterface.readthedocs.io/en/latest/whatisnew.html
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -158,15 +158,15 @@
 - export a report and/or export to phy
 - offer a powerful Qt-based viewer in a separate package [spikeinterface-gui](https://github.com/SpikeInterface/spikeinterface-gui)
 - have powerful sorting components to build your own sorter.
 
 
 ## Documentation
 
-Detailed documentation of the latest PyPI release of SpikeInterface can be found [here](https://spikeinterface.readthedocs.io/en/0.98.2).
+Detailed documentation of the latest PyPI release of SpikeInterface can be found [here](https://spikeinterface.readthedocs.io/en/0.99.1).
 
 Detailed documentation of the development version of SpikeInterface can be found [here](https://spikeinterface.readthedocs.io/en/latest).
 
 Several tutorials to get started can be found in [spiketutorials](https://github.com/SpikeInterface/spiketutorials).
 
 There are also some useful notebooks [on our blog](https://spikeinterface.github.io) that cover advanced benchmarking
 and sorting components.
```

### Comparing `spikeinterface-0.99.0/src/spikeinterface.egg-info/SOURCES.txt` & `spikeinterface-0.99.1/src/spikeinterface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.99.0/src/spikeinterface.egg-info/requires.txt` & `spikeinterface-0.99.1/src/spikeinterface.egg-info/requires.txt`

 * *Files identical despite different names*

