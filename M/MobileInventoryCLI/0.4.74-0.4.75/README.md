# Comparing `tmp/MobileInventoryCLI-0.4.74.tar.gz` & `tmp/MobileInventoryCLI-0.4.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MobileInventoryCLI-0.4.74.tar", last modified: Mon Apr 29 15:58:51 2024, max compression
+gzip compressed data, was "MobileInventoryCLI-0.4.75.tar", last modified: Tue Apr 30 13:02:50 2024, max compression
```

## Comparing `MobileInventoryCLI-0.4.74.tar` & `MobileInventoryCLI-0.4.75.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-29 15:58:51.467644 MobileInventoryCLI-0.4.74/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-29 15:58:51.447644 MobileInventoryCLI-0.4.74/MobileInventoryCLI/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-29 15:58:51.447644 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-29 15:58:51.450977 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-29 15:58:51.454311 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
--rw-r--r--   0 carl      (1000) carl      (1000)    38216 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-29 15:58:51.454311 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
--rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-29 15:58:51.454311 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
--rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-29 15:58:51.454311 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
--rw-r--r--   0 carl      (1000) carl      (1000)     9817 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
--rw-r--r--   0 carl      (1000) carl      (1000)     4937 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   108165 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
--rw-r--r--   0 carl      (1000) carl      (1000)      310 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/testClass.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-29 15:58:51.457644 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
--rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-29 15:58:51.457644 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
--rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-29 15:58:51.457644 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
--rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-29 15:58:51.457644 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
--rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-29 15:58:51.457644 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
--rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-29 15:58:51.457644 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
--rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
--rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-29 15:58:51.457644 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)     6098 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-29 15:58:51.460977 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
--rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-29 15:58:51.460977 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
--rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-29 15:58:51.460977 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
--rw-r--r--   0 carl      (1000) carl      (1000)     3078 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py
--rw-r--r--   0 carl      (1000) carl      (1000)    17392 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)    21197 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-29 15:58:51.460977 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
--rw-r--r--   0 carl      (1000) carl      (1000)    78957 2024-04-29 15:57:24.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-29 15:58:51.460977 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
--rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-29 15:58:51.460977 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
--rw-r--r--   0 carl      (1000) carl      (1000)    28428 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-29 15:58:51.460977 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/
--rw-r--r--   0 carl      (1000) carl      (1000)     1191 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-29 15:58:44.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2249 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     5767 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
--rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-29 15:58:51.460977 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
--rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-29 15:58:51.464311 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
--rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-29 15:58:51.464311 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1042 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-29 15:58:51.464311 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/collected/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/collected/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/dbpath.config
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-29 15:58:51.464311 MobileInventoryCLI-0.4.74/MobileInventoryCLI/error/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/error/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/error/error.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-29 15:58:51.464311 MobileInventoryCLI-0.4.74/MobileInventoryCLI/lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/lookup/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/lookup/lookup.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-29 15:58:51.464311 MobileInventoryCLI-0.4.74/MobileInventoryCLI/mainloop/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/mainloop/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/mainloop/mainloop.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-29 15:58:51.464311 MobileInventoryCLI-0.4.74/MobileInventoryCLI/updateCfg/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/updateCfg/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-28 17:22:29.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI/updateCfg/updateCfg.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-29 15:58:51.464311 MobileInventoryCLI-0.4.74/MobileInventoryCLI.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-04-29 15:58:51.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)     5356 2024-04-29 15:58:51.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI.egg-info/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-29 15:58:51.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-04-29 15:58:51.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-29 15:58:51.000000 MobileInventoryCLI-0.4.74/MobileInventoryCLI.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-04-29 15:58:51.464311 MobileInventoryCLI-0.4.74/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-29 15:58:51.467644 MobileInventoryCLI-0.4.74/setup.cfg
--rw-r--r--   0 carl      (1000) carl      (1000)      956 2024-04-29 15:58:50.000000 MobileInventoryCLI-0.4.74/setup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 13:02:50.140559 MobileInventoryCLI-0.4.75/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 13:02:50.120559 MobileInventoryCLI-0.4.75/MobileInventoryCLI/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 13:02:50.123892 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 13:02:50.127225 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 13:02:50.127225 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
+-rw-r--r--   0 carl      (1000) carl      (1000)    38216 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 13:02:50.127225 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 13:02:50.127225 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 13:02:50.130559 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
+-rw-r--r--   0 carl      (1000) carl      (1000)     9817 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     4937 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   108165 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      310 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/testClass.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 13:02:50.130559 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 13:02:50.130559 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 13:02:50.130559 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
+-rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 13:02:50.130559 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 13:02:50.130559 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 13:02:50.133892 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 13:02:50.133892 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6122 2024-04-30 12:48:33.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 13:02:50.133892 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 13:02:50.133892 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
+-rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 13:02:50.133892 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3078 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    17392 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    21197 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 13:02:50.133892 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
+-rw-r--r--   0 carl      (1000) carl      (1000)    79222 2024-04-30 13:01:42.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 13:02:50.133892 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
+-rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 13:02:50.133892 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
+-rw-r--r--   0 carl      (1000) carl      (1000)    28428 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 13:02:50.137225 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1191 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-30 13:02:43.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2249 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     5767 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 13:02:50.137225 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 13:02:50.137225 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 13:02:50.137225 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1042 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 13:02:50.137225 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/collected/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/collected/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/dbpath.config
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 13:02:50.137225 MobileInventoryCLI-0.4.75/MobileInventoryCLI/error/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/error/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/error/error.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 13:02:50.137225 MobileInventoryCLI-0.4.75/MobileInventoryCLI/lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/lookup/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/lookup/lookup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 13:02:50.137225 MobileInventoryCLI-0.4.75/MobileInventoryCLI/mainloop/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/mainloop/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/mainloop/mainloop.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 13:02:50.140559 MobileInventoryCLI-0.4.75/MobileInventoryCLI/updateCfg/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/updateCfg/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-29 15:59:03.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI/updateCfg/updateCfg.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-30 13:02:50.140559 MobileInventoryCLI-0.4.75/MobileInventoryCLI.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-04-30 13:02:50.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)     5356 2024-04-30 13:02:50.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI.egg-info/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-30 13:02:50.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-04-30 13:02:50.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-30 13:02:50.000000 MobileInventoryCLI-0.4.75/MobileInventoryCLI.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-04-30 13:02:50.140559 MobileInventoryCLI-0.4.75/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-30 13:02:50.140559 MobileInventoryCLI-0.4.75/setup.cfg
+-rw-r--r--   0 carl      (1000) carl      (1000)      956 2024-04-30 13:02:49.000000 MobileInventoryCLI-0.4.75/setup.py
```

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,14 +157,14 @@
 				print(f"{Fore.green}{Style.underline}Lookup Initialized...{Style.reset}")
 				if code.lower() in self.cmds['1']['cmds']:
 					self.cmds['1']['exec']()
 				elif code.lower() in self.cmds['2']['cmds']:
 					break
 				else:
 					with Session(self.engine) as session:	
-						query=session.query(Entry).filter(or_(Entry.Barcode==code,Entry.Code==code))
+						query=session.query(Entry).filter(or_(Entry.Barcode==code,Entry.Code==code,Entry.ALT_Barcode==code))
 						results=query.all()
 						for num,r in enumerate(results):
 							print(f'{Fore.red}{num}{Style.reset}/{Fore.green}{len(results)}{Style.reset} -> {r}')
 						print(f"{Fore.cyan}There were {Fore.green}{Style.bold}{len(results)}{Style.reset} {Fore.cyan}results.{Style.reset}")
 			except Exception as e:
 				print(e)
```

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 from datetime import *
 from colored import Style,Fore
 import json,sys
 
 class TasksMode:
     #extra is for future expansion
     def exportList2Excel(self,fields=False,extra=[]):
