# Comparing `tmp/pyiron_base-0.8.2.tar.gz` & `tmp/pyiron_base-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron_base-0.8.2.tar", last modified: Wed Apr 17 17:00:59 2024, max compression
+gzip compressed data, was "pyiron_base-0.8.3.tar", last modified: Tue Apr 30 13:32:13 2024, max compression
```

## Comparing `pyiron_base-0.8.2.tar` & `pyiron_base-0.8.3.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.565263 pyiron_base-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-04-17 17:00:59.565263 pyiron_base-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.545263 pyiron_base-0.8.2/pyiron_base/
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-17 17:00:59.565263 pyiron_base-0.8.2/pyiron_base/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.549263 pyiron_base-0.8.2/pyiron_base/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/cli/control.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/cli/install.py
--rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/cli/ls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/cli/reloadfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/cli/rm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/cli/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.549263 pyiron_base-0.8.2/pyiron_base/database/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24876 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/database/filetable.py
--rw-r--r--   0 runner    (1001) docker     (127)    36818 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/database/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)    12190 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/database/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/database/jobtable.py
--rw-r--r--   0 runner    (1001) docker     (127)     8633 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/database/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/database/performance.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/database/sqlcolumnlength.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/database/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.549263 pyiron_base-0.8.2/pyiron_base/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/interfaces/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/interfaces/has_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/interfaces/has_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/interfaces/has_hdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    11046 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/interfaces/lockable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/interfaces/object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/interfaces/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.549263 pyiron_base-0.8.2/pyiron_base/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29296 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/datamining.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/dynamic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.553263 pyiron_base-0.8.2/pyiron_base/jobs/flex/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/flex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/flex/executablecontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/flex/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/flex/pythonfunctioncontainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.553263 pyiron_base-0.8.2/pyiron_base/jobs/job/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39577 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.553263 pyiron_base-0.8.2/pyiron_base/jobs/job/extension/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10855 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/extension/executable.py
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/extension/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     9605 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/extension/jobstatus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.553263 pyiron_base-0.8.2/pyiron_base/jobs/job/extension/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/extension/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22428 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/extension/server/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)    14687 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/extension/server/queuestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/extension/server/runmode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    61239 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)    13333 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)    11683 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/jobtype.py
--rw-r--r--   0 runner    (1001) docker     (127)    11822 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/path.py
--rw-r--r--   0 runner    (1001) docker     (127)    29036 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/runfunction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/template.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/toolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)    19730 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/job/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.557263 pyiron_base-0.8.2/pyiron_base/jobs/master/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/master/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/master/flexible.py
--rw-r--r--   0 runner    (1001) docker     (127)    16926 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/master/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/master/interactivewrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9365 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/master/list.py
--rw-r--r--   0 runner    (1001) docker     (127)    32984 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/master/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8168 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/master/submissionstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)    15209 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/script.py
--rw-r--r--   0 runner    (1001) docker     (127)    14687 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/jobs/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.557263 pyiron_base-0.8.2/pyiron_base/project/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.557263 pyiron_base-0.8.2/pyiron_base/project/archiving/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/archiving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/archiving/export_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/archiving/import_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/archiving/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/condaenv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/external.py
--rw-r--r--   0 runner    (1001) docker     (127)    74335 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     9360 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/jobloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/maintenance.py
--rw-r--r--   0 runner    (1001) docker     (127)    13268 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/size.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.557263 pyiron_base-0.8.2/pyiron_base/project/update/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/project/update/pyiron_base_03x_to_04x.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.561263 pyiron_base-0.8.2/pyiron_base/state/
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/state/install.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/state/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/state/publications.py
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/state/queue_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    25130 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/state/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/state/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/state/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.561263 pyiron_base-0.8.2/pyiron_base/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34122 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/storage/datacontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/storage/filedata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/storage/fileio.py
--rw-r--r--   0 runner    (1001) docker     (127)    43875 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/storage/flattenedstorage.py
--rw-r--r--   0 runner    (1001) docker     (127)    14165 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/storage/has_stored_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)    49006 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/storage/hdfio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/storage/hdfstub.py
--rw-r--r--   0 runner    (1001) docker     (127)     6527 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/storage/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/storage/inputlist.py
--rw-r--r--   0 runner    (1001) docker     (127)    33000 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/storage/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.561263 pyiron_base-0.8.2/pyiron_base/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/utils/deprecate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/utils/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/utils/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/utils/jedi.py
--rw-r--r--   0 runner    (1001) docker     (127)    29090 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/utils/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/utils/safetar.py
--rw-r--r--   0 runner    (1001) docker     (127)    14338 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/pyiron_base/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.565263 pyiron_base-0.8.2/pyiron_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-04-17 17:00:59.000000 pyiron_base-0.8.2/pyiron_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-17 17:00:59.000000 pyiron_base-0.8.2/pyiron_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 17:00:59.000000 pyiron_base-0.8.2/pyiron_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-17 17:00:59.000000 pyiron_base-0.8.2/pyiron_base.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-17 17:00:59.000000 pyiron_base-0.8.2/pyiron_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 17:00:59.000000 pyiron_base-0.8.2/pyiron_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-17 17:00:57.000000 pyiron_base-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 17:00:59.565263 pyiron_base-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 17:00:59.561263 pyiron_base-0.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/tests/test_testwithproject.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-17 17:00:08.000000 pyiron_base-0.8.2/tests/test_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.517540 pyiron_base-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-04-30 13:32:13.517540 pyiron_base-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.497539 pyiron_base-0.8.3/pyiron_base/
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-30 13:32:13.517540 pyiron_base-0.8.3/pyiron_base/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.497539 pyiron_base-0.8.3/pyiron_base/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/cli/control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/cli/ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/cli/reloadfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/cli/rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/cli/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.501539 pyiron_base-0.8.3/pyiron_base/database/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24876 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/database/filetable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36818 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/database/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12190 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/database/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/database/jobtable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8633 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/database/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/database/performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/database/sqlcolumnlength.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/database/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.501539 pyiron_base-0.8.3/pyiron_base/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/interfaces/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/interfaces/has_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/interfaces/has_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/interfaces/has_hdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11046 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/interfaces/lockable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/interfaces/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/interfaces/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.501539 pyiron_base-0.8.3/pyiron_base/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29278 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/datamining.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.501539 pyiron_base-0.8.3/pyiron_base/jobs/flex/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/flex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/flex/executablecontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/flex/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/flex/pythonfunctioncontainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.505539 pyiron_base-0.8.3/pyiron_base/jobs/job/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39577 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.505539 pyiron_base-0.8.3/pyiron_base/jobs/job/extension/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10855 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/extension/executable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/extension/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9605 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/extension/jobstatus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.505539 pyiron_base-0.8.3/pyiron_base/jobs/job/extension/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/extension/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22428 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/extension/server/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14687 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/extension/server/queuestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/extension/server/runmode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61634 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13333 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11683 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/jobtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11822 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29036 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/runfunction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19730 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/job/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.505539 pyiron_base-0.8.3/pyiron_base/jobs/master/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/master/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/master/flexible.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16926 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/master/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/master/interactivewrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9365 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/master/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32984 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/master/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8168 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/master/submissionstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15209 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14687 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/jobs/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.509539 pyiron_base-0.8.3/pyiron_base/project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.509539 pyiron_base-0.8.3/pyiron_base/project/archiving/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/archiving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/archiving/export_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/archiving/import_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/archiving/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/condaenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74335 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9360 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/jobloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13268 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/size.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.509539 pyiron_base-0.8.3/pyiron_base/project/update/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/project/update/pyiron_base_03x_to_04x.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.513539 pyiron_base-0.8.3/pyiron_base/state/
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/state/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/state/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/state/publications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/state/queue_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25130 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/state/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/state/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/state/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.513539 pyiron_base-0.8.3/pyiron_base/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34122 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/storage/datacontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/storage/filedata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/storage/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43875 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/storage/flattenedstorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14165 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/storage/has_stored_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49006 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/storage/hdfio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/storage/hdfstub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6527 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/storage/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/storage/inputlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33000 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/storage/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.513539 pyiron_base-0.8.3/pyiron_base/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/utils/deprecate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/utils/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/utils/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/utils/jedi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29090 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/utils/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/utils/safetar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14338 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/pyiron_base/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.517540 pyiron_base-0.8.3/pyiron_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-04-30 13:32:13.000000 pyiron_base-0.8.3/pyiron_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-30 13:32:13.000000 pyiron_base-0.8.3/pyiron_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:32:13.000000 pyiron_base-0.8.3/pyiron_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-30 13:32:13.000000 pyiron_base-0.8.3/pyiron_base.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-30 13:32:13.000000 pyiron_base-0.8.3/pyiron_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 13:32:13.000000 pyiron_base-0.8.3/pyiron_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-30 13:32:11.000000 pyiron_base-0.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 13:32:13.517540 pyiron_base-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:32:13.513539 pyiron_base-0.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/tests/test_testwithproject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-30 13:31:19.000000 pyiron_base-0.8.3/tests/test_toolkit.py
```

### Comparing `pyiron_base-0.8.2/LICENSE` & `pyiron_base-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/PKG-INFO` & `pyiron_base-0.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_base
-Version: 0.8.2
+Version: 0.8.3
 Summary: Core components of the pyiron integrated development environment (IDE) for computational materials science
 Author-email: "Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department" <pyiron@mpie.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2018, Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
         All rights reserved.
         
