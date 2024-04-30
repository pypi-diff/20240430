# Comparing `tmp/neurodamus-3.2.0.tar.gz` & `tmp/neurodamus-3.2.1.tar.gz`

## Comparing `neurodamus-3.2.0.tar` & `neurodamus-3.2.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/__init__.py
--rw-r--r--   0        0        0    38362 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/cell_distributor.py
--rw-r--r--   0        0        0     9136 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/commands.py
--rw-r--r--   0        0        0    32924 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/connection.py
--rw-r--r--   0        0        0    57231 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/connection_manager.py
--rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/gap_junction.py
--rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/hocify.py
--rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/lfp_manager.py
--rw-r--r--   0        0        0    11984 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/metype.py
--rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/modification_manager.py
--rw-r--r--   0        0        0    14276 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/morphio_wrapper.py
--rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/neuromodulation_manager.py
--rw-r--r--   0        0        0    23499 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/ngv.py
--rw-r--r--   0        0        0    80992 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/node.py
--rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/replay.py
--rw-r--r--   0        0        0    11278 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/report.py
--rw-r--r--   0        0        0    28618 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/stimulus_manager.py
--rw-r--r--   0        0        0    25829 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/target_manager.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/core/__init__.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/core/_engine.py
--rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/core/_mpi.py
--rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/core/_neurodamus.py
--rw-r--r--   0        0        0     8136 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/core/_neuron.py
--rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/core/_shmutils.py
--rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/core/_utils.py
--rw-r--r--   0        0        0    14314 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/core/cell.py
--rw-r--r--   0        0        0    44943 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/core/configuration.py
--rw-r--r--   0        0        0     7805 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/core/coreneuron_configuration.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/core/mechanisms.py
--rw-r--r--   0        0        0    13978 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/core/nodeset.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/core/random.py
--rw-r--r--   0        0        0    19170 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/core/stimuli.py
--rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/core/synapses.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/init.py
--rw-r--r--   0        0        0    15774 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/hoc/Cell.hoc
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/hoc/ConnectionUtils.hoc
--rw-r--r--   0        0        0    10723 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/hoc/Map.hoc
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/hoc/MorphIO.hoc
--rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/hoc/RNGSettings.hoc
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/hoc/defvar.hoc
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/hoc/fileUtils.hoc
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/hoc/neurodamus.hoc
--rw-r--r--   0        0        0     8053 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/mod/ALU.mod
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/mod/CoreNEURONArtificialCell.mod
--rw-r--r--   0        0        0    45115 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/mod/HDF5reader.mod
--rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/mod/SonataReportHelper.mod
--rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/mod/SonataReports.mod
--rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/mod/VecStim.mod
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/mod/coreneuron_modlist.txt
--rw-r--r--   0        0        0    15160 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/data/mod/netstim_inhpoisson.mod
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/io/__init__.py
--rw-r--r--   0        0        0    13190 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/io/cell_readers.py
--rw-r--r--   0        0        0    19452 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/io/sonata_config.py
--rw-r--r--   0        0        0    15758 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/io/synapse_reader.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/utils/__init__.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/utils/cli.py
--rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/utils/compat.py
--rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/utils/logging.py
--rw-r--r--   0        0        0    21146 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/utils/memory.py
--rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/utils/multimap.py
--rw-r--r--   0        0        0     8587 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/utils/progressbar.py
--rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/utils/pyutils.py
--rw-r--r--   0        0        0    10745 2020-02-02 00:00:00.000000 neurodamus-3.2.0/neurodamus/utils/timeit.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 neurodamus-3.2.0/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 neurodamus-3.2.0/LICENSE.txt
--rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 neurodamus-3.2.0/README.rst
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 neurodamus-3.2.0/pyproject.toml
--rw-r--r--   0        0        0    18296 2020-02-02 00:00:00.000000 neurodamus-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/__init__.py
+-rw-r--r--   0        0        0    38362 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/cell_distributor.py
+-rw-r--r--   0        0        0     9136 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/commands.py
+-rw-r--r--   0        0        0    32924 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/connection.py
+-rw-r--r--   0        0        0    57231 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/connection_manager.py
+-rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/gap_junction.py
+-rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/hocify.py
+-rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/lfp_manager.py
+-rw-r--r--   0        0        0    11984 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/metype.py
+-rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/modification_manager.py
+-rw-r--r--   0        0        0    14276 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/morphio_wrapper.py
+-rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/neuromodulation_manager.py
+-rw-r--r--   0        0        0    23499 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/ngv.py
+-rw-r--r--   0        0        0    81050 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/node.py
+-rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/replay.py
+-rw-r--r--   0        0        0    11278 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/report.py
+-rw-r--r--   0        0        0    28618 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/stimulus_manager.py
+-rw-r--r--   0        0        0    25829 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/target_manager.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/core/__init__.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/core/_engine.py
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/core/_mpi.py
+-rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/core/_neurodamus.py
+-rw-r--r--   0        0        0     8136 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/core/_neuron.py
+-rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/core/_shmutils.py
+-rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/core/_utils.py
+-rw-r--r--   0        0        0    14314 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/core/cell.py
+-rw-r--r--   0        0        0    44943 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/core/configuration.py
+-rw-r--r--   0        0        0     7805 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/core/coreneuron_configuration.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/core/mechanisms.py
+-rw-r--r--   0        0        0    13978 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/core/nodeset.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/core/random.py
+-rw-r--r--   0        0        0    19170 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/core/stimuli.py
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/core/synapses.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/init.py
+-rw-r--r--   0        0        0    15774 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/hoc/Cell.hoc
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/hoc/ConnectionUtils.hoc
+-rw-r--r--   0        0        0    10723 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/hoc/Map.hoc
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/hoc/MorphIO.hoc
+-rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/hoc/RNGSettings.hoc
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/hoc/defvar.hoc
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/hoc/fileUtils.hoc
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/hoc/neurodamus.hoc
+-rw-r--r--   0        0        0     8053 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/mod/ALU.mod
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/mod/CoreNEURONArtificialCell.mod
+-rw-r--r--   0        0        0    45115 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/mod/HDF5reader.mod
+-rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/mod/SonataReportHelper.mod
+-rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/mod/SonataReports.mod
+-rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/mod/VecStim.mod
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/mod/coreneuron_modlist.txt
+-rw-r--r--   0        0        0    15160 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/data/mod/netstim_inhpoisson.mod
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/io/__init__.py
+-rw-r--r--   0        0        0    13190 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/io/cell_readers.py
+-rw-r--r--   0        0        0    19452 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/io/sonata_config.py
+-rw-r--r--   0        0        0    15758 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/io/synapse_reader.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/utils/__init__.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/utils/cli.py
+-rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/utils/compat.py
+-rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/utils/logging.py
+-rw-r--r--   0        0        0    21146 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/utils/memory.py
+-rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/utils/multimap.py
+-rw-r--r--   0        0        0     8587 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/utils/progressbar.py
+-rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/utils/pyutils.py
+-rw-r--r--   0        0        0    10745 2020-02-02 00:00:00.000000 neurodamus-3.2.1/neurodamus/utils/timeit.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 neurodamus-3.2.1/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 neurodamus-3.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 neurodamus-3.2.1/README.rst
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 neurodamus-3.2.1/pyproject.toml
+-rw-r--r--   0        0        0    18296 2020-02-02 00:00:00.000000 neurodamus-3.2.1/PKG-INFO
```

### Comparing `neurodamus-3.2.0/neurodamus/__init__.py` & `neurodamus-3.2.1/neurodamus/__init__.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/cell_distributor.py` & `neurodamus-3.2.1/neurodamus/cell_distributor.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/commands.py` & `neurodamus-3.2.1/neurodamus/commands.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/connection.py` & `neurodamus-3.2.1/neurodamus/connection.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/connection_manager.py` & `neurodamus-3.2.1/neurodamus/connection_manager.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/gap_junction.py` & `neurodamus-3.2.1/neurodamus/gap_junction.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/hocify.py` & `neurodamus-3.2.1/neurodamus/hocify.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/lfp_manager.py` & `neurodamus-3.2.1/neurodamus/lfp_manager.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/metype.py` & `neurodamus-3.2.1/neurodamus/metype.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/modification_manager.py` & `neurodamus-3.2.1/neurodamus/modification_manager.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/morphio_wrapper.py` & `neurodamus-3.2.1/neurodamus/morphio_wrapper.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/neuromodulation_manager.py` & `neurodamus-3.2.1/neurodamus/neuromodulation_manager.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/ngv.py` & `neurodamus-3.2.1/neurodamus/ngv.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/node.py` & `neurodamus-3.2.1/neurodamus/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -820,15 +820,15 @@
     # @mpi_no_errors - not required since theres a call inside before make_comm()
     @timeit(name="Enable Reports")
     def enable_reports(self):
         """Iterate over reports defined in the config file and instantiate them.
         """
         log_stage("Reports Enabling")
         n_errors = 0
