# Comparing `tmp/cclib-1.8.1rc2.tar.gz` & `tmp/cclib-2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cclib-1.8.1rc2.tar", last modified: Tue Mar 12 03:54:51 2024, max compression
+gzip compressed data, was "cclib-2.0a1.tar", last modified: Tue Apr 30 18:51:34 2024, max compression
```

## Comparing `cclib-1.8.1rc2.tar` & `cclib-2.0a1.tar`

### file list

```diff
@@ -1,101 +1,142 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 03:54:51.091768 cclib-1.8.1rc2/
--rw-r--r--   0 root         (0) root         (0)     2558 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/ANNOUNCE
--rw-r--r--   0 root         (0) root         (0)     1526 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       80 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4718 2024-03-12 03:54:51.091768 cclib-1.8.1rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1066 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/README.md
--rw-r--r--   0 root         (0) root         (0)     3238 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/THANKS
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 03:54:51.071768 cclib-1.8.1rc2/cclib/
--rw-r--r--   0 root         (0) root         (0)     1471 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/__init__.py
--rw-r--r--   0 root         (0) root         (0)       25 2024-03-12 03:54:50.000000 cclib-1.8.1rc2/cclib/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 03:54:51.075768 cclib-1.8.1rc2/cclib/bridge/
--rw-r--r--   0 root         (0) root         (0)      891 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/bridge/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8727 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/bridge/cclib2ase.py
--rw-r--r--   0 root         (0) root         (0)     1036 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/bridge/cclib2biopython.py
--rw-r--r--   0 root         (0) root         (0)     5076 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/bridge/cclib2horton.py
--rw-r--r--   0 root         (0) root         (0)     3410 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/bridge/cclib2openbabel.py
--rw-r--r--   0 root         (0) root         (0)      946 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/bridge/cclib2psi4.py
--rw-r--r--   0 root         (0) root         (0)     1419 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/bridge/cclib2pyquante.py
--rw-r--r--   0 root         (0) root         (0)     4115 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/bridge/cclib2pyscf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 03:54:51.079768 cclib-1.8.1rc2/cclib/io/
--rw-r--r--   0 root         (0) root         (0)      815 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15042 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/io/ccio.py
--rw-r--r--   0 root         (0) root         (0)     1918 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/io/cjsonreader.py
--rw-r--r--   0 root         (0) root         (0)     9878 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/io/cjsonwriter.py
--rw-r--r--   0 root         (0) root         (0)     3421 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/io/cmlwriter.py
--rw-r--r--   0 root         (0) root         (0)     1238 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/io/filereader.py
--rw-r--r--   0 root         (0) root         (0)     5924 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/io/filewriter.py
--rw-r--r--   0 root         (0) root         (0)    13326 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/io/moldenwriter.py
--rw-r--r--   0 root         (0) root         (0)    19059 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/io/wfxwriter.py
--rw-r--r--   0 root         (0) root         (0)     2435 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/io/xyzreader.py
--rw-r--r--   0 root         (0) root         (0)     4214 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/io/xyzwriter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 03:54:51.083768 cclib-1.8.1rc2/cclib/method/
--rw-r--r--   0 root         (0) root         (0)      995 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/method/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9292 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/method/bader.py
--rw-r--r--   0 root         (0) root         (0)     5293 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/method/bickelhaupt.py
--rw-r--r--   0 root         (0) root         (0)     2338 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/method/calculationmethod.py
--rw-r--r--   0 root         (0) root         (0)     4818 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/method/cda.py
--rw-r--r--   0 root         (0) root         (0)     9997 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/method/cm5.py
--rw-r--r--   0 root         (0) root         (0)     3410 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/method/cspa.py
--rw-r--r--   0 root         (0) root         (0)    38725 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/method/ddec.py
--rw-r--r--   0 root         (0) root         (0)     2716 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/method/density.py
--rw-r--r--   0 root         (0) root         (0)     1410 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/method/electrons.py
--rw-r--r--   0 root         (0) root         (0)     5321 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/method/fragments.py
--rw-r--r--   0 root         (0) root         (0)     4614 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/method/hirshfeld.py
--rw-r--r--   0 root         (0) root         (0)     4208 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/method/lpa.py
--rw-r--r--   0 root         (0) root         (0)     3923 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/method/mbo.py
--rw-r--r--   0 root         (0) root         (0)     5540 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/method/moments.py
--rw-r--r--   0 root         (0) root         (0)     3798 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/method/mpa.py
--rw-r--r--   0 root         (0) root         (0)     7302 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/method/nuclear.py
--rw-r--r--   0 root         (0) root         (0)     4041 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/method/opa.py
--rw-r--r--   0 root         (0) root         (0)     1679 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/method/orbitals.py
--rw-r--r--   0 root         (0) root         (0)     3453 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/method/population.py
--rw-r--r--   0 root         (0) root         (0)     9624 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/method/stockholder.py
--rw-r--r--   0 root         (0) root         (0)    15869 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/method/volume.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 03:54:51.087768 cclib-1.8.1rc2/cclib/parser/
--rw-r--r--   0 root         (0) root         (0)     1420 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54145 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/parser/adfparser.py
--rw-r--r--   0 root         (0) root         (0)    61963 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/parser/daltonparser.py
--rw-r--r--   0 root         (0) root         (0)    23134 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/parser/data.py
--rw-r--r--   0 root         (0) root         (0)    15487 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/parser/fchkparser.py
--rw-r--r--   0 root         (0) root         (0)     9952 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/parser/gamessdatparser.py
--rw-r--r--   0 root         (0) root         (0)    77208 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/parser/gamessparser.py
--rw-r--r--   0 root         (0) root         (0)    31670 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/parser/gamessukparser.py
--rw-r--r--   0 root         (0) root         (0)   121489 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/parser/gaussianparser.py
--rw-r--r--   0 root         (0) root         (0)    32476 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/parser/jaguarparser.py
--rw-r--r--   0 root         (0) root         (0)    16842 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/parser/logfileparser.py
--rw-r--r--   0 root         (0) root         (0)    10097 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/parser/logfilewrapper.py
--rw-r--r--   0 root         (0) root         (0)    48354 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/parser/molcasparser.py
--rw-r--r--   0 root         (0) root         (0)    43886 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/parser/molproparser.py
--rw-r--r--   0 root         (0) root         (0)     9751 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/parser/mopacparser.py
--rw-r--r--   0 root         (0) root         (0)    12859 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/parser/nboparser.py
--rw-r--r--   0 root         (0) root         (0)    67600 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/parser/nwchemparser.py
--rw-r--r--   0 root         (0) root         (0)   131390 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/parser/orcaparser.py
--rw-r--r--   0 root         (0) root         (0)    13838 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/parser/psi3parser.py
--rw-r--r--   0 root         (0) root         (0)    57028 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/parser/psi4parser.py
--rw-r--r--   0 root         (0) root         (0)    87750 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/parser/qchemparser.py
--rw-r--r--   0 root         (0) root         (0)    88348 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/parser/turbomoleparser.py
--rw-r--r--   0 root         (0) root         (0)     9743 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/parser/utils.py
--rw-r--r--   0 root         (0) root         (0)    33241 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/parser/xtbparser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 03:54:51.087768 cclib-1.8.1rc2/cclib/progress/
--rw-r--r--   0 root         (0) root         (0)      262 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/progress/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1424 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/progress/textprogress.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 03:54:51.087768 cclib-1.8.1rc2/cclib/scripts/
--rw-r--r--   0 root         (0) root         (0)      215 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/scripts/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2898 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/scripts/ccframe.py
--rw-r--r--   0 root         (0) root         (0)     7790 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/scripts/ccget.py
--rwxr-xr-x   0 root         (0) root         (0)     3705 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/scripts/ccwrite.py
--rw-r--r--   0 root         (0) root         (0)     1966 2024-03-12 03:51:29.000000 cclib-1.8.1rc2/cclib/scripts/cda.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 03:54:51.087768 cclib-1.8.1rc2/cclib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4718 2024-03-12 03:54:51.000000 cclib-1.8.1rc2/cclib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2194 2024-03-12 03:54:51.000000 cclib-1.8.1rc2/cclib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-12 03:54:51.000000 cclib-1.8.1rc2/cclib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      155 2024-03-12 03:54:51.000000 cclib-1.8.1rc2/cclib.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-12 03:51:33.000000 cclib-1.8.1rc2/cclib.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      243 2024-03-12 03:54:51.000000 cclib-1.8.1rc2/cclib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-03-12 03:54:51.000000 cclib-1.8.1rc2/cclib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     4264 2024-03-12 03:51:30.000000 cclib-1.8.1rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-12 03:54:51.091768 cclib-1.8.1rc2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 03:54:51.087768 cclib-1.8.1rc2/tools/
--rw-r--r--   0 root         (0) root         (0)     2274 2024-03-12 03:51:30.000000 cclib-1.8.1rc2/tools/versioningit_override.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:51:34.306783 cclib-2.0a1/
+-rw-r--r--   0 root         (0) root         (0)     2558 2024-04-30 18:50:56.000000 cclib-2.0a1/ANNOUNCE
+-rw-r--r--   0 root         (0) root         (0)     1526 2024-04-30 18:50:56.000000 cclib-2.0a1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       80 2024-04-30 18:50:56.000000 cclib-2.0a1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4705 2024-04-30 18:51:34.306783 cclib-2.0a1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1056 2024-04-30 18:50:56.000000 cclib-2.0a1/README.md
+-rw-r--r--   0 root         (0) root         (0)     3238 2024-04-30 18:50:56.000000 cclib-2.0a1/THANKS
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:51:34.278782 cclib-2.0a1/cclib/
+-rw-r--r--   0 root         (0) root         (0)     1670 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-30 18:51:34.000000 cclib-2.0a1/cclib/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:51:34.286783 cclib-2.0a1/cclib/attribute_parsers/
+-rw-r--r--   0 root         (0) root         (0)     1351 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/attribute_parsers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2322 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/attribute_parsers/aooverlaps.py
+-rw-r--r--   0 root         (0) root         (0)     8231 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/attribute_parsers/atombasis.py
+-rw-r--r--   0 root         (0) root         (0)    10448 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/attribute_parsers/atomcharges.py
+-rw-r--r--   0 root         (0) root         (0)     3975 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/attribute_parsers/atomcoords.py
+-rw-r--r--   0 root         (0) root         (0)     2606 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/attribute_parsers/atommasses.py
+-rw-r--r--   0 root         (0) root         (0)     3684 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/attribute_parsers/atomnos.py
+-rw-r--r--   0 root         (0) root         (0)      558 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/attribute_parsers/base_parser.py
+-rw-r--r--   0 root         (0) root         (0)     2870 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/attribute_parsers/charge.py
+-rw-r--r--   0 root         (0) root         (0)     3423 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/attribute_parsers/coreelectrons.py
+-rw-r--r--   0 root         (0) root         (0)    18564 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/attribute_parsers/data.py
+-rw-r--r--   0 root         (0) root         (0)    14040 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/attribute_parsers/gbasis.py
+-rw-r--r--   0 root         (0) root         (0)     2592 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/attribute_parsers/mocoeffs.py
+-rw-r--r--   0 root         (0) root         (0)     2467 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/attribute_parsers/moenergies.py
+-rw-r--r--   0 root         (0) root         (0)     9181 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/attribute_parsers/mosyms.py
+-rw-r--r--   0 root         (0) root         (0)     2581 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/attribute_parsers/mult.py
+-rw-r--r--   0 root         (0) root         (0)     2255 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/attribute_parsers/natom.py
+-rw-r--r--   0 root         (0) root         (0)     3206 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/attribute_parsers/nbasis.py
+-rw-r--r--   0 root         (0) root         (0)     1854 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/attribute_parsers/nmo.py
+-rw-r--r--   0 root         (0) root         (0)     2144 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/attribute_parsers/scfenergies.py
+-rw-r--r--   0 root         (0) root         (0)     2680 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/attribute_parsers/scftargets.py
+-rw-r--r--   0 root         (0) root         (0)     2660 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/attribute_parsers/scfvalues.py
+-rw-r--r--   0 root         (0) root         (0)     9743 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/attribute_parsers/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:51:34.286783 cclib-2.0a1/cclib/attributes/
+-rw-r--r--   0 root         (0) root         (0)      198 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/attributes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28060 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/attributes/attribute.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:51:34.286783 cclib-2.0a1/cclib/bridge/
+-rw-r--r--   0 root         (0) root         (0)      891 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/bridge/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8727 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/bridge/cclib2ase.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/bridge/cclib2biopython.py
+-rw-r--r--   0 root         (0) root         (0)     5076 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/bridge/cclib2horton.py
+-rw-r--r--   0 root         (0) root         (0)     3410 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/bridge/cclib2openbabel.py
+-rw-r--r--   0 root         (0) root         (0)      946 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/bridge/cclib2psi4.py
+-rw-r--r--   0 root         (0) root         (0)     1419 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/bridge/cclib2pyquante.py
+-rw-r--r--   0 root         (0) root         (0)     4115 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/bridge/cclib2pyscf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:51:34.286783 cclib-2.0a1/cclib/collection/
+-rw-r--r--   0 root         (0) root         (0)      282 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/collection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1269 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/collection/collection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:51:34.286783 cclib-2.0a1/cclib/combinator/
+-rw-r--r--   0 root         (0) root         (0)      239 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/combinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      952 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/combinator/combinator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:51:34.290783 cclib-2.0a1/cclib/driver/
+-rw-r--r--   0 root         (0) root         (0)      330 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/driver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21808 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/driver/ccdriver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:51:34.290783 cclib-2.0a1/cclib/file_handler/
+-rw-r--r--   0 root         (0) root         (0)      343 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/file_handler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14630 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/file_handler/file_handler.py
+-rw-r--r--   0 root         (0) root         (0)     9743 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/file_handler/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:51:34.290783 cclib-2.0a1/cclib/io/
+-rw-r--r--   0 root         (0) root         (0)      968 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11516 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/io/ccio.py
+-rw-r--r--   0 root         (0) root         (0)     1918 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/io/cjsonreader.py
+-rw-r--r--   0 root         (0) root         (0)     9880 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/io/cjsonwriter.py
+-rw-r--r--   0 root         (0) root         (0)     3421 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/io/cmlwriter.py
+-rw-r--r--   0 root         (0) root         (0)     1238 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/io/filereader.py
+-rw-r--r--   0 root         (0) root         (0)     5924 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/io/filewriter.py
+-rw-r--r--   0 root         (0) root         (0)    13291 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/io/moldenwriter.py
+-rw-r--r--   0 root         (0) root         (0)    19059 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/io/wfxwriter.py
+-rw-r--r--   0 root         (0) root         (0)     2435 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/io/xyzreader.py
+-rw-r--r--   0 root         (0) root         (0)     4214 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/io/xyzwriter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:51:34.294782 cclib-2.0a1/cclib/method/
+-rw-r--r--   0 root         (0) root         (0)      995 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/method/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9214 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/method/bader.py
+-rw-r--r--   0 root         (0) root         (0)     5293 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/method/bickelhaupt.py
+-rw-r--r--   0 root         (0) root         (0)     2338 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/method/calculationmethod.py
+-rw-r--r--   0 root         (0) root         (0)     4818 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/method/cda.py
+-rw-r--r--   0 root         (0) root         (0)     9997 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/method/cm5.py
+-rw-r--r--   0 root         (0) root         (0)     3410 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/method/cspa.py
+-rw-r--r--   0 root         (0) root         (0)    38527 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/method/ddec.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/method/density.py
+-rw-r--r--   0 root         (0) root         (0)     1410 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/method/electrons.py
+-rw-r--r--   0 root         (0) root         (0)     5321 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/method/fragments.py
+-rw-r--r--   0 root         (0) root         (0)     4615 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/method/hirshfeld.py
+-rw-r--r--   0 root         (0) root         (0)     4208 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/method/lpa.py
+-rw-r--r--   0 root         (0) root         (0)     3923 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/method/mbo.py
+-rw-r--r--   0 root         (0) root         (0)     5540 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/method/moments.py
+-rw-r--r--   0 root         (0) root         (0)     3798 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/method/mpa.py
+-rw-r--r--   0 root         (0) root         (0)     7302 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/method/nuclear.py
+-rw-r--r--   0 root         (0) root         (0)     4041 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/method/opa.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/method/orbitals.py
+-rw-r--r--   0 root         (0) root         (0)     3453 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/method/population.py
+-rw-r--r--   0 root         (0) root         (0)     9624 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/method/stockholder.py
+-rw-r--r--   0 root         (0) root         (0)    15919 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/method/volume.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:51:34.302783 cclib-2.0a1/cclib/parser/
+-rw-r--r--   0 root         (0) root         (0)      553 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54145 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/parser/adfparser.py
+-rw-r--r--   0 root         (0) root         (0)    61962 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/parser/daltonparser.py
+-rw-r--r--   0 root         (0) root         (0)    15486 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/parser/fchkparser.py
+-rw-r--r--   0 root         (0) root         (0)     9951 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/parser/gamessdatparser.py
+-rw-r--r--   0 root         (0) root         (0)    77207 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/parser/gamessparser.py
+-rw-r--r--   0 root         (0) root         (0)    31669 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/parser/gamessukparser.py
+-rw-r--r--   0 root         (0) root         (0)   121634 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/parser/gaussianparser.py
+-rw-r--r--   0 root         (0) root         (0)    32475 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/parser/jaguarparser.py
+-rw-r--r--   0 root         (0) root         (0)    16842 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/parser/logfileparser.py
+-rw-r--r--   0 root         (0) root         (0)    48360 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/parser/molcasparser.py
+-rw-r--r--   0 root         (0) root         (0)    43885 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/parser/molproparser.py
+-rw-r--r--   0 root         (0) root         (0)     9751 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/parser/mopacparser.py
+-rw-r--r--   0 root         (0) root         (0)    12858 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/parser/nboparser.py
+-rw-r--r--   0 root         (0) root         (0)    67601 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/parser/nwchemparser.py
+-rw-r--r--   0 root         (0) root         (0)   131937 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/parser/orcaparser.py
+-rw-r--r--   0 root         (0) root         (0)    13838 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/parser/psi3parser.py
+-rw-r--r--   0 root         (0) root         (0)    56929 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/parser/psi4parser.py
+-rw-r--r--   0 root         (0) root         (0)    87666 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/parser/qchemparser.py
+-rw-r--r--   0 root         (0) root         (0)    88348 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/parser/turbomoleparser.py
+-rw-r--r--   0 root         (0) root         (0)     9743 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/parser/utils.py
+-rw-r--r--   0 root         (0) root         (0)    33241 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/parser/xtbparser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:51:34.302783 cclib-2.0a1/cclib/progress/
+-rw-r--r--   0 root         (0) root         (0)      262 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/progress/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1424 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/progress/textprogress.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:51:34.302783 cclib-2.0a1/cclib/scripts/
+-rw-r--r--   0 root         (0) root         (0)      215 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/scripts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/scripts/ccframe.py
+-rw-r--r--   0 root         (0) root         (0)     7789 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/scripts/ccget.py
+-rwxr-xr-x   0 root         (0) root         (0)     3705 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/scripts/ccwrite.py
+-rw-r--r--   0 root         (0) root         (0)     1966 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/scripts/cda.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:51:34.302783 cclib-2.0a1/cclib/tree/
+-rw-r--r--   0 root         (0) root         (0)      214 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/tree/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2649 2024-04-30 18:50:56.000000 cclib-2.0a1/cclib/tree/tree.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:51:34.302783 cclib-2.0a1/cclib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4705 2024-04-30 18:51:34.000000 cclib-2.0a1/cclib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3333 2024-04-30 18:51:34.000000 cclib-2.0a1/cclib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 18:51:34.000000 cclib-2.0a1/cclib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      155 2024-04-30 18:51:34.000000 cclib-2.0a1/cclib.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 18:50:59.000000 cclib-2.0a1/cclib.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      243 2024-04-30 18:51:34.000000 cclib-2.0a1/cclib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-30 18:51:34.000000 cclib-2.0a1/cclib.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     4264 2024-04-30 18:50:56.000000 cclib-2.0a1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 18:51:34.306783 cclib-2.0a1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:51:34.302783 cclib-2.0a1/tools/
+-rw-r--r--   0 root         (0) root         (0)     2274 2024-04-30 18:50:57.000000 cclib-2.0a1/tools/versioningit_override.py
```

### Comparing `cclib-1.8.1rc2/ANNOUNCE` & `cclib-2.0a1/ANNOUNCE`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/LICENSE` & `cclib-2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/PKG-INFO` & `cclib-2.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cclib
-Version: 1.8.1rc2
+Version: 2.0a1
 Summary: parsers and algorithms for computational chemistry
 Author-email: cclib development team <cclib@googlegroups.com>
 Maintainer-email: cclib development team <cclib@googlegroups.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, the cclib development team
         All rights reserved.
@@ -75,15 +75,15 @@
 Requires-Dist: cclib[bridges]; extra == "all"
 
 ### cclib
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8280878.svg)](https://doi.org/10.5281/zenodo.8280878)
 [![PyPI version](http://img.shields.io/pypi/v/cclib.svg?style=flat)](https://pypi.python.org/pypi/cclib)
 [![GitHub release](https://img.shields.io/github/release/cclib/cclib.svg?style=flat)](https://github.com/cclib/cclib/releases)
-[![build status](https://github.com/cclib/cclib/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/cclib/cclib/actions/workflows/cclib_pytest.yml)
+[![build status](https://github.com/cclib/cclib/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/cclib/cclib/actions/workflows/ci.yml)
 [![license](http://img.shields.io/badge/license-BSD-blue.svg?style=flat)](https://github.com/cclib/cclib/blob/master/LICENSE)
 
 <img src="./logo.png" alt="cclib logo" width="100" />
 
 cclib is a Python library that provides parsers for output files of computational chemistry packages. It also provides a platform for computational chemists to implement algorithms in a platform-independent way.
 
 For more information, go to [https://cclib.github.io](https://cclib.github.io). There is a mailing list for questions at https://groups.google.com/g/cclib.
```