-        FIELDS=['Barcode','Code','Name','Price','CaseCount']
+        FIELDS=['Barcode','ALT_Barcode','Code','Name','Price','CaseCount']
         cols=[i.name for i in Entry.__table__.columns]
         if fields == True:
             return FIELDS
         for i in extra:
             if i in cols:
                 FIELDS.append(extra)
             else:
                 print(f"{Fore.light_red}{Style.bold}Warning {Style.underline}{Style.reset}{Fore.light_yellow}'{i}' from extra={extra} is not a valid {Style.reset}{Fore.light_green}Field|Column!{Style.reset}")
        
         with Session(self.engine) as session:
             query=session.query(Entry).filter(Entry.InList==True)
             df = pd.read_sql(query.statement, query.session.bind)
-            df=df[['Barcode','Code','Name','Price','CaseCount']]
+            df=df[['Barcode','ALT_Barcode','Code','Name','Price','CaseCount']]
             #df.to_excel()
             def mkT(text,self):
                 if text=='':
                     return 'InList-Export.xlsx'
                 return text
             while True:
                 try:
@@ -50,15 +50,15 @@
             def mkT(text,self):
                 return text
             scanned=Prompt.__init2__(None,func=mkT,ptext='barcode|code[help]?',helpText='',data=self)
             if not scanned:
                 break
             else:
                 with Session(self.engine) as session:
