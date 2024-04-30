# Comparing `tmp/WITecSDK-1.2.4.tar.gz` & `tmp/witecsdk-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WITecSDK-1.2.4.tar", last modified: Thu Mar 14 15:24:09 2024, max compression
+gzip compressed data, was "witecsdk-1.2.5.tar", last modified: Tue Apr 30 10:51:23 2024, max compression
```

## Comparing `WITecSDK-1.2.4.tar` & `witecsdk-1.2.5.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2024-03-14 15:24:08.849650 WITecSDK-1.2.4/
--rw-rw-rw-   0        0        0     3498 2024-03-14 15:24:08.865286 WITecSDK-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     2956 2024-03-14 15:06:42.000000 WITecSDK-1.2.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-14 15:24:02.391671 WITecSDK-1.2.4/WITecSDK/
--rw-rw-rw-   0        0        0     3312 2024-03-07 11:07:34.000000 WITecSDK-1.2.4/WITecSDK/COMClientBase.py
--rw-rw-rw-   0        0        0     2538 2024-03-07 11:07:34.000000 WITecSDK-1.2.4/WITecSDK/COMClientComTyp.py
--rw-rw-rw-   0        0        0     2021 2024-03-07 11:07:34.000000 WITecSDK-1.2.4/WITecSDK/COMClientW32Com.py
-drwxrwxrwx   0        0        0        0 2024-03-14 15:24:07.255735 WITecSDK-1.2.4/WITecSDK/Modules/
--rw-rw-rw-   0        0        0     3343 2024-03-07 11:07:34.000000 WITecSDK-1.2.4/WITecSDK/Modules/ActiveSequencer.py
--rw-rw-rw-   0        0        0      810 2023-07-31 18:45:21.000000 WITecSDK-1.2.4/WITecSDK/Modules/ApertureFieldStop.py
--rw-rw-rw-   0        0        0     1162 2023-07-24 21:55:42.000000 WITecSDK-1.2.4/WITecSDK/Modules/ApplicationControl.py
--rw-rw-rw-   0        0        0     1043 2023-12-11 14:23:11.000000 WITecSDK-1.2.4/WITecSDK/Modules/AutoFocus.py
--rw-rw-rw-   0        0        0     4377 2024-03-14 15:03:29.000000 WITecSDK-1.2.4/WITecSDK/Modules/BeamPath.py
--rw-rw-rw-   0        0        0      498 2023-07-31 18:47:40.000000 WITecSDK-1.2.4/WITecSDK/Modules/ConfigurationLoader.py
--rw-rw-rw-   0        0        0     1838 2023-08-01 07:47:22.000000 WITecSDK-1.2.4/WITecSDK/Modules/DetectorOutput.py
--rw-rw-rw-   0        0        0     1232 2023-07-31 18:47:48.000000 WITecSDK-1.2.4/WITecSDK/Modules/FastTimeSeries.py
--rw-rw-rw-   0        0        0     2264 2023-07-31 18:47:55.000000 WITecSDK-1.2.4/WITecSDK/Modules/Heating.py
--rw-rw-rw-   0        0        0     6496 2023-07-31 14:43:26.000000 WITecSDK-1.2.4/WITecSDK/Modules/HelperStructs.py
--rw-rw-rw-   0        0        0     1409 2024-01-09 15:22:48.000000 WITecSDK-1.2.4/WITecSDK/Modules/Illumination.py
--rw-rw-rw-   0        0        0     7317 2024-01-08 14:57:27.000000 WITecSDK-1.2.4/WITecSDK/Modules/LargeAreaScan.py
--rw-rw-rw-   0        0        0     4761 2024-01-10 15:06:45.000000 WITecSDK-1.2.4/WITecSDK/Modules/LaserManager.py
--rw-rw-rw-   0        0        0     1788 2024-01-10 12:38:21.000000 WITecSDK-1.2.4/WITecSDK/Modules/LaserPowerSeries.py
--rw-rw-rw-   0        0        0     4460 2024-01-10 13:48:34.000000 WITecSDK-1.2.4/WITecSDK/Modules/LineScan.py
--rw-rw-rw-   0        0        0     2983 2023-07-31 18:50:15.000000 WITecSDK-1.2.4/WITecSDK/Modules/ManualTopography.py
--rw-rw-rw-   0        0        0      826 2023-07-31 18:50:27.000000 WITecSDK-1.2.4/WITecSDK/Modules/ObjectiveTurret.py
--rw-rw-rw-   0        0        0     1421 2024-03-07 11:07:34.000000 WITecSDK-1.2.4/WITecSDK/Modules/ParameterNameGetter.py
--rw-rw-rw-   0        0        0     5856 2024-03-14 15:08:24.000000 WITecSDK-1.2.4/WITecSDK/Modules/Polarization.py
--rw-rw-rw-   0        0        0     4964 2024-03-07 11:07:34.000000 WITecSDK-1.2.4/WITecSDK/Modules/ProjectCreatorSaver.py
--rw-rw-rw-   0        0        0     1046 2023-07-31 18:51:23.000000 WITecSDK-1.2.4/WITecSDK/Modules/SampleName.py
--rw-rw-rw-   0        0        0     3666 2024-01-09 15:23:59.000000 WITecSDK-1.2.4/WITecSDK/Modules/SamplePositioner.py
--rw-rw-rw-   0        0        0     2922 2023-07-31 18:51:50.000000 WITecSDK-1.2.4/WITecSDK/Modules/SilentSpectrum.py
--rw-rw-rw-   0        0        0     2611 2024-01-10 13:34:51.000000 WITecSDK-1.2.4/WITecSDK/Modules/SingleSpectrum.py
--rw-rw-rw-   0        0        0     5058 2024-03-07 11:19:56.000000 WITecSDK-1.2.4/WITecSDK/Modules/SlowTimeSeriesBase.py
--rw-rw-rw-   0        0        0     2058 2024-03-07 11:19:56.000000 WITecSDK-1.2.4/WITecSDK/Modules/SlowTimeSeriesManual.py
--rw-rw-rw-   0        0        0     1032 2024-03-07 11:19:56.000000 WITecSDK-1.2.4/WITecSDK/Modules/SlowTimeSeriesTimed.py
--rw-rw-rw-   0        0        0     3958 2024-01-09 16:12:40.000000 WITecSDK-1.2.4/WITecSDK/Modules/SpectralAutofocus.py
--rw-rw-rw-   0        0        0     1925 2024-03-14 15:18:50.000000 WITecSDK-1.2.4/WITecSDK/Modules/SpectralStitching.py
--rw-rw-rw-   0        0        0     1680 2023-12-11 11:21:08.000000 WITecSDK-1.2.4/WITecSDK/Modules/Spectrograph.py
--rw-rw-rw-   0        0        0      742 2023-12-12 11:10:14.000000 WITecSDK-1.2.4/WITecSDK/Modules/StateManager.py
--rw-rw-rw-   0        0        0     2512 2023-12-12 11:52:21.000000 WITecSDK-1.2.4/WITecSDK/Modules/TrueSurface.py
--rw-rw-rw-   0        0        0     6930 2024-01-09 15:47:02.000000 WITecSDK-1.2.4/WITecSDK/Modules/VideoControl.py
--rw-rw-rw-   0        0        0      774 2024-03-14 15:07:22.000000 WITecSDK-1.2.4/WITecSDK/Modules/WITecControlVersionTester.py
--rw-rw-rw-   0        0        0     5908 2023-07-31 18:59:14.000000 WITecSDK-1.2.4/WITecSDK/Modules/XYAxes.py
--rw-rw-rw-   0        0        0    10518 2024-01-09 15:47:11.000000 WITecSDK-1.2.4/WITecSDK/Modules/ZAxis.py
--rw-rw-rw-   0        0        0    20477 2024-03-14 14:58:40.000000 WITecSDK-1.2.4/WITecSDK/Modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-14 15:24:07.677678 WITecSDK-1.2.4/WITecSDK/Parameters/
--rw-rw-rw-   0        0        0     1232 2023-07-25 20:06:09.000000 WITecSDK-1.2.4/WITecSDK/Parameters/COMEnumParameter.py
--rw-rw-rw-   0        0        0     1352 2024-03-07 11:07:35.000000 WITecSDK-1.2.4/WITecSDK/Parameters/COMFillStatusParameter.py
--rw-rw-rw-   0        0        0     1683 2024-03-07 11:07:35.000000 WITecSDK-1.2.4/WITecSDK/Parameters/COMFloatParameter.py
--rw-rw-rw-   0        0        0     1659 2024-03-07 11:07:35.000000 WITecSDK-1.2.4/WITecSDK/Parameters/COMIntParameter.py
--rw-rw-rw-   0        0        0     1450 2024-03-07 11:07:35.000000 WITecSDK-1.2.4/WITecSDK/Parameters/COMParameter.py
--rw-rw-rw-   0        0        0     2640 2024-03-07 11:07:35.000000 WITecSDK-1.2.4/WITecSDK/Parameters/COMParameterBase.py
--rw-rw-rw-   0        0        0     2110 2024-03-07 11:07:35.000000 WITecSDK-1.2.4/WITecSDK/Parameters/COMStatusParameter.py
--rw-rw-rw-   0        0        0     7317 2024-03-07 11:07:35.000000 WITecSDK-1.2.4/WITecSDK/Parameters/__init__.py
--rw-rw-rw-   0        0        0     3190 2024-03-07 11:19:56.000000 WITecSDK-1.2.4/WITecSDK/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-14 15:24:08.771530 WITecSDK-1.2.4/WITecSDK.egg-info/
--rw-rw-rw-   0        0        0     3498 2024-03-14 15:24:00.000000 WITecSDK-1.2.4/WITecSDK.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1915 2024-03-14 15:24:01.000000 WITecSDK-1.2.4/WITecSDK.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-14 15:24:00.000000 WITecSDK-1.2.4/WITecSDK.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-03-14 15:24:00.000000 WITecSDK-1.2.4/WITecSDK.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-03-14 15:24:00.000000 WITecSDK-1.2.4/WITecSDK.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      762 2024-03-14 15:06:53.000000 WITecSDK-1.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-14 15:24:08.990287 WITecSDK-1.2.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-14 15:24:08.584023 WITecSDK-1.2.4/tests/
--rw-rw-rw-   0        0        0     2317 2024-03-14 15:10:29.000000 WITecSDK-1.2.4/tests/TestAllModules.py
+drwxrwxrwx   0        0        0        0 2024-04-30 10:51:22.235633 witecsdk-1.2.5/
+-rw-rw-rw-   0        0        0     3592 2024-04-30 10:51:22.391875 witecsdk-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3049 2024-04-30 10:45:04.000000 witecsdk-1.2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 10:50:55.391904 witecsdk-1.2.5/WITecSDK/
+-rw-rw-rw-   0        0        0     3312 2024-04-30 10:38:55.000000 witecsdk-1.2.5/WITecSDK/COMClientBase.py
+-rw-rw-rw-   0        0        0     2538 2024-04-30 10:38:55.000000 witecsdk-1.2.5/WITecSDK/COMClientComTyp.py
+-rw-rw-rw-   0        0        0     2021 2024-04-30 10:38:56.000000 witecsdk-1.2.5/WITecSDK/COMClientW32Com.py
+drwxrwxrwx   0        0        0        0 2024-04-30 10:51:15.748325 witecsdk-1.2.5/WITecSDK/Modules/
+-rw-rw-rw-   0        0        0     3343 2024-04-30 10:38:56.000000 witecsdk-1.2.5/WITecSDK/Modules/ActiveSequencer.py
+-rw-rw-rw-   0        0        0      810 2023-07-31 18:45:21.000000 witecsdk-1.2.5/WITecSDK/Modules/ApertureFieldStop.py
+-rw-rw-rw-   0        0        0     1162 2023-07-24 21:55:42.000000 witecsdk-1.2.5/WITecSDK/Modules/ApplicationControl.py
+-rw-rw-rw-   0        0        0     1085 2024-04-30 10:40:12.000000 witecsdk-1.2.5/WITecSDK/Modules/AutoFocus.py
+-rw-rw-rw-   0        0        0     4377 2024-03-14 15:03:29.000000 witecsdk-1.2.5/WITecSDK/Modules/BeamPath.py
+-rw-rw-rw-   0        0        0      498 2023-07-31 18:47:40.000000 witecsdk-1.2.5/WITecSDK/Modules/ConfigurationLoader.py
+-rw-rw-rw-   0        0        0     1838 2023-08-01 07:47:22.000000 witecsdk-1.2.5/WITecSDK/Modules/DetectorOutput.py
+-rw-rw-rw-   0        0        0     1232 2023-07-31 18:47:48.000000 witecsdk-1.2.5/WITecSDK/Modules/FastTimeSeries.py
+-rw-rw-rw-   0        0        0     2264 2023-07-31 18:47:55.000000 witecsdk-1.2.5/WITecSDK/Modules/Heating.py
+-rw-rw-rw-   0        0        0     6496 2023-07-31 14:43:26.000000 witecsdk-1.2.5/WITecSDK/Modules/HelperStructs.py
+-rw-rw-rw-   0        0        0     1409 2024-01-09 15:22:48.000000 witecsdk-1.2.5/WITecSDK/Modules/Illumination.py
+-rw-rw-rw-   0        0        0     7317 2024-01-08 14:57:27.000000 witecsdk-1.2.5/WITecSDK/Modules/LargeAreaScan.py
+-rw-rw-rw-   0        0        0     4761 2024-01-10 15:06:45.000000 witecsdk-1.2.5/WITecSDK/Modules/LaserManager.py
+-rw-rw-rw-   0        0        0     1788 2024-01-10 12:38:21.000000 witecsdk-1.2.5/WITecSDK/Modules/LaserPowerSeries.py
+-rw-rw-rw-   0        0        0     4460 2024-01-10 13:48:34.000000 witecsdk-1.2.5/WITecSDK/Modules/LineScan.py
+-rw-rw-rw-   0        0        0     2983 2023-07-31 18:50:15.000000 witecsdk-1.2.5/WITecSDK/Modules/ManualTopography.py
+-rw-rw-rw-   0        0        0      826 2023-07-31 18:50:27.000000 witecsdk-1.2.5/WITecSDK/Modules/ObjectiveTurret.py
+-rw-rw-rw-   0        0        0     1421 2024-04-30 10:38:57.000000 witecsdk-1.2.5/WITecSDK/Modules/ParameterNameGetter.py
+-rw-rw-rw-   0        0        0     5856 2024-03-14 15:08:24.000000 witecsdk-1.2.5/WITecSDK/Modules/Polarization.py
+-rw-rw-rw-   0        0        0     4964 2024-04-30 10:38:57.000000 witecsdk-1.2.5/WITecSDK/Modules/ProjectCreatorSaver.py
+-rw-rw-rw-   0        0        0     1046 2023-07-31 18:51:23.000000 witecsdk-1.2.5/WITecSDK/Modules/SampleName.py
+-rw-rw-rw-   0        0        0     3666 2024-01-09 15:23:59.000000 witecsdk-1.2.5/WITecSDK/Modules/SamplePositioner.py
+-rw-rw-rw-   0        0        0     2922 2023-07-31 18:51:50.000000 witecsdk-1.2.5/WITecSDK/Modules/SilentSpectrum.py
+-rw-rw-rw-   0        0        0     2611 2024-01-10 13:34:51.000000 witecsdk-1.2.5/WITecSDK/Modules/SingleSpectrum.py
+-rw-rw-rw-   0        0        0     5058 2024-03-07 11:19:56.000000 witecsdk-1.2.5/WITecSDK/Modules/SlowTimeSeriesBase.py
+-rw-rw-rw-   0        0        0     2058 2024-03-07 11:19:56.000000 witecsdk-1.2.5/WITecSDK/Modules/SlowTimeSeriesManual.py
+-rw-rw-rw-   0        0        0     1032 2024-03-07 11:19:56.000000 witecsdk-1.2.5/WITecSDK/Modules/SlowTimeSeriesTimed.py
+-rw-rw-rw-   0        0        0     3958 2024-01-09 16:12:40.000000 witecsdk-1.2.5/WITecSDK/Modules/SpectralAutofocus.py
+-rw-rw-rw-   0        0        0     1925 2024-03-14 15:18:50.000000 witecsdk-1.2.5/WITecSDK/Modules/SpectralStitching.py
+-rw-rw-rw-   0        0        0     1680 2023-12-11 11:21:08.000000 witecsdk-1.2.5/WITecSDK/Modules/Spectrograph.py
+-rw-rw-rw-   0        0        0      742 2023-12-12 11:10:14.000000 witecsdk-1.2.5/WITecSDK/Modules/StateManager.py
+-rw-rw-rw-   0        0        0     2512 2023-12-12 11:52:21.000000 witecsdk-1.2.5/WITecSDK/Modules/TrueSurface.py
+-rw-rw-rw-   0        0        0     6930 2024-01-09 15:47:02.000000 witecsdk-1.2.5/WITecSDK/Modules/VideoControl.py
+-rw-rw-rw-   0        0        0      852 2024-04-30 10:40:59.000000 witecsdk-1.2.5/WITecSDK/Modules/WITecControlVersionTester.py
+-rw-rw-rw-   0        0        0     5908 2023-07-31 18:59:14.000000 witecsdk-1.2.5/WITecSDK/Modules/XYAxes.py
+-rw-rw-rw-   0        0        0    10518 2024-01-09 15:47:11.000000 witecsdk-1.2.5/WITecSDK/Modules/ZAxis.py
+-rw-rw-rw-   0        0        0    20477 2024-03-14 14:58:40.000000 witecsdk-1.2.5/WITecSDK/Modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 10:51:20.328771 witecsdk-1.2.5/WITecSDK/Parameters/
+-rw-rw-rw-   0        0        0     1232 2023-07-25 20:06:09.000000 witecsdk-1.2.5/WITecSDK/Parameters/COMEnumParameter.py
+-rw-rw-rw-   0        0        0     1352 2024-04-30 10:38:58.000000 witecsdk-1.2.5/WITecSDK/Parameters/COMFillStatusParameter.py
+-rw-rw-rw-   0        0        0     1683 2024-04-30 10:38:58.000000 witecsdk-1.2.5/WITecSDK/Parameters/COMFloatParameter.py
+-rw-rw-rw-   0        0        0     1659 2024-04-30 10:38:58.000000 witecsdk-1.2.5/WITecSDK/Parameters/COMIntParameter.py
+-rw-rw-rw-   0        0        0     1450 2024-04-30 10:38:59.000000 witecsdk-1.2.5/WITecSDK/Parameters/COMParameter.py
+-rw-rw-rw-   0        0        0     2640 2024-04-30 10:38:59.000000 witecsdk-1.2.5/WITecSDK/Parameters/COMParameterBase.py
+-rw-rw-rw-   0        0        0     2110 2024-04-30 10:38:59.000000 witecsdk-1.2.5/WITecSDK/Parameters/COMStatusParameter.py
+-rw-rw-rw-   0        0        0     7317 2024-04-30 10:39:00.000000 witecsdk-1.2.5/WITecSDK/Parameters/__init__.py
+-rw-rw-rw-   0        0        0     3190 2024-04-30 10:39:00.000000 witecsdk-1.2.5/WITecSDK/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 10:51:21.891826 witecsdk-1.2.5/WITecSDK.egg-info/
+-rw-rw-rw-   0        0        0     3592 2024-04-30 10:50:49.000000 witecsdk-1.2.5/WITecSDK.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1915 2024-04-30 10:50:51.000000 witecsdk-1.2.5/WITecSDK.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 10:50:49.000000 witecsdk-1.2.5/WITecSDK.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-30 10:50:49.000000 witecsdk-1.2.5/WITecSDK.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-30 10:50:49.000000 witecsdk-1.2.5/WITecSDK.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      763 2024-04-30 10:45:11.000000 witecsdk-1.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-30 10:51:22.923184 witecsdk-1.2.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 10:51:20.907360 witecsdk-1.2.5/tests/
+-rw-rw-rw-   0        0        0     2317 2024-03-14 15:10:29.000000 witecsdk-1.2.5/tests/TestAllModules.py
```

### Comparing `WITecSDK-1.2.4/PKG-INFO` & `witecsdk-1.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: WITecSDK
-Version: 1.2.4
+Version: 1.2.5
 Summary: This package allows automation of WITec Control over COM
 Author-email: Matthias Finger <info@witec.de>
 License: MIT License
 Project-URL: Homepage, https://raman.oxinst.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: comtypes>=1.2.0
 
 This package enables control of WITec microscopes over its COM interface (additonal license required).
 
 - Gives access to data acquisition functions
 - Implements all classes of WITec's COM interface
