# Comparing `tmp/SRPAstro.FITS-3.0.1.tar.gz` & `tmp/srpastro_fits-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SRPAstro.FITS-3.0.1.tar", last modified: Mon May 22 10:07:50 2023, max compression
+gzip compressed data, was "srpastro_fits-3.0.3.tar", last modified: Tue Apr 30 14:08:33 2024, max compression
```

## Comparing `SRPAstro.FITS-3.0.1.tar` & `srpastro_fits-3.0.3.tar`

### file list

```diff
@@ -1,167 +1,167 @@
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:50.568093 SRPAstro.FITS-3.0.1/
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.798141 SRPAstro.FITS-3.0.1/Docs/
--rw-------   0 covino     (501) staff       (20)   142337 2017-02-21 14:33:07.000000 SRPAstro.FITS-3.0.1/Docs/SRPAstro.FITS.pdf
--rw-r--r--   0 covino     (501) staff       (20)     1081 2019-05-07 09:54:08.000000 SRPAstro.FITS-3.0.1/LICENSE.txt
--rw-r--r--   0 covino     (501) staff       (20)      258 2020-03-04 14:45:54.000000 SRPAstro.FITS-3.0.1/MANIFEST.in
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.156475 SRPAstro.FITS-3.0.1/Misc/
--rw-------   0 covino     (501) staff       (20)     1288 2019-05-22 19:31:58.000000 SRPAstro.FITS-3.0.1/Misc/ApyPhot.py
--rw-------   0 covino     (501) staff       (20)    23044 2021-02-02 11:59:14.000000 SRPAstro.FITS-3.0.1/Misc/AstrometryClass.py
--rw-r--r--   0 covino     (501) staff       (20)     1507 2023-05-22 10:07:50.568275 SRPAstro.FITS-3.0.1/PKG-INFO
--rw-r--r--   0 covino     (501) staff       (20)      744 2019-07-22 12:26:27.000000 SRPAstro.FITS-3.0.1/README.md
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.886749 SRPAstro.FITS-3.0.1/SRPAstro.FITS.egg-info/
--rw-------   0 covino     (501) staff       (20)     1507 2023-05-22 10:07:49.000000 SRPAstro.FITS-3.0.1/SRPAstro.FITS.egg-info/PKG-INFO
--rw-------   0 covino     (501) staff       (20)     6615 2023-05-22 10:07:49.000000 SRPAstro.FITS-3.0.1/SRPAstro.FITS.egg-info/SOURCES.txt
--rw-------   0 covino     (501) staff       (20)        1 2023-05-22 10:07:49.000000 SRPAstro.FITS-3.0.1/SRPAstro.FITS.egg-info/dependency_links.txt
--rw-------   0 covino     (501) staff       (20)       62 2023-05-22 10:07:49.000000 SRPAstro.FITS-3.0.1/SRPAstro.FITS.egg-info/requires.txt
--rw-------   0 covino     (501) staff       (20)        8 2023-05-22 10:07:49.000000 SRPAstro.FITS-3.0.1/SRPAstro.FITS.egg-info/top_level.txt
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.209299 SRPAstro.FITS-3.0.1/SRPFITS/
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.887494 SRPAstro.FITS-3.0.1/SRPFITS/Data/
--rw-r--r--   0 covino     (501) staff       (20)     8196 2020-03-04 14:48:58.000000 SRPAstro.FITS-3.0.1/SRPFITS/Data/.DS_Store
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.943726 SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/
--rw-------   0 covino     (501) staff       (20)       88 2010-09-28 13:27:42.000000 SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPConvIn
--rw-------   0 covino     (501) staff       (20)      332 2010-09-28 13:33:03.000000 SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPConvLSLASCIn
--rw-------   0 covino     (501) staff       (20)     2165 2010-09-28 13:30:00.000000 SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPNnwIn
--rw-------   0 covino     (501) staff       (20)      179 2013-12-06 14:18:19.000000 SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPParamIn
--rw-------   0 covino     (501) staff       (20)      750 2010-09-28 13:31:35.000000 SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPSexIn
--rw-------   0 covino     (501) staff       (20)      749 2010-09-28 13:33:53.000000 SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPSexLSLASCIn
--rw-------   0 covino     (501) staff       (20)      752 2012-01-25 16:07:42.000000 SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPSexREMREMIRIn
--rw-------   0 covino     (501) staff       (20)      750 2013-08-18 20:17:05.000000 SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPSexREMROS2In
--rw-------   0 covino     (501) staff       (20)      751 2012-04-01 19:58:22.000000 SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPSexREMROSSIn
--rw-------   0 covino     (501) staff       (20)      750 2010-09-28 13:53:56.000000 SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPSexTNGLRSIn
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.326117 SRPAstro.FITS-3.0.1/SRPFITS/Fits/
--rw-------   0 covino     (501) staff       (20)     1930 2017-05-18 14:30:00.000000 SRPAstro.FITS-3.0.1/SRPFITS/Fits/AddHeaderComment.py
--rw-------   0 covino     (501) staff       (20)     2612 2021-07-08 08:39:43.000000 SRPAstro.FITS-3.0.1/SRPFITS/Fits/AddHeaderEntry.py
--rw-------   0 covino     (501) staff       (20)     1967 2015-07-23 12:13:33.000000 SRPAstro.FITS-3.0.1/SRPFITS/Fits/FitsConstants.py
--rw-------   0 covino     (501) staff       (20)     8608 2021-03-02 15:35:24.000000 SRPAstro.FITS-3.0.1/SRPFITS/Fits/FitsImageClass.py
--rw-------   0 covino     (501) staff       (20)      869 2015-07-23 12:13:58.000000 SRPAstro.FITS-3.0.1/SRPFITS/Fits/FitsTabsAppend.py
--rw-------   0 covino     (501) staff       (20)      760 2017-05-18 14:34:24.000000 SRPAstro.FITS-3.0.1/SRPFITS/Fits/GetData.py
--rw-------   0 covino     (501) staff       (20)      802 2017-05-18 14:35:11.000000 SRPAstro.FITS-3.0.1/SRPFITS/Fits/GetHeader.py
--rw-------   0 covino     (501) staff       (20)      875 2017-05-18 14:35:28.000000 SRPAstro.FITS-3.0.1/SRPFITS/Fits/GetHeaderValue.py
--rw-------   0 covino     (501) staff       (20)      997 2017-05-18 13:39:55.000000 SRPAstro.FITS-3.0.1/SRPFITS/Fits/GetSpectrum.py
--rw-------   0 covino     (501) staff       (20)      586 2015-07-23 12:34:36.000000 SRPAstro.FITS-3.0.1/SRPFITS/Fits/GetSpectrumPosition.py
--rw-------   0 covino     (501) staff       (20)     1424 2021-02-09 12:48:15.000000 SRPAstro.FITS-3.0.1/SRPFITS/Fits/GetWCS.py
--rw-------   0 covino     (501) staff       (20)      702 2017-08-22 21:04:15.000000 SRPAstro.FITS-3.0.1/SRPFITS/Fits/IsFits.py
--rw-------   0 covino     (501) staff       (20)      437 2021-01-14 10:07:28.000000 SRPAstro.FITS-3.0.1/SRPFITS/Fits/WCSPixelScale.py
--rw-------   0 covino     (501) staff       (20)      567 2021-01-14 10:40:27.000000 SRPAstro.FITS-3.0.1/SRPFITS/Fits/WCSRotationDeg.py
--rw-------   0 covino     (501) staff       (20)      799 2022-08-10 13:01:02.000000 SRPAstro.FITS-3.0.1/SRPFITS/Fits/__init__.py
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.483192 SRPAstro.FITS-3.0.1/SRPFITS/Frames/
--rw-------   0 covino     (501) staff       (20)    24425 2021-03-17 08:46:10.000000 SRPAstro.FITS-3.0.1/SRPFITS/Frames/AstrometryClass.py
--rw-------   0 covino     (501) staff       (20)     2810 2021-03-02 15:30:39.000000 SRPAstro.FITS-3.0.1/SRPFITS/Frames/DAOObjectClass.py
--rw-------   0 covino     (501) staff       (20)      425 2015-07-23 12:15:58.000000 SRPAstro.FITS-3.0.1/SRPFITS/Frames/EclipseConstants.py
--rw-------   0 covino     (501) staff       (20)     2636 2017-05-16 09:56:28.000000 SRPAstro.FITS-3.0.1/SRPFITS/Frames/EclipseObjectClass.py
--rw-------   0 covino     (501) staff       (20)      853 2020-05-14 16:28:39.000000 SRPAstro.FITS-3.0.1/SRPFITS/Frames/Pixel2WCS.py
--rw-------   0 covino     (501) staff       (20)     1394 2020-05-14 13:44:46.000000 SRPAstro.FITS-3.0.1/SRPFITS/Frames/SExtractorConstants.py
--rw-------   0 covino     (501) staff       (20)      361 2015-07-23 12:16:42.000000 SRPAstro.FITS-3.0.1/SRPFITS/Frames/SexConstants.py
--rw-------   0 covino     (501) staff       (20)     2562 2020-12-11 12:24:32.000000 SRPAstro.FITS-3.0.1/SRPFITS/Frames/SexObjectClass.py
--rw-------   0 covino     (501) staff       (20)     5248 2017-05-26 14:52:54.000000 SRPAstro.FITS-3.0.1/SRPFITS/Frames/SourceObjectsClass.py
--rw-------   0 covino     (501) staff       (20)      865 2020-05-14 14:24:01.000000 SRPAstro.FITS-3.0.1/SRPFITS/Frames/WCS2Pixel.py
--rw-------   0 covino     (501) staff       (20)      588 2017-05-16 09:52:29.000000 SRPAstro.FITS-3.0.1/SRPFITS/Frames/__init__.py
--rw-------   0 covino     (501) staff       (20)      637 2020-03-07 14:00:40.000000 SRPAstro.FITS-3.0.1/SRPFITS/Frames/getCenterRADEC.py
--rw-------   0 covino     (501) staff       (20)     1086 2023-05-22 09:48:40.000000 SRPAstro.FITS-3.0.1/SRPFITS/GetFWHM.py
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.525095 SRPAstro.FITS-3.0.1/SRPFITS/Math/
--rw-------   0 covino     (501) staff       (20)     8163 2021-07-06 13:46:23.000000 SRPAstro.FITS-3.0.1/SRPFITS/Math/TriangleMatch.py
--rw-------   0 covino     (501) staff       (20)      331 2017-03-14 08:48:57.000000 SRPAstro.FITS-3.0.1/SRPFITS/Math/__init__.py
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.598386 SRPAstro.FITS-3.0.1/SRPFITS/Photometry/
--rw-------   0 covino     (501) staff       (20)     1126 2017-04-19 13:53:05.000000 SRPAstro.FITS-3.0.1/SRPFITS/Photometry/ApErr.py
--rw-------   0 covino     (501) staff       (20)     2903 2020-10-05 08:41:16.000000 SRPAstro.FITS-3.0.1/SRPFITS/Photometry/ApyPhot.py
--rw-------   0 covino     (501) staff       (20)      520 2015-12-11 15:46:16.000000 SRPAstro.FITS-3.0.1/SRPFITS/Photometry/Counts2Mag.py
--rw-------   0 covino     (501) staff       (20)      884 2017-08-30 19:36:03.000000 SRPAstro.FITS-3.0.1/SRPFITS/Photometry/DaoPhot.py
--rw-------   0 covino     (501) staff       (20)     5146 2023-05-22 10:06:44.000000 SRPAstro.FITS-3.0.1/SRPFITS/Photometry/FitsPhotometryClass.py
--rw-------   0 covino     (501) staff       (20)      503 2015-07-23 12:26:20.000000 SRPAstro.FITS-3.0.1/SRPFITS/Photometry/Mag2Counts.py
--rw-------   0 covino     (501) staff       (20)     1086 2015-11-13 14:11:34.000000 SRPAstro.FITS-3.0.1/SRPFITS/Photometry/MinMax.py
--rw-------   0 covino     (501) staff       (20)      849 2022-08-10 13:00:32.000000 SRPAstro.FITS-3.0.1/SRPFITS/Photometry/__init__.py
--rw-------   0 covino     (501) staff       (20)     1142 2017-04-19 13:45:07.000000 SRPAstro.FITS-3.0.1/SRPFITS/Photometry/centerGauss.py
--rw-------   0 covino     (501) staff       (20)     1653 2020-03-07 16:49:45.000000 SRPAstro.FITS-3.0.1/SRPFITS/Photometry/centerMoment.py
--rw-------   0 covino     (501) staff       (20)     1563 2017-08-24 08:53:55.000000 SRPAstro.FITS-3.0.1/SRPFITS/Photometry/centerObj.py
--rw-------   0 covino     (501) staff       (20)     1281 2015-11-13 10:37:46.000000 SRPAstro.FITS-3.0.1/SRPFITS/Photometry/getBackground.py
--rw-------   0 covino     (501) staff       (20)      803 2015-11-10 10:11:17.000000 SRPAstro.FITS-3.0.1/SRPFITS/Photometry/resid.py
--rw-------   0 covino     (501) staff       (20)      521 2021-06-02 20:51:07.000000 SRPAstro.FITS-3.0.1/SRPFITS/SRPFITSPath.py
--rw-------   0 covino     (501) staff       (20)     2481 2023-05-22 09:48:36.000000 SRPAstro.FITS-3.0.1/SRPFITS/__init__.py
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:50.539089 SRPAstro.FITS-3.0.1/Scripts/
--rw-------   0 covino     (501) staff       (20)    10932 2021-09-07 09:46:26.000000 SRPAstro.FITS-3.0.1/Scripts/SRPAdvAverage
--rw-------   0 covino     (501) staff       (20)     5242 2021-05-12 11:29:46.000000 SRPAstro.FITS-3.0.1/Scripts/SRPAlignImaging
--rw-------   0 covino     (501) staff       (20)    10433 2021-05-12 11:29:59.000000 SRPAstro.FITS-3.0.1/Scripts/SRPAstrometry
--rw-------   0 covino     (501) staff       (20)     5660 2021-05-12 11:30:11.000000 SRPAstro.FITS-3.0.1/Scripts/SRPAverage
--rw-------   0 covino     (501) staff       (20)     6023 2021-11-16 10:55:28.000000 SRPAstro.FITS-3.0.1/Scripts/SRPBias
--rw-------   0 covino     (501) staff       (20)     3831 2021-05-12 11:30:35.000000 SRPAstro.FITS-3.0.1/Scripts/SRPClassify
--rw-------   0 covino     (501) staff       (20)     7083 2021-05-12 11:30:47.000000 SRPAstro.FITS-3.0.1/Scripts/SRPCut
--rw-------   0 covino     (501) staff       (20)     8464 2021-05-12 11:30:59.000000 SRPAstro.FITS-3.0.1/Scripts/SRPDao2Sky
--rw-------   0 covino     (501) staff       (20)      800 2021-05-12 11:32:34.000000 SRPAstro.FITS-3.0.1/Scripts/SRPFITSVersion
--rw-------   0 covino     (501) staff       (20)     4492 2021-05-12 11:31:10.000000 SRPAstro.FITS-3.0.1/Scripts/SRPFindingChart
--rw-------   0 covino     (501) staff       (20)     3692 2021-05-12 11:31:22.000000 SRPAstro.FITS-3.0.1/Scripts/SRPFitsComposer
--rw-------   0 covino     (501) staff       (20)     6038 2021-05-12 11:31:34.000000 SRPAstro.FITS-3.0.1/Scripts/SRPFitsExtension
--rw-------   0 covino     (501) staff       (20)     3932 2021-05-12 11:31:45.000000 SRPAstro.FITS-3.0.1/Scripts/SRPFitsHeaders
--rw-------   0 covino     (501) staff       (20)     3648 2022-12-02 13:10:06.000000 SRPAstro.FITS-3.0.1/Scripts/SRPFitsSpectrum2ASCII
--rw-------   0 covino     (501) staff       (20)     4314 2021-05-12 11:32:11.000000 SRPAstro.FITS-3.0.1/Scripts/SRPFitsStats
--rw-------   0 covino     (501) staff       (20)     1629 2021-05-12 11:32:22.000000 SRPAstro.FITS-3.0.1/Scripts/SRPFitsTableViewer
--rw-------   0 covino     (501) staff       (20)     7891 2021-11-16 10:55:33.000000 SRPAstro.FITS-3.0.1/Scripts/SRPFlatImaging
--rw-------   0 covino     (501) staff       (20)     9184 2021-11-16 10:56:34.000000 SRPAstro.FITS-3.0.1/Scripts/SRPFlatSpectroscopy
--rw-------   0 covino     (501) staff       (20)     5995 2021-05-12 11:33:10.000000 SRPAstro.FITS-3.0.1/Scripts/SRPGAIA2Sky
--rw-------   0 covino     (501) staff       (20)     7324 2021-05-12 11:33:22.000000 SRPAstro.FITS-3.0.1/Scripts/SRPImageFilter
--rw-------   0 covino     (501) staff       (20)    18568 2022-03-15 18:19:50.000000 SRPAstro.FITS-3.0.1/Scripts/SRPImageMapping
--rw-------   0 covino     (501) staff       (20)     4975 2021-05-12 11:33:46.000000 SRPAstro.FITS-3.0.1/Scripts/SRPKeywords
--rw-------   0 covino     (501) staff       (20)     2948 2021-05-12 11:34:10.000000 SRPAstro.FITS-3.0.1/Scripts/SRPPhotParSet
--rw-------   0 covino     (501) staff       (20)    12835 2021-05-12 11:33:58.000000 SRPAstro.FITS-3.0.1/Scripts/SRPPhotometry
--rw-------   0 covino     (501) staff       (20)    10876 2021-05-12 11:34:22.000000 SRPAstro.FITS-3.0.1/Scripts/SRPQuery
--rw-------   0 covino     (501) staff       (20)     5424 2021-05-12 11:34:46.000000 SRPAstro.FITS-3.0.1/Scripts/SRPRTAlignImaging
--rw-------   0 covino     (501) staff       (20)     7670 2021-09-07 09:42:34.000000 SRPAstro.FITS-3.0.1/Scripts/SRPRotoTransla
--rw-------   0 covino     (501) staff       (20)     8456 2021-05-12 11:34:57.000000 SRPAstro.FITS-3.0.1/Scripts/SRPScienceFramesImaging
--rw-------   0 covino     (501) staff       (20)     4835 2023-05-22 10:03:42.000000 SRPAstro.FITS-3.0.1/Scripts/SRPSourceFinder
--rw-------   0 covino     (501) staff       (20)     3966 2023-05-22 10:05:47.000000 SRPAstro.FITS-3.0.1/Scripts/SRPSourcePhotometry
--rw-------   0 covino     (501) staff       (20)     7534 2021-05-12 11:35:23.000000 SRPAstro.FITS-3.0.1/Scripts/SRPSpectralExtraction
--rw-------   0 covino     (501) staff       (20)     5488 2021-05-12 11:35:35.000000 SRPAstro.FITS-3.0.1/Scripts/SRPWCSPixel
--rw-------   0 covino     (501) staff       (20)     7247 2021-06-02 09:56:24.000000 SRPAstro.FITS-3.0.1/Scripts/SRPZeroPoint
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.097822 SRPAstro.FITS-3.0.1/build/
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.097969 SRPAstro.FITS-3.0.1/build/lib/
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.633581 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.741131 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/
--rw-------   0 covino     (501) staff       (20)     1930 2017-05-18 14:30:00.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/AddHeaderComment.py
--rw-------   0 covino     (501) staff       (20)     2612 2021-07-08 08:39:43.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/AddHeaderEntry.py
--rw-------   0 covino     (501) staff       (20)     1967 2015-07-23 12:13:33.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/FitsConstants.py
--rw-------   0 covino     (501) staff       (20)     8608 2021-03-02 15:35:24.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/FitsImageClass.py
--rw-------   0 covino     (501) staff       (20)      869 2015-07-23 12:13:58.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/FitsTabsAppend.py
--rw-------   0 covino     (501) staff       (20)      760 2017-05-18 14:34:24.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/GetData.py
--rw-------   0 covino     (501) staff       (20)      802 2017-05-18 14:35:11.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/GetHeader.py
--rw-------   0 covino     (501) staff       (20)      875 2017-05-18 14:35:28.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/GetHeaderValue.py
--rw-------   0 covino     (501) staff       (20)      997 2017-05-18 13:39:55.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/GetSpectrum.py
--rw-------   0 covino     (501) staff       (20)      586 2015-07-23 12:34:36.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/GetSpectrumPosition.py
--rw-------   0 covino     (501) staff       (20)     1424 2021-02-09 12:48:15.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/GetWCS.py
--rw-------   0 covino     (501) staff       (20)      702 2017-08-22 21:04:15.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/IsFits.py
--rw-------   0 covino     (501) staff       (20)      437 2021-01-14 10:07:28.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/WCSPixelScale.py
--rw-------   0 covino     (501) staff       (20)      567 2021-01-14 10:40:27.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/WCSRotationDeg.py
--rw-------   0 covino     (501) staff       (20)      799 2022-08-10 13:01:02.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/__init__.py
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.757997 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/
--rw-------   0 covino     (501) staff       (20)    24425 2021-03-17 08:46:10.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/AstrometryClass.py
--rw-------   0 covino     (501) staff       (20)     2810 2021-03-02 15:30:39.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/DAOObjectClass.py
--rw-------   0 covino     (501) staff       (20)      425 2015-07-23 12:15:58.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/EclipseConstants.py
--rw-------   0 covino     (501) staff       (20)     2636 2017-05-16 09:56:28.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/EclipseObjectClass.py
--rw-------   0 covino     (501) staff       (20)      853 2020-05-14 16:28:39.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/Pixel2WCS.py
--rw-------   0 covino     (501) staff       (20)     1394 2020-05-14 13:44:46.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/SExtractorConstants.py
--rw-------   0 covino     (501) staff       (20)      361 2015-07-23 12:16:42.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/SexConstants.py
--rw-------   0 covino     (501) staff       (20)     2562 2020-12-11 12:24:32.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/SexObjectClass.py
--rw-------   0 covino     (501) staff       (20)     5248 2017-05-26 14:52:54.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/SourceObjectsClass.py
--rw-------   0 covino     (501) staff       (20)      865 2020-05-14 14:24:01.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/WCS2Pixel.py
--rw-------   0 covino     (501) staff       (20)      588 2017-05-16 09:52:29.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/__init__.py
--rw-------   0 covino     (501) staff       (20)      637 2020-03-07 14:00:40.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/getCenterRADEC.py
--rw-r--r--   0 covino     (501) staff       (20)     1086 2023-05-22 09:48:40.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/GetFWHM.py
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.759999 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Math/
--rw-------   0 covino     (501) staff       (20)     8163 2021-07-06 13:46:23.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Math/TriangleMatch.py
--rw-------   0 covino     (501) staff       (20)      331 2017-03-14 08:48:57.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Math/__init__.py
-drwxr-xr-x   0 covino     (501) staff       (20)        0 2023-05-22 10:07:49.797392 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/
--rw-------   0 covino     (501) staff       (20)     1126 2017-04-19 13:53:05.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/ApErr.py
--rw-------   0 covino     (501) staff       (20)     2903 2020-10-05 08:41:16.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/ApyPhot.py
--rw-------   0 covino     (501) staff       (20)      520 2015-12-11 15:46:16.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/Counts2Mag.py
--rw-------   0 covino     (501) staff       (20)      884 2017-08-30 19:36:03.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/DaoPhot.py
--rw-r--r--   0 covino     (501) staff       (20)     5146 2023-05-22 09:44:44.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/FitsPhotometryClass.py
--rw-------   0 covino     (501) staff       (20)      503 2015-07-23 12:26:20.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/Mag2Counts.py
--rw-------   0 covino     (501) staff       (20)     1086 2015-11-13 14:11:34.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/MinMax.py
--rw-------   0 covino     (501) staff       (20)      849 2022-08-10 13:00:32.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/__init__.py
--rw-------   0 covino     (501) staff       (20)     1142 2017-04-19 13:45:07.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/centerGauss.py
--rw-------   0 covino     (501) staff       (20)     1653 2020-03-07 16:49:45.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/centerMoment.py
--rw-------   0 covino     (501) staff       (20)     1563 2017-08-24 08:53:55.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/centerObj.py
--rw-------   0 covino     (501) staff       (20)     1281 2015-11-13 10:37:46.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/getBackground.py
--rw-------   0 covino     (501) staff       (20)      803 2015-11-10 10:11:17.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/resid.py
--rw-r--r--   0 covino     (501) staff       (20)      521 2021-06-02 20:51:07.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/SRPFITSPath.py
--rw-r--r--   0 covino     (501) staff       (20)     2481 2023-05-22 09:48:36.000000 SRPAstro.FITS-3.0.1/build/lib/SRPFITS/__init__.py
--rw-r--r--   0 covino     (501) staff       (20)      107 2023-05-22 10:07:50.569128 SRPAstro.FITS-3.0.1/setup.cfg
--rw-------   0 covino     (501) staff       (20)     1780 2023-05-22 09:42:51.000000 SRPAstro.FITS-3.0.1/setup.py
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2024-04-30 14:08:33.660078 srpastro_fits-3.0.3/
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2024-04-30 14:08:33.298609 srpastro_fits-3.0.3/Docs/
+-rw-------   0 covino     (501) staff       (20)   142337 2017-02-21 14:33:07.000000 srpastro_fits-3.0.3/Docs/SRPAstro.FITS.pdf
+-rw-r--r--   0 covino     (501) staff       (20)     1081 2019-05-07 09:54:08.000000 srpastro_fits-3.0.3/LICENSE.txt
+-rw-r--r--   0 covino     (501) staff       (20)      330 2023-11-24 10:48:55.000000 srpastro_fits-3.0.3/MANIFEST.in
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2024-04-30 14:08:33.098073 srpastro_fits-3.0.3/Misc/
+-rw-------   0 covino     (501) staff       (20)     1288 2019-05-22 19:31:58.000000 srpastro_fits-3.0.3/Misc/ApyPhot.py
+-rw-------   0 covino     (501) staff       (20)    23044 2021-02-02 11:59:14.000000 srpastro_fits-3.0.3/Misc/AstrometryClass.py
+-rw-r--r--   0 covino     (501) staff       (20)     1659 2024-04-30 14:08:33.659956 srpastro_fits-3.0.3/PKG-INFO
+-rw-r--r--   0 covino     (501) staff       (20)      744 2019-07-22 12:26:27.000000 srpastro_fits-3.0.3/README.md
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2024-04-30 14:08:33.659419 srpastro_fits-3.0.3/SRPAstro.FITS.egg-info/
+-rw-r--r--   0 covino     (501) staff       (20)     1659 2024-04-30 14:08:33.000000 srpastro_fits-3.0.3/SRPAstro.FITS.egg-info/PKG-INFO
+-rw-------   0 covino     (501) staff       (20)     6615 2024-04-30 14:08:33.000000 srpastro_fits-3.0.3/SRPAstro.FITS.egg-info/SOURCES.txt
+-rw-------   0 covino     (501) staff       (20)        1 2024-04-30 14:08:33.000000 srpastro_fits-3.0.3/SRPAstro.FITS.egg-info/dependency_links.txt
+-rw-------   0 covino     (501) staff       (20)       62 2024-04-30 14:08:33.000000 srpastro_fits-3.0.3/SRPAstro.FITS.egg-info/requires.txt
+-rw-------   0 covino     (501) staff       (20)        8 2024-04-30 14:08:33.000000 srpastro_fits-3.0.3/SRPAstro.FITS.egg-info/top_level.txt
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2024-04-30 14:08:33.315902 srpastro_fits-3.0.3/SRPFITS/
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2024-04-30 14:08:33.316256 srpastro_fits-3.0.3/SRPFITS/Data/
+-rw-r--r--   0 covino     (501) staff       (20)     8196 2020-03-04 14:48:58.000000 srpastro_fits-3.0.3/SRPFITS/Data/.DS_Store
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2024-04-30 14:08:33.349482 srpastro_fits-3.0.3/SRPFITS/Data/SExtractor/
+-rw-------   0 covino     (501) staff       (20)       88 2010-09-28 13:27:42.000000 srpastro_fits-3.0.3/SRPFITS/Data/SExtractor/SRPConvIn
+-rw-------   0 covino     (501) staff       (20)      332 2010-09-28 13:33:03.000000 srpastro_fits-3.0.3/SRPFITS/Data/SExtractor/SRPConvLSLASCIn
+-rw-------   0 covino     (501) staff       (20)     2165 2010-09-28 13:30:00.000000 srpastro_fits-3.0.3/SRPFITS/Data/SExtractor/SRPNnwIn
+-rw-------   0 covino     (501) staff       (20)      179 2013-12-06 14:18:19.000000 srpastro_fits-3.0.3/SRPFITS/Data/SExtractor/SRPParamIn
+-rw-------   0 covino     (501) staff       (20)      750 2010-09-28 13:31:35.000000 srpastro_fits-3.0.3/SRPFITS/Data/SExtractor/SRPSexIn
+-rw-------   0 covino     (501) staff       (20)      749 2010-09-28 13:33:53.000000 srpastro_fits-3.0.3/SRPFITS/Data/SExtractor/SRPSexLSLASCIn
+-rw-------   0 covino     (501) staff       (20)      752 2012-01-25 16:07:42.000000 srpastro_fits-3.0.3/SRPFITS/Data/SExtractor/SRPSexREMREMIRIn
+-rw-------   0 covino     (501) staff       (20)      750 2013-08-18 20:17:05.000000 srpastro_fits-3.0.3/SRPFITS/Data/SExtractor/SRPSexREMROS2In
+-rw-------   0 covino     (501) staff       (20)      751 2012-04-01 19:58:22.000000 srpastro_fits-3.0.3/SRPFITS/Data/SExtractor/SRPSexREMROSSIn
+-rw-------   0 covino     (501) staff       (20)      750 2010-09-28 13:53:56.000000 srpastro_fits-3.0.3/SRPFITS/Data/SExtractor/SRPSexTNGLRSIn
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2024-04-30 14:08:33.352320 srpastro_fits-3.0.3/SRPFITS/Fits/
+-rw-------   0 covino     (501) staff       (20)     1930 2017-05-18 14:30:00.000000 srpastro_fits-3.0.3/SRPFITS/Fits/AddHeaderComment.py
+-rw-------   0 covino     (501) staff       (20)     2612 2021-07-08 08:39:43.000000 srpastro_fits-3.0.3/SRPFITS/Fits/AddHeaderEntry.py
+-rw-------   0 covino     (501) staff       (20)     1967 2015-07-23 12:13:33.000000 srpastro_fits-3.0.3/SRPFITS/Fits/FitsConstants.py
+-rw-------   0 covino     (501) staff       (20)     8608 2021-03-02 15:35:24.000000 srpastro_fits-3.0.3/SRPFITS/Fits/FitsImageClass.py
+-rw-------   0 covino     (501) staff       (20)      869 2015-07-23 12:13:58.000000 srpastro_fits-3.0.3/SRPFITS/Fits/FitsTabsAppend.py
+-rw-------   0 covino     (501) staff       (20)      760 2017-05-18 14:34:24.000000 srpastro_fits-3.0.3/SRPFITS/Fits/GetData.py
+-rw-------   0 covino     (501) staff       (20)      802 2017-05-18 14:35:11.000000 srpastro_fits-3.0.3/SRPFITS/Fits/GetHeader.py
+-rw-------   0 covino     (501) staff       (20)      875 2017-05-18 14:35:28.000000 srpastro_fits-3.0.3/SRPFITS/Fits/GetHeaderValue.py
+-rw-------   0 covino     (501) staff       (20)      997 2017-05-18 13:39:55.000000 srpastro_fits-3.0.3/SRPFITS/Fits/GetSpectrum.py
+-rw-------   0 covino     (501) staff       (20)      586 2015-07-23 12:34:36.000000 srpastro_fits-3.0.3/SRPFITS/Fits/GetSpectrumPosition.py
+-rw-------   0 covino     (501) staff       (20)     1424 2021-02-09 12:48:15.000000 srpastro_fits-3.0.3/SRPFITS/Fits/GetWCS.py
+-rw-------   0 covino     (501) staff       (20)      702 2017-08-22 21:04:15.000000 srpastro_fits-3.0.3/SRPFITS/Fits/IsFits.py
+-rw-------   0 covino     (501) staff       (20)      437 2021-01-14 10:07:28.000000 srpastro_fits-3.0.3/SRPFITS/Fits/WCSPixelScale.py
+-rw-------   0 covino     (501) staff       (20)      567 2021-01-14 10:40:27.000000 srpastro_fits-3.0.3/SRPFITS/Fits/WCSRotationDeg.py
+-rw-------   0 covino     (501) staff       (20)      799 2022-08-10 13:01:02.000000 srpastro_fits-3.0.3/SRPFITS/Fits/__init__.py
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2024-04-30 14:08:33.202860 srpastro_fits-3.0.3/SRPFITS/Frames/
+-rw-------   0 covino     (501) staff       (20)    24425 2021-03-17 08:46:10.000000 srpastro_fits-3.0.3/SRPFITS/Frames/AstrometryClass.py
+-rw-------   0 covino     (501) staff       (20)     2810 2021-03-02 15:30:39.000000 srpastro_fits-3.0.3/SRPFITS/Frames/DAOObjectClass.py
+-rw-------   0 covino     (501) staff       (20)      425 2015-07-23 12:15:58.000000 srpastro_fits-3.0.3/SRPFITS/Frames/EclipseConstants.py
+-rw-------   0 covino     (501) staff       (20)     2636 2017-05-16 09:56:28.000000 srpastro_fits-3.0.3/SRPFITS/Frames/EclipseObjectClass.py
+-rw-------   0 covino     (501) staff       (20)      853 2020-05-14 16:28:39.000000 srpastro_fits-3.0.3/SRPFITS/Frames/Pixel2WCS.py
+-rw-------   0 covino     (501) staff       (20)     1394 2020-05-14 13:44:46.000000 srpastro_fits-3.0.3/SRPFITS/Frames/SExtractorConstants.py
+-rw-------   0 covino     (501) staff       (20)      361 2015-07-23 12:16:42.000000 srpastro_fits-3.0.3/SRPFITS/Frames/SexConstants.py
+-rw-------   0 covino     (501) staff       (20)     2562 2020-12-11 12:24:32.000000 srpastro_fits-3.0.3/SRPFITS/Frames/SexObjectClass.py
+-rw-------   0 covino     (501) staff       (20)     5248 2017-05-26 14:52:54.000000 srpastro_fits-3.0.3/SRPFITS/Frames/SourceObjectsClass.py
+-rw-------   0 covino     (501) staff       (20)      865 2020-05-14 14:24:01.000000 srpastro_fits-3.0.3/SRPFITS/Frames/WCS2Pixel.py
+-rw-------   0 covino     (501) staff       (20)      588 2017-05-16 09:52:29.000000 srpastro_fits-3.0.3/SRPFITS/Frames/__init__.py
+-rw-------   0 covino     (501) staff       (20)      637 2020-03-07 14:00:40.000000 srpastro_fits-3.0.3/SRPFITS/Frames/getCenterRADEC.py
+-rw-------   0 covino     (501) staff       (20)     1086 2023-05-22 09:48:40.000000 srpastro_fits-3.0.3/SRPFITS/GetFWHM.py
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2024-04-30 14:08:33.204365 srpastro_fits-3.0.3/SRPFITS/Math/
+-rw-------   0 covino     (501) staff       (20)     8163 2021-07-06 13:46:23.000000 srpastro_fits-3.0.3/SRPFITS/Math/TriangleMatch.py
+-rw-------   0 covino     (501) staff       (20)      331 2017-03-14 08:48:57.000000 srpastro_fits-3.0.3/SRPFITS/Math/__init__.py
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2024-04-30 14:08:33.355475 srpastro_fits-3.0.3/SRPFITS/Photometry/
+-rw-------   0 covino     (501) staff       (20)     1126 2017-04-19 13:53:05.000000 srpastro_fits-3.0.3/SRPFITS/Photometry/ApErr.py
+-rw-------   0 covino     (501) staff       (20)     2903 2020-10-05 08:41:16.000000 srpastro_fits-3.0.3/SRPFITS/Photometry/ApyPhot.py
+-rw-------   0 covino     (501) staff       (20)      603 2023-11-30 12:49:36.000000 srpastro_fits-3.0.3/SRPFITS/Photometry/Counts2Mag.py
+-rw-------   0 covino     (501) staff       (20)      884 2017-08-30 19:36:03.000000 srpastro_fits-3.0.3/SRPFITS/Photometry/DaoPhot.py
+-rw-------   0 covino     (501) staff       (20)     6203 2024-02-02 14:56:38.000000 srpastro_fits-3.0.3/SRPFITS/Photometry/FitsPhotometryClass.py
+-rw-------   0 covino     (501) staff       (20)      503 2015-07-23 12:26:20.000000 srpastro_fits-3.0.3/SRPFITS/Photometry/Mag2Counts.py
+-rw-------   0 covino     (501) staff       (20)     1086 2015-11-13 14:11:34.000000 srpastro_fits-3.0.3/SRPFITS/Photometry/MinMax.py
+-rw-------   0 covino     (501) staff       (20)      849 2022-08-10 13:00:32.000000 srpastro_fits-3.0.3/SRPFITS/Photometry/__init__.py
+-rw-------   0 covino     (501) staff       (20)     1142 2017-04-19 13:45:07.000000 srpastro_fits-3.0.3/SRPFITS/Photometry/centerGauss.py
+-rw-------   0 covino     (501) staff       (20)     1653 2020-03-07 16:49:45.000000 srpastro_fits-3.0.3/SRPFITS/Photometry/centerMoment.py
+-rw-------   0 covino     (501) staff       (20)     1563 2017-08-24 08:53:55.000000 srpastro_fits-3.0.3/SRPFITS/Photometry/centerObj.py
+-rw-------   0 covino     (501) staff       (20)     1281 2015-11-13 10:37:46.000000 srpastro_fits-3.0.3/SRPFITS/Photometry/getBackground.py
+-rw-------   0 covino     (501) staff       (20)      803 2015-11-10 10:11:17.000000 srpastro_fits-3.0.3/SRPFITS/Photometry/resid.py
+-rw-------   0 covino     (501) staff       (20)      521 2021-06-02 20:51:07.000000 srpastro_fits-3.0.3/SRPFITS/SRPFITSPath.py
+-rw-------   0 covino     (501) staff       (20)     2548 2024-04-30 11:43:02.000000 srpastro_fits-3.0.3/SRPFITS/__init__.py
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2024-04-30 14:08:33.646897 srpastro_fits-3.0.3/Scripts/
+-rw-------   0 covino     (501) staff       (20)    10932 2021-09-07 09:46:26.000000 srpastro_fits-3.0.3/Scripts/SRPAdvAverage
+-rw-------   0 covino     (501) staff       (20)     5242 2021-05-12 11:29:46.000000 srpastro_fits-3.0.3/Scripts/SRPAlignImaging
+-rw-------   0 covino     (501) staff       (20)    10433 2021-05-12 11:29:59.000000 srpastro_fits-3.0.3/Scripts/SRPAstrometry
+-rw-------   0 covino     (501) staff       (20)     5660 2021-05-12 11:30:11.000000 srpastro_fits-3.0.3/Scripts/SRPAverage
+-rw-------   0 covino     (501) staff       (20)     6023 2021-11-16 10:55:28.000000 srpastro_fits-3.0.3/Scripts/SRPBias
+-rw-------   0 covino     (501) staff       (20)     3831 2021-05-12 11:30:35.000000 srpastro_fits-3.0.3/Scripts/SRPClassify
+-rw-------   0 covino     (501) staff       (20)     7083 2021-05-12 11:30:47.000000 srpastro_fits-3.0.3/Scripts/SRPCut
+-rw-------   0 covino     (501) staff       (20)     8464 2021-05-12 11:30:59.000000 srpastro_fits-3.0.3/Scripts/SRPDao2Sky
+-rw-------   0 covino     (501) staff       (20)      800 2021-05-12 11:32:34.000000 srpastro_fits-3.0.3/Scripts/SRPFITSVersion
+-rw-------   0 covino     (501) staff       (20)     4492 2021-05-12 11:31:10.000000 srpastro_fits-3.0.3/Scripts/SRPFindingChart
+-rw-------   0 covino     (501) staff       (20)     3692 2021-05-12 11:31:22.000000 srpastro_fits-3.0.3/Scripts/SRPFitsComposer
+-rw-------   0 covino     (501) staff       (20)     6038 2021-05-12 11:31:34.000000 srpastro_fits-3.0.3/Scripts/SRPFitsExtension
+-rw-------   0 covino     (501) staff       (20)     3932 2021-05-12 11:31:45.000000 srpastro_fits-3.0.3/Scripts/SRPFitsHeaders
+-rw-------   0 covino     (501) staff       (20)     3648 2022-12-02 13:10:06.000000 srpastro_fits-3.0.3/Scripts/SRPFitsSpectrum2ASCII
+-rw-------   0 covino     (501) staff       (20)     4314 2021-05-12 11:32:11.000000 srpastro_fits-3.0.3/Scripts/SRPFitsStats
+-rw-------   0 covino     (501) staff       (20)     1629 2021-05-12 11:32:22.000000 srpastro_fits-3.0.3/Scripts/SRPFitsTableViewer
+-rw-------   0 covino     (501) staff       (20)     7891 2021-11-16 10:55:33.000000 srpastro_fits-3.0.3/Scripts/SRPFlatImaging
+-rw-------   0 covino     (501) staff       (20)     9184 2021-11-16 10:56:34.000000 srpastro_fits-3.0.3/Scripts/SRPFlatSpectroscopy
+-rw-------   0 covino     (501) staff       (20)     5995 2021-05-12 11:33:10.000000 srpastro_fits-3.0.3/Scripts/SRPGAIA2Sky
+-rw-------   0 covino     (501) staff       (20)     7324 2021-05-12 11:33:22.000000 srpastro_fits-3.0.3/Scripts/SRPImageFilter
+-rw-------   0 covino     (501) staff       (20)    18568 2022-03-15 18:19:50.000000 srpastro_fits-3.0.3/Scripts/SRPImageMapping
+-rw-------   0 covino     (501) staff       (20)     4975 2021-05-12 11:33:46.000000 srpastro_fits-3.0.3/Scripts/SRPKeywords
+-rw-------   0 covino     (501) staff       (20)     2948 2021-05-12 11:34:10.000000 srpastro_fits-3.0.3/Scripts/SRPPhotParSet
+-rw-------   0 covino     (501) staff       (20)    12835 2021-05-12 11:33:58.000000 srpastro_fits-3.0.3/Scripts/SRPPhotometry
+-rw-------   0 covino     (501) staff       (20)    10876 2021-05-12 11:34:22.000000 srpastro_fits-3.0.3/Scripts/SRPQuery
+-rw-------   0 covino     (501) staff       (20)     5424 2021-05-12 11:34:46.000000 srpastro_fits-3.0.3/Scripts/SRPRTAlignImaging
+-rw-------   0 covino     (501) staff       (20)     7670 2021-09-07 09:42:34.000000 srpastro_fits-3.0.3/Scripts/SRPRotoTransla
+-rw-------   0 covino     (501) staff       (20)     8456 2021-05-12 11:34:57.000000 srpastro_fits-3.0.3/Scripts/SRPScienceFramesImaging
+-rw-------   0 covino     (501) staff       (20)     4835 2023-05-22 10:03:42.000000 srpastro_fits-3.0.3/Scripts/SRPSourceFinder
+-rw-------   0 covino     (501) staff       (20)     4053 2024-02-29 10:37:30.000000 srpastro_fits-3.0.3/Scripts/SRPSourcePhotometry
+-rw-------   0 covino     (501) staff       (20)     7564 2024-04-30 12:08:46.000000 srpastro_fits-3.0.3/Scripts/SRPSpectralExtraction
+-rw-------   0 covino     (501) staff       (20)     5488 2021-05-12 11:35:35.000000 srpastro_fits-3.0.3/Scripts/SRPWCSPixel
+-rw-------   0 covino     (501) staff       (20)     7247 2021-06-02 09:56:24.000000 srpastro_fits-3.0.3/Scripts/SRPZeroPoint
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2024-04-30 14:08:33.061485 srpastro_fits-3.0.3/build/
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2024-04-30 14:08:33.061615 srpastro_fits-3.0.3/build/lib/
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2024-04-30 14:08:33.241148 srpastro_fits-3.0.3/build/lib/SRPFITS/
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2024-04-30 14:08:33.277076 srpastro_fits-3.0.3/build/lib/SRPFITS/Fits/
+-rw-------   0 covino     (501) staff       (20)     1930 2017-05-18 14:30:00.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Fits/AddHeaderComment.py
+-rw-r--r--   0 covino     (501) staff       (20)     2612 2021-07-08 08:39:43.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Fits/AddHeaderEntry.py
+-rw-------   0 covino     (501) staff       (20)     1967 2015-07-23 12:13:33.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Fits/FitsConstants.py
+-rw-------   0 covino     (501) staff       (20)     8608 2021-03-02 15:35:24.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Fits/FitsImageClass.py
+-rw-------   0 covino     (501) staff       (20)      869 2015-07-23 12:13:58.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Fits/FitsTabsAppend.py
+-rw-------   0 covino     (501) staff       (20)      760 2017-05-18 14:34:24.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Fits/GetData.py
+-rw-------   0 covino     (501) staff       (20)      802 2017-05-18 14:35:11.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Fits/GetHeader.py
+-rw-------   0 covino     (501) staff       (20)      875 2017-05-18 14:35:28.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Fits/GetHeaderValue.py
+-rw-------   0 covino     (501) staff       (20)      997 2017-05-18 13:39:55.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Fits/GetSpectrum.py
+-rw-------   0 covino     (501) staff       (20)      586 2015-07-23 12:34:36.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Fits/GetSpectrumPosition.py
+-rw-------   0 covino     (501) staff       (20)     1424 2021-02-09 12:48:15.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Fits/GetWCS.py
+-rw-------   0 covino     (501) staff       (20)      702 2017-08-22 21:04:15.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Fits/IsFits.py
+-rw-------   0 covino     (501) staff       (20)      437 2021-01-14 10:07:28.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Fits/WCSPixelScale.py
+-rw-------   0 covino     (501) staff       (20)      567 2021-01-14 10:40:27.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Fits/WCSRotationDeg.py
+-rw-r--r--   0 covino     (501) staff       (20)      799 2022-08-10 13:01:02.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Fits/__init__.py
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2024-04-30 14:08:33.288175 srpastro_fits-3.0.3/build/lib/SRPFITS/Frames/
+-rw-------   0 covino     (501) staff       (20)    24425 2021-03-17 08:46:10.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Frames/AstrometryClass.py
+-rw-------   0 covino     (501) staff       (20)     2810 2021-03-02 15:30:39.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Frames/DAOObjectClass.py
+-rw-------   0 covino     (501) staff       (20)      425 2015-07-23 12:15:58.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Frames/EclipseConstants.py
+-rw-------   0 covino     (501) staff       (20)     2636 2017-05-16 09:56:28.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Frames/EclipseObjectClass.py
+-rw-------   0 covino     (501) staff       (20)      853 2020-05-14 16:28:39.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Frames/Pixel2WCS.py
+-rw-------   0 covino     (501) staff       (20)     1394 2020-05-14 13:44:46.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Frames/SExtractorConstants.py
+-rw-------   0 covino     (501) staff       (20)      361 2015-07-23 12:16:42.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Frames/SexConstants.py
+-rw-------   0 covino     (501) staff       (20)     2562 2020-12-11 12:24:32.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Frames/SexObjectClass.py
+-rw-------   0 covino     (501) staff       (20)     5248 2017-05-26 14:52:54.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Frames/SourceObjectsClass.py
+-rw-------   0 covino     (501) staff       (20)      865 2020-05-14 14:24:01.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Frames/WCS2Pixel.py
+-rw-------   0 covino     (501) staff       (20)      588 2017-05-16 09:52:29.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Frames/__init__.py
+-rw-------   0 covino     (501) staff       (20)      637 2020-03-07 14:00:40.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Frames/getCenterRADEC.py
+-rw-r--r--   0 covino     (501) staff       (20)     1086 2023-05-22 09:48:40.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/GetFWHM.py
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2024-04-30 14:08:33.289485 srpastro_fits-3.0.3/build/lib/SRPFITS/Math/
+-rw-------   0 covino     (501) staff       (20)     8163 2021-07-06 13:46:23.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Math/TriangleMatch.py
+-rw-------   0 covino     (501) staff       (20)      331 2017-03-14 08:48:57.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Math/__init__.py
+drwxr-xr-x   0 covino     (501) staff       (20)        0 2024-04-30 14:08:33.297926 srpastro_fits-3.0.3/build/lib/SRPFITS/Photometry/
+-rw-------   0 covino     (501) staff       (20)     1126 2017-04-19 13:53:05.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Photometry/ApErr.py
+-rw-------   0 covino     (501) staff       (20)     2903 2020-10-05 08:41:16.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Photometry/ApyPhot.py
+-rw-r--r--   0 covino     (501) staff       (20)      603 2023-11-30 12:49:36.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Photometry/Counts2Mag.py
+-rw-------   0 covino     (501) staff       (20)      884 2017-08-30 19:36:03.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Photometry/DaoPhot.py
+-rw-r--r--   0 covino     (501) staff       (20)     6203 2024-02-02 14:56:38.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Photometry/FitsPhotometryClass.py
+-rw-------   0 covino     (501) staff       (20)      503 2015-07-23 12:26:20.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Photometry/Mag2Counts.py
+-rw-------   0 covino     (501) staff       (20)     1086 2015-11-13 14:11:34.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Photometry/MinMax.py
+-rw-r--r--   0 covino     (501) staff       (20)      849 2022-08-10 13:00:32.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Photometry/__init__.py
+-rw-------   0 covino     (501) staff       (20)     1142 2017-04-19 13:45:07.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Photometry/centerGauss.py
+-rw-------   0 covino     (501) staff       (20)     1653 2020-03-07 16:49:45.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Photometry/centerMoment.py
+-rw-------   0 covino     (501) staff       (20)     1563 2017-08-24 08:53:55.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Photometry/centerObj.py
+-rw-------   0 covino     (501) staff       (20)     1281 2015-11-13 10:37:46.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Photometry/getBackground.py
+-rw-------   0 covino     (501) staff       (20)      803 2015-11-10 10:11:17.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/Photometry/resid.py
+-rw-r--r--   0 covino     (501) staff       (20)      521 2021-06-02 20:51:07.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/SRPFITSPath.py
+-rw-r--r--   0 covino     (501) staff       (20)     2548 2024-04-30 11:43:02.000000 srpastro_fits-3.0.3/build/lib/SRPFITS/__init__.py
+-rw-r--r--   0 covino     (501) staff       (20)      107 2024-04-30 14:08:33.660511 srpastro_fits-3.0.3/setup.cfg
+-rw-------   0 covino     (501) staff       (20)     1780 2023-05-22 09:42:51.000000 srpastro_fits-3.0.3/setup.py
```

### Comparing `SRPAstro.FITS-3.0.1/Docs/SRPAstro.FITS.pdf` & `srpastro_fits-3.0.3/Docs/SRPAstro.FITS.pdf`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/LICENSE.txt` & `srpastro_fits-3.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Misc/ApyPhot.py` & `srpastro_fits-3.0.3/Misc/ApyPhot.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Misc/AstrometryClass.py` & `srpastro_fits-3.0.3/Misc/AstrometryClass.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/PKG-INFO` & `srpastro_fits-3.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SRPAstro.FITS
-Version: 3.0.1
+Version: 3.0.3
 Summary: Tools for handling FITS files under SRP
 Home-page: https://pypi.python.org/pypi/SRPAstro.FITS
 Author: Stefano Covino
 Author-email: stefano.covino@inaf.it
 Keywords: astronomy data analysis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -14,14 +14,20 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: SRPAstro>=4.4
+Requires-Dist: sep
+Requires-Dist: photutils
+Requires-Dist: astropy
+Requires-Dist: astLib>=0.11.5
+Requires-Dist: astroalign
 
 # Swift Reduction Package
 
 Background
 The Swift Reduction Package (hereafter SRP) is a packet of command line tools to solve problems (e.g. basic reduction and analysis tasks of optical/NIR astronomical data, quick cosmological computations, units conversions, etc.) often met in astronomical research activities.
 
 SRP was originally developed in the context of the Swift follow-up activities of the Milan GRB team at the INAF/Brera Astronomical Observatory. The package is designed to be an aid to any researcher to drive further observation of a followed-up GRB counterpart and “swift” can therefore be read simply as “rapid”, “agile”, etc.
```

