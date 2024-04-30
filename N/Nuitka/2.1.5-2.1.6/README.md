# Comparing `tmp/Nuitka-2.1.5.tar.gz` & `tmp/Nuitka-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Nuitka-2.1.5.tar", last modified: Sat Apr  6 13:33:51 2024, max compression, from Unix
+gzip compressed data, was "Nuitka-2.1.6.tar", last modified: Fri Apr 19 13:34:36 2024, max compression, from Unix
```

## Comparing `Nuitka-2.1.5.tar` & `Nuitka-2.1.6.tar`

### file list

```diff
@@ -1,1831 +1,1831 @@
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.111591 Nuitka-2.1.5/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      228 2024-03-04 14:35:43.000000 Nuitka-2.1.5/Changelog.rst
--rw-r--r--   0 hayen     (1000) hayen     (2000)   152282 2024-03-04 14:35:43.000000 Nuitka-2.1.5/Developer_Manual.rst
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11348 2021-04-22 06:31:42.000000 Nuitka-2.1.5/LICENSE.txt
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1707 2024-01-26 12:30:51.000000 Nuitka-2.1.5/MANIFEST.in
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.031591 Nuitka-2.1.5/Nuitka.egg-info/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    82956 2024-04-06 13:33:49.000000 Nuitka-2.1.5/Nuitka.egg-info/PKG-INFO
--rw-r--r--   0 hayen     (1000) hayen     (2000)    77774 2024-04-06 13:33:50.000000 Nuitka-2.1.5/Nuitka.egg-info/SOURCES.txt
--rw-r--r--   0 hayen     (1000) hayen     (2000)        1 2024-04-06 13:33:49.000000 Nuitka-2.1.5/Nuitka.egg-info/dependency_links.txt
--rw-r--r--   0 hayen     (1000) hayen     (2000)      393 2024-04-06 13:33:49.000000 Nuitka-2.1.5/Nuitka.egg-info/entry_points.txt
--rw-r--r--   0 hayen     (1000) hayen     (2000)        1 2024-02-02 15:24:24.000000 Nuitka-2.1.5/Nuitka.egg-info/not-zip-safe
--rw-r--r--   0 hayen     (1000) hayen     (2000)        7 2024-04-06 13:33:49.000000 Nuitka-2.1.5/Nuitka.egg-info/top_level.txt
--rw-r--r--   0 hayen     (1000) hayen     (2000)    82956 2024-04-06 13:33:50.111591 Nuitka-2.1.5/PKG-INFO
--rw-r--r--   0 hayen     (1000) hayen     (2000)    80812 2024-03-04 14:35:43.000000 Nuitka-2.1.5/README.rst
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.031591 Nuitka-2.1.5/bin/
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     1166 2024-03-04 14:35:43.000000 Nuitka-2.1.5/bin/autoformat-nuitka-source
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     1165 2024-03-04 14:35:43.000000 Nuitka-2.1.5/bin/check-nuitka-with-pylint
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     1181 2024-03-04 14:35:43.000000 Nuitka-2.1.5/bin/compare_with_cpython
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     3105 2024-03-04 14:35:43.000000 Nuitka-2.1.5/bin/compare_with_xml
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     1194 2024-03-04 14:35:43.000000 Nuitka-2.1.5/bin/measure-construct-performance
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     1716 2024-03-04 14:35:43.000000 Nuitka-2.1.5/bin/nuitka
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     1716 2024-03-04 14:35:43.000000 Nuitka-2.1.5/bin/nuitka-run
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.031591 Nuitka-2.1.5/doc/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.031591 Nuitka-2.1.5/doc/Logo/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1797 2024-03-04 14:35:43.000000 Nuitka-2.1.5/doc/Logo/Nuitka-Logo-Horizontal.svg
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1553 2024-03-04 14:35:43.000000 Nuitka-2.1.5/doc/Logo/Nuitka-Logo-Symbol.svg
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1793 2024-03-04 14:35:43.000000 Nuitka-2.1.5/doc/Logo/Nuitka-Logo-Vertical.svg
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.031591 Nuitka-2.1.5/doc/images/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7585 2021-04-22 06:31:42.000000 Nuitka-2.1.5/doc/images/Nuitka-Logo-Horizontal.png
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4452 2021-04-22 06:31:42.000000 Nuitka-2.1.5/doc/images/Nuitka-Logo-Symbol.png
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9828 2022-01-09 15:54:20.000000 Nuitka-2.1.5/doc/images/Nuitka-Logo-Vertical.png
--rw-r--r--   0 hayen     (1000) hayen     (2000)    33808 2024-03-11 17:07:05.000000 Nuitka-2.1.5/doc/nuitka-run.1
--rw-r--r--   0 hayen     (1000) hayen     (2000)    33832 2024-03-11 17:07:05.000000 Nuitka-2.1.5/doc/nuitka.1
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.031591 Nuitka-2.1.5/lib/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4640 2024-03-04 14:35:43.000000 Nuitka-2.1.5/lib/hints.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.031591 Nuitka-2.1.5/misc/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      924 2024-03-04 14:35:43.000000 Nuitka-2.1.5/misc/nuitka-run.bat
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1061 2024-03-04 14:35:43.000000 Nuitka-2.1.5/misc/nuitka.bat
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.031591 Nuitka-2.1.5/nuitka/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7560 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/Builtins.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5787 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/BytecodeCaching.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3800 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/Bytecodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1855 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/CacheCleanup.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11181 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/Constants.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2479 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/Errors.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10335 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/HardImportRegistry.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    38348 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/MainControl.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8616 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/ModuleRegistry.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    62344 2024-03-22 08:13:25.000000 Nuitka-2.1.5/nuitka/OptionParsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    74907 2024-04-06 13:33:42.000000 Nuitka-2.1.5/nuitka/Options.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5276 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/OutputDirectories.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14940 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/PostProcessing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6797 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/Progress.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9654 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/PythonFlavors.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4093 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/PythonOperators.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14557 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/PythonVersions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8989 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/Serialization.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4703 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/SourceCodeReferences.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13335 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/Tracing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3513 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/TreeXML.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15470 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/Variables.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2466 2024-04-06 13:33:42.000000 Nuitka-2.1.5/nuitka/Version.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6373 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/__main__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5604 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/__past__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.041591 Nuitka-2.1.5/nuitka/build/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    36393 2024-03-11 17:07:05.000000 Nuitka-2.1.5/nuitka/build/Backend.scons
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8583 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/CCompilerVersion.scons
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3485 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/DataComposerInterface.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17733 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/Onefile.scons
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14643 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/SconsCaching.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    35437 2024-03-11 17:07:05.000000 Nuitka-2.1.5/nuitka/build/SconsCompilerSettings.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5592 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/SconsHacks.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15933 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/SconsInterface.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2704 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/SconsProgress.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13210 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/SconsSpawn.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    26957 2024-03-22 08:13:25.000000 Nuitka-2.1.5/nuitka/build/SconsUtils.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.021591 Nuitka-2.1.5/nuitka/build/include/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.041591 Nuitka-2.1.5/nuitka/build/include/nuitka/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8001 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/allocator.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3499 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/builtins.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5196 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/calling.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2006 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/checkers.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1123 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/checksum_tools.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9333 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/compiled_asyncgen.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2195 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/compiled_cell.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9233 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/compiled_coroutine.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17661 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/compiled_frame.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7267 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/compiled_function.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9189 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/compiled_generator.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1866 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/compiled_method.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7620 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/constants.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1345 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/constants_blob.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1187 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/environment_variables.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1872 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/environment_variables_system.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5302 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/exception_groups.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    34114 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/exceptions.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3792 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/filesystem_paths.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6474 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/freelists.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    86326 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/hedley.h
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.041591 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3698 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/attributes.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2692 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/boolean.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1233 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/bytearrays.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1164 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/bytes.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11894 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/calling_generated.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13169 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/comparisons_eq.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10645 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/comparisons_ge.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10644 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/comparisons_gt.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13169 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/comparisons_le.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13168 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/comparisons_lt.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10645 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/comparisons_ne.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1834 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/complex.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13551 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/dictionaries.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1235 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/floats.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4291 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/import_hard.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1827 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/indexes.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2970 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/ints.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9599 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/iterators.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3601 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/lists.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1662 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/lists_generated.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1386 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/mappings.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4671 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12714 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_add.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5692 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_bitand.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5670 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_bitor.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5692 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5451 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_divmod.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5489 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5144 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_lshift.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2828 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_matmult.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15807 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_mod.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13239 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_mult.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5820 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4743 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_pow.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5144 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_rshift.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5853 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_sub.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5467 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_truediv.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    20173 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_builtin_types.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8699 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_add.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3796 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3782 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3796 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4875 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3040 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2756 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10655 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_mod.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9230 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_mult.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5176 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4378 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_pow.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3040 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5004 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_sub.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4855 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3381 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/raising.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2367 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/rangeobjects.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1175 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/richcomparisons.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1141 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/sequences.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1054 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/sets.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8750 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/slices.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1363 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/strings.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17975 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/subscripts.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5749 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helper/tuples.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    16626 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/helpers.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6150 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/importing.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12979 2022-10-08 15:33:22.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/incbin.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15484 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/prelude.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2899 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/printing.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1811 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/python_pgo.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2343 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/safe_string_ops.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3809 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/threading.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3447 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/tracing.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3135 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/include/nuitka/unfreezing.h
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.021591 Nuitka-2.1.5/nuitka/build/inline_copy/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.041591 Nuitka-2.1.5/nuitka/build/inline_copy/appdirs/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1097 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/appdirs/LICENSE.txt
--rw-r--r--   0 hayen     (1000) hayen     (2000)    24824 2022-10-08 09:07:15.000000 Nuitka-2.1.5/nuitka/build/inline_copy/appdirs/appdirs.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.041591 Nuitka-2.1.5/nuitka/build/inline_copy/atomicwrites/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1069 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/atomicwrites/LICENSE
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6794 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/atomicwrites/atomicwrites.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.041591 Nuitka-2.1.5/nuitka/build/inline_copy/bin/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1695 2023-11-22 13:25:43.000000 Nuitka-2.1.5/nuitka/build/inline_copy/bin/scons.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.021591 Nuitka-2.1.5/nuitka/build/inline_copy/clcache/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.041591 Nuitka-2.1.5/nuitka/build/inline_copy/clcache/clcache/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1585 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/clcache/clcache/LICENSE
--rw-r--r--   0 hayen     (1000) hayen     (2000)       93 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/clcache/clcache/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    65424 2023-03-17 17:23:10.000000 Nuitka-2.1.5/nuitka/build/inline_copy/clcache/clcache/caching.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.041591 Nuitka-2.1.5/nuitka/build/inline_copy/colorama/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1491 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/colorama/LICENSE.txt
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.041591 Nuitka-2.1.5/nuitka/build/inline_copy/colorama/colorama/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      243 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/colorama/colorama/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2522 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/colorama/colorama/ansi.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10517 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1915 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/colorama/colorama/initialise.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5404 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/colorama/colorama/win32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6438 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/colorama/colorama/winterm.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.041591 Nuitka-2.1.5/nuitka/build/inline_copy/glob2/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1359 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/glob2/LICENSE
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.041591 Nuitka-2.1.5/nuitka/build/inline_copy/glob2/glob2/
--rw-r--r--   0 hayen     (1000) hayen     (2000)       82 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/glob2/glob2/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6859 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/glob2/glob2/compat.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4463 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/glob2/glob2/fnmatch.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8304 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/glob2/glob2/impl.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.041591 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1467 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/LICENSE.rst
--rw-r--r--   0 hayen     (1000) hayen     (2000)       85 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/README.rst
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.041591 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2423 2022-10-08 09:07:15.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2685 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/_compat.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1726 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12719 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/bccache.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    65386 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/compiler.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1626 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/constants.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12281 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/debug.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1400 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/defaults.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    50849 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/environment.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4428 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    24500 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/ext.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    36528 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/filters.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9197 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    28559 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/lexer.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17473 2022-10-08 09:07:15.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/loaders.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4340 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/meta.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7308 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    30853 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/nodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1722 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    35875 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/parser.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    27644 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/runtime.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17080 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4214 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/tests.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    20501 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/utils.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3316 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/visitor.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.041591 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1466 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/LICENSE.rst
--rw-r--r--   0 hayen     (1000) hayen     (2000)       84 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/README.rst
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.041591 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2616 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2685 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1726 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12719 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    65386 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1626 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12281 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1400 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    50849 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4428 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    24500 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    36528 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9197 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    28559 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17474 2022-10-08 09:07:15.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4340 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7308 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    30853 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1722 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    35875 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    27644 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17080 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4214 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    20501 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3316 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.021591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.021591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.041591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    47844 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    33996 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8083 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    27693 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6938 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17622 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    96183 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7358 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    21540 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    16000 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9589 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.041591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4197 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)   121420 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4164 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    49503 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.041591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1950 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1950 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1950 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1965 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2736 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2614 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8467 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.041591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9314 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3131 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1989 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2483 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1718 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1605 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2170 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4179 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1882 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15042 2024-01-26 12:30:51.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    39700 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12950 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.041591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4810 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3751 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3233 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2011 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14663 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.041591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14029 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    52665 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    40719 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    24133 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14053 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2305 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    34903 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    40510 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.051591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2166 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2433 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2859 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    18084 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.051591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2078 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2004 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9248 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2784 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14869 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    19499 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    20832 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3763 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5149 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2290 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2328 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2657 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    31283 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2379 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2267 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2681 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2720 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2796 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2147 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2936 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2935 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3432 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3785 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2777 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1711 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      142 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/dmd.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.051591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    29618 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3428 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2681 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2433 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1844 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3472 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4782 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2025 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2256 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2460 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2639 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1810 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2333 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2140 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1902 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2077 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2043 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    18600 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    25816 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3328 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8394 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3953 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2309 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2945 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6919 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4381 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4658 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4224 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2168 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13881 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1804 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11380 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    72761 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6841 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3579 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2618 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4375 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2827 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2513 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1991 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1819 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2123 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2502 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4695 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1927 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2349 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2473 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5992 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1831 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3730 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13016 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3415 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    48938 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.051591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3007 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3784 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4380 2024-01-26 12:30:51.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3557 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5612 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11034 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6824 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1563 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.051591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8120 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3596 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1818 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1742 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2465 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1776 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    19253 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    44500 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    19664 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7509 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2107 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.021591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.051591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    53545 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    34985 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13596 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    28403 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7533 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    20988 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    96818 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7752 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    22350 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    16068 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9565 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.051591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5239 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)   135413 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5758 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    63474 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8354 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.051591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11500 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3180 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2227 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2739 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1767 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1654 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1460 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2219 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4476 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1931 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4003 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17055 2024-01-26 12:30:51.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    41186 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13880 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.051591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4853 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3812 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3643 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2328 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15053 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.051591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13779 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    53260 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    39394 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    26467 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14489 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    35863 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    42204 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.051591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2211 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    18207 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.051591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2152 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2057 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10674 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2855 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15165 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    33537 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    21762 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4464 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    50660 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1667 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2316 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2475 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2840 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8618 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2226 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2978 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2977 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1653 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3827 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3389 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.051591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      313 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3631 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3444 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8494 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1753 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.051591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    29765 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3472 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1630 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1977 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3686 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2580 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2948 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2655 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1645 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1859 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2765 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2386 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2189 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1944 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2123 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2085 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15791 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    26195 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13924 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4041 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2351 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2987 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7808 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4956 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5235 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4808 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2475 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14751 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1847 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12588 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    82939 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6883 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3663 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2660 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4904 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2877 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2567 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1652 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1868 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2088 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2176 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2366 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1658 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1976 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5335 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2583 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2515 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6756 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1873 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3773 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13982 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3201 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    53803 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.061591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3064 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3818 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4435 2024-01-26 12:30:51.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3643 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5579 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11655 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6504 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1647 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.061591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6869 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1784 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    19816 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9002 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2149 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.021591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.061591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    56578 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    35213 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11061 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    27408 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7884 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    21423 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    97269 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3979 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7515 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    21937 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    16583 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9430 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.061591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5126 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)   136271 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6167 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    63768 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8183 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.061591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12836 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3087 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2107 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2630 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1674 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1536 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1311 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2076 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4356 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1805 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3860 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14831 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    41983 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14673 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.061591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7394 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4357 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3546 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1972 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15577 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.061591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13597 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    53509 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    42760 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    26676 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14272 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    36753 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    41191 2022-10-08 09:07:15.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.061591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2122 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15570 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.061591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2014 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1943 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13182 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2734 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15027 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    38783 2023-03-17 17:23:10.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    22570 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4368 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    32724 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1578 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2228 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2386 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2616 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7993 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2141 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1661 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2893 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2889 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1567 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3742 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3296 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.061591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      343 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3534 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3259 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7461 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1663 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3379 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1544 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1891 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3616 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2377 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2437 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2526 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1557 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1772 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2677 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2206 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2096 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1851 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1954 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1995 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    19180 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    25826 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2588 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.061591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4649 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7652 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6064 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3931 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2266 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2900 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8622 2022-10-08 09:07:15.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4577 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4517 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4113 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2387 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14473 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1752 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12902 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    84784 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6788 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3576 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2573 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4817 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2788 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2479 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1563 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1780 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1999 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2006 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2271 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1569 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1888 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4879 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2419 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2429 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6412 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1786 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3687 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12548 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4076 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    71693 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.061591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6632 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)        0 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15278 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.061591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3134 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3896 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4648 2024-01-26 12:30:51.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3536 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5588 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12708 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6785 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      353 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.061591 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4307 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1644 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3395 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    21614 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9295 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2032 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.061591 Nuitka-2.1.5/nuitka/build/inline_copy/markupsafe/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1467 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/markupsafe/LICENSE.rst
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.061591 Nuitka-2.1.5/nuitka/build/inline_copy/markupsafe/markupsafe/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10126 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      558 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4690 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1873 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.021591 Nuitka-2.1.5/nuitka/build/inline_copy/pkg_resources/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.061591 Nuitka-2.1.5/nuitka/build/inline_copy/pkg_resources/pkg_resources/
--rw-r--r--   0 hayen     (1000) hayen     (2000)   107452 2022-10-08 09:07:15.000000 Nuitka-2.1.5/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      538 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.021591 Nuitka-2.1.5/nuitka/build/inline_copy/tqdm/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.061591 Nuitka-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1595 2023-11-22 13:25:43.000000 Nuitka-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      283 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/_main.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3687 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      283 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/_tqdm.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      307 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_notebook.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      888 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      596 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/_utils.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1106 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/auto.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      857 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1376 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/dask.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10790 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/notebook.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    57572 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/std.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6948 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/tk.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9726 2023-11-22 13:25:43.000000 Nuitka-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/utils.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      167 2024-01-07 19:01:51.000000 Nuitka-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/version.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.061591 Nuitka-2.1.5/nuitka/build/inline_copy/yaml/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1101 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml/LICENSE
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.061591 Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13170 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4883 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/composer.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    28639 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/constructor.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3851 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/cyaml.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2837 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/dumper.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    43006 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/emitter.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2533 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/error.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2445 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/events.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2061 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/loader.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1440 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/nodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    25495 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/parser.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6794 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/reader.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14184 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/representer.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8999 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/resolver.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    51277 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/scanner.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4165 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/serializer.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2573 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/tokens.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.061591 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1101 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/LICENSE
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.061591 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9776 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4921 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/composer.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    25145 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/constructor.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3290 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2719 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/dumper.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    43298 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/emitter.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2559 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/error.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2445 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/events.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1132 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/loader.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1440 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/nodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    25542 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/parser.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6746 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/reader.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17711 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/representer.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9122 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/resolver.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    52446 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/scanner.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4171 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/serializer.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2573 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/tokens.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.061591 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1101 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/LICENSE
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.061591 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9607 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4881 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/composer.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    25554 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/constructor.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3294 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2723 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/dumper.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    42954 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/emitter.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2533 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/error.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2445 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/events.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1138 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/loader.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1440 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/nodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    25495 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/parser.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6854 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/reader.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14097 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/representer.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8970 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/resolver.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    51695 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/scanner.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4165 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/serializer.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2573 2022-01-09 15:54:20.000000 Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/tokens.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.071591 Nuitka-2.1.5/nuitka/build/inline_copy/zlib/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1002 2023-11-22 13:25:43.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zlib/LICENSE
--rw-r--r--   0 hayen     (1000) hayen     (2000)    31605 2023-11-22 13:25:43.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zlib/crc32.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   591749 2023-11-22 13:25:43.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zlib/crc32.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    16682 2023-11-22 13:25:43.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zlib/zconf.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    96778 2023-11-22 13:25:43.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zlib/zlib.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7247 2023-11-22 13:25:43.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zlib/zutil.h
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.071591 Nuitka-2.1.5/nuitka/build/inline_copy/zstd/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1530 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zstd/LICENSE.txt
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.071591 Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    18198 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/bitstream.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10157 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/compiler.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4455 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/cpu.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3763 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/debug.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13662 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/entropy_common.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3009 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/error_private.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2441 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/error_private.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    34422 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/fse.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14748 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/fse_decompress.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    20216 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/huf.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13930 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/mem.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    26976 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/xxhash.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11706 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/xxhash.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2728 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/zstd_common.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2497 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/zstd_deps.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3828 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/zstd_errors.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15880 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/zstd_internal.h
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.071591 Nuitka-2.1.5/nuitka/build/inline_copy/zstd/decompress/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    54982 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9164 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1321 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    80283 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    66784 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2253 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7906 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)   138334 2021-04-22 06:31:42.000000 Nuitka-2.1.5/nuitka/build/inline_copy/zstd/zstd.h
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.071591 Nuitka-2.1.5/nuitka/build/static_src/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    84761 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/CompiledAsyncgenType.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9142 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/CompiledCellType.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    58739 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/CompiledCodeHelpers.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    73577 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/CompiledCoroutineType.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    40760 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/CompiledFrameType.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   109285 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/CompiledFunctionType.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    63983 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/CompiledGeneratorType.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    56631 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    22473 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/CompiledMethodType.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    19054 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersAllocator.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    38264 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersAttributes.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    23678 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersBuiltin.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   114017 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersBuiltinTypeMethods.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3062 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersBytes.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13376 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersCalling.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   481627 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersCallingGenerated.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2065 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersChecksumTools.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3051 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersClasses.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   318307 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersComparisonEq.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4762 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersComparisonEqUtils.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   313126 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersComparisonGe.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   312537 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersComparisonGt.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   316340 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersComparisonLe.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   315751 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersComparisonLt.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   315055 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersComparisonNe.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    36776 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersConstantsBlob.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    20361 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersDeepcopy.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    39584 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersDictionaries.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    26620 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersDictionariesGenerated.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2066 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersDumpBacktraces.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2194 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersEnvironmentVariables.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2979 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersEnvironmentVariablesSystem.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7145 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersExceptions.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8018 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersFiles.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    28806 2024-03-28 13:28:39.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersFilesystemPaths.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2455 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersFloats.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1803 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersHeapStorage.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    16080 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersImport.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    16403 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersImportHard.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    19996 2024-03-28 13:28:39.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersLists.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13944 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersListsGenerated.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1669 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersMappings.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3587 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersMatching.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   181603 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryAdd.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    16729 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    77972 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryBitand.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    77811 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryBitor.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    77972 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryBitxor.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    68218 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryDivmod.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1265 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    69479 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6300 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    83954 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryLshift.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13805 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryMatmult.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   183867 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryMod.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   188543 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryMult.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3433 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    67184 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    79484 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryPow.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1052 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    77854 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryRshift.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    70494 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinarySub.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    68736 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryTruediv.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   150679 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationInplaceAdd.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4240 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    53253 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationInplaceBitand.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    53151 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationInplaceBitor.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    53253 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationInplaceBitxor.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    77119 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    47857 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationInplaceLshift.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17771 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationInplaceMatmult.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   136385 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationInplaceMod.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   142240 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationInplaceMult.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    74749 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    83262 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationInplacePow.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    45341 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationInplaceRshift.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    82871 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationInplaceSub.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    76950 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationInplaceTruediv.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3394 2024-03-22 08:13:25.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersProfiling.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3840 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersPythonPgo.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15663 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersRaising.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3868 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersSafeStrings.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3759 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersSequences.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1975 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersSlices.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    27056 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersStrings.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4181 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersTuples.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5628 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/HelpersTypes.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12136 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/InspectPatcher.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    54017 2024-04-06 13:33:42.000000 Nuitka-2.1.5/nuitka/build/static_src/MainProgram.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    63759 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/MetaPathBasedLoader.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4827 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6651 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    21896 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    31916 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/OnefileBootstrap.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8050 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/build/static_src/OnefileSplashScreen.cpp
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.081591 Nuitka-2.1.5/nuitka/code_generation/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6491 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/AsyncgenCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10821 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/AttributeCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    21894 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/BinaryOperationHelperDefinitions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2371 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/BranchCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17005 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/BuiltinCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    36111 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/CallCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4958 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/ClassCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    52589 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/CodeGeneration.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2408 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/CodeHelperSelection.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14272 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/CodeHelpers.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5083 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/CodeObjectCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17645 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/ComparisonCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4479 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/ComparisonHelperDefinitions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7368 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/ConditionalCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6661 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/ConstantCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    33901 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/Contexts.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8589 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/CoroutineCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1607 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/CtypesCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    28934 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/DictCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2158 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/Emission.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9415 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/ErrorCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12951 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/EvalCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9011 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/ExceptionCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7383 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2126 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/ExpressionCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17804 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/FrameCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    28337 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/FunctionCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7828 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/GeneratorCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6384 2024-03-28 13:28:39.000000 Nuitka-2.1.5/nuitka/code_generation/GlobalConstants.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6985 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/GlobalsLocalsCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1870 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/IdCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14684 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/ImportCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1429 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/Indentation.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1574 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/IndexCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1066 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/InjectCCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3567 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/IntegerCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12211 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/IteratorCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2055 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/LabelCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2645 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/LineNumberCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    16152 2024-03-28 13:28:39.000000 Nuitka-2.1.5/nuitka/code_generation/ListCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6658 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/LoaderCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10016 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/LocalsDictCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3174 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/LoopCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1638 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/MatchCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6455 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/ModuleCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8225 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/Namify.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12685 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/OperationCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    30146 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/PackageResourceCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3054 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/PrintCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5670 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/PythonAPICodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13251 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/RaisingCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3476 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/Reports.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5267 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/ReturnCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6591 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/SetCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14005 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/SliceCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10087 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/StringCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8302 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/SubscriptCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11208 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/TryCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3840 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/TupleCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14747 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/VariableCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9154 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/VariableDeclarations.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8129 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/YieldCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.081591 Nuitka-2.1.5/nuitka/code_generation/c_types/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6102 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/c_types/CTypeBases.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3432 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/c_types/CTypeBooleans.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1837 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/c_types/CTypeCFloats.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1411 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/c_types/CTypeCLongs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3642 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/c_types/CTypeModuleDictVariables.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5161 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5244 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/c_types/CTypeNuitkaInts.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3988 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/c_types/CTypeNuitkaVoids.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    19696 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/c_types/CTypePyObjectPointers.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2885 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/c_types/CTypeVoids.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/c_types/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.081591 Nuitka-2.1.5/nuitka/code_generation/templates/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2948 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8928 2024-03-22 08:13:25.000000 Nuitka-2.1.5/nuitka/code_generation/templates/CodeTemplatesConstants.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3040 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates/CodeTemplatesCoroutines.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2358 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates/CodeTemplatesExceptions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6483 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates/CodeTemplatesFrames.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3460 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates/CodeTemplatesFunction.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3390 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2409 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates/CodeTemplatesIterators.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4535 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates/CodeTemplatesLoader.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    22938 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates/CodeTemplatesModules.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6800 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates/CodeTemplatesVariables.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2508 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates/TemplateDebugWrapper.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.081591 Nuitka-2.1.5/nuitka/code_generation/templates_c/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11318 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5829 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)    23986 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5438 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1755 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1693 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2706 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13624 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1894 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperImportHard.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2618 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperLongTools.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1394 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperObjectTools.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7047 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12700 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4138 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1938 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1968 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4081 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7257 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4142 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3710 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4379 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11758 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)    19167 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2693 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3485 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11336 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15540 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2829 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperSlotsList.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10271 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2407 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2870 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2834 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3128 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.081591 Nuitka-2.1.5/nuitka/containers/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1468 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/containers/Namedtuples.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6553 2022-10-08 09:07:15.000000 Nuitka-2.1.5/nuitka/containers/OrderedDicts.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      554 2022-10-08 09:07:15.000000 Nuitka-2.1.5/nuitka/containers/OrderedSets.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4430 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/containers/OrderedSetsFallback.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/containers/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.081591 Nuitka-2.1.5/nuitka/distutils/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2308 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/distutils/Build.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15025 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/distutils/DistutilCommands.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/distutils/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.081591 Nuitka-2.1.5/nuitka/finalizations/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1257 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/finalizations/Finalization.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6059 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/finalizations/FinalizeMarkups.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/finalizations/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.081591 Nuitka-2.1.5/nuitka/freezer/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7778 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/freezer/DependsExe.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2616 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/freezer/DllDependenciesCommon.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12609 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/freezer/DllDependenciesMacOS.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7469 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/freezer/DllDependenciesPosix.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6633 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/freezer/DllDependenciesWin32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11979 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/freezer/ImportDetection.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17908 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/freezer/IncludedDataFiles.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11415 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/freezer/IncludedEntryPoints.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9551 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/freezer/Onefile.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11988 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/freezer/Standalone.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/freezer/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.081591 Nuitka-2.1.5/nuitka/importing/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11040 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/importing/IgnoreListing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2932 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/importing/ImportCache.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7560 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/importing/ImportResolving.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    31922 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/importing/Importing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4869 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/importing/PreloadedPackages.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    18804 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/importing/Recursion.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12787 2024-04-06 13:33:42.000000 Nuitka-2.1.5/nuitka/importing/StandardLibrary.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/importing/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.081591 Nuitka-2.1.5/nuitka/nodes/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3670 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/AsyncgenNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4115 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/AttributeLookupNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13255 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/AttributeNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)   378777 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/AttributeNodesGenerated.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3856 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/BuiltinAllNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4131 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/BuiltinAnyNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2529 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/BuiltinComplexNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1731 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/BuiltinDecodingNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2760 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/BuiltinDecoratorNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4727 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/BuiltinDictNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4981 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/BuiltinFormatNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2275 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/BuiltinHashNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1457 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/BuiltinInputNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5367 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/BuiltinIntegerNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12756 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/BuiltinIteratorNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2029 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/BuiltinLenNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3639 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/BuiltinNextNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3787 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/BuiltinOpenNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)   245569 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    18648 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/BuiltinRangeNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9100 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/BuiltinRefNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3353 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/BuiltinSumNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13576 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/BuiltinTypeNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1606 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/BuiltinVarsNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    26146 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/BytesNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6511 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/CallNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1583 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/Checkers.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)   623739 2024-03-11 17:07:05.000000 Nuitka-2.1.5/nuitka/nodes/ChildrenHavingMixins.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8480 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/ClassNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6618 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/CodeObjectSpecs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    21716 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/ComparisonNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    30300 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/ConditionalNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    46568 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/ConstantRefNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12246 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/ContainerMakingNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2867 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/ContainerOperationNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4614 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/CoroutineNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1747 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/CtypesNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    51054 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/DictionaryNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7889 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/ExceptionNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7408 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/ExecEvalNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    44902 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/ExpressionBases.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    55109 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/ExpressionBasesGenerated.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    21311 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/ExpressionShapeMixins.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12024 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/FrameNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3577 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/FunctionAttributeNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    39667 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/FunctionNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5409 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/FutureSpecs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6288 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/GeneratorNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6961 2024-04-06 13:33:42.000000 Nuitka-2.1.5/nuitka/nodes/GlobalsLocalsNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    92183 2024-03-11 17:07:05.000000 Nuitka-2.1.5/nuitka/nodes/HardImportNodesGenerated.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5378 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/ImportHardNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    47515 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/ImportNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2766 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/IndicatorMixins.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1534 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/InjectCNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11519 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/IterationHandles.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11035 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/KeyValuePairNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    16821 2024-03-11 17:07:05.000000 Nuitka-2.1.5/nuitka/nodes/ListOperationNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    23177 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/LocalsDictNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15007 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/LocalsScopes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15995 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/LoopNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1745 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/MatchNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6567 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/ModuleAttributeNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    32713 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/ModuleNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    24461 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/NodeBases.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15147 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/NodeMakingHelpers.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5580 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/NodeMetaClasses.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    31948 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/OperatorNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8975 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/OperatorNodesUnary.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5229 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/OsSysNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12468 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/OutlineNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    34736 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/PackageMetadataNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12241 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/PackageResourceNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3440 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/PrintNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6805 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/ReturnNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4748 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/SideEffectNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12547 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/SliceNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    97361 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/StatementBasesGenerated.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9336 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/StatementNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    28691 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/StrNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3537 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/StringConcatenationNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8329 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/SubscriptNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17886 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/TryNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2438 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/TypeMatchNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11094 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/TypeNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    42396 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/VariableAssignNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10779 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/VariableDelNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4607 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/VariableNameNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    31228 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/VariableRefNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4781 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/VariableReleaseNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3937 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/YieldNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.081591 Nuitka-2.1.5/nuitka/nodes/shapes/
--rw-r--r--   0 hayen     (1000) hayen     (2000)   157197 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/shapes/BuiltinTypeShapes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4420 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/shapes/ControlFlowDescriptions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5076 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/shapes/ShapeMixins.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    42509 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/shapes/StandardShapes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/nodes/shapes/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.091591 Nuitka-2.1.5/nuitka/optimizations/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3358 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/optimizations/BytecodeDemotion.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3953 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/optimizations/FunctionInlining.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2177 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/optimizations/Graphs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10866 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/optimizations/Optimization.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    52487 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/optimizations/OptimizeBuiltinCalls.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2288 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/optimizations/Tags.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    45089 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/optimizations/TraceCollections.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    24504 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/optimizations/ValueTraces.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/optimizations/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.091591 Nuitka-2.1.5/nuitka/pgo/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4932 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/pgo/PGO.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/pgo/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.091591 Nuitka-2.1.5/nuitka/plugins/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    56921 2024-03-28 13:28:39.000000 Nuitka-2.1.5/nuitka/plugins/PluginBase.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    59723 2024-03-14 10:27:18.000000 Nuitka-2.1.5/nuitka/plugins/Plugins.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/plugins/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.091591 Nuitka-2.1.5/nuitka/plugins/standard/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    30408 2024-03-14 10:27:18.000000 Nuitka-2.1.5/nuitka/plugins/standard/AntiBloatPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3510 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10754 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/plugins/standard/DataFilesPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5080 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/plugins/standard/DelvewheelPlugin.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.091591 Nuitka-2.1.5/nuitka/plugins/standard/DillPlugin/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1646 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/plugins/standard/DillPlugin/DillPlugin.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9826 2024-03-22 08:13:25.000000 Nuitka-2.1.5/nuitka/plugins/standard/DillPlugin/dill-postLoad.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2679 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/plugins/standard/DillPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    16277 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/plugins/standard/DllFilesPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2095 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/plugins/standard/EnumPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1938 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/plugins/standard/EventletPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1913 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/plugins/standard/GeventPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4017 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/plugins/standard/GiPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4854 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/plugins/standard/GlfwPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    32261 2024-03-28 13:28:39.000000 Nuitka-2.1.5/nuitka/plugins/standard/ImplicitImports.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5024 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/plugins/standard/KivyPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8823 2024-03-28 13:28:39.000000 Nuitka-2.1.5/nuitka/plugins/standard/MatplotlibPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7080 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/plugins/standard/MultiprocessingPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1220 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/plugins/standard/NumpyPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7433 2024-03-28 13:28:39.000000 Nuitka-2.1.5/nuitka/plugins/standard/OptionsNannyPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1940 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/plugins/standard/PbrPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4875 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/plugins/standard/PkgResourcesPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7042 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/plugins/standard/PmwPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    53098 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/plugins/standard/PySidePyQtPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3020 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/plugins/standard/PywebViewPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1193 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/plugins/standard/TensorflowPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13878 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/plugins/standard/TkinterPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1173 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/plugins/standard/TorchPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12838 2024-04-06 13:33:42.000000 Nuitka-2.1.5/nuitka/plugins/standard/TransformersPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1106 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/plugins/standard/TrioPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5668 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/plugins/standard/UpxPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/plugins/standard/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)   231363 2024-04-06 13:33:42.000000 Nuitka-2.1.5/nuitka/plugins/standard/standard.nuitka-package.config.yml
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2352 2024-01-26 12:30:51.000000 Nuitka-2.1.5/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12392 2024-01-26 12:30:51.000000 Nuitka-2.1.5/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.091591 Nuitka-2.1.5/nuitka/reports/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2287 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/reports/CompilationReportReader.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2089 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/reports/LicenseReport.rst.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)    27497 2024-03-28 13:28:39.000000 Nuitka-2.1.5/nuitka/reports/Reports.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/reports/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.091591 Nuitka-2.1.5/nuitka/specs/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5943 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/specs/BuiltinBytesOperationSpecs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2818 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/specs/BuiltinDictOperationSpecs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2573 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/specs/BuiltinListOperationSpecs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    26786 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/specs/BuiltinParameterSpecs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6097 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/specs/BuiltinStrOperationSpecs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1191 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/specs/BuiltinTypeOperationSpecs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4834 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/specs/BuiltinUnicodeOperationSpecs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6244 2024-03-11 17:07:05.000000 Nuitka-2.1.5/nuitka/specs/HardImportSpecs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    18739 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/specs/ParameterSpecs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/specs/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.091591 Nuitka-2.1.5/nuitka/tools/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1631 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/Basics.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.091591 Nuitka-2.1.5/nuitka/tools/commercial/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      847 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/commercial/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.091591 Nuitka-2.1.5/nuitka/tools/data_composer/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15004 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/data_composer/DataComposer.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/data_composer/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1338 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/data_composer/__main__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.091591 Nuitka-2.1.5/nuitka/tools/environments/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2481 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/environments/CreateEnvironment.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4199 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/environments/Virtualenv.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/environments/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.091591 Nuitka-2.1.5/nuitka/tools/general/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/general/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.091591 Nuitka-2.1.5/nuitka/tools/general/dll_report/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/general/dll_report/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2352 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/general/dll_report/__main__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.091591 Nuitka-2.1.5/nuitka/tools/general/find_module/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3953 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/general/find_module/FindModuleCode.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/general/find_module/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.091591 Nuitka-2.1.5/nuitka/tools/onefile_compressor/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12545 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/onefile_compressor/OnefileCompressor.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/onefile_compressor/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1343 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/onefile_compressor/__main__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.091591 Nuitka-2.1.5/nuitka/tools/podman/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1905 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/podman/Podman.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/podman/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11623 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/podman/__main__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.091591 Nuitka-2.1.5/nuitka/tools/profiler/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/profiler/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2561 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/profiler/__main__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.091591 Nuitka-2.1.5/nuitka/tools/scanning/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3590 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/scanning/DisplayPackageDLLs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2314 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/scanning/DisplayPackageData.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/scanning/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.091591 Nuitka-2.1.5/nuitka/tools/specialize/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    51531 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/specialize/CTypeDescriptions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7717 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/specialize/Common.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    39659 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/specialize/SpecializeC.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    35715 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/specialize/SpecializePython.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/specialize/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.091591 Nuitka-2.1.5/nuitka/tools/testing/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    55682 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/testing/Common.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1516 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/testing/Constructs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10024 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/testing/OutputComparison.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1311 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/testing/Pythons.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8061 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/testing/RuntimeTracing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5413 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/testing/SearchModes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3408 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/testing/Valgrind.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/testing/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.091591 Nuitka-2.1.5/nuitka/tools/testing/check_reference_counts/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/testing/check_reference_counts/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3095 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/testing/check_reference_counts/__main__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.091591 Nuitka-2.1.5/nuitka/tools/testing/compare_with_cpython/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/testing/compare_with_cpython/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    29877 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/testing/compare_with_cpython/__main__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.091591 Nuitka-2.1.5/nuitka/tools/testing/find_sxs_modules/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/testing/find_sxs_modules/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1980 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/testing/find_sxs_modules/__main__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.091591 Nuitka-2.1.5/nuitka/tools/testing/measure_construct_performance/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/testing/measure_construct_performance/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8758 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/testing/measure_construct_performance/__main__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.091591 Nuitka-2.1.5/nuitka/tools/testing/run_nuitka_tests/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/testing/run_nuitka_tests/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    35342 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/testing/run_nuitka_tests/__main__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.091591 Nuitka-2.1.5/nuitka/tools/watch/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3476 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/watch/GitHub.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tools/watch/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    20868 2024-03-04 15:35:30.000000 Nuitka-2.1.5/nuitka/tools/watch/__main__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.091591 Nuitka-2.1.5/nuitka/tree/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    50370 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/Building.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    75150 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/ComplexCallHelperFunctions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1733 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/Extractions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2604 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/InternalModule.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1544 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/Operations.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2840 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/ReformulationAssertStatements.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    43101 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/ReformulationAssignmentStatements.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2981 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/ReformulationBooleanExpressions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11746 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/ReformulationCallExpressions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15446 2024-03-14 10:27:18.000000 Nuitka-2.1.5/nuitka/tree/ReformulationClasses.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    38235 2024-03-14 10:27:18.000000 Nuitka-2.1.5/nuitka/tree/ReformulationClasses3.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6523 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/ReformulationComparisonExpressions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    22175 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/ReformulationContractionExpressions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11196 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/ReformulationDictionaryCreation.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14757 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/ReformulationExecStatements.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7858 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/ReformulationForLoopStatements.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    30821 2024-03-11 17:07:05.000000 Nuitka-2.1.5/nuitka/tree/ReformulationFunctionStatements.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14095 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/ReformulationImportStatements.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6630 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/ReformulationLambdaExpressions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    21311 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/ReformulationMatchStatements.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2442 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/ReformulationMultidist.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7608 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/ReformulationNamespacePackages.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4711 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/ReformulationPrintStatements.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15606 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/ReformulationSequenceCreation.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4857 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/ReformulationSubscriptExpressions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14948 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/ReformulationTryExceptStatements.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7014 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/ReformulationTryFinallyStatements.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5707 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/ReformulationWhileLoopStatements.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14439 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/ReformulationWithStatements.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3852 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/ReformulationYieldExpressions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13212 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/SourceHandling.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3790 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/SyntaxErrors.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    23005 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/TreeHelpers.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    20465 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/VariableClosure.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/tree/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.091591 Nuitka-2.1.5/nuitka/utils/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3020 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/utils/AppDirs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4148 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/utils/CStrings.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6395 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/utils/CommandLineOptions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14981 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/utils/Distributions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6413 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/utils/Download.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13185 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/utils/Execution.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    41401 2024-03-28 13:28:39.000000 Nuitka-2.1.5/nuitka/utils/FileOperations.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3753 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/utils/Hashing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2395 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/utils/Images.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10121 2024-03-04 15:32:38.000000 Nuitka-2.1.5/nuitka/utils/Importing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7884 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/utils/InstalledPythons.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2257 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/utils/InstanceCounters.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4586 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/utils/Jinja2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1271 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/utils/Json.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4477 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/utils/MacOSApp.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5092 2024-03-22 08:13:25.000000 Nuitka-2.1.5/nuitka/utils/MemoryUsage.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9951 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/utils/ModuleNames.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4588 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/utils/ReExecute.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1889 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/utils/Rest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    23857 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/utils/SharedLibraries.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3697 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/utils/Shebang.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3687 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/utils/Signing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2084 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/utils/SlotMetaClasses.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6603 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/utils/StaticLibraries.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2634 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/utils/ThreadedExecutor.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2798 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/utils/Timing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11527 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/utils/Utils.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10606 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/utils/WindowsFileUsage.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    19837 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/utils/WindowsResources.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7014 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/utils/Yaml.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/nuitka/utils/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.5/pyproject.toml
--rw-r--r--   0 hayen     (1000) hayen     (2000)       38 2024-04-06 13:33:50.111591 Nuitka-2.1.5/setup.cfg
--rw-r--r--   0 hayen     (1000) hayen     (2000)    16677 2024-03-04 14:35:43.000000 Nuitka-2.1.5/setup.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.091591 Nuitka-2.1.5/tests/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/basics/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1798 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/AssertsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5966 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/AssignmentsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5910 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/AssignmentsTest32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4086 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/BranchingTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1136 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/BuiltinOverload.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3781 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/BuiltinSuperTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17112 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/BuiltinsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      898 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/ClassMinimalTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4796 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/ClassesTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3446 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/ClassesTest32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1438 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/ClassesTest34.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4729 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/ComparisonChainsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4672 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/ConstantsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1027 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/ConstantsTest27.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1661 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/DecoratorsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2349 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/DefaultParametersTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1159 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/DoubleDeletionsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      838 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/EmptyModuleTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14418 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/ExceptionRaisingTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      993 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/ExceptionRaisingTest32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1490 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/ExceptionRaisingTest33.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6779 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/ExecEvalTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1449 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/ExtremeClosureTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1690 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/FunctionObjectsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12367 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/FunctionsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3635 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/FunctionsTest32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2659 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/FunctionsTest_2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      922 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/FutureTest32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5841 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/GeneratorExpressionsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1073 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/GeneratorExpressionsTest_37.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3856 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/GlobalStatementTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1318 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/HelloWorldTest_2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2501 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/ImportingTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1328 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/InplaceOperationsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4259 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/InspectionTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1536 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/InspectionTest_35.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1650 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/InspectionTest_36.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1703 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/LambdasTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2763 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/LateClosureAssignmentTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2955 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/ListContractionsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3361 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/LoopingTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1568 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/MainProgramsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1957 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/ModuleAttributesTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2008 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/OperatorsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14935 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/OrderChecksTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1859 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/OrderChecksTest27.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1484 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/OverflowFunctionsTest_2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5885 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/ParameterErrorsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1931 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/ParameterErrorsTest32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      895 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/PrintFutureTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1444 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/PrintingTest_2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      910 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/RecursionTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    24719 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/ReferencingTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2109 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/ReferencingTest27.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7850 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/ReferencingTest33.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5041 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/ReferencingTest35.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5478 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/ReferencingTest36.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2932 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/ReferencingTest_2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1662 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/SlotsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1191 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/ThreadedGeneratorsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    22998 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/TrickAssignmentsTest32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1573 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/TrickAssignmentsTest35.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1820 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/TrickAssignmentsTest_2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2118 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/TryContinueFinallyTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2244 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/TryExceptContinueTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2307 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/TryExceptFinallyTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2336 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/TryExceptFramesTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2874 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/TryReturnFinallyTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2360 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/TryYieldFinallyTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1125 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/UnicodeTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1909 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/UnpackingTest35.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2143 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/VarargsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4913 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/WithStatementsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3103 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/YieldFromTest33.py
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     3851 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/run_all.py
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     2302 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/basics/run_xml.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/onefile/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1341 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/onefile/HelloWorldTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1339 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/onefile/KeyboardInterruptTest.py
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     5846 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/onefile/run_all.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/optimizations/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      991 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/optimizations/ArgumentTypes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1087 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/optimizations/Attributes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1053 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/optimizations/Calls.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      953 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/optimizations/Conditions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      941 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/optimizations/DecodingOperations.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1246 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/optimizations/FormatStrings36.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1183 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/optimizations/HardImports.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1007 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/optimizations/HardImports_2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      950 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/optimizations/Iterations.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1292 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/optimizations/Len.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1133 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/optimizations/Matching310.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2295 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/optimizations/Operations.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1365 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/optimizations/Subscripts.py
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     8827 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/optimizations/run_all.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/packages/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/packages/package_data_files_embedding/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1576 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/packages/package_data_files_embedding/PackageDataFilesEmbedding.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      956 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/packages/package_data_files_embedding/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/packages/package_import_success_after_failure/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2414 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/packages/package_import_success_after_failure/variable_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      975 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1201 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/packages/package_import_success_after_failure/variable_package/__init__.py
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     4138 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/packages/run_all.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.031591 Nuitka-2.1.5/tests/packages/sub_package/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/packages/sub_package/kitty/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1262 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/packages/sub_package/kitty/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      940 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/packages/sub_package/kitty/bigkitty.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      942 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/packages/sub_package/kitty/smallkitty.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/packages/sub_package/kitty/speak/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      961 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/packages/sub_package/kitty/speak/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1085 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/packages/sub_package/kitty/speak/hello.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      999 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/packages/sub_package/kitty/speak/miau.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1001 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/packages/sub_package/kitty/speak/purr.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.031591 Nuitka-2.1.5/tests/packages/top_level_attributes_3/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/packages/top_level_attributes_3/some_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2368 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/packages/top_level_attributes_3/some_package/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      939 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/packages/top_level_attributes_3/some_package/some_module.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/plugins/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/plugins/code_signing/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1202 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/plugins/code_signing/CodeSigningMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/plugins/data_files/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1474 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/plugins/data_files/DataFilesMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/plugins/data_files/data_files_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      956 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/plugins/data_files/data_files_package/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)        0 2022-10-08 09:07:15.000000 Nuitka-2.1.5/tests/plugins/data_files/data_files_package/lala.txt
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/plugins/data_files/data_files_package/sub_dir/
--rw-r--r--   0 hayen     (1000) hayen     (2000)        0 2022-10-08 09:07:15.000000 Nuitka-2.1.5/tests/plugins/data_files/data_files_package/sub_dir/lulu.txt
--rw-r--r--   0 hayen     (1000) hayen     (2000)      309 2024-01-26 12:30:51.000000 Nuitka-2.1.5/tests/plugins/data_files/test_case.nuitka-package.config.yml
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/plugins/parameters/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1051 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/plugins/parameters/ParametersMain.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2218 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/plugins/parameters/parameter-using-plugin.py
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     3892 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/plugins/run_all.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/absolute_import/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      899 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/absolute_import/AbsoluteImportMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/absolute_import/foobar/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      828 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/absolute_import/foobar/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1076 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/absolute_import/foobar/foobar.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      911 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/absolute_import/foobar/local.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      893 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/absolute_import/foobar/util.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/case_imports1/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      840 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/case_imports1/CasedImportingMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/case_imports1/path1/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      830 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/case_imports1/path1/Some_Module.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/case_imports1/path1/Some_Package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      831 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/case_imports1/path1/Some_Package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/case_imports1/path2/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      830 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/case_imports1/path2/some_module.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/case_imports1/path2/some_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      831 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/case_imports1/path2/some_package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/case_imports2/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      840 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/case_imports2/CasedImportingMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/case_imports2/path1/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/case_imports2/path1/some_module.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/case_imports2/path1/some_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/case_imports2/path1/some_package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/case_imports2/path2/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      830 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/case_imports2/path2/Some_Module.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/case_imports2/path2/Some_Package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      831 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/case_imports2/path2/Some_Package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/case_imports3/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1107 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/case_imports3/CasedImportingMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/case_imports3/path1/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      841 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/case_imports3/path1/Some_Module.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/case_imports3/path1/Some_Package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      842 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/case_imports3/path1/Some_Package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/case_imports3/path2/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      841 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/case_imports3/path2/Some_Module.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/case_imports3/path2/Some_Package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      842 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/case_imports3/path2/Some_Package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/cyclic_imports/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      833 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/cyclic_imports/CyclicImportsMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/cyclic_imports/cyclic_importing_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      907 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      907 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      874 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/dash_import/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      920 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/dash_import/DashImportMain.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      849 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/dash_import/dash-module.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      849 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/dash_import/plus+module.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/dash_main/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      841 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/dash_main/Dash-Main.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/deep/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      930 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/deep/DeepProgramMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/deep/some_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1012 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/deep/some_package/DeepBrother.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      941 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/deep/some_package/DeepChild.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/deep/some_package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/deep/some_package/deep_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      908 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/deep/some_package/deep_package/DeepDeepChild.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      984 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/deep/some_package/deep_package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/dunderinit_imports/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      826 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/dunderinit_imports/DunderInitImportsMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/dunderinit_imports/package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      829 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/dunderinit_imports/package/SubModule.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      889 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/dunderinit_imports/package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/import_variants/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1037 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/import_variants/ImportVariationsMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/import_variants/some_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      978 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/import_variants/some_package/Child1.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1130 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/import_variants/some_package/Child2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      854 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/import_variants/some_package/Child3.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1026 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/import_variants/some_package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/main_raises/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      943 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/main_raises/ErrorMain.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      841 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/main_raises/ErrorRaising.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/main_raises2/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1112 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/main_raises2/ErrorInFunctionMain.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      841 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/main_raises2/ErrorRaising.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/module_attributes/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1561 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/module_attributes/ModuleAttributesMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/module_attributes/package_level1/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1776 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/module_attributes/package_level1/Nearby1.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1643 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/module_attributes/package_level1/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/module_attributes/package_level1/package_level2/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1776 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1643 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/module_attributes/package_level1/package_level2/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/module_attributes/package_level1/package_level2/package_level3/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1776 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1643 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/module_exits/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      901 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/module_exits/ErrorExitingModule.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      899 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/module_exits/Main.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/module_object_replacing/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1110 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1391 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/module_object_replacing/SelfReplacingModule.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/multiprocessing_using/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1022 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/multiprocessing_using/foo/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/multiprocessing_using/foo/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      868 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/multiprocessing_using/foo/__main__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1791 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/multiprocessing_using/foo/entry.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/named_imports/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      878 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/named_imports/NamedImportsMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/named_imports/some_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/named_imports/some_package/SomeModule.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      856 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/named_imports/some_package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/named_imports/some_package/sub_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/named_imports/some_package/sub_package/SomeModule.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/package_code/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      832 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/package_code/PackageInitCodeMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/package_code/some_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      842 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/package_code/some_package/SomeModule.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      841 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/package_code/some_package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/package_contains_main/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      821 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/package_contains_main/PackageContainsMain.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/package_contains_main/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      833 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/package_contains_main/local.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/package_init_import/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      855 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/package_init_import/PackageInitImportMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/package_init_import/some_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1040 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/package_init_import/some_package/PackageLocal.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1201 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/package_init_import/some_package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/package_init_issue/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      821 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/package_init_issue/PackageInitIssueMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/package_init_issue/some_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      830 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/package_init_issue/some_package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/package_init_issue/some_package/child_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      830 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/package_init_issue/some_package/child_package/SomeModule.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      827 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/package_init_issue/some_package/child_package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/package_missing_init/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      958 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/package_missing_init/PackageMissingInitMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/package_missing_init/some_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      997 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/package_missing_init/some_package/some_module.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/package_missing_init/some_package/sub_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1009 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/package_module_collision/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      933 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/package_module_collision/Something/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      842 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/package_module_collision/Something/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      833 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/package_module_collision/something.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/package_overload/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      884 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/package_overload/Main.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/package_overload/foo/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      831 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/package_overload/foo/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/package_overload/foo/bar.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/package_overload/foo/bar2.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/package_prevents_submodule/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3004 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/package_prevents_submodule/some_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1111 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/package_prevents_submodule/some_package/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      833 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/package_prevents_submodule/some_package/some_module.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.031591 Nuitka-2.1.5/tests/programs/package_program/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/package_program/PackageAsMain/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      920 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/package_program/PackageAsMain/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1662 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/package_program/PackageAsMain/__main__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/pkgutil_itermodules/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1760 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/pkgutil_itermodules/some_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/pkgutil_itermodules/some_package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/pkgutil_itermodules/some_package/sub_package1/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/pkgutil_itermodules/some_package/sub_package2/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/pkgutil_usage/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1328 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/pkgutil_usage/PkgUtilUsageMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/pkgutil_usage/package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)       13 2021-04-22 06:31:42.000000 Nuitka-2.1.5/tests/programs/pkgutil_usage/package/DATA_FILE.txt
--rw-r--r--   0 hayen     (1000) hayen     (2000)       14 2022-10-08 09:07:15.000000 Nuitka-2.1.5/tests/programs/pkgutil_usage/package/DATA_FILE2.txt
--rw-r--r--   0 hayen     (1000) hayen     (2000)       14 2022-10-08 09:07:15.000000 Nuitka-2.1.5/tests/programs/pkgutil_usage/package/DATA_FILE3.txt
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1585 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/pkgutil_usage/package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/plugin_import/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      891 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/plugin_import/PluginImportMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/plugin_import/some_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      803 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/plugin_import/some_package/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      813 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/plugin_import/some_package/some_module.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/reimport_main_dynamic/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      943 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/reimport_main_static/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      930 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/reimport_main_static/ImportItselfStaticMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/relative_import/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      874 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/relative_import/RelativeImportMain.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/relative_import/dircache.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/resource_reader37/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1201 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/resource_reader37/ResourceReaderMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/resource_reader37/some_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)       13 2022-10-08 09:07:15.000000 Nuitka-2.1.5/tests/programs/resource_reader37/some_package/DATA_FILE.txt
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/resource_reader37/some_package/__init__.py
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     6646 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/run_all.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/stdlib_overload/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1203 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/stdlib_overload/StdlibOverloadMain.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      831 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/stdlib_overload/pyexpat.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/stdlib_overload/some_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/stdlib_overload/some_package/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      941 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/stdlib_overload/some_package/normal_importing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      842 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/stdlib_overload/some_package/pyexpat.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1268 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/stdlib_overload/some_package/star_importing.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/syntax_errors/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      822 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/syntax_errors/IndentationErroring.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      833 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/syntax_errors/SyntaxErroring.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1111 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/syntax_errors/SyntaxErrorsMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/unicode_bom/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      995 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/unicode_bom/UnicodeBomMain.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      878 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/unicode_bom/unicode_bom.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/programs/with space/
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)      858 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/programs/with space/Space Main.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.101591 Nuitka-2.1.5/tests/reflected/
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)    14194 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/reflected/compile_itself.py
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     1274 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/run-tests
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.111591 Nuitka-2.1.5/tests/standalone/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1090 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/BrotliUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2586 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/CtypesUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1950 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/DateutilsUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1168 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/FlaskUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1274 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/GiUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1022 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/GlfwUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1216 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/GtkUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1057 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/HexEncodingTest_2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1118 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/IdnaUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1215 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/LxmlUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1598 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/MatplotlibUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2570 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/MetadataPackagesUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1759 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/NumpyUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      979 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/OpenGLUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1479 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/PandasUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1098 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/PasslibUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1248 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/PendulumUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2106 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/PkgResourcesRequiresUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1099 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/PmwUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1369 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/PyQt5Plugins.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1253 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/PyQt5SSLSupport.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2198 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/PyQt5Using.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1203 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/PyQt6Plugins.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2168 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/PyQt6Using.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1789 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/PySide2Using.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1123 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/PySide6Plugins.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1789 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/PySide6Using.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1371 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/RsaUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1227 2024-03-22 08:13:25.000000 Nuitka-2.1.5/tests/standalone/SetuptoolsUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1005 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/ShlibUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1569 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/SocketUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1973 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/TkInterUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3260 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/Urllib3Using.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1232 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/Win32ComUsing.py
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     9912 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/run_all.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.111591 Nuitka-2.1.5/tests/standalone/zip_importer/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1296 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/standalone/zip_importer/ZipImporterMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-06 13:33:50.111591 Nuitka-2.1.5/tests/syntax/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      844 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/AsyncgenReturn36.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      818 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/AwaitInModule36.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      901 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/BreakWithoutLoop.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      824 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/ClassReturn.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1002 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/ClosureDel_2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      882 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/ContinueWithoutLoop.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      824 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/DuplicateArgument.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1142 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/ExecWithNesting_2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      858 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/FutureBraces.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      837 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/FutureUnknown.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1073 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/GeneratorExpressions38.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      911 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/GeneratorReturn_2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      825 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/GlobalForParameter.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1027 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/Importing32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      830 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/IndentationError.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      947 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/LateFutureImport.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      874 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/MisplacedFutureImport.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      832 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/ModuleReturn.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      915 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/NonAsciiWithoutEncoding_2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      827 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/NonlocalForParameter32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      900 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/NonlocalNotFound32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      939 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/StarImportExtra.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      900 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/SyntaxError.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      907 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/TryExceptAllNotLast.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      908 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/TryFinallyContinue_37.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      808 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/UnpackNoTuple.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      841 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/UnpackTwoStars32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      825 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/YieldFromInModule.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      837 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/YieldInAsync35.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      956 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/YieldInGenexp38.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      813 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/YieldInModule.py
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     2234 2024-03-04 14:35:43.000000 Nuitka-2.1.5/tests/syntax/run_all.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.837068 Nuitka-2.1.6/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      228 2024-03-04 14:35:43.000000 Nuitka-2.1.6/Changelog.rst
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   152282 2024-03-04 14:35:43.000000 Nuitka-2.1.6/Developer_Manual.rst
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11348 2021-04-22 06:31:42.000000 Nuitka-2.1.6/LICENSE.txt
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1707 2024-01-26 12:30:51.000000 Nuitka-2.1.6/MANIFEST.in
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.637068 Nuitka-2.1.6/Nuitka.egg-info/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    82956 2024-04-19 13:34:34.000000 Nuitka-2.1.6/Nuitka.egg-info/PKG-INFO
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    77774 2024-04-19 13:34:34.000000 Nuitka-2.1.6/Nuitka.egg-info/SOURCES.txt
+-rw-r--r--   0 hayen     (1000) hayen     (2000)        1 2024-04-19 13:34:34.000000 Nuitka-2.1.6/Nuitka.egg-info/dependency_links.txt
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      393 2024-04-19 13:34:34.000000 Nuitka-2.1.6/Nuitka.egg-info/entry_points.txt
+-rw-r--r--   0 hayen     (1000) hayen     (2000)        1 2024-02-02 15:24:24.000000 Nuitka-2.1.6/Nuitka.egg-info/not-zip-safe
+-rw-r--r--   0 hayen     (1000) hayen     (2000)        7 2024-04-19 13:34:34.000000 Nuitka-2.1.6/Nuitka.egg-info/top_level.txt
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    82956 2024-04-19 13:34:34.837068 Nuitka-2.1.6/PKG-INFO
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    80812 2024-03-04 14:35:43.000000 Nuitka-2.1.6/README.rst
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.637068 Nuitka-2.1.6/bin/
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     1166 2024-03-04 14:35:43.000000 Nuitka-2.1.6/bin/autoformat-nuitka-source
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     1165 2024-03-04 14:35:43.000000 Nuitka-2.1.6/bin/check-nuitka-with-pylint
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     1181 2024-03-04 14:35:43.000000 Nuitka-2.1.6/bin/compare_with_cpython
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     3105 2024-03-04 14:35:43.000000 Nuitka-2.1.6/bin/compare_with_xml
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     1194 2024-03-04 14:35:43.000000 Nuitka-2.1.6/bin/measure-construct-performance
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     1716 2024-03-04 14:35:43.000000 Nuitka-2.1.6/bin/nuitka
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     1716 2024-03-04 14:35:43.000000 Nuitka-2.1.6/bin/nuitka-run
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.637068 Nuitka-2.1.6/doc/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.637068 Nuitka-2.1.6/doc/Logo/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1797 2024-03-04 14:35:43.000000 Nuitka-2.1.6/doc/Logo/Nuitka-Logo-Horizontal.svg
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1553 2024-03-04 14:35:43.000000 Nuitka-2.1.6/doc/Logo/Nuitka-Logo-Symbol.svg
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1793 2024-03-04 14:35:43.000000 Nuitka-2.1.6/doc/Logo/Nuitka-Logo-Vertical.svg
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.637068 Nuitka-2.1.6/doc/images/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7585 2021-04-22 06:31:42.000000 Nuitka-2.1.6/doc/images/Nuitka-Logo-Horizontal.png
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4452 2021-04-22 06:31:42.000000 Nuitka-2.1.6/doc/images/Nuitka-Logo-Symbol.png
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9828 2022-01-09 15:54:20.000000 Nuitka-2.1.6/doc/images/Nuitka-Logo-Vertical.png
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    33808 2024-03-11 17:07:05.000000 Nuitka-2.1.6/doc/nuitka-run.1
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    33832 2024-03-11 17:07:05.000000 Nuitka-2.1.6/doc/nuitka.1
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.637068 Nuitka-2.1.6/lib/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4640 2024-03-04 14:35:43.000000 Nuitka-2.1.6/lib/hints.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.637068 Nuitka-2.1.6/misc/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      924 2024-03-04 14:35:43.000000 Nuitka-2.1.6/misc/nuitka-run.bat
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1061 2024-03-04 14:35:43.000000 Nuitka-2.1.6/misc/nuitka.bat
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.647068 Nuitka-2.1.6/nuitka/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7560 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/Builtins.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5787 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/BytecodeCaching.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3800 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/Bytecodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1855 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/CacheCleanup.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11181 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/Constants.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2479 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/Errors.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10335 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/HardImportRegistry.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    38348 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/MainControl.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8616 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/ModuleRegistry.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    62344 2024-03-22 08:13:25.000000 Nuitka-2.1.6/nuitka/OptionParsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    74907 2024-04-06 13:33:42.000000 Nuitka-2.1.6/nuitka/Options.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5276 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/OutputDirectories.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14940 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/PostProcessing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6797 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/Progress.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9654 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/PythonFlavors.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4093 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/PythonOperators.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14557 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/PythonVersions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8989 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/Serialization.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4703 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/SourceCodeReferences.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13335 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/Tracing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3513 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/TreeXML.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15470 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/Variables.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2466 2024-04-19 13:34:22.000000 Nuitka-2.1.6/nuitka/Version.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6373 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/__main__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5604 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/__past__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.647068 Nuitka-2.1.6/nuitka/build/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    36393 2024-03-11 17:07:05.000000 Nuitka-2.1.6/nuitka/build/Backend.scons
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8583 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/CCompilerVersion.scons
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3485 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/DataComposerInterface.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17733 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/Onefile.scons
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14643 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/SconsCaching.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    35437 2024-03-11 17:07:05.000000 Nuitka-2.1.6/nuitka/build/SconsCompilerSettings.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5592 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/SconsHacks.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15933 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/SconsInterface.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2704 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/SconsProgress.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13210 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/SconsSpawn.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    26957 2024-04-19 13:34:22.000000 Nuitka-2.1.6/nuitka/build/SconsUtils.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.577068 Nuitka-2.1.6/nuitka/build/include/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.647068 Nuitka-2.1.6/nuitka/build/include/nuitka/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8001 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/allocator.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3499 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/builtins.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5196 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/calling.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2006 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/checkers.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1123 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/checksum_tools.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9333 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/compiled_asyncgen.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2195 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/compiled_cell.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9233 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/compiled_coroutine.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17661 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/compiled_frame.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7267 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/compiled_function.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9189 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/compiled_generator.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1866 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/compiled_method.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7688 2024-04-19 13:34:22.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/constants.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1345 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/constants_blob.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1187 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/environment_variables.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1872 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/environment_variables_system.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5302 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/exception_groups.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    34114 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/exceptions.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3792 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/filesystem_paths.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6474 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/freelists.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    86326 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/hedley.h
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.647068 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3698 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/attributes.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2692 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/boolean.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1233 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/bytearrays.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1164 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/bytes.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11894 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/calling_generated.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13169 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/comparisons_eq.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10645 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/comparisons_ge.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10644 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/comparisons_gt.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13169 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/comparisons_le.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13168 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/comparisons_lt.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10645 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/comparisons_ne.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1834 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/complex.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13551 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/dictionaries.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1235 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/floats.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4291 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/import_hard.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1827 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/indexes.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2970 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/ints.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9599 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/iterators.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3601 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/lists.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1662 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/lists_generated.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1386 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/mappings.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4671 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12714 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_binary_add.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5692 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_binary_bitand.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5670 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_binary_bitor.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5692 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5451 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_binary_divmod.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5489 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5144 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_binary_lshift.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2828 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_binary_matmult.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15807 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_binary_mod.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13239 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_binary_mult.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5820 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4743 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_binary_pow.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5144 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_binary_rshift.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5853 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_binary_sub.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5467 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_binary_truediv.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    20173 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_builtin_types.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8699 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_inplace_add.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3796 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3782 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3796 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4875 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3040 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2756 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10655 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_inplace_mod.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9230 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_inplace_mult.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5176 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4378 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_inplace_pow.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3040 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5004 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_inplace_sub.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4855 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3381 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/raising.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2367 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/rangeobjects.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1175 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/richcomparisons.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1141 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/sequences.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1054 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/sets.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8750 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/slices.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1363 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/strings.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17975 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/subscripts.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5749 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helper/tuples.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    16704 2024-04-19 13:34:22.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/helpers.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6150 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/importing.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12979 2022-10-08 15:33:22.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/incbin.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15484 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/prelude.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2899 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/printing.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1811 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/python_pgo.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2343 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/safe_string_ops.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3809 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/threading.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3447 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/tracing.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3135 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/include/nuitka/unfreezing.h
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.607068 Nuitka-2.1.6/nuitka/build/inline_copy/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.647068 Nuitka-2.1.6/nuitka/build/inline_copy/appdirs/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1097 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/appdirs/LICENSE.txt
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    24824 2022-10-08 09:07:15.000000 Nuitka-2.1.6/nuitka/build/inline_copy/appdirs/appdirs.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.647068 Nuitka-2.1.6/nuitka/build/inline_copy/atomicwrites/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1069 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/atomicwrites/LICENSE
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6794 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/atomicwrites/atomicwrites.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.647068 Nuitka-2.1.6/nuitka/build/inline_copy/bin/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1695 2023-11-22 13:25:43.000000 Nuitka-2.1.6/nuitka/build/inline_copy/bin/scons.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.587068 Nuitka-2.1.6/nuitka/build/inline_copy/clcache/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.647068 Nuitka-2.1.6/nuitka/build/inline_copy/clcache/clcache/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1585 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/clcache/clcache/LICENSE
+-rw-r--r--   0 hayen     (1000) hayen     (2000)       93 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/clcache/clcache/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    65424 2023-03-17 17:23:10.000000 Nuitka-2.1.6/nuitka/build/inline_copy/clcache/clcache/caching.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.647068 Nuitka-2.1.6/nuitka/build/inline_copy/colorama/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1491 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/colorama/LICENSE.txt
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.667068 Nuitka-2.1.6/nuitka/build/inline_copy/colorama/colorama/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      243 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/colorama/colorama/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2522 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/colorama/colorama/ansi.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10517 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1915 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/colorama/colorama/initialise.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5404 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/colorama/colorama/win32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6438 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/colorama/colorama/winterm.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.667068 Nuitka-2.1.6/nuitka/build/inline_copy/glob2/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1359 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/glob2/LICENSE
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.667068 Nuitka-2.1.6/nuitka/build/inline_copy/glob2/glob2/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)       82 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/glob2/glob2/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6859 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/glob2/glob2/compat.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4463 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/glob2/glob2/fnmatch.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8304 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/glob2/glob2/impl.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.667068 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1467 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/LICENSE.rst
+-rw-r--r--   0 hayen     (1000) hayen     (2000)       85 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/README.rst
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.667068 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2423 2022-10-08 09:07:15.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2685 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/_compat.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1726 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12719 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/bccache.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    65386 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/compiler.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1626 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/constants.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12281 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/debug.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1400 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/defaults.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    50849 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/environment.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4428 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    24500 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/ext.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    36528 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/filters.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9197 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    28559 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/lexer.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17473 2022-10-08 09:07:15.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/loaders.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4340 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/meta.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7308 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    30853 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/nodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1722 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    35875 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/parser.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    27644 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/runtime.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17080 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4214 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/tests.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    20501 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/utils.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3316 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/visitor.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.667068 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1466 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/LICENSE.rst
+-rw-r--r--   0 hayen     (1000) hayen     (2000)       84 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/README.rst
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.667068 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2616 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2685 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1726 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12719 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    65386 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1626 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12281 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1400 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    50849 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4428 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    24500 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    36528 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9197 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    28559 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17474 2022-10-08 09:07:15.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4340 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7308 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    30853 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1722 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    35875 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    27644 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17080 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4214 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    20501 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3316 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.597068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.597068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.667068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    47844 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    33996 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8083 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    27693 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6938 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17622 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    96183 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7358 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    21540 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    16000 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9589 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.677068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4197 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   121420 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4164 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    49503 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.677068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1950 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1950 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1950 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1965 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2736 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2614 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8467 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.677068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9314 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3131 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1989 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2483 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1718 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1605 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2170 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4179 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1882 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15042 2024-01-26 12:30:51.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    39700 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12950 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.677068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4810 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3751 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3233 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2011 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14663 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.677068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14029 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    52665 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    40719 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    24133 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14053 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2305 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    34903 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    40510 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.687068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2166 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2433 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2859 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    18084 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.687068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2078 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2004 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9248 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2784 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14869 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    19499 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    20832 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3763 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5149 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2290 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2328 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2657 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    31283 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2379 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2267 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2681 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2720 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2796 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2147 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2936 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2935 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3432 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3785 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2777 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1711 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      142 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/dmd.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.687068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    29618 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3428 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2681 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2433 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1844 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3472 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4782 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2025 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2256 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2460 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2639 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1810 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2333 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2140 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1902 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2077 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2043 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    18600 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    25816 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3328 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8394 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3953 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2309 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2945 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6919 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4381 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4658 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4224 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2168 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13881 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1804 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11380 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    72761 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6841 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3579 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2618 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4375 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2827 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2513 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1991 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1819 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2123 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2502 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4695 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1927 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2349 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2473 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5992 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1831 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3730 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13016 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3415 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    48938 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.687068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3007 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3784 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4380 2024-01-26 12:30:51.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3557 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5612 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11034 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6824 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1563 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.687068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8120 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3596 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1818 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1742 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2465 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1776 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    19253 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    44500 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    19664 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7509 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2107 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.597068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.697068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    53545 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    34985 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13596 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    28403 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7533 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    20988 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    96818 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7752 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    22350 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    16068 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9565 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.697068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5239 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   135413 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5758 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    63474 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8354 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.697068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11500 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3180 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2227 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2739 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1767 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1654 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1460 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2219 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4476 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1931 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4003 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17055 2024-01-26 12:30:51.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    41186 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13880 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.707068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4853 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3812 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3643 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2328 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15053 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.707068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13779 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    53260 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    39394 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    26467 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14489 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    35863 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    42204 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.707068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2211 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    18207 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.717068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2152 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2057 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10674 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2855 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15165 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    33537 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    21762 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4464 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    50660 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1667 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2316 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2475 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2840 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8618 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2226 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2978 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2977 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1653 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3827 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3389 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.717068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      313 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3631 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3444 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8494 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1753 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.717068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    29765 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3472 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1630 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1977 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3686 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2580 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2948 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2655 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1645 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1859 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2765 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2386 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2189 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1944 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2123 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2085 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15791 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    26195 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13924 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4041 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2351 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2987 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7808 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4956 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5235 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4808 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2475 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14751 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1847 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12588 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    82939 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6883 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3663 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2660 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4904 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2877 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2567 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1652 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1868 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2088 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2176 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2366 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1658 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1976 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5335 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2583 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2515 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6756 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1873 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3773 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13982 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3201 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    53803 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.717068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3064 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3818 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4435 2024-01-26 12:30:51.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3643 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5579 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11655 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6504 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1647 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.717068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6869 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1784 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    19816 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9002 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2149 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.597068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.727068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    56578 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    35213 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11061 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    27408 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7884 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    21423 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    97269 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3979 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7515 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    21937 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    16583 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9430 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.727068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5126 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   136271 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6167 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    63768 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8183 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.727068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12836 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3087 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2107 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2630 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1674 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1536 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1311 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2076 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4356 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1805 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3860 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14831 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    41983 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14673 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.727068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7394 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4357 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3546 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1972 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15577 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.727068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13597 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    53509 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    42760 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    26676 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14272 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    36753 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    41191 2022-10-08 09:07:15.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.737068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2122 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15570 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.737068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2014 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1943 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13182 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2734 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15027 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    38783 2023-03-17 17:23:10.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    22570 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4368 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    32724 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1578 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2228 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2386 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2616 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7993 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2141 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1661 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2893 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2889 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1567 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3742 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3296 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.737068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      343 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3534 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3259 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7461 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1663 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3379 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1544 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1891 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3616 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2377 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2437 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2526 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1557 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1772 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2677 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2206 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2096 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1851 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1954 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1995 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    19180 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    25826 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2588 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.737068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4649 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7652 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6064 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3931 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2266 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2900 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8622 2022-10-08 09:07:15.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4577 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4517 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4113 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2387 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14473 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1752 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12902 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    84784 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6788 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3576 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2573 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4817 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2788 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2479 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1563 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1780 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1999 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2006 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2271 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1569 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1888 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4879 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2419 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2429 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6412 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1786 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3687 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12548 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4076 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    71693 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.737068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6632 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)        0 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15278 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.737068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3134 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3896 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4648 2024-01-26 12:30:51.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3536 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5588 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12708 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6785 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      353 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.737068 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4307 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1644 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3395 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    21614 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9295 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2032 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.737068 Nuitka-2.1.6/nuitka/build/inline_copy/markupsafe/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1467 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/markupsafe/LICENSE.rst
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.737068 Nuitka-2.1.6/nuitka/build/inline_copy/markupsafe/markupsafe/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10126 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      558 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4690 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1873 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.597068 Nuitka-2.1.6/nuitka/build/inline_copy/pkg_resources/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.737068 Nuitka-2.1.6/nuitka/build/inline_copy/pkg_resources/pkg_resources/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   107452 2022-10-08 09:07:15.000000 Nuitka-2.1.6/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      538 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.597068 Nuitka-2.1.6/nuitka/build/inline_copy/tqdm/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.737068 Nuitka-2.1.6/nuitka/build/inline_copy/tqdm/tqdm/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1595 2023-11-22 13:25:43.000000 Nuitka-2.1.6/nuitka/build/inline_copy/tqdm/tqdm/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      283 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/tqdm/tqdm/_main.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3687 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      283 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/tqdm/tqdm/_tqdm.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      307 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_notebook.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      888 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      596 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/tqdm/tqdm/_utils.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1106 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/tqdm/tqdm/auto.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      857 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1376 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/tqdm/tqdm/dask.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10790 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/tqdm/tqdm/notebook.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    57572 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/tqdm/tqdm/std.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6948 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/tqdm/tqdm/tk.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9726 2023-11-22 13:25:43.000000 Nuitka-2.1.6/nuitka/build/inline_copy/tqdm/tqdm/utils.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      167 2024-01-07 19:01:51.000000 Nuitka-2.1.6/nuitka/build/inline_copy/tqdm/tqdm/version.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.737068 Nuitka-2.1.6/nuitka/build/inline_copy/yaml/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1101 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml/LICENSE
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.737068 Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13170 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4883 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/composer.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    28639 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/constructor.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3851 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/cyaml.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2837 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/dumper.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    43006 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/emitter.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2533 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/error.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2445 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/events.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2061 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/loader.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1440 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/nodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    25495 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/parser.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6794 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/reader.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14184 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/representer.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8999 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/resolver.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    51277 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/scanner.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4165 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/serializer.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2573 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/tokens.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.737068 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1101 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/LICENSE
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.747068 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9776 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4921 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/composer.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    25145 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/constructor.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3290 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2719 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/dumper.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    43298 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/emitter.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2559 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/error.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2445 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/events.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1132 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/loader.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1440 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/nodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    25542 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/parser.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6746 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/reader.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17711 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/representer.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9122 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/resolver.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    52446 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/scanner.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4171 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/serializer.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2573 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/tokens.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.747068 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1101 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/LICENSE
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.747068 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9607 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4881 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/composer.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    25554 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/constructor.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3294 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2723 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/dumper.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    42954 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/emitter.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2533 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/error.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2445 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/events.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1138 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/loader.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1440 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/nodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    25495 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/parser.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6854 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/reader.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14097 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/representer.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8970 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/resolver.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    51695 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/scanner.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4165 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/serializer.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2573 2022-01-09 15:54:20.000000 Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/tokens.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.747068 Nuitka-2.1.6/nuitka/build/inline_copy/zlib/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1002 2023-11-22 13:25:43.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zlib/LICENSE
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    31605 2023-11-22 13:25:43.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zlib/crc32.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   591749 2023-11-22 13:25:43.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zlib/crc32.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    16682 2023-11-22 13:25:43.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zlib/zconf.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    96778 2023-11-22 13:25:43.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zlib/zlib.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7247 2023-11-22 13:25:43.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zlib/zutil.h
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.747068 Nuitka-2.1.6/nuitka/build/inline_copy/zstd/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1530 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zstd/LICENSE.txt
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.747068 Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    18198 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/bitstream.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10157 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/compiler.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4455 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/cpu.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3763 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/debug.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13662 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/entropy_common.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3009 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/error_private.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2441 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/error_private.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    34422 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/fse.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14748 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/fse_decompress.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    20216 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/huf.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13930 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/mem.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    26976 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/xxhash.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11706 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/xxhash.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2728 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/zstd_common.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2497 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/zstd_deps.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3828 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/zstd_errors.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15880 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/zstd_internal.h
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.747068 Nuitka-2.1.6/nuitka/build/inline_copy/zstd/decompress/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    54982 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9164 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1321 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    80283 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    66784 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2253 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7906 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   138334 2021-04-22 06:31:42.000000 Nuitka-2.1.6/nuitka/build/inline_copy/zstd/zstd.h
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.767068 Nuitka-2.1.6/nuitka/build/static_src/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    84761 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/CompiledAsyncgenType.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9142 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/CompiledCellType.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    58739 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/CompiledCodeHelpers.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    73577 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/CompiledCoroutineType.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    40760 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/CompiledFrameType.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   109285 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/CompiledFunctionType.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    63983 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/CompiledGeneratorType.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    56631 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    22473 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/CompiledMethodType.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    19054 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersAllocator.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    38264 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersAttributes.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    23678 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersBuiltin.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   114017 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersBuiltinTypeMethods.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3062 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersBytes.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13376 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersCalling.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   481627 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersCallingGenerated.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2065 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersChecksumTools.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3051 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersClasses.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   318307 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersComparisonEq.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4762 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersComparisonEqUtils.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   313126 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersComparisonGe.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   312537 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersComparisonGt.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   316340 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersComparisonLe.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   315751 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersComparisonLt.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   315055 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersComparisonNe.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    36776 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersConstantsBlob.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    20361 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersDeepcopy.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    39584 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersDictionaries.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    26620 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersDictionariesGenerated.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2066 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersDumpBacktraces.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2194 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersEnvironmentVariables.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2979 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersEnvironmentVariablesSystem.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7145 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersExceptions.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8349 2024-04-19 13:34:22.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersFiles.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    28806 2024-03-28 13:28:39.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersFilesystemPaths.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2455 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersFloats.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1803 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersHeapStorage.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    16080 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersImport.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    16403 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersImportHard.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    19996 2024-03-28 13:28:39.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersLists.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13944 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersListsGenerated.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1669 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersMappings.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3587 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersMatching.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   181603 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryAdd.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    16729 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    77972 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryBitand.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    77811 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryBitor.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    77972 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryBitxor.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    68218 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryDivmod.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1265 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    69479 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6300 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    83954 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryLshift.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13805 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryMatmult.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   183867 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryMod.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   188543 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryMult.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3433 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    67184 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    79484 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryPow.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1052 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    77854 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryRshift.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    70494 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinarySub.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    68736 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryTruediv.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   150679 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationInplaceAdd.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4240 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    53253 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationInplaceBitand.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    53151 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationInplaceBitor.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    53253 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationInplaceBitxor.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    77119 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    47857 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationInplaceLshift.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17771 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationInplaceMatmult.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   136385 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationInplaceMod.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   142240 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationInplaceMult.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    74749 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    83262 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationInplacePow.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    45341 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationInplaceRshift.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    82871 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationInplaceSub.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    76950 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationInplaceTruediv.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3394 2024-03-22 08:13:25.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersProfiling.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3840 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersPythonPgo.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15663 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersRaising.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3868 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersSafeStrings.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3759 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersSequences.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1975 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersSlices.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    27056 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersStrings.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4181 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersTuples.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5628 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/HelpersTypes.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12136 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/InspectPatcher.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    54017 2024-04-06 13:33:42.000000 Nuitka-2.1.6/nuitka/build/static_src/MainProgram.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    63759 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/MetaPathBasedLoader.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4827 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6651 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    21896 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    31916 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/OnefileBootstrap.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8050 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/build/static_src/OnefileSplashScreen.cpp
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.767068 Nuitka-2.1.6/nuitka/code_generation/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6491 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/AsyncgenCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10821 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/AttributeCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    21894 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/BinaryOperationHelperDefinitions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2371 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/BranchCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17005 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/BuiltinCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    36111 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/CallCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4958 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/ClassCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    52589 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/CodeGeneration.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2408 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/CodeHelperSelection.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14272 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/CodeHelpers.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5083 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/CodeObjectCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17645 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/ComparisonCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4479 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/ComparisonHelperDefinitions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7368 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/ConditionalCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6661 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/ConstantCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    33901 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/Contexts.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8589 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/CoroutineCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1607 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/CtypesCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    28934 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/DictCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2158 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/Emission.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9415 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/ErrorCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12951 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/EvalCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9011 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/ExceptionCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7383 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2126 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/ExpressionCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17804 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/FrameCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    28337 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/FunctionCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7828 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/GeneratorCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6404 2024-04-19 13:34:22.000000 Nuitka-2.1.6/nuitka/code_generation/GlobalConstants.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6985 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/GlobalsLocalsCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1870 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/IdCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14684 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/ImportCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1429 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/Indentation.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1574 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/IndexCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1066 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/InjectCCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3567 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/IntegerCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12211 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/IteratorCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2055 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/LabelCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2645 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/LineNumberCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    16152 2024-03-28 13:28:39.000000 Nuitka-2.1.6/nuitka/code_generation/ListCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6658 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/LoaderCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10016 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/LocalsDictCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3174 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/LoopCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1638 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/MatchCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6455 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/ModuleCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8225 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/Namify.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12685 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/OperationCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    30146 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/PackageResourceCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3054 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/PrintCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5670 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/PythonAPICodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13251 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/RaisingCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3476 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/Reports.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5267 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/ReturnCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6591 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/SetCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14005 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/SliceCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10087 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/StringCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8302 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/SubscriptCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11208 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/TryCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3840 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/TupleCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14747 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/VariableCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9154 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/VariableDeclarations.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8129 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/YieldCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.767068 Nuitka-2.1.6/nuitka/code_generation/c_types/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6102 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/c_types/CTypeBases.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3432 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/c_types/CTypeBooleans.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1837 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/c_types/CTypeCFloats.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1411 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/c_types/CTypeCLongs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3642 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/c_types/CTypeModuleDictVariables.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5161 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5244 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/c_types/CTypeNuitkaInts.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3988 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/c_types/CTypeNuitkaVoids.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    19696 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/c_types/CTypePyObjectPointers.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2885 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/c_types/CTypeVoids.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/c_types/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.777068 Nuitka-2.1.6/nuitka/code_generation/templates/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2948 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8994 2024-04-19 13:34:22.000000 Nuitka-2.1.6/nuitka/code_generation/templates/CodeTemplatesConstants.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3040 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates/CodeTemplatesCoroutines.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2358 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates/CodeTemplatesExceptions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6483 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates/CodeTemplatesFrames.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3460 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates/CodeTemplatesFunction.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3390 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2409 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates/CodeTemplatesIterators.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4535 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates/CodeTemplatesLoader.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    22938 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates/CodeTemplatesModules.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6800 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates/CodeTemplatesVariables.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2508 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates/TemplateDebugWrapper.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.777068 Nuitka-2.1.6/nuitka/code_generation/templates_c/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11318 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5829 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    23986 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5438 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1755 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1693 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2706 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13624 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1894 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperImportHard.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2618 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperLongTools.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1394 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperObjectTools.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7047 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12700 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4138 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1938 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1968 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4081 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7257 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4142 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3710 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4379 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11758 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    19167 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2693 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3485 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11336 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15540 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2829 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperSlotsList.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10271 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2407 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2870 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2834 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3128 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.777068 Nuitka-2.1.6/nuitka/containers/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1468 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/containers/Namedtuples.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6553 2022-10-08 09:07:15.000000 Nuitka-2.1.6/nuitka/containers/OrderedDicts.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      554 2022-10-08 09:07:15.000000 Nuitka-2.1.6/nuitka/containers/OrderedSets.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4430 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/containers/OrderedSetsFallback.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/containers/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.777068 Nuitka-2.1.6/nuitka/distutils/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2308 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/distutils/Build.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15025 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/distutils/DistutilCommands.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/distutils/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.777068 Nuitka-2.1.6/nuitka/finalizations/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1257 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/finalizations/Finalization.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6059 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/finalizations/FinalizeMarkups.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/finalizations/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.777068 Nuitka-2.1.6/nuitka/freezer/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7778 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/freezer/DependsExe.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2616 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/freezer/DllDependenciesCommon.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12609 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/freezer/DllDependenciesMacOS.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7469 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/freezer/DllDependenciesPosix.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6633 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/freezer/DllDependenciesWin32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11979 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/freezer/ImportDetection.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17908 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/freezer/IncludedDataFiles.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11415 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/freezer/IncludedEntryPoints.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9551 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/freezer/Onefile.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11988 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/freezer/Standalone.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/freezer/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.777068 Nuitka-2.1.6/nuitka/importing/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11040 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/importing/IgnoreListing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2932 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/importing/ImportCache.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7560 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/importing/ImportResolving.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    31922 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/importing/Importing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4869 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/importing/PreloadedPackages.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    18804 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/importing/Recursion.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12787 2024-04-06 13:33:42.000000 Nuitka-2.1.6/nuitka/importing/StandardLibrary.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/importing/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.787068 Nuitka-2.1.6/nuitka/nodes/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3670 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/AsyncgenNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4115 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/AttributeLookupNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13255 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/AttributeNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   378777 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/AttributeNodesGenerated.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3856 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/BuiltinAllNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4131 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/BuiltinAnyNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2529 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/BuiltinComplexNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1731 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/BuiltinDecodingNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2760 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/BuiltinDecoratorNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4727 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/BuiltinDictNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4981 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/BuiltinFormatNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2275 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/BuiltinHashNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1457 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/BuiltinInputNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5367 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/BuiltinIntegerNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12756 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/BuiltinIteratorNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2029 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/BuiltinLenNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3639 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/BuiltinNextNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3787 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/BuiltinOpenNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   245569 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    18648 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/BuiltinRangeNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9100 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/BuiltinRefNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3353 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/BuiltinSumNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13576 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/BuiltinTypeNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1606 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/BuiltinVarsNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    26146 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/BytesNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6511 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/CallNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1583 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/Checkers.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   623739 2024-03-11 17:07:05.000000 Nuitka-2.1.6/nuitka/nodes/ChildrenHavingMixins.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8480 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/ClassNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6618 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/CodeObjectSpecs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    21716 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/ComparisonNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    30300 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/ConditionalNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    46568 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/ConstantRefNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12246 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/ContainerMakingNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2867 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/ContainerOperationNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4614 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/CoroutineNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1747 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/CtypesNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    51054 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/DictionaryNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7889 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/ExceptionNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7408 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/ExecEvalNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    44902 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/ExpressionBases.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    55109 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/ExpressionBasesGenerated.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    21311 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/ExpressionShapeMixins.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12024 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/FrameNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3577 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/FunctionAttributeNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    39667 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/FunctionNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5409 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/FutureSpecs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6288 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/GeneratorNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6961 2024-04-06 13:33:42.000000 Nuitka-2.1.6/nuitka/nodes/GlobalsLocalsNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    92183 2024-03-11 17:07:05.000000 Nuitka-2.1.6/nuitka/nodes/HardImportNodesGenerated.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5378 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/ImportHardNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    47515 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/ImportNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2766 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/IndicatorMixins.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1534 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/InjectCNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11519 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/IterationHandles.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11035 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/KeyValuePairNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    16821 2024-03-11 17:07:05.000000 Nuitka-2.1.6/nuitka/nodes/ListOperationNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    23177 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/LocalsDictNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15007 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/LocalsScopes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15995 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/LoopNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1745 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/MatchNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6567 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/ModuleAttributeNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    32713 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/ModuleNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    24461 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/NodeBases.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15147 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/NodeMakingHelpers.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5580 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/NodeMetaClasses.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    31948 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/OperatorNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8975 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/OperatorNodesUnary.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5229 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/OsSysNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12468 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/OutlineNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    34736 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/PackageMetadataNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12241 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/PackageResourceNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3440 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/PrintNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6805 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/ReturnNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4748 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/SideEffectNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12547 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/SliceNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    97361 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/StatementBasesGenerated.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9336 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/StatementNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    28691 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/StrNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3537 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/StringConcatenationNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8329 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/SubscriptNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17886 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/TryNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2438 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/TypeMatchNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11094 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/TypeNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    42396 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/VariableAssignNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10779 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/VariableDelNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4607 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/VariableNameNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    31228 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/VariableRefNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4781 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/VariableReleaseNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3937 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/YieldNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.787068 Nuitka-2.1.6/nuitka/nodes/shapes/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   157197 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/shapes/BuiltinTypeShapes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4420 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/shapes/ControlFlowDescriptions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5076 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/shapes/ShapeMixins.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    42509 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/shapes/StandardShapes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/nodes/shapes/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.787068 Nuitka-2.1.6/nuitka/optimizations/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3358 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/optimizations/BytecodeDemotion.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3953 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/optimizations/FunctionInlining.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2177 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/optimizations/Graphs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10866 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/optimizations/Optimization.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    52487 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/optimizations/OptimizeBuiltinCalls.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2288 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/optimizations/Tags.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    45089 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/optimizations/TraceCollections.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    24504 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/optimizations/ValueTraces.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/optimizations/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.787068 Nuitka-2.1.6/nuitka/pgo/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4932 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/pgo/PGO.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/pgo/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.797068 Nuitka-2.1.6/nuitka/plugins/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    56921 2024-03-28 13:28:39.000000 Nuitka-2.1.6/nuitka/plugins/PluginBase.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    59723 2024-03-14 10:27:18.000000 Nuitka-2.1.6/nuitka/plugins/Plugins.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/plugins/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.797068 Nuitka-2.1.6/nuitka/plugins/standard/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    30408 2024-03-14 10:27:18.000000 Nuitka-2.1.6/nuitka/plugins/standard/AntiBloatPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3510 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10754 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/plugins/standard/DataFilesPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5080 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/plugins/standard/DelvewheelPlugin.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.797068 Nuitka-2.1.6/nuitka/plugins/standard/DillPlugin/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1646 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/plugins/standard/DillPlugin/DillPlugin.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9826 2024-03-22 08:13:25.000000 Nuitka-2.1.6/nuitka/plugins/standard/DillPlugin/dill-postLoad.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2679 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/plugins/standard/DillPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    16277 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/plugins/standard/DllFilesPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2095 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/plugins/standard/EnumPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1938 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/plugins/standard/EventletPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1913 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/plugins/standard/GeventPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4017 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/plugins/standard/GiPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4854 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/plugins/standard/GlfwPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    32335 2024-04-19 13:34:22.000000 Nuitka-2.1.6/nuitka/plugins/standard/ImplicitImports.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5024 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/plugins/standard/KivyPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8823 2024-03-28 13:28:39.000000 Nuitka-2.1.6/nuitka/plugins/standard/MatplotlibPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7080 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/plugins/standard/MultiprocessingPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1220 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/plugins/standard/NumpyPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7433 2024-03-28 13:28:39.000000 Nuitka-2.1.6/nuitka/plugins/standard/OptionsNannyPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1940 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/plugins/standard/PbrPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4875 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/plugins/standard/PkgResourcesPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7042 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/plugins/standard/PmwPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    53098 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/plugins/standard/PySidePyQtPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3020 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/plugins/standard/PywebViewPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1193 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/plugins/standard/TensorflowPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13878 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/plugins/standard/TkinterPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1173 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/plugins/standard/TorchPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12838 2024-04-06 13:33:42.000000 Nuitka-2.1.6/nuitka/plugins/standard/TransformersPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1106 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/plugins/standard/TrioPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5668 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/plugins/standard/UpxPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/plugins/standard/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   230512 2024-04-19 13:34:22.000000 Nuitka-2.1.6/nuitka/plugins/standard/standard.nuitka-package.config.yml
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2352 2024-01-26 12:30:51.000000 Nuitka-2.1.6/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12392 2024-01-26 12:30:51.000000 Nuitka-2.1.6/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.797068 Nuitka-2.1.6/nuitka/reports/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2287 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/reports/CompilationReportReader.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2089 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/reports/LicenseReport.rst.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    27497 2024-03-28 13:28:39.000000 Nuitka-2.1.6/nuitka/reports/Reports.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/reports/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.797068 Nuitka-2.1.6/nuitka/specs/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5943 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/specs/BuiltinBytesOperationSpecs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2818 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/specs/BuiltinDictOperationSpecs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2573 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/specs/BuiltinListOperationSpecs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    26786 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/specs/BuiltinParameterSpecs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6097 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/specs/BuiltinStrOperationSpecs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1191 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/specs/BuiltinTypeOperationSpecs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4834 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/specs/BuiltinUnicodeOperationSpecs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6244 2024-03-11 17:07:05.000000 Nuitka-2.1.6/nuitka/specs/HardImportSpecs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    18739 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/specs/ParameterSpecs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/specs/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.797068 Nuitka-2.1.6/nuitka/tools/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1631 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/Basics.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.797068 Nuitka-2.1.6/nuitka/tools/commercial/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      847 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/commercial/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.797068 Nuitka-2.1.6/nuitka/tools/data_composer/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15004 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/data_composer/DataComposer.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/data_composer/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1338 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/data_composer/__main__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.797068 Nuitka-2.1.6/nuitka/tools/environments/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2481 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/environments/CreateEnvironment.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4199 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/environments/Virtualenv.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/environments/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.797068 Nuitka-2.1.6/nuitka/tools/general/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/general/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.797068 Nuitka-2.1.6/nuitka/tools/general/dll_report/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/general/dll_report/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2352 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/general/dll_report/__main__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.797068 Nuitka-2.1.6/nuitka/tools/general/find_module/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3953 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/general/find_module/FindModuleCode.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/general/find_module/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.797068 Nuitka-2.1.6/nuitka/tools/onefile_compressor/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12545 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/onefile_compressor/OnefileCompressor.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/onefile_compressor/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1343 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/onefile_compressor/__main__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.797068 Nuitka-2.1.6/nuitka/tools/podman/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1905 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/podman/Podman.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/podman/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11623 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/podman/__main__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.797068 Nuitka-2.1.6/nuitka/tools/profiler/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/profiler/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2561 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/profiler/__main__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.797068 Nuitka-2.1.6/nuitka/tools/scanning/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3590 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/scanning/DisplayPackageDLLs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2314 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/scanning/DisplayPackageData.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/scanning/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.797068 Nuitka-2.1.6/nuitka/tools/specialize/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    51531 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/specialize/CTypeDescriptions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7717 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/specialize/Common.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    39659 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/specialize/SpecializeC.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    35715 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/specialize/SpecializePython.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/specialize/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.797068 Nuitka-2.1.6/nuitka/tools/testing/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    55682 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/testing/Common.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1516 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/testing/Constructs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10024 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/testing/OutputComparison.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1311 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/testing/Pythons.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8061 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/testing/RuntimeTracing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5413 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/testing/SearchModes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3408 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/testing/Valgrind.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/testing/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.797068 Nuitka-2.1.6/nuitka/tools/testing/check_reference_counts/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/testing/check_reference_counts/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3095 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/testing/check_reference_counts/__main__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.797068 Nuitka-2.1.6/nuitka/tools/testing/compare_with_cpython/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/testing/compare_with_cpython/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    29877 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/testing/compare_with_cpython/__main__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.797068 Nuitka-2.1.6/nuitka/tools/testing/find_sxs_modules/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/testing/find_sxs_modules/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1980 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/testing/find_sxs_modules/__main__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.797068 Nuitka-2.1.6/nuitka/tools/testing/measure_construct_performance/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/testing/measure_construct_performance/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8758 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/testing/measure_construct_performance/__main__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.797068 Nuitka-2.1.6/nuitka/tools/testing/run_nuitka_tests/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/testing/run_nuitka_tests/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    35342 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/testing/run_nuitka_tests/__main__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.797068 Nuitka-2.1.6/nuitka/tools/watch/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3476 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/watch/GitHub.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tools/watch/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    20868 2024-03-04 15:35:30.000000 Nuitka-2.1.6/nuitka/tools/watch/__main__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.797068 Nuitka-2.1.6/nuitka/tree/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    50370 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/Building.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    75150 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/ComplexCallHelperFunctions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1733 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/Extractions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2604 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/InternalModule.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1544 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/Operations.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2840 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/ReformulationAssertStatements.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    43101 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/ReformulationAssignmentStatements.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2981 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/ReformulationBooleanExpressions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11746 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/ReformulationCallExpressions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15446 2024-03-14 10:27:18.000000 Nuitka-2.1.6/nuitka/tree/ReformulationClasses.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    38235 2024-03-14 10:27:18.000000 Nuitka-2.1.6/nuitka/tree/ReformulationClasses3.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6523 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/ReformulationComparisonExpressions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    22175 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/ReformulationContractionExpressions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11196 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/ReformulationDictionaryCreation.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14757 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/ReformulationExecStatements.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7858 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/ReformulationForLoopStatements.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    30821 2024-03-11 17:07:05.000000 Nuitka-2.1.6/nuitka/tree/ReformulationFunctionStatements.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14095 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/ReformulationImportStatements.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6630 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/ReformulationLambdaExpressions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    21311 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/ReformulationMatchStatements.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2442 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/ReformulationMultidist.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7608 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/ReformulationNamespacePackages.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4711 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/ReformulationPrintStatements.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15606 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/ReformulationSequenceCreation.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4857 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/ReformulationSubscriptExpressions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14948 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/ReformulationTryExceptStatements.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7014 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/ReformulationTryFinallyStatements.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5707 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/ReformulationWhileLoopStatements.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14439 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/ReformulationWithStatements.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3852 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/ReformulationYieldExpressions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13212 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/SourceHandling.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3790 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/SyntaxErrors.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    23005 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/TreeHelpers.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    20465 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/VariableClosure.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/tree/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/nuitka/utils/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3020 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/utils/AppDirs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4148 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/utils/CStrings.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6395 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/utils/CommandLineOptions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14981 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/utils/Distributions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6413 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/utils/Download.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13185 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/utils/Execution.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    41397 2024-04-19 13:34:22.000000 Nuitka-2.1.6/nuitka/utils/FileOperations.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3753 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/utils/Hashing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2395 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/utils/Images.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10121 2024-03-04 15:32:38.000000 Nuitka-2.1.6/nuitka/utils/Importing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7884 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/utils/InstalledPythons.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2257 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/utils/InstanceCounters.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4586 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/utils/Jinja2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1271 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/utils/Json.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4477 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/utils/MacOSApp.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5092 2024-03-22 08:13:25.000000 Nuitka-2.1.6/nuitka/utils/MemoryUsage.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9951 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/utils/ModuleNames.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4588 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/utils/ReExecute.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1889 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/utils/Rest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    23857 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/utils/SharedLibraries.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3697 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/utils/Shebang.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3687 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/utils/Signing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2084 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/utils/SlotMetaClasses.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6603 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/utils/StaticLibraries.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2634 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/utils/ThreadedExecutor.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2798 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/utils/Timing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11527 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/utils/Utils.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10606 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/utils/WindowsFileUsage.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    19837 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/utils/WindowsResources.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7014 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/utils/Yaml.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/nuitka/utils/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.1.6/pyproject.toml
+-rw-r--r--   0 hayen     (1000) hayen     (2000)       38 2024-04-19 13:34:34.837068 Nuitka-2.1.6/setup.cfg
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    16677 2024-03-04 14:35:43.000000 Nuitka-2.1.6/setup.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/basics/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1798 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/AssertsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5966 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/AssignmentsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5910 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/AssignmentsTest32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4086 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/BranchingTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1136 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/BuiltinOverload.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3781 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/BuiltinSuperTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17112 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/BuiltinsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      898 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/ClassMinimalTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4796 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/ClassesTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3446 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/ClassesTest32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1438 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/ClassesTest34.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4729 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/ComparisonChainsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4672 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/ConstantsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1027 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/ConstantsTest27.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1661 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/DecoratorsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2349 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/DefaultParametersTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1159 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/DoubleDeletionsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      838 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/EmptyModuleTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14418 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/ExceptionRaisingTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      993 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/ExceptionRaisingTest32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1490 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/ExceptionRaisingTest33.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6779 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/ExecEvalTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1449 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/ExtremeClosureTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1690 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/FunctionObjectsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12367 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/FunctionsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3635 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/FunctionsTest32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2659 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/FunctionsTest_2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      922 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/FutureTest32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5841 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/GeneratorExpressionsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1073 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/GeneratorExpressionsTest_37.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3856 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/GlobalStatementTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1318 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/HelloWorldTest_2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2501 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/ImportingTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1328 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/InplaceOperationsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4259 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/InspectionTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1536 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/InspectionTest_35.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1650 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/InspectionTest_36.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1703 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/LambdasTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2763 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/LateClosureAssignmentTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2955 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/ListContractionsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3361 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/LoopingTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1568 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/MainProgramsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1957 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/ModuleAttributesTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2008 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/OperatorsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14935 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/OrderChecksTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1859 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/OrderChecksTest27.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1484 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/OverflowFunctionsTest_2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5885 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/ParameterErrorsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1931 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/ParameterErrorsTest32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      895 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/PrintFutureTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1444 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/PrintingTest_2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      910 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/RecursionTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    24719 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/ReferencingTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2109 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/ReferencingTest27.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7850 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/ReferencingTest33.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5041 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/ReferencingTest35.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5478 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/ReferencingTest36.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2932 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/ReferencingTest_2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1662 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/SlotsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1191 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/ThreadedGeneratorsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    22998 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/TrickAssignmentsTest32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1573 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/TrickAssignmentsTest35.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1820 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/TrickAssignmentsTest_2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2118 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/TryContinueFinallyTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2244 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/TryExceptContinueTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2307 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/TryExceptFinallyTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2336 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/TryExceptFramesTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2874 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/TryReturnFinallyTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2360 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/TryYieldFinallyTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1125 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/UnicodeTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1909 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/UnpackingTest35.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2143 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/VarargsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4913 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/WithStatementsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3103 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/YieldFromTest33.py
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     3851 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/run_all.py
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     2302 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/basics/run_xml.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/onefile/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1341 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/onefile/HelloWorldTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1339 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/onefile/KeyboardInterruptTest.py
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     5846 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/onefile/run_all.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/optimizations/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      991 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/optimizations/ArgumentTypes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1087 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/optimizations/Attributes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1053 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/optimizations/Calls.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      953 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/optimizations/Conditions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      941 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/optimizations/DecodingOperations.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1246 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/optimizations/FormatStrings36.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1183 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/optimizations/HardImports.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1007 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/optimizations/HardImports_2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      950 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/optimizations/Iterations.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1292 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/optimizations/Len.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1133 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/optimizations/Matching310.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2295 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/optimizations/Operations.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1365 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/optimizations/Subscripts.py
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     8827 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/optimizations/run_all.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/packages/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/packages/package_data_files_embedding/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1576 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/packages/package_data_files_embedding/PackageDataFilesEmbedding.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      956 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/packages/package_data_files_embedding/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/packages/package_import_success_after_failure/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2414 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/packages/package_import_success_after_failure/variable_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      975 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1201 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/packages/package_import_success_after_failure/variable_package/__init__.py
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     4138 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/packages/run_all.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.627068 Nuitka-2.1.6/tests/packages/sub_package/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/packages/sub_package/kitty/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1262 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/packages/sub_package/kitty/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      940 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/packages/sub_package/kitty/bigkitty.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      942 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/packages/sub_package/kitty/smallkitty.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/packages/sub_package/kitty/speak/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      961 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/packages/sub_package/kitty/speak/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1085 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/packages/sub_package/kitty/speak/hello.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      999 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/packages/sub_package/kitty/speak/miau.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1001 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/packages/sub_package/kitty/speak/purr.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.627068 Nuitka-2.1.6/tests/packages/top_level_attributes_3/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/packages/top_level_attributes_3/some_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2368 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/packages/top_level_attributes_3/some_package/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      939 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/packages/top_level_attributes_3/some_package/some_module.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/plugins/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/plugins/code_signing/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1202 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/plugins/code_signing/CodeSigningMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/plugins/data_files/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1474 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/plugins/data_files/DataFilesMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/plugins/data_files/data_files_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      956 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/plugins/data_files/data_files_package/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)        0 2022-10-08 09:07:15.000000 Nuitka-2.1.6/tests/plugins/data_files/data_files_package/lala.txt
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/plugins/data_files/data_files_package/sub_dir/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)        0 2022-10-08 09:07:15.000000 Nuitka-2.1.6/tests/plugins/data_files/data_files_package/sub_dir/lulu.txt
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      309 2024-01-26 12:30:51.000000 Nuitka-2.1.6/tests/plugins/data_files/test_case.nuitka-package.config.yml
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/plugins/parameters/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1051 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/plugins/parameters/ParametersMain.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2218 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/plugins/parameters/parameter-using-plugin.py
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     3892 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/plugins/run_all.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/programs/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/programs/absolute_import/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      899 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/absolute_import/AbsoluteImportMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/programs/absolute_import/foobar/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      828 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/absolute_import/foobar/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1076 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/absolute_import/foobar/foobar.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      911 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/absolute_import/foobar/local.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      893 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/absolute_import/foobar/util.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/programs/case_imports1/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      840 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/case_imports1/CasedImportingMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/programs/case_imports1/path1/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      830 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/case_imports1/path1/Some_Module.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/programs/case_imports1/path1/Some_Package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      831 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/case_imports1/path1/Some_Package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/programs/case_imports1/path2/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      830 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/case_imports1/path2/some_module.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/programs/case_imports1/path2/some_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      831 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/case_imports1/path2/some_package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/programs/case_imports2/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      840 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/case_imports2/CasedImportingMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/programs/case_imports2/path1/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/case_imports2/path1/some_module.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/programs/case_imports2/path1/some_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/case_imports2/path1/some_package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/programs/case_imports2/path2/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      830 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/case_imports2/path2/Some_Module.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/programs/case_imports2/path2/Some_Package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      831 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/case_imports2/path2/Some_Package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/programs/case_imports3/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1107 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/case_imports3/CasedImportingMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/programs/case_imports3/path1/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      841 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/case_imports3/path1/Some_Module.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/programs/case_imports3/path1/Some_Package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      842 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/case_imports3/path1/Some_Package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/programs/case_imports3/path2/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      841 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/case_imports3/path2/Some_Module.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/programs/case_imports3/path2/Some_Package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      842 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/case_imports3/path2/Some_Package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/programs/cyclic_imports/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      833 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/cyclic_imports/CyclicImportsMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/programs/cyclic_imports/cyclic_importing_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      907 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      907 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      874 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/programs/dash_import/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      920 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/dash_import/DashImportMain.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      849 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/dash_import/dash-module.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      849 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/dash_import/plus+module.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/programs/dash_main/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      841 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/dash_main/Dash-Main.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/programs/deep/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      930 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/deep/DeepProgramMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/programs/deep/some_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1012 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/deep/some_package/DeepBrother.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      941 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/deep/some_package/DeepChild.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/deep/some_package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/programs/deep/some_package/deep_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      908 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/deep/some_package/deep_package/DeepDeepChild.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      984 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/deep/some_package/deep_package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/programs/dunderinit_imports/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      826 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/dunderinit_imports/DunderInitImportsMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/programs/dunderinit_imports/package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      829 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/dunderinit_imports/package/SubModule.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      889 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/dunderinit_imports/package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/programs/import_variants/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1037 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/import_variants/ImportVariationsMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/programs/import_variants/some_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      978 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/import_variants/some_package/Child1.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1130 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/import_variants/some_package/Child2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      854 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/import_variants/some_package/Child3.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1026 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/import_variants/some_package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/programs/main_raises/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      943 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/main_raises/ErrorMain.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      841 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/main_raises/ErrorRaising.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.817068 Nuitka-2.1.6/tests/programs/main_raises2/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1112 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/main_raises2/ErrorInFunctionMain.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      841 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/main_raises2/ErrorRaising.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/module_attributes/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1561 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/module_attributes/ModuleAttributesMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/module_attributes/package_level1/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1776 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/module_attributes/package_level1/Nearby1.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1643 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/module_attributes/package_level1/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/module_attributes/package_level1/package_level2/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1776 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1643 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/module_attributes/package_level1/package_level2/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/module_attributes/package_level1/package_level2/package_level3/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1776 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1643 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/module_exits/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      901 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/module_exits/ErrorExitingModule.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      899 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/module_exits/Main.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/module_object_replacing/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1110 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1391 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/module_object_replacing/SelfReplacingModule.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/multiprocessing_using/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1022 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/multiprocessing_using/foo/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/multiprocessing_using/foo/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      868 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/multiprocessing_using/foo/__main__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1791 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/multiprocessing_using/foo/entry.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/named_imports/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      878 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/named_imports/NamedImportsMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/named_imports/some_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/named_imports/some_package/SomeModule.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      856 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/named_imports/some_package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/named_imports/some_package/sub_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/named_imports/some_package/sub_package/SomeModule.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/package_code/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      832 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/package_code/PackageInitCodeMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/package_code/some_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      842 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/package_code/some_package/SomeModule.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      841 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/package_code/some_package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/package_contains_main/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      821 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/package_contains_main/PackageContainsMain.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/package_contains_main/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      833 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/package_contains_main/local.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/package_init_import/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      855 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/package_init_import/PackageInitImportMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/package_init_import/some_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1040 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/package_init_import/some_package/PackageLocal.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1201 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/package_init_import/some_package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/package_init_issue/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      821 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/package_init_issue/PackageInitIssueMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/package_init_issue/some_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      830 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/package_init_issue/some_package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/package_init_issue/some_package/child_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      830 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/package_init_issue/some_package/child_package/SomeModule.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      827 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/package_init_issue/some_package/child_package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/package_missing_init/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      958 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/package_missing_init/PackageMissingInitMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/package_missing_init/some_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      997 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/package_missing_init/some_package/some_module.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/package_missing_init/some_package/sub_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1009 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/package_module_collision/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      933 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/package_module_collision/Something/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      842 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/package_module_collision/Something/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      833 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/package_module_collision/something.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/package_overload/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      884 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/package_overload/Main.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/package_overload/foo/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      831 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/package_overload/foo/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/package_overload/foo/bar.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/package_overload/foo/bar2.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/package_prevents_submodule/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3004 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/package_prevents_submodule/some_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1111 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/package_prevents_submodule/some_package/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      833 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/package_prevents_submodule/some_package/some_module.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.627068 Nuitka-2.1.6/tests/programs/package_program/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/package_program/PackageAsMain/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      920 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/package_program/PackageAsMain/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1662 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/package_program/PackageAsMain/__main__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/pkgutil_itermodules/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1760 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/pkgutil_itermodules/some_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/pkgutil_itermodules/some_package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/pkgutil_usage/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1328 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/pkgutil_usage/PkgUtilUsageMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/pkgutil_usage/package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)       13 2021-04-22 06:31:42.000000 Nuitka-2.1.6/tests/programs/pkgutil_usage/package/DATA_FILE.txt
+-rw-r--r--   0 hayen     (1000) hayen     (2000)       14 2022-10-08 09:07:15.000000 Nuitka-2.1.6/tests/programs/pkgutil_usage/package/DATA_FILE2.txt
+-rw-r--r--   0 hayen     (1000) hayen     (2000)       14 2022-10-08 09:07:15.000000 Nuitka-2.1.6/tests/programs/pkgutil_usage/package/DATA_FILE3.txt
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1585 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/pkgutil_usage/package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/plugin_import/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      891 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/plugin_import/PluginImportMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/plugin_import/some_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      803 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/plugin_import/some_package/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      813 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/plugin_import/some_package/some_module.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/reimport_main_dynamic/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      943 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/reimport_main_static/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      930 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/reimport_main_static/ImportItselfStaticMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/relative_import/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      874 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/relative_import/RelativeImportMain.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/relative_import/dircache.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/resource_reader37/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1201 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/resource_reader37/ResourceReaderMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/resource_reader37/some_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)       13 2022-10-08 09:07:15.000000 Nuitka-2.1.6/tests/programs/resource_reader37/some_package/DATA_FILE.txt
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/resource_reader37/some_package/__init__.py
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     6646 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/run_all.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/stdlib_overload/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1203 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/stdlib_overload/StdlibOverloadMain.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      831 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/stdlib_overload/pyexpat.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/stdlib_overload/some_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/stdlib_overload/some_package/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      941 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/stdlib_overload/some_package/normal_importing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      842 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/stdlib_overload/some_package/pyexpat.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1268 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/stdlib_overload/some_package/star_importing.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/syntax_errors/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      822 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/syntax_errors/IndentationErroring.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      833 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/syntax_errors/SyntaxErroring.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1111 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/syntax_errors/SyntaxErrorsMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/unicode_bom/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      995 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/unicode_bom/UnicodeBomMain.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      878 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/unicode_bom/unicode_bom.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/programs/with space/
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)      858 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/programs/with space/Space Main.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.827068 Nuitka-2.1.6/tests/reflected/
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)    14194 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/reflected/compile_itself.py
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     1274 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/run-tests
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.837068 Nuitka-2.1.6/tests/standalone/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1090 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/BrotliUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2586 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/CtypesUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1950 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/DateutilsUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1168 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/FlaskUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1274 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/GiUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1022 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/GlfwUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1216 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/GtkUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1057 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/HexEncodingTest_2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1118 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/IdnaUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1215 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/LxmlUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1598 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/MatplotlibUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2570 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/MetadataPackagesUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1759 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/NumpyUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      979 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/OpenGLUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1479 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/PandasUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1098 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/PasslibUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1248 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/PendulumUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2106 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/PkgResourcesRequiresUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1099 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/PmwUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1369 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/PyQt5Plugins.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1253 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/PyQt5SSLSupport.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2198 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/PyQt5Using.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1203 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/PyQt6Plugins.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2168 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/PyQt6Using.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1789 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/PySide2Using.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1123 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/PySide6Plugins.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1789 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/PySide6Using.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1371 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/RsaUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1227 2024-03-22 08:13:25.000000 Nuitka-2.1.6/tests/standalone/SetuptoolsUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1005 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/ShlibUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1569 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/SocketUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1973 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/TkInterUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3260 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/Urllib3Using.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1232 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/Win32ComUsing.py
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     9912 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/run_all.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.837068 Nuitka-2.1.6/tests/standalone/zip_importer/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1296 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/standalone/zip_importer/ZipImporterMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-19 13:34:34.837068 Nuitka-2.1.6/tests/syntax/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      844 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/AsyncgenReturn36.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      818 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/AwaitInModule36.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      901 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/BreakWithoutLoop.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      824 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/ClassReturn.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1002 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/ClosureDel_2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      882 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/ContinueWithoutLoop.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      824 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/DuplicateArgument.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1142 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/ExecWithNesting_2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      858 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/FutureBraces.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      837 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/FutureUnknown.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1073 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/GeneratorExpressions38.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      911 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/GeneratorReturn_2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      825 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/GlobalForParameter.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1027 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/Importing32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      830 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/IndentationError.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      947 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/LateFutureImport.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      874 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/MisplacedFutureImport.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      832 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/ModuleReturn.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      915 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/NonAsciiWithoutEncoding_2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      827 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/NonlocalForParameter32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      900 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/NonlocalNotFound32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      939 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/StarImportExtra.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      900 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/SyntaxError.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      907 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/TryExceptAllNotLast.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      908 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/TryFinallyContinue_37.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      808 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/UnpackNoTuple.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      841 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/UnpackTwoStars32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      825 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/YieldFromInModule.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      837 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/YieldInAsync35.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      956 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/YieldInGenexp38.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      813 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/YieldInModule.py
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     2234 2024-03-04 14:35:43.000000 Nuitka-2.1.6/tests/syntax/run_all.py
```

### Comparing `Nuitka-2.1.5/Developer_Manual.rst` & `Nuitka-2.1.6/Developer_Manual.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/LICENSE.txt` & `Nuitka-2.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/MANIFEST.in` & `Nuitka-2.1.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/Nuitka.egg-info/PKG-INFO` & `Nuitka-2.1.6/Nuitka.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nuitka
-Version: 2.1.5
+Version: 2.1.6
 Summary: Python compiler with full language support and CPython compatibility
 Home-page: https://nuitka.net
 Author: Kay Hayen
 Author-email: Kay.Hayen@gmail.com
 License: Apache License, Version 2.0
 Project-URL: Commercial, https://nuitka.net/doc/commercial.html
 Project-URL: Support, https://nuitka.net/pages/support.html