@@ -51,25 +51,25 @@
 License-File: LICENSE
 Requires-Dist: cloudpickle<=3.0.0,>=2.0.0
 Requires-Dist: gitpython<=3.1.43,>=3.1.23
 Requires-Dist: h5io_browser<=0.0.12,>=0.0.6
 Requires-Dist: h5py<=3.11.0,>=3.6.0
 Requires-Dist: jinja2<=3.1.3,>=2.11.3
 Requires-Dist: numpy<=1.26.4,>=1.23.5
-Requires-Dist: monty<=2024.3.31,>=2021.3.3
+Requires-Dist: monty<=2024.4.17,>=2021.3.3
 Requires-Dist: pandas<=2.2.2,>=2.0.0
 Requires-Dist: pint<=0.23,>=0.18
 Requires-Dist: psutil<=5.9.8,>=5.8.0
 Requires-Dist: pyfileindex<=0.0.24,>=0.0.16
-Requires-Dist: pympipool<=0.7.17,>=0.7.11
-Requires-Dist: pysqa<=0.1.18,>=0.1.12
+Requires-Dist: pympipool<=0.8.1,>=0.8.0
+Requires-Dist: pysqa<=0.1.19,>=0.1.12
 Requires-Dist: sqlalchemy<=2.0.29,>=2.0.22
 Requires-Dist: tables<=3.9.2,>=3.6.1
 Requires-Dist: tqdm<=4.66.2,>=4.44.0