-                    result=session.query(Entry).filter(or_(Entry.Barcode==scanned,Entry.Code==scanned),Entry.InList==True).first()
+                    result=session.query(Entry).filter(or_(Entry.Barcode==scanned,Entry.Code==scanned,Entry.ALT_Barcode==scanned),Entry.InList==True).first()
                     if result:
                         backroom=result.BackRoom
                         total=0
                         for f in self.valid_fields:
                             if f not in self.special:
                                 if getattr(result,f) not in [None,'']:
                                     total+=float(getattr(result,f))
@@ -101,15 +101,15 @@
             
 
     def display_field(self,fieldname,load=False,above=None,below=None):
         color1=Fore.red
         color2=Fore.yellow
         color3=Fore.cyan
         color4=Fore.green_yellow
-        m=f"Item Num |Name|Barcode|Code|{fieldname}|EID"
+        m=f"Item Num |Name|Barcode|ALT_Barcode|Code|{fieldname}|EID"
         hr='-'*len(m)
         print(f"{m}\n{hr}")
         if (fieldname in self.valid_fields) or (load == True and fieldname == 'ListQty'):
             with Session(self.engine) as session:
                 query=session.query(Entry).filter(Entry.InList==True)
                 if above == None:
                     def mkT(text,self):
@@ -134,15 +134,15 @@
                     query=query.filter(getattr(Entry,fieldname)>above)
                 if below != None:
                     query=query.filter(getattr(Entry,fieldname)<below)
                 results=query.all()
                 if len(results) < 1:
                     print(f"{Fore.red}{Style.bold}Nothing is in List!{Style.reset}")
                 for num,result in enumerate(results):
-                    print(f"{Fore.red}{num}{Style.reset} -> {color1}{result.Name}{Style.reset}|{color2}{result.Barcode}{Style.reset}|{color3}{result.Code}{Style.reset}|{color4}{getattr(result,fieldname)}{Style.reset}|{Fore.yellow}{getattr(result,'EntryId')}{Style.reset}")
+                    print(f"{Fore.red}{num}{Style.reset} -> {color1}{result.Name}{Style.reset}|{color2}{result.Barcode}|{result.ALT_Barcode}{Style.reset}|{color3}{result.Code}{Style.reset}|{color4}{getattr(result,fieldname)}{Style.reset}|{Fore.yellow}{getattr(result,'EntryId')}{Style.reset}")
         print(f"{m}\n{hr}")
 
     def SearchAuto(self,InList=None,skipReturn=False):
         while True:
             try:
                 with Session(self.engine) as session:
                     def mkT(text,self):
@@ -210,15 +210,15 @@
                 print(e)
 
 
     def setFieldInList(self,fieldname,load=False):
         tmp_fieldname=fieldname
         while True:
             if (fieldname not in self.special or fieldname in ['Facings'] )or (load==True and fieldname in ['ListQty',]):
-                m=f"Item Num |Name|Barcode|Code|{fieldname}|EID"
+                m=f"Item Num |Name|Barcode|ALT_Barcode|Code|{fieldname}|EID"
                 hr='-'*len(m)
                 if (fieldname in self.valid_fields) or (load==True and fieldname in ['ListQty',]) or fieldname == None:
                     with Session(self.engine) as session:
                         code=''
                         
                         def mkT(text,self):
                             return str(text)