### Comparing `SRPAstro.FITS-3.0.1/README.md` & `srpastro_fits-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPAstro.FITS.egg-info/PKG-INFO` & `srpastro_fits-3.0.3/SRPAstro.FITS.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SRPAstro.FITS
-Version: 3.0.1
+Version: 3.0.3
 Summary: Tools for handling FITS files under SRP
 Home-page: https://pypi.python.org/pypi/SRPAstro.FITS
 Author: Stefano Covino
 Author-email: stefano.covino@inaf.it
 Keywords: astronomy data analysis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -14,14 +14,20 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: SRPAstro>=4.4
+Requires-Dist: sep
+Requires-Dist: photutils
+Requires-Dist: astropy
+Requires-Dist: astLib>=0.11.5
+Requires-Dist: astroalign
 
 # Swift Reduction Package
 
 Background
 The Swift Reduction Package (hereafter SRP) is a packet of command line tools to solve problems (e.g. basic reduction and analysis tasks of optical/NIR astronomical data, quick cosmological computations, units conversions, etc.) often met in astronomical research activities.
 
 SRP was originally developed in the context of the Swift follow-up activities of the Milan GRB team at the INAF/Brera Astronomical Observatory. The package is designed to be an aid to any researcher to drive further observation of a followed-up GRB counterpart and “swift” can therefore be read simply as “rapid”, “agile”, etc.