@@ -43,14 +43,19 @@
 
 # Contribution and feature requests
 
 If you want to share your own extensions or have feature wishes please contact the [WITec support team](https://raman.oxinst.com/contact).
 
 # Changelog
 
+## Changes in 1.2.5
+
+- Bug in Autofocus fixed
+- Bug in WITecControlVersionTester fixed
+
 ## Changes in 1.2.4
 
 - Spectral Stitching added
 - WITecControlVersionTester reworked
 
 ## Changes in 1.2.3
```

### Comparing `WITecSDK-1.2.4/README.md` & `witecsdk-1.2.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,19 @@
 
 # Contribution and feature requests
 
 If you want to share your own extensions or have feature wishes please contact the [WITec support team](https://raman.oxinst.com/contact).
 
 # Changelog
 
+## Changes in 1.2.5
+
+- Bug in Autofocus fixed
+- Bug in WITecControlVersionTester fixed
+
 ## Changes in 1.2.4
 
 - Spectral Stitching added
 - WITecControlVersionTester reworked
 
 ## Changes in 1.2.3
```

### Comparing `WITecSDK-1.2.4/WITecSDK/COMClientBase.py` & `witecsdk-1.2.5/WITecSDK/COMClientBase.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/COMClientComTyp.py` & `witecsdk-1.2.5/WITecSDK/COMClientComTyp.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/COMClientW32Com.py` & `witecsdk-1.2.5/WITecSDK/COMClientW32Com.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/ActiveSequencer.py` & `witecsdk-1.2.5/WITecSDK/Modules/ActiveSequencer.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/ApertureFieldStop.py` & `witecsdk-1.2.5/WITecSDK/Modules/ApertureFieldStop.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/ApplicationControl.py` & `witecsdk-1.2.5/WITecSDK/Modules/ApplicationControl.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/AutoFocus.py` & `witecsdk-1.2.5/WITecSDK/Modules/AutoFocus.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     async def _waitForAutoFocus(self) -> bool:
         await sleep(5)
         return True
         
 class AutoFocus61(AutoFocus):
 
     def __init__(self, aCOMParameters: COMParameters):
+        super().__init__(aCOMParameters)
         self._statusAutoFocusCOM = aCOMParameters.GetEnumParameter(self._parampath + "AutoFocus|Status")
         #"Running", "LastSucceeded", "LastFailed"
 
     async def _waitForAutoFocus(self) -> bool:
         afstate: int = 0
         while afstate == 0:
             await sleep(0.1)
```

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/BeamPath.py` & `witecsdk-1.2.5/WITecSDK/Modules/BeamPath.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/DetectorOutput.py` & `witecsdk-1.2.5/WITecSDK/Modules/DetectorOutput.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/FastTimeSeries.py` & `witecsdk-1.2.5/WITecSDK/Modules/FastTimeSeries.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/Heating.py` & `witecsdk-1.2.5/WITecSDK/Modules/Heating.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/HelperStructs.py` & `witecsdk-1.2.5/WITecSDK/Modules/HelperStructs.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/Illumination.py` & `witecsdk-1.2.5/WITecSDK/Modules/Illumination.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/LargeAreaScan.py` & `witecsdk-1.2.5/WITecSDK/Modules/LargeAreaScan.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/LaserManager.py` & `witecsdk-1.2.5/WITecSDK/Modules/LaserManager.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/LaserPowerSeries.py` & `witecsdk-1.2.5/WITecSDK/Modules/LaserPowerSeries.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/LineScan.py` & `witecsdk-1.2.5/WITecSDK/Modules/LineScan.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/ManualTopography.py` & `witecsdk-1.2.5/WITecSDK/Modules/ManualTopography.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/ObjectiveTurret.py` & `witecsdk-1.2.5/WITecSDK/Modules/ObjectiveTurret.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/ParameterNameGetter.py` & `witecsdk-1.2.5/WITecSDK/Modules/ParameterNameGetter.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/Polarization.py` & `witecsdk-1.2.5/WITecSDK/Modules/Polarization.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/ProjectCreatorSaver.py` & `witecsdk-1.2.5/WITecSDK/Modules/ProjectCreatorSaver.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/SampleName.py` & `witecsdk-1.2.5/WITecSDK/Modules/SampleName.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/SamplePositioner.py` & `witecsdk-1.2.5/WITecSDK/Modules/SamplePositioner.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/SilentSpectrum.py` & `witecsdk-1.2.5/WITecSDK/Modules/SilentSpectrum.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/SingleSpectrum.py` & `witecsdk-1.2.5/WITecSDK/Modules/SingleSpectrum.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/SlowTimeSeriesBase.py` & `witecsdk-1.2.5/WITecSDK/Modules/SlowTimeSeriesBase.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/SlowTimeSeriesManual.py` & `witecsdk-1.2.5/WITecSDK/Modules/SlowTimeSeriesManual.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/SlowTimeSeriesTimed.py` & `witecsdk-1.2.5/WITecSDK/Modules/SlowTimeSeriesTimed.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/SpectralAutofocus.py` & `witecsdk-1.2.5/WITecSDK/Modules/SpectralAutofocus.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/SpectralStitching.py` & `witecsdk-1.2.5/WITecSDK/Modules/SpectralStitching.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/Spectrograph.py` & `witecsdk-1.2.5/WITecSDK/Modules/Spectrograph.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/StateManager.py` & `witecsdk-1.2.5/WITecSDK/Modules/StateManager.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/TrueSurface.py` & `witecsdk-1.2.5/WITecSDK/Modules/TrueSurface.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/VideoControl.py` & `witecsdk-1.2.5/WITecSDK/Modules/VideoControl.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/WITecControlVersionTester.py` & `witecsdk-1.2.5/WITecSDK/Modules/WITecControlVersionTester.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 ﻿from WITecSDK.Parameters import COMParameters
 
 class WITecControlVersionTester:
 
     def __init__(self, aCOMParameters: COMParameters):
         self._programVersionCOM = aCOMParameters.GetStringParameter("Status|Software|Application|ProgramVersion")
-        self.Version: float = float(self.StringVersion.split(",")[1].strip())
+        # Could be i.e. "WITec Control, 6.2 Develop, Build: 6.02.3.4"
+        self.Version: float = float(self.StringVersion.split(", ")[1].split(" ")[0])
         # Create IsVersionGreater... attributes
         versions: list[float,...] = [5.1, 5.2, 5.3, 6.0, 6.1, 6.2, 6.3]
         isversions: list[bool,...] = [(str(int(ver * 10)), self.Version >= ver) for ver in versions]
         for verstr, isver in isversions:
             setattr(self, 'IsVersionGreater' + verstr, isver)
     
     @property
```

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/XYAxes.py` & `witecsdk-1.2.5/WITecSDK/Modules/XYAxes.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/ZAxis.py` & `witecsdk-1.2.5/WITecSDK/Modules/ZAxis.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Modules/__init__.py` & `witecsdk-1.2.5/WITecSDK/Modules/__init__.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Parameters/COMEnumParameter.py` & `witecsdk-1.2.5/WITecSDK/Parameters/COMEnumParameter.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Parameters/COMFillStatusParameter.py` & `witecsdk-1.2.5/WITecSDK/Parameters/COMFillStatusParameter.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Parameters/COMFloatParameter.py` & `witecsdk-1.2.5/WITecSDK/Parameters/COMFloatParameter.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Parameters/COMIntParameter.py` & `witecsdk-1.2.5/WITecSDK/Parameters/COMIntParameter.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Parameters/COMParameter.py` & `witecsdk-1.2.5/WITecSDK/Parameters/COMParameter.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Parameters/COMParameterBase.py` & `witecsdk-1.2.5/WITecSDK/Parameters/COMParameterBase.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Parameters/COMStatusParameter.py` & `witecsdk-1.2.5/WITecSDK/Parameters/COMStatusParameter.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/Parameters/__init__.py` & `witecsdk-1.2.5/WITecSDK/Parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK/__init__.py` & `witecsdk-1.2.5/WITecSDK/__init__.py`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/WITecSDK.egg-info/PKG-INFO` & `witecsdk-1.2.5/WITecSDK.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: WITecSDK
-Version: 1.2.4
+Version: 1.2.5
 Summary: This package allows automation of WITec Control over COM
 Author-email: Matthias Finger <info@witec.de>
 License: MIT License
 Project-URL: Homepage, https://raman.oxinst.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: comtypes>=1.2.0
 
 This package enables control of WITec microscopes over its COM interface (additonal license required).
 
 - Gives access to data acquisition functions
 - Implements all classes of WITec's COM interface
@@ -43,14 +43,19 @@
 
 # Contribution and feature requests
 
 If you want to share your own extensions or have feature wishes please contact the [WITec support team](https://raman.oxinst.com/contact).
 
 # Changelog
 
+## Changes in 1.2.5
+
+- Bug in Autofocus fixed
+- Bug in WITecControlVersionTester fixed
+
 ## Changes in 1.2.4
 
 - Spectral Stitching added
 - WITecControlVersionTester reworked
 
 ## Changes in 1.2.3
```

### Comparing `WITecSDK-1.2.4/WITecSDK.egg-info/SOURCES.txt` & `witecsdk-1.2.5/WITecSDK.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `WITecSDK-1.2.4/pyproject.toml` & `witecsdk-1.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "WITecSDK"
-version = "1.2.4"
+version = "1.2.5"
 authors = [
   { name="Matthias Finger", email="info@witec.de" },
 ]
 description = "This package allows automation of WITec Control over COM"
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 license = {text = "MIT License"}
 dependencies = [
     "comtypes >= 1.2.0",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `WITecSDK-1.2.4/tests/TestAllModules.py` & `witecsdk-1.2.5/tests/TestAllModules.py`

 * *Files identical despite different names*