### Comparing `cclib-1.8.1rc2/README.md` & `cclib-2.0a1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ### cclib
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8280878.svg)](https://doi.org/10.5281/zenodo.8280878)
 [![PyPI version](http://img.shields.io/pypi/v/cclib.svg?style=flat)](https://pypi.python.org/pypi/cclib)
 [![GitHub release](https://img.shields.io/github/release/cclib/cclib.svg?style=flat)](https://github.com/cclib/cclib/releases)
-[![build status](https://github.com/cclib/cclib/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/cclib/cclib/actions/workflows/cclib_pytest.yml)
+[![build status](https://github.com/cclib/cclib/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/cclib/cclib/actions/workflows/ci.yml)
 [![license](http://img.shields.io/badge/license-BSD-blue.svg?style=flat)](https://github.com/cclib/cclib/blob/master/LICENSE)
 
 <img src="./logo.png" alt="cclib logo" width="100" />
 
 cclib is a Python library that provides parsers for output files of computational chemistry packages. It also provides a platform for computational chemists to implement algorithms in a platform-independent way.
 
 For more information, go to [https://cclib.github.io](https://cclib.github.io). There is a mailing list for questions at https://groups.google.com/g/cclib.
```

### Comparing `cclib-1.8.1rc2/THANKS` & `cclib-2.0a1/THANKS`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/__init__.py` & `cclib-2.0a1/cclib/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,21 +16,33 @@
 To this end, cclib provides a number of bridges to help transfer data to other libraries
 as well as example methods that take parsed data as input.
 """
 
 from cclib._version import __version__
 
 # isort: off
-from cclib import parser, progress, method, bridge, io
+# from cclib import parser, progress, method, bridge
+from cclib import (
+    io,
+    file_handler,
+    collection,
+    combinator,
+    driver,
+    attributes,
+    attribute_parsers,
+    tree,
+)
 # isort: on
 
 # The test module can be imported if it was installed with cclib.
-try:
-    from cclib import test
-except ImportError:
-    pass
+# todo try:
+# todo     from cclib import test
+# todo except ImportError:
+# todo     pass
 
 # The objects below constitute our public API. These names will not change
 # over time. Names in the sub-modules will typically also be backwards
 # compatible, but may sometimes change when code is moved around.
-ccopen = io.ccopen
-ccwrite = io.ccwrite
+# ccopen = io.ccopen
+# ccwrite = io.ccwrite
+
+ccDriver = driver.ccDriver
```

### Comparing `cclib-1.8.1rc2/cclib/bridge/__init__.py` & `cclib-2.0a1/cclib/bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/bridge/cclib2ase.py` & `cclib-2.0a1/cclib/bridge/cclib2ase.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/bridge/cclib2biopython.py` & `cclib-2.0a1/cclib/bridge/cclib2biopython.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/bridge/cclib2horton.py` & `cclib-2.0a1/cclib/bridge/cclib2horton.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/bridge/cclib2openbabel.py` & `cclib-2.0a1/cclib/bridge/cclib2openbabel.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/bridge/cclib2psi4.py` & `cclib-2.0a1/cclib/bridge/cclib2psi4.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/bridge/cclib2pyquante.py` & `cclib-2.0a1/cclib/bridge/cclib2pyquante.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/bridge/cclib2pyscf.py` & `cclib-2.0a1/cclib/bridge/cclib2pyscf.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/io/ccio.py` & `cclib-2.0a1/cclib/io/ccio.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,437 +8,332 @@
 import logging
 import os
 import pathlib
 import typing
 import warnings
 from typing import Optional, Union
 
-from cclib.io import (
-    cjsonreader,
-    cjsonwriter,
-    cmlwriter,
-    moldenwriter,
-    wfxwriter,
-    xyzreader,
-    xyzwriter,
-)
-from cclib.parser import data, logfileparser
-from cclib.parser.adfparser import ADF
-from cclib.parser.daltonparser import DALTON
-from cclib.parser.fchkparser import FChk
-from cclib.parser.gamessdatparser import GAMESSDAT
-from cclib.parser.gamessparser import GAMESS
-from cclib.parser.gamessukparser import GAMESSUK
-from cclib.parser.gaussianparser import Gaussian
-from cclib.parser.jaguarparser import Jaguar
-from cclib.parser.logfilewrapper import FileWrapper
-from cclib.parser.molcasparser import Molcas
-from cclib.parser.molproparser import Molpro
-from cclib.parser.mopacparser import MOPAC
-from cclib.parser.nboparser import NBO
-from cclib.parser.nwchemparser import NWChem
-from cclib.parser.orcaparser import ORCA
-from cclib.parser.psi3parser import Psi3
-from cclib.parser.psi4parser import Psi4
-from cclib.parser.qchemparser import QChem
-from cclib.parser.turbomoleparser import Turbomole
-from cclib.parser.utils import find_package
-from cclib.parser.xtbparser import XTB
-
-_has_cclib2openbabel = find_package("openbabel")
-if _has_cclib2openbabel:
-    from cclib.bridge import cclib2openbabel
-
-_has_pandas = find_package("pandas")
-if _has_pandas:
-    import pandas as pd
+# from cclib.io import (
+#    cjsonreader,
+#    cjsonwriter,
+#    cmlwriter,
+#    moldenwriter,
+#    wfxwriter,
+#    xyzreader,
+#    xyzwriter,
+# )
+# from cclib.parser import data, logfileparser
+from cclib.driver import ccDriver
+from cclib.file_handler import FileHandler
+
+# _has_cclib2openbabel = find_package("openbabel")
+# if _has_cclib2openbabel:
+#    from cclib.bridge import cclib2openbabel
+
+# _has_pandas = find_package("pandas")
+# if _has_pandas:
+#    import pandas as pd
 
 # Parser choice is triggered by certain phrases occurring the logfile. Where these
 # strings are unique, we can set the parser and break. In other cases, the situation
 # is a little but more complicated. Here are the exceptions:
 #   1. The GAMESS trigger also works for GAMESS-UK files, so we can't break
 #      after finding GAMESS in case the more specific phrase is found.
 #   2. Molpro log files don't have the program header, but always contain
 #      the generic string 1PROGRAM, so don't break here either to be cautious.
 #   3. "MOPAC" is used in some packages like GAMESS, so match MOPAC20##
 #
 # The triggers are defined by the tuples in the list below like so:
 #   (parser, phrases, flag whether we should break)
-triggers = [
-    (ADF, ["Amsterdam Density Functional"], True),
-    (DALTON, ["Dalton - An Electronic Structure Program"], True),
-    (FChk, ["Number of atoms", "I"], True),
-    (GAMESS, ["GAMESS"], False),
-    (GAMESS, ["Firefly (PC GAMESS)"], True),
-    (GAMESS, ["GAMESS VERSION"], True),
-    (GAMESSUK, ["G A M E S S - U K"], True),
-    (GAMESSDAT, ["$DATA"], True),
-    (Gaussian, ["Gaussian, Inc."], True),
-    (Jaguar, ["Jaguar"], True),
-    (Molcas, ["MOLCAS"], True),
-    (Molpro, ["PROGRAM SYSTEM MOLPRO"], True),
-    (Molpro, ["1PROGRAM"], False),
-    (MOPAC, ["MOPAC20"], True),
-    (NBO, ["N A T U R A L   A T O M I C   O R B I T A L   A N D"], True),
-    (NWChem, ["Northwest Computational Chemistry Package"], True),
-    (ORCA, ["O   R   C   A"], True),
-    (Psi3, ["PSI3: An Open-Source Ab Initio Electronic Structure Package"], True),
-    (Psi4, ["Psi4: An Open-Source Ab Initio Electronic Structure Package"], True),
-    (QChem, ["A Quantum Leap Into The Future Of Chemistry"], True),
-    (Turbomole, ["TURBOMOLE"], True),
-    (XTB, ["x T B"], True),
-]
-
-readerclasses = {"cjson": cjsonreader.CJSON, "json": cjsonreader.CJSON, "xyz": xyzreader.XYZ}
-
-writerclasses = {
-    "cjson": cjsonwriter.CJSON,
-    "json": cjsonwriter.CJSON,
-    "cml": cmlwriter.CML,
-    "molden": moldenwriter.MOLDEN,
-    "wfx": wfxwriter.WFXWriter,
-    "xyz": xyzwriter.XYZ,
-}
 
+# readerclasses = {"cjson": cjsonreader.CJSON, "json": cjsonreader.CJSON, "xyz": xyzreader.XYZ}
 
-class UnknownOutputFormatError(Exception):
-    """Raised when an unknown output format is encountered."""
+# writerclasses = {
+#     "cjson": cjsonwriter.CJSON,
+#     "json": cjsonwriter.CJSON,
+#     "cml": cmlwriter.CML,
+#     "molden": moldenwriter.MOLDEN,
+#     "wfx": wfxwriter.WFXWriter,
+#     "xyz": xyzwriter.XYZ,
+# }
 
 
-def is_xyz(inputfile: FileWrapper) -> bool:
-    """Is the given inputfile actually an XYZ file?
-
-    The only way to determine this without reading the entire file is to
-    inspect the file extension.
-    """
-    return (
-        len(inputfile.filenames) == 1
-        and os.path.splitext(inputfile.filenames[0])[1].lower() == ".xyz"
-    )
-
-
-def guess_filetype(inputfile) -> Optional[logfileparser.Logfile]:
-    """Try to guess the filetype by searching for trigger strings."""
-    filetype = None
-    logger = logging.getLogger("cclib")
-    try:
-        if isinstance(inputfile, FileWrapper) and is_xyz(inputfile):
-            logger.info("Found XYZ file based on file extension")
-            return filetype
-        for line in inputfile:
-            for parser, phrases, do_break in triggers:
-                if all([line.lower().find(p.lower()) >= 0 for p in phrases]):
-                    filetype = parser
-                    if do_break:
-                        return filetype
-    except Exception:
-        # guess_filetype() is expected to be quiet by default...
-        logger.error("Failed to determine log file type", exc_info=True)
-
-    return filetype
-
+class UnknownOutputFormatError(Exception):
+    """Raised when an unknown output format is encountered."""
 
-def sort_turbomole_outputs(fileinputs):
-    """
-    Sorts a list of inputs (or list of log files) according to the order
-    required by the Turbomole parser for correct parsing. Unrecognised
-    files are appended to the end of the list in the same order they are
-    given.
 
-    This function has been deprecated as of version 1.8; use:
-    cclib.parser.turbomoleparser.Turbomole.sort_input() instead
+# def is_xyz(inputfile: FileWrapper) -> bool:
+#     """Is the given inputfile actually an XYZ file?
 
-    Inputs:
-      filelist - a list of Turbomole log files needed to be parsed.
-    Returns:
-      sorted_list - a sorted list of Turbomole files needed for proper parsing.
-    """
-    warnings.warn(
-        "sort_turbomole_outputs() has been deprecated as of v1.8; use: "
-        + "cclib.parser.turbomoleparser.Turbomole.sort_input() instead"
-    )
-    return Turbomole.sort_input(fileinputs)
+#     The only way to determine this without reading the entire file is to
+#     inspect the file extension.
+#     """
+#     return (
+#         len(inputfile.filenames) == 1
+#         and os.path.splitext(inputfile.filenames[0])[1].lower() == ".xyz"
+#     )
+
+
+# def guess_filetype(inputfile) -> Optional[logfileparser.Logfile]:
+#     """Try to guess the filetype by searching for trigger strings."""
+#     filetype = None
+#     logger = logging.getLogger("cclib")
+#     try:
+#         if isinstance(inputfile, FileWrapper) and is_xyz(inputfile):
+#             logger.info("Found XYZ file based on file extension")
+#             return filetype
+#         for line in inputfile:
+#             for parser, phrases, do_break in triggers:
+#                 if all([line.lower().find(p.lower()) >= 0 for p in phrases]):
+#                     filetype = parser
+#                     if do_break:
+#                         return filetype
+#     except Exception:
+#         # guess_filetype() is expected to be quiet by default...
+#         logger.error("Failed to determine log file type", exc_info=True)
+
+#     return filetype
+
+
+# def sort_turbomole_outputs(fileinputs):
+#     """
+#     Sorts a list of inputs (or list of log files) according to the order
+#     required by the Turbomole parser for correct parsing. Unrecognised
+#     files are appended to the end of the list in the same order they are
+#     given.
+
+#     This function has been deprecated as of version 1.8; use:
+#     cclib.parser.turbomoleparser.Turbomole.sort_input() instead
+
+#     Inputs:
+#       filelist - a list of Turbomole log files needed to be parsed.
+#     Returns:
+#       sorted_list - a sorted list of Turbomole files needed for proper parsing.
+#     """
+#     warnings.warn(
+#         "sort_turbomole_outputs() has been deprecated as of v1.8; use: "
+#         + "cclib.parser.turbomoleparser.Turbomole.sort_input() instead"
+#     )
+#     return Turbomole.sort_input(fileinputs)
 
 
 def ccread(
-    source: Union[str, typing.IO, FileWrapper, typing.List[Union[str, typing.IO]]], *args, **kwargs
+    source: Union[str, typing.IO, FileHandler, typing.List[Union[str, typing.IO]]], *args, **kwargs
 ):
     """Attempt to open and read computational chemistry data from a file.
 
     If the file is not appropriate for cclib parsers, a fallback mechanism
     will try to recognize some common chemistry formats and read those using
     the appropriate bridge such as Open Babel.
 
     Inputs:
         source - a single logfile, a list of logfiles (for a single job),
                  an input stream, or an URL pointing to a log file.
         *args, **kwargs - arguments and keyword arguments passed to ccopen
     Returns:
         a ccData object containing cclib data attributes
     """
-    log = None
-    try:
-        log = ccopen(source, *args, **kwargs)
-        logger = logging.getLogger("cclib")
-        if log:
-            logger.info("Identified logfile to be in {} format".format(type(log).__name__))
-
-            return log.parse()
-        else:
-            logger.info("Attempting to use fallback mechanism to read file")
-            return fallback(source)
-
-    finally:
-        if log:
-            log.inputfile.close()
+    if not isinstance(source, list):
+        source = [source]
+
+    a = ccDriver(source)
+    a.process_combinator()
+    return a._ccCollection
 
 
 def ccopen(
-    source: Union[str, typing.IO, FileWrapper, typing.List[Union[str, typing.IO]]],
+    source: Union[str, typing.IO, FileHandler, typing.List[Union[str, typing.IO]]],
     *args,
     quiet: bool = False,
     cjson: bool = False,
     **kwargs,
 ):
     """Guess the identity of a particular log file and return an instance of it.
 
     Inputs:
         source - a single logfile, a list of logfiles (for a single job),
                  an input stream, or an URL pointing to a log file.
         *args, **kwargs - arguments and keyword arguments passed to filetype
 
     Returns:
-      one of ADF, DALTON, GAMESS, GAMESS UK, Gaussian, Jaguar,
-      Molpro, MOPAC, NWChem, ORCA, Psi3, Psi/Psi4, QChem, CJSON or None
-      (if it cannot figure it out or the file does not exist).
+        ccCollection: by default a single point combinator, eventually dynamically determined.
     """
     if not isinstance(source, list):
         source = [source]
 
-    inputfile = None
-
-    logger = logging.getLogger("cclib")
-
-    try:
-        # Wrap our input with custom file object.
-        inputfile = FileWrapper(*source)
-
-        if cjson:
-            filetype = readerclasses["cjson"]
-
-        else:
-            # Try and guess the parser we need.
-            filetype = guess_filetype(inputfile)
-
-            # Reset our position back to 0.
-            inputfile.reset()
-
-        # If the input file isn't a standard compchem log file, try one of
-        # the readers, falling back to Open Babel.
-        if not filetype:
-            # TODO: This assumes we only got a single file...
-            filename = list(inputfile.filenames)[0]
-            ext = pathlib.Path(filename).name[1:].lower()
-
-            for extension in readerclasses:
-                if ext == extension:
-                    filetype = readerclasses[extension]
-
-        # Proceed to return an instance of the logfile parser only if the filetype
-        # could be guessed.
-        if filetype:
-            return filetype(inputfile, *args, **kwargs)
-
-        elif inputfile is not None:
-            inputfile.close()
-            # Stop us closing twice in the except block.
-            inputfile = None
-
-        logger.warning(
-            "Unable to determine the type of logfile %s, try the fallback mechanism", source
-        )
-
-    except Exception:
-        if inputfile is not None:
-            inputfile.close()
-
-        if not quiet:
-            raise
-
-        # We're going to swallow this exception if quiet is True.
-        # This can hide a lot of errors, so we'll make sure to log it.
-        logger.error("Failed to open logfile", exc_info=True)
+    ccdriver_inst = ccDriver(source)
+    return ccdriver_inst
 
 
-def fallback(source):
-    """Attempt to read standard molecular formats using other libraries.
+# def fallback(source):
+#     """Attempt to read standard molecular formats using other libraries.
 
-    Currently this will read XYZ files with OpenBabel, but this can easily
-    be extended to other formats and libraries, too.
-    """
-
-    if isinstance(source, str):
-        ext = os.path.splitext(source)[1][1:].lower()
-        if _has_cclib2openbabel:
-            # From OB 3.0 onward, Pybel is contained inside the OB module.
-            try:
-                import openbabel.pybel as pb
-            except:
-                import pybel as pb
-            if ext in pb.informats:
-                return cclib2openbabel.readfile(source, ext)
-        else:
-            # This should be a warning, but warnings are currently disabled by default.
-            logging.getLogger("cclib").error(
-                "Could not import `openbabel`, fallback mechanism might not work."
-            )
-
-
-def ccwrite(
-    ccobj,
-    outputtype=None,
-    outputdest=None,
-    indices=None,
-    terse=False,
-    returnstr=False,
-    *args,
-    **kwargs,
-):
-    """Write the parsed data from an outputfile to a standard chemical
-    representation.
-
-    Inputs:
-        ccobj - Either a job (from ccopen) or a data (from job.parse()) object
-        outputtype - The output format (should be a string)
-        outputdest - A filename or file object for writing
-        indices - One or more indices for extracting specific geometries/etc. (zero-based)
-        terse -  This option is currently limited to the cjson/json format. Whether to indent the cjson/json or not
-        returnstr - Whether or not to return a string representation.
-
-    The different writers may take additional arguments, which are
-    documented in their respective docstrings.
-
-    Returns:
-        the string representation of the chemical datatype
-          requested, or None.
-    """
-
-    # Determine the correct output format.
-    outputclass = _determine_output_format(outputtype, outputdest)
-
-    # Is ccobj an job object (unparsed), or is it a ccdata object (parsed)?
-    if isinstance(ccobj, logfileparser.Logfile):
-        jobfilename = ccobj.filename
-        ccdata = ccobj.parse()
-    elif isinstance(ccobj, data.ccData):
-        jobfilename = None
-        ccdata = ccobj
-    else:
-        raise ValueError
-
-    # If the logfile name has been passed in through kwargs (such as
-    # in the ccwrite script), make sure it has precedence.
-    if "jobfilename" in kwargs:
-        jobfilename = kwargs["jobfilename"]
-        # Avoid passing multiple times into the main call.
-        del kwargs["jobfilename"]
-
-    outputobj = outputclass(
-        ccdata, jobfilename=jobfilename, indices=indices, terse=terse, *args, **kwargs
-    )
-    output = outputobj.generate_repr()
-
-    # If outputdest isn't None, write the output to disk.
-    if outputdest is not None:
-        if isinstance(outputdest, str):
-            with open(outputdest, "w") as outputobj:
-                outputobj.write(output)
-        elif isinstance(outputdest, io.IOBase):
-            outputdest.write(output)
-        else:
-            raise ValueError
-    # If outputdest is None, return a string representation of the output.
-    else:
-        return output
-
-    if returnstr:
-        return output
-
-
-def _determine_output_format(outputtype, outputdest):
-    """
-    Determine the correct output format.
-
-    Inputs:
-      outputtype - a string corresponding to the file type
-      outputdest - a filename string or file handle
-    Returns:
-      outputclass - the class corresponding to the correct output format
-    Raises:
-      UnknownOutputFormatError for unsupported file writer extensions
-    """
-
-    # Priority for determining the correct output format:
-    #  1. outputtype
-    #  2. outputdest
-
-    outputclass = None
-    # First check outputtype.
-    if isinstance(outputtype, str):
-        extension = outputtype.lower()
-        if extension in writerclasses:
-            outputclass = writerclasses[extension]
-        else:
-            raise UnknownOutputFormatError(extension)
-    else:
-        # Then checkout outputdest.
-        if isinstance(outputdest, str):
-            extension = os.path.splitext(outputdest)[1].lower()
-        elif isinstance(outputdest, io.IOBase):
-            extension = os.path.splitext(outputdest.name)[1].lower()
-        else:
-            raise UnknownOutputFormatError
-        if extension in writerclasses:
-            outputclass = writerclasses[extension]
-        else:
-            raise UnknownOutputFormatError(extension)
-
-    return outputclass
-
-
-def _check_pandas(found_pandas):
-    if not found_pandas:
-        raise ImportError("You must install `pandas` to use this function")
-
-
-def ccframe(ccobjs, *args, **kwargs):
-    """Returns a pandas.DataFrame of data attributes parsed by cclib from one
-    or more logfiles.
-
-    Inputs:
-        ccobjs - an iterable of either cclib jobs (from ccopen) or data (from
-        job.parse()) objects
-
-    Returns:
-        a pandas.DataFrame
-    """
-    _check_pandas(_has_pandas)
-    logfiles = []
-    for ccobj in ccobjs:
-        # Is ccobj an job object (unparsed), or is it a ccdata object (parsed)?
-        if isinstance(ccobj, logfileparser.Logfile):
-            jobfilename = ccobj.filename
-            ccdata = ccobj.parse()
-        elif isinstance(ccobj, data.ccData):
-            jobfilename = None
-            ccdata = ccobj
-        else:
-            raise ValueError
+#     Currently this will read XYZ files with OpenBabel, but this can easily
+#     be extended to other formats and libraries, too.
+#     """
+
+#     if isinstance(source, str):
+#         ext = os.path.splitext(source)[1][1:].lower()
+#         if _has_cclib2openbabel:
+#             # From OB 3.0 onward, Pybel is contained inside the OB module.
+#             try:
+#                 import openbabel.pybel as pb
+#             except:
+#                 import pybel as pb
+#             if ext in pb.informats:
+#                 return cclib2openbabel.readfile(source, ext)
+#         else:
+#             # This should be a warning, but warnings are currently disabled by default.
+#             logging.getLogger("cclib").error(
+#                 "Could not import `openbabel`, fallback mechanism might not work."
+#             )
+
+
+# def ccwrite(
+#     ccobj,
+#     outputtype=None,
+#     outputdest=None,
+#     indices=None,
+#     terse=False,
+#     returnstr=False,
+#     *args,
+#     **kwargs,
+# ):
+#     """Write the parsed data from an outputfile to a standard chemical
+#     representation.
+
+#     Inputs:
+#         ccobj - Either a job (from ccopen) or a data (from job.parse()) object
+#         outputtype - The output format (should be a string)
+#         outputdest - A filename or file object for writing
+#         indices - One or more indices for extracting specific geometries/etc. (zero-based)
+#         terse -  This option is currently limited to the cjson/json format. Whether to indent the cjson/json or not
+#         returnstr - Whether or not to return a string representation.
+
+#     The different writers may take additional arguments, which are
+#     documented in their respective docstrings.
+
+#     Returns:
+#         the string representation of the chemical datatype
+#           requested, or None.
+#     """
+
+#     # Determine the correct output format.
+#     outputclass = _determine_output_format(outputtype, outputdest)
+
+#     # Is ccobj an job object (unparsed), or is it a ccdata object (parsed)?
+#     if isinstance(ccobj, logfileparser.Logfile):
+#         jobfilename = ccobj.filename
+#         ccdata = ccobj.parse()
+#     elif isinstance(ccobj, data.ccData):
+#         jobfilename = None
+#         ccdata = ccobj
+#     else:
+#         raise ValueError
+
+#     # If the logfile name has been passed in through kwargs (such as
+#     # in the ccwrite script), make sure it has precedence.
+#     if "jobfilename" in kwargs:
+#         jobfilename = kwargs["jobfilename"]
+#         # Avoid passing multiple times into the main call.
+#         del kwargs["jobfilename"]
+
+#     outputobj = outputclass(
+#         ccdata, jobfilename=jobfilename, indices=indices, terse=terse, *args, **kwargs
+#     )
+#     output = outputobj.generate_repr()
+
+#     # If outputdest isn't None, write the output to disk.
+#     if outputdest is not None:
+#         if isinstance(outputdest, str):
+#             with open(outputdest, "w") as outputobj:
+#                 outputobj.write(output)
+#         elif isinstance(outputdest, io.IOBase):
+#             outputdest.write(output)
+#         else:
+#             raise ValueError
+#     # If outputdest is None, return a string representation of the output.
+#     else:
+#         return output
+
+#     if returnstr:
+#         return output
+
+
+# def _determine_output_format(outputtype, outputdest):
+#     """
+#     Determine the correct output format.
+
+#     Inputs:
+#       outputtype - a string corresponding to the file type
+#       outputdest - a filename string or file handle
+#     Returns:
+#       outputclass - the class corresponding to the correct output format
+#     Raises:
+#       UnknownOutputFormatError for unsupported file writer extensions
+#     """
+
+#     # Priority for determining the correct output format:
+#     #  1. outputtype
+#     #  2. outputdest
+
+#     outputclass = None
+#     # First check outputtype.
+#     if isinstance(outputtype, str):
+#         extension = outputtype.lower()
+#         if extension in writerclasses:
+#             outputclass = writerclasses[extension]
+#         else:
+#             raise UnknownOutputFormatError(extension)
+#     else:
+#         # Then checkout outputdest.
+#         if isinstance(outputdest, str):
+#             extension = os.path.splitext(outputdest)[1].lower()
+#         elif isinstance(outputdest, io.IOBase):
+#             extension = os.path.splitext(outputdest.name)[1].lower()
+#         else:
+#             raise UnknownOutputFormatError
+#         if extension in writerclasses:
+#             outputclass = writerclasses[extension]
+#         else:
+#             raise UnknownOutputFormatError(extension)
+
+#     return outputclass
+
+
+# def _check_pandas(found_pandas):
+#     if not found_pandas:
+#         raise ImportError("You must install `pandas` to use this function")
+
+
+# def ccframe(ccobjs, *args, **kwargs):
+#     """Returns a pandas.DataFrame of data attributes parsed by cclib from one
+#     or more logfiles.
+
+#     Inputs:
+#         ccobjs - an iterable of either cclib jobs (from ccopen) or data (from
+#         job.parse()) objects
+
+#     Returns:
+#         a pandas.DataFrame
+#     """
+#     _check_pandas(_has_pandas)
+#     logfiles = []
+#     for ccobj in ccobjs:
+#         # Is ccobj an job object (unparsed), or is it a ccdata object (parsed)?
+#         if isinstance(ccobj, logfileparser.Logfile):
+#             jobfilename = ccobj.filename
+#             ccdata = ccobj.parse()
+#         elif isinstance(ccobj, data.ccData):
+#             jobfilename = None
+#             ccdata = ccobj
+#         else:
+#             raise ValueError
 
-        attributes = ccdata.getattributes()
-        attributes.update({"jobfilename": jobfilename})
+#         attributes = ccdata.getattributes()
+#         attributes.update({"jobfilename": jobfilename})
 
-        logfiles.append(pd.Series(attributes))
-    return pd.DataFrame(logfiles)
+#         logfiles.append(pd.Series(attributes))
+#     return pd.DataFrame(logfiles)
 
 
-del find_package
+# del find_package
```

### Comparing `cclib-1.8.1rc2/cclib/io/cjsonreader.py` & `cclib-2.0a1/cclib/io/cjsonreader.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/io/cjsonwriter.py` & `cclib-2.0a1/cclib/io/cjsonwriter.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,17 +70,17 @@
 
             # 'moments' and 'atomcoords' key will contain processed data
             # obtained from the output file. TODO rewrite this
             if attribute_name in ("moments", "atomcoords"):
                 if attribute_name == "moments":
                     dipole_moment = self._calculate_total_dipole_moment()
                     if dipole_moment is not None:
-                        cjson_dict["properties"][
-                            ccData._attributes["moments"].json_key
-                        ] = dipole_moment
+                        cjson_dict["properties"][ccData._attributes["moments"].json_key] = (
+                            dipole_moment
+                        )
                 else:
                     cjson_dict["atoms"]["coords"] = dict()
                     cjson_dict["atoms"]["coords"]["3d"] = (
                         self.ccdata.atomcoords[-1].flatten().tolist()
                     )
                 continue
```

### Comparing `cclib-1.8.1rc2/cclib/io/cmlwriter.py` & `cclib-2.0a1/cclib/io/cmlwriter.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/io/filereader.py` & `cclib-2.0a1/cclib/io/filereader.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/io/filewriter.py` & `cclib-2.0a1/cclib/io/filewriter.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/io/moldenwriter.py` & `cclib-2.0a1/cclib/io/moldenwriter.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,20 +265,17 @@
         # [Atoms] (Angs|AU)
         unit = "Angs"
         molden_lines.append(f"[Atoms] {unit}")
         # Last set of coordinates for geometry optimization runs.
         index = -1
         molden_lines.extend(self._coords_from_ccdata(index))
 
-        (
-            mosyms,
-            moenergies,
-            mooccs,
-            mocoeffs,
-        ) = self._syms_energies_occs_coeffs_from_ccdata_for_moldenwriter()
+        (mosyms, moenergies, mooccs, mocoeffs) = (
+            self._syms_energies_occs_coeffs_from_ccdata_for_moldenwriter()
+        )
 
         if hasattr(self.ccdata, "gbasis"):
             molden_lines.append("[GTO]")
             molden_lines.extend(self._gto_from_ccdata())
         if all(attr is not None for attr in (mosyms, moenergies, mooccs)):
             molden_lines.append("[MO]")
             molden_lines.extend(self._mo_from_ccdata(mosyms, moenergies, mooccs, mocoeffs))
```

### Comparing `cclib-1.8.1rc2/cclib/io/wfxwriter.py` & `cclib-2.0a1/cclib/io/wfxwriter.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/io/xyzreader.py` & `cclib-2.0a1/cclib/io/xyzreader.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/io/xyzwriter.py` & `cclib-2.0a1/cclib/io/xyzwriter.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/method/__init__.py` & `cclib-2.0a1/cclib/method/__init__.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/method/bader.py` & `cclib-2.0a1/cclib/method/bader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 # Copyright (c) 2024, the cclib development team
 #
 # This file is part of cclib (http://cclib.github.io) and is distributed under
 # the terms of the BSD 3-Clause License.
 
 """Calculation of Bader's QTAIM charges based on data parsed by cclib."""
-import copy
+
 import logging
-import math
-import random
 
 from cclib.method.calculationmethod import Method
 from cclib.method.volume import electrondensity_spin
-from cclib.parser.utils import convertor
 
 import numpy
 
 # Distance between two adjacent grids (sqrt[2] or sqrt[3] for uniform Cartesian grid).
 _griddist = numpy.array(
     [
         [[1.73205, 1.41421, 1.73205], [1.41421, 1, 1.41421], [1.73205, 1.41421, 1.73205]],
```

### Comparing `cclib-1.8.1rc2/cclib/method/bickelhaupt.py` & `cclib-2.0a1/cclib/method/bickelhaupt.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/method/calculationmethod.py` & `cclib-2.0a1/cclib/method/calculationmethod.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/method/cda.py` & `cclib-2.0a1/cclib/method/cda.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/method/cm5.py` & `cclib-2.0a1/cclib/method/cm5.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/method/cspa.py` & `cclib-2.0a1/cclib/method/cspa.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/method/ddec.py` & `cclib-2.0a1/cclib/method/ddec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 # Copyright (c) 2024, the cclib development team
 #
 # This file is part of cclib (http://cclib.github.io) and is distributed under
 # the terms of the BSD 3-Clause License.
 
 """Calculation of DDEC charges based on data parsed by cclib."""
+
 import copy
 import logging
 import math
-import os
-import random
-import sys
-from typing import List
 
-from cclib.method.calculationmethod import Method
 from cclib.method.stockholder import Stockholder
-from cclib.method.volume import electrondensity_spin
-from cclib.parser.utils import convertor, find_package
+from cclib.parser.utils import convertor
 
 import numpy
 
 
 class MissingInputError(Exception):
     pass
 
@@ -110,19 +105,17 @@
             f"Total charge density in the grid is {integrated_density}. If this does not match what is expected, using a finer grid may help."
         )
 
         # * STEP 1 *
         # Carry out step 1 of DDEC6 algorithm [Determining reference charge value]
         # Refer to equations 49-57 in doi: 10.1039/c6ra04656h
         self.logger.info("Creating first reference charges. (Step 1/7)")
-        (
-            reference_charges,
-            localized_charges,
-            stockholder_charges,
-        ) = self.calculate_reference_charges()
+        (reference_charges, localized_charges, stockholder_charges) = (
+            self.calculate_reference_charges()
+        )
         self.reference_charges = [reference_charges]
         self._localized_charges = [localized_charges]
         self._stockholder_charges = [stockholder_charges]
 
         # * STEP 2 *
         # Load new proatom densities based on the reference charges determined in step 1.
         self.logger.info("Creating second reference charges. (Step 2/7)")
```

### Comparing `cclib-1.8.1rc2/cclib/method/density.py` & `cclib-2.0a1/cclib/method/density.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/method/electrons.py` & `cclib-2.0a1/cclib/method/electrons.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/method/fragments.py` & `cclib-2.0a1/cclib/method/fragments.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/method/hirshfeld.py` & `cclib-2.0a1/cclib/method/hirshfeld.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (c) 2024, the cclib development team
 #
 # This file is part of cclib (http://cclib.github.io) and is distributed under
 # the terms of the BSD 3-Clause License.
 
 """Calculation of Hirshfeld charges based on data parsed by cclib."""
+
 import copy
 import logging
 import math
 import os
 import random
 import sys
 from typing import List
```

### Comparing `cclib-1.8.1rc2/cclib/method/lpa.py` & `cclib-2.0a1/cclib/method/lpa.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/method/mbo.py` & `cclib-2.0a1/cclib/method/mbo.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/method/moments.py` & `cclib-2.0a1/cclib/method/moments.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/method/mpa.py` & `cclib-2.0a1/cclib/method/mpa.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/method/nuclear.py` & `cclib-2.0a1/cclib/method/nuclear.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/method/opa.py` & `cclib-2.0a1/cclib/method/opa.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/method/orbitals.py` & `cclib-2.0a1/cclib/method/orbitals.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/method/population.py` & `cclib-2.0a1/cclib/method/population.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/method/stockholder.py` & `cclib-2.0a1/cclib/method/stockholder.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/method/volume.py` & `cclib-2.0a1/cclib/method/volume.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # This file is part of cclib (http://cclib.github.io) and is distributed under
 # the terms of the BSD 3-Clause License.
 
 """Calculation methods related to volume based on cclib data."""
 
 import copy
 
+from cclib.file_handler import FileHandler
 from cclib.parser.utils import convertor, find_package
 
 import numpy
 
 """ In the dictionary sym2powerlist below, each element is a list that contain the combinations of
     powers that are applied to x, y, and z in the equation for the gaussian primitives --
     \psi (x, y, z) = x^a * y^b * z^c * exp(-\lambda * r^2)
@@ -405,15 +406,15 @@
     Input:
         filepath -- path to the cube file
 
     Output:
         vol -- Volume object filled with data from cube file
     """
 
-    with open(filepath) as f:
+    with FileHandler(filepath) as f:
         lines = f.readlines()
 
         # First two lines are comments
         # Lines 3-6 specify the grid in Cartesian coordinates
         # Line 3 -- [Number of atoms] [Origin x] [Origin y] [Origin z]
         natom = (int)(lines[2].split()[0])
         originx, originy, originz = numpy.asanyarray(lines[2].split()[1:], dtype=float)
```

### Comparing `cclib-1.8.1rc2/cclib/parser/adfparser.py` & `cclib-2.0a1/cclib/parser/adfparser.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/parser/daltonparser.py` & `cclib-2.0a1/cclib/parser/daltonparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright (c) 2024, the cclib development team
 #
 # This file is part of cclib (http://cclib.github.io) and is distributed under
 # the terms of the BSD 3-Clause License.
 
 """Parser for DALTON output files"""
 
-
 import re
 
 from cclib.parser import logfileparser, utils
 
 import numpy
```

### Comparing `cclib-1.8.1rc2/cclib/parser/data.py` & `cclib-2.0a1/cclib/attribute_parsers/data.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,20 +5,19 @@
 
 """Classes and tools for storing and handling parsed data"""
 
 import logging
 from collections import namedtuple
 from typing import Any, Dict, List, Mapping, Optional
 
+from cclib.attributes.attribute import Attribute, _attributes
 from cclib.method import Electrons, orbitals
 
 import numpy
 
-Attribute = namedtuple("Attribute", ["type", "json_key", "attribute_path"])
-
 
 class ccData:
     """Stores data extracted by cclib parsers
 
     Description of cclib attributes:
         aonames -- atomic orbital names (list of strings)
         aooverlaps -- atomic orbital overlap matrix (array[2])
@@ -65,15 +64,15 @@
         nmo -- number of molecular orbitals (integer)
         nmrtensors -- Nuclear magnetic resonance chemical shielding tensors (dict of dicts of array[2])
         nmrcouplingtensors -- Nuclear magnetic resonance spin-spin coupling tensors (dict of dicts of array[2])
         nocoeffs -- natural orbital coefficients (array[2])
         nooccnos -- natural orbital occupation numbers (array[1])
         nsocoeffs -- natural spin orbital coefficients (list of array[2])
         nsooccnos -- natural spin orbital occupation numbers (list of array[1])
-        optdone -- flags whether an optimization has converged (Boolean)
+        optdone -- flags whether an optimization has converged (List)
         optstatus -- optimization status for each set of atomic coordinates (array[1])
         polarizabilities -- (dipole) polarizabilities, static or dynamic (list of arrays[2])
         pressure -- pressure used for Thermochemistry (float, atm)
         rotconsts -- rotational constants (array[2], GHz)
         scancoords -- geometries of each scan step (array[3], angstroms)
         scanenergies -- energies of potential energy surface (list)
         scannames -- names of variables scanned (list of strings)
@@ -99,93 +98,14 @@
     (3) Python indexes arrays/lists starting at zero, so if homos==[10], then
             the 11th molecular orbital is the HOMO
     """
 
     # The expected types for all supported attributes.
     # The json_key is the key name used for attributes in the CJSON/JSON format
     # 'TBD' - To Be Decided are the key names of attributes which haven't been included in the cjson format
-    _attributes = {
-        "aonames": Attribute(list, "names", "atoms:orbitals"),
-        "aooverlaps": Attribute(numpy.ndarray, "overlaps", "properties:orbitals"),
-        "atombasis": Attribute(list, "indices", "atoms:orbitals"),
-        "atomcharges": Attribute(dict, "partial charges", "properties"),
-        "atomcoords": Attribute(numpy.ndarray, "coords", "atoms:coords:3d"),
-        "atommasses": Attribute(numpy.ndarray, "mass", "atoms"),
-        "atomnos": Attribute(numpy.ndarray, "number", "atoms:elements"),
-        "atomspins": Attribute(dict, "spins", "atoms"),
-        "ccenergies": Attribute(numpy.ndarray, "coupled cluster", "properties:energy"),
-        "charge": Attribute(int, "charge", "properties"),
-        "coreelectrons": Attribute(numpy.ndarray, "core electrons", "atoms"),
-        "dispersionenergies": Attribute(
-            numpy.ndarray, "dispersion correction", "properties:energy"
-        ),
-        "enthalpy": Attribute(float, "enthalpy", "properties"),
-        "entropy": Attribute(float, "entropy", "properties"),
-        "etenergies": Attribute(numpy.ndarray, "electronic transitions", "transitions"),
-        "etoscs": Attribute(numpy.ndarray, "oscillator strength", "transitions"),
-        "etdips": Attribute(numpy.ndarray, "electic transition dipoles", "transitions"),
-        "etveldips": Attribute(
-            numpy.ndarray, "velocity-gauge electric transition dipoles", "transitions"
-        ),
-        "etmagdips": Attribute(numpy.ndarray, "magnetic transition dipoles", "transitions"),
-        "etrotats": Attribute(numpy.ndarray, "rotatory strength", "transitions"),
-        "etsecs": Attribute(list, "one excited config", "transitions"),
-        "etsyms": Attribute(list, "symmetry", "transitions"),
-        "freeenergy": Attribute(float, "free energy", "properties:energy"),
-        "fonames": Attribute(list, "orbital names", "fragments"),
-        "fooverlaps": Attribute(numpy.ndarray, "orbital overlap", "fragments"),
-        "fragnames": Attribute(list, "fragment names", "fragments"),
-        "frags": Attribute(list, "atom indices", "fragments"),
-        "gbasis": Attribute(list, "basis functions", "atoms:orbitals"),
-        "geotargets": Attribute(numpy.ndarray, "geometric targets", "optimization"),
-        "geovalues": Attribute(numpy.ndarray, "geometric values", "optimization"),
-        "grads": Attribute(numpy.ndarray, "TBD", "N/A"),
-        "hessian": Attribute(numpy.ndarray, "hessian matrix", "vibrations"),
-        "homos": Attribute(numpy.ndarray, "homos", "properties:orbitals"),
-        "metadata": Attribute(dict, "TBD", "N/A"),
-        "mocoeffs": Attribute(list, "coeffs", "properties:orbitals"),
-        "moenergies": Attribute(list, "energies", "properties:orbitals"),
-        "moments": Attribute(list, "total dipole moment", "properties"),
-        "mosyms": Attribute(list, "molecular orbital symmetry", "properties:orbitals"),
-        "mpenergies": Attribute(numpy.ndarray, "moller plesset", "properties:energy"),
-        "mult": Attribute(int, "multiplicity", "properties"),
-        "natom": Attribute(int, "number of atoms", "properties"),
-        "nbasis": Attribute(int, "basis number", "properties:orbitals"),
-        "nmo": Attribute(int, "MO number", "properties:orbitals"),
-        "nmrtensors": Attribute(dict, "NMR chemical shielding tensors", "properties:nmr"),
-        "nmrcouplingtensors": Attribute(dict, "NMR spin-spin coupling tensors", "properties:nmr"),
-        "nocoeffs": Attribute(numpy.ndarray, "TBD", "N/A"),
-        "nooccnos": Attribute(numpy.ndarray, "TBD", "N/A"),
-        "nsocoeffs": Attribute(list, "TBD", "N/A"),
-        "nsooccnos": Attribute(list, "TBD", "N/A"),
-        "optdone": Attribute(list, "done", "optimization"),
-        "optstatus": Attribute(numpy.ndarray, "status", "optimization"),
-        "polarizabilities": Attribute(list, "polarizabilities", "N/A"),
-        "pressure": Attribute(float, "pressure", "properties"),
-        "rotconsts": Attribute(numpy.ndarray, "rotational constants", "atoms:coords:rotconsts"),
-        "scancoords": Attribute(numpy.ndarray, "step geometry", "optimization:scan"),
-        "scanenergies": Attribute(list, "PES energies", "optimization:scan"),
-        "scannames": Attribute(list, "variable names", "optimization:scan"),
-        "scanparm": Attribute(list, "PES parameter values", "optimization:scan"),
-        "scfenergies": Attribute(numpy.ndarray, "scf energies", "optimization:scf"),
-        "scftargets": Attribute(numpy.ndarray, "targets", "optimization:scf"),
-        "scfvalues": Attribute(list, "values", "optimization:scf"),
-        "temperature": Attribute(float, "temperature", "properties"),
-        "time": Attribute(numpy.ndarray, "time", "N/A"),
-        "transprop": Attribute(dict, "electronic transitions", "transitions"),
-        "vibanharms": Attribute(numpy.ndarray, "anharmonicity constants", "vibrations"),
-        "vibdisps": Attribute(numpy.ndarray, "displacement", "vibrations"),
-        "vibfreqs": Attribute(numpy.ndarray, "frequencies", "vibrations"),
-        "vibfconsts": Attribute(numpy.ndarray, "force constants", "vibrations"),
-        "vibirs": Attribute(numpy.ndarray, "IR", "vibrations:intensities"),
-        "vibramans": Attribute(numpy.ndarray, "raman", "vibrations:intensities"),
-        "vibrmasses": Attribute(numpy.ndarray, "reduced masses", "vibrations"),
-        "vibsyms": Attribute(list, "vibration symmetry", "vibrations"),
-        "zpve": Attribute(float, "zero-point correction", "properties:energies"),
-    }
 
     # The name of all attributes can be generated from the dictionary above.
     _attrlist = sorted(_attributes.keys())
 
     # Arrays are double precision by default, but these will be integer arrays.
     _intarrays = ["atomnos", "coreelectrons", "homos", "optstatus"]
 
@@ -214,23 +134,25 @@
 
         Normally called in the parse() method of a Logfile subclass.
 
         Inputs:
             attributes - optional dictionary of attributes to load as data
         """
 
+        self._parsed_attributes = dict()
+
         if attributes:
             self.setattributes(attributes)
 
     def listify(self) -> None:
         """Converts all attributes that are arrays or lists/dicts of arrays to lists."""
 
         attrlist = [k for k in self._attrlist if hasattr(self, k)]
         for k in attrlist:
-            v = self._attributes[k].type
+            v = _attributes[k].type
             if v == numpy.ndarray:
                 setattr(self, k, getattr(self, k).tolist())
             elif v == list and k in self._listsofarrays:
                 setattr(self, k, [x.tolist() for x in getattr(self, k)])
             elif v == dict and k in self._dictsofarrays:
                 items = getattr(self, k).items()
                 pairs = [(key, val.tolist()) for key, val in items]
@@ -245,15 +167,15 @@
                 setattr(self, k, dict(pairs))
 
     def arrayify(self) -> None:
         """Converts appropriate attributes to arrays or lists/dicts of arrays."""
 
         attrlist = [k for k in self._attrlist if hasattr(self, k)]
         for k in attrlist:
-            v = self._attributes[k].type
+            v = _attributes[k].type
             precision = "d"
             if k in self._intarrays:
                 precision = "i"
             if v == numpy.ndarray:
                 setattr(self, k, numpy.array(getattr(self, k), precision))
             elif v == list and k in self._listsofarrays:
                 setattr(self, k, [numpy.array(x, precision) for x in getattr(self, k)])
@@ -300,45 +222,47 @@
         Inputs:
             attributes - dictionary of attributes to set
         Outputs:
             invalid - list of attributes names that were not set, which
                       means they are not specified in self._attrlist
         """
 
-        if type(attributes) is not dict:
+        if not isinstance(attributes, dict):
             raise TypeError("attributes must be in a dictionary")
 
         valid = [a for a in attributes if a in self._attrlist]
         invalid = [a for a in attributes if a not in self._attrlist]
 
         for attr in valid:
             setattr(self, attr, attributes[attr])
 
-        self.arrayify()
-        self.typecheck()
+        # self.arrayify()
+        # self.typecheck()
 
         return invalid
 
     def typecheck(self) -> None:
         """Check the types of all attributes.
 
         If an attribute does not match the expected type, then attempt to
         convert; if that fails, only then raise a TypeError.
         """
 
         self.arrayify()
         for attr in [a for a in self._attrlist if hasattr(self, a)]:
+            # attr.typecheck()
+
             val = getattr(self, attr)
-            if type(val) == self._attributes[attr].type:
+            if isinstance(val, _attributes[attr].type):
                 continue
 
             try:
-                val = self._attributes[attr].type(val)
+                val = _attributes[attr].type(val)
             except ValueError:
-                args = (attr, type(val), self._attributes[attr].type)
+                args = (attr, type(val), _attributes[attr].type)
                 raise TypeError(
                     f"attribute {args[0]} is {args[1]} instead of {args[2]} and could not be converted"
                 )
 
     def check_values(self, logger=logging) -> None:
         """Perform custom checks on the values of attributes."""
         if hasattr(self, "etenergies") and any(e < 0 for e in self.etenergies):
@@ -441,21 +365,51 @@
     def nelectrons(self) -> int:
         return Electrons(self).count()
 
     @property
     def closed_shell(self) -> bool:
         return orbitals.Orbitals(self).closed_shell()
 
+    def __setattr__(self, name: str, value: Any) -> None:
+        if name in _attributes:
+            self._parsed_attributes[name] = value
+        else:
+            super().__setattr__(name, value)
+
+    def __getattr__(self, name: str) -> Any:
+        # If we couldn't find an attribute directly on the class, which, for
+        # an Attribute, should actually be a property, then it's not
+        # implemented as a property yet and is in our special attribute
+        # container.
+        try:
+            return self._parsed_attributes[name]
+        except KeyError:
+            pass
+            # raise AttributeError
+
+    @property
+    def aonames(self):
+        try:
+            return self._parsed_attributes["aonames"]
+        except:
+            pass
+        # except KeyError:
+        #    raise AttributeError
+
+    # @aonames.setter
+    # def aonames(self, val):
+    #     setattr(self, "aonames", val)
+
 
 class ccData_optdone_bool(ccData):
     """This is the version of ccData where optdone is a Boolean."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self._attributes["optdone"] = Attribute(bool, "done", "optimization")
+        _attributes["optdone"] = Attribute(bool, "done", "optimization")
 
     def setattributes(self, *args, **kwargs):
         invalid = super().setattributes(*args, **kwargs)
 
         # Reduce optdone to a Boolean, because it will be parsed as a list. If this list has any element,
         # it means that there was an optimized structure and optdone should be True.
         if hasattr(self, "optdone"):
```

### Comparing `cclib-1.8.1rc2/cclib/parser/fchkparser.py` & `cclib-2.0a1/cclib/parser/fchkparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright (c) 2024, the cclib development team
 #
 # This file is part of cclib (http://cclib.github.io) and is distributed under
 # the terms of the BSD 3-Clause License.
 
 """Parser for Formatted Checkpoint files"""
 
-
 from cclib.parser import logfileparser, utils
 
 import numpy
 
 SHELL_ORBITALS = {
     0: ["S"],
     1: ["PX", "PY", "PZ"],
```

### Comparing `cclib-1.8.1rc2/cclib/parser/gamessdatparser.py` & `cclib-2.0a1/cclib/parser/gamessdatparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright (c) 2024, the cclib development team
 #
 # This file is part of cclib (http://cclib.github.io) and is distributed under
 # the terms of the BSD 3-Clause License.
 
 """Parser for GAMESS(US) .dat output files"""
 
-
 import re
 
 from cclib.parser import logfileparser, utils
 from cclib.parser.utils import PeriodicTable
 
 import numpy
```

### Comparing `cclib-1.8.1rc2/cclib/parser/gamessparser.py` & `cclib-2.0a1/cclib/parser/gamessparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright (c) 2024, the cclib development team
 #
 # This file is part of cclib (http://cclib.github.io) and is distributed under
 # the terms of the BSD 3-Clause License.
 
 """Parser for GAMESS(US) output files"""
 
-
 import re
 
 from cclib.parser import logfileparser, utils
 
 import numpy
```

### Comparing `cclib-1.8.1rc2/cclib/parser/gamessukparser.py` & `cclib-2.0a1/cclib/parser/gamessukparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright (c) 2024, the cclib development team
 #
 # This file is part of cclib (http://cclib.github.io) and is distributed under
 # the terms of the BSD 3-Clause License.
 
 """Parser for GAMESS-UK output files"""
 
-
 import re
 
 from cclib.parser import logfileparser, utils
 
 import numpy
```

### Comparing `cclib-1.8.1rc2/cclib/parser/gaussianparser.py` & `cclib-2.0a1/cclib/parser/gaussianparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright (c) 2024, the cclib development team
 #
 # This file is part of cclib (http://cclib.github.io) and is distributed under
 # the terms of the BSD 3-Clause License.
 
 """Parser for Gaussian output files"""
 
-
 import datetime
 import re
 
 from cclib.parser import data, logfileparser, utils
 from cclib.parser.logfileparser import StopParsing
 
 import numpy
@@ -204,34 +203,38 @@
             _, _, platform_full_version, compile_date = next(inputfile).split()
             run_date = next(inputfile).strip()
             platform_full_version_tokens = platform_full_version.split("-")
             full_version = platform_full_version_tokens[-1]
             platform = "-".join(platform_full_version_tokens[:-1])
             year_suffix = full_version[1:3]
             revision = full_version[6:]
-            self.metadata[
-                "package_version"
-            ] = f"{self.YEAR_SUFFIXES_TO_YEARS[year_suffix]}+{revision}"
+            self.metadata["package_version"] = (
+                f"{self.YEAR_SUFFIXES_TO_YEARS[year_suffix]}+{revision}"
+            )
             self.metadata["platform"] = platform
 
         if line.strip().startswith("Link1:  Proceeding to internal job step number"):
             self.new_internal_job()
 
         # Parse performance info.
         if "Will use up to" in line and "processors via shared memory." in line:
             self.metadata["num_cpu"] = int(line.split()[4])
 
         elif "Leave Link    1" in line and "MaxMem=" in line and "num_cpu" in self.metadata:
             # Leave Link    1 at Wed Apr  4 10:49:19 2018, MaxMem=   805306368 cpu:               0.3 elap:               0.0
-            # Gaussian helpfully prints the total 'available' memory for us. There are, however a few caveates here:
+            # Gaussian helpfully prints the total 'available' memory for us. There are, however a few caveats here:
             # 1) This memory (in bytes) is per CPU
             # 2) The total memory here (x num_cpu) will not equal the amount requested in %mem because Gaussian (probably erroneously)
             #    interprets GB as gibibytes (1024 x 1024 x 1024 bytes) rather than gigabytes. This has the unfortunate consequence of
             #    Gaussian assigning more memory than you probably expected.
-            memory_per_cpu = int(line[line.index("MaxMem=") :].split()[1])
+            #
+            # MaxMem can appear with or without whitespace:
+            # MaxMem=  805306368
+            # MaxMem=174483046400
+            memory_per_cpu = int(re.search(r"MaxMem=\s*(\d+)", line).group(1))
             self.metadata["memory_used"] = memory_per_cpu * self.metadata["num_cpu"]
 
         elif line[1:6].lower() == "%mem=":
             # The maximum amount of memory requested.
             # We need to do some unit juggling.
             mem_str = line.strip().upper()
             # No space is allowed between units, units can probably only be uppercase but convert anyway.
```

### Comparing `cclib-1.8.1rc2/cclib/parser/jaguarparser.py` & `cclib-2.0a1/cclib/parser/jaguarparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright (c) 2024, the cclib development team
 #
 # This file is part of cclib (http://cclib.github.io) and is distributed under
 # the terms of the BSD 3-Clause License.
 
 """Parser for Jaguar output files"""
 
-
 import re
 
 from cclib.parser import logfileparser, utils
 
 import numpy
```

### Comparing `cclib-1.8.1rc2/cclib/parser/logfileparser.py` & `cclib-2.0a1/cclib/parser/logfileparser.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/parser/logfilewrapper.py` & `cclib-2.0a1/cclib/file_handler/file_handler.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,24 +5,28 @@
 
 # TOOD: This file belongs in cclib.io, but circular dependency issues mean it can't go there just now.
 
 import bz2
 import codecs
 import collections
 import gzip
+import inspect
 import io
 import logging
 import pathlib
 import re
 import typing
 import zipfile
 from tempfile import NamedTemporaryFile
+from typing import Any, Iterable, List, Optional
 from urllib.error import URLError
 from urllib.request import urlopen
 
+from cclib.file_handler import utils
+
 # Regular expression for validating URLs
 URL_PATTERN = re.compile(
     r"^(?:http|ftp)s?://"  # http:// or https://
     r"(?:(?:[A-Z0-9](?:[A-Z0-9-]{0,61}[A-Z0-9])?\.)+(?:[A-Z]{2,6}\.?|[A-Z0-9-]{2,}\.?)|"  # domain...
     r"localhost|"  # localhost...
     r"\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})"  # ...or ip
     r"(?::\d+)?"  # optional port
@@ -41,15 +45,15 @@
     # First item is a replacement character. Second is the position to continue from.
     return ("", error.start + 1)
 
 
 codecs.register_error("logerror", logerror)
 
 
-class FileWrapper:
+class FileHandler:
     """Wrap any supported input file type."""
 
     def __init__(self, *sources) -> None:
         # The total size of all our files.
         self.size = 0
         # Current 'byte' position in all our files.
         self.pos = 0
@@ -97,15 +101,15 @@
 
     @property
     def file_name(self) -> str:
         return ", ".join(self.filenames)
 
     def sort(self, order: list) -> None:
         """
-        Sort the individual files that make up this FileWrapper.
+        Sort the individual files that make up this FileHandler.
 
         order is an ordered list of filenames.
         """
         # Reset all our streams.
         self.reset()
 
         filenames = []
@@ -206,14 +210,65 @@
         else:
             # Normal text file.
 
             fileobject = open(filename, mode, encoding=encoding, errors=errors)
 
         return filename, fileobject
 
+    def __enter__(self):
+        """
+        Enter context.
+        """
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        """
+        Exit context
+        """
+        self.close()
+
+    def virtual_set(self):
+        """
+        For use with property parsers to handle parsing
+        through a block of text without changing the state of fileHandler.
+
+        Sets the virtual_file_pointer to the current file_pointer
+        """
+        self.virtual_reset_position = self.pos
+
+    def virtual_reset(self):
+        """
+        For use with property parsers to handle parsing
+        through a block of text without changing the state of fileHandler.
+
+        Sets the virtual_file_pointer to the current file_pointer
+        """
+        if self.virtual_reset_position is None:
+            raise RuntimeError("virtual_set() must be called before reset and virtual_next")
+        self.files[self.file_pointer].seek(self.virtual_reset_position)
+        self.pos = self.virtual_reset_position
+        self.virtual_reset_position = None
+
+    def virtual_next(self):
+        """
+        For use with property parsers to handle parsing
+        through a block of text without changing the state of fileHandler
+
+        virtual_next will _not_ advance to the next file
+        """
+        if self.virtual_reset_position is None:
+            raise RuntimeError("virtual_set() must be called before reset and virtual_next")
+        try:
+            line = next(self.files[self.file_pointer])
+            self.pos += len(line)
+            return line
+        except:
+            # possibly raise a warning? but we are ok just reaching the end of a file for a subparser parsing
+            return
+
     def next(self) -> str:
         """
         Get the next line from this log file.
         """
         try:
             try:
                 line = next(self.files[self.file_pointer])
@@ -222,15 +277,16 @@
                 return line
 
             except StopIteration:
                 self.file_pointer += 1
                 return self.next()
 
         except IndexError:
-            raise StopIteration()
+            return False
+            # raise StopIteration()
 
     @property
     def last_line(self) -> str:
         """
         Return the last line read by this parser.
         """
         return self.last_lines[-1]
@@ -244,14 +300,20 @@
     # TODO: support size parameter.
     def readline(self) -> str:
         """
         Read one line from this file.
         """
         return next(self)
 
+    def readlines(self) -> typing.List[str]:
+        """
+        Read all the lines from this file.
+        """
+        return list(self)
+
     # TODO: support size parameter.
     def read(self) -> str:
         """
         Read everything from this file.
 
         Be aware that this function will load the entire file into a single string.
         """
@@ -271,15 +333,15 @@
         Note that there is no guarantee when or if this function will get called;
         user's should ensure to close their own files once they are finished with them.
         """
         self.close()
 
     def seek(self, offset: int, whence: int = 0) -> None:
         if offset != 0 or whence not in (0, 2):
-            raise NotImplementedError("FileWrapper only supports seeking to start or end")
+            raise NotImplementedError("FileHandler only supports seeking to start or end")
 
         if whence == 0:
             self.reset()
 
         elif whence == 2:
             self.finish()
 
@@ -304,7 +366,62 @@
     def finish(self):
         # Equivalent to seeking to 2 for all our files.
         for file in self.files:
             file.seek(0, 2)
 
         self.file_pointer = len(self.files) - 1
         self.pos = self.size
+
+    def skip_lines(self, sequence: Iterable[str], virtual=False) -> List[str]:
+        """Read trivial line types and check they are what they are supposed to be.
+
+        This function will read len(sequence) lines and do certain checks on them,
+        when the elements of sequence have the appropriate values. Currently the
+        following elements trigger checks:
+            'blank' or 'b'      - the line should be blank
+            'dashes' or 'd'     - the line should contain only dashes (or spaces)
+            'equals' or 'e'     - the line should contain only equal signs (or spaces)
+            'stars' or 's'      - the line should contain only stars (or spaces)
+        """
+
+        expected_characters = {"-": ["dashes", "d"], "=": ["equals", "e"], "*": ["stars", "s"]}
+
+        lines = []
+        for expected in sequence:
+            # Read the line we want to skip.
+            if virtual:
+                line = self.virtual_next()
+            else:
+                line = self.next()
+
+            # Blank lines are perhaps the most common thing we want to check for.
+            if expected in ["blank", "b"]:
+                try:
+                    assert line.strip() == ""
+                except AssertionError:
+                    frame, fname, lno, funcname, funcline, index = inspect.getouterframes(
+                        inspect.currentframe()
+                    )[1]
+                    parser = fname.split("/")[-1]
+                    msg = (
+                        f"In {parser}, line {int(lno)}, line not blank as expected: {line.strip()}"
+                    )
+                    # self.logger.warning(msg)
+
+            # All cases of heterogeneous lines can be dealt with by the same code.
+            for character, keys in expected_characters.items():
+                if expected in keys:
+                    try:
+                        assert utils.str_contains_only(line.strip(), [character, " "])
+                    except AssertionError:
+                        frame, fname, lno, funcname, funcline, index = inspect.getouterframes(
+                            inspect.currentframe()
+                        )[1]
+                        parser = fname.split("/")[-1]
+                        msg = f"In {parser}, line {int(lno)}, line not all {keys[0]} as expected: {line.strip()}"
+                        # self.logger.warning(msg)
+                        continue
+
+            # Save the skipped line, and we will return the whole list.
+            lines.append(line)
+
+        return lines
```

### Comparing `cclib-1.8.1rc2/cclib/parser/molcasparser.py` & `cclib-2.0a1/cclib/parser/molcasparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,25 +42,25 @@
             # Use the short version as the legacy version.
             self.metadata["legacy_package_version"] = self.metadata["package_version"]
             # If there is both a tag and the full hash, place the tag
             # first. Both are chosen to be local, since there isn't a
             # distinction between development and release builds in their
             # version cycle.
             if "tag" in self.metadata and "revision" in self.metadata:
-                self.metadata[
-                    "package_version"
-                ] = f"{self.metadata['package_version']}+{self.metadata['tag']}.{self.metadata['revision']}"
+                self.metadata["package_version"] = (
+                    f"{self.metadata['package_version']}+{self.metadata['tag']}.{self.metadata['revision']}"
+                )
             elif "tag" in self.metadata:
-                self.metadata[
-                    "package_version"
-                ] = f"{self.metadata['package_version']}+{self.metadata['tag']}"
+                self.metadata["package_version"] = (
+                    f"{self.metadata['package_version']}+{self.metadata['tag']}"
+                )
             elif "revision" in self.metadata:
-                self.metadata[
-                    "package_version"
-                ] = f"{self.metadata['package_version']}+{self.metadata['revision']}"
+                self.metadata["package_version"] = (
+                    f"{self.metadata['package_version']}+{self.metadata['revision']}"
+                )
 
     def before_parsing(self):
         # Compile the regex for extracting the element symbol from the
         # atom label in the "Molecular structure info" block.
         self.re_atomelement = re.compile(r"([a-zA-Z]+)\d?")
 
         # Compile the dashes-and-or-spaces-only regex.
```

### Comparing `cclib-1.8.1rc2/cclib/parser/molproparser.py` & `cclib-2.0a1/cclib/parser/molproparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright (c) 2024, the cclib development team
 #
 # This file is part of cclib (http://cclib.github.io) and is distributed under
 # the terms of the BSD 3-Clause License.
 
 """Parser for Molpro output files"""
 
-
 import itertools
 
 from cclib.parser import logfileparser, utils
 
 import numpy
```

### Comparing `cclib-1.8.1rc2/cclib/parser/mopacparser.py` & `cclib-2.0a1/cclib/parser/mopacparser.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/parser/nboparser.py` & `cclib-2.0a1/cclib/parser/nboparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright (c) 2024, the cclib development team
 #
 # This file is part of cclib (http://cclib.github.io) and is distributed under
 # the terms of the BSD 3-Clause License.
 
 """Parser for NBO output files"""
 
-
 import re
 
 from cclib.parser import logfileparser, utils
 from cclib.parser.utils import PeriodicTable
 
 import numpy
```

### Comparing `cclib-1.8.1rc2/cclib/parser/nwchemparser.py` & `cclib-2.0a1/cclib/parser/nwchemparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright (c) 2024, the cclib development team
 #
 # This file is part of cclib (http://cclib.github.io) and is distributed under
 # the terms of the BSD 3-Clause License.
 
 """Parser for NWChem output files"""
 
-
 import itertools
 import re
 
 from cclib.parser import logfileparser, utils
 
 import numpy
 
@@ -48,17 +47,17 @@
             base_package_version = line.split()[3]
             self.metadata["legacy_package_version"] = base_package_version
             self.metadata["package_version"] = base_package_version
             line = next(inputfile)
             if "nwchem revision" in line:
                 revision = line.split()[3].split("-")[-1]
                 if revision != "N/A":
-                    self.metadata[
-                        "package_version"
-                    ] = f"{self.metadata['package_version']}+{revision}"
+                    self.metadata["package_version"] = (
+                        f"{self.metadata['package_version']}+{revision}"
+                    )
 
         # This is printed in the input module, so should always be the first coordinates,
         # and contains some basic information we want to parse as well. However, this is not
         # the only place where the coordinates are printed during geometry optimization,
         # since the gradients module has a separate coordinate printout, which happens
         # alongside the coordinate gradients. This geometry printout happens at the
         # beginning of each optimization step only.
```

### Comparing `cclib-1.8.1rc2/cclib/parser/orcaparser.py` & `cclib-2.0a1/cclib/parser/orcaparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright (c) 2024, the cclib development team
 #
 # This file is part of cclib (http://cclib.github.io) and is distributed under
 # the terms of the BSD 3-Clause License.
 
 """Parser for ORCA output files"""
 
-
 import datetime
 import re
 from itertools import zip_longest
 
 from cclib.parser import logfileparser, utils
 
 import numpy
@@ -49,14 +48,17 @@
 
         # Used to estimate CPU time from wall time.
         self.metadata["num_cpu"] = 1
 
         # The excited state multiplicity for post-HF excited states
         self.mdci_et_mult = None
 
+        # needs to be here so regression tests pass
+        self.reference = [0.0, 0.0, 0.0]
+
     def after_parsing(self):
         # ORCA doesn't add the dispersion energy to the "Total energy" (which
         # we parse), only to the "FINAL SINGLE POINT ENERGY" (which we don't
         # parse).
         if hasattr(self, "scfenergies") and hasattr(self, "dispersionenergies"):
             for i, (scfenergy, dispersionenergy) in enumerate(
                 zip_longest(self.scfenergies, self.dispersionenergies)
@@ -2159,47 +2161,60 @@
         # ...
         # --------------------------------
         # Total charge:    -0.000000
         # --------------------------------
         if line.startswith("CHELPG Charges"):
             self.parse_charge_section(line, inputfile, "chelpg")
 
+        # The center of mass is used as the origin
         # It is not stated explicitely, but the dipole moment components printed by ORCA
-        # seem to be in atomic units, so they will need to be converted. Also, they
-        # are most probably calculated with respect to the origin .
-        #
+        # seem to be in atomic units, so they will need to be converted.
+
+        # example:
+        # The origin for moment calculation is the CENTER OF MASS  = (-1.651256, -1.258772 -1.572312)
+
         # -------------
         # DIPOLE MOMENT
         # -------------
         #                                 X             Y             Z
         # Electronic contribution:      0.00000      -0.00000      -0.00000
         # Nuclear contribution   :      0.00000       0.00000       0.00000
         #                         -----------------------------------------
         # Total Dipole Moment    :      0.00000      -0.00000      -0.00000
         #                         -----------------------------------------
         # Magnitude (a.u.)       :      0.00000
         # Magnitude (Debye)      :      0.00000
         #
-        if line.strip() == "DIPOLE MOMENT":
+        # TODO: add quadrupole moment parsing, which can be optionally calculated with ORCA
+
+        # the origin/reference might be printed in multiple places in the output file
+        # depending on the calculation type
+        if line.startswith("The origin for moment calculation is"):
+            tmp_reference = line.split()[-3:]
+            reference_x = float(tmp_reference[0].replace("(", "").replace(",", ""))
+            reference_y = float(tmp_reference[1])
+            reference_z = float(tmp_reference[2].replace(")", ""))
+            self.reference = numpy.array([reference_x, reference_y, reference_z])
+
+        if line.startswith("DIPOLE MOMENT"):
             self.skip_lines(inputfile, ["d", "XYZ", "electronic", "nuclear", "d"])
             total = next(inputfile)
             assert "Total Dipole Moment" in total
 
-            reference = [0.0, 0.0, 0.0]
             dipole = numpy.array([float(d) for d in total.split()[-3:]])
             dipole = utils.convertor(dipole, "ebohr", "Debye")
 
             if not hasattr(self, "moments"):
-                self.set_attribute("moments", [reference, dipole])
+                self.set_attribute("moments", [self.reference, dipole])
             else:
                 try:
                     assert numpy.all(self.moments[1] == dipole)
                 except AssertionError:
                     self.logger.warning("Overwriting previous multipole moments with new values")
-                    self.set_attribute("moments", [reference, dipole])
+                    self.set_attribute("moments", [self.reference, dipole])
 
         if "Molecular Dynamics Iteration" in line:
             self.skip_lines(inputfile, ["d", "ORCA MD", "d", "New Coordinates"])
             line = next(inputfile)
             tokens = line.split()
             assert tokens[0] == "time"
             time = utils.convertor(float(tokens[2]), "time_au", "fs")
@@ -2771,33 +2786,37 @@
                 self.scfvalues[-1].append([deltaE, maxDP, rmsDP])
 
         return
 
     # end of parse_scf_expanded_format
 
     def _append_scfvalues_scftargets(self, inputfile, line):
-        # The SCF convergence targets are always printed after this, but apparently
-        # not all of them always -- for example the RMS Density is missing for geometry
-        # optimization steps. So, assume the previous value is still valid if it is
-        # not found. For additional certainty, assert that the other targets are unchanged.
+        # The SCF convergence targets are always printed in this next section
+        # but which targets are available depends on the SCF method in use,
+        # among other things.
         while not "Last Energy change" in line:
             line = next(inputfile)
+
         deltaE_value = float(line.split()[4])
         deltaE_target = float(line.split()[7])
+        maxDP_value = None
+        rmsDP_value = None
+        maxDP_target = None
+        rmsDP_target = None
+
         line = next(inputfile)
         if "Last MAX-Density change" in line:
             maxDP_value = float(line.split()[4])
             maxDP_target = float(line.split()[7])
             line = next(inputfile)
             if "Last RMS-Density change" in line:
                 rmsDP_value = float(line.split()[4])
                 rmsDP_target = float(line.split()[7])
             else:
-                rmsDP_value = self.scfvalues[-1][-1][2]
-                rmsDP_target = self.scftargets[-1][2]
-                assert deltaE_target == self.scftargets[-1][0]
-                assert maxDP_target == self.scftargets[-1][1]
-            self.scfvalues[-1].append([deltaE_value, maxDP_value, rmsDP_value])
-            self.scftargets.append([deltaE_target, maxDP_target, rmsDP_target])
+                rmsDP_value = None
+                rmsDP_target = None
+
+        self.scfvalues[-1].append([deltaE_value, maxDP_value, rmsDP_value])
+        self.scftargets.append([deltaE_target, maxDP_target, rmsDP_target])
 
 
 _METHODS_SEMIEMPIRICAL = {"AM1", "MNDO", "PM3", "ZINDO/1", "ZINDO/S"}
```

### Comparing `cclib-1.8.1rc2/cclib/parser/psi3parser.py` & `cclib-2.0a1/cclib/parser/psi3parser.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/parser/psi4parser.py` & `cclib-2.0a1/cclib/parser/psi4parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1080,22 +1080,17 @@
                 line = next(inputfile)
 
             n_modes = 0
             # Parse all the Vibration blocks
             while line.strip().startswith("Vibration"):
                 n = len(line.split()) - 1
                 n_modes += n
-                (
-                    vibfreqs_,
-                    vibsyms_,
-                    vibdisps_,
-                    vibrmasses_,
-                    vibfconsts_,
-                    vibirs_,
-                ) = self.parse_vibration(n, inputfile)
+                (vibfreqs_, vibsyms_, vibdisps_, vibrmasses_, vibfconsts_, vibirs_) = (
+                    self.parse_vibration(n, inputfile)
+                )
                 vibfreqs.extend(vibfreqs_)
                 vibsyms.extend(vibsyms_)
                 vibdisps.extend(vibdisps_)
                 vibrmasses.extend(vibrmasses_)
                 vibfconsts.extend(vibfconsts_)
                 vibirs.extend(vibirs_)
                 line = next(inputfile)
```

### Comparing `cclib-1.8.1rc2/cclib/parser/qchemparser.py` & `cclib-2.0a1/cclib/parser/qchemparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -463,17 +463,17 @@
             line = next(inputfile)
             svn_branch = line.split()[3].replace("/", "_")
             if (
                 "package_version" in self.metadata
                 and hasattr(self, "parsed_svn_revision")
                 and not self.parsed_svn_revision
             ):
-                self.metadata[
-                    "package_version"
-                ] = f"{self.metadata['package_version']}dev+{svn_branch}-{svn_revision}"
+                self.metadata["package_version"] = (
+                    f"{self.metadata['package_version']}dev+{svn_branch}-{svn_revision}"
+                )
                 parsed_version = parse_version(self.metadata["package_version"])
                 assert isinstance(parsed_version, Version)
                 self.set_attribute("package_version", parsed_version)
                 self.set_attribute("parsed_svn_revision", True)
 
         # Disable/enable parsing for fragment sections.
         if any(message in line for message in self.fragment_section_headers):
@@ -1323,27 +1323,23 @@
                 #  21 Bu   22 Ag   22 Bu   23 Bu   23 Ag   24 Ag   24 Bu   25 Ag
                 #   0.816
                 #  25 Bu
                 #  --------------------------------------------------------------
 
                 self.skip_line(inputfile, "dashes")
                 line = next(inputfile)
-                (
-                    energies_alpha,
-                    symbols_alpha,
-                    homo_alpha,
-                ) = self.parse_orbital_energies_and_symmetries(inputfile)
+                (energies_alpha, symbols_alpha, homo_alpha) = (
+                    self.parse_orbital_energies_and_symmetries(inputfile)
+                )
                 # Only look at the second block if doing an unrestricted calculation.
                 # This might be a problem for ROHF/ROKS.
                 if self.unrestricted:
-                    (
-                        energies_beta,
-                        symbols_beta,
-                        homo_beta,
-                    ) = self.parse_orbital_energies_and_symmetries(inputfile)
+                    (energies_beta, symbols_beta, homo_beta) = (
+                        self.parse_orbital_energies_and_symmetries(inputfile)
+                    )
 
                 # For now, only keep the last set of MO energies, even though it is
                 # printed at every step of geometry optimizations and fragment jobs.
                 self.set_attribute("moenergies", [numpy.array(energies_alpha)])
                 self.set_attribute("homos", [homo_alpha])
                 self.set_attribute("mosyms", [symbols_alpha])
                 if self.unrestricted:
```

### Comparing `cclib-1.8.1rc2/cclib/parser/turbomoleparser.py` & `cclib-2.0a1/cclib/parser/turbomoleparser.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/parser/utils.py` & `cclib-2.0a1/cclib/attribute_parsers/utils.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/parser/xtbparser.py` & `cclib-2.0a1/cclib/parser/xtbparser.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/progress/textprogress.py` & `cclib-2.0a1/cclib/progress/textprogress.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/scripts/ccframe.py` & `cclib-2.0a1/cclib/scripts/ccframe.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/scripts/ccget.py` & `cclib-2.0a1/cclib/scripts/ccget.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (c) 2024, the cclib development team
 #
 # This file is part of cclib (http://cclib.github.io) and is distributed under
 # the terms of the BSD 3-Clause License.
 
 """Script for loading data from computational chemistry files."""
 
-
 import difflib
 import glob
 import logging
 import os.path
 
 # This is needed for testing purposes only.
 import sys
```

### Comparing `cclib-1.8.1rc2/cclib/scripts/ccwrite.py` & `cclib-2.0a1/cclib/scripts/ccwrite.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib/scripts/cda.py` & `cclib-2.0a1/cclib/scripts/cda.py`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/cclib.egg-info/PKG-INFO` & `cclib-2.0a1/cclib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cclib
-Version: 1.8.1rc2
+Version: 2.0a1
 Summary: parsers and algorithms for computational chemistry
 Author-email: cclib development team <cclib@googlegroups.com>
 Maintainer-email: cclib development team <cclib@googlegroups.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, the cclib development team
         All rights reserved.
@@ -75,15 +75,15 @@
 Requires-Dist: cclib[bridges]; extra == "all"
 
 ### cclib
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8280878.svg)](https://doi.org/10.5281/zenodo.8280878)
 [![PyPI version](http://img.shields.io/pypi/v/cclib.svg?style=flat)](https://pypi.python.org/pypi/cclib)
 [![GitHub release](https://img.shields.io/github/release/cclib/cclib.svg?style=flat)](https://github.com/cclib/cclib/releases)
-[![build status](https://github.com/cclib/cclib/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/cclib/cclib/actions/workflows/cclib_pytest.yml)
+[![build status](https://github.com/cclib/cclib/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/cclib/cclib/actions/workflows/ci.yml)
 [![license](http://img.shields.io/badge/license-BSD-blue.svg?style=flat)](https://github.com/cclib/cclib/blob/master/LICENSE)
 
 <img src="./logo.png" alt="cclib logo" width="100" />
 
 cclib is a Python library that provides parsers for output files of computational chemistry packages. It also provides a platform for computational chemists to implement algorithms in a platform-independent way.
 
 For more information, go to [https://cclib.github.io](https://cclib.github.io). There is a mailing list for questions at https://groups.google.com/g/cclib.
```

### Comparing `cclib-1.8.1rc2/pyproject.toml` & `cclib-2.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cclib-1.8.1rc2/tools/versioningit_override.py` & `cclib-2.0a1/tools/versioningit_override.py`

 * *Files identical despite different names*