@@ -278,29 +278,29 @@
                             while True:
                                 fieldname=Prompt.__init2__(None,func=mkfields,ptext="Location Field(see h|help)",helpText=hstring,data=self)
                                 if fieldname in [None,]:
                                     break
                                 break
                             if fieldname in [None,]:
                                 continue
-                            m=f"Item Num |Name|Barcode|Code|{fieldname}|EID"
+                            m=f"Item Num |Name|Barcode|ALT_Barcode|Code|{fieldname}|EID"
                             hr='-'*len(m)
 
                         p=Prompt.__init2__(None,func=mkT,ptext="amount|+amount|-amount",helpText=self.helpText_barcodes,data=self)
                         if p:
                             value,text,suffix=p
                         else:
                             continue
                         try:
                             color1=Fore.red
                             color2=Fore.yellow
                             color3=Fore.cyan
                             color4=Fore.green_yellow 
                             if text.startswith("-") or text.startswith("+"):
-                                result=session.query(Entry).filter(or_(Entry.Barcode==code,Entry.Code==code)).first()
+                                result=session.query(Entry).filter(or_(Entry.Barcode==code,Entry.Code==code,ENtry.ALT_Barcode==code)).first()
                                 if result:
                                     if suffix.lower() in ['c',]:
                                         if result.CaseCount in [None,]:
                                             result.CaseCount=1
                                             session.commit()
                                             session.flush()
                                             session.refresh(result)
@@ -311,27 +311,27 @@
                                             session.refresh(result)
                                         value=float(value)*result.CaseCount
                                     setattr(result,fieldname,getattr(result,fieldname)+float(value))
                                     result.InList=True
                                     session.commit()
                                     session.flush()
                                     session.refresh(result)
-                                    print(f"{Fore.red}0{Style.reset} -> {color1}{result.Name}{Style.reset}|{color2}{result.Barcode}{Style.reset}|{color3}{result.Code}{Style.reset}|{color4}{getattr(result,fieldname)}{Style.reset}|{color4}{getattr(result,'EntryId')}{Style.reset}")
+                                    print(f"{Fore.red}0{Style.reset} -> {color1}{result.Name}{Style.reset}|{color2}{result.Barcode}|{result.ALT_Barcode}{Style.reset}|{color3}{result.Code}{Style.reset}|{color4}{getattr(result,fieldname)}{Style.reset}|{color4}{getattr(result,'EntryId')}{Style.reset}")
                                     print(f"{m}\n{hr}")
                                 else:
                                     replacement=self.SearchAuto()
                                     if isinstance(replacement,int):
                                         result=session.query(Entry).filter(Entry.EntryId==replacement).first()
                                         if result:
                                             setattr(result,fieldname,getattr(result,fieldname)+float(value))
                                             result.InList=True
                                             session.commit()
                                             session.flush()
                                             session.refresh(result)
-                                            print(f"{Fore.red}0{Style.reset} -> {color1}{result.Name}{Style.reset}|{color2}{result.Barcode}{Style.reset}|{color3}{result.Code}{Style.reset}|{color4}{getattr(result,fieldname)}{Style.reset}|{color4}{getattr(result,'EntryId')}{Style.reset}")
+                                            print(f"{Fore.red}0{Style.reset} -> {color1}{result.Name}{Style.reset}|{color2}{result.Barcode}|{result.ALT_Barcode}{Style.reset}|{color3}{result.Code}{Style.reset}|{color4}{getattr(result,fieldname)}{Style.reset}|{color4}{getattr(result,'EntryId')}{Style.reset}")
                                             print(f"{m}\n{hr}")
                                         else:
                                             raise Exception(f"result is {result}")
                                     else:
                                         name=code
                                         while True:
                                             try:
@@ -385,19 +385,19 @@
                                         n=Entry(Barcode=code,Code=icode,Price=iprice,Name=name,CaseCount=icc,InList=True,Note="New Item")
                                         setattr(n,fieldname,value)
                                         session.add(n)
                                         session.commit()
                                         session.flush()
                                         session.refresh(n)
                                         result=n