```

### Comparing `SRPAstro.FITS-3.0.1/SRPAstro.FITS.egg-info/SOURCES.txt` & `srpastro_fits-3.0.3/SRPAstro.FITS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Data/.DS_Store` & `srpastro_fits-3.0.3/SRPFITS/Data/.DS_Store`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPNnwIn` & `srpastro_fits-3.0.3/SRPFITS/Data/SExtractor/SRPNnwIn`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPSexIn` & `srpastro_fits-3.0.3/SRPFITS/Data/SExtractor/SRPSexIn`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPSexLSLASCIn` & `srpastro_fits-3.0.3/SRPFITS/Data/SExtractor/SRPSexLSLASCIn`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPSexREMREMIRIn` & `srpastro_fits-3.0.3/SRPFITS/Data/SExtractor/SRPSexREMREMIRIn`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPSexREMROS2In` & `srpastro_fits-3.0.3/SRPFITS/Data/SExtractor/SRPSexREMROS2In`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPSexREMROSSIn` & `srpastro_fits-3.0.3/SRPFITS/Data/SExtractor/SRPSexREMROSSIn`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Data/SExtractor/SRPSexTNGLRSIn` & `srpastro_fits-3.0.3/SRPFITS/Data/SExtractor/SRPSexTNGLRSIn`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Fits/AddHeaderComment.py` & `srpastro_fits-3.0.3/SRPFITS/Fits/AddHeaderComment.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Fits/AddHeaderEntry.py` & `srpastro_fits-3.0.3/SRPFITS/Fits/AddHeaderEntry.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Fits/FitsConstants.py` & `srpastro_fits-3.0.3/SRPFITS/Fits/FitsConstants.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Fits/FitsImageClass.py` & `srpastro_fits-3.0.3/SRPFITS/Fits/FitsImageClass.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Fits/FitsTabsAppend.py` & `srpastro_fits-3.0.3/SRPFITS/Fits/FitsTabsAppend.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Fits/GetData.py` & `srpastro_fits-3.0.3/SRPFITS/Fits/GetData.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Fits/GetHeader.py` & `srpastro_fits-3.0.3/SRPFITS/Fits/GetHeader.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Fits/GetHeaderValue.py` & `srpastro_fits-3.0.3/SRPFITS/Fits/GetHeaderValue.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Fits/GetSpectrum.py` & `srpastro_fits-3.0.3/SRPFITS/Fits/GetSpectrum.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Fits/GetSpectrumPosition.py` & `srpastro_fits-3.0.3/SRPFITS/Fits/GetSpectrumPosition.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Fits/GetWCS.py` & `srpastro_fits-3.0.3/SRPFITS/Fits/GetWCS.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Fits/IsFits.py` & `srpastro_fits-3.0.3/SRPFITS/Fits/IsFits.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Fits/WCSRotationDeg.py` & `srpastro_fits-3.0.3/SRPFITS/Fits/WCSRotationDeg.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Fits/__init__.py` & `srpastro_fits-3.0.3/SRPFITS/Fits/__init__.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Frames/AstrometryClass.py` & `srpastro_fits-3.0.3/SRPFITS/Frames/AstrometryClass.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Frames/DAOObjectClass.py` & `srpastro_fits-3.0.3/SRPFITS/Frames/DAOObjectClass.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Frames/EclipseObjectClass.py` & `srpastro_fits-3.0.3/SRPFITS/Frames/EclipseObjectClass.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Frames/Pixel2WCS.py` & `srpastro_fits-3.0.3/SRPFITS/Frames/Pixel2WCS.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Frames/SExtractorConstants.py` & `srpastro_fits-3.0.3/SRPFITS/Frames/SExtractorConstants.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Frames/SexObjectClass.py` & `srpastro_fits-3.0.3/SRPFITS/Frames/SexObjectClass.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Frames/SourceObjectsClass.py` & `srpastro_fits-3.0.3/SRPFITS/Frames/SourceObjectsClass.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Frames/WCS2Pixel.py` & `srpastro_fits-3.0.3/SRPFITS/Frames/WCS2Pixel.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Frames/__init__.py` & `srpastro_fits-3.0.3/SRPFITS/Frames/__init__.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Frames/getCenterRADEC.py` & `srpastro_fits-3.0.3/SRPFITS/Frames/getCenterRADEC.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/GetFWHM.py` & `srpastro_fits-3.0.3/SRPFITS/GetFWHM.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Math/TriangleMatch.py` & `srpastro_fits-3.0.3/SRPFITS/Math/TriangleMatch.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Photometry/ApErr.py` & `srpastro_fits-3.0.3/SRPFITS/Photometry/ApErr.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Photometry/ApyPhot.py` & `srpastro_fits-3.0.3/SRPFITS/Photometry/ApyPhot.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Photometry/Counts2Mag.py` & `srpastro_fits-3.0.3/SRPFITS/Photometry/Counts2Mag.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """ Utility functions and classes for SRP
 
 Context : SRP
 Module  : Photometry
-Version : 1.0.0
+Version : 1.1.0
 Author  : Stefano Covino
-Date    : 15/02/2012
-E-mail  : stefano.covino@brera.inaf.it
+Date    : 30/11/2034
+E-mail  : stefano.covino@inaf.it
 URL:    : http://www.merate.mi.astro.it/utenti/covino
 
 Usage   : to be imported
 
 Remarks : 
     
 History : (15/02/2012) First version.
-
+        : (30/11/2023) Zeropoint error. 
 """
 
 import math
 import numpy
 
 