-Requires-Dist: traitlets<=5.14.2,>=5.1.1
+Requires-Dist: traitlets<=5.14.3,>=5.1.1
 Provides-Extra: conda
 Requires-Dist: conda==23.11.0; extra == "conda"
 Requires-Dist: conda_subprocess==0.0.1; extra == "conda"
 
 pyiron
 ======
```

### Comparing `pyiron_base-0.8.2/README.rst` & `pyiron_base-0.8.3/README.rst`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/__init__.py` & `pyiron_base-0.8.3/pyiron_base/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/_tests.py` & `pyiron_base-0.8.3/pyiron_base/_tests.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/cli/control.py` & `pyiron_base-0.8.3/pyiron_base/cli/control.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/cli/install.py` & `pyiron_base-0.8.3/pyiron_base/cli/install.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/cli/ls.py` & `pyiron_base-0.8.3/pyiron_base/cli/ls.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/cli/reloadfile.py` & `pyiron_base-0.8.3/pyiron_base/cli/reloadfile.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/cli/rm.py` & `pyiron_base-0.8.3/pyiron_base/cli/rm.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/cli/wrapper.py` & `pyiron_base-0.8.3/pyiron_base/cli/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/database/filetable.py` & `pyiron_base-0.8.3/pyiron_base/database/filetable.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/database/generic.py` & `pyiron_base-0.8.3/pyiron_base/database/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/database/interface.py` & `pyiron_base-0.8.3/pyiron_base/database/interface.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/database/jobtable.py` & `pyiron_base-0.8.3/pyiron_base/database/jobtable.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/database/manager.py` & `pyiron_base-0.8.3/pyiron_base/database/manager.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/database/performance.py` & `pyiron_base-0.8.3/pyiron_base/database/performance.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/database/tables.py` & `pyiron_base-0.8.3/pyiron_base/database/tables.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/interfaces/factory.py` & `pyiron_base-0.8.3/pyiron_base/interfaces/factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/interfaces/has_dict.py` & `pyiron_base-0.8.3/pyiron_base/interfaces/has_dict.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/interfaces/has_groups.py` & `pyiron_base-0.8.3/pyiron_base/interfaces/has_groups.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/interfaces/has_hdf.py` & `pyiron_base-0.8.3/pyiron_base/interfaces/has_hdf.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/interfaces/lockable.py` & `pyiron_base-0.8.3/pyiron_base/interfaces/lockable.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/interfaces/object.py` & `pyiron_base-0.8.3/pyiron_base/interfaces/object.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/interfaces/singleton.py` & `pyiron_base-0.8.3/pyiron_base/interfaces/singleton.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/jobs/datamining.py` & `pyiron_base-0.8.3/pyiron_base/jobs/datamining.py`

 * *Files 0% similar despite different names*