```

### Comparing `Nuitka-2.1.5/Nuitka.egg-info/SOURCES.txt` & `Nuitka-2.1.6/Nuitka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/PKG-INFO` & `Nuitka-2.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nuitka
-Version: 2.1.5
+Version: 2.1.6
 Summary: Python compiler with full language support and CPython compatibility
 Home-page: https://nuitka.net
 Author: Kay Hayen
 Author-email: Kay.Hayen@gmail.com
 License: Apache License, Version 2.0
 Project-URL: Commercial, https://nuitka.net/doc/commercial.html
 Project-URL: Support, https://nuitka.net/pages/support.html
```

### Comparing `Nuitka-2.1.5/README.rst` & `Nuitka-2.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/bin/autoformat-nuitka-source` & `Nuitka-2.1.6/bin/autoformat-nuitka-source`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/bin/check-nuitka-with-pylint` & `Nuitka-2.1.6/bin/check-nuitka-with-pylint`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/bin/compare_with_cpython` & `Nuitka-2.1.6/bin/compare_with_cpython`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/bin/compare_with_xml` & `Nuitka-2.1.6/bin/compare_with_xml`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/bin/measure-construct-performance` & `Nuitka-2.1.6/bin/measure-construct-performance`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/bin/nuitka` & `Nuitka-2.1.6/bin/nuitka`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/bin/nuitka-run` & `Nuitka-2.1.6/bin/nuitka-run`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/doc/Logo/Nuitka-Logo-Horizontal.svg` & `Nuitka-2.1.6/doc/Logo/Nuitka-Logo-Horizontal.svg`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/doc/Logo/Nuitka-Logo-Symbol.svg` & `Nuitka-2.1.6/doc/Logo/Nuitka-Logo-Symbol.svg`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/doc/Logo/Nuitka-Logo-Vertical.svg` & `Nuitka-2.1.6/doc/Logo/Nuitka-Logo-Vertical.svg`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/doc/images/Nuitka-Logo-Horizontal.png` & `Nuitka-2.1.6/doc/images/Nuitka-Logo-Horizontal.png`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/doc/images/Nuitka-Logo-Symbol.png` & `Nuitka-2.1.6/doc/images/Nuitka-Logo-Symbol.png`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/doc/images/Nuitka-Logo-Vertical.png` & `Nuitka-2.1.6/doc/images/Nuitka-Logo-Vertical.png`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/doc/nuitka-run.1` & `Nuitka-2.1.6/doc/nuitka-run.1`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/doc/nuitka.1` & `Nuitka-2.1.6/doc/nuitka.1`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/lib/hints.py` & `Nuitka-2.1.6/lib/hints.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/misc/nuitka-run.bat` & `Nuitka-2.1.6/misc/nuitka-run.bat`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/misc/nuitka.bat` & `Nuitka-2.1.6/misc/nuitka.bat`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/Builtins.py` & `Nuitka-2.1.6/nuitka/Builtins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/BytecodeCaching.py` & `Nuitka-2.1.6/nuitka/BytecodeCaching.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/Bytecodes.py` & `Nuitka-2.1.6/nuitka/Bytecodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/CacheCleanup.py` & `Nuitka-2.1.6/nuitka/CacheCleanup.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/Constants.py` & `Nuitka-2.1.6/nuitka/Constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/Errors.py` & `Nuitka-2.1.6/nuitka/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/HardImportRegistry.py` & `Nuitka-2.1.6/nuitka/HardImportRegistry.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/MainControl.py` & `Nuitka-2.1.6/nuitka/MainControl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/ModuleRegistry.py` & `Nuitka-2.1.6/nuitka/ModuleRegistry.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/OptionParsing.py` & `Nuitka-2.1.6/nuitka/OptionParsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/Options.py` & `Nuitka-2.1.6/nuitka/Options.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/OutputDirectories.py` & `Nuitka-2.1.6/nuitka/OutputDirectories.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/PostProcessing.py` & `Nuitka-2.1.6/nuitka/PostProcessing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/Progress.py` & `Nuitka-2.1.6/nuitka/Progress.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/PythonFlavors.py` & `Nuitka-2.1.6/nuitka/PythonFlavors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/PythonOperators.py` & `Nuitka-2.1.6/nuitka/PythonOperators.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/PythonVersions.py` & `Nuitka-2.1.6/nuitka/PythonVersions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/Serialization.py` & `Nuitka-2.1.6/nuitka/Serialization.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/SourceCodeReferences.py` & `Nuitka-2.1.6/nuitka/SourceCodeReferences.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/Tracing.py` & `Nuitka-2.1.6/nuitka/Tracing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/TreeXML.py` & `Nuitka-2.1.6/nuitka/TreeXML.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/Variables.py` & `Nuitka-2.1.6/nuitka/Variables.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/Version.py` & `Nuitka-2.1.6/nuitka/Version.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #     limitations under the License.
 #
 """ Nuitka version related stuff.
 
 """
 
 version_string = """\
-Nuitka V2.1.5
+Nuitka V2.1.6
 Copyright (C) 2024 Kay Hayen."""
 
 
 def getNuitkaVersion():
     """Return Nuitka version as a string.
 
     This should not be used for >= comparisons directly.
```