-                                        print(f"{Fore.red}0{Style.reset} -> {color1}{result.Name}{Style.reset}|{color2}{result.Barcode}{Style.reset}|{color3}{result.Code}{Style.reset}|{color4}{getattr(result,fieldname)}{Style.reset}|{color4}{getattr(result,'EntryId')}{Style.reset}")
+                                        print(f"{Fore.red}0{Style.reset} -> {color1}{result.Name}{Style.reset}|{color2}{result.Barcode}|{result.ALT_Barcode}{Style.reset}|{color3}{result.Code}{Style.reset}|{color4}{getattr(result,fieldname)}{Style.reset}|{color4}{getattr(result,'EntryId')}{Style.reset}")
 
                                         print(f"{m}\n{hr}")
                             else:
-                                result=session.query(Entry).filter(or_(Entry.Barcode==code,Entry.Code==code)).first()
+                                result=session.query(Entry).filter(or_(Entry.Barcode==code,Entry.Code==code,Entry.ALT_Barcode==code)).first()
                                 if result:
                                     if suffix.lower() in ['c',]:
                                         if result.CaseCount in [None,]:
                                             result.CaseCount=1
                                             session.commit()
                                             session.flush()
                                             session.refresh(result)
@@ -408,29 +408,29 @@
                                             session.refresh(result)
                                         value=float(value)*result.CaseCount
                                     setattr(result,fieldname,value)
                                     result.InList=True
                                     session.commit()
                                     session.flush()
                                     session.refresh(result)
-                                    print(f"{Fore.red}0{Style.reset} -> {color1}{result.Name}{Style.reset}|{color2}{result.Barcode}{Style.reset}|{color3}{result.Code}{Style.reset}|{color4}{getattr(result,fieldname)}{Style.reset}|{color4}{getattr(result,'EntryId')}{Style.reset}")
+                                    print(f"{Fore.red}0{Style.reset} -> {color1}{result.Name}{Style.reset}|{color2}{result.Barcode}|{result.ALT_Barcode}{Style.reset}|{color3}{result.Code}{Style.reset}|{color4}{getattr(result,fieldname)}{Style.reset}|{color4}{getattr(result,'EntryId')}{Style.reset}")
 
                                     print(f"{m}\n{hr}")
 
                                 else:
                                     replacement=self.SearchAuto()
                                     if isinstance(replacement,int):
                                         result=session.query(Entry).filter(Entry.EntryId==replacement).first()
                                         if result:
                                             setattr(result,fieldname,getattr(result,fieldname)+float(value))
                                             result.InList=True
                                             session.commit()
                                             session.flush()
                                             session.refresh(result)
-                                            print(f"{Fore.red}0{Style.reset} -> {color1}{result.Name}{Style.reset}|{color2}{result.Barcode}{Style.reset}|{color3}{result.Code}{Style.reset}|{color4}{getattr(result,fieldname)}{Style.reset}|{color4}{getattr(result,'EntryId')}{Style.reset}")
+                                            print(f"{Fore.red}0{Style.reset} -> {color1}{result.Name}{Style.reset}|{color2}{result.Barcode}|{result.ALT_Barcode}{Style.reset}|{color3}{result.Code}{Style.reset}|{color4}{getattr(result,fieldname)}{Style.reset}|{color4}{getattr(result,'EntryId')}{Style.reset}")
                                             print(f"{m}\n{hr}")
                                         else:
                                             raise Exception(f"result is {result}")
                                     else:
                                         name=code
                                         while True:
                                             try:
```

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/__init__.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/__init__.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/lookup/lookup.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/lookup/lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/mainloop/mainloop.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/mainloop/mainloop.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI/updateCfg/updateCfg.py` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI/updateCfg/updateCfg.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI.egg-info/PKG-INFO` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.74
+Version: 0.4.75
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Android
```

### Comparing `MobileInventoryCLI-0.4.74/MobileInventoryCLI.egg-info/SOURCES.txt` & `MobileInventoryCLI-0.4.75/MobileInventoryCLI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.74/PKG-INFO` & `MobileInventoryCLI-0.4.75/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.74
+Version: 0.4.75
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Android
```

### Comparing `MobileInventoryCLI-0.4.74/setup.py` & `MobileInventoryCLI-0.4.75/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 from datetime import datetime
-version='0.4.74'
+version='0.4.75'
 
 setup(name='MobileInventoryCLI',
       version=version,
       author="Carl Joseph Hirner III",
       author_email="k.j.hirner.wisdom@gmail.com",
       description="modify/update/use MobileInventoryPro *.bck files",
       classifiers=[
```