-def Counts2Mag (cnt, ecnt, zp=0.0):
+def Counts2Mag (cnt, ecnt, zp=0.0, ezp=0.0):
     mag = -2.5*numpy.log10(numpy.array(cnt)) + zp
     emag = (2.5/math.log(10))*(numpy.array(ecnt)/numpy.array(cnt))
+    emag = numpy.sqrt(emag**2 + ezp**2)
     return mag, emag
```

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Photometry/DaoPhot.py` & `srpastro_fits-3.0.3/SRPFITS/Photometry/DaoPhot.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Photometry/FitsPhotometryClass.py` & `srpastro_fits-3.0.3/SRPFITS/Photometry/FitsPhotometryClass.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,70 @@
 """ Utility functions and classes for SRP
 
 Context : SRP
 Module  : PhotometryClass.py
 Version : 1.0.0
 Author  : Stefano Covino
-Date    : 10/08/2022
+Date    : 02/02/2024
 E-mail  : stefano.covino@inaf.it
 URL:    : http://www.merate.mi.astro.it/utenti/covino
 
 Usage   : to be imported
 
 Remarks :
 
-History : (10/08/2022) First version.
+History : (02/02/2024) First version.
 """
 
 #import os
 import numpy
 from astropy.table import Table
 import sep
 from SRPFITS.Photometry.ApyPhot import ApyPhot
 #from SRPFITS.Photometry.DaoPhot import DaoPhot
-
-#from .GetData import GetData
+from SRPFITS.Fits.GetData import GetData
 #from .GetHeader import GetHeader
 #from SRPFITS.Fits.GetWCS import GetWCS
 #from .GetHeaderValue import GetHeaderValue
 #from . import FitsConstants as FitsConstants
 #from SRPFITS.GetFWHM import GetFWHM
-
+from SRPFITS.Photometry.Counts2Mag import Counts2Mag
 #from SRPFITS.Frames.SourceObjectsClass import SourceObjects
 #from SRPFITS.Frames.SexObjectClass import SexObjects
 #from SRPFITS.Frames.DAOObjectClass import DAOObjects
 #from SRPFITS.Frames.Pixel2WCS import Pixel2WCS
 #from astropy import log
 #log.setLevel('WARNING')
 
 class FitsPhotometry:
-    def __init__ (self, fitsfile, objlist, exptime, airmass, extcoeff, zeropoint, level):
+    def __init__ (self, fitsfile, objlist, exptime=1., airmass=1., extcoeff=0., zeropoint=(25.0,0.0), level=3):
         self.Fitsfile = fitsfile
         self.ObjList = objlist
         self.Exptime = exptime
         self.Airmass = airmass
         self.ExtCoeff = extcoeff
         self.Zeropoint = zeropoint
         self.Level = level
 
     def GetImageData (self, extension=0):
-        self.Data = FitsImage (self.Fitsfile, extension).Data
+        try:
+            self.Data = GetData (self.Fitsfile, extension)[0]
+            return True
+        except:
+            return False
+        
+    def GetObjPos (self):
+        try:
+            iftab = Table.read(self.ObjList,format='ascii')
+            self.X = iftab.columns[1]
+            self.Y = iftab.columns[2]
+            return True
+        except:
+            return False
+    
     
     def SexPhotometry (self):
         # From here: https://python.hotexamples.com/it/examples/sep/-/set_extract_pixstack/python-set_extract_pixstack-function-examples.html
         data = self.Data
         #
         try:
             bkg = sep.Background(data)
@@ -109,19 +122,35 @@
         sources['y'] += 1.0
         sources['xpeak'] += 1
         sources['ypeak'] += 1
         sources['xwin'] += 1.0
         sources['ywin'] += 1.0
         sources['theta'] = np.degrees(sources['theta'])
         #
+        # Exptime
+        flux, fluxerr = flux/self.Exptime, fluxerr/self.Exptime
         # Convert to magnitudes
+        # Zero point
+        mag,magerr = Counts2Mag(flux,fluxerr,self.Zeropoint[0],self.Zeropoint[1])
+        # Airmass
+        mag = msg - self.ExtCoeff*self.Airmass
+        #
+        sources['mag'] = mag
+        sources['emag'] = magerr
+        return sources
         
         
     def ApyPhotometry (self, rds=(5,10,15),backgr=True,gain=1.,ron=0.):
             flux,fluxerr = ApyPhot (self.X,self.Y,self.Data,rds,backgr,gain,ron)
-            return Table([self.X,self.Y,flux,fluxerr],names=('X','Y','Flux','eFlux'))
+            # Exptime
+            flux, fluxerr = flux/self.Exptime, fluxerr/self.Exptime
+            # Zero point
+            mag, emag = Counts2Mag (flux,fluxerr,self.Zeropoint[0],self.Zeropoint[1])
+            # Airmass
+            mag = msg - self.ExtCoeff*self.Airmass
+            return Table([self.X,self.Y,flux,fluxerr,mag,emag],names=('X','Y','Flux','eFlux','Mag','eMag'))
 
                        
     #def DaoPhotometry (self, rds=(5,10,15),backgr=True,gain=1.,ron=0.,skyalg='mmm'):
     #        flux,fluxerr = DaoPhot (self.X,self.Y,self.Data,rds,backgr,gain,ron,skyalg)
     #        return Table([self.X,self.Y,flux,fluxerr],names=('X','Y','Flux','eFlux'))
```

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Photometry/MinMax.py` & `srpastro_fits-3.0.3/SRPFITS/Photometry/MinMax.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Photometry/__init__.py` & `srpastro_fits-3.0.3/SRPFITS/Photometry/__init__.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Photometry/centerGauss.py` & `srpastro_fits-3.0.3/SRPFITS/Photometry/centerGauss.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Photometry/centerMoment.py` & `srpastro_fits-3.0.3/SRPFITS/Photometry/centerMoment.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Photometry/centerObj.py` & `srpastro_fits-3.0.3/SRPFITS/Photometry/centerObj.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Photometry/getBackground.py` & `srpastro_fits-3.0.3/SRPFITS/Photometry/getBackground.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/Photometry/resid.py` & `srpastro_fits-3.0.3/SRPFITS/Photometry/resid.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/SRPFITSPath.py` & `srpastro_fits-3.0.3/SRPFITS/SRPFITSPath.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/SRPFITS/__init__.py` & `srpastro_fits-3.0.3/SRPFITS/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ 
 
 Context : SRP
 Module  : FITS