```diff
@@ -782,15 +782,15 @@
         """
         if job_status_list is None:
             job_status_list = self.job_status
         if self.job_id is not None:
             self.project.db.item_update({"timestart": datetime.now()}, self.job_id)
         with self.project_hdf5.open("input") as hdf5_input:
             if self._executor_type is None and self.server.cores > 1:
-                self._executor_type = "pympipool.mpi.executor.PyMPIExecutor"
+                self._executor_type = "pympipool.Executor"
             if self._executor_type is not None:
                 with self._get_executor(max_workers=self.server.cores) as exe:
                     self._pyiron_table.create_table(
                         file=hdf5_input,
                         job_status_list=job_status_list,
                         enforce_update=self._enforce_update,
                         executor=exe,
```

### Comparing `pyiron_base-0.8.2/pyiron_base/jobs/dynamic.py` & `pyiron_base-0.8.3/pyiron_base/jobs/dynamic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/jobs/flex/executablecontainer.py` & `pyiron_base-0.8.3/pyiron_base/jobs/flex/executablecontainer.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/jobs/flex/factory.py` & `pyiron_base-0.8.3/pyiron_base/jobs/flex/factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/jobs/flex/pythonfunctioncontainer.py` & `pyiron_base-0.8.3/pyiron_base/jobs/flex/pythonfunctioncontainer.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/jobs/job/core.py` & `pyiron_base-0.8.3/pyiron_base/jobs/job/core.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/jobs/job/extension/executable.py` & `pyiron_base-0.8.3/pyiron_base/jobs/job/extension/executable.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/jobs/job/extension/files.py` & `pyiron_base-0.8.3/pyiron_base/jobs/job/extension/files.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/jobs/job/extension/jobstatus.py` & `pyiron_base-0.8.3/pyiron_base/jobs/job/extension/jobstatus.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/jobs/job/extension/server/generic.py` & `pyiron_base-0.8.3/pyiron_base/jobs/job/extension/server/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/jobs/job/extension/server/queuestatus.py` & `pyiron_base-0.8.3/pyiron_base/jobs/job/extension/server/queuestatus.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/jobs/job/extension/server/runmode.py` & `pyiron_base-0.8.3/pyiron_base/jobs/job/extension/server/runmode.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/jobs/job/factory.py` & `pyiron_base-0.8.3/pyiron_base/jobs/job/factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/jobs/job/generic.py` & `pyiron_base-0.8.3/pyiron_base/jobs/job/generic.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         self._exclude_groups_hdf = list()
         self._executor_type = None
         self._process = None
         self._compress_by_default = False
         self._python_only_job = False
         self._write_work_dir_warnings = True
         self.interactive_cache = None