### Comparing `Nuitka-2.1.5/nuitka/__init__.py` & `Nuitka-2.1.6/nuitka/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/__main__.py` & `Nuitka-2.1.6/nuitka/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/__past__.py` & `Nuitka-2.1.6/nuitka/__past__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/Backend.scons` & `Nuitka-2.1.6/nuitka/build/Backend.scons`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/CCompilerVersion.scons` & `Nuitka-2.1.6/nuitka/build/CCompilerVersion.scons`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/DataComposerInterface.py` & `Nuitka-2.1.6/nuitka/build/DataComposerInterface.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/Onefile.scons` & `Nuitka-2.1.6/nuitka/build/Onefile.scons`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/SconsCaching.py` & `Nuitka-2.1.6/nuitka/build/SconsCaching.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/SconsCompilerSettings.py` & `Nuitka-2.1.6/nuitka/build/SconsCompilerSettings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/SconsHacks.py` & `Nuitka-2.1.6/nuitka/build/SconsHacks.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/SconsInterface.py` & `Nuitka-2.1.6/nuitka/build/SconsInterface.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/SconsProgress.py` & `Nuitka-2.1.6/nuitka/build/SconsProgress.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/SconsSpawn.py` & `Nuitka-2.1.6/nuitka/build/SconsSpawn.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/SconsUtils.py` & `Nuitka-2.1.6/nuitka/build/SconsUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,15 +311,15 @@
     path_elements = search_path.split(os.pathsep)
 
     for path_element in path_elements:
         path_element = path_element.strip('"')
 
         full = os.path.normpath(os.path.join(path_element, filename))
 