-Version : 1.9.4
+Version : 1.9.6
 Author  : Stefano Covino
-Date    : 22/05/2023
+Date    : 30/04/2024
 E-mail  : stefano.covino@inaf.it
 URL     : http://www.me.oa-brera.inaf.it/utenti/covino
 
 
 Usage   : to be imported
 
 Remarks :
@@ -72,17 +72,19 @@
         : (08/07/2021) V. 2.9.4.
         : (07/09/2021) V. 2.9.5.
         : (16/11/2021) V. 2.9.6.
         : (15/03/2022) V. 2.9.7.
         : (29/03/2022) V. 3.0.0beta.
         : (02/12/2022) V. 3.0.0.
         : (22/05/2023) V. 3.0.1.
+        : (06/07/2023) V. 3.0.2b.
+        : (30/04/2024) V. 3.0.3.
 """
 
-__version__ = '3.0.1'
+__version__ = '3.0.3'
 
 
 
 __all__ =  ['Fits', 'Frames', 'GetFWHM', 'Math', 'Photometry', 'SRPFITSPath']
```

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPAdvAverage` & `srpastro_fits-3.0.3/Scripts/SRPAdvAverage`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPAlignImaging` & `srpastro_fits-3.0.3/Scripts/SRPAlignImaging`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPAstrometry` & `srpastro_fits-3.0.3/Scripts/SRPAstrometry`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPAverage` & `srpastro_fits-3.0.3/Scripts/SRPAverage`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPBias` & `srpastro_fits-3.0.3/Scripts/SRPBias`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPClassify` & `srpastro_fits-3.0.3/Scripts/SRPClassify`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPCut` & `srpastro_fits-3.0.3/Scripts/SRPCut`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPDao2Sky` & `srpastro_fits-3.0.3/Scripts/SRPDao2Sky`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPFITSVersion` & `srpastro_fits-3.0.3/Scripts/SRPFITSVersion`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPFindingChart` & `srpastro_fits-3.0.3/Scripts/SRPFindingChart`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPFitsComposer` & `srpastro_fits-3.0.3/Scripts/SRPFitsComposer`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPFitsExtension` & `srpastro_fits-3.0.3/Scripts/SRPFitsExtension`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPFitsHeaders` & `srpastro_fits-3.0.3/Scripts/SRPFitsHeaders`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPFitsSpectrum2ASCII` & `srpastro_fits-3.0.3/Scripts/SRPFitsSpectrum2ASCII`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPFitsStats` & `srpastro_fits-3.0.3/Scripts/SRPFitsStats`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPFitsTableViewer` & `srpastro_fits-3.0.3/Scripts/SRPFitsTableViewer`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPFlatImaging` & `srpastro_fits-3.0.3/Scripts/SRPFlatImaging`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPFlatSpectroscopy` & `srpastro_fits-3.0.3/Scripts/SRPFlatSpectroscopy`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPGAIA2Sky` & `srpastro_fits-3.0.3/Scripts/SRPGAIA2Sky`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPImageFilter` & `srpastro_fits-3.0.3/Scripts/SRPImageFilter`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPImageMapping` & `srpastro_fits-3.0.3/Scripts/SRPImageMapping`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPKeywords` & `srpastro_fits-3.0.3/Scripts/SRPKeywords`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPPhotParSet` & `srpastro_fits-3.0.3/Scripts/SRPPhotParSet`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPPhotometry` & `srpastro_fits-3.0.3/Scripts/SRPPhotometry`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPQuery` & `srpastro_fits-3.0.3/Scripts/SRPQuery`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPRTAlignImaging` & `srpastro_fits-3.0.3/Scripts/SRPRTAlignImaging`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPRotoTransla` & `srpastro_fits-3.0.3/Scripts/SRPRotoTransla`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPScienceFramesImaging` & `srpastro_fits-3.0.3/Scripts/SRPScienceFramesImaging`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPSourceFinder` & `srpastro_fits-3.0.3/Scripts/SRPSourceFinder`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPSourcePhotometry` & `srpastro_fits-3.0.3/Scripts/SRPSourcePhotometry`

 * *Files 19% similar despite different names*

```diff
@@ -1,94 +1,88 @@
 #! python
 """ Code to extract sources from a fits frame
 
 Context : SRP
 Module  : SRPSorcePhotometry
 Author  : Stefano Covino