-        self.error = GenericError(job=self)
+        self.error = GenericError(working_directory=self.project_hdf5.working_directory)
 
     @property
     def version(self):
         """
         Get the version of the hamiltonian, which is also the version of the executable unless a custom executable is
         used.
 
@@ -1548,30 +1548,33 @@
 
     def _get_executor(self, max_workers=None):
         if self._executor_type is None:
             raise ValueError(
                 "No executor type defined - Please set self.executor_type."
             )
         elif (
-            self._executor_type == "pympipool.mpi.executor.PyMPIExecutor"
+            self._executor_type == "pympipool.Executor"
             and platform.system() == "Darwin"
         ):
             # The Mac firewall might prevent connections based on the network address - especially Github CI
             return import_class(self._executor_type)(
-                max_workers=max_workers, hostname_localhost=True
+                max_cores=max_workers, hostname_localhost=True
             )
+        elif self._executor_type == "pympipool.Executor":
+            # The pympipool Executor defines max_cores rather than max_workers
+            return import_class(self._executor_type)(max_cores=max_workers)
         elif isinstance(self._executor_type, str):
             return import_class(self._executor_type)(max_workers=max_workers)
         else:
             raise TypeError("The self.executor_type has to be a string.")
 
 
 class GenericError(object):
-    def __init__(self, job):
-        self._job = job
+    def __init__(self, working_directory):
+        self._working_directory = working_directory
 
     def __repr__(self):
         all_messages = ""
         for message in [self.print_message(), self.print_queue()]:
             if message is True:
                 all_messages += message
         if len(all_messages) == 0:
@@ -1581,11 +1584,12 @@
     def print_message(self, string=""):
         return self._print_error(file_name="error.msg", string=string)
 
     def print_queue(self, string=""):
         return self._print_error(file_name="error.out", string=string)
 
     def _print_error(self, file_name, string="", print_yes=True):
-        if self._job[file_name] is None:
+        if not os.path.exists(os.path.join(self._working_directory, file_name)):
             return ""
         elif print_yes:
-            return string.join(self._job[file_name])
+            with open(os.path.join(self._working_directory, file_name)) as f:
+                return string.join(f.readlines())
```

### Comparing `pyiron_base-0.8.2/pyiron_base/jobs/job/interactive.py` & `pyiron_base-0.8.3/pyiron_base/jobs/job/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/jobs/job/jobtype.py` & `pyiron_base-0.8.3/pyiron_base/jobs/job/jobtype.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/jobs/job/path.py` & `pyiron_base-0.8.3/pyiron_base/jobs/job/path.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/jobs/job/runfunction.py` & `pyiron_base-0.8.3/pyiron_base/jobs/job/runfunction.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/jobs/job/template.py` & `pyiron_base-0.8.3/pyiron_base/jobs/job/template.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/jobs/job/toolkit.py` & `pyiron_base-0.8.3/pyiron_base/jobs/job/toolkit.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/jobs/job/util.py` & `pyiron_base-0.8.3/pyiron_base/jobs/job/util.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/jobs/job/wrapper.py` & `pyiron_base-0.8.3/pyiron_base/jobs/job/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/jobs/master/flexible.py` & `pyiron_base-0.8.3/pyiron_base/jobs/master/flexible.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/jobs/master/generic.py` & `pyiron_base-0.8.3/pyiron_base/jobs/master/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/jobs/master/interactivewrapper.py` & `pyiron_base-0.8.3/pyiron_base/jobs/master/interactivewrapper.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/jobs/master/list.py` & `pyiron_base-0.8.3/pyiron_base/jobs/master/list.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/jobs/master/parallel.py` & `pyiron_base-0.8.3/pyiron_base/jobs/master/parallel.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/jobs/master/submissionstatus.py` & `pyiron_base-0.8.3/pyiron_base/jobs/master/submissionstatus.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/jobs/script.py` & `pyiron_base-0.8.3/pyiron_base/jobs/script.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/jobs/worker.py` & `pyiron_base-0.8.3/pyiron_base/jobs/worker.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/project/archiving/export_archive.py` & `pyiron_base-0.8.3/pyiron_base/project/archiving/export_archive.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/project/archiving/import_archive.py` & `pyiron_base-0.8.3/pyiron_base/project/archiving/import_archive.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/project/condaenv.py` & `pyiron_base-0.8.3/pyiron_base/project/condaenv.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/project/data.py` & `pyiron_base-0.8.3/pyiron_base/project/data.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/project/external.py` & `pyiron_base-0.8.3/pyiron_base/project/external.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/project/generic.py` & `pyiron_base-0.8.3/pyiron_base/project/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/project/gui.py` & `pyiron_base-0.8.3/pyiron_base/project/gui.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/project/jobloader.py` & `pyiron_base-0.8.3/pyiron_base/project/jobloader.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/project/maintenance.py` & `pyiron_base-0.8.3/pyiron_base/project/maintenance.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/project/path.py` & `pyiron_base-0.8.3/pyiron_base/project/path.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/project/size.py` & `pyiron_base-0.8.3/pyiron_base/project/size.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/project/update/pyiron_base_03x_to_04x.py` & `pyiron_base-0.8.3/pyiron_base/project/update/pyiron_base_03x_to_04x.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/state/__init__.py` & `pyiron_base-0.8.3/pyiron_base/state/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/state/install.py` & `pyiron_base-0.8.3/pyiron_base/state/install.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/state/logger.py` & `pyiron_base-0.8.3/pyiron_base/state/logger.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/state/publications.py` & `pyiron_base-0.8.3/pyiron_base/state/publications.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/state/queue_adapter.py` & `pyiron_base-0.8.3/pyiron_base/state/queue_adapter.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/state/settings.py` & `pyiron_base-0.8.3/pyiron_base/state/settings.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/state/signal.py` & `pyiron_base-0.8.3/pyiron_base/state/signal.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/state/update.py` & `pyiron_base-0.8.3/pyiron_base/state/update.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/storage/datacontainer.py` & `pyiron_base-0.8.3/pyiron_base/storage/datacontainer.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/storage/filedata.py` & `pyiron_base-0.8.3/pyiron_base/storage/filedata.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/storage/fileio.py` & `pyiron_base-0.8.3/pyiron_base/storage/fileio.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/storage/flattenedstorage.py` & `pyiron_base-0.8.3/pyiron_base/storage/flattenedstorage.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/storage/has_stored_traits.py` & `pyiron_base-0.8.3/pyiron_base/storage/has_stored_traits.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/storage/hdfio.py` & `pyiron_base-0.8.3/pyiron_base/storage/hdfio.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/storage/hdfstub.py` & `pyiron_base-0.8.3/pyiron_base/storage/hdfstub.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/storage/helper_functions.py` & `pyiron_base-0.8.3/pyiron_base/storage/helper_functions.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/storage/parameters.py` & `pyiron_base-0.8.3/pyiron_base/storage/parameters.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/utils/deprecate.py` & `pyiron_base-0.8.3/pyiron_base/utils/deprecate.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/utils/error.py` & `pyiron_base-0.8.3/pyiron_base/utils/error.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/utils/instance.py` & `pyiron_base-0.8.3/pyiron_base/utils/instance.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/utils/jedi.py` & `pyiron_base-0.8.3/pyiron_base/utils/jedi.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/utils/parser.py` & `pyiron_base-0.8.3/pyiron_base/utils/parser.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/utils/safetar.py` & `pyiron_base-0.8.3/pyiron_base/utils/safetar.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base/utils/units.py` & `pyiron_base-0.8.3/pyiron_base/utils/units.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyiron_base.egg-info/PKG-INFO` & `pyiron_base-0.8.3/pyiron_base.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_base
-Version: 0.8.2
+Version: 0.8.3
 Summary: Core components of the pyiron integrated development environment (IDE) for computational materials science
 Author-email: "Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department" <pyiron@mpie.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2018, Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
         All rights reserved.
         
@@ -51,25 +51,25 @@
 License-File: LICENSE
 Requires-Dist: cloudpickle<=3.0.0,>=2.0.0
 Requires-Dist: gitpython<=3.1.43,>=3.1.23
 Requires-Dist: h5io_browser<=0.0.12,>=0.0.6
 Requires-Dist: h5py<=3.11.0,>=3.6.0
 Requires-Dist: jinja2<=3.1.3,>=2.11.3
 Requires-Dist: numpy<=1.26.4,>=1.23.5
-Requires-Dist: monty<=2024.3.31,>=2021.3.3
+Requires-Dist: monty<=2024.4.17,>=2021.3.3
 Requires-Dist: pandas<=2.2.2,>=2.0.0
 Requires-Dist: pint<=0.23,>=0.18
 Requires-Dist: psutil<=5.9.8,>=5.8.0
 Requires-Dist: pyfileindex<=0.0.24,>=0.0.16
-Requires-Dist: pympipool<=0.7.17,>=0.7.11
-Requires-Dist: pysqa<=0.1.18,>=0.1.12
+Requires-Dist: pympipool<=0.8.1,>=0.8.0
+Requires-Dist: pysqa<=0.1.19,>=0.1.12
 Requires-Dist: sqlalchemy<=2.0.29,>=2.0.22
 Requires-Dist: tables<=3.9.2,>=3.6.1
 Requires-Dist: tqdm<=4.66.2,>=4.44.0
-Requires-Dist: traitlets<=5.14.2,>=5.1.1
+Requires-Dist: traitlets<=5.14.3,>=5.1.1
 Provides-Extra: conda
 Requires-Dist: conda==23.11.0; extra == "conda"
 Requires-Dist: conda_subprocess==0.0.1; extra == "conda"
 
 pyiron
 ======
```

### Comparing `pyiron_base-0.8.2/pyiron_base.egg-info/SOURCES.txt` & `pyiron_base-0.8.3/pyiron_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/pyproject.toml` & `pyiron_base-0.8.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -26,25 +26,25 @@
 dependencies = [
     "cloudpickle>=2.0.0,<=3.0.0",
     "gitpython>=3.1.23,<=3.1.43",
     "h5io_browser>=0.0.6,<=0.0.12",
     "h5py>=3.6.0,<=3.11.0",
     "jinja2>=2.11.3,<=3.1.3",
     "numpy>=1.23.5,<=1.26.4",
-    "monty>=2021.3.3,<=2024.3.31",
+    "monty>=2021.3.3,<=2024.4.17",
     "pandas>=2.0.0,<=2.2.2",
     "pint>=0.18,<=0.23",
     "psutil>=5.8.0,<=5.9.8",
     "pyfileindex>=0.0.16,<=0.0.24",
-    "pympipool>=0.7.11,<=0.7.17",
-    "pysqa>=0.1.12,<=0.1.18",
+    "pympipool>=0.8.0,<=0.8.1",
+    "pysqa>=0.1.12,<=0.1.19",
     "sqlalchemy>=2.0.22,<=2.0.29",
     "tables>=3.6.1,<=3.9.2",
     "tqdm>=4.44.0,<=4.66.2",
-    "traitlets>=5.1.1,<=5.14.2",
+    "traitlets>=5.1.1,<=5.14.3",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/pyiron/pyiron_base"
 Documentation = "https://github.com/pyiron/pyiron_base"
 Repository = "https://github.com/pyiron/pyiron_base"
```

### Comparing `pyiron_base-0.8.2/tests/test_testwithproject.py` & `pyiron_base-0.8.3/tests/test_testwithproject.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.8.2/tests/test_toolkit.py` & `pyiron_base-0.8.3/tests/test_toolkit.py`

 * *Files identical despite different names*