-        if os.path.exists(full):
+        if os.path.isfile(full):
             return full
 
     return None
 
 
 def changeKeyboardInterruptToErrorExit():
     def signalHandler(
```

### Comparing `Nuitka-2.1.5/nuitka/build/__init__.py` & `Nuitka-2.1.6/nuitka/build/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/allocator.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/allocator.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/builtins.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/builtins.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/calling.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/calling.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/checkers.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/checkers.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/checksum_tools.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/checksum_tools.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/compiled_asyncgen.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/compiled_asyncgen.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/compiled_cell.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/compiled_cell.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/compiled_coroutine.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/compiled_coroutine.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/compiled_frame.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/compiled_frame.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/compiled_function.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/compiled_function.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/compiled_generator.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/compiled_generator.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/compiled_method.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/compiled_method.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/constants.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/constants.h`

 * *Files 0% similar despite different names*

```diff
@@ -137,14 +137,16 @@
 #define const_str_plain_basename global_constants[42]
 // 'dirname'
 #define const_str_plain_dirname global_constants[42]
 // 'abspath'
 #define const_str_plain_abspath global_constants[42]
 // 'isabs'
 #define const_str_plain_isabs global_constants[42]
+// 'normpath'
+#define const_str_plain_normpath global_constants[42]
 // 'path'
 #define const_str_plain_path global_constants[42]
 // '__newobj__'
 #define const_str_plain___newobj__ global_constants[44]
 // '.'
 #define const_str_dot global_constants[45]
 // '_'
```

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/constants_blob.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/constants_blob.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/environment_variables.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/environment_variables.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/environment_variables_system.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/environment_variables_system.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/exception_groups.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/exception_groups.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/exceptions.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/exceptions.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/filesystem_paths.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/filesystem_paths.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/freelists.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/freelists.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/hedley.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/hedley.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/attributes.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/attributes.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/boolean.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/boolean.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/bytearrays.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/bytearrays.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/bytes.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/bytes.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/calling_generated.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/calling_generated.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/comparisons_eq.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/comparisons_eq.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/comparisons_ge.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/comparisons_ge.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/comparisons_gt.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/comparisons_gt.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/comparisons_le.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/comparisons_le.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/comparisons_lt.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/comparisons_lt.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/comparisons_ne.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/comparisons_ne.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/complex.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/complex.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/dictionaries.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/dictionaries.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/floats.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/floats.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/import_hard.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/import_hard.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/indexes.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/indexes.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/ints.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/ints.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/iterators.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/iterators.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/lists.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/lists.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/lists_generated.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/lists_generated.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/mappings.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/mappings.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_add.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_binary_add.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_bitand.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_binary_bitand.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_bitor.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_binary_bitor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_divmod.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_binary_divmod.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_lshift.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_binary_lshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_matmult.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_binary_matmult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_mod.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_binary_mod.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_mult.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_binary_mult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_pow.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_binary_pow.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_rshift.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_binary_rshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_sub.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_binary_sub.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_binary_truediv.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_binary_truediv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_builtin_types.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_builtin_types.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_add.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_inplace_add.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_mod.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_inplace_mod.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_mult.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_inplace_mult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_pow.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_inplace_pow.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_sub.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_inplace_sub.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/raising.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/raising.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/rangeobjects.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/rangeobjects.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/richcomparisons.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/richcomparisons.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/sequences.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/sequences.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/sets.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/sets.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/slices.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/slices.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/strings.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/strings.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/subscripts.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/subscripts.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helper/tuples.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helper/tuples.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/helpers.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/helpers.h`

 * *Files 0% similar despite different names*

```diff
@@ -183,14 +183,15 @@
 #endif
 
 // Small helpers to work with filenames from "os.path" module
 extern PyObject *OS_PATH_BASENAME(PyThreadState *tstate, PyObject *filename);
 extern PyObject *OS_PATH_DIRNAME(PyThreadState *tstate, PyObject *filename);
 extern PyObject *OS_PATH_ABSPATH(PyThreadState *tstate, PyObject *filename);
 extern PyObject *OS_PATH_ISABS(PyThreadState *tstate, PyObject *filename);
+extern PyObject *OS_PATH_NORMPATH(PyThreadState *tstate, PyObject *filename);
 
 // Compare two paths if they are the same.
 nuitka_bool compareFilePaths(PyThreadState *tstate, PyObject *filename_a, PyObject *filename_b);
 
 // For quicker built-in chr() functionality.
 extern PyObject *BUILTIN_CHR(PyThreadState *tstate, PyObject *value);
```

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/importing.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/importing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/incbin.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/incbin.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/prelude.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/prelude.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/printing.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/printing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/python_pgo.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/python_pgo.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/safe_string_ops.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/safe_string_ops.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/threading.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/threading.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/tracing.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/tracing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/include/nuitka/unfreezing.h` & `Nuitka-2.1.6/nuitka/build/include/nuitka/unfreezing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/appdirs/LICENSE.txt` & `Nuitka-2.1.6/nuitka/build/inline_copy/appdirs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/appdirs/appdirs.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/appdirs/appdirs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/atomicwrites/LICENSE` & `Nuitka-2.1.6/nuitka/build/inline_copy/atomicwrites/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/atomicwrites/atomicwrites.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/atomicwrites/atomicwrites.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/bin/scons.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/bin/scons.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/clcache/clcache/LICENSE` & `Nuitka-2.1.6/nuitka/build/inline_copy/clcache/clcache/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/clcache/clcache/caching.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/clcache/clcache/caching.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/colorama/LICENSE.txt` & `Nuitka-2.1.6/nuitka/build/inline_copy/colorama/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/colorama/colorama/ansi.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/colorama/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/colorama/colorama/initialise.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/colorama/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/colorama/colorama/win32.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/colorama/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/colorama/colorama/winterm.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/colorama/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/glob2/LICENSE` & `Nuitka-2.1.6/nuitka/build/inline_copy/glob2/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/glob2/glob2/compat.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/glob2/glob2/compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/glob2/glob2/fnmatch.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/glob2/glob2/fnmatch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/glob2/glob2/impl.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/glob2/glob2/impl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/LICENSE.rst` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/_compat.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/_compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/bccache.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/bccache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/compiler.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/compiler.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/constants.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/debug.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/defaults.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/environment.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/ext.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/ext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/filters.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/filters.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/lexer.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/lexer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/loaders.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/loaders.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/meta.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/meta.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/nodes.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/parser.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/runtime.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/runtime.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/tests.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/tests.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/utils.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2/jinja2/visitor.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2/jinja2/visitor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/LICENSE.rst` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/markupsafe/LICENSE.rst` & `Nuitka-2.1.6/nuitka/build/inline_copy/markupsafe/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/tqdm/tqdm/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/_utils.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/tqdm/tqdm/_utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/auto.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/tqdm/tqdm/auto.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/dask.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/tqdm/tqdm/dask.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/notebook.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/tqdm/tqdm/notebook.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/std.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/tqdm/tqdm/std.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/tk.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/tqdm/tqdm/tk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/tqdm/tqdm/utils.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/tqdm/tqdm/utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml/LICENSE` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/composer.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/constructor.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/cyaml.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/dumper.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/emitter.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/error.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/error.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/events.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/events.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/loader.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/nodes.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/parser.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/reader.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/representer.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/resolver.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/scanner.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/serializer.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml/yaml/tokens.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/LICENSE` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/composer.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/constructor.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/dumper.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/emitter.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/error.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/error.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/events.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/events.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/loader.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/nodes.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/parser.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/reader.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/representer.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/resolver.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/scanner.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/serializer.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_27/yaml/tokens.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_27/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/LICENSE` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/__init__.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/composer.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/constructor.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/dumper.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/emitter.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/error.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/error.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/events.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/events.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/loader.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/nodes.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/parser.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/reader.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/representer.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/resolver.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/scanner.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/serializer.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/yaml_35/yaml/tokens.py` & `Nuitka-2.1.6/nuitka/build/inline_copy/yaml_35/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zlib/LICENSE` & `Nuitka-2.1.6/nuitka/build/inline_copy/zlib/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zlib/crc32.c` & `Nuitka-2.1.6/nuitka/build/inline_copy/zlib/crc32.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zlib/crc32.h` & `Nuitka-2.1.6/nuitka/build/inline_copy/zlib/crc32.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zlib/zconf.h` & `Nuitka-2.1.6/nuitka/build/inline_copy/zlib/zconf.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zlib/zlib.h` & `Nuitka-2.1.6/nuitka/build/inline_copy/zlib/zlib.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zlib/zutil.h` & `Nuitka-2.1.6/nuitka/build/inline_copy/zlib/zutil.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zstd/LICENSE.txt` & `Nuitka-2.1.6/nuitka/build/inline_copy/zstd/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/bitstream.h` & `Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/bitstream.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/compiler.h` & `Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/compiler.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/cpu.h` & `Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/cpu.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/debug.h` & `Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/debug.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/entropy_common.c` & `Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/entropy_common.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/error_private.c` & `Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/error_private.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/error_private.h` & `Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/error_private.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/fse.h` & `Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/fse.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/fse_decompress.c` & `Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/fse_decompress.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/huf.h` & `Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/huf.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/mem.h` & `Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/mem.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/xxhash.c` & `Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/xxhash.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/xxhash.h` & `Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/xxhash.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/zstd_common.c` & `Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/zstd_common.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/zstd_deps.h` & `Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/zstd_deps.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/zstd_errors.h` & `Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/zstd_errors.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zstd/common/zstd_internal.h` & `Nuitka-2.1.6/nuitka/build/inline_copy/zstd/common/zstd_internal.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c` & `Nuitka-2.1.6/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c` & `Nuitka-2.1.6/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h` & `Nuitka-2.1.6/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c` & `Nuitka-2.1.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c` & `Nuitka-2.1.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h` & `Nuitka-2.1.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h` & `Nuitka-2.1.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/inline_copy/zstd/zstd.h` & `Nuitka-2.1.6/nuitka/build/inline_copy/zstd/zstd.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/CompiledAsyncgenType.c` & `Nuitka-2.1.6/nuitka/build/static_src/CompiledAsyncgenType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/CompiledCellType.c` & `Nuitka-2.1.6/nuitka/build/static_src/CompiledCellType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/CompiledCodeHelpers.c` & `Nuitka-2.1.6/nuitka/build/static_src/CompiledCodeHelpers.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/CompiledCoroutineType.c` & `Nuitka-2.1.6/nuitka/build/static_src/CompiledCoroutineType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/CompiledFrameType.c` & `Nuitka-2.1.6/nuitka/build/static_src/CompiledFrameType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/CompiledFunctionType.c` & `Nuitka-2.1.6/nuitka/build/static_src/CompiledFunctionType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/CompiledGeneratorType.c` & `Nuitka-2.1.6/nuitka/build/static_src/CompiledGeneratorType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c` & `Nuitka-2.1.6/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/CompiledMethodType.c` & `Nuitka-2.1.6/nuitka/build/static_src/CompiledMethodType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersAllocator.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersAllocator.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersAttributes.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersAttributes.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersBuiltin.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersBuiltin.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersBuiltinTypeMethods.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersBuiltinTypeMethods.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersBytes.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersBytes.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersCalling.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersCalling.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersCallingGenerated.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersCallingGenerated.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersChecksumTools.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersChecksumTools.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersClasses.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersClasses.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersComparisonEq.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersComparisonEq.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersComparisonEqUtils.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersComparisonEqUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersComparisonGe.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersComparisonGe.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersComparisonGt.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersComparisonGt.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersComparisonLe.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersComparisonLe.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersComparisonLt.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersComparisonLt.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersComparisonNe.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersComparisonNe.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersConstantsBlob.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersConstantsBlob.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersDeepcopy.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersDeepcopy.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersDictionaries.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersDictionaries.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersDictionariesGenerated.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersDictionariesGenerated.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersDumpBacktraces.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersDumpBacktraces.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersEnvironmentVariables.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersEnvironmentVariables.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersEnvironmentVariablesSystem.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersEnvironmentVariablesSystem.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersExceptions.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersExceptions.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersFiles.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersFiles.c`

 * *Files 2% similar despite different names*

```diff
@@ -225,14 +225,23 @@
 
     PyObject *result = CALL_FUNCTION_WITH_SINGLE_ARG(tstate, isabs_func, filename);
 
     Py_DECREF(isabs_func);
     return result;
 }
 
+extern PyObject *OS_PATH_NORMPATH(PyThreadState *tstate, PyObject *filename) {
+    PyObject *normpath_func = LOOKUP_ATTRIBUTE(tstate, IMPORT_HARD_OS_PATH(tstate), const_str_plain_normpath);
+
+    PyObject *result = CALL_FUNCTION_WITH_SINGLE_ARG(tstate, normpath_func, filename);
+
+    Py_DECREF(normpath_func);
+    return result;
+}
+
 nuitka_bool compareFilePaths(PyThreadState *tstate, PyObject *filename_a, PyObject *filename_b) {
     filename_a = OS_PATH_ABSPATH(tstate, filename_a);
 
     if (unlikely(filename_a == NULL)) {
         return NUITKA_BOOL_EXCEPTION;
     }
```

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersFilesystemPaths.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersFilesystemPaths.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersFloats.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersFloats.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersHeapStorage.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersHeapStorage.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersImport.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersImport.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersImportHard.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersImportHard.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersLists.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersLists.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersListsGenerated.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersListsGenerated.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersMappings.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersMappings.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersMatching.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersMatching.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryAdd.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryAdd.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryBitand.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryBitand.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryBitor.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryBitor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryBitxor.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryBitxor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryDivmod.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryDivmod.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryLshift.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryLshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryMatmult.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryMatmult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryMod.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryMod.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryMult.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryMult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryPow.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryPow.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryRshift.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryRshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinarySub.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinarySub.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationBinaryTruediv.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationBinaryTruediv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationInplaceAdd.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationInplaceAdd.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationInplaceBitand.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationInplaceBitand.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationInplaceBitor.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationInplaceBitor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationInplaceBitxor.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationInplaceBitxor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationInplaceLshift.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationInplaceLshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationInplaceMatmult.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationInplaceMatmult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationInplaceMod.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationInplaceMod.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationInplaceMult.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationInplaceMult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationInplacePow.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationInplacePow.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationInplaceRshift.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationInplaceRshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationInplaceSub.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationInplaceSub.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersOperationInplaceTruediv.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersOperationInplaceTruediv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersProfiling.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersProfiling.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersPythonPgo.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersPythonPgo.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersRaising.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersRaising.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersSafeStrings.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersSafeStrings.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersSequences.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersSequences.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersSlices.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersSlices.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersStrings.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersStrings.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersTuples.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersTuples.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/HelpersTypes.c` & `Nuitka-2.1.6/nuitka/build/static_src/HelpersTypes.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/InspectPatcher.c` & `Nuitka-2.1.6/nuitka/build/static_src/InspectPatcher.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/MainProgram.c` & `Nuitka-2.1.6/nuitka/build/static_src/MainProgram.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/MetaPathBasedLoader.c` & `Nuitka-2.1.6/nuitka/build/static_src/MetaPathBasedLoader.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c` & `Nuitka-2.1.6/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c` & `Nuitka-2.1.6/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c` & `Nuitka-2.1.6/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/OnefileBootstrap.c` & `Nuitka-2.1.6/nuitka/build/static_src/OnefileBootstrap.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/build/static_src/OnefileSplashScreen.cpp` & `Nuitka-2.1.6/nuitka/build/static_src/OnefileSplashScreen.cpp`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/AsyncgenCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/AsyncgenCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/AttributeCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/AttributeCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/BinaryOperationHelperDefinitions.py` & `Nuitka-2.1.6/nuitka/code_generation/BinaryOperationHelperDefinitions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/BranchCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/BranchCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/BuiltinCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/BuiltinCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/CallCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/CallCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/ClassCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/ClassCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/CodeGeneration.py` & `Nuitka-2.1.6/nuitka/code_generation/CodeGeneration.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/CodeHelperSelection.py` & `Nuitka-2.1.6/nuitka/code_generation/CodeHelperSelection.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/CodeHelpers.py` & `Nuitka-2.1.6/nuitka/code_generation/CodeHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/CodeObjectCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/CodeObjectCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/ComparisonCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/ComparisonCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/ComparisonHelperDefinitions.py` & `Nuitka-2.1.6/nuitka/code_generation/ComparisonHelperDefinitions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/ConditionalCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/ConditionalCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/ConstantCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/ConstantCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/Contexts.py` & `Nuitka-2.1.6/nuitka/code_generation/Contexts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/CoroutineCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/CoroutineCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/CtypesCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/CtypesCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/DictCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/DictCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/Emission.py` & `Nuitka-2.1.6/nuitka/code_generation/Emission.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/ErrorCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/ErrorCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/EvalCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/EvalCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/ExceptionCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/ExceptionCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py` & `Nuitka-2.1.6/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/ExpressionCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/ExpressionCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/FrameCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/FrameCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/FunctionCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/FunctionCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/GeneratorCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/GeneratorCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/GlobalConstants.py` & `Nuitka-2.1.6/nuitka/code_generation/GlobalConstants.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,14 +97,15 @@
         "/",
         "\\",
         "path",
         "basename",
         "dirname",
         "abspath",
         "isabs",
+        "normpath",
         "exists",
         "isdir",
         "isfile",
         "listdir",
     ]
 
     # Pickling of instance methods.
```

### Comparing `Nuitka-2.1.5/nuitka/code_generation/GlobalsLocalsCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/GlobalsLocalsCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/IdCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/IdCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/ImportCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/ImportCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/Indentation.py` & `Nuitka-2.1.6/nuitka/code_generation/Indentation.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/IndexCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/IndexCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/InjectCCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/InjectCCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/IntegerCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/IntegerCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/IteratorCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/IteratorCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/LabelCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/LabelCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/LineNumberCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/LineNumberCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/ListCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/ListCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/LoaderCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/LoaderCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/LocalsDictCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/LocalsDictCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/LoopCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/LoopCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/MatchCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/MatchCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/ModuleCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/ModuleCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/Namify.py` & `Nuitka-2.1.6/nuitka/code_generation/Namify.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/OperationCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/OperationCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/PackageResourceCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/PackageResourceCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/PrintCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/PrintCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/PythonAPICodes.py` & `Nuitka-2.1.6/nuitka/code_generation/PythonAPICodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/RaisingCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/RaisingCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/Reports.py` & `Nuitka-2.1.6/nuitka/code_generation/Reports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/ReturnCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/ReturnCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/SetCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/SetCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/SliceCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/SliceCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/StringCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/StringCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/SubscriptCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/SubscriptCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/TryCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/TryCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/TupleCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/TupleCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/VariableCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/VariableCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/VariableDeclarations.py` & `Nuitka-2.1.6/nuitka/code_generation/VariableDeclarations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/YieldCodes.py` & `Nuitka-2.1.6/nuitka/code_generation/YieldCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/__init__.py` & `Nuitka-2.1.6/nuitka/code_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/c_types/CTypeBases.py` & `Nuitka-2.1.6/nuitka/code_generation/c_types/CTypeBases.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/c_types/CTypeBooleans.py` & `Nuitka-2.1.6/nuitka/code_generation/c_types/CTypeBooleans.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/c_types/CTypeCFloats.py` & `Nuitka-2.1.6/nuitka/code_generation/c_types/CTypeCFloats.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/c_types/CTypeCLongs.py` & `Nuitka-2.1.6/nuitka/code_generation/c_types/CTypeCLongs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/c_types/CTypeModuleDictVariables.py` & `Nuitka-2.1.6/nuitka/code_generation/c_types/CTypeModuleDictVariables.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py` & `Nuitka-2.1.6/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/c_types/CTypeNuitkaInts.py` & `Nuitka-2.1.6/nuitka/code_generation/c_types/CTypeNuitkaInts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/c_types/CTypeNuitkaVoids.py` & `Nuitka-2.1.6/nuitka/code_generation/c_types/CTypeNuitkaVoids.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/c_types/CTypePyObjectPointers.py` & `Nuitka-2.1.6/nuitka/code_generation/c_types/CTypePyObjectPointers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/c_types/CTypeVoids.py` & `Nuitka-2.1.6/nuitka/code_generation/c_types/CTypeVoids.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/c_types/__init__.py` & `Nuitka-2.1.6/nuitka/code_generation/c_types/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py` & `Nuitka-2.1.6/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates/CodeTemplatesConstants.py` & `Nuitka-2.1.6/nuitka/code_generation/templates/CodeTemplatesConstants.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,14 +145,15 @@
     PyStructSequence_SET_ITEM(Nuitka_dunder_compiled_value, 0, PyInt_FromLong(%(nuitka_version_major)s));
     PyStructSequence_SET_ITEM(Nuitka_dunder_compiled_value, 1, PyInt_FromLong(%(nuitka_version_minor)s));
     PyStructSequence_SET_ITEM(Nuitka_dunder_compiled_value, 2, PyInt_FromLong(%(nuitka_version_micro)s));
 
     PyStructSequence_SET_ITEM(Nuitka_dunder_compiled_value, 3, Nuitka_String_FromString("%(nuitka_version_level)s"));
 
     PyObject *binary_directory = getContainingDirectoryObject(false);
+    binary_directory = OS_PATH_ABSPATH(tstate, binary_directory);
 #ifdef _NUITKA_STANDALONE
 #ifndef _NUITKA_ONEFILE_MODE
     binary_directory = STRIP_DIRNAME(binary_directory);
 #endif
 
 #ifdef _NUITKA_MACOS_BUNDLE
     binary_directory = STRIP_DIRNAME(binary_directory);
```

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates/CodeTemplatesCoroutines.py` & `Nuitka-2.1.6/nuitka/code_generation/templates/CodeTemplatesCoroutines.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates/CodeTemplatesExceptions.py` & `Nuitka-2.1.6/nuitka/code_generation/templates/CodeTemplatesExceptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates/CodeTemplatesFrames.py` & `Nuitka-2.1.6/nuitka/code_generation/templates/CodeTemplatesFrames.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates/CodeTemplatesFunction.py` & `Nuitka-2.1.6/nuitka/code_generation/templates/CodeTemplatesFunction.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py` & `Nuitka-2.1.6/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates/CodeTemplatesIterators.py` & `Nuitka-2.1.6/nuitka/code_generation/templates/CodeTemplatesIterators.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates/CodeTemplatesLoader.py` & `Nuitka-2.1.6/nuitka/code_generation/templates/CodeTemplatesLoader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates/CodeTemplatesModules.py` & `Nuitka-2.1.6/nuitka/code_generation/templates/CodeTemplatesModules.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates/CodeTemplatesVariables.py` & `Nuitka-2.1.6/nuitka/code_generation/templates/CodeTemplatesVariables.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates/TemplateDebugWrapper.py` & `Nuitka-2.1.6/nuitka/code_generation/templates/TemplateDebugWrapper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates/__init__.py` & `Nuitka-2.1.6/nuitka/code_generation/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperImportHard.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperImportHard.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperLongTools.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperLongTools.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperObjectTools.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperObjectTools.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperSlotsList.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperSlotsList.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2` & `Nuitka-2.1.6/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/containers/Namedtuples.py` & `Nuitka-2.1.6/nuitka/containers/Namedtuples.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/containers/OrderedDicts.py` & `Nuitka-2.1.6/nuitka/containers/OrderedDicts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/containers/OrderedSets.py` & `Nuitka-2.1.6/nuitka/containers/OrderedSets.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/containers/OrderedSetsFallback.py` & `Nuitka-2.1.6/nuitka/containers/OrderedSetsFallback.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/containers/__init__.py` & `Nuitka-2.1.6/nuitka/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/distutils/Build.py` & `Nuitka-2.1.6/nuitka/distutils/Build.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/distutils/DistutilCommands.py` & `Nuitka-2.1.6/nuitka/distutils/DistutilCommands.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/distutils/__init__.py` & `Nuitka-2.1.6/nuitka/distutils/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/finalizations/Finalization.py` & `Nuitka-2.1.6/nuitka/finalizations/Finalization.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/finalizations/FinalizeMarkups.py` & `Nuitka-2.1.6/nuitka/finalizations/FinalizeMarkups.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/finalizations/__init__.py` & `Nuitka-2.1.6/nuitka/finalizations/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/freezer/DependsExe.py` & `Nuitka-2.1.6/nuitka/freezer/DependsExe.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/freezer/DllDependenciesCommon.py` & `Nuitka-2.1.6/nuitka/freezer/DllDependenciesCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/freezer/DllDependenciesMacOS.py` & `Nuitka-2.1.6/nuitka/freezer/DllDependenciesMacOS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/freezer/DllDependenciesPosix.py` & `Nuitka-2.1.6/nuitka/freezer/DllDependenciesPosix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/freezer/DllDependenciesWin32.py` & `Nuitka-2.1.6/nuitka/freezer/DllDependenciesWin32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/freezer/ImportDetection.py` & `Nuitka-2.1.6/nuitka/freezer/ImportDetection.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/freezer/IncludedDataFiles.py` & `Nuitka-2.1.6/nuitka/freezer/IncludedDataFiles.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/freezer/IncludedEntryPoints.py` & `Nuitka-2.1.6/nuitka/freezer/IncludedEntryPoints.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/freezer/Onefile.py` & `Nuitka-2.1.6/nuitka/freezer/Onefile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/freezer/Standalone.py` & `Nuitka-2.1.6/nuitka/freezer/Standalone.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/freezer/__init__.py` & `Nuitka-2.1.6/nuitka/freezer/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/importing/IgnoreListing.py` & `Nuitka-2.1.6/nuitka/importing/IgnoreListing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/importing/ImportCache.py` & `Nuitka-2.1.6/nuitka/importing/ImportCache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/importing/ImportResolving.py` & `Nuitka-2.1.6/nuitka/importing/ImportResolving.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/importing/Importing.py` & `Nuitka-2.1.6/nuitka/importing/Importing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/importing/PreloadedPackages.py` & `Nuitka-2.1.6/nuitka/importing/PreloadedPackages.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/importing/Recursion.py` & `Nuitka-2.1.6/nuitka/importing/Recursion.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/importing/StandardLibrary.py` & `Nuitka-2.1.6/nuitka/importing/StandardLibrary.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/importing/__init__.py` & `Nuitka-2.1.6/nuitka/importing/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/AsyncgenNodes.py` & `Nuitka-2.1.6/nuitka/nodes/AsyncgenNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/AttributeLookupNodes.py` & `Nuitka-2.1.6/nuitka/nodes/AttributeLookupNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/AttributeNodes.py` & `Nuitka-2.1.6/nuitka/nodes/AttributeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/AttributeNodesGenerated.py` & `Nuitka-2.1.6/nuitka/nodes/AttributeNodesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/BuiltinAllNodes.py` & `Nuitka-2.1.6/nuitka/nodes/BuiltinAllNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/BuiltinAnyNodes.py` & `Nuitka-2.1.6/nuitka/nodes/BuiltinAnyNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/BuiltinComplexNodes.py` & `Nuitka-2.1.6/nuitka/nodes/BuiltinComplexNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/BuiltinDecodingNodes.py` & `Nuitka-2.1.6/nuitka/nodes/BuiltinDecodingNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/BuiltinDecoratorNodes.py` & `Nuitka-2.1.6/nuitka/nodes/BuiltinDecoratorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/BuiltinDictNodes.py` & `Nuitka-2.1.6/nuitka/nodes/BuiltinDictNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/BuiltinFormatNodes.py` & `Nuitka-2.1.6/nuitka/nodes/BuiltinFormatNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/BuiltinHashNodes.py` & `Nuitka-2.1.6/nuitka/nodes/BuiltinHashNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/BuiltinInputNodes.py` & `Nuitka-2.1.6/nuitka/nodes/BuiltinInputNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/BuiltinIntegerNodes.py` & `Nuitka-2.1.6/nuitka/nodes/BuiltinIntegerNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/BuiltinIteratorNodes.py` & `Nuitka-2.1.6/nuitka/nodes/BuiltinIteratorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/BuiltinLenNodes.py` & `Nuitka-2.1.6/nuitka/nodes/BuiltinLenNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/BuiltinNextNodes.py` & `Nuitka-2.1.6/nuitka/nodes/BuiltinNextNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/BuiltinOpenNodes.py` & `Nuitka-2.1.6/nuitka/nodes/BuiltinOpenNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py` & `Nuitka-2.1.6/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/BuiltinRangeNodes.py` & `Nuitka-2.1.6/nuitka/nodes/BuiltinRangeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/BuiltinRefNodes.py` & `Nuitka-2.1.6/nuitka/nodes/BuiltinRefNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/BuiltinSumNodes.py` & `Nuitka-2.1.6/nuitka/nodes/BuiltinSumNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/BuiltinTypeNodes.py` & `Nuitka-2.1.6/nuitka/nodes/BuiltinTypeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/BuiltinVarsNodes.py` & `Nuitka-2.1.6/nuitka/nodes/BuiltinVarsNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/BytesNodes.py` & `Nuitka-2.1.6/nuitka/nodes/BytesNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/CallNodes.py` & `Nuitka-2.1.6/nuitka/nodes/CallNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/Checkers.py` & `Nuitka-2.1.6/nuitka/nodes/Checkers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/ChildrenHavingMixins.py` & `Nuitka-2.1.6/nuitka/nodes/ChildrenHavingMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/ClassNodes.py` & `Nuitka-2.1.6/nuitka/nodes/ClassNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/CodeObjectSpecs.py` & `Nuitka-2.1.6/nuitka/nodes/CodeObjectSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/ComparisonNodes.py` & `Nuitka-2.1.6/nuitka/nodes/ComparisonNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/ConditionalNodes.py` & `Nuitka-2.1.6/nuitka/nodes/ConditionalNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/ConstantRefNodes.py` & `Nuitka-2.1.6/nuitka/nodes/ConstantRefNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/ContainerMakingNodes.py` & `Nuitka-2.1.6/nuitka/nodes/ContainerMakingNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/ContainerOperationNodes.py` & `Nuitka-2.1.6/nuitka/nodes/ContainerOperationNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/CoroutineNodes.py` & `Nuitka-2.1.6/nuitka/nodes/CoroutineNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/CtypesNodes.py` & `Nuitka-2.1.6/nuitka/nodes/CtypesNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/DictionaryNodes.py` & `Nuitka-2.1.6/nuitka/nodes/DictionaryNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/ExceptionNodes.py` & `Nuitka-2.1.6/nuitka/nodes/ExceptionNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/ExecEvalNodes.py` & `Nuitka-2.1.6/nuitka/nodes/ExecEvalNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/ExpressionBases.py` & `Nuitka-2.1.6/nuitka/nodes/ExpressionBases.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/ExpressionBasesGenerated.py` & `Nuitka-2.1.6/nuitka/nodes/ExpressionBasesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/ExpressionShapeMixins.py` & `Nuitka-2.1.6/nuitka/nodes/ExpressionShapeMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/FrameNodes.py` & `Nuitka-2.1.6/nuitka/nodes/FrameNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/FunctionAttributeNodes.py` & `Nuitka-2.1.6/nuitka/nodes/FunctionAttributeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/FunctionNodes.py` & `Nuitka-2.1.6/nuitka/nodes/FunctionNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/FutureSpecs.py` & `Nuitka-2.1.6/nuitka/nodes/FutureSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/GeneratorNodes.py` & `Nuitka-2.1.6/nuitka/nodes/GeneratorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/GlobalsLocalsNodes.py` & `Nuitka-2.1.6/nuitka/nodes/GlobalsLocalsNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/HardImportNodesGenerated.py` & `Nuitka-2.1.6/nuitka/nodes/HardImportNodesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/ImportHardNodes.py` & `Nuitka-2.1.6/nuitka/nodes/ImportHardNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/ImportNodes.py` & `Nuitka-2.1.6/nuitka/nodes/ImportNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/IndicatorMixins.py` & `Nuitka-2.1.6/nuitka/nodes/IndicatorMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/InjectCNodes.py` & `Nuitka-2.1.6/nuitka/nodes/InjectCNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/IterationHandles.py` & `Nuitka-2.1.6/nuitka/nodes/IterationHandles.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/KeyValuePairNodes.py` & `Nuitka-2.1.6/nuitka/nodes/KeyValuePairNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/ListOperationNodes.py` & `Nuitka-2.1.6/nuitka/nodes/ListOperationNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/LocalsDictNodes.py` & `Nuitka-2.1.6/nuitka/nodes/LocalsDictNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/LocalsScopes.py` & `Nuitka-2.1.6/nuitka/nodes/LocalsScopes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/LoopNodes.py` & `Nuitka-2.1.6/nuitka/nodes/LoopNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/MatchNodes.py` & `Nuitka-2.1.6/nuitka/nodes/MatchNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/ModuleAttributeNodes.py` & `Nuitka-2.1.6/nuitka/nodes/ModuleAttributeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/ModuleNodes.py` & `Nuitka-2.1.6/nuitka/nodes/ModuleNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/NodeBases.py` & `Nuitka-2.1.6/nuitka/nodes/NodeBases.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/NodeMakingHelpers.py` & `Nuitka-2.1.6/nuitka/nodes/NodeMakingHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/NodeMetaClasses.py` & `Nuitka-2.1.6/nuitka/nodes/NodeMetaClasses.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/OperatorNodes.py` & `Nuitka-2.1.6/nuitka/nodes/OperatorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/OperatorNodesUnary.py` & `Nuitka-2.1.6/nuitka/nodes/OperatorNodesUnary.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/OsSysNodes.py` & `Nuitka-2.1.6/nuitka/nodes/OsSysNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/OutlineNodes.py` & `Nuitka-2.1.6/nuitka/nodes/OutlineNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/PackageMetadataNodes.py` & `Nuitka-2.1.6/nuitka/nodes/PackageMetadataNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/PackageResourceNodes.py` & `Nuitka-2.1.6/nuitka/nodes/PackageResourceNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/PrintNodes.py` & `Nuitka-2.1.6/nuitka/nodes/PrintNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/ReturnNodes.py` & `Nuitka-2.1.6/nuitka/nodes/ReturnNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/SideEffectNodes.py` & `Nuitka-2.1.6/nuitka/nodes/SideEffectNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/SliceNodes.py` & `Nuitka-2.1.6/nuitka/nodes/SliceNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/StatementBasesGenerated.py` & `Nuitka-2.1.6/nuitka/nodes/StatementBasesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/StatementNodes.py` & `Nuitka-2.1.6/nuitka/nodes/StatementNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/StrNodes.py` & `Nuitka-2.1.6/nuitka/nodes/StrNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/StringConcatenationNodes.py` & `Nuitka-2.1.6/nuitka/nodes/StringConcatenationNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/SubscriptNodes.py` & `Nuitka-2.1.6/nuitka/nodes/SubscriptNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/TryNodes.py` & `Nuitka-2.1.6/nuitka/nodes/TryNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/TypeMatchNodes.py` & `Nuitka-2.1.6/nuitka/nodes/TypeMatchNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/TypeNodes.py` & `Nuitka-2.1.6/nuitka/nodes/TypeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/VariableAssignNodes.py` & `Nuitka-2.1.6/nuitka/nodes/VariableAssignNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/VariableDelNodes.py` & `Nuitka-2.1.6/nuitka/nodes/VariableDelNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/VariableNameNodes.py` & `Nuitka-2.1.6/nuitka/nodes/VariableNameNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/VariableRefNodes.py` & `Nuitka-2.1.6/nuitka/nodes/VariableRefNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/VariableReleaseNodes.py` & `Nuitka-2.1.6/nuitka/nodes/VariableReleaseNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/YieldNodes.py` & `Nuitka-2.1.6/nuitka/nodes/YieldNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/__init__.py` & `Nuitka-2.1.6/nuitka/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/shapes/BuiltinTypeShapes.py` & `Nuitka-2.1.6/nuitka/nodes/shapes/BuiltinTypeShapes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/shapes/ControlFlowDescriptions.py` & `Nuitka-2.1.6/nuitka/nodes/shapes/ControlFlowDescriptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/shapes/ShapeMixins.py` & `Nuitka-2.1.6/nuitka/nodes/shapes/ShapeMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/shapes/StandardShapes.py` & `Nuitka-2.1.6/nuitka/nodes/shapes/StandardShapes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/nodes/shapes/__init__.py` & `Nuitka-2.1.6/nuitka/nodes/shapes/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/optimizations/BytecodeDemotion.py` & `Nuitka-2.1.6/nuitka/optimizations/BytecodeDemotion.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/optimizations/FunctionInlining.py` & `Nuitka-2.1.6/nuitka/optimizations/FunctionInlining.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/optimizations/Graphs.py` & `Nuitka-2.1.6/nuitka/optimizations/Graphs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/optimizations/Optimization.py` & `Nuitka-2.1.6/nuitka/optimizations/Optimization.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/optimizations/OptimizeBuiltinCalls.py` & `Nuitka-2.1.6/nuitka/optimizations/OptimizeBuiltinCalls.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/optimizations/Tags.py` & `Nuitka-2.1.6/nuitka/optimizations/Tags.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/optimizations/TraceCollections.py` & `Nuitka-2.1.6/nuitka/optimizations/TraceCollections.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/optimizations/ValueTraces.py` & `Nuitka-2.1.6/nuitka/optimizations/ValueTraces.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/optimizations/__init__.py` & `Nuitka-2.1.6/nuitka/optimizations/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/pgo/PGO.py` & `Nuitka-2.1.6/nuitka/pgo/PGO.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/pgo/__init__.py` & `Nuitka-2.1.6/nuitka/pgo/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/PluginBase.py` & `Nuitka-2.1.6/nuitka/plugins/PluginBase.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/Plugins.py` & `Nuitka-2.1.6/nuitka/plugins/Plugins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/__init__.py` & `Nuitka-2.1.6/nuitka/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/AntiBloatPlugin.py` & `Nuitka-2.1.6/nuitka/plugins/standard/AntiBloatPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py` & `Nuitka-2.1.6/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/DataFilesPlugin.py` & `Nuitka-2.1.6/nuitka/plugins/standard/DataFilesPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/DelvewheelPlugin.py` & `Nuitka-2.1.6/nuitka/plugins/standard/DelvewheelPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/DillPlugin/DillPlugin.c` & `Nuitka-2.1.6/nuitka/plugins/standard/DillPlugin/DillPlugin.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/DillPlugin/dill-postLoad.py` & `Nuitka-2.1.6/nuitka/plugins/standard/DillPlugin/dill-postLoad.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/DillPlugin.py` & `Nuitka-2.1.6/nuitka/plugins/standard/DillPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/DllFilesPlugin.py` & `Nuitka-2.1.6/nuitka/plugins/standard/DllFilesPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/EnumPlugin.py` & `Nuitka-2.1.6/nuitka/plugins/standard/EnumPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/EventletPlugin.py` & `Nuitka-2.1.6/nuitka/plugins/standard/EventletPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/GeventPlugin.py` & `Nuitka-2.1.6/nuitka/plugins/standard/GeventPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/GiPlugin.py` & `Nuitka-2.1.6/nuitka/plugins/standard/GiPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/GlfwPlugin.py` & `Nuitka-2.1.6/nuitka/plugins/standard/GlfwPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/ImplicitImports.py` & `Nuitka-2.1.6/nuitka/plugins/standard/ImplicitImports.py`

 * *Files 0% similar despite different names*

```diff
@@ -656,14 +656,15 @@
         "azure.mgmt.compute",  # Too large generated code
         "transformers.utils.dummy_pt_objects",  # Not performance relevant.
         "transformers.utils.dummy_flax_objects",  # Not performance relevant.
         "transformers.utils.dummy_tf_objects",  # Not performance relevant.
         "rich",  #  Not performance relevant and memory leaking due to empty compiled cell leaks
         "altair.vegalite.v5.schema",  # Not performance relevant.
         "azure",  # Not performance relevant.
+        "networkx",  # Needs solutions for bytecode requiring decorators.
     )
 
     unworthy_modulename_patterns = (
         "tensorflow.*test",  # Not performance relevant.
         "tensorflow.**.test_util",  # Not performance relevant.
     )
```

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/KivyPlugin.py` & `Nuitka-2.1.6/nuitka/plugins/standard/KivyPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/MatplotlibPlugin.py` & `Nuitka-2.1.6/nuitka/plugins/standard/MatplotlibPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/MultiprocessingPlugin.py` & `Nuitka-2.1.6/nuitka/plugins/standard/MultiprocessingPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/NumpyPlugin.py` & `Nuitka-2.1.6/nuitka/plugins/standard/NumpyPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/OptionsNannyPlugin.py` & `Nuitka-2.1.6/nuitka/plugins/standard/OptionsNannyPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/PbrPlugin.py` & `Nuitka-2.1.6/nuitka/plugins/standard/PbrPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/PkgResourcesPlugin.py` & `Nuitka-2.1.6/nuitka/plugins/standard/PkgResourcesPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/PmwPlugin.py` & `Nuitka-2.1.6/nuitka/plugins/standard/PmwPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/PySidePyQtPlugin.py` & `Nuitka-2.1.6/nuitka/plugins/standard/PySidePyQtPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/PywebViewPlugin.py` & `Nuitka-2.1.6/nuitka/plugins/standard/PywebViewPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/TensorflowPlugin.py` & `Nuitka-2.1.6/nuitka/plugins/standard/TensorflowPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/TkinterPlugin.py` & `Nuitka-2.1.6/nuitka/plugins/standard/TkinterPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/TorchPlugin.py` & `Nuitka-2.1.6/nuitka/plugins/standard/TorchPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/TransformersPlugin.py` & `Nuitka-2.1.6/nuitka/plugins/standard/TransformersPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/TrioPlugin.py` & `Nuitka-2.1.6/nuitka/plugins/standard/TrioPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/UpxPlugin.py` & `Nuitka-2.1.6/nuitka/plugins/standard/UpxPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/__init__.py` & `Nuitka-2.1.6/nuitka/plugins/standard/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/standard.nuitka-package.config.yml` & `Nuitka-2.1.6/nuitka/plugins/standard/standard.nuitka-package.config.yml`

 * *Files 0% similar despite different names*

```diff
@@ -2259,34 +2259,14 @@
 - module-name: 'networkx.classes.backends' # checksum: 29bf8c92
   anti-bloat:
     - description: 'remove pytest reference'
       replacements_plain:
         'os.environ.get("NETWORKX_GRAPH_CONVERT")': 'None'
       when: 'not use_pytest'
 
-- module-name: 'networkx.utils.decorators' # checksum: 7f34ff95
-  anti-bloat:
-    - description: 'required for decorator compatibility'
-      replacements_plain:
-        'func.__defaults__ = f.__defaults__': ''
-        'real_func = func.__argmap__.compile(func.__wrapped__)': 'return func'
-        '    return argmap(_not_implemented_for, 0)': |
-          #
-              import functools
-              def inner(func):
-                  @functools.wraps(func)
-                  def _not_implemented_for(g):
-                      if (mval is None or mval == g.is_multigraph()) and (
-                          dval is None or dval == g.is_directed()
-                      ):
-                          raise nx.NetworkXNotImplemented(errmsg)
-                      return func(g)
-                  return _not_implemented_for
-              return inner
-
 - module-name: 'nose.core' # checksum: 8247f58b
   data-files:
     patterns:
       - 'usage.txt'
 
 - module-name: 'numba' # checksum: a8eab062
   parameters:
```

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml` & `Nuitka-2.1.6/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml` & `Nuitka-2.1.6/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/reports/CompilationReportReader.py` & `Nuitka-2.1.6/nuitka/reports/CompilationReportReader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/reports/LicenseReport.rst.j2` & `Nuitka-2.1.6/nuitka/reports/LicenseReport.rst.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/reports/Reports.py` & `Nuitka-2.1.6/nuitka/reports/Reports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/reports/__init__.py` & `Nuitka-2.1.6/nuitka/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/specs/BuiltinBytesOperationSpecs.py` & `Nuitka-2.1.6/nuitka/specs/BuiltinBytesOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/specs/BuiltinDictOperationSpecs.py` & `Nuitka-2.1.6/nuitka/specs/BuiltinDictOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/specs/BuiltinListOperationSpecs.py` & `Nuitka-2.1.6/nuitka/specs/BuiltinListOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/specs/BuiltinParameterSpecs.py` & `Nuitka-2.1.6/nuitka/specs/BuiltinParameterSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/specs/BuiltinStrOperationSpecs.py` & `Nuitka-2.1.6/nuitka/specs/BuiltinStrOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/specs/BuiltinTypeOperationSpecs.py` & `Nuitka-2.1.6/nuitka/specs/BuiltinTypeOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/specs/BuiltinUnicodeOperationSpecs.py` & `Nuitka-2.1.6/nuitka/specs/BuiltinUnicodeOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/specs/HardImportSpecs.py` & `Nuitka-2.1.6/nuitka/specs/HardImportSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/specs/ParameterSpecs.py` & `Nuitka-2.1.6/nuitka/specs/ParameterSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/specs/__init__.py` & `Nuitka-2.1.6/nuitka/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/Basics.py` & `Nuitka-2.1.6/nuitka/tools/Basics.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/__init__.py` & `Nuitka-2.1.6/nuitka/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/commercial/__init__.py` & `Nuitka-2.1.6/nuitka/tools/commercial/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/data_composer/DataComposer.py` & `Nuitka-2.1.6/nuitka/tools/data_composer/DataComposer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/data_composer/__init__.py` & `Nuitka-2.1.6/nuitka/tools/data_composer/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/data_composer/__main__.py` & `Nuitka-2.1.6/nuitka/tools/data_composer/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/environments/CreateEnvironment.py` & `Nuitka-2.1.6/nuitka/tools/environments/CreateEnvironment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/environments/Virtualenv.py` & `Nuitka-2.1.6/nuitka/tools/environments/Virtualenv.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/environments/__init__.py` & `Nuitka-2.1.6/nuitka/tools/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/general/__init__.py` & `Nuitka-2.1.6/nuitka/tools/general/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/general/dll_report/__init__.py` & `Nuitka-2.1.6/nuitka/tools/general/dll_report/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/general/dll_report/__main__.py` & `Nuitka-2.1.6/nuitka/tools/general/dll_report/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/general/find_module/FindModuleCode.py` & `Nuitka-2.1.6/nuitka/tools/general/find_module/FindModuleCode.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/general/find_module/__init__.py` & `Nuitka-2.1.6/nuitka/tools/general/find_module/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/onefile_compressor/OnefileCompressor.py` & `Nuitka-2.1.6/nuitka/tools/onefile_compressor/OnefileCompressor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/onefile_compressor/__init__.py` & `Nuitka-2.1.6/nuitka/tools/onefile_compressor/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/onefile_compressor/__main__.py` & `Nuitka-2.1.6/nuitka/tools/onefile_compressor/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/podman/Podman.py` & `Nuitka-2.1.6/nuitka/tools/podman/Podman.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/podman/__init__.py` & `Nuitka-2.1.6/nuitka/tools/podman/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/podman/__main__.py` & `Nuitka-2.1.6/nuitka/tools/podman/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/profiler/__init__.py` & `Nuitka-2.1.6/nuitka/tools/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/profiler/__main__.py` & `Nuitka-2.1.6/nuitka/tools/profiler/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/scanning/DisplayPackageDLLs.py` & `Nuitka-2.1.6/nuitka/tools/scanning/DisplayPackageDLLs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/scanning/DisplayPackageData.py` & `Nuitka-2.1.6/nuitka/tools/scanning/DisplayPackageData.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/scanning/__init__.py` & `Nuitka-2.1.6/nuitka/tools/scanning/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/specialize/CTypeDescriptions.py` & `Nuitka-2.1.6/nuitka/tools/specialize/CTypeDescriptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/specialize/Common.py` & `Nuitka-2.1.6/nuitka/tools/specialize/Common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/specialize/SpecializeC.py` & `Nuitka-2.1.6/nuitka/tools/specialize/SpecializeC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/specialize/SpecializePython.py` & `Nuitka-2.1.6/nuitka/tools/specialize/SpecializePython.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/specialize/__init__.py` & `Nuitka-2.1.6/nuitka/tools/specialize/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/testing/Common.py` & `Nuitka-2.1.6/nuitka/tools/testing/Common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/testing/Constructs.py` & `Nuitka-2.1.6/nuitka/tools/testing/Constructs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/testing/OutputComparison.py` & `Nuitka-2.1.6/nuitka/tools/testing/OutputComparison.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/testing/Pythons.py` & `Nuitka-2.1.6/nuitka/tools/testing/Pythons.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/testing/RuntimeTracing.py` & `Nuitka-2.1.6/nuitka/tools/testing/RuntimeTracing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/testing/SearchModes.py` & `Nuitka-2.1.6/nuitka/tools/testing/SearchModes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/testing/Valgrind.py` & `Nuitka-2.1.6/nuitka/tools/testing/Valgrind.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/testing/__init__.py` & `Nuitka-2.1.6/nuitka/tools/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/testing/check_reference_counts/__init__.py` & `Nuitka-2.1.6/nuitka/tools/testing/check_reference_counts/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/testing/check_reference_counts/__main__.py` & `Nuitka-2.1.6/nuitka/tools/testing/check_reference_counts/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/testing/compare_with_cpython/__init__.py` & `Nuitka-2.1.6/nuitka/tools/testing/compare_with_cpython/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/testing/compare_with_cpython/__main__.py` & `Nuitka-2.1.6/nuitka/tools/testing/compare_with_cpython/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/testing/find_sxs_modules/__init__.py` & `Nuitka-2.1.6/nuitka/tools/testing/find_sxs_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/testing/find_sxs_modules/__main__.py` & `Nuitka-2.1.6/nuitka/tools/testing/find_sxs_modules/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/testing/measure_construct_performance/__init__.py` & `Nuitka-2.1.6/nuitka/tools/testing/measure_construct_performance/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/testing/measure_construct_performance/__main__.py` & `Nuitka-2.1.6/nuitka/tools/testing/measure_construct_performance/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/testing/run_nuitka_tests/__init__.py` & `Nuitka-2.1.6/nuitka/tools/testing/run_nuitka_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/testing/run_nuitka_tests/__main__.py` & `Nuitka-2.1.6/nuitka/tools/testing/run_nuitka_tests/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/watch/GitHub.py` & `Nuitka-2.1.6/nuitka/tools/watch/GitHub.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/watch/__init__.py` & `Nuitka-2.1.6/nuitka/tools/watch/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tools/watch/__main__.py` & `Nuitka-2.1.6/nuitka/tools/watch/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/Building.py` & `Nuitka-2.1.6/nuitka/tree/Building.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/ComplexCallHelperFunctions.py` & `Nuitka-2.1.6/nuitka/tree/ComplexCallHelperFunctions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/Extractions.py` & `Nuitka-2.1.6/nuitka/tree/Extractions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/InternalModule.py` & `Nuitka-2.1.6/nuitka/tree/InternalModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/Operations.py` & `Nuitka-2.1.6/nuitka/tree/Operations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/ReformulationAssertStatements.py` & `Nuitka-2.1.6/nuitka/tree/ReformulationAssertStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/ReformulationAssignmentStatements.py` & `Nuitka-2.1.6/nuitka/tree/ReformulationAssignmentStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/ReformulationBooleanExpressions.py` & `Nuitka-2.1.6/nuitka/tree/ReformulationBooleanExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/ReformulationCallExpressions.py` & `Nuitka-2.1.6/nuitka/tree/ReformulationCallExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/ReformulationClasses.py` & `Nuitka-2.1.6/nuitka/tree/ReformulationClasses.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/ReformulationClasses3.py` & `Nuitka-2.1.6/nuitka/tree/ReformulationClasses3.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/ReformulationComparisonExpressions.py` & `Nuitka-2.1.6/nuitka/tree/ReformulationComparisonExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/ReformulationContractionExpressions.py` & `Nuitka-2.1.6/nuitka/tree/ReformulationContractionExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/ReformulationDictionaryCreation.py` & `Nuitka-2.1.6/nuitka/tree/ReformulationDictionaryCreation.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/ReformulationExecStatements.py` & `Nuitka-2.1.6/nuitka/tree/ReformulationExecStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/ReformulationForLoopStatements.py` & `Nuitka-2.1.6/nuitka/tree/ReformulationForLoopStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/ReformulationFunctionStatements.py` & `Nuitka-2.1.6/nuitka/tree/ReformulationFunctionStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/ReformulationImportStatements.py` & `Nuitka-2.1.6/nuitka/tree/ReformulationImportStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/ReformulationLambdaExpressions.py` & `Nuitka-2.1.6/nuitka/tree/ReformulationLambdaExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/ReformulationMatchStatements.py` & `Nuitka-2.1.6/nuitka/tree/ReformulationMatchStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/ReformulationMultidist.py` & `Nuitka-2.1.6/nuitka/tree/ReformulationMultidist.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/ReformulationNamespacePackages.py` & `Nuitka-2.1.6/nuitka/tree/ReformulationNamespacePackages.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/ReformulationPrintStatements.py` & `Nuitka-2.1.6/nuitka/tree/ReformulationPrintStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/ReformulationSequenceCreation.py` & `Nuitka-2.1.6/nuitka/tree/ReformulationSequenceCreation.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/ReformulationSubscriptExpressions.py` & `Nuitka-2.1.6/nuitka/tree/ReformulationSubscriptExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/ReformulationTryExceptStatements.py` & `Nuitka-2.1.6/nuitka/tree/ReformulationTryExceptStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/ReformulationTryFinallyStatements.py` & `Nuitka-2.1.6/nuitka/tree/ReformulationTryFinallyStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/ReformulationWhileLoopStatements.py` & `Nuitka-2.1.6/nuitka/tree/ReformulationWhileLoopStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/ReformulationWithStatements.py` & `Nuitka-2.1.6/nuitka/tree/ReformulationWithStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/ReformulationYieldExpressions.py` & `Nuitka-2.1.6/nuitka/tree/ReformulationYieldExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/SourceHandling.py` & `Nuitka-2.1.6/nuitka/tree/SourceHandling.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/SyntaxErrors.py` & `Nuitka-2.1.6/nuitka/tree/SyntaxErrors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/TreeHelpers.py` & `Nuitka-2.1.6/nuitka/tree/TreeHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/VariableClosure.py` & `Nuitka-2.1.6/nuitka/tree/VariableClosure.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/tree/__init__.py` & `Nuitka-2.1.6/nuitka/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/utils/AppDirs.py` & `Nuitka-2.1.6/nuitka/utils/AppDirs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/utils/CStrings.py` & `Nuitka-2.1.6/nuitka/utils/CStrings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/utils/CommandLineOptions.py` & `Nuitka-2.1.6/nuitka/utils/CommandLineOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/utils/Distributions.py` & `Nuitka-2.1.6/nuitka/utils/Distributions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/utils/Download.py` & `Nuitka-2.1.6/nuitka/utils/Download.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/utils/Execution.py` & `Nuitka-2.1.6/nuitka/utils/Execution.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/utils/FileOperations.py` & `Nuitka-2.1.6/nuitka/utils/FileOperations.py`

 * *Files 0% similar despite different names*

```diff
@@ -538,15 +538,15 @@
     """
 
     # Accept None value as well.
     prefix = prefix or ""
 
     # On Windows, we check exe suffixes, on other platforms we shell all filenames,
     # matching the prefix, but they have to the executable bit set.
-    if suffixes is None and isWin32OrPosixWindows():
+    if not suffixes and isWin32OrPosixWindows():
         suffixes = "exe", "bin"
 
     if suffixes:
         pattern_list = [prefix + "*." + suffix for suffix in suffixes]
     else:
         pattern_list = [prefix + "*"]
```

### Comparing `Nuitka-2.1.5/nuitka/utils/Hashing.py` & `Nuitka-2.1.6/nuitka/utils/Hashing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/utils/Images.py` & `Nuitka-2.1.6/nuitka/utils/Images.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/utils/Importing.py` & `Nuitka-2.1.6/nuitka/utils/Importing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/utils/InstalledPythons.py` & `Nuitka-2.1.6/nuitka/utils/InstalledPythons.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/utils/InstanceCounters.py` & `Nuitka-2.1.6/nuitka/utils/InstanceCounters.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/utils/Jinja2.py` & `Nuitka-2.1.6/nuitka/utils/Jinja2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/utils/Json.py` & `Nuitka-2.1.6/nuitka/utils/Json.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/utils/MacOSApp.py` & `Nuitka-2.1.6/nuitka/utils/MacOSApp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/utils/MemoryUsage.py` & `Nuitka-2.1.6/nuitka/utils/MemoryUsage.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/utils/ModuleNames.py` & `Nuitka-2.1.6/nuitka/utils/ModuleNames.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/utils/ReExecute.py` & `Nuitka-2.1.6/nuitka/utils/ReExecute.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/utils/Rest.py` & `Nuitka-2.1.6/nuitka/utils/Rest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/utils/SharedLibraries.py` & `Nuitka-2.1.6/nuitka/utils/SharedLibraries.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/utils/Shebang.py` & `Nuitka-2.1.6/nuitka/utils/Shebang.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/utils/Signing.py` & `Nuitka-2.1.6/nuitka/utils/Signing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/utils/SlotMetaClasses.py` & `Nuitka-2.1.6/nuitka/utils/SlotMetaClasses.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/utils/StaticLibraries.py` & `Nuitka-2.1.6/nuitka/utils/StaticLibraries.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/utils/ThreadedExecutor.py` & `Nuitka-2.1.6/nuitka/utils/ThreadedExecutor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/utils/Timing.py` & `Nuitka-2.1.6/nuitka/utils/Timing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/utils/Utils.py` & `Nuitka-2.1.6/nuitka/utils/Utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/utils/WindowsFileUsage.py` & `Nuitka-2.1.6/nuitka/utils/WindowsFileUsage.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/utils/WindowsResources.py` & `Nuitka-2.1.6/nuitka/utils/WindowsResources.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/utils/Yaml.py` & `Nuitka-2.1.6/nuitka/utils/Yaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/nuitka/utils/__init__.py` & `Nuitka-2.1.6/nuitka/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/pyproject.toml` & `Nuitka-2.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/setup.py` & `Nuitka-2.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/AssertsTest.py` & `Nuitka-2.1.6/tests/basics/AssertsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/AssignmentsTest.py` & `Nuitka-2.1.6/tests/basics/AssignmentsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/AssignmentsTest32.py` & `Nuitka-2.1.6/tests/basics/AssignmentsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/BranchingTest.py` & `Nuitka-2.1.6/tests/basics/BranchingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/BuiltinOverload.py` & `Nuitka-2.1.6/tests/basics/BuiltinOverload.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/BuiltinSuperTest.py` & `Nuitka-2.1.6/tests/basics/BuiltinSuperTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/BuiltinsTest.py` & `Nuitka-2.1.6/tests/basics/BuiltinsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/ClassMinimalTest.py` & `Nuitka-2.1.6/tests/basics/ClassMinimalTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/ClassesTest.py` & `Nuitka-2.1.6/tests/basics/ClassesTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/ClassesTest32.py` & `Nuitka-2.1.6/tests/basics/ClassesTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/ClassesTest34.py` & `Nuitka-2.1.6/tests/basics/ClassesTest34.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/ComparisonChainsTest.py` & `Nuitka-2.1.6/tests/basics/ComparisonChainsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/ConstantsTest.py` & `Nuitka-2.1.6/tests/basics/ConstantsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/ConstantsTest27.py` & `Nuitka-2.1.6/tests/basics/ConstantsTest27.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/DecoratorsTest.py` & `Nuitka-2.1.6/tests/basics/DecoratorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/DefaultParametersTest.py` & `Nuitka-2.1.6/tests/basics/DefaultParametersTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/DoubleDeletionsTest.py` & `Nuitka-2.1.6/tests/basics/DoubleDeletionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/EmptyModuleTest.py` & `Nuitka-2.1.6/tests/basics/EmptyModuleTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/ExceptionRaisingTest.py` & `Nuitka-2.1.6/tests/basics/ExceptionRaisingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/ExceptionRaisingTest32.py` & `Nuitka-2.1.6/tests/basics/ExceptionRaisingTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/ExceptionRaisingTest33.py` & `Nuitka-2.1.6/tests/basics/ExceptionRaisingTest33.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/ExecEvalTest.py` & `Nuitka-2.1.6/tests/basics/ExecEvalTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/ExtremeClosureTest.py` & `Nuitka-2.1.6/tests/basics/ExtremeClosureTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/FunctionObjectsTest.py` & `Nuitka-2.1.6/tests/basics/FunctionObjectsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/FunctionsTest.py` & `Nuitka-2.1.6/tests/basics/FunctionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/FunctionsTest32.py` & `Nuitka-2.1.6/tests/basics/FunctionsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/FunctionsTest_2.py` & `Nuitka-2.1.6/tests/basics/FunctionsTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/FutureTest32.py` & `Nuitka-2.1.6/tests/basics/FutureTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/GeneratorExpressionsTest.py` & `Nuitka-2.1.6/tests/basics/GeneratorExpressionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/GeneratorExpressionsTest_37.py` & `Nuitka-2.1.6/tests/basics/GeneratorExpressionsTest_37.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/GlobalStatementTest.py` & `Nuitka-2.1.6/tests/basics/GlobalStatementTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/HelloWorldTest_2.py` & `Nuitka-2.1.6/tests/basics/HelloWorldTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/ImportingTest.py` & `Nuitka-2.1.6/tests/basics/ImportingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/InplaceOperationsTest.py` & `Nuitka-2.1.6/tests/basics/InplaceOperationsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/InspectionTest.py` & `Nuitka-2.1.6/tests/basics/InspectionTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/InspectionTest_35.py` & `Nuitka-2.1.6/tests/basics/InspectionTest_35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/InspectionTest_36.py` & `Nuitka-2.1.6/tests/basics/InspectionTest_36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/LambdasTest.py` & `Nuitka-2.1.6/tests/basics/LambdasTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/LateClosureAssignmentTest.py` & `Nuitka-2.1.6/tests/basics/LateClosureAssignmentTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/ListContractionsTest.py` & `Nuitka-2.1.6/tests/basics/ListContractionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/LoopingTest.py` & `Nuitka-2.1.6/tests/basics/LoopingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/MainProgramsTest.py` & `Nuitka-2.1.6/tests/basics/MainProgramsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/ModuleAttributesTest.py` & `Nuitka-2.1.6/tests/basics/ModuleAttributesTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/OperatorsTest.py` & `Nuitka-2.1.6/tests/basics/OperatorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/OrderChecksTest.py` & `Nuitka-2.1.6/tests/basics/OrderChecksTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/OrderChecksTest27.py` & `Nuitka-2.1.6/tests/basics/OrderChecksTest27.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/OverflowFunctionsTest_2.py` & `Nuitka-2.1.6/tests/basics/OverflowFunctionsTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/ParameterErrorsTest.py` & `Nuitka-2.1.6/tests/basics/ParameterErrorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/ParameterErrorsTest32.py` & `Nuitka-2.1.6/tests/basics/ParameterErrorsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/PrintFutureTest.py` & `Nuitka-2.1.6/tests/basics/PrintFutureTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/PrintingTest_2.py` & `Nuitka-2.1.6/tests/basics/PrintingTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/RecursionTest.py` & `Nuitka-2.1.6/tests/basics/RecursionTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/ReferencingTest.py` & `Nuitka-2.1.6/tests/basics/ReferencingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/ReferencingTest27.py` & `Nuitka-2.1.6/tests/basics/ReferencingTest27.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/ReferencingTest33.py` & `Nuitka-2.1.6/tests/basics/ReferencingTest33.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/ReferencingTest35.py` & `Nuitka-2.1.6/tests/basics/ReferencingTest35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/ReferencingTest36.py` & `Nuitka-2.1.6/tests/basics/ReferencingTest36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/ReferencingTest_2.py` & `Nuitka-2.1.6/tests/basics/ReferencingTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/SlotsTest.py` & `Nuitka-2.1.6/tests/basics/SlotsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/ThreadedGeneratorsTest.py` & `Nuitka-2.1.6/tests/basics/ThreadedGeneratorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/TrickAssignmentsTest32.py` & `Nuitka-2.1.6/tests/basics/TrickAssignmentsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/TrickAssignmentsTest35.py` & `Nuitka-2.1.6/tests/basics/TrickAssignmentsTest35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/TrickAssignmentsTest_2.py` & `Nuitka-2.1.6/tests/basics/TrickAssignmentsTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/TryContinueFinallyTest.py` & `Nuitka-2.1.6/tests/basics/TryContinueFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/TryExceptContinueTest.py` & `Nuitka-2.1.6/tests/basics/TryExceptContinueTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/TryExceptFinallyTest.py` & `Nuitka-2.1.6/tests/basics/TryExceptFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/TryExceptFramesTest.py` & `Nuitka-2.1.6/tests/basics/TryExceptFramesTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/TryReturnFinallyTest.py` & `Nuitka-2.1.6/tests/basics/TryReturnFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/TryYieldFinallyTest.py` & `Nuitka-2.1.6/tests/basics/TryYieldFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/UnicodeTest.py` & `Nuitka-2.1.6/tests/basics/UnicodeTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/UnpackingTest35.py` & `Nuitka-2.1.6/tests/basics/UnpackingTest35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/VarargsTest.py` & `Nuitka-2.1.6/tests/basics/VarargsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/WithStatementsTest.py` & `Nuitka-2.1.6/tests/basics/WithStatementsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/YieldFromTest33.py` & `Nuitka-2.1.6/tests/basics/YieldFromTest33.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/run_all.py` & `Nuitka-2.1.6/tests/basics/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/basics/run_xml.py` & `Nuitka-2.1.6/tests/basics/run_xml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/onefile/HelloWorldTest.py` & `Nuitka-2.1.6/tests/onefile/HelloWorldTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/onefile/KeyboardInterruptTest.py` & `Nuitka-2.1.6/tests/onefile/KeyboardInterruptTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/onefile/run_all.py` & `Nuitka-2.1.6/tests/onefile/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/optimizations/ArgumentTypes.py` & `Nuitka-2.1.6/tests/optimizations/ArgumentTypes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/optimizations/Attributes.py` & `Nuitka-2.1.6/tests/optimizations/Attributes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/optimizations/Calls.py` & `Nuitka-2.1.6/tests/optimizations/Calls.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/optimizations/Conditions.py` & `Nuitka-2.1.6/tests/optimizations/Conditions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/optimizations/DecodingOperations.py` & `Nuitka-2.1.6/tests/optimizations/DecodingOperations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/optimizations/FormatStrings36.py` & `Nuitka-2.1.6/tests/optimizations/FormatStrings36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/optimizations/HardImports.py` & `Nuitka-2.1.6/tests/optimizations/HardImports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/optimizations/HardImports_2.py` & `Nuitka-2.1.6/tests/optimizations/HardImports_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/optimizations/Iterations.py` & `Nuitka-2.1.6/tests/optimizations/Iterations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/optimizations/Len.py` & `Nuitka-2.1.6/tests/optimizations/Len.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/optimizations/Matching310.py` & `Nuitka-2.1.6/tests/optimizations/Matching310.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/optimizations/Operations.py` & `Nuitka-2.1.6/tests/optimizations/Operations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/optimizations/Subscripts.py` & `Nuitka-2.1.6/tests/optimizations/Subscripts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/optimizations/run_all.py` & `Nuitka-2.1.6/tests/optimizations/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/packages/package_data_files_embedding/PackageDataFilesEmbedding.py` & `Nuitka-2.1.6/tests/packages/package_data_files_embedding/PackageDataFilesEmbedding.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/packages/package_data_files_embedding/__init__.py` & `Nuitka-2.1.6/tests/packages/package_data_files_embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py` & `Nuitka-2.1.6/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py` & `Nuitka-2.1.6/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/packages/package_import_success_after_failure/variable_package/__init__.py` & `Nuitka-2.1.6/tests/packages/package_import_success_after_failure/variable_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/packages/run_all.py` & `Nuitka-2.1.6/tests/packages/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/packages/sub_package/kitty/__init__.py` & `Nuitka-2.1.6/tests/packages/sub_package/kitty/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/packages/sub_package/kitty/bigkitty.py` & `Nuitka-2.1.6/tests/packages/sub_package/kitty/bigkitty.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/packages/sub_package/kitty/smallkitty.py` & `Nuitka-2.1.6/tests/packages/sub_package/kitty/smallkitty.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/packages/sub_package/kitty/speak/__init__.py` & `Nuitka-2.1.6/tests/packages/sub_package/kitty/speak/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/packages/sub_package/kitty/speak/hello.py` & `Nuitka-2.1.6/tests/packages/sub_package/kitty/speak/hello.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/packages/sub_package/kitty/speak/miau.py` & `Nuitka-2.1.6/tests/packages/sub_package/kitty/speak/miau.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/packages/sub_package/kitty/speak/purr.py` & `Nuitka-2.1.6/tests/packages/sub_package/kitty/speak/purr.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/packages/top_level_attributes_3/some_package/__init__.py` & `Nuitka-2.1.6/tests/packages/top_level_attributes_3/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/packages/top_level_attributes_3/some_package/some_module.py` & `Nuitka-2.1.6/tests/packages/top_level_attributes_3/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/plugins/code_signing/CodeSigningMain.py` & `Nuitka-2.1.6/tests/plugins/code_signing/CodeSigningMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/plugins/data_files/DataFilesMain.py` & `Nuitka-2.1.6/tests/plugins/data_files/DataFilesMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/plugins/data_files/data_files_package/__init__.py` & `Nuitka-2.1.6/tests/plugins/data_files/data_files_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/plugins/parameters/ParametersMain.py` & `Nuitka-2.1.6/tests/plugins/parameters/ParametersMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/plugins/parameters/parameter-using-plugin.py` & `Nuitka-2.1.6/tests/plugins/parameters/parameter-using-plugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/plugins/run_all.py` & `Nuitka-2.1.6/tests/plugins/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/absolute_import/AbsoluteImportMain.py` & `Nuitka-2.1.6/tests/programs/absolute_import/AbsoluteImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/absolute_import/foobar/__init__.py` & `Nuitka-2.1.6/tests/programs/absolute_import/foobar/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/absolute_import/foobar/foobar.py` & `Nuitka-2.1.6/tests/programs/absolute_import/foobar/foobar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/absolute_import/foobar/local.py` & `Nuitka-2.1.6/tests/programs/absolute_import/foobar/local.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/absolute_import/foobar/util.py` & `Nuitka-2.1.6/tests/programs/absolute_import/foobar/util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/case_imports1/CasedImportingMain.py` & `Nuitka-2.1.6/tests/programs/case_imports1/CasedImportingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/case_imports1/path1/Some_Module.py` & `Nuitka-2.1.6/tests/programs/case_imports1/path1/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/case_imports1/path1/Some_Package/__init__.py` & `Nuitka-2.1.6/tests/programs/case_imports1/path1/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/case_imports1/path2/some_module.py` & `Nuitka-2.1.6/tests/programs/case_imports1/path2/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/case_imports1/path2/some_package/__init__.py` & `Nuitka-2.1.6/tests/programs/case_imports1/path2/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/case_imports2/CasedImportingMain.py` & `Nuitka-2.1.6/tests/programs/case_imports2/CasedImportingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/case_imports2/path1/some_module.py` & `Nuitka-2.1.6/tests/programs/case_imports2/path1/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/case_imports2/path1/some_package/__init__.py` & `Nuitka-2.1.6/tests/programs/case_imports2/path1/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/case_imports2/path2/Some_Module.py` & `Nuitka-2.1.6/tests/programs/case_imports2/path2/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/case_imports2/path2/Some_Package/__init__.py` & `Nuitka-2.1.6/tests/programs/case_imports2/path2/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/case_imports3/CasedImportingMain.py` & `Nuitka-2.1.6/tests/programs/case_imports3/CasedImportingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/case_imports3/path1/Some_Module.py` & `Nuitka-2.1.6/tests/programs/case_imports3/path1/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/case_imports3/path1/Some_Package/__init__.py` & `Nuitka-2.1.6/tests/programs/case_imports3/path1/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/case_imports3/path2/Some_Module.py` & `Nuitka-2.1.6/tests/programs/case_imports3/path2/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/case_imports3/path2/Some_Package/__init__.py` & `Nuitka-2.1.6/tests/programs/case_imports3/path2/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/cyclic_imports/CyclicImportsMain.py` & `Nuitka-2.1.6/tests/programs/cyclic_imports/CyclicImportsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py` & `Nuitka-2.1.6/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py` & `Nuitka-2.1.6/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py` & `Nuitka-2.1.6/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/dash_import/DashImportMain.py` & `Nuitka-2.1.6/tests/programs/dash_import/DashImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/dash_import/dash-module.py` & `Nuitka-2.1.6/tests/programs/dash_import/dash-module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/dash_import/plus+module.py` & `Nuitka-2.1.6/tests/programs/dash_import/plus+module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/dash_main/Dash-Main.py` & `Nuitka-2.1.6/tests/programs/dash_main/Dash-Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/deep/DeepProgramMain.py` & `Nuitka-2.1.6/tests/programs/deep/DeepProgramMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/deep/some_package/DeepBrother.py` & `Nuitka-2.1.6/tests/programs/deep/some_package/DeepBrother.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/deep/some_package/DeepChild.py` & `Nuitka-2.1.6/tests/programs/deep/some_package/DeepChild.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/deep/some_package/__init__.py` & `Nuitka-2.1.6/tests/programs/deep/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/deep/some_package/deep_package/DeepDeepChild.py` & `Nuitka-2.1.6/tests/programs/deep/some_package/deep_package/DeepDeepChild.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/deep/some_package/deep_package/__init__.py` & `Nuitka-2.1.6/tests/programs/deep/some_package/deep_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/dunderinit_imports/DunderInitImportsMain.py` & `Nuitka-2.1.6/tests/programs/dunderinit_imports/DunderInitImportsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/dunderinit_imports/package/SubModule.py` & `Nuitka-2.1.6/tests/programs/dunderinit_imports/package/SubModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/dunderinit_imports/package/__init__.py` & `Nuitka-2.1.6/tests/programs/dunderinit_imports/package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/import_variants/ImportVariationsMain.py` & `Nuitka-2.1.6/tests/programs/import_variants/ImportVariationsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/import_variants/some_package/Child1.py` & `Nuitka-2.1.6/tests/programs/import_variants/some_package/Child1.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/import_variants/some_package/Child2.py` & `Nuitka-2.1.6/tests/programs/import_variants/some_package/Child2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/import_variants/some_package/Child3.py` & `Nuitka-2.1.6/tests/programs/import_variants/some_package/Child3.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/import_variants/some_package/__init__.py` & `Nuitka-2.1.6/tests/programs/import_variants/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/main_raises/ErrorMain.py` & `Nuitka-2.1.6/tests/programs/main_raises/ErrorMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/main_raises/ErrorRaising.py` & `Nuitka-2.1.6/tests/programs/main_raises/ErrorRaising.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/main_raises2/ErrorInFunctionMain.py` & `Nuitka-2.1.6/tests/programs/main_raises2/ErrorInFunctionMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/main_raises2/ErrorRaising.py` & `Nuitka-2.1.6/tests/programs/main_raises2/ErrorRaising.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/module_attributes/ModuleAttributesMain.py` & `Nuitka-2.1.6/tests/programs/module_attributes/ModuleAttributesMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/module_attributes/package_level1/Nearby1.py` & `Nuitka-2.1.6/tests/programs/module_attributes/package_level1/Nearby1.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/module_attributes/package_level1/__init__.py` & `Nuitka-2.1.6/tests/programs/module_attributes/package_level1/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py` & `Nuitka-2.1.6/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/module_attributes/package_level1/package_level2/__init__.py` & `Nuitka-2.1.6/tests/programs/module_attributes/package_level1/package_level2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py` & `Nuitka-2.1.6/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py` & `Nuitka-2.1.6/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/module_exits/ErrorExitingModule.py` & `Nuitka-2.1.6/tests/programs/module_exits/ErrorExitingModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/module_exits/Main.py` & `Nuitka-2.1.6/tests/programs/module_exits/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py` & `Nuitka-2.1.6/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/module_object_replacing/SelfReplacingModule.py` & `Nuitka-2.1.6/tests/programs/module_object_replacing/SelfReplacingModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py` & `Nuitka-2.1.6/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/multiprocessing_using/foo/__init__.py` & `Nuitka-2.1.6/tests/programs/multiprocessing_using/foo/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/multiprocessing_using/foo/__main__.py` & `Nuitka-2.1.6/tests/programs/multiprocessing_using/foo/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/multiprocessing_using/foo/entry.py` & `Nuitka-2.1.6/tests/programs/multiprocessing_using/foo/entry.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/named_imports/NamedImportsMain.py` & `Nuitka-2.1.6/tests/programs/named_imports/NamedImportsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/named_imports/some_package/SomeModule.py` & `Nuitka-2.1.6/tests/programs/named_imports/some_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/named_imports/some_package/__init__.py` & `Nuitka-2.1.6/tests/programs/named_imports/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/named_imports/some_package/sub_package/SomeModule.py` & `Nuitka-2.1.6/tests/programs/named_imports/some_package/sub_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/package_code/PackageInitCodeMain.py` & `Nuitka-2.1.6/tests/programs/package_code/PackageInitCodeMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/package_code/some_package/SomeModule.py` & `Nuitka-2.1.6/tests/programs/package_code/some_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/package_code/some_package/__init__.py` & `Nuitka-2.1.6/tests/programs/package_code/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/package_contains_main/PackageContainsMain.py` & `Nuitka-2.1.6/tests/programs/package_contains_main/PackageContainsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/package_contains_main/__init__.py` & `Nuitka-2.1.6/tests/programs/package_contains_main/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/package_contains_main/local.py` & `Nuitka-2.1.6/tests/programs/package_contains_main/local.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/package_init_import/PackageInitImportMain.py` & `Nuitka-2.1.6/tests/programs/package_init_import/PackageInitImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/package_init_import/some_package/PackageLocal.py` & `Nuitka-2.1.6/tests/programs/package_init_import/some_package/PackageLocal.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/package_init_import/some_package/__init__.py` & `Nuitka-2.1.6/tests/programs/package_init_import/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/package_init_issue/PackageInitIssueMain.py` & `Nuitka-2.1.6/tests/programs/package_init_issue/PackageInitIssueMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/package_init_issue/some_package/__init__.py` & `Nuitka-2.1.6/tests/programs/package_init_issue/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/package_init_issue/some_package/child_package/SomeModule.py` & `Nuitka-2.1.6/tests/programs/package_init_issue/some_package/child_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/package_init_issue/some_package/child_package/__init__.py` & `Nuitka-2.1.6/tests/programs/package_init_issue/some_package/child_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/package_missing_init/PackageMissingInitMain.py` & `Nuitka-2.1.6/tests/programs/package_missing_init/PackageMissingInitMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/package_missing_init/some_package/some_module.py` & `Nuitka-2.1.6/tests/programs/package_missing_init/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py` & `Nuitka-2.1.6/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py` & `Nuitka-2.1.6/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/package_module_collision/Something/__init__.py` & `Nuitka-2.1.6/tests/programs/package_module_collision/Something/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/package_module_collision/something.py` & `Nuitka-2.1.6/tests/programs/package_module_collision/something.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/package_overload/Main.py` & `Nuitka-2.1.6/tests/programs/package_overload/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/package_overload/foo/__init__.py` & `Nuitka-2.1.6/tests/programs/package_overload/foo/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/package_overload/foo/bar.py` & `Nuitka-2.1.6/tests/programs/package_overload/foo/bar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/package_overload/foo/bar2.py` & `Nuitka-2.1.6/tests/programs/package_overload/foo/bar2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py` & `Nuitka-2.1.6/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/package_prevents_submodule/some_package/__init__.py` & `Nuitka-2.1.6/tests/programs/package_prevents_submodule/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/package_prevents_submodule/some_package/some_module.py` & `Nuitka-2.1.6/tests/programs/package_prevents_submodule/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/package_program/PackageAsMain/__init__.py` & `Nuitka-2.1.6/tests/programs/package_program/PackageAsMain/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/package_program/PackageAsMain/__main__.py` & `Nuitka-2.1.6/tests/programs/package_program/PackageAsMain/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py` & `Nuitka-2.1.6/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/pkgutil_itermodules/some_package/__init__.py` & `Nuitka-2.1.6/tests/programs/pkgutil_itermodules/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py` & `Nuitka-2.1.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py` & `Nuitka-2.1.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py` & `Nuitka-2.1.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py` & `Nuitka-2.1.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py` & `Nuitka-2.1.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py` & `Nuitka-2.1.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/pkgutil_usage/PkgUtilUsageMain.py` & `Nuitka-2.1.6/tests/programs/pkgutil_usage/PkgUtilUsageMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/pkgutil_usage/package/__init__.py` & `Nuitka-2.1.6/tests/programs/pkgutil_usage/package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/plugin_import/PluginImportMain.py` & `Nuitka-2.1.6/tests/programs/plugin_import/PluginImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/plugin_import/some_package/__init__.py` & `Nuitka-2.1.6/tests/programs/plugin_import/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/plugin_import/some_package/some_module.py` & `Nuitka-2.1.6/tests/programs/plugin_import/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py` & `Nuitka-2.1.6/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/reimport_main_static/ImportItselfStaticMain.py` & `Nuitka-2.1.6/tests/programs/reimport_main_static/ImportItselfStaticMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/relative_import/RelativeImportMain.py` & `Nuitka-2.1.6/tests/programs/relative_import/RelativeImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/relative_import/dircache.py` & `Nuitka-2.1.6/tests/programs/relative_import/dircache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/resource_reader37/ResourceReaderMain.py` & `Nuitka-2.1.6/tests/programs/resource_reader37/ResourceReaderMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/resource_reader37/some_package/__init__.py` & `Nuitka-2.1.6/tests/programs/resource_reader37/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/run_all.py` & `Nuitka-2.1.6/tests/programs/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/stdlib_overload/StdlibOverloadMain.py` & `Nuitka-2.1.6/tests/programs/stdlib_overload/StdlibOverloadMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/stdlib_overload/pyexpat.py` & `Nuitka-2.1.6/tests/programs/stdlib_overload/pyexpat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/stdlib_overload/some_package/__init__.py` & `Nuitka-2.1.6/tests/programs/stdlib_overload/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/stdlib_overload/some_package/normal_importing.py` & `Nuitka-2.1.6/tests/programs/stdlib_overload/some_package/normal_importing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/stdlib_overload/some_package/pyexpat.py` & `Nuitka-2.1.6/tests/programs/stdlib_overload/some_package/pyexpat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/stdlib_overload/some_package/star_importing.py` & `Nuitka-2.1.6/tests/programs/stdlib_overload/some_package/star_importing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/syntax_errors/IndentationErroring.py` & `Nuitka-2.1.6/tests/programs/syntax_errors/IndentationErroring.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/syntax_errors/SyntaxErroring.py` & `Nuitka-2.1.6/tests/programs/syntax_errors/SyntaxErroring.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/syntax_errors/SyntaxErrorsMain.py` & `Nuitka-2.1.6/tests/programs/syntax_errors/SyntaxErrorsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/unicode_bom/UnicodeBomMain.py` & `Nuitka-2.1.6/tests/programs/unicode_bom/UnicodeBomMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/unicode_bom/unicode_bom.py` & `Nuitka-2.1.6/tests/programs/unicode_bom/unicode_bom.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/programs/with space/Space Main.py` & `Nuitka-2.1.6/tests/programs/with space/Space Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/reflected/compile_itself.py` & `Nuitka-2.1.6/tests/reflected/compile_itself.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/run-tests` & `Nuitka-2.1.6/tests/run-tests`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/BrotliUsing.py` & `Nuitka-2.1.6/tests/standalone/BrotliUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/CtypesUsing.py` & `Nuitka-2.1.6/tests/standalone/CtypesUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/DateutilsUsing.py` & `Nuitka-2.1.6/tests/standalone/DateutilsUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/FlaskUsing.py` & `Nuitka-2.1.6/tests/standalone/FlaskUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/GiUsing.py` & `Nuitka-2.1.6/tests/standalone/GiUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/GlfwUsing.py` & `Nuitka-2.1.6/tests/standalone/GlfwUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/GtkUsing.py` & `Nuitka-2.1.6/tests/standalone/GtkUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/HexEncodingTest_2.py` & `Nuitka-2.1.6/tests/standalone/HexEncodingTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/IdnaUsing.py` & `Nuitka-2.1.6/tests/standalone/IdnaUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/LxmlUsing.py` & `Nuitka-2.1.6/tests/standalone/LxmlUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/MatplotlibUsing.py` & `Nuitka-2.1.6/tests/standalone/MatplotlibUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/MetadataPackagesUsing.py` & `Nuitka-2.1.6/tests/standalone/MetadataPackagesUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/NumpyUsing.py` & `Nuitka-2.1.6/tests/standalone/NumpyUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/OpenGLUsing.py` & `Nuitka-2.1.6/tests/standalone/OpenGLUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/PandasUsing.py` & `Nuitka-2.1.6/tests/standalone/PandasUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/PasslibUsing.py` & `Nuitka-2.1.6/tests/standalone/PasslibUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/PendulumUsing.py` & `Nuitka-2.1.6/tests/standalone/PendulumUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/PkgResourcesRequiresUsing.py` & `Nuitka-2.1.6/tests/standalone/PkgResourcesRequiresUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/PmwUsing.py` & `Nuitka-2.1.6/tests/standalone/PmwUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/PyQt5Plugins.py` & `Nuitka-2.1.6/tests/standalone/PyQt5Plugins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/PyQt5SSLSupport.py` & `Nuitka-2.1.6/tests/standalone/PyQt5SSLSupport.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/PyQt5Using.py` & `Nuitka-2.1.6/tests/standalone/PyQt5Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/PyQt6Plugins.py` & `Nuitka-2.1.6/tests/standalone/PyQt6Plugins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/PyQt6Using.py` & `Nuitka-2.1.6/tests/standalone/PyQt6Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/PySide2Using.py` & `Nuitka-2.1.6/tests/standalone/PySide2Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/PySide6Plugins.py` & `Nuitka-2.1.6/tests/standalone/PySide6Plugins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/PySide6Using.py` & `Nuitka-2.1.6/tests/standalone/PySide6Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/RsaUsing.py` & `Nuitka-2.1.6/tests/standalone/RsaUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/SetuptoolsUsing.py` & `Nuitka-2.1.6/tests/standalone/SetuptoolsUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/ShlibUsing.py` & `Nuitka-2.1.6/tests/standalone/ShlibUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/SocketUsing.py` & `Nuitka-2.1.6/tests/standalone/SocketUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/TkInterUsing.py` & `Nuitka-2.1.6/tests/standalone/TkInterUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/Urllib3Using.py` & `Nuitka-2.1.6/tests/standalone/Urllib3Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/Win32ComUsing.py` & `Nuitka-2.1.6/tests/standalone/Win32ComUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/run_all.py` & `Nuitka-2.1.6/tests/standalone/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/standalone/zip_importer/ZipImporterMain.py` & `Nuitka-2.1.6/tests/standalone/zip_importer/ZipImporterMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/AsyncgenReturn36.py` & `Nuitka-2.1.6/tests/syntax/AsyncgenReturn36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/AwaitInModule36.py` & `Nuitka-2.1.6/tests/syntax/AwaitInModule36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/BreakWithoutLoop.py` & `Nuitka-2.1.6/tests/syntax/BreakWithoutLoop.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/ClassReturn.py` & `Nuitka-2.1.6/tests/syntax/ClassReturn.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/ClosureDel_2.py` & `Nuitka-2.1.6/tests/syntax/ClosureDel_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/ContinueWithoutLoop.py` & `Nuitka-2.1.6/tests/syntax/ContinueWithoutLoop.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/DuplicateArgument.py` & `Nuitka-2.1.6/tests/syntax/DuplicateArgument.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/ExecWithNesting_2.py` & `Nuitka-2.1.6/tests/syntax/ExecWithNesting_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/FutureBraces.py` & `Nuitka-2.1.6/tests/syntax/FutureBraces.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/FutureUnknown.py` & `Nuitka-2.1.6/tests/syntax/FutureUnknown.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/GeneratorExpressions38.py` & `Nuitka-2.1.6/tests/syntax/GeneratorExpressions38.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/GeneratorReturn_2.py` & `Nuitka-2.1.6/tests/syntax/GeneratorReturn_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/GlobalForParameter.py` & `Nuitka-2.1.6/tests/syntax/GlobalForParameter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/Importing32.py` & `Nuitka-2.1.6/tests/syntax/Importing32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/IndentationError.py` & `Nuitka-2.1.6/tests/syntax/IndentationError.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/LateFutureImport.py` & `Nuitka-2.1.6/tests/syntax/LateFutureImport.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/MisplacedFutureImport.py` & `Nuitka-2.1.6/tests/syntax/MisplacedFutureImport.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/ModuleReturn.py` & `Nuitka-2.1.6/tests/syntax/ModuleReturn.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/NonAsciiWithoutEncoding_2.py` & `Nuitka-2.1.6/tests/syntax/NonAsciiWithoutEncoding_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/NonlocalForParameter32.py` & `Nuitka-2.1.6/tests/syntax/NonlocalForParameter32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/NonlocalNotFound32.py` & `Nuitka-2.1.6/tests/syntax/NonlocalNotFound32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/StarImportExtra.py` & `Nuitka-2.1.6/tests/syntax/StarImportExtra.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/SyntaxError.py` & `Nuitka-2.1.6/tests/syntax/SyntaxError.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/TryExceptAllNotLast.py` & `Nuitka-2.1.6/tests/syntax/TryExceptAllNotLast.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/TryFinallyContinue_37.py` & `Nuitka-2.1.6/tests/syntax/TryFinallyContinue_37.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/UnpackNoTuple.py` & `Nuitka-2.1.6/tests/syntax/UnpackNoTuple.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/UnpackTwoStars32.py` & `Nuitka-2.1.6/tests/syntax/UnpackTwoStars32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/YieldFromInModule.py` & `Nuitka-2.1.6/tests/syntax/YieldFromInModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/YieldInAsync35.py` & `Nuitka-2.1.6/tests/syntax/YieldInAsync35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/YieldInGenexp38.py` & `Nuitka-2.1.6/tests/syntax/YieldInGenexp38.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/YieldInModule.py` & `Nuitka-2.1.6/tests/syntax/YieldInModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.1.5/tests/syntax/run_all.py` & `Nuitka-2.1.6/tests/syntax/run_all.py`

 * *Files identical despite different names*