-Date    : 22/05/2023
+Date    : 29/02/2024
 E-mail  : stefano.covino@inaf.it
 URL:    : http://www.merate.mi.astro.it/utenti/covino
 Purpose :
 
 
-History : (22/05/2023) First version.
+History : (29/02/2024) First version.
 """
 
-__version__ = '1.0.0'
+__version__ = '0.1.0'
 
 from SRPFITS.Photometry.FitsPhotometryClass import FitsPhotometry
 #from SRPFITS.Fits import FitsConstants
 from SRPFITS.Fits.IsFits import IsFits
 from SRP.SRPSystem.ReadTextFile import ReadTextFile
 import argparse
 
 
 parser = argparse.ArgumentParser()
-parser.add_argument("-a", "--airmass", action="store", nargs=1, type=float, default=0.0, help="Airmass", metavar='airmass')
-parser.add_argument("-e", "--exptime", action="store", nargs=1, type=float, default=1.0, help="Exposure time (s)", metavar='exptime')
-parser.add_argument("-f", "--fitsfile", action="store", nargs=1, help="Input FITS file", metavar='ifits')
-parser.add_argument("-i", "--inputtab", action="store", nargs=1, help="Input file with star position", metavar='itab')
-parser.add_argument("-k", "--extcoeff", action="store", nargs=1, type=float, default=0.0, help="Extinction coefficient (mag)", metavar='extcoeff')
+parser.add_argument("-a", "--airmass", action="store", type=float, default=0.0, help="Airmass", metavar='airmass')
+parser.add_argument("-e", "--exptime", action="store", type=float, default=1.0, help="Exposure time (s)", metavar='exptime')
+parser.add_argument("-f", "--fitsfile", action="store", help="Input FITS file", metavar='ifits')
+parser.add_argument("-g", "--gain", action="store", type=float, default=1.0, help="Gain (ADU/e)", metavar='gain')
+parser.add_argument("-i", "--inputtab", action="store", help="Input file with star position", metavar='itab')
+parser.add_argument("-k", "--extcoeff", action="store", type=float, default=0.0, help="Extinction coefficient (mag)", metavar='extcoeff')
+parser.add_argument("-l", "--sexlev", action="store", type=float, default=3.0, help="Deepness of SEXTractor search", metavar='sexlev')
+parser.add_argument("-n", "--ron", action="store", type=float, default=1.0, help="RON (ADU)", metavar='ron')
+parser.add_argument("-r", "--photradii", action="store", type=float, nargs=3, default=(4.0,8.0,12.0), help="Inner, Outer and Background radii", metavar='photradii')
 parser.add_argument("-w", "--whichphotalg", choices=['sex','apyap'], default='apyap', help="Photometric algorithm")
-#parser.add_argument("-o", "--object", action="store", nargs=2, type=float, required=True, help="Object coordinates (hh.ddd dd.ddd)", metavar=('RA','DEC'))
-#parser.add_argument("-p", "--framepath", action="store", required=True, help="Base path for FITS frames", metavar='frpath')
-#parser.add_argument("-s", "--selpattern", action="store", default='*.fits', help="Selection pattern", metavar='spatt')
 parser.add_argument("-v", "--verbose", action="store_true", help="Fully describe operations")
 parser.add_argument("--version", action="version", version=__version__)
 parser.add_argument("-z", "--zeropoints", action="store", nargs=2, type=float, default=(25.0,0.0), help="Zero point (mag, magerr)", metavar=('mag','magerr'))
 options = parser.parse_args()
 
 
 
 if options.fitsfile and options.inputtab:
     if not IsFits(options.fitsfile):
         parser.error("Fits file %s not found." % options.fitsfile)
     #
     ifile = ReadTextFile(options.inputtab)
-    if ifile != None:
+    if ifile == None:
         parser.error("Input file %s not found or not readable." % options.inputtab)
     #
     if options.exptime <= 0:
         parser.error("Improper exposure time: %.3f." % options.exptime)
     #
     if options.airmass < 0:
         parser.error("Improper airmass: %.3f." % options.airmass)
     #
-    fphot = FitsPhotometry(options.fitsfile,ifile,option.exptime,options.airmass,optins.extcoeff,options.zeropoints)
+    if options.extcoeff < 0:
+        parser.error("Improper extinction coefficent: %.3f." % options.extcoeff)
     #
-    if options.whichphotlag == 'apyap':
-        pass
+    if options.sexlev < 0 and options.whchhotalg == 'sex:
+        parser.error("Improper SEXtractor search level: %.1f." % options.sexlev)
+    #
+    fphot = FitsPhotometry(options.fitsfile,ifile,options.exptime,options.airmass,options.extcoeff,options.zeropoints)
+    # Read fits file
+    if not fphot.GetImageData():
+        parser.error("Problem in accessing image data.")
+    # Read obj file
+    if not fphot.GetObjPos():
+        parser.error("Problem in accessing objlist data.")
+    #
+    if options.whichphotalg == 'apyap':
+        resphot = fphot.ApyPhotometry (rds=options.photradii,backgr=True,gain=options.gain,ron=options.ron)
     elif options.whchhotalg == 'sex':
-        pass
-
-    sys.exit(1)
-
+        resphot = fphot.SexPhotometry ()
+    #     
+        
+    print(resphot)
+    
+    sys.exit(0)
 
-    # Open file
-    if options.verbose:
-        print("Opening FITS file %s" % options.fits)
-    d = FitsImage(options.fits)
-    if d == None:
-        parser.error("Problem in reading FITS file %s" % options.fits)
-
-    # Sources
-    if options.verbose:
-        print("Source extraction...")
-    if options.daophot:
-        d.DAOSources(options.thre)
-    elif options.native:
-        d.Sources(options.thre,options.minpix)
-    elif options.sex:
-        d.SexSources(options.thre)
-    if options.verbose:
-        print("FWHM computation...")
-    d.GetFWHM()
-    if options.verbose:
-        print("Source list sorting...")
-    d.SortSourceList()
+    
 
     # Save results
     froot,fext = os.path.splitext(options.fits)
     if options.skycat:
         fname = froot+FitsConstants.SkyData
     else:
         fname = froot+FitsConstants.RegData
```

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPSpectralExtraction` & `srpastro_fits-3.0.3/Scripts/SRPSpectralExtraction`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! python
 """ Code to derive instrumental Stokes parameters
     
 Context : SRP
 Module  : SRPSpectralExtraction
 Author  : Stefano Covino