-        reports_conf = SimConfig.reports
+        reports_conf = {name: conf for name, conf in SimConfig.reports.items() if conf["Enabled"]}
         self._report_list = []
 
         # Create a map of offsets so that it can be used even on coreneuron save-restore
         if self._circuits.initialized():
             self._circuits.write_population_offsets()
             pop_offsets_alias = self._circuits.get_population_offsets()
         else:
```

### Comparing `neurodamus-3.2.0/neurodamus/replay.py` & `neurodamus-3.2.1/neurodamus/replay.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/report.py` & `neurodamus-3.2.1/neurodamus/report.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/stimulus_manager.py` & `neurodamus-3.2.1/neurodamus/stimulus_manager.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/target_manager.py` & `neurodamus-3.2.1/neurodamus/target_manager.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/core/__init__.py` & `neurodamus-3.2.1/neurodamus/core/__init__.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/core/_engine.py` & `neurodamus-3.2.1/neurodamus/core/_engine.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/core/_mpi.py` & `neurodamus-3.2.1/neurodamus/core/_mpi.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/core/_neurodamus.py` & `neurodamus-3.2.1/neurodamus/core/_neurodamus.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/core/_neuron.py` & `neurodamus-3.2.1/neurodamus/core/_neuron.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/core/_shmutils.py` & `neurodamus-3.2.1/neurodamus/core/_shmutils.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/core/_utils.py` & `neurodamus-3.2.1/neurodamus/core/_utils.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/core/cell.py` & `neurodamus-3.2.1/neurodamus/core/cell.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/core/configuration.py` & `neurodamus-3.2.1/neurodamus/core/configuration.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/core/coreneuron_configuration.py` & `neurodamus-3.2.1/neurodamus/core/coreneuron_configuration.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/core/mechanisms.py` & `neurodamus-3.2.1/neurodamus/core/mechanisms.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/core/nodeset.py` & `neurodamus-3.2.1/neurodamus/core/nodeset.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/core/random.py` & `neurodamus-3.2.1/neurodamus/core/random.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/core/stimuli.py` & `neurodamus-3.2.1/neurodamus/core/stimuli.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/core/synapses.py` & `neurodamus-3.2.1/neurodamus/core/synapses.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/data/init.py` & `neurodamus-3.2.1/neurodamus/data/init.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/data/hoc/Cell.hoc` & `neurodamus-3.2.1/neurodamus/data/hoc/Cell.hoc`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/data/hoc/ConnectionUtils.hoc` & `neurodamus-3.2.1/neurodamus/data/hoc/ConnectionUtils.hoc`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/data/hoc/Map.hoc` & `neurodamus-3.2.1/neurodamus/data/hoc/Map.hoc`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/data/hoc/MorphIO.hoc` & `neurodamus-3.2.1/neurodamus/data/hoc/MorphIO.hoc`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/data/hoc/RNGSettings.hoc` & `neurodamus-3.2.1/neurodamus/data/hoc/RNGSettings.hoc`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/data/hoc/defvar.hoc` & `neurodamus-3.2.1/neurodamus/data/hoc/defvar.hoc`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/data/hoc/fileUtils.hoc` & `neurodamus-3.2.1/neurodamus/data/hoc/fileUtils.hoc`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/data/mod/ALU.mod` & `neurodamus-3.2.1/neurodamus/data/mod/ALU.mod`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/data/mod/HDF5reader.mod` & `neurodamus-3.2.1/neurodamus/data/mod/HDF5reader.mod`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/data/mod/SonataReportHelper.mod` & `neurodamus-3.2.1/neurodamus/data/mod/SonataReportHelper.mod`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/data/mod/SonataReports.mod` & `neurodamus-3.2.1/neurodamus/data/mod/SonataReports.mod`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/data/mod/VecStim.mod` & `neurodamus-3.2.1/neurodamus/data/mod/VecStim.mod`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/data/mod/netstim_inhpoisson.mod` & `neurodamus-3.2.1/neurodamus/data/mod/netstim_inhpoisson.mod`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/io/cell_readers.py` & `neurodamus-3.2.1/neurodamus/io/cell_readers.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/io/sonata_config.py` & `neurodamus-3.2.1/neurodamus/io/sonata_config.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/io/synapse_reader.py` & `neurodamus-3.2.1/neurodamus/io/synapse_reader.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/utils/cli.py` & `neurodamus-3.2.1/neurodamus/utils/cli.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/utils/compat.py` & `neurodamus-3.2.1/neurodamus/utils/compat.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/utils/logging.py` & `neurodamus-3.2.1/neurodamus/utils/logging.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/utils/memory.py` & `neurodamus-3.2.1/neurodamus/utils/memory.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/utils/multimap.py` & `neurodamus-3.2.1/neurodamus/utils/multimap.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/utils/progressbar.py` & `neurodamus-3.2.1/neurodamus/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/utils/pyutils.py` & `neurodamus-3.2.1/neurodamus/utils/pyutils.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/neurodamus/utils/timeit.py` & `neurodamus-3.2.1/neurodamus/utils/timeit.py`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/LICENSE.txt` & `neurodamus-3.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/README.rst` & `neurodamus-3.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/pyproject.toml` & `neurodamus-3.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `neurodamus-3.2.0/PKG-INFO` & `neurodamus-3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: neurodamus
-Version: 3.2.0
+Version: 3.2.1
 Summary: A BBP Simulation Control application for NEURON
 Project-URL: Homepage, https://github.com/BlueBrain/neurodamus
 Project-URL: Repository, https://github.com/BlueBrain/neurodamus.git
 Project-URL: Tracker, https://github.com/BlueBrain/neurodamus/issues
 Author: Blue Brain Project, EPFL
 License:                                  Apache License
                                    Version 2.0, January 2004
```