-Date    : 26/05/2017
+Date    : 30/04/2024
 E-mail  : stefano.covino@brera.inaf.it
 URL:    : http://www.merate.mi.astro.it/utenti/covino
 Purpose : Extract spectra from 2D frames
 
 usage   : SRPSpectralExtraction [-h] [-c clip value] [-e ext] -i file
             [-l pixel pixel] [-m] -s pixel pixel [-v]
             [--version] [-u pixel pixel]
@@ -23,26 +23,27 @@
             -u Upper sky window (pixel)
     
 History : (28/03/2013) First version.
         : (03/04/2013) Automatic spectrum location.
         : (25/03/2014) Deal with non standard FITS headers.
         : (18/05/2017) Minor update.
         : (26/05/2017) Minor update.
+        : (30/04/2024) Bug correction.
 """
 
-__version__ = '1.1.3'
+__version__ = '1.1.4'
 
 
 import argparse, os, warnings
 from SRPFITS.Fits.AddHeaderComment import AddHeaderComment
 from SRPFITS.Fits.GetData import GetData
 from SRPFITS.Fits.GetHeader import GetHeader
 from SRPFITS.Fits.IsFits import IsFits
 from SRPFITS.Fits.GetSpectrumPosition import GetSpectrumPosition
-from SRP.SRPStatistics.AverIterSigmaClipp import AverIterSigmaClipp
+from SRPSTATS.AverIterSigmaClipp import AverIterSigmaClipp
 import numpy
 from astropy.io import fits
 
 
 skyext = '_sky'
 skysub = '_skysub'
 obj    = '_obj'
```

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPWCSPixel` & `srpastro_fits-3.0.3/Scripts/SRPWCSPixel`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/Scripts/SRPZeroPoint` & `srpastro_fits-3.0.3/Scripts/SRPZeroPoint`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/AddHeaderComment.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Fits/AddHeaderComment.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/AddHeaderEntry.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Fits/AddHeaderEntry.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/FitsConstants.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Fits/FitsConstants.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/FitsImageClass.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Fits/FitsImageClass.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/FitsTabsAppend.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Fits/FitsTabsAppend.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/GetData.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Fits/GetData.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/GetHeader.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Fits/GetHeader.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/GetHeaderValue.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Fits/GetHeaderValue.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/GetSpectrum.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Fits/GetSpectrum.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/GetSpectrumPosition.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Fits/GetSpectrumPosition.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/GetWCS.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Fits/GetWCS.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/IsFits.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Fits/IsFits.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/WCSRotationDeg.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Fits/WCSRotationDeg.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Fits/__init__.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Fits/__init__.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/AstrometryClass.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Frames/AstrometryClass.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/DAOObjectClass.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Frames/DAOObjectClass.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/EclipseObjectClass.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Frames/EclipseObjectClass.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/Pixel2WCS.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Frames/Pixel2WCS.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/SExtractorConstants.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Frames/SExtractorConstants.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/SexObjectClass.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Frames/SexObjectClass.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/SourceObjectsClass.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Frames/SourceObjectsClass.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/WCS2Pixel.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Frames/WCS2Pixel.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/__init__.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Frames/__init__.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Frames/getCenterRADEC.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Frames/getCenterRADEC.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/GetFWHM.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/GetFWHM.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Math/TriangleMatch.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Math/TriangleMatch.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/ApErr.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Photometry/ApErr.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/ApyPhot.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Photometry/ApyPhot.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/Counts2Mag.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Photometry/Counts2Mag.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """ Utility functions and classes for SRP
 
 Context : SRP
 Module  : Photometry
-Version : 1.0.0
+Version : 1.1.0
 Author  : Stefano Covino
-Date    : 15/02/2012
-E-mail  : stefano.covino@brera.inaf.it
+Date    : 30/11/2034
+E-mail  : stefano.covino@inaf.it
 URL:    : http://www.merate.mi.astro.it/utenti/covino
 
 Usage   : to be imported
 
 Remarks : 
     
 History : (15/02/2012) First version.
-
+        : (30/11/2023) Zeropoint error. 
 """
 
 import math
 import numpy
 
 
-def Counts2Mag (cnt, ecnt, zp=0.0):
+def Counts2Mag (cnt, ecnt, zp=0.0, ezp=0.0):
     mag = -2.5*numpy.log10(numpy.array(cnt)) + zp
     emag = (2.5/math.log(10))*(numpy.array(ecnt)/numpy.array(cnt))
+    emag = numpy.sqrt(emag**2 + ezp**2)
     return mag, emag
```

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/DaoPhot.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Photometry/DaoPhot.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/FitsPhotometryClass.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Photometry/FitsPhotometryClass.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,70 @@
 """ Utility functions and classes for SRP
 
 Context : SRP
 Module  : PhotometryClass.py
 Version : 1.0.0
 Author  : Stefano Covino
-Date    : 10/08/2022
+Date    : 02/02/2024
 E-mail  : stefano.covino@inaf.it
 URL:    : http://www.merate.mi.astro.it/utenti/covino
 
 Usage   : to be imported
 
 Remarks :
 
-History : (10/08/2022) First version.
+History : (02/02/2024) First version.
 """
 
 #import os
 import numpy
 from astropy.table import Table
 import sep
 from SRPFITS.Photometry.ApyPhot import ApyPhot
 #from SRPFITS.Photometry.DaoPhot import DaoPhot
-
-#from .GetData import GetData
+from SRPFITS.Fits.GetData import GetData
 #from .GetHeader import GetHeader
 #from SRPFITS.Fits.GetWCS import GetWCS
 #from .GetHeaderValue import GetHeaderValue
 #from . import FitsConstants as FitsConstants
 #from SRPFITS.GetFWHM import GetFWHM
-
+from SRPFITS.Photometry.Counts2Mag import Counts2Mag
 #from SRPFITS.Frames.SourceObjectsClass import SourceObjects
 #from SRPFITS.Frames.SexObjectClass import SexObjects
 #from SRPFITS.Frames.DAOObjectClass import DAOObjects
 #from SRPFITS.Frames.Pixel2WCS import Pixel2WCS
 #from astropy import log
 #log.setLevel('WARNING')
 
 class FitsPhotometry:
-    def __init__ (self, fitsfile, objlist, exptime, airmass, extcoeff, zeropoint, level):
+    def __init__ (self, fitsfile, objlist, exptime=1., airmass=1., extcoeff=0., zeropoint=(25.0,0.0), level=3):
         self.Fitsfile = fitsfile
         self.ObjList = objlist
         self.Exptime = exptime
         self.Airmass = airmass
         self.ExtCoeff = extcoeff
         self.Zeropoint = zeropoint
         self.Level = level
 
     def GetImageData (self, extension=0):
-        self.Data = FitsImage (self.Fitsfile, extension).Data
+        try:
+            self.Data = GetData (self.Fitsfile, extension)[0]
+            return True
+        except:
+            return False
+        
+    def GetObjPos (self):
+        try:
+            iftab = Table.read(self.ObjList,format='ascii')
+            self.X = iftab.columns[1]
+            self.Y = iftab.columns[2]
+            return True
+        except:
+            return False
+    
     
     def SexPhotometry (self):
         # From here: https://python.hotexamples.com/it/examples/sep/-/set_extract_pixstack/python-set_extract_pixstack-function-examples.html
         data = self.Data
         #
         try:
             bkg = sep.Background(data)
@@ -109,19 +122,35 @@
         sources['y'] += 1.0
         sources['xpeak'] += 1
         sources['ypeak'] += 1
         sources['xwin'] += 1.0
         sources['ywin'] += 1.0
         sources['theta'] = np.degrees(sources['theta'])
         #
+        # Exptime
+        flux, fluxerr = flux/self.Exptime, fluxerr/self.Exptime
         # Convert to magnitudes
+        # Zero point
+        mag,magerr = Counts2Mag(flux,fluxerr,self.Zeropoint[0],self.Zeropoint[1])
+        # Airmass
+        mag = msg - self.ExtCoeff*self.Airmass
+        #
+        sources['mag'] = mag
+        sources['emag'] = magerr
+        return sources
         
         
     def ApyPhotometry (self, rds=(5,10,15),backgr=True,gain=1.,ron=0.):
             flux,fluxerr = ApyPhot (self.X,self.Y,self.Data,rds,backgr,gain,ron)
-            return Table([self.X,self.Y,flux,fluxerr],names=('X','Y','Flux','eFlux'))
+            # Exptime
+            flux, fluxerr = flux/self.Exptime, fluxerr/self.Exptime
+            # Zero point
+            mag, emag = Counts2Mag (flux,fluxerr,self.Zeropoint[0],self.Zeropoint[1])
+            # Airmass
+            mag = msg - self.ExtCoeff*self.Airmass
+            return Table([self.X,self.Y,flux,fluxerr,mag,emag],names=('X','Y','Flux','eFlux','Mag','eMag'))
 
                        
     #def DaoPhotometry (self, rds=(5,10,15),backgr=True,gain=1.,ron=0.,skyalg='mmm'):
     #        flux,fluxerr = DaoPhot (self.X,self.Y,self.Data,rds,backgr,gain,ron,skyalg)
     #        return Table([self.X,self.Y,flux,fluxerr],names=('X','Y','Flux','eFlux'))
```

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/MinMax.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Photometry/MinMax.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/__init__.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Photometry/__init__.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/centerGauss.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Photometry/centerGauss.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/centerMoment.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Photometry/centerMoment.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/centerObj.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Photometry/centerObj.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/getBackground.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Photometry/getBackground.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/Photometry/resid.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/Photometry/resid.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/SRPFITSPath.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/SRPFITSPath.py`

 * *Files identical despite different names*

### Comparing `SRPAstro.FITS-3.0.1/build/lib/SRPFITS/__init__.py` & `srpastro_fits-3.0.3/build/lib/SRPFITS/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ 
 
 Context : SRP
 Module  : FITS
-Version : 1.9.4
+Version : 1.9.6
 Author  : Stefano Covino
-Date    : 22/05/2023
+Date    : 30/04/2024
 E-mail  : stefano.covino@inaf.it
 URL     : http://www.me.oa-brera.inaf.it/utenti/covino
 
 
 Usage   : to be imported
 
 Remarks :
@@ -72,17 +72,19 @@
         : (08/07/2021) V. 2.9.4.
         : (07/09/2021) V. 2.9.5.
         : (16/11/2021) V. 2.9.6.
         : (15/03/2022) V. 2.9.7.
         : (29/03/2022) V. 3.0.0beta.
         : (02/12/2022) V. 3.0.0.
         : (22/05/2023) V. 3.0.1.
+        : (06/07/2023) V. 3.0.2b.
+        : (30/04/2024) V. 3.0.3.
 """
 
-__version__ = '3.0.1'
+__version__ = '3.0.3'
 
 
 
 __all__ =  ['Fits', 'Frames', 'GetFWHM', 'Math', 'Photometry', 'SRPFITSPath']
```

### Comparing `SRPAstro.FITS-3.0.1/setup.py` & `srpastro_fits-3.0.3/setup.py`

 * *Files identical despite different names*

