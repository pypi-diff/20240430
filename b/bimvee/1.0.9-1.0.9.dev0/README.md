# Comparing `tmp/bimvee-1.0.9.tar.gz` & `tmp/bimvee-1.0.9.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\bimvee-1.0.9.tar", last modified: Fri Jul 31 13:13:28 2020, max compression
+gzip compressed data, was "dist/bimvee-1.0.9.dev0.tar", last modified: Thu Feb 24 09:22:21 2022, max compression
```

## Comparing `bimvee-1.0.9.tar` & `bimvee-1.0.9.dev0.tar`

### file list

```diff
@@ -1,61 +1,80 @@
-drwxrwxrwx   0        0        0        0 2020-07-31 13:13:28.000000 bimvee-1.0.9/
--rw-rw-rw-   0        0        0      903 2020-06-22 16:03:26.000000 bimvee-1.0.9/LICENSE.txt
--rw-rw-rw-   0        0        0    13202 2020-07-31 13:13:28.000000 bimvee-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0    10165 2020-07-31 13:10:17.000000 bimvee-1.0.9/README.md
-drwxrwxrwx   0        0        0        0 2020-07-31 13:13:28.000000 bimvee-1.0.9/bimvee/
--rw-rw-rw-   0        0        0        0 2020-06-11 13:24:38.000000 bimvee-1.0.9/bimvee/__init__.py
--rw-rw-rw-   0        0        0     2155 2020-07-24 11:51:11.000000 bimvee-1.0.9/bimvee/container.py
--rw-rw-rw-   0        0        0     2856 2020-07-13 09:32:20.000000 bimvee-1.0.9/bimvee/exportHdf5.py
--rw-rw-rw-   0        0        0    23484 2020-07-30 09:50:01.000000 bimvee-1.0.9/bimvee/exportIitYarp.py
--rw-rw-rw-   0        0        0     2207 2020-06-11 13:24:38.000000 bimvee-1.0.9/bimvee/exportPoseRpgEsimCsv.py
--rw-rw-rw-   0        0        0     9358 2020-07-31 13:11:33.000000 bimvee-1.0.9/bimvee/geometry.py
--rw-rw-rw-   0        0        0     5932 2020-07-10 11:27:38.000000 bimvee-1.0.9/bimvee/importAe.py
--rw-rw-rw-   0        0        0     3615 2020-06-23 09:23:30.000000 bimvee-1.0.9/bimvee/importAer2.py
--rw-rw-rw-   0        0        0     4758 2020-06-22 09:51:34.000000 bimvee-1.0.9/bimvee/importExportBatches.py
--rw-rw-rw-   0        0        0     3269 2020-07-24 12:45:40.000000 bimvee-1.0.9/bimvee/importFrames.py
--rw-rw-rw-   0        0        0     1376 2020-06-11 13:24:38.000000 bimvee-1.0.9/bimvee/importHdf5.py
--rw-rw-rw-   0        0        0     7147 2020-06-26 11:08:32.000000 bimvee-1.0.9/bimvee/importIitNumpy.py
--rw-rw-rw-   0        0        0     7802 2020-07-10 13:35:14.000000 bimvee-1.0.9/bimvee/importIitVicon.py
--rw-rw-rw-   0        0        0    23420 2020-07-30 09:50:01.000000 bimvee-1.0.9/bimvee/importIitYarp.py
-drwxrwxrwx   0        0        0        0 2020-07-31 13:13:28.000000 bimvee-1.0.9/bimvee/importRosbag/
-drwxrwxrwx   0        0        0        0 2020-07-31 13:13:28.000000 bimvee-1.0.9/bimvee/importRosbag/importRosbag/
--rw-rw-rw-   0        0        0        0 2020-06-11 13:49:20.000000 bimvee-1.0.9/bimvee/importRosbag/importRosbag/__init__.py
--rw-rw-rw-   0        0        0    11492 2020-06-11 13:49:20.000000 bimvee-1.0.9/bimvee/importRosbag/importRosbag/importRosbag.py
-drwxrwxrwx   0        0        0        0 2020-07-31 13:13:28.000000 bimvee-1.0.9/bimvee/importRosbag/importRosbag/messageTypes/
--rw-rw-rw-   0        0        0     2326 2020-06-11 13:49:20.000000 bimvee-1.0.9/bimvee/importRosbag/importRosbag/messageTypes/common.py
--rw-rw-rw-   0        0        0     3284 2020-06-11 13:49:20.000000 bimvee-1.0.9/bimvee/importRosbag/importRosbag/messageTypes/dvs_msgs_EventArray.py
--rw-rw-rw-   0        0        0     2614 2020-06-11 13:49:20.000000 bimvee-1.0.9/bimvee/importRosbag/importRosbag/messageTypes/esim_msgs_OpticFlow.py
--rw-rw-rw-   0        0        0     2856 2020-06-11 13:49:20.000000 bimvee-1.0.9/bimvee/importRosbag/importRosbag/messageTypes/geometry_msgs_PoseStamped.py
--rw-rw-rw-   0        0        0     2712 2020-06-11 13:49:20.000000 bimvee-1.0.9/bimvee/importRosbag/importRosbag/messageTypes/geometry_msgs_Transform.py
--rw-rw-rw-   0        0        0     2915 2020-06-11 13:49:20.000000 bimvee-1.0.9/bimvee/importRosbag/importRosbag/messageTypes/geometry_msgs_TransformStamped.py
--rw-rw-rw-   0        0        0     2446 2020-06-11 13:49:20.000000 bimvee-1.0.9/bimvee/importRosbag/importRosbag/messageTypes/geometry_msgs_TwistStamped.py
--rw-rw-rw-   0        0        0     2897 2020-06-11 13:49:20.000000 bimvee-1.0.9/bimvee/importRosbag/importRosbag/messageTypes/sensor_msgs_CameraInfo.py
--rw-rw-rw-   0        0        0     3828 2020-06-11 13:49:20.000000 bimvee-1.0.9/bimvee/importRosbag/importRosbag/messageTypes/sensor_msgs_Image.py
--rw-rw-rw-   0        0        0     3722 2020-06-11 13:49:20.000000 bimvee-1.0.9/bimvee/importRosbag/importRosbag/messageTypes/sensor_msgs_Imu.py
--rw-rw-rw-   0        0        0     4037 2020-06-11 13:49:20.000000 bimvee-1.0.9/bimvee/importRosbag/importRosbag/messageTypes/sensor_msgs_PointCloud2.py
--rw-rw-rw-   0        0        0     3434 2020-06-11 13:49:20.000000 bimvee-1.0.9/bimvee/importRosbag/importRosbag/messageTypes/tf_tfMessage.py
--rw-rw-rw-   0        0        0     6145 2020-06-11 13:51:20.000000 bimvee-1.0.9/bimvee/importRpgDvsRos.py
--rw-rw-rw-   0        0        0     7235 2020-06-11 13:24:38.000000 bimvee-1.0.9/bimvee/importSecDvs.py
--rw-rw-rw-   0        0        0     4586 2020-06-11 13:24:38.000000 bimvee-1.0.9/bimvee/info.py
--rw-rw-rw-   0        0        0     2629 2020-06-25 11:56:58.000000 bimvee-1.0.9/bimvee/plot.py
--rw-rw-rw-   0        0        0    14924 2020-06-11 13:24:38.000000 bimvee-1.0.9/bimvee/plotCorrelogram.py
--rw-rw-rw-   0        0        0    12713 2020-06-11 13:24:38.000000 bimvee-1.0.9/bimvee/plotDvsContrast.py
--rw-rw-rw-   0        0        0     7315 2020-07-31 11:42:10.000000 bimvee-1.0.9/bimvee/plotDvsLastTs.py
--rw-rw-rw-   0        0        0     4630 2020-06-11 13:24:38.000000 bimvee-1.0.9/bimvee/plotEventRate.py
--rw-rw-rw-   0        0        0     5177 2020-06-11 13:24:38.000000 bimvee-1.0.9/bimvee/plotFlow.py
--rw-rw-rw-   0        0        0     5201 2020-07-31 10:42:09.000000 bimvee-1.0.9/bimvee/plotFrame.py
--rw-rw-rw-   0        0        0     7059 2020-07-31 11:03:20.000000 bimvee-1.0.9/bimvee/plotImu.py
--rw-rw-rw-   0        0        0     6343 2020-07-24 18:30:42.000000 bimvee-1.0.9/bimvee/plotPose.py
--rw-rw-rw-   0        0        0     4712 2020-06-11 13:24:38.000000 bimvee-1.0.9/bimvee/plotSpikeogram.py
--rw-rw-rw-   0        0        0    22736 2020-07-21 14:17:58.000000 bimvee-1.0.9/bimvee/pose.py
--rw-rw-rw-   0        0        0    15961 2020-07-24 17:29:02.000000 bimvee-1.0.9/bimvee/split.py
--rw-rw-rw-   0        0        0    16087 2020-06-11 13:24:38.000000 bimvee-1.0.9/bimvee/timestamps.py
--rw-rw-rw-   0        0        0    29524 2020-07-31 13:11:33.000000 bimvee-1.0.9/bimvee/visualiser.py
-drwxrwxrwx   0        0        0        0 2020-07-31 13:13:28.000000 bimvee-1.0.9/bimvee.egg-info/
--rw-rw-rw-   0        0        0    13202 2020-07-31 13:13:27.000000 bimvee-1.0.9/bimvee.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1795 2020-07-31 13:13:28.000000 bimvee-1.0.9/bimvee.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-07-31 13:13:27.000000 bimvee-1.0.9/bimvee.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2020-07-31 13:13:27.000000 bimvee-1.0.9/bimvee.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2020-07-31 13:13:27.000000 bimvee-1.0.9/bimvee.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2020-07-31 13:13:28.000000 bimvee-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1792 2020-07-31 13:12:32.000000 bimvee-1.0.9/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2022-02-24 09:22:21.832320 bimvee-1.0.9.dev0/
+-rwxrwxrwx   0 root         (0) root         (0)      886 2021-09-17 08:00:54.000000 bimvee-1.0.9.dev0/LICENSE.txt
+-rwxrwxrwx   0 root         (0) root         (0)    11870 2022-02-24 09:22:21.832594 bimvee-1.0.9.dev0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)    10800 2021-11-04 13:06:46.000000 bimvee-1.0.9.dev0/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2022-02-24 09:22:21.822237 bimvee-1.0.9.dev0/bimvee/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2021-09-17 08:00:54.000000 bimvee-1.0.9.dev0/bimvee/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2481 2021-09-17 08:00:54.000000 bimvee-1.0.9.dev0/bimvee/container.py
+-rwxrwxrwx   0 root         (0) root         (0)     6177 2021-11-04 13:06:46.000000 bimvee-1.0.9.dev0/bimvee/events.py
+-rwxrwxrwx   0 root         (0) root         (0)     1527 2021-09-17 08:00:54.000000 bimvee-1.0.9.dev0/bimvee/exportHdf5.py
+-rwxrwxrwx   0 root         (0) root         (0)    24765 2021-11-12 10:57:35.000000 bimvee-1.0.9.dev0/bimvee/exportIitYarp.py
+-rwxrwxrwx   0 root         (0) root         (0)     2167 2021-09-17 08:00:54.000000 bimvee-1.0.9.dev0/bimvee/exportPoseRpgEsimCsv.py
+-rwxrwxrwx   0 root         (0) root         (0)     7922 2021-09-17 08:00:54.000000 bimvee-1.0.9.dev0/bimvee/exportRpgDvsRos.py
+-rwxrwxrwx   0 root         (0) root         (0)     9122 2021-09-17 08:00:54.000000 bimvee-1.0.9.dev0/bimvee/geometry.py
+-rwxrwxrwx   0 root         (0) root         (0)     7342 2021-11-12 10:57:35.000000 bimvee-1.0.9.dev0/bimvee/importAe.py
+-rwxrwxrwx   0 root         (0) root         (0)     3522 2021-09-17 08:00:54.000000 bimvee-1.0.9.dev0/bimvee/importAer2.py
+-rwxrwxrwx   0 root         (0) root         (0)      413 2021-11-04 13:06:46.000000 bimvee-1.0.9.dev0/bimvee/importBoundingBoxes.py
+-rwxrwxrwx   0 root         (0) root         (0)     4758 2021-09-17 08:00:54.000000 bimvee-1.0.9.dev0/bimvee/importExportBatches.py
+-rwxrwxrwx   0 root         (0) root         (0)     3205 2021-09-17 08:00:54.000000 bimvee-1.0.9.dev0/bimvee/importFrames.py
+-rwxrwxrwx   0 root         (0) root         (0)     1374 2021-09-17 08:00:54.000000 bimvee-1.0.9.dev0/bimvee/importHdf5.py
+-rwxrwxrwx   0 root         (0) root         (0)     6993 2021-09-17 08:00:54.000000 bimvee-1.0.9.dev0/bimvee/importIitNumpy.py
+-rwxrwxrwx   0 root         (0) root         (0)     7358 2021-09-17 08:00:54.000000 bimvee-1.0.9.dev0/bimvee/importIitVicon.py
+-rwxrwxrwx   0 root         (0) root         (0)    34617 2022-02-24 09:17:20.000000 bimvee-1.0.9.dev0/bimvee/importIitYarp.py
+-rwxrwxrwx   0 root         (0) root         (0)     9442 2021-11-04 13:06:46.000000 bimvee-1.0.9.dev0/bimvee/importProph.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2022-02-24 09:22:21.823888 bimvee-1.0.9.dev0/bimvee/importRosbag/
+drwxrwxrwx   0 root         (0) root         (0)        0 2022-02-24 09:22:21.824458 bimvee-1.0.9.dev0/bimvee/importRosbag/importRosbag/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2021-09-17 12:13:09.000000 bimvee-1.0.9.dev0/bimvee/importRosbag/importRosbag/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    11251 2021-09-17 12:13:09.000000 bimvee-1.0.9.dev0/bimvee/importRosbag/importRosbag/importRosbag.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2022-02-24 09:22:21.827992 bimvee-1.0.9.dev0/bimvee/importRosbag/importRosbag/messageTypes/
+-rwxrwxrwx   0 root         (0) root         (0)     2258 2021-09-17 12:13:09.000000 bimvee-1.0.9.dev0/bimvee/importRosbag/importRosbag/messageTypes/common.py
+-rwxrwxrwx   0 root         (0) root         (0)     3210 2021-09-17 12:13:09.000000 bimvee-1.0.9.dev0/bimvee/importRosbag/importRosbag/messageTypes/dvs_msgs_EventArray.py
+-rwxrwxrwx   0 root         (0) root         (0)     2545 2021-09-17 12:13:09.000000 bimvee-1.0.9.dev0/bimvee/importRosbag/importRosbag/messageTypes/esim_msgs_OpticFlow.py
+-rwxrwxrwx   0 root         (0) root         (0)     2791 2021-09-17 12:13:09.000000 bimvee-1.0.9.dev0/bimvee/importRosbag/importRosbag/messageTypes/geometry_msgs_PoseStamped.py
+-rwxrwxrwx   0 root         (0) root         (0)     2649 2021-09-17 12:13:09.000000 bimvee-1.0.9.dev0/bimvee/importRosbag/importRosbag/messageTypes/geometry_msgs_Transform.py
+-rwxrwxrwx   0 root         (0) root         (0)     2848 2021-09-17 12:13:09.000000 bimvee-1.0.9.dev0/bimvee/importRosbag/importRosbag/messageTypes/geometry_msgs_TransformStamped.py
+-rwxrwxrwx   0 root         (0) root         (0)     2387 2021-09-17 12:13:09.000000 bimvee-1.0.9.dev0/bimvee/importRosbag/importRosbag/messageTypes/geometry_msgs_TwistStamped.py
+-rwxrwxrwx   0 root         (0) root         (0)     2830 2021-09-17 12:13:09.000000 bimvee-1.0.9.dev0/bimvee/importRosbag/importRosbag/messageTypes/sensor_msgs_CameraInfo.py
+-rwxrwxrwx   0 root         (0) root         (0)     4173 2021-09-17 12:13:09.000000 bimvee-1.0.9.dev0/bimvee/importRosbag/importRosbag/messageTypes/sensor_msgs_Image.py
+-rwxrwxrwx   0 root         (0) root         (0)     3637 2021-09-17 12:13:09.000000 bimvee-1.0.9.dev0/bimvee/importRosbag/importRosbag/messageTypes/sensor_msgs_Imu.py
+-rwxrwxrwx   0 root         (0) root         (0)     3944 2021-09-17 12:13:09.000000 bimvee-1.0.9.dev0/bimvee/importRosbag/importRosbag/messageTypes/sensor_msgs_PointCloud2.py
+-rwxrwxrwx   0 root         (0) root         (0)     3354 2021-09-17 12:13:09.000000 bimvee-1.0.9.dev0/bimvee/importRosbag/importRosbag/messageTypes/tf_tfMessage.py
+-rwxrwxrwx   0 root         (0) root         (0)     1486 2021-09-17 12:13:09.000000 bimvee-1.0.9.dev0/bimvee/importRosbag/setup.py
+-rwxrwxrwx   0 root         (0) root         (0)     6058 2021-09-17 08:00:54.000000 bimvee-1.0.9.dev0/bimvee/importRpgDvsRos.py
+-rwxrwxrwx   0 root         (0) root         (0)     7451 2021-09-17 08:00:54.000000 bimvee-1.0.9.dev0/bimvee/importSecDvs.py
+-rwxrwxrwx   0 root         (0) root         (0)      920 2021-12-26 14:04:19.000000 bimvee-1.0.9.dev0/bimvee/importSkeleton.py
+-rwxrwxrwx   0 root         (0) root         (0)     7763 2021-09-17 08:00:54.000000 bimvee-1.0.9.dev0/bimvee/importUdsAedat.py
+-rwxrwxrwx   0 root         (0) root         (0)     4658 2021-09-17 08:00:54.000000 bimvee-1.0.9.dev0/bimvee/info.py
+-rwxrwxrwx   0 root         (0) root         (0)     2684 2021-09-17 08:00:54.000000 bimvee-1.0.9.dev0/bimvee/plot.py
+-rwxrwxrwx   0 root         (0) root         (0)    14586 2021-09-17 08:00:54.000000 bimvee-1.0.9.dev0/bimvee/plotCorrelogram.py
+-rwxrwxrwx   0 root         (0) root         (0)    14953 2021-12-26 14:04:19.000000 bimvee-1.0.9.dev0/bimvee/plotDvsContrast.py
+-rwxrwxrwx   0 root         (0) root         (0)     7139 2021-09-17 08:00:54.000000 bimvee-1.0.9.dev0/bimvee/plotDvsLastTs.py
+-rwxrwxrwx   0 root         (0) root         (0)     2562 2021-09-17 08:00:54.000000 bimvee-1.0.9.dev0/bimvee/plotDvsSpaceTime.py
+-rwxrwxrwx   0 root         (0) root         (0)     4522 2021-09-17 08:00:54.000000 bimvee-1.0.9.dev0/bimvee/plotEventRate.py
+-rwxrwxrwx   0 root         (0) root         (0)     5057 2021-09-17 08:00:54.000000 bimvee-1.0.9.dev0/bimvee/plotFlow.py
+-rwxrwxrwx   0 root         (0) root         (0)     5073 2021-09-17 08:00:54.000000 bimvee-1.0.9.dev0/bimvee/plotFrame.py
+-rwxrwxrwx   0 root         (0) root         (0)     7026 2021-09-17 08:00:54.000000 bimvee-1.0.9.dev0/bimvee/plotImu.py
+-rwxrwxrwx   0 root         (0) root         (0)     9660 2021-09-17 08:00:54.000000 bimvee-1.0.9.dev0/bimvee/plotPose.py
+-rwxrwxrwx   0 root         (0) root         (0)    10353 2021-09-17 08:00:54.000000 bimvee-1.0.9.dev0/bimvee/plotSpikeogram.py
+-rwxrwxrwx   0 root         (0) root         (0)    31252 2021-09-17 08:00:54.000000 bimvee-1.0.9.dev0/bimvee/pose.py
+-rwxrwxrwx   0 root         (0) root         (0)    19157 2021-11-04 13:06:46.000000 bimvee-1.0.9.dev0/bimvee/split.py
+-rwxrwxrwx   0 root         (0) root         (0)    20499 2021-09-17 08:00:54.000000 bimvee-1.0.9.dev0/bimvee/timestamps.py
+-rwxrwxrwx   0 root         (0) root         (0)     2690 2021-11-12 10:57:35.000000 bimvee-1.0.9.dev0/bimvee/visualiser.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2022-02-24 09:22:21.831920 bimvee-1.0.9.dev0/bimvee/visualisers/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2021-11-04 13:06:46.000000 bimvee-1.0.9.dev0/bimvee/visualisers/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2572 2021-10-07 09:32:16.000000 bimvee-1.0.9.dev0/bimvee/visualisers/visualiserBase.py
+-rwxrwxrwx   0 root         (0) root         (0)     5428 2021-11-04 13:06:46.000000 bimvee-1.0.9.dev0/bimvee/visualisers/visualiserBoundingBoxes.py
+-rwxrwxrwx   0 root         (0) root         (0)     4512 2021-12-26 14:04:19.000000 bimvee-1.0.9.dev0/bimvee/visualisers/visualiserDvs.py
+-rwxrwxrwx   0 root         (0) root         (0)     5166 2021-09-17 08:00:54.000000 bimvee-1.0.9.dev0/bimvee/visualisers/visualiserFrame.py
+-rwxrwxrwx   0 root         (0) root         (0)    11137 2021-11-04 13:06:46.000000 bimvee-1.0.9.dev0/bimvee/visualisers/visualiserImu.py
+-rwxrwxrwx   0 root         (0) root         (0)     7787 2021-09-17 08:00:54.000000 bimvee-1.0.9.dev0/bimvee/visualisers/visualiserOpticFlow.py
+-rwxrwxrwx   0 root         (0) root         (0)     7824 2021-11-04 13:06:46.000000 bimvee-1.0.9.dev0/bimvee/visualisers/visualiserPoint3.py
+-rwxrwxrwx   0 root         (0) root         (0)    12803 2021-11-04 13:06:46.000000 bimvee-1.0.9.dev0/bimvee/visualisers/visualiserPose6q.py
+-rwxrwxrwx   0 root         (0) root         (0)     4552 2021-11-12 10:57:35.000000 bimvee-1.0.9.dev0/bimvee/visualisers/visualiserSkeleton.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2022-02-24 09:22:21.823609 bimvee-1.0.9.dev0/bimvee.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)    11870 2022-02-24 09:22:21.000000 bimvee-1.0.9.dev0/bimvee.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2381 2022-02-24 09:22:21.000000 bimvee-1.0.9.dev0/bimvee.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2022-02-24 09:22:21.000000 bimvee-1.0.9.dev0/bimvee.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       70 2022-02-24 09:22:21.000000 bimvee-1.0.9.dev0/bimvee.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        7 2022-02-24 09:22:21.000000 bimvee-1.0.9.dev0/bimvee.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)      107 2022-02-24 09:22:21.833082 bimvee-1.0.9.dev0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1825 2022-02-24 09:22:20.000000 bimvee-1.0.9.dev0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bimvee-1.0.9/LICENSE.txt` & `bimvee-1.0.9.dev0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-Copyright (C) 2019- Event-driven Perception for Robotics
-Authors: Sim Bamford
-		 Suman Ghosh
-		 Aiko Dinale
-		 Massimiliano Iacono
-Additional code contributions from:
-        Vadim Tikhanoff
-		Marco Monforte
-		Contains several third-party contributions esp. geometry.py 
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
+Copyright (C) 2019- Event-driven Perception for Robotics
+Authors: Sim Bamford
+		 Suman Ghosh
+		 Aiko Dinale
+		 Massimiliano Iacono
+Additional code contributions from:
+        Vadim Tikhanoff
+		Marco Monforte
+		Contains several third-party contributions esp. geometry.py 
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
```

### Comparing `bimvee-1.0.9/README.md` & `bimvee-1.0.9.dev0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,246 +1,272 @@
-# bimvee - Batch Import, Manipulation, Visualisation, and Export Events etc.
-
-<img src="https://raw.githubusercontent.com/event-driven-robotics/bimvee/master/images/events.png" width="300"/> <img src="https://raw.githubusercontent.com/event-driven-robotics/bimvee/master/images/frames.png" width="300"/>
-<img src="https://raw.githubusercontent.com/event-driven-robotics/bimvee/master/images/imu.png" width="300"/>
-<img src="https://raw.githubusercontent.com/event-driven-robotics/bimvee/master/images/pose.png" width="300"/>
-<img src="https://raw.githubusercontent.com/event-driven-robotics/bimvee/master/images/dvslastts.png" width="300"/>
-<img src="https://raw.githubusercontent.com/event-driven-robotics/bimvee/master/images/eventrate.png" width="300"/>
-
-# Quickstart 
-
-Look at 'examples/examples.py' for examples of how to use the functionality in this library.
-
-Important! When you clone this repo, use --recurse-submodules option, as this repo uses 'importRosbag' library as a submodule. 
-
-Want to play back your timestamped multi-channel data? Consider using https://github.com/event-driven-robotics/mustard
-
-# Introduction
-
-Working with timestamped address-event data from event cameras (dvs), and 
-possibly other neuromorphic sensors alongside other timestamped data 
-that we need for our experiments, including but not limited to:
-- frame-based camera images
-- IMU
-- 6-DOF poses
-- derived datatypes, such as optical (flow) events, or labelled dvs events (dvsL) etc 
-- Camera calibration info is also imported from e.g. ros (cam)
-
-File formats supported include:
-- IIT YARP .log - ATIS Gen1 and IMU
-- rpg_dvs_ros - DVS/DAVIS .bag 
-- Third-party datasets recorded by using the above rosbag importer (e.g. Penn MvSEC, UMD EvIMO, Intel Realsense etc)
-- Vicon - as dumped by yarpDumper
-- Samsung (SEC) Gen3 VGA .bin
-- Pull requests welcome for importers or exporters of other file formats.
-
-# Contents of library
-
-## Import functions:
-
-The aim is to bring the different formats into as common a format as possible.
-Parameters: at least the param "filePathOrName" (otherwise working from current directory)
-Returns a dict containing:
-
-    {'info': {<filePathOrName, any other info derivable from file headers>},
-    
-    'data': {
-     
-         channel0: {}
-         channel1: {}
-         ...
-         }}
-
-The 'data' branch contains a dict for each channel. A 'channel' is an arbitrary 
-grouping of datasets. It might be that there is one channel for each sensor, 
-so for example a file might contain 'left' and 'right' 
-camera channels, and each of these channels might contain dvs events alongside 
-other data types like frames. 
-Each channel is a dict containing one dict for each type of data.
-Data types may include:
-- dvs (Timestamped (ts) 2D address-events (x, y) with polarity (pol), from an event camera)
-- frame
-- imu
-- flow 
-- pose
-- etc
-
-dvs data type, for example, then contains:
-
-- "pol": numpy array of bool
-- "x": numpy array of np.uint16
-- "y": numpy array of np.uint16
-- "ts": numpy array of np.float64 
-
-timestamps are always converted to seconds; 
-(raw formats are, however, e.g. int with unit increments of 80 ns for ATIS, 
-int with unit increments of 1 us for DAVIS, etc) 
-
-To the extent possible, dvs polarity is imported so that 1/True = ON/increase-in-light and
-0/False = OFF/decrease-in-light. Be aware that individual datasets may contain the opposite convention. 
-
-Multiple files imported simultaneously appear in a list of dicts;
-lists and dicts are referred to jointly as containers, 
-and the manipulation, visualistation and export functions which follow 
-tend toward accepting containers with an arbitrarily deep hierarchy.
-
-## Visualisation functions
-
-There is a set of general functions for common visualisations of imported datasets, using matplotlib or seaborn.
-
-- plotDvsContrast
-- plotDvsLastTs
-- plotSpikeogram
-- plotEventRate
-- plotFrame
-- plotImu
-- plotPose
-- plotCorrelogram
-- plotFlow
-
-These functions have several kwargs to modify their behaviour, and they support a 'callback' kwarg so you can pass in a function to do post-modification of the plots. 
-
-There are two different visualisation concepts. In the 'continuous' concept, a single plot shows all timestamped data for a given container. This might be limited to a certain time range, as defined by kwargs minTime and maxTime. Examples include:
-- plotEventRate 
-- plotImu
-- plotPose
-- plotSpikeogram
-
-In the 'snapshot' concept, a representation is generated for a chosen moment in time. In the case of frames this might be the nearest frame to the chosen time. In the case of dvs events this might be an image composed of events recruited from around that moment in time, for which there is a concept of the time window. In the case of poses this might be a projected view of the pose at the given time, where the pose might be linearly interpolated between the two nearest timestamped poses. Examples include:
-- plotDvsContrastSingle
-- plotDvsLastTs (in this case, the visualisation is based on all data up to the chosen time)
-
-In the case of the snapshot views, there are general functions which when passed a data container will choose a set of times distributed throughout the time range of that data and generate a snapshot view for each of these moments. Examples include:
-- plotDvsContrast
-- plotFrame
-
-'visualiser.py' defines a set of classes, one for each of a selection of data types, which generate snapshot views. These are output as numpy arrays, to be rendered by an external application. 
-
-info.py includes various functions to give quick text info about the contents of the containers that result from imports.
-
-## Manipulation functions
-
-There are some functions for standard manipulations of data:
-
-timestamps.py contains timestamp manipulations 
-including jointly zeroing timestamps across multiple files, channels and datatypes. 
-split.py includes various common ways by which datasets need to be split, e.g. splitByPolarity
-
-## Export functions
-
-exportIitYarp - exports to IIT's EDPR YARP format. Alongside data.log and 
-info.log files, it exports an xml which specifies to yarpmanager how to 
-visualise the resulting data. 
-
-# Dependencies:
-
-This library uses importRosbag library to import rosbag data without needing a ros installation.
-This is included as a submodule. 
-
-Beyond the python standard library, the main dependencies are:
-
-- numpy
-- tqdm (for progress bars during import and export functions)
-
-For the 'plot' family of visualisation functions:
-
-- matplotlib
-- mpl_toolkits (only for certain 3d visualisations)
-- seaborn
-
-The "visualiser", however, generates graphics as numpy arrays 
-without reference to matplotlib, for rendering by an external application.
-
-plotDvsLastTs uses rankdata from scipy; however if it's not installed, 
-it defaults to a local definition; scipy is therefore an optional dependency.
-
-import/export Hdf5 functions use:
-
-- hickle
-
-# Type definitions
-
-bimvee doesn't use classes for datatypes. Consequently, the code doesn't have a central place to refer to for the definition of datatypes. The types are intended to be used loosely, with minimal features which can be extended by adding optional fields. There is an optional container class which gives some functions for easier data manipulation.
-
-There are some datatypes which are simply dicts which act as containers to group information, for example the 'cam' type. However most of the functionality of the library is based around the idea of a datatype dict containing a set of keys where each is a numpy array (or other iterable) where there is a 'ts' key, containing a numpy array of np.float64 timestamps, and then each iterable key should have the same number of elements (in the zeroth dimension) as the ts field. Thus a set of timestamped 'events' or other data type is defined. Other keys may be included which either aren't iterables or don't have the same number of elements in the zeroth dimension. These are therefore not interpreted as contributing dimensions to the set of data points. Concretely the datatypes which have some kind of support are:
-
-- dvs
-- frame
-- sample
-- imu
-- pose6q
-- point3
-- flow
-
-- cam
-
-Definitions of minimal and optional(*) fields follow.
-
-- fieldName   dimensions  datatype(numpy array unless otherwise stated) notes
-
-## dvs:
-
-- ts  n np.float64
-- x   n np.uint16
-- y   n np.uint16 As the sensor outputs it; plot functions assume that y increases in downward direction, following https://arxiv.org/pdf/1610.08336.pdf
-- pol n np.bool To the extent possible, True means increase in light, False means decrease. 
-- dimX* 1 int
-- dimY* 1 int
-
-## frame:
-
-- ts    n np.float64
-- frame n list (of np.array of 2 or 3 dimensions np.uint8)
-
-## sample:
-
-- ts     n np.float64
-- sensor n np.uint8
-- value  n np.int16
-
-## imu:
-
-- ts  n    np.float64
-- acc  nx3 np.float64 accelerometer readings [x,y,z] in m/s
-- angV nx3 np.float64 angV readings [yaw, pitch roll?] in rad/s
-- mag  nx3 np.float64 magnetometer readings [x, y, z] in tesla
-- temp n   np.float64
-
-## point3:
-
-- ts    n   np.float64
-- point nx3 np.float64 row format is [x, y, z]
-
-
-## pose6q (effectively extends point3):
-
-- ts       n   np.float64
-- point    nx3 np.float64 row format is [x, y, z]
-- rotation nx4 np.float64 row format is [rw, rx, ry, rz] where r(wxyz) define a quaternion
-
-Note: quaternion order follows the convention of e.g. blender (wxyz) but not e.g. ros. (xyzw)
-
-## flow: (per-pixel flow events)
-
-- ts  n np.float64
-- x   n np.uint16
-- y   n np.uint16  
-- vx   n np.uint16
-- vy   n np.uint16  
-
-## cam:
-
-Following ros msg camera info, the fields this might contain include:
-
-- height           1   int
-- width            1   int
-- distortion_model     string 
-- D                5   np.float64 distortion params
-- K                3x3 np.float64 Intrinsic camera matrix
-- R                3x4 np.float64 Rectification matrix
-- P                4x4 np.float64 projection matrix
-
-
-
-
-
-
+# bimvee - Batch Import, Manipulation, Visualisation, and Export of Events etc.
+
+<img src="https://raw.githubusercontent.com/event-driven-robotics/bimvee/master/images/events.png" width="300"/> <img src="https://raw.githubusercontent.com/event-driven-robotics/bimvee/master/images/frames.png" width="300"/>
+<img src="https://raw.githubusercontent.com/event-driven-robotics/bimvee/master/images/imu.png" width="300"/>
+<img src="https://raw.githubusercontent.com/event-driven-robotics/bimvee/master/images/pose.png" width="300"/>
+<img src="https://raw.githubusercontent.com/event-driven-robotics/bimvee/master/images/dvslastts.png" width="300"/>
+<img src="https://raw.githubusercontent.com/event-driven-robotics/bimvee/master/images/eventrate.png" width="300"/>
+
+# Quickstart
+
+## Installation
+
+There is a pip installer:
+
+    pip install bimvee
+
+Important! If you clone this repo, use --recurse-submodules option, as this repo uses 'importRosbag' library as a submodule.
+
+## Usage
+
+Look at [examples.py](https://github.com/event-driven-robotics/bimvee/blob/master/examples/examples.py) for examples of how to use the functionality in this library.
+
+Want to play back your timestamped multi-channel data? Consider using https://github.com/event-driven-robotics/mustard
+
+# Introduction
+
+Working with timestamped address-event data from event cameras (dvs), and
+possibly other neuromorphic sensors alongside other timestamped data
+that we need for our experiments, including but not limited to:
+- frame-based camera images
+- IMU
+- 6-DOF poses
+- derived datatypes, such as optical (flow) events, or labelled dvs events (dvsL) etc
+- Camera calibration info is also imported from e.g. ros (cam)
+
+File formats supported include:
+- IIT YARP .log - ATIS Gen1 and IMU
+- rpg_dvs_ros - DVS/DAVIS .bag
+- Third-party datasets recorded by using the above rosbag importer (e.g. Penn MvSEC, UMD EvIMO, Intel Realsense etc)
+- Vicon - as dumped by yarpDumper
+- Samsung (SEC) Gen3 VGA .bin
+- Pull requests welcome for importers or exporters of other file formats.
+
+# Contents of library
+
+## Import functions:
+
+The aim is to bring the different formats into as common a format as possible.
+Parameters: at least the param "filePathOrName" (otherwise working from current directory)
+Returns a dict containing:
+
+    {'info': {<filePathOrName, any other info derivable from file headers>},
+
+    'data': {
+
+         channel0: {}
+         channel1: {}
+         ...
+         }}
+
+The 'data' branch contains a dict for each channel. A 'channel' is an arbitrary
+grouping of datasets. It might be that there is one channel for each sensor,
+so for example a file might contain 'left' and 'right'
+camera channels, and each of these channels might contain dvs events alongside
+other data types like frames.
+Each channel is a dict containing one dict for each type of data.
+Data types may include:
+- dvs (Timestamped (ts) 2D address-events (x, y) with polarity (pol), from an event camera)
+- frame
+- imu
+- flow
+- pose
+- etc
+
+dvs data type, for example, then contains:
+
+- "pol": numpy array of bool
+- "x": numpy array of np.uint16
+- "y": numpy array of np.uint16
+- "ts": numpy array of np.float64
+
+timestamps are always converted to seconds;
+(raw formats are, however, e.g. int with unit increments of 80 ns for ATIS,
+int with unit increments of 1 us for DAVIS, etc)
+
+To the extent possible, dvs polarity is imported so that 1/True = ON/increase-in-light and
+0/False = OFF/decrease-in-light. Be aware that individual datasets may contain the opposite convention.
+
+Multiple files imported simultaneously appear in a list of dicts;
+lists and dicts are referred to jointly as containers,
+and the manipulation, visualistation and export functions which follow
+tend toward accepting containers with an arbitrarily deep hierarchy.
+
+## Visualisation functions
+
+There is a set of general functions for common visualisations of imported datasets, using matplotlib or seaborn.
+
+- plotDvsContrast
+- plotDvsLastTs
+- plotSpikeogram
+- plotEventRate
+- plotFrame
+- plotImu
+- plotPose
+- plotCorrelogram
+- plotFlow
+
+These functions have several kwargs to modify their behaviour, and they support a 'callback' kwarg so you can pass in a function to do post-modification of the plots.
+
+There are two different visualisation concepts. In the 'continuous' concept, a single plot shows all timestamped data for a given container. This might be limited to a certain time range, as defined by kwargs minTime and maxTime. Examples include:
+- plotEventRate
+- plotImu
+- plotPose
+- plotSpikeogram
+
+In the 'snapshot' concept, a representation is generated for a chosen moment in time. In the case of frames this might be the nearest frame to the chosen time. In the case of dvs events this might be an image composed of events recruited from around that moment in time, for which there is a concept of the time window. In the case of poses this might be a projected view of the pose at the given time, where the pose might be linearly interpolated between the two nearest timestamped poses. Examples include:
+- plotDvsContrastSingle
+- plotDvsLastTs (in this case, the visualisation is based on all data up to the chosen time)
+
+In the case of the snapshot views, there are general functions which when passed a data container will choose a set of times distributed throughout the time range of that data and generate a snapshot view for each of these moments. Examples include:
+- plotDvsContrast
+- plotFrame
+
+'visualiser.py' defines a set of classes, one for each of a selection of data types, which generate snapshot views. These are output as numpy arrays, to be rendered by an external application.
+
+info.py includes various functions to give quick text info about the contents of the containers that result from imports.
+
+## Manipulation functions
+
+There are some functions for standard manipulations of data:
+
+timestamps.py contains timestamp manipulations
+including jointly zeroing timestamps across multiple files, channels and datatypes.
+split.py includes various common ways by which datasets need to be split, e.g. splitByPolarity
+
+## Export functions
+
+exportIitYarp - exports to IIT's EDPR YARP format. Alongside data.log and
+info.log files, it exports an xml which specifies to yarpmanager how to
+visualise the resulting data.
+
+# Dependencies:
+
+This library uses importRosbag library to import rosbag data without needing a ros installation.
+This is included as a submodule.
+
+Beyond the python standard library, the main dependencies are:
+
+- numpy
+- tqdm (for progress bars during import and export functions)
+
+For the 'plot' family of visualisation functions:
+
+- matplotlib
+- mpl_toolkits (only for certain 3d visualisations)
+- seaborn
+
+The "visualiser", however, generates graphics as numpy arrays
+without reference to matplotlib, for rendering by an external application.
+
+plotDvsLastTs uses rankdata from scipy; however if it's not installed,
+it defaults to a local definition; scipy is therefore an optional dependency.
+
+undistortEvents function in events.py uses cv2 (openCv).
+
+import/export Hdf5 functions use:
+
+- hickle
+
+# Type definitions
+
+bimvee doesn't use classes for datatypes. Consequently, the code doesn't have a central place to refer to for the definition of datatypes. The types are intended to be used loosely, with minimal features which can be extended by adding optional fields. There is an optional container class which gives some functions for easier data manipulation.
+
+There are some datatypes which are simply dicts which act as containers to group information, for example the 'cam' type. However most of the functionality of the library is based around the idea of a datatype dict containing a set of keys where each is a numpy array (or other iterable) where there is a 'ts' key, containing a numpy array of np.float64 timestamps, and then each iterable key should have the same number of elements (in the zeroth dimension) as the ts field. Thus a set of timestamped 'events' or other data type is defined. Other keys may be included which either aren't iterables or don't have the same number of elements in the zeroth dimension. These are therefore not interpreted as contributing dimensions to the set of data points. Concretely the datatypes which have some kind of support are:
+
+- dvs
+- frame
+- sample
+- imu
+- pose6q
+- point3
+- flow
+- skinSamples
+- skinEvents
+- ear
+- cam
+
+Definitions of minimal and optional(*) fields follow.
+
+- fieldName   dimensions  datatype(numpy array unless otherwise stated) notes
+
+## dvs:
+
+- ts  n np.float64
+- x   n np.uint16
+- y   n np.uint16 As the sensor outputs it; plot functions assume that y increases in downward direction, following https://arxiv.org/pdf/1610.08336.pdf
+- pol n np.bool To the extent possible, True means increase in light, False means decrease.
+- dimX* 1 int
+- dimY* 1 int
+
+## frame:
+
+- ts    n np.float64
+- frame n list (of np.array of 2 or 3 dimensions np.uint8)
+
+## sample:
+
+- ts     n np.float64
+- sensor n np.uint8
+- value  n np.int16
+
+## imu:
+
+- ts  n    np.float64
+- acc  nx3 np.float64 accelerometer readings [x,y,z] in m/s
+- angV nx3 np.float64 angV readings [yaw, pitch roll?] in rad/s
+- mag  nx3 np.float64 magnetometer readings [x, y, z] in tesla
+- temp n   np.float64
+
+## point3:
+
+- ts    n   np.float64
+- point nx3 np.float64 row format is [x, y, z]
+
+
+## pose6q (effectively extends point3):
+
+- ts       n   np.float64
+- point    nx3 np.float64 row format is [x, y, z]
+- rotation nx4 np.float64 row format is [rw, rx, ry, rz] where r(wxyz) define a quaternion
+
+Note: quaternion order follows the convention of e.g. blender (wxyz) but not e.g. ros. (xyzw)
+
+## flow: (per-pixel flow events)
+
+- ts  n np.float64
+- x   n np.uint16
+- y   n np.uint16  
+- vx   n np.uint16
+- vy   n np.uint16  
+
+## skinEvents: (intended for iCub neuromorphic skin events; could be generalised)
+
+- ts n np.float64
+- taxel n np.unit16
+- bodyPart n np.uint8
+- pol n np.bool
+
+## skinSamples: (intended for dense iCub skin samples; could be generalised)
+
+- ts n np.float64
+- pressure nxm np.float64; m is the number of taxels concurrently sampled. Note:
+there exist in the wild examples where the pressure value is a raw 8-bit sample.
+
+## ear: (intended for cochlea events from UDS / Gutierrez-Galan, could be generalised)
+
+- ts n np.float64
+- freq n np.uint8
+- pol n np.bool
+- (There follow a number of model-specific fields which contribute to the full address: xsoType, auditoryModel, itdNeuronIds)
+
+## cam:
+
+Following ros msg camera info, the fields this might contain include:
+
+- height           1   int
+- width            1   int
+- distortion_model     string
+- D                5   np.float64 distortion params
+- K                3x3 np.float64 Intrinsic camera matrix
+- R                3x4 np.float64 Rectification matrix
+- P                4x4 np.float64 projection matrix
```

### Comparing `bimvee-1.0.9/bimvee/exportIitYarp.py` & `bimvee-1.0.9.dev0/bimvee/exportIitYarp.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,461 +1,511 @@
-# -*- coding: utf-8 -*-
-"""
-Copyright (C) 2019 Event-driven Perception for Robotics
-Authors: Sim Bamford
-Code contributions from:
-        Vadim Tikhanoff
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
-exportIitYarp takes a data dict resulting from importAe.
-Exports data.log and info.log for each channel contained.
-Uses the "exportFilePath" parameter for the top-level folder,
-creating it if it doesn't exist. This can be relative or absolute.
-Defaults to the current directory.
-Uses the "yarpOutputPort" parameter for the port defined in info.log.
-Default is "/file" - then the following is appended: "/AE:o"
-Where more than one channel is contained, the channel name is used in place of "AE".
-If the "viewerApp" parameter is True (default = True), then a play.xml 
-file is created at the top level directory, which is configured so that when
-run from yarpmanager, the data which has been exported can be viewed.
-"writeProtected" (default=True) protects any existing data in the target exportFilePath from being overwritten.
-"writeMode" (default='w') can be set to append mode ('a') for exporting (large) files in batches.
-"""
-
-#%%
-
-import os
-import numpy as np
-from tqdm import tqdm
-import string
-
-# TODO: this could come from header info in some cases
-def getDims(dataTypeDict):
-    if 'pol' in dataTypeDict: # dvs
-        minX = np.min(dataTypeDict['x'])
-        maxX = np.max(dataTypeDict['x'])
-        minY = np.min(dataTypeDict['y'])
-        maxY = np.max(dataTypeDict['y'])
-    elif 'frames' in dataTypeDict:
-        minX = 0
-        maxX = (dataTypeDict['frames'][0].shape)[0]
-        minY = 0
-        maxY = (dataTypeDict['frames'][0].shape)[1]
-    return minX, maxX, minY, maxY
-    
-def writeModule(xmlFile, name, **kwargs):
-    xmlFile.write('<module>\n')
-    xmlFile.write('    <name> ' + name + ' </name>\n')
-    parameters = kwargs.get('parameters', '')
-    xmlFile.write('    <parameters> ' + parameters + ' </parameters>\n')
-    dependencies = kwargs.get('dependencies', '')
-    if dependencies != '':
-        xmlFile.write('    <dependencies>\n')
-        xmlFile.write('        ' + dependencies + '\n')
-        xmlFile.write('    </dependencies>\n')
-    xmlFile.write('    <node> localhost </node>\n')
-    xmlFile.write('</module>\n')
-    xmlFile.write('\n')
-
-def writeConnection(xmlFile, fromPort, toPort, **kwargs):
-    xmlFile.write('<connection>\n')
-    xmlFile.write('    <from> ' + fromPort + ' </from>\n')
-    xmlFile.write('    <to> ' + toPort + ' </to>\n')
-    protocol = kwargs.get('protocol', 'udp')
-    xmlFile.write('<protocol> ' + protocol + ' </protocol>\n')
-    xmlFile.write('</connection>\n')
-    xmlFile.write('\n')
-
-def exportIitYarpViewer(importedDict, **kwargs):
-    exportFilePath = kwargs.get('exportFilePath', './')
-    with open(os.path.join(exportFilePath, 'play.xml'), 'w') as xmlFile:
-        xmlFile.write('<application>\n')
-        xmlFile.write('<name>play </name>\n')
-        xmlFile.write('\n')
-        writeModule(xmlFile=xmlFile, name='yarpdataplayer')
-        pathForPlayback = kwargs.get('pathForPlayback', exportFilePath)
-        #dependencyStr = ''
-        dependencyStr = '<port timeout="100.0" request="load ' + pathForPlayback + '" reply="[ok]">/yarpdataplayer/rpc:i</port>'
-        dataTypesToExport = kwargs.get('dataTypes')
-        for channelKey in importedDict['data']:
-            for dataType in importedDict['data'][channelKey]:
-                if dataTypesToExport is not None and dataType not in dataTypesToExport: continue
-                channelKeyStripped = str(channelKey).translate(str.maketrans('', '', string.punctuation))
-                channelAndDataType = channelKeyStripped + dataType
-
-                if dataType == 'dvs':
-                    minX, maxX, minY, maxY = getDims(importedDict['data'][channelKey][dataType])
-                    height = maxY + 1
-                    width = maxX + 1
-                    paramsFramer = '--name /framer' + channelAndDataType + \
-                                                   ' --height ' + str(height) + \
-                                                   ' --width ' + str(width) + \
-                                                   ' --displays "(/' + channelAndDataType + ' (AE ISO))"'
-                    writeModule(xmlFile=xmlFile, name='vFramerLite', parameters=paramsFramer, dependencies=dependencyStr)
-                    dependencyStr = ''                    
-                    paramsViewer = '--name /viewer/' + channelAndDataType + \
-                                    ' --w ' + str((width) * 2) + \
-                                    ' --h ' + str((height) * 2) + ' --synch'
-                    writeModule(xmlFile=xmlFile, name='yarpview', parameters=paramsViewer)
-                    
-                    fromPort = '/file/' + channelAndDataType + ':o'
-                    toPort = '/framer' + channelAndDataType + '/' + channelAndDataType + '/AE:i'
-                    writeConnection(xmlFile=xmlFile, fromPort=fromPort, toPort=toPort)
-                    
-                    fromPort = '/framer' + channelAndDataType + '/' + channelAndDataType + '/image:o'
-                    toPort = '/viewer/' + channelAndDataType 
-                    writeConnection(xmlFile=xmlFile, fromPort=fromPort, toPort=toPort)
-                    
-                if dataType == 'frame':
-                    minX, maxX, minY, maxY = getDims(importedDict['data'][channelKey][dataType])
-                    height = maxY + 1
-                    width = maxX + 1
-                    paramsViewer = '--name /viewer/' + channelAndDataType + \
-                                    ' --w ' + str((width) * 2) + \
-                                    ' --h ' + str((height) * 2) + ' --synch' + \
-                                    ' --RefreshTime 33'
-                    writeModule(xmlFile=xmlFile, name='yarpview', parameters=paramsViewer, dependencies=dependencyStr)
-                    dependencyStr = ''                    
-
-                    fromPort = '/file/' + channelAndDataType + ':o'
-                    toPort = '/viewer/' + channelAndDataType 
-                    writeConnection(xmlFile=xmlFile, fromPort=fromPort, toPort=toPort)
-
-                if dataType == 'imu':
-                    paramsFramer = '--name /framer' + channelAndDataType + \
-                                                  ' --height 200' + \
-                                                  ' --width 200' + \
-                                                  ' --displays "(/' + channelAndDataType + ' (AE IMU))"'
-                    writeModule(xmlFile=xmlFile, name='vFramerLite', parameters=paramsFramer, dependencies=dependencyStr)
-                    dependencyStr = ''                    
-                    paramsViewer = '--name /viewer/' + channelAndDataType + \
-                                    ' --w 400 --h 400 --synch'
-                    writeModule(xmlFile=xmlFile, name='yarpview', parameters=paramsViewer)
-                    
-                    fromPort = '/file/' + channelAndDataType + ':o'
-                    toPort = '/framer' + channelAndDataType + '/' + channelAndDataType + '/IMUS:i'
-                    writeConnection(xmlFile=xmlFile, fromPort=fromPort, toPort=toPort)
-                    
-                    fromPort = '/framer' + channelAndDataType + '/' + channelAndDataType + '/image:o'
-                    toPort = '/viewer/' + channelAndDataType 
-                    writeConnection(xmlFile=xmlFile, fromPort=fromPort, toPort=toPort)
-                    
-                    
-        xmlFile.write('</application>\n')
-
-def encodeEvents24Bit(ts, x, y, pol, **kwargs):
-    # timestamps(ts) are 32 bit integers counted with an 80 ns clock. 
-    # Events are encoded as 32 bits with x,y,channel(ch)(c) and polarity(pol)(p) as shown below
-    # 0000 0000 tcrr yyyy yyyy rrxx xxxx xxxp    (r = reserved)
-    # t = 0 to indicate events
-    # Ignoring channel though
-    ts = ts / 0.00000008
-    ts = ts.astype(np.uint32) # Timestamp wrapping occurs here
-    ts = np.expand_dims(ts, 1)
-    x = x.astype(np.int32)
-    y = y.astype(np.int32)
-    pol = (~pol).astype(np.int32)
-    channel = kwargs.get('channel', 0)
-    ae = (channel << 22) + (y << 12) + (x << 1) + pol
-    ae = np.expand_dims(ae, 1)
-    data = np.concatenate([ts, ae], axis=1)
-    data = data.flatten().tolist()
-    data = list(map(str, data))
-    return data
-
-def exportDvs(dataFile, data, bottleNumber, **kwargs):
-    # preconvert numpy arrays into bottle-ready data
-    print('Converting event arrays to bottle-ready string format ...')
-    eventsAsListOfStrings = encodeEvents24Bit(data['ts'], 
-                                              data['x'],
-                                              data['y'],
-                                              data['pol'],
-                                              **kwargs)
-    print('Breaking into bottles by time')
-    # Output dvs data bottle by bottle.
-    minTimeStepPerBottle = kwargs.get('minTimeStepPerBottle', 2e-3)
-    numEvents = len(data['ts'])
-    ptr = 0
-    pbar = tqdm(total=numEvents, position=0, leave=True)
-    bottleStrs = []
-    while ptr < numEvents:
-        firstTs = data['ts'][ptr]
-        nextPtr = np.searchsorted(data['ts'], firstTs + minTimeStepPerBottle)
-        pbar.update(nextPtr-ptr)
-        bottleStrs.append(str(bottleNumber) + ' ' + 
-                       '{0:.6f}'.format(firstTs) + ' AE (' +
-                       ' '.join(eventsAsListOfStrings[ptr*2 : nextPtr*2]) + ')')
-        ptr = nextPtr
-        bottleNumber += 1 
-    dataFile.write('\n'.join(bottleStrs))
-
-def exportFrame(dataFile, data, **kwargs):
-    # Here is an example from the python camera - rgb though:
-    # 1368 1571751370.660680 [mat] [rgb] (3 230400 8 320 240) {45 43 ... }
-    lineStrs = []
-    for bottleNum, tsFrameTuple in enumerate(tqdm(list(zip(data['ts'], data['frames'])), position=0, leave=True)):
-        ts, frame = tsFrameTuple
-        xDim, yDim = frame.shape
-        lineStrs.append(str(bottleNum + 1) + ' ' + "{0:.3f}".format(ts) + ' [mat] [mono] (' + 
-            ' '.join(['1', str(frame.size), '8', str((frame.shape)[0]), str((frame.shape)[1])]) + ') {' +
-            ' '.join(list(map(str, frame.flatten().tolist()))) + '}\n')
-
-        ''' expand mono to rgb
-        frameRgb = np.reshape(frame, (-1, 1))
-        frameRgb = (frameRgb.astype('float64') * 99 / 255).astype('uint8')  
-        frameRgb = np.concatenate((frameRgb, frameRgb, frameRgb), axis=1).flatten()
-        frameRgb = np.random.randint(low=0, high=100, size=129600, dtype=np.uint8)
-        lineStrs.append(str(bottleNum + 1) + ' ' + "{0:.6f}".format(ts) + ' [mat] [rgb] (' + 
-            ' '.join(['3', str(frame.size * 3), '8', str((frame.shape)[0]), str((frame.shape)[1])]) + ') {' +
-            ' '.join(list(map(str, frameRgb.tolist()))) + '}\n')
-        '''
-    dataFile.write(''.join(lineStrs))
-
-def exportPose6q(dataFile, data, **kwargs):
-    # Following Prashanth's lead here:  https://github.com/robotology/whole-body-estimators/blob/b55be34ce0abab46a14b7bb25d39d9ede5d05d0e/devices/baseEstimatorV1/include/baseEstimatorV1.h#L421
-    pass
-
-def encodeImu(ts, **kwargs):
-    # An IMU reading should go in a bottle with 10 consecutive events.
-    # Bottles may contain multiple packets like this
-    # An event is a 4-byte ts followed by a 4-byte sample
-    # timestamps(ts) are 32 bit integers counted with an 80 ns clock. 
-    # Events are encoded as 32 bits with value(v), sensor(s), channel(c), and typet) as shown below
-    # rrrr rrrr tcrr ssss vvvv vvvv vvvv vvvv    (r = reserved = 0)
-    # Ignoring channel though
-    ''' Struct of imu sample is (from LSB to MSB):
-    int value:16;
-    unsigned int sensor:4; - see below ...
-    unsigned int _r1:2; - reserved
-    unsigned int channel:1; - left vs right
-    unsigned int type:1; - should be 1 to indicate sample (cf event)
-    unsigned int _r2:8; - reserved
-    'Sensor' is defined as: 
-    0: Accel -Y
-    1: Accel X
-    2: Accel Z
-    3: Gyro -Y
-    4: Gyro X
-    5: Gyro Z
-    6: Temperature
-    7: Mag -Y
-    8: Mag X
-    9: Mag Z
-    
-    For the IMU on STEFI, which is this one:
-    ICM-20648, gyro full scale is +/-2000 degrees per second,
-    accelerometer full scale is +/-2 g.    
-    temp - 333.87 - but does it zero at 0K or at room temperature? (+21deg)
-    mag - no idea - this model doesn't have an internal mag
-    '''
-    numSamples = len(ts)
-    accConversionFactor = kwargs.get('accConversionFactor', (32768 / 2) / 9.80665)
-    angVConversionFactor = kwargs.get('angVConversionFactor', (32768 / 250) * (180 / np.pi))
-    tempConversionFactor = kwargs.get('tempConversionFactor', 333.87)
-    tempConversionOffset = kwargs.get('tempConversionOffset', -273.15 - 21)
-    magConversionFactor = kwargs.get('magConversionFactor', (32768 / 4900) * 1000000)
-    
-    acc = kwargs.get('acc')
-    angV = kwargs.get('angV')
-    temp = kwargs.get('temp')
-    mag = kwargs.get('mag')
-    
-    acc = np.zeros((numSamples, 3), dtype = np.int16) if acc is None else (acc * accConversionFactor).astype(np.int16)
-    angV = np.zeros((numSamples, 3), dtype = np.int16) if angV is None else (angV * angVConversionFactor).astype(np.int16)
-    temp = np.zeros((numSamples, 1), dtype = np.int16) if temp is None else ((temp + tempConversionOffset) * tempConversionFactor).astype(np.int16)
-    mag = np.zeros((numSamples, 3), dtype = np.int16) if mag is None else (mag * magConversionFactor).astype(np.int16)
-    
-    # switch X and Y; negate Y, to match IMU as mounted on Stefi
-    acc = acc[:, [1, 0, 2]]
-    angV = angV[:, [1, 0, 2]]
-    mag = mag[:, [1, 0, 2]]
-    acc[:, 0] = - acc[:, 0]
-    angV[:, 0] = - angV[:, 0]
-    mag[:, 0] = - mag[:, 0]
-    
-    ts = ts / 0.00000008
-    ts = ts.astype(np.uint32) # Timestamp wrapping occurs here
-    ts = np.tile(ts, (1, 10))
-    ts = ts.flatten(order='C')
-    ts = np.expand_dims(ts, 1)
-    values = np.concatenate((acc, angV, temp, mag), axis=1)
-    values = values.flatten(order='C')
-    sensor = np.tile(np.arange(10, dtype=np.uint32), (numSamples, 1))
-    sensor = sensor.flatten(order='C')
-    channel = kwargs.get('channel', 0)
-    eventType = 1
-    ae = (eventType << 23) + (channel << 22) + (sensor << 16) + values 
-    ae = np.expand_dims(ae, 1)
-    data = np.concatenate([ts, ae], axis=1)
-    data = data.flatten().tolist()
-    data = list(map(str, data))
-    return data
-      
-def exportImu(dataFile, data, bottleNumber, **kwargs):
-    # preconvert numpy arrays into bottle-ready data
-    print('Converting event arrays to bottle-ready string format ...')
-    eventsAsListOfStrings = encodeImu(ts=data['ts'], 
-                                      acc=data['acc'],
-                                      angV=data['angV'])
-    print('Breaking into bottles by time')
-    # Output dvs data bottle by bottle.
-    minTimeStepPerBottle = kwargs.get('minTimeStepPerBottle', 2e-3)
-    numEvents = len(data['ts'])
-    ptr = 0
-    pbar = tqdm(total=numEvents, position=0, leave=True)
-    bottleStrs = []
-    while ptr < numEvents:
-        firstTs = data['ts'][ptr]
-        nextPtr = np.searchsorted(data['ts'], firstTs + minTimeStepPerBottle)
-        pbar.update(nextPtr-ptr)
-        # Why 20 in the following? Because there are 10 samples per imu and 2 ints per sample that need to be included. 
-        bottleStrs.append(str(bottleNumber) + ' ' + 
-                       '{0:.6f}'.format(firstTs) + ' IMUS (' +
-                       ' '.join(eventsAsListOfStrings[ptr*20 : nextPtr*20]) + ')')
-        ptr = nextPtr
-        bottleNumber += 1 
-    dataFile.write('\n'.join(bottleStrs))
-
-def encodeSample(data, **kwargs):
-    # Samples are encoded like this
-    # An event is a 4-byte ts followed by a 4-byte sample
-    # timestamps(ts) are 32 bit integers counted with an 80 ns clock. 
-    # Events are encoded as 32 bits with value(v), sensor(s), channel(c), and typet) as shown below
-    # rrrr rrrr tcrr ssss vvvv vvvv vvvv vvvv    (r = reserved = 0)
-    # Ignoring channel though
-    
-    #Unpack
-    ts = data['ts']
-    sensor = data['sensor'].astype(np.uint32) # change type to allow shifting up bits
-    value = data['value'].astype(np.uint16) # change to unsigned int to avoid wrapping in the sum below
-    ts = ts / 0.00000008
-    ts = ts.astype(np.uint32) # Timestamp wrapping occurs here
-    ts = np.expand_dims(ts, 1)
-    channel = kwargs.get('channel', 0)
-    eventType = 1
-    ae = (eventType << 23) + (channel << 22) + (sensor << 16) + value
-    ae = np.expand_dims(ae, 1)
-    data = np.concatenate([ts, ae], axis=1)
-    data = data.flatten().tolist()
-    data = list(map(str, data))
-    return data
-      
-
-def exportSample(dataFile, data, bottleNumber, **kwargs):
-    # preconvert numpy arrays into bottle-ready data
-    print('Converting event arrays to bottle-ready string format ...')
-    eventsAsListOfStrings = encodeSample(data, **kwargs)
-    print('Breaking into bottles by time')
-    # Output dvs data bottle by bottle.
-    minTimeStepPerBottle = kwargs.get('minTimeStepPerBottle', 2e-3)
-    numEvents = len(data['ts'])
-    ptr = 0
-    pbar = tqdm(total=numEvents, position=0, leave=True)
-    bottleStrs = []
-    while ptr < numEvents:
-        firstTs = data['ts'][ptr]
-        nextPtr = np.searchsorted(data['ts'], firstTs + minTimeStepPerBottle)
-        pbar.update(nextPtr-ptr)
-        # Why 20 in the following? Because there are 10 samples per imu and 2 ints per sample that need to be included. 
-        bottleStrs.append(str(bottleNumber) + ' ' + 
-                       '{0:.6f}'.format(firstTs) + ' IMUS (' +
-                       ' '.join(eventsAsListOfStrings[ptr*2 : nextPtr*2]) + ')')
-        ptr = nextPtr
-        bottleNumber += 1 
-    dataFile.write('\n'.join(bottleStrs))
-      
-def exportIitYarp(importedDict, **kwargs):
-    exportFilePath = kwargs.get('exportFilePath', './')
-    if isinstance(importedDict, list):
-        for idx, elem in enumerate(importedDict):
-            kwargs['exportFilePath'] = exportFilePath + '/' + str(idx)
-            exportIitYarp(elem, **kwargs)
-        return
-    print('exportIitYarp called for data imported from ' + 
-          str(importedDict['info']) +
-          ' targeting folder ' + exportFilePath)
-    try:
-        os.makedirs(exportFilePath)
-    except FileExistsError: # The folder already exists
-        pass
-    yarpOutputPort = kwargs.get('yarpOutputPort', '/file')
-    channelNames = importedDict['data'].keys()
-    dataTypesToExport = kwargs.get('dataTypes')
-    for channelName in channelNames:
-        if channelName in ['1', 'right']:
-            kwargs['channel'] = 1
-        else:
-            kwargs['channel'] = 0
-        dataTypes = importedDict['data'][channelName].keys()
-        for dataType in dataTypes:
-            if dataTypesToExport is None or dataType in dataTypesToExport: # , 'pose6', 'imu'                
-                if dataType not in ['dvs', 'frame', 'imu', 'sample']: 
-                    print('unknown datatype')
-                    continue # Exclude unknown datatypes
-                channelNameAndDataType = channelName + dataType # This is used as a new channel name
-                channelPath = os.path.join(exportFilePath, str(channelNameAndDataType))
-                try:
-                    os.mkdir(channelPath)
-                except FileExistsError: # The folder already exists
-                    pass
-                dirList = os.listdir(channelPath)
-
-                writeMode = kwargs.get('writeMode', 'w')
-                if 'data.log' in dirList:
-                    print('data already exists in export directory for channel and datatype' + str(channelNameAndDataType))
-                    if kwargs.get('protectedWrite', True):
-                        print('export not performed')
-                        continue
-                    else:
-                        if writeMode == 'w':
-                            print('data is being overwritten!')
-                        elif writeMode == 'a':
-                            print('data is being appended!')
-                            with open(os.path.join(channelPath, 'data.log'), 'r') as f:
-                                lines = f.read().splitlines()
-                                bottleNumberStart = len(lines)
-
-                # Write the info.log file
-                yarpOutputPortForChannel = yarpOutputPort + '/' + channelNameAndDataType + ":o"
-                with open(os.path.join(channelPath, 'info.log'), 'w') as infoFile:
-                    infoFile.write('Type: Bottle;\n')
-                    # TODO: get the real start time from the 'info', if it exists 
-                    # - placeholder 0.0 put in the following line 
-                    infoFile.write('[0.0] ' + yarpOutputPortForChannel + ' [connected]\n')
-                # Write the data.log file
-                with open(os.path.join(channelPath, 'data.log'), writeMode) as dataFile:
-                    if writeMode == 'a':
-                        dataFile.write('\n')
-                    data = importedDict['data'][channelName][dataType]
-                    if dataType == 'dvs':
-                        if writeMode == 'a':
-                             exportDvs(dataFile, data, bottleNumberStart, **kwargs)
-                        else:
-                            exportDvs(dataFile, data, 0, **kwargs)
-                    elif dataType == 'frame':
-                        # TODO: handle bottle numbering for writeMode = 'a'
-                        exportFrame(dataFile, data, **kwargs)
-                    elif dataType == 'imu':
-                        if writeMode == 'a':
-                            exportImu(dataFile, data, bottleNumberStart, **kwargs)
-                        else:
-                            exportImu(dataFile, data, 0, **kwargs)
-                    elif dataType == 'pose6q':
-                        # TODO: handle bottle numbering for writeMode = 'a'
-                        exportPose6q(dataFile, data, **kwargs)
-                    elif dataType == 'sample':
-                        if writeMode == 'a':
-                            exportSample(dataFile, data, bottleNumberStart, **kwargs)
-                        else:
-                            exportSample(dataFile, data, 0, **kwargs)
-            else:
-                print("datatype: ", dataType, " not handled yet")
-    if kwargs.get('viewerApp', True):
+# -*- coding: utf-8 -*-
+"""
+Copyright (C) 2019 Event-driven Perception for Robotics
+Authors: Sim Bamford
+Code contributions from:
+        Vadim Tikhanoff
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
+exportIitYarp takes a data dict resulting from importAe.
+Exports data.log and info.log for each channel contained.
+Uses the "exportFilePath" parameter for the top-level folder,
+creating it if it doesn't exist. This can be relative or absolute.
+Defaults to the current directory.
+Uses the "yarpOutputPort" parameter for the port defined in info.log.
+Default is "/file" - then the following is appended: "/AE:o"
+Where more than one channel is contained, the channel name is used in place of "AE".
+If the "viewerApp" parameter is True (default = True), then a play.xml 
+file is created at the top level directory, which is configured so that when
+run from yarpmanager, the data which has been exported can be viewed.
+"writeProtected" (default=True) protects any existing data in the target exportFilePath from being overwritten.
+"writeMode" (default='w') can be set to append mode ('a') for exporting (large) files in batches.
+"""
+
+#%%
+
+import os
+import numpy as np
+from tqdm import tqdm
+import string
+
+# TODO: this could come from header info in some cases
+def getDims(dataTypeDict):
+    if 'pol' in dataTypeDict: # dvs
+        minX = np.min(dataTypeDict['x'])
+        maxX = np.max(dataTypeDict['x'])
+        minY = np.min(dataTypeDict['y'])
+        maxY = np.max(dataTypeDict['y'])
+    elif 'frames' in dataTypeDict:
+        minX = 0
+        maxX = (dataTypeDict['frames'][0].shape)[0]
+        minY = 0
+        maxY = (dataTypeDict['frames'][0].shape)[1]
+    return minX, maxX, minY, maxY
+
+def writeModule(xmlFile, name, **kwargs):
+    xmlFile.write('<module>\n')
+    xmlFile.write('    <name> ' + name + ' </name>\n')
+    parameters = kwargs.get('parameters', '')
+    xmlFile.write('    <parameters> ' + parameters + ' </parameters>\n')
+    dependencies = kwargs.get('dependencies', '')
+    if dependencies != '':
+        xmlFile.write('    <dependencies>\n')
+        xmlFile.write('        ' + dependencies + '\n')
+        xmlFile.write('    </dependencies>\n')
+    xmlFile.write('    <node> localhost </node>\n')
+    xmlFile.write('</module>\n')
+    xmlFile.write('\n')
+
+def writeConnection(xmlFile, fromPort, toPort, **kwargs):
+    xmlFile.write('<connection>\n')
+    xmlFile.write('    <from> ' + fromPort + ' </from>\n')
+    xmlFile.write('    <to> ' + toPort + ' </to>\n')
+    protocol = kwargs.get('protocol', 'udp')
+    xmlFile.write('<protocol> ' + protocol + ' </protocol>\n')
+    xmlFile.write('</connection>\n')
+    xmlFile.write('\n')
+
+def exportIitYarpViewer(importedDict, **kwargs):
+    exportFilePath = kwargs.get('exportFilePath', './')
+    with open(os.path.join(exportFilePath, 'play.xml'), 'w') as xmlFile:
+        xmlFile.write('<application>\n')
+        xmlFile.write('<name>play </name>\n')
+        xmlFile.write('\n')
+        writeModule(xmlFile=xmlFile, name='yarpdataplayer')
+        pathForPlayback = kwargs.get('pathForPlayback', exportFilePath)
+        #dependencyStr = ''
+        dependencyStr = '<port timeout="100.0" request="load ' + pathForPlayback + '" reply="[ok]">/yarpdataplayer/rpc:i</port>'
+        dataTypesToExport = kwargs.get('dataTypes')
+        for channelKey in importedDict['data']:
+            for dataType in importedDict['data'][channelKey]:
+                if dataTypesToExport is not None and dataType not in dataTypesToExport: continue
+                channelKeyStripped = str(channelKey).translate(str.maketrans('', '', string.punctuation))
+                channelAndDataType = channelKeyStripped + dataType
+
+                if dataType == 'dvs':
+                    minX, maxX, minY, maxY = getDims(importedDict['data'][channelKey][dataType])
+                    height = maxY + 1
+                    width = maxX + 1
+                    paramsFramer = '--name /framer' + channelAndDataType + \
+                                                   ' --height ' + str(height) + \
+                                                   ' --width ' + str(width) + \
+                                                   ' --displays "(/' + channelAndDataType + ' (AE ISO))"'
+                    writeModule(xmlFile=xmlFile, name='vFramerLite', parameters=paramsFramer, dependencies=dependencyStr)
+                    dependencyStr = ''
+                    paramsViewer = '--name /viewer/' + channelAndDataType + \
+                                    ' --w ' + str((width) * 2) + \
+                                    ' --h ' + str((height) * 2) + ' --synch'
+                    writeModule(xmlFile=xmlFile, name='yarpview', parameters=paramsViewer)
+
+                    fromPort = '/file/' + channelAndDataType + ':o'
+                    toPort = '/framer' + channelAndDataType + '/' + channelAndDataType + '/AE:i'
+                    writeConnection(xmlFile=xmlFile, fromPort=fromPort, toPort=toPort)
+
+                    fromPort = '/framer' + channelAndDataType + '/' + channelAndDataType + '/image:o'
+                    toPort = '/viewer/' + channelAndDataType
+                    writeConnection(xmlFile=xmlFile, fromPort=fromPort, toPort=toPort)
+
+                if dataType == 'frame':
+                    minX, maxX, minY, maxY = getDims(importedDict['data'][channelKey][dataType])
+                    height = maxY + 1
+                    width = maxX + 1
+                    paramsViewer = '--name /viewer/' + channelAndDataType + \
+                                    ' --w ' + str((width) * 2) + \
+                                    ' --h ' + str((height) * 2) + ' --synch' + \
+                                    ' --RefreshTime 33'
+                    writeModule(xmlFile=xmlFile, name='yarpview', parameters=paramsViewer, dependencies=dependencyStr)
+                    dependencyStr = ''
+
+                    fromPort = '/file/' + channelAndDataType + ':o'
+                    toPort = '/viewer/' + channelAndDataType
+                    writeConnection(xmlFile=xmlFile, fromPort=fromPort, toPort=toPort)
+
+                if dataType == 'imu':
+                    paramsFramer = '--name /framer' + channelAndDataType + \
+                                                  ' --height 200' + \
+                                                  ' --width 200' + \
+                                                  ' --displays "(/' + channelAndDataType + ' (AE IMU))"'
+                    writeModule(xmlFile=xmlFile, name='vFramerLite', parameters=paramsFramer, dependencies=dependencyStr)
+                    dependencyStr = ''
+                    paramsViewer = '--name /viewer/' + channelAndDataType + \
+                                    ' --w 400 --h 400 --synch'
+                    writeModule(xmlFile=xmlFile, name='yarpview', parameters=paramsViewer)
+
+                    fromPort = '/file/' + channelAndDataType + ':o'
+                    toPort = '/framer' + channelAndDataType + '/' + channelAndDataType + '/IMUS:i'
+                    writeConnection(xmlFile=xmlFile, fromPort=fromPort, toPort=toPort)
+
+                    fromPort = '/framer' + channelAndDataType + '/' + channelAndDataType + '/image:o'
+                    toPort = '/viewer/' + channelAndDataType
+                    writeConnection(xmlFile=xmlFile, fromPort=fromPort, toPort=toPort)
+
+
+        xmlFile.write('</application>\n')
+
+def encodeEvents24Bit(ts, x, y, pol, ch=None, **kwargs):
+    # timestamps(ts) are 32 bit integers counted with an 80 ns clock. 
+    # Events are encoded as 32 bits with x,y,channel(ch)(c) and polarity(pol)(p) as shown below
+    # 0000 0000 tcrr yyyy yyyy rrxx xxxx xxxp    (r = reserved)
+    # t = 0 to indicate events
+    # Ignoring channel though
+    ts = ts / 0.00000008
+    ts = ts.astype(np.uint32) # Timestamp wrapping occurs here
+    ts = np.expand_dims(ts, 1)
+    x = x.astype(np.uint32)
+    y = y.astype(np.uint32)
+    pol = (~pol).astype(np.uint32)
+    # if ch stream is absent, data has already been split into left and right channels
+    # in that case, assign channel value of the whole stream (left or right) from kwargs
+    if ch is None:
+        ch = kwargs.get('channel', 0)
+        ch = np.uint32(ch)
+    else:
+        ch = ch.astype(np.uint32)
+    ae = (ch << 22) + (y << 12) + (x << 1) + pol
+    ae = np.expand_dims(ae, 1)
+    data = np.concatenate([ts, ae], axis=1)
+    data = data.flatten().tolist()
+    data = list(map(str, data))
+    return data
+
+def exportDvs(dataFile, data, bottleNumber, **kwargs):
+    # preconvert numpy arrays into bottle-ready data
+    print('Converting event arrays to bottle-ready string format ...')
+    ch=None
+    if 'ch' in data:
+        ch = data['ch']
+    eventsAsListOfStrings = encodeEvents24Bit(data['ts'],
+                                              data['x'],
+                                              data['y'],
+                                              data['pol'],
+                                              ch,
+                                              **kwargs)
+    print('Breaking into bottles by time')
+    # Output dvs data bottle by bottle.
+    minTimeStepPerBottle = kwargs.get('minTimeStepPerBottle', 2e-3)
+    numEvents = len(data['ts'])
+    ptr = 0
+    pbar = tqdm(total=numEvents, position=0, leave=True)
+    bottleStrs = []
+    while ptr < numEvents:
+        firstTs = data['ts'][ptr]
+        nextPtr = np.searchsorted(data['ts'], firstTs + minTimeStepPerBottle)
+        pbar.update(nextPtr-ptr)
+        bottleStrs.append(str(bottleNumber) + ' ' +
+                       '{0:.6f}'.format(firstTs) + ' AE (' +
+                       ' '.join(eventsAsListOfStrings[ptr*2 : nextPtr*2]) + ')')
+        ptr = nextPtr
+        bottleNumber += 1
+    dataFile.write('\n'.join(bottleStrs))
+
+def exportFrame(dataFile, data, **kwargs):
+    # Here is an example from the python camera - rgb though:
+    # 1368 1571751370.660680 [mat] [rgb] (3 230400 8 320 240) {45 43 ... }
+    lineStrs = []
+    for bottleNum, tsFrameTuple in enumerate(tqdm(list(zip(data['ts'], data['frames'])), position=0, leave=True)):
+        ts, frame = tsFrameTuple
+        xDim, yDim = frame.shape
+        lineStrs.append(str(bottleNum + 1) + ' ' + "{0:.3f}".format(ts) + ' [mat] [mono] (' +
+            ' '.join(['1', str(frame.size), '8', str((frame.shape)[0]), str((frame.shape)[1])]) + ') {' +
+            ' '.join(list(map(str, frame.flatten().tolist()))) + '}\n')
+
+        ''' expand mono to rgb
+        frameRgb = np.reshape(frame, (-1, 1))
+        frameRgb = (frameRgb.astype('float64') * 99 / 255).astype('uint8')  
+        frameRgb = np.concatenate((frameRgb, frameRgb, frameRgb), axis=1).flatten()
+        frameRgb = np.random.randint(low=0, high=100, size=129600, dtype=np.uint8)
+        lineStrs.append(str(bottleNum + 1) + ' ' + "{0:.6f}".format(ts) + ' [mat] [rgb] (' + 
+            ' '.join(['3', str(frame.size * 3), '8', str((frame.shape)[0]), str((frame.shape)[1])]) + ') {' +
+            ' '.join(list(map(str, frameRgb.tolist()))) + '}\n')
+        '''
+    dataFile.write(''.join(lineStrs))
+
+def exportPose6q(dataFile, data, **kwargs):
+    # Following Prashanth's lead here:  https://github.com/robotology/whole-body-estimators/blob/b55be34ce0abab46a14b7bb25d39d9ede5d05d0e/devices/baseEstimatorV1/include/baseEstimatorV1.h#L421
+    pass
+
+def encodeImu(ts, **kwargs):
+    # An IMU reading should go in a bottle with 10 consecutive events.
+    # Bottles may contain multiple packets like this
+    # An event is a 4-byte ts followed by a 4-byte sample
+    # timestamps(ts) are 32 bit integers counted with an 80 ns clock. 
+    # Events are encoded as 32 bits with value(v), sensor(s), channel(c), and typet) as shown below
+    # rrrr rrrr tcrr ssss vvvv vvvv vvvv vvvv    (r = reserved = 0)
+    # Ignoring channel though
+    ''' Struct of imu sample is (from LSB to MSB):
+    int value:16;
+    unsigned int sensor:4; - see below ...
+    unsigned int _r1:2; - reserved
+    unsigned int channel:1; - left vs right
+    unsigned int type:1; - should be 1 to indicate sample (cf event)
+    unsigned int _r2:8; - reserved
+    'Sensor' is defined as: 
+    0: Accel -Y
+    1: Accel X
+    2: Accel Z
+    3: Gyro -Y
+    4: Gyro X
+    5: Gyro Z
+    6: Temperature
+    7: Mag -Y
+    8: Mag X
+    9: Mag Z
+    
+    For the IMU on STEFI, which is this one:
+    ICM-20648, gyro full scale is +/-2000 degrees per second,
+    accelerometer full scale is +/-2 g.    
+    temp - 333.87 - but does it zero at 0K or at room temperature? (+21deg)
+    mag - no idea - this model doesn't have an internal mag
+    '''
+    numSamples = len(ts)
+    accConversionFactor = kwargs.get('accConversionFactor', (32768 / 2) / 9.80665)
+    angVConversionFactor = kwargs.get('angVConversionFactor', (32768 / 250) * (180 / np.pi))
+    tempConversionFactor = kwargs.get('tempConversionFactor', 333.87)
+    tempConversionOffset = kwargs.get('tempConversionOffset', -273.15 - 21)
+    magConversionFactor = kwargs.get('magConversionFactor', (32768 / 4900) * 1000000)
+
+    acc = kwargs.get('acc')
+    angV = kwargs.get('angV')
+    temp = kwargs.get('temp')
+    mag = kwargs.get('mag')
+
+    acc = np.zeros((numSamples, 3), dtype = np.int16) if acc is None else (acc * accConversionFactor).astype(np.int16)
+    angV = np.zeros((numSamples, 3), dtype = np.int16) if angV is None else (angV * angVConversionFactor).astype(np.int16)
+    temp = np.zeros((numSamples, 1), dtype = np.int16) if temp is None else ((temp + tempConversionOffset) * tempConversionFactor).astype(np.int16)
+    mag = np.zeros((numSamples, 3), dtype = np.int16) if mag is None else (mag * magConversionFactor).astype(np.int16)
+
+    # switch X and Y; negate Y, to match IMU as mounted on Stefi
+    acc = acc[:, [1, 0, 2]]
+    angV = angV[:, [1, 0, 2]]
+    mag = mag[:, [1, 0, 2]]
+    acc[:, 0] = - acc[:, 0]
+    angV[:, 0] = - angV[:, 0]
+    mag[:, 0] = - mag[:, 0]
+
+    ts = ts / 0.00000008
+    ts = ts.astype(np.uint32) # Timestamp wrapping occurs here
+    ts = np.tile(ts, (1, 10))
+    ts = ts.flatten(order='C')
+    ts = np.expand_dims(ts, 1)
+    values = np.concatenate((acc, angV, temp, mag), axis=1)
+    values = values.flatten(order='C')
+    sensor = np.tile(np.arange(10, dtype=np.uint32), (numSamples, 1))
+    sensor = sensor.flatten(order='C')
+    channel = kwargs.get('channel', 0)
+    eventType = 1
+    ae = (eventType << 23) + (channel << 22) + (sensor << 16) + values
+    ae = np.expand_dims(ae, 1)
+    data = np.concatenate([ts, ae], axis=1)
+    data = data.flatten().tolist()
+    data = list(map(str, data))
+    return data
+
+def exportImu(dataFile, data, bottleNumber, **kwargs):
+    # preconvert numpy arrays into bottle-ready data
+    print('Converting event arrays to bottle-ready string format ...')
+    eventsAsListOfStrings = encodeImu(ts=data['ts'],
+                                      acc=data['acc'],
+                                      angV=data['angV'])
+    print('Breaking into bottles by time')
+    # Output dvs data bottle by bottle.
+    minTimeStepPerBottle = kwargs.get('minTimeStepPerBottle', 2e-3)
+    numEvents = len(data['ts'])
+    ptr = 0
+    pbar = tqdm(total=numEvents, position=0, leave=True)
+    bottleStrs = []
+    while ptr < numEvents:
+        firstTs = data['ts'][ptr]
+        nextPtr = np.searchsorted(data['ts'], firstTs + minTimeStepPerBottle)
+        pbar.update(nextPtr-ptr)
+        # Why 20 in the following? Because there are 10 samples per imu and 2 ints per sample that need to be included. 
+        bottleStrs.append(str(bottleNumber) + ' ' +
+                       '{0:.6f}'.format(firstTs) + ' IMUS (' +
+                       ' '.join(eventsAsListOfStrings[ptr*20 : nextPtr*20]) + ')')
+        ptr = nextPtr
+        bottleNumber += 1
+    dataFile.write('\n'.join(bottleStrs))
+
+def encodeSample(data, **kwargs):
+    # Samples are encoded like this
+    # An event is a 4-byte ts followed by a 4-byte sample
+    # timestamps(ts) are 32 bit integers counted with an 80 ns clock. 
+    # Events are encoded as 32 bits with value(v), sensor(s), channel(c), and typet) as shown below
+    # rrrr rrrr tcrr ssss vvvv vvvv vvvv vvvv    (r = reserved = 0)
+    # Ignoring channel though
+
+    #Unpack
+    ts = data['ts']
+    sensor = data['sensor'].astype(np.uint32) # change type to allow shifting up bits
+    value = data['value'].astype(np.uint16) # change to unsigned int to avoid wrapping in the sum below
+    ts = ts / 0.00000008
+    ts = ts.astype(np.uint32) # Timestamp wrapping occurs here
+    ts = np.expand_dims(ts, 1)
+    channel = kwargs.get('channel', 0)
+    eventType = 1
+    ae = (eventType << 23) + (channel << 22) + (sensor << 16) + value
+    ae = np.expand_dims(ae, 1)
+    data = np.concatenate([ts, ae], axis=1)
+    data = data.flatten().tolist()
+    data = list(map(str, data))
+    return data
+
+
+def exportSample(dataFile, data, bottleNumber, **kwargs):
+    # preconvert numpy arrays into bottle-ready data
+    print('Converting event arrays to bottle-ready string format ...')
+    eventsAsListOfStrings = encodeSample(data, **kwargs)
+    print('Breaking into bottles by time')
+    # Output dvs data bottle by bottle.
+    minTimeStepPerBottle = kwargs.get('minTimeStepPerBottle', 2e-3)
+    numEvents = len(data['ts'])
+    ptr = 0
+    pbar = tqdm(total=numEvents, position=0, leave=True)
+    bottleStrs = []
+    while ptr < numEvents:
+        firstTs = data['ts'][ptr]
+        nextPtr = np.searchsorted(data['ts'], firstTs + minTimeStepPerBottle)
+        pbar.update(nextPtr-ptr)
+        # Why 20 in the following? Because there are 10 samples per imu and 2 ints per sample that need to be included. 
+        bottleStrs.append(str(bottleNumber) + ' ' +
+                       '{0:.6f}'.format(firstTs) + ' IMUS (' +
+                       ' '.join(eventsAsListOfStrings[ptr*2 : nextPtr*2]) + ')')
+        ptr = nextPtr
+        bottleNumber += 1
+    dataFile.write('\n'.join(bottleStrs))
+    
+    
+def encodeSkeleton(inData, **kwargs):
+    data = np.array([], dtype = np.uint32)
+    for i in range(len(inData['ts'])):
+        for key in inData:
+            if(key != 'ts'):
+                data = np.append(data, inData[key][i].astype(np.uint32))
+ 
+    data = data.flatten().tolist()
+    data = list(map(str, data))
+    return data
+
+def exportSkeleton(dataFile, data, bottleNumber, **kwargs):
+    # preconvert numpy arrays into bottle-ready data
+    print('Converting skeleton arrays to bottle-ready string format ...')
+    eventsAsListOfStrings = encodeSkeleton(data, **kwargs)
+    print('Breaking into bottles by time')
+    # Output skeleton data bottle by bottle.
+    minTimeStepPerBottle = kwargs.get('minTimeStepPerBottle', 2e-3)
+    numEvents = len(data['ts'])
+    ptr = 0
+    pbar = tqdm(total=numEvents, position=0, leave=True)
+    bottleStrs = []
+    while ptr < numEvents:
+        firstTs = data['ts'][ptr]
+        nextPtr = np.searchsorted(data['ts'], firstTs + minTimeStepPerBottle)
+        pbar.update(nextPtr-ptr)
+        bottleStrs.append(str(bottleNumber) + ' ' +
+                        '{0:.6f}'.format(firstTs) + ' SKLT (' +
+                        ' '.join(eventsAsListOfStrings[ptr*13*2 : nextPtr*13*2]) + ')')
+        ptr = nextPtr
+        bottleNumber += 1
+    dataFile.write('\n'.join(bottleStrs))
+    
+
+def exportIitYarp(importedDict, **kwargs):
+    exportFilePath = kwargs.get('exportFilePath', './')
+    if isinstance(importedDict, list):
+        for idx, elem in enumerate(importedDict):
+            kwargs['exportFilePath'] = exportFilePath + '/' + str(idx)
+            exportIitYarp(elem, **kwargs)
+        return
+    print('exportIitYarp called for data imported from ' +
+          str(importedDict['info']) +
+          ' targeting folder ' + exportFilePath)
+    try:
+        os.makedirs(exportFilePath)
+    except FileExistsError: # The folder already exists
+        pass
+    yarpOutputPort = kwargs.get('yarpOutputPort', '/file')
+    channelNames = importedDict['data'].keys()
+    dataTypesToExport = kwargs.get('dataTypes')
+    for channelName in channelNames:
+        if channelName in ['1', 'right']:
+            kwargs['channel'] = 1
+        else:
+            kwargs['channel'] = 0
+        dataTypes = importedDict['data'][channelName].keys()
+        for dataType in dataTypes:
+            if dataTypesToExport is None or dataType in dataTypesToExport: # , 'pose6', 'imu'
+                if dataType not in ['dvs', 'frame', 'imu', 'sample', 'skeleton']:
+                    print('unknown datatype')
+                    continue # Exclude unknown datatypes
+                channelNameAndDataType = channelName + dataType # This is used as a new channel name
+                channelPath = os.path.join(exportFilePath, str(channelNameAndDataType))
+                try:
+                    os.mkdir(channelPath)
+                except FileExistsError: # The folder already exists
+                    pass
+                dirList = os.listdir(channelPath)
+
+                writeMode = kwargs.get('writeMode', 'w')
+                if 'data.log' in dirList:
+                    print('data already exists in export directory for channel and datatype' + str(channelNameAndDataType))
+                    if kwargs.get('protectedWrite', True):
+                        print('export not performed')
+                        continue
+                    else:
+                        if writeMode == 'w':
+                            print('data is being overwritten!')
+                        elif writeMode == 'a':
+                            print('data is being appended!')
+                            with open(os.path.join(channelPath, 'data.log'), 'r') as f:
+                                lines = f.read().splitlines()
+                                bottleNumberStart = len(lines)
+
+                # Write the info.log file
+                yarpOutputPortForChannel = yarpOutputPort + '/' + channelNameAndDataType + ":o"
+                with open(os.path.join(channelPath, 'info.log'), 'w') as infoFile:
+                    infoFile.write('Type: Bottle;\n')
+                    # TODO: get the real start time from the 'info', if it exists 
+                    # - placeholder 0.0 put in the following line 
+                    infoFile.write('[0.0] ' + yarpOutputPortForChannel + ' [connected]\n')
+                # Write the data.log file
+                with open(os.path.join(channelPath, 'data.log'), writeMode) as dataFile:
+                    if writeMode == 'a':
+                        dataFile.write('\n')
+                    data = importedDict['data'][channelName][dataType]
+                    if dataType == 'dvs':
+                        if writeMode == 'a':
+                             exportDvs(dataFile, data, bottleNumberStart, **kwargs)
+                        else:
+                            exportDvs(dataFile, data, 0, **kwargs)
+                    elif dataType == 'frame':
+                        # TODO: handle bottle numbering for writeMode = 'a'
+                        exportFrame(dataFile, data, **kwargs)
+                    elif dataType == 'imu':
+                        if writeMode == 'a':
+                            exportImu(dataFile, data, bottleNumberStart, **kwargs)
+                        else:
+                            exportImu(dataFile, data, 0, **kwargs)
+                    elif dataType == 'pose6q':
+                        # TODO: handle bottle numbering for writeMode = 'a'
+                        exportPose6q(dataFile, data, **kwargs)
+                    elif dataType == 'sample':
+                        if writeMode == 'a':
+                            exportSample(dataFile, data, bottleNumberStart, **kwargs)
+                        else:
+                            exportSample(dataFile, data, 0, **kwargs)
+                    elif dataType == 'skeleton':
+                        if writeMode == 'a':
+                            exportSkeleton(dataFile, data, bottleNumberStart, **kwargs)
+                        else:
+                            exportSkeleton(dataFile, data, 0, **kwargs)
+            else:
+                print("datatype: ", dataType, " not handled yet")
+    if kwargs.get('viewerApp', True):
         exportIitYarpViewer(importedDict, **kwargs)
```

### Comparing `bimvee-1.0.9/bimvee/exportPoseRpgEsimCsv.py` & `bimvee-1.0.9.dev0/bimvee/exportPoseRpgEsimCsv.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# -*- coding: utf-8 -*-
-"""
-Copyright (C) 2020 Event-driven Perception for Robotics
-Authors: Simeon Bamford
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
-A function which exports a pose6q dataType dict as a csv for use by Rpg's eSim
-simulator (https://github.com/uzh-rpg/rpg_esim)
-
-Note:
-    a) conversion of ts to ns
-    b) switch of quaternion to qx, qy, qz, qw format
-"""
-
-
-def exportPoseRpgEsimCsv(poseDict, filePathAndName='poses.csv'):
-    ts = poseDict['ts']
-    point = poseDict['point']
-    rotation = poseDict['rotation']
-    with open(filePathAndName, 'w') as file:
-        file.write('# timestamp, x, y, z, qx, qy, qz, qw\n')
-        for idx in range(ts.shape[0]):
-            file.write('%f, %f, %f, %f, %f, %f, %f, %f\n' % (
-                    ts[idx] * 1000000000,                                                       
-                    point[idx, 0],                                                       
-                    point[idx, 1],                                                       
-                    point[idx, 2],                                                       
-                    rotation[idx, 1],                                                       
-                    rotation[idx, 2],                                                       
-                    rotation[idx, 3],                                                       
-                    rotation[idx, 0],                                                       
-                    ))
+# -*- coding: utf-8 -*-
+"""
+Copyright (C) 2020 Event-driven Perception for Robotics
+Authors: Simeon Bamford
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
+A function which exports a pose6q dataType dict as a csv for use by Rpg's eSim
+simulator (https://github.com/uzh-rpg/rpg_esim)
+
+Note:
+    a) conversion of ts to ns
+    b) switch of quaternion to qx, qy, qz, qw format
+"""
+
+
+def exportPoseRpgEsimCsv(poseDict, filePathAndName='poses.csv'):
+    ts = poseDict['ts']
+    point = poseDict['point']
+    rotation = poseDict['rotation']
+    with open(filePathAndName, 'w') as file:
+        file.write('# timestamp, x, y, z, qx, qy, qz, qw\n')
+        for idx in range(ts.shape[0]):
+            file.write('%f, %f, %f, %f, %f, %f, %f, %f\n' % (
+                    ts[idx] * 1000000000,                                                       
+                    point[idx, 0],                                                       
+                    point[idx, 1],                                                       
+                    point[idx, 2],                                                       
+                    rotation[idx, 1],                                                       
+                    rotation[idx, 2],                                                       
+                    rotation[idx, 3],                                                       
+                    rotation[idx, 0],                                                       
+                    ))
```

### Comparing `bimvee-1.0.9/bimvee/geometry.py` & `bimvee-1.0.9.dev0/bimvee/geometry.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,236 +1,236 @@
-# -*- coding: utf-8 -*-
-"""
-Copyright (C) 2020 Event-driven Perception for Robotics
-Author: Sim Bamford
-
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
-Low-level gemeotry functions, 
-for example, for manipulating poses, orientations, projections etc
-"""
-
-import numpy as np
-
-# local imports
-from .timestamps import sortDataTypeDictByTime
-
-# Can accept an existing matrix, which should be min 3x3; 
-#if it creates a matrix it makes it 4x4
-def quat2RotM(quat, M=None):
-    if M is None: 
-        M = np.zeros((4, 4))
-        M[3, 3] = 1
-    elif M.shape[0] == 3:
-        M[:, 3] = 0
-        M[3, :] = 0
-        M[3, 3] = 1
-    w = quat[0]
-    x = quat[1]
-    y = quat[2]
-    z = quat[3]
-    M[0, 0] = 1 - 2*y**2 - 2*z**2
-    M[0, 1] = 2*x*y - 2*z*w
-    M[0, 2] = 2*x*z + 2*y*w
-    M[1, 0] = 2*x*y + 2*z*w
-    M[1, 1] = 1 - 2*x**2 - 2*z**2
-    M[1, 2] = 2*y*z - 2*x*w
-    M[2, 0] = 2*x*z - 2*y*w
-    M[2, 1] = 2*y*z + 2*x*w
-    M[2, 2] = 1 - 2*x**2 - 2*y**2
-    return M
-
-# Spherical linear interpolation, adapted from https://en.wikipedia.org/wiki/Slerp
-DOT_THRESHOLD = 0.9995
-def slerp(q1, q2, time_relative):
-    dot = np.sum(q1 * q2)
-    if dot < 0.0:
-        q2 = -q2
-        dot = -dot
-    if dot > DOT_THRESHOLD:
-        result = q1 + time_relative * (q2 - q1)
-        return (result.T / np.linalg.norm(result)).T
-    theta_0 = np.arccos(dot)
-    sin_theta_0 = np.sin(theta_0)
-    theta = theta_0 * time_relative
-    sin_theta = np.sin(theta)
-    s0 = np.cos(theta) - dot * sin_theta / sin_theta_0
-    s1 = sin_theta / sin_theta_0
-    return (s0 * q1) + (s1 * q2)
-
-''' 
-expects pose dict in the form: {'ts': 1d np.array of np.float64 timestamps,
-                                'point': 2d array np.float64 of positions [x, y, z], 
-                                'rotation': 2d array np.float64 of quaternions [rw, rx, ry, rz]
-                                (i.e. 6dof with rotation as quaternion)}
-Two modes of operation:
-If time is not None, then returns the interpolated pose at that time -
-    returns (point, rotation) tuple, being np.array 1d x 3 and 4 respectively, np.float64,    which is interpolated pose;
-Else if maxPeriod is not None, then it returns the entire pose dict,
-    but with additional points necessary to ensure that time between samples 
-    never exceeds maxPeriod
-'''
-def pose6qInterp(poseDict, time=None, maxPeriod=None):
-    ts = poseDict['ts']
-    points = poseDict['point']
-    rotations = poseDict['rotation']
-    if time is not None:
-        idxPre = np.searchsorted(ts, time, side='right') - 1
-        timePre = ts[idxPre]
-        if timePre == time:
-            # In this edge-case of desired time == timestamp, there is no need 
-            # to interpolate 
-            return (points[idxPre, :], rotations[idxPre, :])
-        if idxPre < 0:
-            return (points[0, :], rotations[0, :])
-        if idxPre >= len(poseDict['ts']):
-            return (points[-1, :], rotations[-1, :])
-        timePost = ts[idxPre + 1]
-        rotPre = rotations[idxPre, :]
-        rotPost = rotations[idxPre + 1, :]
-        timeRel = (time - timePre) / (timePost - timePre)
-        rotOut = slerp(rotPre, rotPost, timeRel)
-        pointPre = points[idxPre, :] 
-        pointPost = points[idxPre + 1, :]
-        pointOut = pointPre * (1-timeRel) + pointPost * timeRel
-        return (pointOut, rotOut)
-    elif maxPeriod is not None:
-        firstTime = ts[0]
-        lastTime = ts[-1]
-        proposedAdditionalTimes = np.arange(firstTime, lastTime, maxPeriod)
-        prevIds = np.searchsorted(ts, proposedAdditionalTimes, side='right') - 1
-        distPre = proposedAdditionalTimes - ts[prevIds]
-        distPost = ts[prevIds + 1] - proposedAdditionalTimes
-        dist = distPre + distPost
-        keepAdditional = dist > maxPeriod
-        additionalTimes = proposedAdditionalTimes[keepAdditional]
-        additionalPoses = [pose6qInterp(poseDict, time=additionalTime) 
-                            for additionalTime in additionalTimes] 
-        additionalPoints, additionalRotations = zip(*additionalPoses)
-        ts = np.concatenate((ts, additionalTimes))
-        points = np.concatenate((points, np.array(additionalPoints)))
-        rotations = np.concatenate((rotations, np.array(additionalRotations)))
-        poseDict['ts'] = ts
-        poseDict['point'] = points
-        poseDict['rotation'] = rotations
-        poseDict = sortDataTypeDictByTime(poseDict)
-        return poseDict
-
-def quaternionProduct(q1, q2):
-    return np.array([ 
-    q1[0] * q2[0] - q1[1] * q2[1] - q1[2] * q2[2] - q1[3] * q2[3],
-    q1[0] * q2[1] + q1[1] * q2[0] + q1[2] * q2[3] - q1[3] * q2[2],
-    q1[0] * q2[2] - q1[1] * q2[3] + q1[2] * q2[0] + q1[3] * q2[1],
-    q1[0] * q2[3] + q1[1] * q2[2] - q1[2] * q2[1] + q1[3] * q2[0] ])
-    ''' alternative definition - less efficient
-    w1 = q1[0]
-    v1 = q1[1:4]
-    w2 = q2[0]
-    v2 = q2[1:4]
-    wOut = w1*w2 - np.dot(v1.T, v2)
-    vOut = w1*v2 + w2*v1 + np.cross(v1, v2)
-    qOut = np.zeros_like(q1)
-    qOut[0] = wOut
-    qOut[1:4] = vOut
-    return qOut
-    '''
-
-# Legacy name for Quaternion multiplication
-def combineTwoQuaternions(q1, q2):
-    return quaternionProduct(q1, q2)
-
-def quaternionConjugate(q):
-    return np.array([q[0], -q[1], -q[2], -q[3]])
-
-def quaternionInverse(q):
-    return quaternionConjugate(q) / np.sum(q ** 2)
-
-def angleBetweenTwoQuaternions(q1, q2):
-    # returns minimal angle in radians between two unit quaternions, following:
-    # https://www.researchgate.net/post/How_do_I_calculate_the_smallest_angle_between_two_quaternions    
-    qP = quaternionProduct(q1, quaternionInverse(q2))
-    normV = np.linalg.norm(qP[1:])
-    return 2 * np.arcsin(normV)
-
-'''
-following https://github.com/KieranWynn/pyquaternion/blob/master/pyquaternion/quaternion.py
-'''
-def axisAngle2Quat(axis, angle):
-    mag_sq = np.dot(axis, axis)
-    if mag_sq == 0.0:
-        raise ZeroDivisionError("Provided rotation axis has no length")
-    # Ensure axis is in unit vector form
-    if (abs(1.0 - mag_sq) > 1e-12):
-        axis = axis / np.sqrt(mag_sq)
-    theta = angle / 2.0
-    r = np.cos(theta)
-    i = axis * np.sin(theta)
-    quat = np.concatenate((np.ones((1)) * r, i))
-    quat = quat / np.linalg.norm(quat)
-    return quat
-
-'''
-following: https://answers.unity.com/questions/1266985/convert-rotation-vector-or-matrix-to-quaternion.html
-Receives a rotation vector and returns a quaternion
-'''
-def rotVToQuat(rotV):
-    theta = np.linalg.norm(rotV)
-    quat = axisAngle2Quat(rotV[:, 0], theta)
-    return quat
-    
-'''
-Expects 
-    - poseDict in bimvee form {'ts', 'point', 'rotation' as above}
-    - translation as np array of x,y,z
-    - rotation as a np array of w,x,y,z (quaternion)
-If either translation or rotation are passed, these are applied to all poses 
-in the poseDict.
-The rotations are defined wrt local axes, unlike the translations.
-Returns a copy of the poseDict, rotated
-'''    
-def transformPoses(poseDict, translation=None, rotation=None):
-    # Create a copy of the input array - use the same contents
-    outDict = {}
-    for key in poseDict.keys():
-        outDict[key] = poseDict[key]
-    if translation is not None:
-        outDict['point'] = poseDict['point'] + translation
-    if rotation is not None:
-        for idx in range(outDict['rotation'].shape[0]): # TODO: this could be matricised
-            outDict['rotation'][idx, :] = \
-                combineTwoQuaternions(outDict['rotation'][idx, :], rotation)
-    return outDict
-        
-
-# The following adapted from https://github.com/christophhagen/averaging-quaternions
-# Note that the signs of the output quaternion can be reversed, 
-# since q and -q describe the same orientation.
-# w is an optional weight array, which must have the same number of elements 
-# as the number of quaternions
-def averageOfQuaternions(allQ, w=None):
-    # Number of quaternions to average
-    M = allQ.shape[0]
-    A = np.zeros((4,4), dtype = np.float64)
-    if w is None:
-        w = np.ones(M,)
-    weightSum = 0
-    for i in range(0, M):
-        q = allQ[i, :]
-        # multiply q with its transposed version q' and add A
-        A = w[i] * np.outer(q,q) + A
-        weightSum += w[i]
-    # scale
-    A = (1.0 / M) * A
-    # compute eigenvalues and -vectors
-    eigenValues, eigenVectors = np.linalg.eig(A)
-    # Sort by largest eigenvalue
-    eigenVectors = eigenVectors[:,eigenValues.argsort()[::-1]]
-    # return the real part of the largest eigenvector (has only real part)
-    return eigenVectors[:,0]
+# -*- coding: utf-8 -*-
+"""
+Copyright (C) 2020 Event-driven Perception for Robotics
+Author: Sim Bamford
+
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
+Low-level gemeotry functions, 
+for example, for manipulating poses, orientations, projections etc
+"""
+
+import numpy as np
+
+# local imports
+from .timestamps import sortDataTypeDictByTime
+
+# Can accept an existing matrix, which should be min 3x3; 
+#if it creates a matrix it makes it 4x4
+def quat2RotM(quat, M=None):
+    if M is None: 
+        M = np.zeros((4, 4))
+        M[3, 3] = 1
+    elif M.shape[0] == 3:
+        M[:, 3] = 0
+        M[3, :] = 0
+        M[3, 3] = 1
+    w = quat[0]
+    x = quat[1]
+    y = quat[2]
+    z = quat[3]
+    M[0, 0] = 1 - 2*y**2 - 2*z**2
+    M[0, 1] = 2*x*y - 2*z*w
+    M[0, 2] = 2*x*z + 2*y*w
+    M[1, 0] = 2*x*y + 2*z*w
+    M[1, 1] = 1 - 2*x**2 - 2*z**2
+    M[1, 2] = 2*y*z - 2*x*w
+    M[2, 0] = 2*x*z - 2*y*w
+    M[2, 1] = 2*y*z + 2*x*w
+    M[2, 2] = 1 - 2*x**2 - 2*y**2
+    return M
+
+# Spherical linear interpolation, adapted from https://en.wikipedia.org/wiki/Slerp
+DOT_THRESHOLD = 0.9995
+def slerp(q1, q2, time_relative):
+    dot = np.sum(q1 * q2)
+    if dot < 0.0:
+        q2 = -q2
+        dot = -dot
+    if dot > DOT_THRESHOLD:
+        result = q1 + time_relative * (q2 - q1)
+        return (result.T / np.linalg.norm(result)).T
+    theta_0 = np.arccos(dot)
+    sin_theta_0 = np.sin(theta_0)
+    theta = theta_0 * time_relative
+    sin_theta = np.sin(theta)
+    s0 = np.cos(theta) - dot * sin_theta / sin_theta_0
+    s1 = sin_theta / sin_theta_0
+    return (s0 * q1) + (s1 * q2)
+
+''' 
+expects pose dict in the form: {'ts': 1d np.array of np.float64 timestamps,
+                                'point': 2d array np.float64 of positions [x, y, z], 
+                                'rotation': 2d array np.float64 of quaternions [rw, rx, ry, rz]
+                                (i.e. 6dof with rotation as quaternion)}
+Two modes of operation:
+If time is not None, then returns the interpolated pose at that time -
+    returns (point, rotation) tuple, being np.array 1d x 3 and 4 respectively, np.float64,    which is interpolated pose;
+Else if maxPeriod is not None, then it returns the entire pose dict,
+    but with additional points necessary to ensure that time between samples 
+    never exceeds maxPeriod
+'''
+def pose6qInterp(poseDict, time=None, maxPeriod=None):
+    ts = poseDict['ts']
+    points = poseDict['point']
+    rotations = poseDict['rotation']
+    if time is not None:
+        idxPre = np.searchsorted(ts, time, side='right') - 1
+        timePre = ts[idxPre]
+        if timePre == time:
+            # In this edge-case of desired time == timestamp, there is no need 
+            # to interpolate 
+            return (points[idxPre, :], rotations[idxPre, :])
+        if idxPre < 0:
+            return (points[0, :], rotations[0, :])
+        if idxPre >= len(poseDict['ts']):
+            return (points[-1, :], rotations[-1, :])
+        timePost = ts[idxPre + 1]
+        rotPre = rotations[idxPre, :]
+        rotPost = rotations[idxPre + 1, :]
+        timeRel = (time - timePre) / (timePost - timePre)
+        rotOut = slerp(rotPre, rotPost, timeRel)
+        pointPre = points[idxPre, :] 
+        pointPost = points[idxPre + 1, :]
+        pointOut = pointPre * (1-timeRel) + pointPost * timeRel
+        return (pointOut, rotOut)
+    elif maxPeriod is not None:
+        firstTime = ts[0]
+        lastTime = ts[-1]
+        proposedAdditionalTimes = np.arange(firstTime, lastTime, maxPeriod)
+        prevIds = np.searchsorted(ts, proposedAdditionalTimes, side='right') - 1
+        distPre = proposedAdditionalTimes - ts[prevIds]
+        distPost = ts[prevIds + 1] - proposedAdditionalTimes
+        dist = distPre + distPost
+        keepAdditional = dist > maxPeriod
+        additionalTimes = proposedAdditionalTimes[keepAdditional]
+        additionalPoses = [pose6qInterp(poseDict, time=additionalTime) 
+                            for additionalTime in additionalTimes] 
+        additionalPoints, additionalRotations = zip(*additionalPoses)
+        ts = np.concatenate((ts, additionalTimes))
+        points = np.concatenate((points, np.array(additionalPoints)))
+        rotations = np.concatenate((rotations, np.array(additionalRotations)))
+        poseDict['ts'] = ts
+        poseDict['point'] = points
+        poseDict['rotation'] = rotations
+        poseDict = sortDataTypeDictByTime(poseDict)
+        return poseDict
+
+def quaternionProduct(q1, q2):
+    return np.array([ 
+    q1[0] * q2[0] - q1[1] * q2[1] - q1[2] * q2[2] - q1[3] * q2[3],
+    q1[0] * q2[1] + q1[1] * q2[0] + q1[2] * q2[3] - q1[3] * q2[2],
+    q1[0] * q2[2] - q1[1] * q2[3] + q1[2] * q2[0] + q1[3] * q2[1],
+    q1[0] * q2[3] + q1[1] * q2[2] - q1[2] * q2[1] + q1[3] * q2[0] ])
+    ''' alternative definition - less efficient
+    w1 = q1[0]
+    v1 = q1[1:4]
+    w2 = q2[0]
+    v2 = q2[1:4]
+    wOut = w1*w2 - np.dot(v1.T, v2)
+    vOut = w1*v2 + w2*v1 + np.cross(v1, v2)
+    qOut = np.zeros_like(q1)
+    qOut[0] = wOut
+    qOut[1:4] = vOut
+    return qOut
+    '''
+
+# Legacy name for Quaternion multiplication
+def combineTwoQuaternions(q1, q2):
+    return quaternionProduct(q1, q2)
+
+def quaternionConjugate(q):
+    return np.array([q[0], -q[1], -q[2], -q[3]])
+
+def quaternionInverse(q):
+    return quaternionConjugate(q) / np.sum(q ** 2)
+
+def angleBetweenTwoQuaternions(q1, q2):
+    # returns minimal angle in radians between two unit quaternions, following:
+    # https://www.researchgate.net/post/How_do_I_calculate_the_smallest_angle_between_two_quaternions    
+    qP = quaternionProduct(q1, quaternionInverse(q2))
+    normV = np.linalg.norm(qP[1:])
+    return 2 * np.arcsin(normV)
+
+'''
+following https://github.com/KieranWynn/pyquaternion/blob/master/pyquaternion/quaternion.py
+'''
+def axisAngle2Quat(axis, angle):
+    mag_sq = np.dot(axis, axis)
+    if mag_sq == 0.0:
+        raise ZeroDivisionError("Provided rotation axis has no length")
+    # Ensure axis is in unit vector form
+    if (abs(1.0 - mag_sq) > 1e-12):
+        axis = axis / np.sqrt(mag_sq)
+    theta = angle / 2.0
+    r = np.cos(theta)
+    i = axis * np.sin(theta)
+    quat = np.concatenate((np.ones((1)) * r, i))
+    quat = quat / np.linalg.norm(quat)
+    return quat
+
+'''
+following: https://answers.unity.com/questions/1266985/convert-rotation-vector-or-matrix-to-quaternion.html
+Receives a rotation vector and returns a quaternion
+'''
+def rotVToQuat(rotV):
+    theta = np.linalg.norm(rotV)
+    quat = axisAngle2Quat(rotV[:, 0], theta)
+    return quat
+    
+'''
+Expects 
+    - poseDict in bimvee form {'ts', 'point', 'rotation' as above}
+    - translation as np array of x,y,z
+    - rotation as a np array of w,x,y,z (quaternion)
+If either translation or rotation are passed, these are applied to all poses 
+in the poseDict.
+The rotations are defined wrt local axes, unlike the translations.
+Returns a copy of the poseDict, rotated
+'''    
+def transformPoses(poseDict, translation=None, rotation=None):
+    # Create a copy of the input array - use the same contents
+    outDict = {}
+    for key in poseDict.keys():
+        outDict[key] = poseDict[key]
+    if translation is not None:
+        outDict['point'] = poseDict['point'] + translation
+    if rotation is not None:
+        for idx in range(outDict['rotation'].shape[0]): # TODO: this could be matricised
+            outDict['rotation'][idx, :] = \
+                combineTwoQuaternions(outDict['rotation'][idx, :], rotation)
+    return outDict
+        
+
+# The following adapted from https://github.com/christophhagen/averaging-quaternions
+# Note that the signs of the output quaternion can be reversed, 
+# since q and -q describe the same orientation.
+# w is an optional weight array, which must have the same number of elements 
+# as the number of quaternions
+def averageOfQuaternions(allQ, w=None):
+    # Number of quaternions to average
+    M = allQ.shape[0]
+    A = np.zeros((4,4), dtype = np.float64)
+    if w is None:
+        w = np.ones(M,)
+    weightSum = 0
+    for i in range(0, M):
+        q = allQ[i, :]
+        # multiply q with its transposed version q' and add A
+        A = w[i] * np.outer(q,q) + A
+        weightSum += w[i]
+    # scale
+    A = (1.0 / M) * A
+    # compute eigenvalues and -vectors
+    eigenValues, eigenVectors = np.linalg.eig(A)
+    # Sort by largest eigenvalue
+    eigenVectors = eigenVectors[:,eigenValues.argsort()[::-1]]
+    # return the real part of the largest eigenvector (has only real part)
+    return eigenVectors[:,0]
```

### Comparing `bimvee-1.0.9/bimvee/importAe.py` & `bimvee-1.0.9.dev0/bimvee/importAe.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,130 +1,164 @@
-# -*- coding: utf-8 -*-
-"""
-Copyright (C) 2019 Event-driven Perception for Robotics
-Authors: Sim Bamford
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
-importAe is a function for importing timestamped address-event data, given a path 
-(defaulting to the current directory, intended for the yarp format) or a file.  
-If the file format is not stated, there is an attempt to determine this from the file.
-Then a sub-function is called, specialised for importing the data contained 
-into the workspace. Depending on the format, additional data may also be imported,
-including frame data, imu samples, skin data, 2d or 3d coords etc etc.
-  
-The output is a dictionary containing:
-    - info
-    - data
-The exact contents varies according to the file type import but in general:
-    info: this is a dict which starts life as the kwargs passed in, and is 
-    augmented and modified by the actual contents of the file. It may include 
-    any informational fields in file headers. Minimally, it will contain:
-        - filePathAndName
-        - fileFormat
-    data: this is a list of dicts, one for each sensor or "channel" which has 
-    been imported. Bear in mind that sub-functions may optionally split or join 
-    channels. Within each dict, there is a field for each type of data contained.
-    A file for example may contain data from a several sensors, but a single sensor 
-    may produce polarity events ("pol"), aps samples ("aps"), imu samples etc.
-    Within each of these fields, there is a dict, generally containing fields for 
-    each data column, so in the case of pol events, there are 4-5 fields:
-        - ts
-        - x
-        - y 
-        - pol
-        - optionally ch (channel)
-        each containing a numpy array of the appropriate type for the data 
-        contained, where all these arrays will be of the same length.
-
-Aim is to support:
-
-YARP .log - ATIS Gen1 - 24 bit - includes, IMU, Vicon, (also SKIN?)
-rpg_dvs_ros - DVS/DAVIS
-Maybe others? 
-jAER / cAER .aedat (v1/2/3) DVS / DAVIS / Cochlea?
-Samsung Gen3 VGA?
-Celex ...???
-"""
-
-#%%
-
-import os
-
-# local imports
-from .importIitNumpy import importIitNumpy
-from .importIitYarp import importIitYarp
-from .importRpgDvsRos import importRpgDvsRos
-from .importSecDvs import importSecDvs
-from .importAer2 import importAer2
-from .importFrames import importFrames
-
-def getOrInsertDefault(inDict, arg, default):
-    # get an arg from a dict.
-    # If the the dict doesn't contain the arg, return the default, 
-    # and also insert the default into the dict
-    value = inDict.get(arg, default)
-    if value == default:
-        inDict[arg] = default
-    return value
-
-
-def importAe(**kwargs):
-    print(kwargs)
-    filePathOrName = getOrInsertDefault(kwargs, 'filePathOrName', '.')
-    print(kwargs)
-    if not os.path.exists(filePathOrName):
-        raise FileNotFoundError("File or folder not found.")
-    fileFormat = kwargs.get('fileFormat', '').lower()
-    if not fileFormat:
-        # Try to determine the file format
-        if os.path.isdir(filePathOrName):
-            # It's a path - assume YARP log directory
-            # Note that it could also be a folder full of frames
-            kwargs['fileFormat'] = 'iityarp'
-        else:
-            ext = os.path.splitext(filePathOrName)[1]
-            if ext == '.aedat' or ext == '.dat':
-                # Assume it's aedat
-                kwargs['fileFormat'] = 'aedat'
-            elif ext == '.bag':
-                # Assume it's rpg_dvs_ros
-                kwargs['fileFormat'] = 'rosbag'
-            elif ext == '.bin':
-                # Assume it's a secdvs file
-                kwargs['fileFormat'] = 'secdvs'
-            elif ext == '.npy':
-                kwargs['fileFormat'] = 'iitnpy'
-            elif ext == '.aer2':
-                kwargs['fileFormat'] = 'aer2'
-            # etc ...
-            else:
-                raise Exception("The file format cannot be determined.")
-    # Let the fileformat parameter dictate the file or folder format
-    fileFormat = kwargs.get('fileFormat').lower()
-    if fileFormat in ['iityarp', 'yarp', 'iit', 'log', 'yarplog']: 
-        importedData = importIitYarp(**kwargs)
-    elif fileFormat in ['rpgdvsros', 'rosbag', 'rpg', 'ros', 'bag', 'rpgdvs']:
-        if 'template' not in kwargs or kwargs['template'] is None:
-            print('Template for ROS bag not defined - all data-type dicts will be imported into separate channels')
-        importedData = importRpgDvsRos(**kwargs)
-    elif fileFormat in ['iitnpy', 'npy', 'numpy']:
-        importedData = importIitNumpy(**kwargs)
-    #elif fileFormat in ['iniaedat', 'aedat', 'dat', 'jaer', 'caer', 'ini', 'inivation', 'inilabs']:
-    #    importedData = importIniAedat(kwargs)
-    elif fileFormat in ['secdvs', 'bin', 'samsung', 'sec', 'gen3']:
-        importedData = importSecDvs(**kwargs)
-    elif fileFormat in ['aer2']:
-        importedData = importAer2(**kwargs)
-    elif fileFormat in ['frames', 'png', 'pngfolder', 'imagefolder']:
-        importedData = importFrames(**kwargs)
-    else:
-        raise Exception("fileFormat: " + str(fileFormat) + " not supported.")
-    #celex
+# -*- coding: utf-8 -*-
+"""
+Copyright (C) 2019 Event-driven Perception for Robotics
+Authors: Sim Bamford
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
+importAe is a function for importing timestamped address-event data, given a path 
+(defaulting to the current directory, intended for the yarp format) or a file.  
+If the file format is not stated, there is an attempt to determine this from the file.
+Then a sub-function is called, specialised for importing the data contained 
+into the workspace. Depending on the format, additional data may also be imported,
+including frame data, imu samples, skin data, 2d or 3d coords etc etc.
+  
+The output is a dictionary containing:
+    - info
+    - data
+The exact contents varies according to the file type import but in general:
+    info: this is a dict which starts life as the kwargs passed in, and is 
+    augmented and modified by the actual contents of the file. It may include 
+    any informational fields in file headers. Minimally, it will contain:
+        - filePathAndName
+        - fileFormat
+    data: this is a list of dicts, one for each sensor or "channel" which has 
+    been imported. Bear in mind that sub-functions may optionally split or join 
+    channels. Within each dict, there is a field for each type of data contained.
+    A file for example may contain data from a several sensors, but a single sensor 
+    may produce polarity events ("pol"), aps samples ("aps"), imu samples etc.
+    Within each of these fields, there is a dict, generally containing fields for 
+    each data column, so in the case of pol events, there are 4-5 fields:
+        - ts
+        - x
+        - y 
+        - pol
+        - optionally ch (channel)
+        each containing a numpy array of the appropriate type for the data 
+        contained, where all these arrays will be of the same length.
+
+Aim is to support:
+
+YARP .log - ATIS Gen1 - 24 bit - includes, IMU, Vicon, (also SKIN?)
+rpg_dvs_ros - DVS/DAVIS
+Maybe others? 
+jAER / cAER .aedat (v1/2/3) DVS / DAVIS / Cochlea?
+Samsung Gen3 VGA?
+Celex ...???
+"""
+
+#%%
+
+import os
+
+# local imports
+from .importIitNumpy import importIitNumpy
+from .importIitYarp import importIitYarp
+from .importRpgDvsRos import importRpgDvsRos
+from .importSecDvs import importSecDvs
+from .importAer2 import importAer2
+from .importFrames import importFrames
+from .timestamps import rezeroTimestampsForImportedDicts
+from .importHdf5 import importHdf5
+from .importProph import importProph
+
+def getOrInsertDefault(inDict, arg, default):
+    # get an arg from a dict.
+    # If the the dict doesn't contain the arg, return the default, 
+    # and also insert the default into the dict
+    value = inDict.get(arg, default)
+    if value == default:
+        inDict[arg] = default
+    return value
+
+
+def importAe(**kwargs):
+    print(kwargs)
+    filePathOrName = getOrInsertDefault(kwargs, 'filePathOrName', '.')
+    print(kwargs)
+    if not os.path.exists(filePathOrName):
+        raise FileNotFoundError("File or folder not found.")
+    fileFormat = kwargs.get('fileFormat', '').lower()
+    if not fileFormat:
+        # Try to determine the file format
+        if os.path.isdir(filePathOrName):
+            # It's a path - it could contain yarp .log or frames
+            listDir = os.listdir(filePathOrName)
+            fileTypes = [subName.split(".")[-1] for subName in listDir]
+            mostCommonFileType = max(set(fileTypes), key=fileTypes.count)
+            if mostCommonFileType == 'log':
+                kwargs['fileFormat'] = 'iityarp'
+            elif mostCommonFileType == 'png':
+                kwargs['fileFormat'] = 'frames'
+            else:
+                # recurse into this folder
+                resultsList = []
+                for subName in listDir:
+                    kwargs['filePathOrName'] = os.path.join(filePathOrName, subName)
+                    try:
+                        result = importAe(**kwargs)
+                    except ValueError:
+                        continue
+                    if isinstance(result, list):
+                        resultsList = resultsList + result
+                    else:
+                        resultsList.append(result)
+                if len(resultsList) > 1 and \
+                    kwargs.get('zeroTime', kwargs.get('zeroTimestamps', True)):
+                        # Optional: start the timestamps at zero for the first event
+                        # This is done collectively for all the concurrent imports
+                        rezeroTimestampsForImportedDicts(resultsList)
+                elif len(resultsList) == 1:
+                    resultsList = resultsList[0]
+ 
+                return resultsList
+        else:
+            # Guess the file format based on file extension
+            ext = os.path.splitext(filePathOrName)[1]
+            if ext == '.dat' or ext == '.raw':
+                kwargs['fileFormat'] = 'dat'
+            elif ext == '.bag':
+                kwargs['fileFormat'] = 'rosbag'
+            elif ext == '.bin':
+                kwargs['fileFormat'] = 'secdvs'
+            elif ext == '.npy':
+                kwargs['fileFormat'] = 'iitnpy'
+            elif ext == '.aer2':
+                kwargs['fileFormat'] = 'aer2'
+            elif ext == '.hdf5':
+                kwargs['fileFormat'] = 'hdf5'
+            elif ext == '.log':
+                kwargs['fileFormat'] = 'iit'
+            # etc ...
+            else:
+                raise ValueError("The file format cannot be determined.")
+    # Let the fileformat parameter dictate the file or folder format
+    fileFormat = kwargs.get('fileFormat').lower()
+    if fileFormat in ['iityarp', 'yarp', 'iit', 'log', 'yarplog']:
+        if not os.path.isdir(kwargs['filePathOrName']):
+            kwargs['filePathOrName'] = os.path.dirname(kwargs['filePathOrName'])
+        importedData = importIitYarp(**kwargs)
+    elif fileFormat in ['rpgdvsros', 'rosbag', 'rpg', 'ros', 'bag', 'rpgdvs']:
+        importedData = importRpgDvsRos(**kwargs)
+    elif fileFormat in ['iitnpy', 'npy', 'numpy']:
+        importedData = importIitNumpy(**kwargs)
+    elif fileFormat in ['dat', 'raw']:
+        importedData = importProph(**kwargs)
+    elif fileFormat in ['secdvs', 'bin', 'samsung', 'sec', 'gen3']:
+        importedData = importSecDvs(**kwargs)
+    elif fileFormat in ['aer2']:
+        importedData = importAer2(**kwargs)
+    elif fileFormat in ['frame', 'frames', 'png', 'pngfolder', 'imagefolder']:
+        importedData = importFrames(**kwargs)
+    elif fileFormat in ['hdf5', 'bimveehdf5']:
+        importedData = importHdf5(**kwargs)
+    else:
+        raise Exception("fileFormat: " + str(fileFormat) + " not supported.")
+    #celex
     return importedData
```

### Comparing `bimvee-1.0.9/bimvee/importAer2.py` & `bimvee-1.0.9.dev0/bimvee/importAer2.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-# -*- coding: utf-8 -*-
-"""
-Copyright (C) 2020 Event-driven Perception for Robotics
-Authors: Sim Bamford
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
-An example of 'aer2' format in the wild is:
-    
-https://github.com/VLOGroup/dvs-reconstruction/blob/master/data/sample_data.tar.bz2
-
-It's a text file, no headers, where each event encodes one line, in the  format:
-    
-ts x y pol
-
-importAer2 opens such a file (pass with filePathOrName parameter) 
-and returns a dict in this format:
-{'info': {},
- 'data': {
-         ch0: {
-               dvs: {
-                     'ts': np.array of np.float64 in seconds 
-                     'x': np.array of np.uint16 in pixels
-                     'y': np.array of np.uint16 in pixels
-                     'pol': np.array of np.bool -- 1 = ON event 
-                    }}}}
-"""
-
-import numpy as np
-from tqdm import tqdm 
-
-# Local imports
-from .timestamps import zeroTimestampsForADataType
-
-def inferDim(array):
-    dimStops = np.array([32, 64, 128, 180, 240, 256, 260, 304, 320, 346, 480, 640, 720, 1080, 1280, 1920], dtype=np.uint16)
-    idx = np.searchsorted(dimStops, np.max(array))
-    try:
-        return dimStops[idx]
-    except IndexError:
-        return np.max(array) + 1
-    
-def importAer2(**kwargs):
-    filePathOrName = kwargs['filePathOrName']
-    print('Attempting to import ' + filePathOrName + ' as aer2')
-    sizeOfArray = 1024
-    ts = np.zeros((sizeOfArray), dtype=np.float64)
-    x = np.zeros((sizeOfArray), dtype=np.uint16)
-    y = np.zeros((sizeOfArray), dtype=np.uint16)
-    pol = np.zeros((sizeOfArray), dtype=np.bool)
-
-    with open(filePathOrName, 'r') as file:
-        for idx, line in enumerate(tqdm(file)):
-            if idx == sizeOfArray:
-                ts = np.concatenate((ts, np.zeros((sizeOfArray), dtype=np.float64)))
-                x = np.concatenate((x, np.zeros((sizeOfArray), dtype=np.uint16)))
-                y = np.concatenate((y, np.zeros((sizeOfArray), dtype=np.uint16)))
-                pol = np.concatenate((pol, np.zeros((sizeOfArray), dtype=np.bool)))
-                sizeOfArray *= 2
-            lineSplit = line.split()
-            ts[idx] = float(lineSplit[0])
-            x[idx] = int(lineSplit[1])
-            y[idx] = int(lineSplit[2])
-            pol[idx] = int(lineSplit[3])
-        numEvents = idx + 1
-    dvsDict = {'ts': ts[:numEvents] / 1000000,
-           'x': x[:numEvents],
-           'y': y[:numEvents],
-           'pol': pol[:numEvents],
-           'dimX': inferDim(x),
-           'dimY': inferDim(y)
-           }
-
-    if kwargs.get('zeroTime', kwargs.get('zeroTimestamps', True)): 
-        zeroTimestampsForADataType(dvsDict)
-    outDict = {
-    'info': {'filePathOrName':filePathOrName,
-        'fileFormat': 'aer2'},
-    'data': {
-        'ch0': {
-            'dvs': dvsDict
-            }
-        }
-    }
-    print('Done.')
-    return outDict
+# -*- coding: utf-8 -*-
+"""
+Copyright (C) 2020 Event-driven Perception for Robotics
+Authors: Sim Bamford
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
+An example of 'aer2' format in the wild is:
+    
+https://github.com/VLOGroup/dvs-reconstruction/blob/master/data/sample_data.tar.bz2
+
+It's a text file, no headers, where each event encodes one line, in the  format:
+    
+ts x y pol
+
+importAer2 opens such a file (pass with filePathOrName parameter) 
+and returns a dict in this format:
+{'info': {},
+ 'data': {
+         ch0: {
+               dvs: {
+                     'ts': np.array of np.float64 in seconds 
+                     'x': np.array of np.uint16 in pixels
+                     'y': np.array of np.uint16 in pixels
+                     'pol': np.array of np.bool -- 1 = ON event 
+                    }}}}
+"""
+
+import numpy as np
+from tqdm import tqdm 
+
+# Local imports
+from .timestamps import zeroTimestampsForADataType
+
+def inferDim(array):
+    dimStops = np.array([32, 64, 128, 180, 240, 256, 260, 304, 320, 346, 480, 640, 720, 1080, 1280, 1920], dtype=np.uint16)
+    idx = np.searchsorted(dimStops, np.max(array))
+    try:
+        return dimStops[idx]
+    except IndexError:
+        return np.max(array) + 1
+    
+def importAer2(**kwargs):
+    filePathOrName = kwargs['filePathOrName']
+    print('Attempting to import ' + filePathOrName + ' as aer2')
+    sizeOfArray = 1024
+    ts = np.zeros((sizeOfArray), dtype=np.float64)
+    x = np.zeros((sizeOfArray), dtype=np.uint16)
+    y = np.zeros((sizeOfArray), dtype=np.uint16)
+    pol = np.zeros((sizeOfArray), dtype=np.bool)
+
+    with open(filePathOrName, 'r') as file:
+        for idx, line in enumerate(tqdm(file)):
+            if idx == sizeOfArray:
+                ts = np.concatenate((ts, np.zeros((sizeOfArray), dtype=np.float64)))
+                x = np.concatenate((x, np.zeros((sizeOfArray), dtype=np.uint16)))
+                y = np.concatenate((y, np.zeros((sizeOfArray), dtype=np.uint16)))
+                pol = np.concatenate((pol, np.zeros((sizeOfArray), dtype=np.bool)))
+                sizeOfArray *= 2
+            lineSplit = line.split()
+            ts[idx] = float(lineSplit[0])
+            x[idx] = int(lineSplit[1])
+            y[idx] = int(lineSplit[2])
+            pol[idx] = int(lineSplit[3])
+        numEvents = idx + 1
+    dvsDict = {'ts': ts[:numEvents] / 1000000,
+           'x': x[:numEvents],
+           'y': y[:numEvents],
+           'pol': pol[:numEvents],
+           'dimX': inferDim(x),
+           'dimY': inferDim(y)
+           }
+
+    if kwargs.get('zeroTime', kwargs.get('zeroTimestamps', True)): 
+        zeroTimestampsForADataType(dvsDict)
+    outDict = {
+    'info': {'filePathOrName':filePathOrName,
+        'fileFormat': 'aer2'},
+    'data': {
+        'ch0': {
+            'dvs': dvsDict
+            }
+        }
+    }
+    print('Done.')
+    return outDict
```

### Comparing `bimvee-1.0.9/bimvee/importExportBatches.py` & `bimvee-1.0.9.dev0/bimvee/importExportBatches.py`

 * *Files identical despite different names*

### Comparing `bimvee-1.0.9/bimvee/importFrames.py` & `bimvee-1.0.9.dev0/bimvee/importFrames.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,85 @@
-# -*- coding: utf-8 -*-
-"""
-Copyright (C) 2020 Event-driven Perception for Robotics
-Authors: Sim Bamford
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
-
-importFrames imports a folder full of (timestamped) frames saved as image files.  
-It might make sense to generalise this using e.g. https://github.com/soft-matter/pims
-but on day one this imports frames in the format exported by:
-https://github.com/uzh-rpg/rpg_e2vid
-i.e. a folder full of png, also containing a 'timestamps.txt' file, with a timestamp
-in seconds written on each line. 
-
-Returns a dict:
-{'info': {'filePathOrName': str},
- 'data': {
-     channel0: {
-         frame: {
-             "ts": numpy array of float - seconds
-             "frames": a list of numpy arrays where dim 0 = y (increasing downwards)
-
-"""
-
-#%%
-
-import re
-import numpy as np
-import os
-from tqdm import tqdm
-import struct
-import imageio
-
-# local imports
-from .timestamps import zeroTimestampsForAChannel, rezeroTimestampsForAnImportedDict
-
-def getOrInsertDefault(inDict, arg, default):
-    # get an arg from a dict.
-    # If the the dict doesn't contain the arg, return the default, 
-    # and also insert the default into the dict
-    value = inDict.get(arg, default)
-    if value == default:
-        inDict[arg] = default
-    return value
-
-def importFrames(**kwargs):
-    '''
-    '''
-    path = getOrInsertDefault(kwargs, 'filePathOrName', '.')
-    print('importFrames trying path: ' + path)
-    if not os.path.exists(path):
-        raise FileNotFoundError("path not found.")
-    if not os.path.isdir(path):
-        raise FileNotFoundError("path is not a directory.")
-    files = sorted(os.listdir(path))
-    # TODO: trusting the os to sort the files may not work
-    frames = []
-    for file in tqdm(files):
-        filePathAndName = os.path.join(path, file) 
-        if file == 'timestamps.txt': # todo: is there a more general form?
-            ts = np.loadtxt(filePathAndName)
-        elif os.path.isfile(filePathAndName):
-            frames.append(imageio.imread(filePathAndName))
-    channelDict = {'frame': 
-                       {'ts': ts,
-                        'frames': frames}}
-    if getOrInsertDefault(kwargs, 'zeroTimestamps', True):
-        zeroTimestampsForAChannel(channelDict)
-    importedDict = {
-        'info': kwargs,
-        'data': {'ch0': channelDict}
-        }
-    importedDict['info']['fileFormat'] = 'imagefolder'
-    if kwargs.get('zeroTimestamps'):
-        rezeroTimestampsForAnImportedDict(importedDict)
-    return importedDict
-        
-    
+# -*- coding: utf-8 -*-
+"""
+Copyright (C) 2020 Event-driven Perception for Robotics
+Authors: Sim Bamford
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
+
+importFrames imports a folder full of (timestamped) frames saved as image files.  
+It might make sense to generalise this using e.g. https://github.com/soft-matter/pims
+but on day one this imports frames in the format exported by:
+https://github.com/uzh-rpg/rpg_e2vid
+i.e. a folder full of png, also containing a 'timestamps.txt' file, with a timestamp
+in seconds written on each line. 
+
+Returns a dict:
+{'info': {'filePathOrName': str},
+ 'data': {
+     channel0: {
+         frame: {
+             "ts": numpy array of float - seconds
+             "frames": a list of numpy arrays where dim 0 = y (increasing downwards)
+
+"""
+
+#%%
+
+import re
+import numpy as np
+import os
+from tqdm import tqdm
+import struct
+import imageio
+
+# local imports
+from .timestamps import zeroTimestampsForAChannel, rezeroTimestampsForAnImportedDict
+
+def getOrInsertDefault(inDict, arg, default):
+    # get an arg from a dict.
+    # If the the dict doesn't contain the arg, return the default, 
+    # and also insert the default into the dict
+    value = inDict.get(arg, default)
+    if value == default:
+        inDict[arg] = default
+    return value
+
+def importFrames(**kwargs):
+    path = getOrInsertDefault(kwargs, 'filePathOrName', '.')
+    print('importFrames trying path: ' + path)
+    if not os.path.exists(path):
+        raise FileNotFoundError("path not found.")
+    if not os.path.isdir(path):
+        raise FileNotFoundError("path is not a directory.")
+    files = sorted(os.listdir(path))
+    # TODO: trusting the os to sort the files may not work
+    frames = []
+    for file in tqdm(files):
+        filePathAndName = os.path.join(path, file) 
+        if file == 'timestamps.txt': # todo: is there a more general form?
+            ts = np.loadtxt(filePathAndName)
+        elif os.path.isfile(filePathAndName):
+            frames.append(imageio.imread(filePathAndName))
+    channelDict = {'frame': 
+                       {'ts': ts,
+                        'frames': frames}}
+    if kwargs.get('zeroTime', kwargs.get('zeroTimestamps', True)):
+        zeroTimestampsForAChannel(channelDict)
+    importedDict = {
+        'info': kwargs,
+        'data': {'ch0': channelDict}
+        }
+    importedDict['info']['fileFormat'] = 'imagefolder'
+    if kwargs.get('zeroTime', kwargs.get('zeroTimestamps', True)):
+        rezeroTimestampsForAnImportedDict(importedDict)
+    return importedDict
+        
+
```

### Comparing `bimvee-1.0.9/bimvee/importHdf5.py` & `bimvee-1.0.9.dev0/bimvee/exportHdf5.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,36 @@
-# -*- coding: utf-8 -*-
-"""
-Copyright (C) 2020 Event-driven Perception for Robotics
-Authors: Sim Bamford
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
-
-Using hickle to add hierarchical lists and dicts to hdf5 automatically
-https://github.com/telegraphic/hickle
-In fact, thess are just thin wrappers around hickle.dump/load, 
-to offer a similar export function to other export calls.
-pack/unpackWorkspaceVars are facilities that allows extra random data WIP 
-to get bundled together. All files are included in both the import and export script for convenience. 
-TODO: This script to import and pass through functions from exportHdf5
-"""
-#%%
-
-# local imports
-from .exportHdf5 import *
+# -*- coding: utf-8 -*-
+"""
+Copyright (C) 2020 Event-driven Perception for Robotics
+Authors: Sim Bamford
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
+
+Using hickle to add hierarchical lists and dicts to hdf5 automatically
+https://github.com/telegraphic/hickle
+In fact, these are just thin wrappers around hickle.dump/load, 
+to offer a similar export function to other export calls.
+"""
+
+#%%
+
+import hickle
+import os
+
+def exportHdf5(data, exportFilePathAndName='./temp.hdf5', **kwargs):
+    if exportFilePathAndName[-5:] != '.hdf5':
+        exportFilePathAndName = exportFilePathAndName + '.hdf5'
+    print('exportHdf5 called, targeting file path and name' + exportFilePathAndName)
+    absPath = os.path.dirname(os.path.abspath(exportFilePathAndName))
+    if not os.path.exists(absPath):
+        os.mkdir(absPath)
+    hickle.dump(data, exportFilePathAndName)
+
+
```

### Comparing `bimvee-1.0.9/bimvee/importIitNumpy.py` & `bimvee-1.0.9.dev0/bimvee/importIitNumpy.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,155 +1,155 @@
-# -*- coding: utf-8 -*-
-"""
-Copyright (C) 2019 Event-driven Perception for Robotics
-Authors: Massimiliano Iacono
-This program is free software: you can redistribute it and/or modify it under
-the terms of the GNU General Public License as published by the Free Software
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
-importIitNumpy imports timestamped address-event data, given a path to a .npy file.
-It serves the needs of a specific data format developed at IIT involving events, 
-frames and bounding boxes.
-If available at the predetermined locations, relative to the npy file additional 
-data may also be imported, such as frames and bounding boxes used to label the 
-data. At the moment frames and boxes are stored in a data.log file using the 
-YARP format (see importIitYarp as an example). TODO: generalize data structure
-
-The output is a dictionary containing:
-    - info
-    - data
-The exact contents varies according to the file type import but in general:
-    info: this is a dict which starts life as the kwargs passed in, and is
-    augmented and modified by the actual contents of the file. It may include
-    any informational fields in file headers. Minimally, it will contain:
-        - filePathAndName
-        - fileFormat
-    data: this is a list of dicts, one for each sensor or "channel" which has
-    been imported. Bear in mind that sub-functions may optionally split or join
-    channels. Within each dict, there is a field for each type of data contained.
-    A file for example may contain data from a several sensors, but a single sensor
-    may produce polarity events ("pol"), aps samples ("aps"), imu samples etc.
-    Within each of these fields, there is a dict, generally containing fields for
-    each data column, so in the case of pol events, there are 4-5 fields:
-        - ts
-        - x
-        - y
-        - pol
-        - optionally ch (channel)
-        each containing a numpy array of the appropriate type for the data
-        contained, where all these arrays will be of the same length.
-    Similarly bounding boxes are saved in the channel in a separate dictionary containing the following fields:
-        - ts
-        - minY
-        - minX
-        - maxY
-        - maxX
-"""
-
-import numpy as np
-import os
-
-def importIitNumpy(filePathOrName, **kwargs):
-    outDict = {
-        'info': kwargs,
-        'data': {}
-    }
-    outDict['info']['filePathOrName'] = filePathOrName
-
-    # Importing events
-    events = np.load(filePathOrName)
-
-    outDict['data']['labelledEvents'] = {}
-    outDict['data']['labelledEvents']['dvs'] = {}
-
-    tsOffset = events[0, 0]
-    ts_to_sync = [events[:, 0]]
-
-    outDict['data']['labelledEvents']['dvs']['ts'] = events[:, 0]
-    outDict['data']['labelledEvents']['dvs']['x'] = events[:, 1].astype(np.int)
-    outDict['data']['labelledEvents']['dvs']['y'] = events[:, 2].astype(np.int)
-    outDict['data']['labelledEvents']['dvs']['pol'] = events[:, 3].astype(np.bool)
-    outDict['data']['labelledEvents']['dvs']['dimX'] = 304
-    outDict['data']['labelledEvents']['dvs']['dimY'] = 240
-
-
-    # Importing bounding boxes for events
-    gt_filename = os.path.join(os.path.dirname(filePathOrName), 'boxes.npy')
-
-    if os.path.exists(gt_filename):
-        b_boxes = np.load(gt_filename)
-        outDict['data']['labelledEvents']['boundingBoxes'] = {}
-
-        tsOffset = min(tsOffset, b_boxes[0, 0])
-        ts_to_sync.append(b_boxes[:, 0])
-        outDict['data']['labelledEvents']['boundingBoxes']['ts'] = b_boxes[:, 0]
-        outDict['data']['labelledEvents']['boundingBoxes']['minY'] = b_boxes[:, 1]
-        outDict['data']['labelledEvents']['boundingBoxes']['minX'] = b_boxes[:, 2]
-        outDict['data']['labelledEvents']['boundingBoxes']['maxY'] = b_boxes[:, 3]
-        outDict['data']['labelledEvents']['boundingBoxes']['maxX'] = b_boxes[:, 4]
-        outDict['data']['labelledEvents']['boundingBoxes']['label'] = b_boxes[:, 5]
-
-    # Importing frames
-    framesPath = (os.path.join(os.path.dirname(filePathOrName), '../processed/frames_left')) # TODO make path argument
-    if os.path.exists(framesPath):
-        import re
-        from imageio import imread
-        pattern = re.compile('\d+ (\d+\.\d+) (.+\.\w+) \[rgb\]')
-        with open(os.path.join(framesPath, 'data.log')) as f:
-            content = f.read()
-            found = np.array(pattern.findall(content))
-
-        outDict['data']['labelledFrames'] = {}
-        outDict['data']['labelledFrames']['frame'] = {}
-
-        frames_ts = found[:, 0].astype(np.float)
-        tsOffset = min(tsOffset, frames_ts[0])
-        ts_to_sync.append(frames_ts)
-
-        outDict['data']['labelledFrames']['frame']['ts'] = frames_ts
-        outDict['data']['labelledFrames']['frame']['frames'] = [imread(os.path.join(framesPath, x)) for x in found[:, 1]]
-
-
-    # Importing Bounding Boxes for frames
-    framesPath = (os.path.join(os.path.dirname(filePathOrName), '../processed/gt_left')) # TODO make path argument
-    if os.path.exists(framesPath):
-        import re
-        pattern = re.compile('\d+ (\d+\.\d+) (\d+\.\w+) (.*)') # TODO specific to yarp data format
-        pattern2 = re.compile('\( (\d+ \d+ \d+ \d+) \) (\d+) (\d+\.\d+)')
-        with open(os.path.join(framesPath, 'data.log')) as f:
-            content = f.read()
-            found = np.array(pattern.findall(content))
-
-        boxes = []
-        boxes_ts = []
-        labels = []
-
-        for ts, frame_name, bbs in found:
-            for box, label, _ in pattern2.findall(bbs): # TODO third element is confidence score. not used at the moment
-                boxes.append(box.split(' '))
-                labels.append(label)
-                boxes_ts.append(ts)
-
-        boxes_ts = np.array(boxes_ts).astype(np.float)
-        labels = np.array(labels).astype(np.int)
-        boxes = np.array(boxes).astype(np.int)
-
-        tsOffset = min(tsOffset, boxes_ts[0])
-        ts_to_sync.append(boxes_ts)
-        outDict['data']['labelledFrames']['boundingBoxes'] = {}
-        outDict['data']['labelledFrames']['boundingBoxes']['ts'] = boxes_ts
-        outDict['data']['labelledFrames']['boundingBoxes']['minY'] = boxes[:, 0]
-        outDict['data']['labelledFrames']['boundingBoxes']['minX'] = boxes[:, 1]
-        outDict['data']['labelledFrames']['boundingBoxes']['maxY'] = boxes[:, 2]
-        outDict['data']['labelledFrames']['boundingBoxes']['maxX'] = boxes[:, 3]
-        outDict['data']['labelledFrames']['boundingBoxes']['label'] = labels
-
-    for x in ts_to_sync:
-        x -= tsOffset
-
+# -*- coding: utf-8 -*-
+"""
+Copyright (C) 2019 Event-driven Perception for Robotics
+Authors: Massimiliano Iacono
+This program is free software: you can redistribute it and/or modify it under
+the terms of the GNU General Public License as published by the Free Software
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
+importIitNumpy imports timestamped address-event data, given a path to a .npy file.
+It serves the needs of a specific data format developed at IIT involving events, 
+frames and bounding boxes.
+If available at the predetermined locations, relative to the npy file additional 
+data may also be imported, such as frames and bounding boxes used to label the 
+data. At the moment frames and boxes are stored in a data.log file using the 
+YARP format (see importIitYarp as an example). TODO: generalize data structure
+
+The output is a dictionary containing:
+    - info
+    - data
+The exact contents varies according to the file type import but in general:
+    info: this is a dict which starts life as the kwargs passed in, and is
+    augmented and modified by the actual contents of the file. It may include
+    any informational fields in file headers. Minimally, it will contain:
+        - filePathAndName
+        - fileFormat
+    data: this is a list of dicts, one for each sensor or "channel" which has
+    been imported. Bear in mind that sub-functions may optionally split or join
+    channels. Within each dict, there is a field for each type of data contained.
+    A file for example may contain data from a several sensors, but a single sensor
+    may produce polarity events ("pol"), aps samples ("aps"), imu samples etc.
+    Within each of these fields, there is a dict, generally containing fields for
+    each data column, so in the case of pol events, there are 4-5 fields:
+        - ts
+        - x
+        - y
+        - pol
+        - optionally ch (channel)
+        each containing a numpy array of the appropriate type for the data
+        contained, where all these arrays will be of the same length.
+    Similarly bounding boxes are saved in the channel in a separate dictionary containing the following fields:
+        - ts
+        - minY
+        - minX
+        - maxY
+        - maxX
+"""
+
+import numpy as np
+import os
+
+def importIitNumpy(filePathOrName, **kwargs):
+    outDict = {
+        'info': kwargs,
+        'data': {}
+    }
+    outDict['info']['filePathOrName'] = filePathOrName
+
+    # Importing events
+    events = np.load(filePathOrName)
+
+    outDict['data']['labelledEvents'] = {}
+    outDict['data']['labelledEvents']['dvs'] = {}
+
+    tsOffset = events[0, 0]
+    ts_to_sync = [events[:, 0]]
+
+    outDict['data']['labelledEvents']['dvs']['ts'] = events[:, 0]
+    outDict['data']['labelledEvents']['dvs']['x'] = events[:, 1].astype(np.int)
+    outDict['data']['labelledEvents']['dvs']['y'] = events[:, 2].astype(np.int)
+    outDict['data']['labelledEvents']['dvs']['pol'] = events[:, 3].astype(np.bool)
+    outDict['data']['labelledEvents']['dvs']['dimX'] = 304
+    outDict['data']['labelledEvents']['dvs']['dimY'] = 240
+
+
+    # Importing bounding boxes for events
+    gt_filename = os.path.join(os.path.dirname(filePathOrName), 'boxes.npy')
+
+    if os.path.exists(gt_filename):
+        b_boxes = np.load(gt_filename)
+        outDict['data']['labelledEvents']['boundingBoxes'] = {}
+
+        tsOffset = min(tsOffset, b_boxes[0, 0])
+        ts_to_sync.append(b_boxes[:, 0])
+        outDict['data']['labelledEvents']['boundingBoxes']['ts'] = b_boxes[:, 0]
+        outDict['data']['labelledEvents']['boundingBoxes']['minY'] = b_boxes[:, 1]
+        outDict['data']['labelledEvents']['boundingBoxes']['minX'] = b_boxes[:, 2]
+        outDict['data']['labelledEvents']['boundingBoxes']['maxY'] = b_boxes[:, 3]
+        outDict['data']['labelledEvents']['boundingBoxes']['maxX'] = b_boxes[:, 4]
+        outDict['data']['labelledEvents']['boundingBoxes']['label'] = b_boxes[:, 5]
+
+    # Importing frames
+    framesPath = (os.path.join(os.path.dirname(filePathOrName), '../processed/frames_left')) # TODO make path argument
+    if os.path.exists(framesPath):
+        import re
+        from imageio import imread
+        pattern = re.compile('\d+ (\d+\.\d+) (.+\.\w+) \[rgb\]')
+        with open(os.path.join(framesPath, 'data.log')) as f:
+            content = f.read()
+            found = np.array(pattern.findall(content))
+
+        outDict['data']['labelledFrames'] = {}
+        outDict['data']['labelledFrames']['frame'] = {}
+
+        frames_ts = found[:, 0].astype(np.float)
+        tsOffset = min(tsOffset, frames_ts[0])
+        ts_to_sync.append(frames_ts)
+
+        outDict['data']['labelledFrames']['frame']['ts'] = frames_ts
+        outDict['data']['labelledFrames']['frame']['frames'] = [imread(os.path.join(framesPath, x)) for x in found[:, 1]]
+
+
+    # Importing Bounding Boxes for frames
+    framesPath = (os.path.join(os.path.dirname(filePathOrName), '../processed/gt_left')) # TODO make path argument
+    if os.path.exists(framesPath):
+        import re
+        pattern = re.compile('\d+ (\d+\.\d+) (\d+\.\w+) (.*)') # TODO specific to yarp data format
+        pattern2 = re.compile('\( (\d+ \d+ \d+ \d+) \) (\d+) (\d+\.\d+)')
+        with open(os.path.join(framesPath, 'data.log')) as f:
+            content = f.read()
+            found = np.array(pattern.findall(content))
+
+        boxes = []
+        boxes_ts = []
+        labels = []
+
+        for ts, frame_name, bbs in found:
+            for box, label, _ in pattern2.findall(bbs): # TODO third element is confidence score. not used at the moment
+                boxes.append(box.split(' '))
+                labels.append(label)
+                boxes_ts.append(ts)
+
+        boxes_ts = np.array(boxes_ts).astype(np.float)
+        labels = np.array(labels).astype(np.int)
+        boxes = np.array(boxes).astype(np.int)
+
+        tsOffset = min(tsOffset, boxes_ts[0])
+        ts_to_sync.append(boxes_ts)
+        outDict['data']['labelledFrames']['boundingBoxes'] = {}
+        outDict['data']['labelledFrames']['boundingBoxes']['ts'] = boxes_ts
+        outDict['data']['labelledFrames']['boundingBoxes']['minY'] = boxes[:, 0]
+        outDict['data']['labelledFrames']['boundingBoxes']['minX'] = boxes[:, 1]
+        outDict['data']['labelledFrames']['boundingBoxes']['maxY'] = boxes[:, 2]
+        outDict['data']['labelledFrames']['boundingBoxes']['maxX'] = boxes[:, 3]
+        outDict['data']['labelledFrames']['boundingBoxes']['label'] = labels
+
+    for x in ts_to_sync:
+        x -= tsOffset
+
     return outDict
```

### Comparing `bimvee-1.0.9/bimvee/importIitVicon.py` & `bimvee-1.0.9.dev0/bimvee/importIitVicon.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,168 +1,159 @@
-# -*- coding: utf-8 -*-
-"""
-Copyright (C) 2019 Event-driven Perception for Robotics
-Author: Suman Ghosh
-        Sim Bamford
-This program is free software: you can redistribute it and/or modify it under
-the terms of the GNU General Public License as published by the Free Software
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Input:
-vicon data log recorded through yarp
-
-There are two output formats. If 'parameter' separateBodiesAsChannels is present 
-and True then the format is:
-    outDict = {
-        'info': {
-            'filePathOrName': <filepath>
-            'uniqueIds': np.array of strings, one for each unique bodyId 
-            }, 
-        'data': { 
-            <bodyID>: {
-                'pose6q': {
-                    'ts' : <1D array of timestamps>,
-                    'point' : <2D array where each row has 3d position of a body at a time instant>,
-                    'rotation' : <2D array where each row has rotation of a body at a time instant expressed as a quaternion (4d)>} } } }
-Otherwise:
-    outDict = {
-        'info': {
-            'filePathOrName': <filepath>
-            }, 
-        'data': {
-            'vicon': {
-                'pose6q': {
-                    'ts' : <1D array of timestamps>,
-                    'point' : <2D array where each row has 3d position of a body at a time instant>,
-                    'rotation' : <2D array where each row has rotation of a body at a time instant expressed as a quaternion (4d)>,
-                    'bodyId' : <1D array where each row has the bodyId of the corresponding marker>,
-                    } } } }
-    
-A bodyID is the name assigned by vicon to a marker (labeled / unlableled) or rigid body
-The pose consists of a point in the form [x, y, z]
-and a rotation as a quaternion [r_w, r_x, r_y, r_z] (Caution with alternative orderings here)
-The datatype is called 'pose6q', referring to the 6dof with rotation in quaternion form.
-
-Additionally, if separateBodiesAsChannels is not present or false, 
-and the separateMarkersAndSegments parameter is present and True,
-then the data in the vicon channel is broken into two datatypes:
-        ...
-            'vicon': {
-                'pose6q': {
-                    'ts' : <1D array of timestamps>,
-                    'point' : <2D array where each row has 3d position of a body at a time instant>,
-                    'rotation' : <2D array where each row has the rotation of a body at a time instant expressed as a quaternion (4d)>,
-                    'bodyId' : <1D array where each row has the bodyId of the corresponding marker>,
-                    } 
-                'point3': {
-                    'ts' : <1D array of timestamps>,
-                    'point' : <2D array where each row has 3d position of a body at a time instant>,
-                    'bodyId' : <1D array where each row has the bodyId of the corresponding marker>,
-                    } ...
-                
-Known Issue: timestamps may not be monotonic in the raw data, 
-and this function doesn't attempt to correct it.
-Timestamps are monotonic for a single segment, but not necessarily for multiple 
-segments imported in the same container.
-"""
-
-import os
-import re
-import numpy as np
-
-# local imports
-from .timestamps import zeroTimestampsForADataType
-from .split import splitByLabel
-
-def getOrInsertDefault(inDict, arg, default):
-    # get an arg from a dict.
-    # If the the dict doesn't contain the arg, return the default, 
-    # and also insert the default into the dict
-    value = inDict.get(arg, default)
-    if value == default:
-        inDict[arg] = default
-    return value
-
-# accepts a pose6q datatype dict; returns a channel dict containing pose6q and point3 datatypes
-def separateMarkersFromSegments(poseDict):
-    isMarker = np.apply_along_axis(lambda x : 'Marker' in str(x[0]), 1, poseDict['bodyId'][..., np.newaxis])
-    pointDict = {
-        'ts': poseDict['ts'][isMarker],
-        'point': poseDict['point'][isMarker, :],
-        'bodyId': poseDict['bodyId'][isMarker],
-        }
-    poseDict = {
-        'ts': poseDict['ts'][~isMarker],
-        'point': poseDict['point'][~isMarker, :],
-        'rotation': poseDict['rotation'][~isMarker, :],
-        'bodyId': poseDict['bodyId'][~isMarker],
-        }
-    return {
-        'pose6q': poseDict,
-        'point3': pointDict}
-    
-def importIitVicon(**kwargs):
-    filePathOrName = kwargs.get('filePathOrName')
-    # handle the case in which filename is not specified - iterate through files 
-    # in the current directory looking for data.log
-    if filePathOrName is None:
-        files = [file for file in os.listdir('.') if os.path.isfile(file)]
-        for filename in files:
-            if filename == 'data.log':
-                kwargs['filePathOrName'] = filename
-                return importIitVicon(**kwargs)
-        print('No suitable file found')
-        return None
-    pattern = re.compile('(\d+) (\d+\.\d+) \((.*)\)')
-    # yarpBottleTimes = []
-    outDict = {'info': {'filePathOrName': filePathOrName}, 'data': {}}
-    poseDict = {'ts': [], 'point': [], 'rotation': [], 'bodyId': []}
-    with open(filePathOrName, 'r') as file:
-        print('Found file to read')
-        line = file.readline()
-        while line:
-            found = pattern.search(line.strip())
-            # yarpBottleTimes.append(float(found.group(2)))
-            viconData = found.group(3)
-            bodies = viconData.split(') (')
-            for body in bodies:
-                elements = body.split(" ")
-                bodyId = elements[1].strip('\"')
-                ts = elements[2]
-                point = elements[3:6]
-                # Note: quaternion order is [w,x,y,z] - this is defined by yarp 
-                # IFrameTransform component, so ignore vicon documentation
-                rotation = elements[6:] 
-                poseDict['ts'].append(ts)
-                poseDict['point'].append(point)
-                poseDict['rotation'].append(rotation)
-                poseDict['bodyId'].append(bodyId)
-            line = file.readline()
-
-    # converting lists of strings to numpy arrays of objects
-    poseDict['ts'] = np.array(poseDict['ts'], dtype=np.float64)
-    poseDict['point'] = np.array(poseDict['point'], dtype=np.float64)
-    poseDict['rotation'] = np.array(poseDict['rotation'], dtype=np.float64)
-    poseDict['bodyId'] = np.array(poseDict['bodyId'], dtype=object)
-    if kwargs.get('zeroTime', kwargs.get('zeroTimestamps', True)):
-        zeroTimestampsForADataType(poseDict)
-    if kwargs.get('separateBodiesAsChannels', False):
-        outDict['info']['uniqueIds'] = np.unique(poseDict['bodyId'])
-        separatedBodies = splitByLabel(poseDict, 'bodyId')
-        # The next line inserts the missing 'pose6q' dataType level into the hierarchy
-        outDict['data'] = {bodyName: {'pose6q': bodyDict} 
-                           for bodyName, bodyDict in zip(
-                                   separatedBodies.keys(), 
-                                   separatedBodies.values())}
-    elif kwargs.get('separateMarkersFromSegments', False):
-        outDict['data']['vicon'] = separateMarkersFromSegments(poseDict)
-    else:            
-        outDict['data']['vicon'] = {'pose6q': poseDict}
-    return outDict
-
-
-
+# -*- coding: utf-8 -*-
+"""
+Copyright (C) 2019 Event-driven Perception for Robotics
+Author: Suman Ghosh
+        Sim Bamford
+This program is free software: you can redistribute it and/or modify it under
+the terms of the GNU General Public License as published by the Free Software
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Input:
+vicon data log recorded through yarp
+
+There are two output formats. If 'parameter' separateBodiesAsChannels is present 
+and True then the format is:
+    outDict = {
+        'info': {
+            'filePathOrName': <filepath>
+            'uniqueIds': np.array of strings, one for each unique bodyId 
+            }, 
+        'data': { 
+            <bodyID>: {
+                'pose6q': {
+                    'ts' : <1D array of timestamps>,
+                    'point' : <2D array where each row has 3d position of a body at a time instant>,
+                    'rotation' : <2D array where each row has rotation of a body at a time instant expressed as a quaternion (4d)>} } } }
+Otherwise:
+    outDict = {
+        'info': {
+            'filePathOrName': <filepath>
+            }, 
+        'data': {
+            'vicon': {
+                'pose6q': {
+                    'ts' : <1D array of timestamps>,
+                    'point' : <2D array where each row has 3d position of a body at a time instant>,
+                    'rotation' : <2D array where each row has rotation of a body at a time instant expressed as a quaternion (4d)>,
+                    'bodyId' : <1D array where each row has the bodyId of the corresponding marker>,
+                    } } } }
+    
+A bodyID is the name assigned by vicon to a marker (labeled / unlableled) or rigid body
+The pose consists of a point in the form [x, y, z]
+and a rotation as a quaternion [r_w, r_x, r_y, r_z] (Caution with alternative orderings here)
+The datatype is called 'pose6q', referring to the 6dof with rotation in quaternion form.
+
+Additionally, if separateBodiesAsChannels is not present or false, 
+and the separateMarkersAndSegments parameter is present and True,
+then the data in the vicon channel is broken into two datatypes:
+        ...
+            'vicon': {
+                'pose6q': {
+                    'ts' : <1D array of timestamps>,
+                    'point' : <2D array where each row has 3d position of a body at a time instant>,
+                    'rotation' : <2D array where each row has the rotation of a body at a time instant expressed as a quaternion (4d)>,
+                    'bodyId' : <1D array where each row has the bodyId of the corresponding marker>,
+                    } 
+                'point3': {
+                    'ts' : <1D array of timestamps>,
+                    'point' : <2D array where each row has 3d position of a body at a time instant>,
+                    'bodyId' : <1D array where each row has the bodyId of the corresponding marker>,
+                    } ...
+                
+Known Issue: timestamps may not be monotonic in the raw data, 
+and this function doesn't attempt to correct it.
+Timestamps are monotonic for a single segment, but not necessarily for multiple 
+segments imported in the same container.
+"""
+
+import os
+import re
+import numpy as np
+
+# local imports
+from .timestamps import zeroTimestampsForADataType
+from .split import splitByLabel, selectByBool
+
+def getOrInsertDefault(inDict, arg, default):
+    # get an arg from a dict.
+    # If the the dict doesn't contain the arg, return the default, 
+    # and also insert the default into the dict
+    value = inDict.get(arg, default)
+    if value == default:
+        inDict[arg] = default
+    return value
+
+# accepts a pose6q datatype dict; returns a channel dict containing pose6q and point3 datatypes
+def separateMarkersFromSegments(poseDict):
+    isMarker = np.apply_along_axis(lambda x : 'Marker' in str(x[0]), 1, poseDict['bodyId'][..., np.newaxis])
+    pointDict = selectByBool(poseDict, isMarker)
+    poseDict = selectByBool(poseDict, ~isMarker)
+    return {
+        'pose6q': poseDict,
+        'point3': pointDict}
+    
+def importIitVicon(**kwargs):
+    filePathOrName = kwargs.get('filePathOrName')
+    # handle the case in which filename is not specified - iterate through files 
+    # in the current directory looking for data.log
+    if filePathOrName is None:
+        files = [file for file in os.listdir('.') if os.path.isfile(file)]
+        for filename in files:
+            if filename == 'data.log':
+                kwargs['filePathOrName'] = filename
+                return importIitVicon(**kwargs)
+        print('No suitable file found')
+        return None
+    pattern = re.compile('(\d+) (\d+\.\d+) \((.*)\)')
+    # yarpBottleTimes = []
+    outDict = {'info': {'filePathOrName': filePathOrName}, 'data': {}}
+    poseDict = {'ts': [], 'point': [], 'rotation': [], 'bodyId': []}
+    with open(filePathOrName, 'r') as file:
+        print('Found file to read')
+        line = file.readline()
+        while line:
+            found = pattern.search(line.strip())
+            # yarpBottleTimes.append(float(found.group(2)))
+            viconData = found.group(3)
+            bodies = viconData.split(') (')
+            for body in bodies:
+                elements = body.split(" ")
+                bodyId = elements[1].strip('\"')
+                ts = elements[2]
+                point = elements[3:6]
+                # Note: quaternion order is [w,x,y,z] - this is defined by yarp 
+                # IFrameTransform component, so ignore vicon documentation
+                rotation = elements[6:] 
+                poseDict['ts'].append(ts)
+                poseDict['point'].append(point)
+                poseDict['rotation'].append(rotation)
+                poseDict['bodyId'].append(bodyId)
+            line = file.readline()
+
+    # converting lists of strings to numpy arrays of objects
+    poseDict['ts'] = np.array(poseDict['ts'], dtype=np.float64)
+    poseDict['point'] = np.array(poseDict['point'], dtype=np.float64)
+    poseDict['rotation'] = np.array(poseDict['rotation'], dtype=np.float64)
+    poseDict['bodyId'] = np.array(poseDict['bodyId'], dtype=object)
+    if kwargs.get('zeroTime', kwargs.get('zeroTimestamps', True)):
+        zeroTimestampsForADataType(poseDict)
+    if kwargs.get('separateBodiesAsChannels', False):
+        outDict['info']['uniqueIds'] = np.unique(poseDict['bodyId'])
+        separatedBodies = splitByLabel(poseDict, 'bodyId')
+        # The next line inserts the missing 'pose6q' dataType level into the hierarchy
+        outDict['data'] = {bodyName: {'pose6q': bodyDict} 
+                           for bodyName, bodyDict in zip(
+                                   separatedBodies.keys(), 
+                                   separatedBodies.values())}
+    elif kwargs.get('separateMarkersFromSegments', False):
+        outDict['data']['vicon'] = separateMarkersFromSegments(poseDict)
+    else:            
+        outDict['data']['vicon'] = {'pose6q': poseDict}
+    return outDict
+
+
+
```

### Comparing `bimvee-1.0.9/bimvee/importRosbag/importRosbag/importRosbag.py` & `bimvee-1.0.9.dev0/bimvee/importRosbag/importRosbag/importRosbag.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,241 +1,241 @@
-# -*- coding: utf-8 -*-
-
-"""
-Copyright (C) 2019 Event-driven Perception for Robotics
-Authors: Sim Bamford
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Unpacks a rosbag into its topics and messages
-Uses the topic types to interpret the messages from each topic, 
-yielding dicts for each topic containing iterables for each field.
-By default unpacks all topics, but you can use any of the following keyword 
-params to limit which topics are intepretted:
-    - 'listTopics' = True - no unpacking - just returns a list of the topics contained in 
-       the file and their associated types
-    - 'importTopics' = <list of strings> - only imports the listed topics
-    - 'importTypes' = <list of strings> - only imports the listed types
-
-Message types supported are strictly those listed in the initial imports section
-of this file. There are a selection of standard message types and a couple
-related to event-based sensors. 
-The method of importation is honed to the particular needs of
-the author, sometimes ignoring certain fields, grouping data in particular ways 
-etc. However it should serve as a model for anyone who wishes to import rosbags.
-Although it's possible to import messages programmatically given only the 
-message definition files, we have chosen not to do this, because if we did it
-we would anyway need to take the resulting data and pick out the bits we wanted. 
-
-"""
-
-#%%
-
-from struct import unpack
-from struct import error as structError
-from tqdm import tqdm
-
-# Local imports
-
-from .messageTypes.common import unpackHeader
-
-from .messageTypes.dvs_msgs_EventArray import importTopic as import_dvs_msgs_EventArray
-from .messageTypes.esim_msgs_OpticFlow import importTopic as import_esim_msgs_OpticFlow
-from .messageTypes.geometry_msgs_PoseStamped import importTopic as import_geometry_msgs_PoseStamped
-from .messageTypes.geometry_msgs_Transform import importTopic as import_geometry_msgs_Transform
-from .messageTypes.geometry_msgs_TransformStamped import importTopic as import_geometry_msgs_TransformStamped
-from .messageTypes.geometry_msgs_TwistStamped import importTopic as import_geometry_msgs_TwistStamped
-from .messageTypes.sensor_msgs_CameraInfo import importTopic as import_sensor_msgs_CameraInfo
-from .messageTypes.sensor_msgs_Image import importTopic as import_sensor_msgs_Image
-from .messageTypes.sensor_msgs_Imu import importTopic as import_sensor_msgs_Imu
-from .messageTypes.sensor_msgs_PointCloud2 import importTopic as import_sensor_msgs_PointCloud2
-from .messageTypes.tf_tfMessage import importTopic as import_tf_tfMessage
-
-def importTopic(topic, **kwargs):
-    msgs = topic['msgs']
-    topicType = topic['type'].replace('/','_')
-    if topicType == 'dvs_msgs_EventArray': topicDict = import_dvs_msgs_EventArray(msgs, **kwargs)
-    elif topicType == 'esim_msgs_OpticFlow': topicDict = import_esim_msgs_OpticFlow(msgs, **kwargs)
-    elif topicType == 'geometry_msgs_PoseStamped': topicDict = import_geometry_msgs_PoseStamped(msgs, **kwargs)
-    elif topicType == 'geometry_msgs_Transform': topicDict = import_geometry_msgs_Transform(msgs, **kwargs)
-    elif topicType == 'geometry_msgs_TransformStamped': topicDict = import_geometry_msgs_TransformStamped(msgs, **kwargs)
-    elif topicType == 'geometry_msgs_TwistStamped': topicDict = import_geometry_msgs_TwistStamped(msgs, **kwargs)
-    elif topicType == 'sensor_msgs_CameraInfo': topicDict = import_sensor_msgs_CameraInfo(msgs, **kwargs)
-    elif topicType == 'sensor_msgs_Image': topicDict = import_sensor_msgs_Image(msgs, **kwargs)
-    elif topicType == 'sensor_msgs_Imu': topicDict = import_sensor_msgs_Imu(msgs, **kwargs)
-    elif topicType == 'sensor_msgs_PointCloud2': topicDict = import_sensor_msgs_PointCloud2(msgs, **kwargs)
-    elif topicType == 'tf_tfMessage': topicDict = import_tf_tfMessage(msgs, **kwargs)
-    else: 
-        return None
-    if topicDict:
-        topicDict['rosbagType'] = topic['type']
-    return topicDict
-
-def readFile(filePathOrName):
-    print('Attempting to import ' + filePathOrName + ' as a rosbag 2.0 file.')
-    with open(filePathOrName, 'rb') as file:
-        # File format string
-        fileFormatString = file.readline().decode("utf-8")
-        print('ROSBAG file format: ' + fileFormatString)
-        if fileFormatString != '#ROSBAG V2.0\n':
-            print('This file format might not be supported')
-        eof = False
-        conns = []
-        chunks = []
-        while not eof:
-            # Read a record header
-            try:
-                headerLen = unpack('=l', file.read(4))[0]
-            except structError:
-                if len(file.read(1)) == 0: # Distinguish EOF from other struct errors 
-                   # a struct error could also occur if the data is downloaded by one os and read by another.
-                   eof = True
-                   continue
-            # unpack the header into fields 
-            headerBytes = file.read(headerLen)
-            fields = unpackHeader(headerLen, headerBytes)
-            # Read the record data
-            dataLen = unpack('=l', file.read(4))[0]
-            data = file.read(dataLen)
-            # The op code tells us what to do with the record
-            op = unpack('=b', fields['op'])[0]
-            fields['op'] = op
-            if op == 2:
-                # It's a message
-                # AFAIK these are not found unpacked in the file
-                #fields['data'] = data 
-                #msgs.append(fields)
-                pass
-            elif op == 3:
-                # It's a bag header - use this to do progress bar for the read
-                chunkCount = unpack('=l', fields['chunk_count'])[0]
-                pbar = tqdm(total=chunkCount, position=0, leave=True)
-            elif op == 4:
-                # It's an index - this is used to index the previous chunk
-                conn = unpack('=l', fields['conn'])[0]
-                count = unpack('=l', fields['count'])[0]
-                for idx in range(count):
-                    time, offset = unpack('=ql', data[idx*12:idx*12+12])
-                    chunks[-1]['ids'].append((conn, time, offset))
-            elif op == 5:
-                # It's a chunk
-                fields['data'] = data
-                fields['ids'] = []
-                chunks.append(fields)
-                pbar.update(len(chunks))
-            elif op == 6:
-                # It's a chunk-info - seems to be redundant
-                pass
-            elif op == 7:
-                # It's a conn
-                # interpret data as a string containing the connection header
-                connFields = unpackHeader(dataLen, data)
-                connFields.update(fields) 
-                connFields['conn'] = unpack('=l', connFields['conn'])[0]
-                connFields['topic'] = connFields['topic'].decode("utf-8")
-                connFields['type'] = connFields['type'].decode("utf-8").replace('/', '_')
-                conns.append(connFields)
-    return conns, chunks
-
-#%% Break chunks into msgs
-
-def breakChunksIntoMsgs(chunks):
-    msgs = [] 
-    print('Breaking chunks into msgs ...')           
-    for chunk in tqdm(chunks, position=0, leave=True):
-        for idx in chunk['ids']:
-            ptr = idx[2]
-            headerLen = unpack('=l', chunk['data'][ptr:ptr+4])[0]
-            ptr += 4
-            # unpack the header into fields 
-            headerBytes = chunk['data'][ptr:ptr+headerLen]
-            ptr += headerLen
-            fields = unpackHeader(headerLen, headerBytes)
-            # Read the record data
-            dataLen = unpack('=l', chunk['data'][ptr:ptr+4])[0]
-            ptr += 4
-            fields['data'] = chunk['data'][ptr:ptr+dataLen]
-            fields['conn'] = unpack('=l', fields['conn'])[0]
-            msgs.append(fields)
-    return msgs
-
-def rekeyConnsByTopic(connDict):
-    topics = {}
-    for conn in connDict:
-        topics[connDict[conn]['topic']] = connDict[conn]
-    return topics
-
-
-def importRosbag(filePathOrName, **kwargs):
-    print('Importing file: ', filePathOrName) 
-    conns, chunks = readFile(filePathOrName)
-    # Restructure conns as a dictionary keyed by conn number
-    connDict = {}
-    for conn in conns:
-        connDict[conn['conn']] = conn
-        conn['msgs'] = []
-    if kwargs.get('listTopics', False):
-        topics = rekeyConnsByTopic(connDict)
-        print('Topics in the file are (with types):')
-        for topicKey, topic in topics.items():
-            del topic['conn']
-            del topic['md5sum']
-            del topic['msgs']
-            del topic['op']
-            del topic['topic']
-            topic['message_definition'] = topic['message_definition'].decode("utf-8")
-            print('    ' + topicKey + ' --- ' + topic['type'])
-        return topics
-    msgs = breakChunksIntoMsgs(chunks)
-    for msg in msgs:     
-        connDict[msg['conn']]['msgs'].append(msg)
-    topics = rekeyConnsByTopic(connDict)
-
-    importedTopics = {}
-    importTopics = kwargs.get('importTopics')
-    importTypes = kwargs.get('importTypes')
-    if importTopics is not None:
-        for topicToImport in importTopics:
-            for topicInFile in topics.keys():
-                if topicInFile == topicToImport:
-                    importedTopic = importTopic(topics[topicInFile], **kwargs)
-                    if importedTopic is not None:
-                        importedTopics[topicToImport] = importedTopic
-                        del topics[topicInFile]            
-    elif importTypes is not None:
-        for typeToImport in importTypes:
-            typeToImport = typeToImport.replace('/', '_')
-            for topicInFile in list(topics.keys()):
-                if topics[topicInFile]['type'].replace('/', '_') == typeToImport:
-                    importedTopic = importTopic(topics[topicInFile], **kwargs)
-                    if importedTopic is not None:
-                        importedTopics[topicInFile] = importedTopic
-                        del topics[topicInFile]    
-    else: # import everything
-        for topicInFile in list(topics.keys()):
-            importedTopic = importTopic(topics[topicInFile], **kwargs)
-            if importedTopic is not None:
-                importedTopics[topicInFile] = importedTopic
-                del topics[topicInFile]
-
-    print()
-    if importedTopics:
-        print('Topics imported are:')
-        for topic in importedTopics.keys():
-            print(topic + ' --- ' + importedTopics[topic]['rosbagType'])
-            #del importedTopics[topic]['rosbagType']
-        print()
-
-    if topics:
-        print('Topics not imported are:')
-        for topic in topics.keys():
-            print(topic + ' --- ' + topics[topic]['type'])
-        print()
-    
-    return importedTopics
-
+# -*- coding: utf-8 -*-
+
+"""
+Copyright (C) 2019 Event-driven Perception for Robotics
+Authors: Sim Bamford
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Unpacks a rosbag into its topics and messages
+Uses the topic types to interpret the messages from each topic, 
+yielding dicts for each topic containing iterables for each field.
+By default unpacks all topics, but you can use any of the following keyword 
+params to limit which topics are intepretted:
+    - 'listTopics' = True - no unpacking - just returns a list of the topics contained in 
+       the file and their associated types
+    - 'importTopics' = <list of strings> - only imports the listed topics
+    - 'importTypes' = <list of strings> - only imports the listed types
+
+Message types supported are strictly those listed in the initial imports section
+of this file. There are a selection of standard message types and a couple
+related to event-based sensors. 
+The method of importation is honed to the particular needs of
+the author, sometimes ignoring certain fields, grouping data in particular ways 
+etc. However it should serve as a model for anyone who wishes to import rosbags.
+Although it's possible to import messages programmatically given only the 
+message definition files, we have chosen not to do this, because if we did it
+we would anyway need to take the resulting data and pick out the bits we wanted. 
+
+"""
+
+#%%
+
+from struct import unpack
+from struct import error as structError
+from tqdm import tqdm
+
+# Local imports
+
+from .messageTypes.common import unpackHeader
+
+from .messageTypes.dvs_msgs_EventArray import importTopic as import_dvs_msgs_EventArray
+from .messageTypes.esim_msgs_OpticFlow import importTopic as import_esim_msgs_OpticFlow
+from .messageTypes.geometry_msgs_PoseStamped import importTopic as import_geometry_msgs_PoseStamped
+from .messageTypes.geometry_msgs_Transform import importTopic as import_geometry_msgs_Transform
+from .messageTypes.geometry_msgs_TransformStamped import importTopic as import_geometry_msgs_TransformStamped
+from .messageTypes.geometry_msgs_TwistStamped import importTopic as import_geometry_msgs_TwistStamped
+from .messageTypes.sensor_msgs_CameraInfo import importTopic as import_sensor_msgs_CameraInfo
+from .messageTypes.sensor_msgs_Image import importTopic as import_sensor_msgs_Image
+from .messageTypes.sensor_msgs_Imu import importTopic as import_sensor_msgs_Imu
+from .messageTypes.sensor_msgs_PointCloud2 import importTopic as import_sensor_msgs_PointCloud2
+from .messageTypes.tf_tfMessage import importTopic as import_tf_tfMessage
+
+def importTopic(topic, **kwargs):
+    msgs = topic['msgs']
+    topicType = topic['type'].replace('/','_')
+    if topicType == 'dvs_msgs_EventArray': topicDict = import_dvs_msgs_EventArray(msgs, **kwargs)
+    elif topicType == 'esim_msgs_OpticFlow': topicDict = import_esim_msgs_OpticFlow(msgs, **kwargs)
+    elif topicType == 'geometry_msgs_PoseStamped': topicDict = import_geometry_msgs_PoseStamped(msgs, **kwargs)
+    elif topicType == 'geometry_msgs_Transform': topicDict = import_geometry_msgs_Transform(msgs, **kwargs)
+    elif topicType == 'geometry_msgs_TransformStamped': topicDict = import_geometry_msgs_TransformStamped(msgs, **kwargs)
+    elif topicType == 'geometry_msgs_TwistStamped': topicDict = import_geometry_msgs_TwistStamped(msgs, **kwargs)
+    elif topicType == 'sensor_msgs_CameraInfo': topicDict = import_sensor_msgs_CameraInfo(msgs, **kwargs)
+    elif topicType == 'sensor_msgs_Image': topicDict = import_sensor_msgs_Image(msgs, **kwargs)
+    elif topicType == 'sensor_msgs_Imu': topicDict = import_sensor_msgs_Imu(msgs, **kwargs)
+    elif topicType == 'sensor_msgs_PointCloud2': topicDict = import_sensor_msgs_PointCloud2(msgs, **kwargs)
+    elif topicType == 'tf_tfMessage': topicDict = import_tf_tfMessage(msgs, **kwargs)
+    else: 
+        return None
+    if topicDict:
+        topicDict['rosbagType'] = topic['type']
+    return topicDict
+
+def readFile(filePathOrName):
+    print('Attempting to import ' + filePathOrName + ' as a rosbag 2.0 file.')
+    with open(filePathOrName, 'rb') as file:
+        # File format string
+        fileFormatString = file.readline().decode("utf-8")
+        print('ROSBAG file format: ' + fileFormatString)
+        if fileFormatString != '#ROSBAG V2.0\n':
+            print('This file format might not be supported')
+        eof = False
+        conns = []
+        chunks = []
+        while not eof:
+            # Read a record header
+            try:
+                headerLen = unpack('=l', file.read(4))[0]
+            except structError:
+                if len(file.read(1)) == 0: # Distinguish EOF from other struct errors 
+                   # a struct error could also occur if the data is downloaded by one os and read by another.
+                   eof = True
+                   continue
+            # unpack the header into fields 
+            headerBytes = file.read(headerLen)
+            fields = unpackHeader(headerLen, headerBytes)
+            # Read the record data
+            dataLen = unpack('=l', file.read(4))[0]
+            data = file.read(dataLen)
+            # The op code tells us what to do with the record
+            op = unpack('=b', fields['op'])[0]
+            fields['op'] = op
+            if op == 2:
+                # It's a message
+                # AFAIK these are not found unpacked in the file
+                #fields['data'] = data 
+                #msgs.append(fields)
+                pass
+            elif op == 3:
+                # It's a bag header - use this to do progress bar for the read
+                chunkCount = unpack('=l', fields['chunk_count'])[0]
+                pbar = tqdm(total=chunkCount, position=0, leave=True)
+            elif op == 4:
+                # It's an index - this is used to index the previous chunk
+                conn = unpack('=l', fields['conn'])[0]
+                count = unpack('=l', fields['count'])[0]
+                for idx in range(count):
+                    time, offset = unpack('=ql', data[idx*12:idx*12+12])
+                    chunks[-1]['ids'].append((conn, time, offset))
+            elif op == 5:
+                # It's a chunk
+                fields['data'] = data
+                fields['ids'] = []
+                chunks.append(fields)
+                pbar.update(len(chunks))
+            elif op == 6:
+                # It's a chunk-info - seems to be redundant
+                pass
+            elif op == 7:
+                # It's a conn
+                # interpret data as a string containing the connection header
+                connFields = unpackHeader(dataLen, data)
+                connFields.update(fields) 
+                connFields['conn'] = unpack('=l', connFields['conn'])[0]
+                connFields['topic'] = connFields['topic'].decode("utf-8")
+                connFields['type'] = connFields['type'].decode("utf-8").replace('/', '_')
+                conns.append(connFields)
+    return conns, chunks
+
+#%% Break chunks into msgs
+
+def breakChunksIntoMsgs(chunks):
+    msgs = [] 
+    print('Breaking chunks into msgs ...')           
+    for chunk in tqdm(chunks, position=0, leave=True):
+        for idx in chunk['ids']:
+            ptr = idx[2]
+            headerLen = unpack('=l', chunk['data'][ptr:ptr+4])[0]
+            ptr += 4
+            # unpack the header into fields 
+            headerBytes = chunk['data'][ptr:ptr+headerLen]
+            ptr += headerLen
+            fields = unpackHeader(headerLen, headerBytes)
+            # Read the record data
+            dataLen = unpack('=l', chunk['data'][ptr:ptr+4])[0]
+            ptr += 4
+            fields['data'] = chunk['data'][ptr:ptr+dataLen]
+            fields['conn'] = unpack('=l', fields['conn'])[0]
+            msgs.append(fields)
+    return msgs
+
+def rekeyConnsByTopic(connDict):
+    topics = {}
+    for conn in connDict:
+        topics[connDict[conn]['topic']] = connDict[conn]
+    return topics
+
+
+def importRosbag(filePathOrName, **kwargs):
+    print('Importing file: ', filePathOrName) 
+    conns, chunks = readFile(filePathOrName)
+    # Restructure conns as a dictionary keyed by conn number
+    connDict = {}
+    for conn in conns:
+        connDict[conn['conn']] = conn
+        conn['msgs'] = []
+    if kwargs.get('listTopics', False):
+        topics = rekeyConnsByTopic(connDict)
+        print('Topics in the file are (with types):')
+        for topicKey, topic in topics.items():
+            del topic['conn']
+            del topic['md5sum']
+            del topic['msgs']
+            del topic['op']
+            del topic['topic']
+            topic['message_definition'] = topic['message_definition'].decode("utf-8")
+            print('    ' + topicKey + ' --- ' + topic['type'])
+        return topics
+    msgs = breakChunksIntoMsgs(chunks)
+    for msg in msgs:     
+        connDict[msg['conn']]['msgs'].append(msg)
+    topics = rekeyConnsByTopic(connDict)
+
+    importedTopics = {}
+    importTopics = kwargs.get('importTopics')
+    importTypes = kwargs.get('importTypes')
+    if importTopics is not None:
+        for topicToImport in importTopics:
+            for topicInFile in topics.keys():
+                if topicInFile == topicToImport:
+                    importedTopic = importTopic(topics[topicInFile], **kwargs)
+                    if importedTopic is not None:
+                        importedTopics[topicToImport] = importedTopic
+                        del topics[topicInFile]            
+    elif importTypes is not None:
+        for typeToImport in importTypes:
+            typeToImport = typeToImport.replace('/', '_')
+            for topicInFile in list(topics.keys()):
+                if topics[topicInFile]['type'].replace('/', '_') == typeToImport:
+                    importedTopic = importTopic(topics[topicInFile], **kwargs)
+                    if importedTopic is not None:
+                        importedTopics[topicInFile] = importedTopic
+                        del topics[topicInFile]    
+    else: # import everything
+        for topicInFile in list(topics.keys()):
+            importedTopic = importTopic(topics[topicInFile], **kwargs)
+            if importedTopic is not None:
+                importedTopics[topicInFile] = importedTopic
+                del topics[topicInFile]
+
+    print()
+    if importedTopics:
+        print('Topics imported are:')
+        for topic in importedTopics.keys():
+            print(topic + ' --- ' + importedTopics[topic]['rosbagType'])
+            #del importedTopics[topic]['rosbagType']
+        print()
+
+    if topics:
+        print('Topics not imported are:')
+        for topic in topics.keys():
+            print(topic + ' --- ' + topics[topic]['type'])
+        print()
+    
+    return importedTopics
+
```

### Comparing `bimvee-1.0.9/bimvee/importRosbag/importRosbag/messageTypes/common.py` & `bimvee-1.0.9.dev0/bimvee/importRosbag/importRosbag/messageTypes/common.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-# -*- coding: utf-8 -*-
-
-"""
-Copyright (C) 2019 Event-driven Perception for Robotics
-Authors: Sim Bamford
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Intended as part of importRosbag.
-
-"""
-
-#%%
-
-from struct import unpack
-import numpy as np
-
-def unpackHeader(headerLen, headerBytes):
-    fields = {}
-    ptr = 0
-    while ptr < headerLen:
-        fieldLen = unpack('=l', headerBytes[ptr:ptr+4])[0]
-        ptr += 4
-        #print(fieldLen)
-        field = headerBytes[ptr:ptr+fieldLen]
-        ptr += fieldLen
-        #print(field)
-        fieldSplit = field.find(b'\x3d')
-        fieldName = field[:fieldSplit].decode("utf-8")
-        fieldValue = field[fieldSplit+1:]
-        fields[fieldName] = fieldValue
-    return fields
-
-def unpackRosUint32(data, ptr):
-    return unpack('=L', data[ptr:ptr+4])[0], ptr+4
-
-def unpackRosUint8(data, ptr):
-    return unpack('=B', data[ptr:ptr+1])[0], ptr+1
-
-def unpackRosString(data, ptr):
-    stringLen = unpack('=L', data[ptr:ptr+4])[0]
-    ptr += 4
-    try:
-        outStr = data[ptr:ptr+stringLen].decode('utf-8')
-    except UnicodeDecodeError:
-        outStr = 'UnicodeDecodeError'
-    ptr += stringLen
-    return outStr, ptr
-
-def unpackRosFloat64Array(data, num, ptr):
-    return np.frombuffer(data[ptr:ptr+num*8], dtype=np.float64), ptr+num*8 
-    
-def unpackRosFloat32Array(data, num, ptr):
-    return np.frombuffer(data[ptr:ptr+num*4], dtype=np.float32), ptr+num*4 
-    
-def unpackRosFloat32(data, ptr):
-    return unpack('=f', data[ptr:ptr+4])[0], ptr+4 
-    
-def unpackRosTimestamp(data, ptr):
-    timeS, timeNs = unpack('=LL', data[ptr:ptr+8])
-    timeFloat = np.float64(timeS)+np.float64(timeNs)*0.000000001 
-    return timeFloat, ptr+8
+# -*- coding: utf-8 -*-
+
+"""
+Copyright (C) 2019 Event-driven Perception for Robotics
+Authors: Sim Bamford
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Intended as part of importRosbag.
+
+"""
+
+#%%
+
+from struct import unpack
+import numpy as np
+
+def unpackHeader(headerLen, headerBytes):
+    fields = {}
+    ptr = 0
+    while ptr < headerLen:
+        fieldLen = unpack('=l', headerBytes[ptr:ptr+4])[0]
+        ptr += 4
+        #print(fieldLen)
+        field = headerBytes[ptr:ptr+fieldLen]
+        ptr += fieldLen
+        #print(field)
+        fieldSplit = field.find(b'\x3d')
+        fieldName = field[:fieldSplit].decode("utf-8")
+        fieldValue = field[fieldSplit+1:]
+        fields[fieldName] = fieldValue
+    return fields
+
+def unpackRosUint32(data, ptr):
+    return unpack('=L', data[ptr:ptr+4])[0], ptr+4
+
+def unpackRosUint8(data, ptr):
+    return unpack('=B', data[ptr:ptr+1])[0], ptr+1
+
+def unpackRosString(data, ptr):
+    stringLen = unpack('=L', data[ptr:ptr+4])[0]
+    ptr += 4
+    try:
+        outStr = data[ptr:ptr+stringLen].decode('utf-8')
+    except UnicodeDecodeError:
+        outStr = 'UnicodeDecodeError'
+    ptr += stringLen
+    return outStr, ptr
+
+def unpackRosFloat64Array(data, num, ptr):
+    return np.frombuffer(data[ptr:ptr+num*8], dtype=np.float64), ptr+num*8 
+    
+def unpackRosFloat32Array(data, num, ptr):
+    return np.frombuffer(data[ptr:ptr+num*4], dtype=np.float32), ptr+num*4 
+    
+def unpackRosFloat32(data, ptr):
+    return unpack('=f', data[ptr:ptr+4])[0], ptr+4 
+    
+def unpackRosTimestamp(data, ptr):
+    timeS, timeNs = unpack('=LL', data[ptr:ptr+8])
+    timeFloat = np.float64(timeS)+np.float64(timeNs)*0.000000001 
+    return timeFloat, ptr+8
```

### Comparing `bimvee-1.0.9/bimvee/importRosbag/importRosbag/messageTypes/dvs_msgs_EventArray.py` & `bimvee-1.0.9.dev0/bimvee/importRosbag/importRosbag/messageTypes/dvs_msgs_EventArray.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-# -*- coding: utf-8 -*-
-
-"""
-Copyright (C) 2019 Event-driven Perception for Robotics
-Authors: Sim Bamford
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Intended as part of importRosbag.
-
-The importTopic function receives a list of messages and returns
-a dict with one field for each data field in the message, where the field
-will contain an appropriate iterable to contain the interpretted contents of each message.
-In some cases, static info is repeated in each message; in which case a field may not contain an iterable. 
-
-This function imports the ros message type defined at:
-https://github.com/uzh-rpg/rpg_dvs_ros/tree/master/dvs_msgs/msg
-"""
-
-#%%
-
-from tqdm import tqdm
-import numpy as np
-
-# local imports
-
-from .common import unpackRosString, unpackRosUint32
-
-def importTopic(msgs, **kwargs):
-
-    tsByMessage = []
-    xByMessage = []
-    yByMessage = []
-    polByMessage = []
-    for msg in tqdm(msgs, position=0, leave=True):
-        # TODO: maybe implement kwargs['useRosMsgTimestamps']
-        data = msg['data']
-        #seq = unpack('=L', data[0:4])[0]
-        #timeS, timeNs = unpack('=LL', data[4:12])
-        frame_id, ptr = unpackRosString(data, 12)
-        height, ptr = unpackRosUint32(data, ptr)
-        width, ptr = unpackRosUint32(data, ptr) 
-        numEventsInMsg, ptr = unpackRosUint32(data, ptr)
-        # The format of the event is x=Uint16, y=Uint16, ts = Uint32, tns (nano seconds) = Uint32, pol=Bool  
-        # Unpack in batch into uint8 and then compose
-        dataAsArray = np.frombuffer(data[ptr:ptr+numEventsInMsg*13], dtype=np.uint8)
-        dataAsArray = dataAsArray.reshape((-1, 13), order='C')
-        # Assuming big-endian
-        xByMessage.append((dataAsArray[:, 0] + dataAsArray[:, 1] * 2**8).astype(np.uint16))
-        yByMessage.append((dataAsArray[:, 2] + dataAsArray[:, 3] * 2**8).astype(np.uint16))
-        ts = ((dataAsArray[:, 4] + \
-              dataAsArray[:, 5] * 2**8 + \
-              dataAsArray[:, 6] * 2**16 + \
-              dataAsArray[:, 7] * 2**24 ).astype(np.float64))
-        tns = ((dataAsArray[:, 8] + \
-               dataAsArray[:, 9] * 2**8 + \
-               dataAsArray[:, 10] * 2**16 + \
-               dataAsArray[:, 11] * 2**24).astype(np.float64))
-        tsByMessage.append(ts + tns / 1000000000) # Combine timestamp parts, result is in seconds
-        polByMessage.append(dataAsArray[:, 12].astype(np.bool))
-    outDict = {
-        'x': np.concatenate(xByMessage),
-        'y': np.concatenate(yByMessage),
-        'ts': np.concatenate(tsByMessage),
-        'pol': np.concatenate(polByMessage),
-        'dimX': width,
-        'dimY': height}
-    return outDict
+# -*- coding: utf-8 -*-
+
+"""
+Copyright (C) 2019 Event-driven Perception for Robotics
+Authors: Sim Bamford
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Intended as part of importRosbag.
+
+The importTopic function receives a list of messages and returns
+a dict with one field for each data field in the message, where the field
+will contain an appropriate iterable to contain the interpretted contents of each message.
+In some cases, static info is repeated in each message; in which case a field may not contain an iterable. 
+
+This function imports the ros message type defined at:
+https://github.com/uzh-rpg/rpg_dvs_ros/tree/master/dvs_msgs/msg
+"""
+
+#%%
+
+from tqdm import tqdm
+import numpy as np
+
+# local imports
+
+from .common import unpackRosString, unpackRosUint32
+
+def importTopic(msgs, **kwargs):
+
+    tsByMessage = []
+    xByMessage = []
+    yByMessage = []
+    polByMessage = []
+    for msg in tqdm(msgs, position=0, leave=True):
+        # TODO: maybe implement kwargs['useRosMsgTimestamps']
+        data = msg['data']
+        #seq = unpack('=L', data[0:4])[0]
+        #timeS, timeNs = unpack('=LL', data[4:12])
+        frame_id, ptr = unpackRosString(data, 12)
+        height, ptr = unpackRosUint32(data, ptr)
+        width, ptr = unpackRosUint32(data, ptr) 
+        numEventsInMsg, ptr = unpackRosUint32(data, ptr)
+        # The format of the event is x=Uint16, y=Uint16, ts = Uint32, tns (nano seconds) = Uint32, pol=Bool  
+        # Unpack in batch into uint8 and then compose
+        dataAsArray = np.frombuffer(data[ptr:ptr+numEventsInMsg*13], dtype=np.uint8)
+        dataAsArray = dataAsArray.reshape((-1, 13), order='C')
+        # Assuming big-endian
+        xByMessage.append((dataAsArray[:, 0] + dataAsArray[:, 1] * 2**8).astype(np.uint16))
+        yByMessage.append((dataAsArray[:, 2] + dataAsArray[:, 3] * 2**8).astype(np.uint16))
+        ts = ((dataAsArray[:, 4] + \
+              dataAsArray[:, 5] * 2**8 + \
+              dataAsArray[:, 6] * 2**16 + \
+              dataAsArray[:, 7] * 2**24 ).astype(np.float64))
+        tns = ((dataAsArray[:, 8] + \
+               dataAsArray[:, 9] * 2**8 + \
+               dataAsArray[:, 10] * 2**16 + \
+               dataAsArray[:, 11] * 2**24).astype(np.float64))
+        tsByMessage.append(ts + tns / 1000000000) # Combine timestamp parts, result is in seconds
+        polByMessage.append(dataAsArray[:, 12].astype(np.bool))
+    outDict = {
+        'x': np.concatenate(xByMessage),
+        'y': np.concatenate(yByMessage),
+        'ts': np.concatenate(tsByMessage),
+        'pol': np.concatenate(polByMessage),
+        'dimX': width,
+        'dimY': height}
+    return outDict
```

### Comparing `bimvee-1.0.9/bimvee/importRosbag/importRosbag/messageTypes/esim_msgs_OpticFlow.py` & `bimvee-1.0.9.dev0/bimvee/importRosbag/importRosbag/messageTypes/esim_msgs_OpticFlow.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-# -*- coding: utf-8 -*-
-
-"""
-Copyright (C) 2019 Event-driven Perception for Robotics
-Authors: Sim Bamford
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Intended as part of importRosbag.
-
-The importRosbag function receives a list of messages and returns
-a dict with one field for each data field in the message, where the field
-will contain an appropriate iterable to contain the interpretted contents of each message.
-
-This function imports the ros message type defined at:
-
-https://github.com/uzh-rpg/rpg_esim/blob/master/event_camera_simulator/esim_msgs/msg/OpticFlow.msg
-
-"""
-
-#%%
-
-from tqdm import tqdm
-import numpy as np
-
-from .common import unpackRosFloat32Array, unpackRosUint32, \
-                    unpackRosTimestamp, unpackRosString
-
-def importTopic(msgs, **kwargs):
-
-    tsAll = []
-    flowMaps = []
-    for msg in tqdm(msgs):
-        
-        data = msg['data']
-        ptr = 0
-        seq, ptr = unpackRosUint32(data, ptr) # Not used
-        ts, ptr = unpackRosTimestamp(data, ptr)
-        frame_id, ptr = unpackRosString(data, ptr) # Not used
-        height, ptr = unpackRosUint32(data, ptr)
-        width, ptr = unpackRosUint32(data, ptr) 
-
-        if width > 0 and height > 0:
-            arraySize, ptr = unpackRosUint32(data, ptr)
-            #assert arraySize == width*height
-            flowMapX, ptr = unpackRosFloat32Array(data, width*height, ptr)
-            arraySize, ptr = unpackRosUint32(data, ptr)
-            #assert arraySize == width*height
-            flowMapY, ptr = unpackRosFloat32Array(data, width*height, ptr)
-            flowMap = np.concatenate((flowMapX.reshape(height, width, 1), 
-                                      flowMapY.reshape(height, width, 1)), 
-                                     axis=2)
-            flowMaps.append(flowMap)
-            tsAll.append(ts)
-    if not tsAll:
-        return None
-    outDict = {
-        'ts': np.array(tsAll, dtype=np.float64),
-        'flowMaps': flowMaps,
-        }
-    return outDict
-
-
+# -*- coding: utf-8 -*-
+
+"""
+Copyright (C) 2019 Event-driven Perception for Robotics
+Authors: Sim Bamford
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Intended as part of importRosbag.
+
+The importRosbag function receives a list of messages and returns
+a dict with one field for each data field in the message, where the field
+will contain an appropriate iterable to contain the interpretted contents of each message.
+
+This function imports the ros message type defined at:
+
+https://github.com/uzh-rpg/rpg_esim/blob/master/event_camera_simulator/esim_msgs/msg/OpticFlow.msg
+
+"""
+
+#%%
+
+from tqdm import tqdm
+import numpy as np
+
+from .common import unpackRosFloat32Array, unpackRosUint32, \
+                    unpackRosTimestamp, unpackRosString
+
+def importTopic(msgs, **kwargs):
+
+    tsAll = []
+    flowMaps = []
+    for msg in tqdm(msgs):
+        
+        data = msg['data']
+        ptr = 0
+        seq, ptr = unpackRosUint32(data, ptr) # Not used
+        ts, ptr = unpackRosTimestamp(data, ptr)
+        frame_id, ptr = unpackRosString(data, ptr) # Not used
+        height, ptr = unpackRosUint32(data, ptr)
+        width, ptr = unpackRosUint32(data, ptr) 
+
+        if width > 0 and height > 0:
+            arraySize, ptr = unpackRosUint32(data, ptr)
+            #assert arraySize == width*height
+            flowMapX, ptr = unpackRosFloat32Array(data, width*height, ptr)
+            arraySize, ptr = unpackRosUint32(data, ptr)
+            #assert arraySize == width*height
+            flowMapY, ptr = unpackRosFloat32Array(data, width*height, ptr)
+            flowMap = np.concatenate((flowMapX.reshape(height, width, 1), 
+                                      flowMapY.reshape(height, width, 1)), 
+                                     axis=2)
+            flowMaps.append(flowMap)
+            tsAll.append(ts)
+    if not tsAll:
+        return None
+    outDict = {
+        'ts': np.array(tsAll, dtype=np.float64),
+        'flowMaps': flowMaps,
+        }
+    return outDict
+
+
```

### Comparing `bimvee-1.0.9/bimvee/importRosbag/importRosbag/messageTypes/geometry_msgs_PoseStamped.py` & `bimvee-1.0.9.dev0/bimvee/importRosbag/importRosbag/messageTypes/geometry_msgs_PoseStamped.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-# -*- coding: utf-8 -*-
-
-"""
-Copyright (C) 2019 Event-driven Perception for Robotics
-Authors: Sim Bamford
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Intended as part of importRosbag.
-
-The importTopic function receives a list of messages and returns
-a dict with one field for each data field in the message, where the field
-will contain an appropriate iterable to contain the interpretted contents of each message.
-In some cases, static info is repeated in each message; in which case a field may not contain an iterable. 
-
-This function imports the ros message type defined at:    
-http://docs.ros.org/melodic/api/geometry_msgs/html/msg/PoseStamped.html
-
-The result is a ts plus a 7-column np array of np.float64,
-where the cols are x, y, z, q-w, q-x, q-y, q-z, (i.e. quaternion orientation)
-
-NOTE: QUATERNION ORDER GETS MODIFIED from xyzw to wxyz
-"""
-
-#%%
-
-from tqdm import tqdm
-import numpy as np
-
-from .common import unpackRosString, unpackRosTimestamp, unpackRosFloat64Array
-
-def importTopic(msgs, **kwargs):
-    #if 'Stamped' not in kwargs.get('messageType', 'Stamped'):
-    #    return interpretMsgsAsPose6qAlt(msgs, **kwargs)
-    sizeOfArray = 1024
-    tsAll = np.zeros((sizeOfArray), dtype=np.float64)
-    poseAll = np.zeros((sizeOfArray, 7), dtype=np.float64)
-    for idx, msg in enumerate(tqdm(msgs, position=0, leave=True)):
-        if sizeOfArray <= idx:
-            tsAll = np.append(tsAll, np.zeros((sizeOfArray), dtype=np.float64))
-            poseAll = np.concatenate((poseAll, np.zeros((sizeOfArray, 7), dtype=np.float64)))
-            sizeOfArray *= 2
-        # TODO: maybe implement kwargs['useRosMsgTimestamps']
-        data = msg['data']
-        #seq = unpack('=L', data[0:4])[0]
-        tsAll[idx], ptr = unpackRosTimestamp(data, 4)
-        frame_id, ptr = unpackRosString(data, ptr)
-        poseAll[idx, :], _ = unpackRosFloat64Array(data, 7, ptr)
-    # Crop arrays to number of events
-    numEvents = idx + 1
-    tsAll = tsAll[:numEvents]
-    poseAll = poseAll[:numEvents]
-    point = poseAll[:, 0:3]
-    rotation = poseAll[:, [6, 3, 4, 5]] # Switch quaternion form from xyzw to wxyz
-    outDict = {
-        'ts': tsAll,
-        'point': point,
-        'rotation': rotation}
-    return outDict
+# -*- coding: utf-8 -*-
+
+"""
+Copyright (C) 2019 Event-driven Perception for Robotics
+Authors: Sim Bamford
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Intended as part of importRosbag.
+
+The importTopic function receives a list of messages and returns
+a dict with one field for each data field in the message, where the field
+will contain an appropriate iterable to contain the interpretted contents of each message.
+In some cases, static info is repeated in each message; in which case a field may not contain an iterable. 
+
+This function imports the ros message type defined at:    
+http://docs.ros.org/melodic/api/geometry_msgs/html/msg/PoseStamped.html
+
+The result is a ts plus a 7-column np array of np.float64,
+where the cols are x, y, z, q-w, q-x, q-y, q-z, (i.e. quaternion orientation)
+
+NOTE: QUATERNION ORDER GETS MODIFIED from xyzw to wxyz
+"""
+
+#%%
+
+from tqdm import tqdm
+import numpy as np
+
+from .common import unpackRosString, unpackRosTimestamp, unpackRosFloat64Array
+
+def importTopic(msgs, **kwargs):
+    #if 'Stamped' not in kwargs.get('messageType', 'Stamped'):
+    #    return interpretMsgsAsPose6qAlt(msgs, **kwargs)
+    sizeOfArray = 1024
+    tsAll = np.zeros((sizeOfArray), dtype=np.float64)
+    poseAll = np.zeros((sizeOfArray, 7), dtype=np.float64)
+    for idx, msg in enumerate(tqdm(msgs, position=0, leave=True)):
+        if sizeOfArray <= idx:
+            tsAll = np.append(tsAll, np.zeros((sizeOfArray), dtype=np.float64))
+            poseAll = np.concatenate((poseAll, np.zeros((sizeOfArray, 7), dtype=np.float64)))
+            sizeOfArray *= 2
+        # TODO: maybe implement kwargs['useRosMsgTimestamps']
+        data = msg['data']
+        #seq = unpack('=L', data[0:4])[0]
+        tsAll[idx], ptr = unpackRosTimestamp(data, 4)
+        frame_id, ptr = unpackRosString(data, ptr)
+        poseAll[idx, :], _ = unpackRosFloat64Array(data, 7, ptr)
+    # Crop arrays to number of events
+    numEvents = idx + 1
+    tsAll = tsAll[:numEvents]
+    poseAll = poseAll[:numEvents]
+    point = poseAll[:, 0:3]
+    rotation = poseAll[:, [6, 3, 4, 5]] # Switch quaternion form from xyzw to wxyz
+    outDict = {
+        'ts': tsAll,
+        'point': point,
+        'rotation': rotation}
+    return outDict
```

### Comparing `bimvee-1.0.9/bimvee/importRosbag/importRosbag/messageTypes/geometry_msgs_Transform.py` & `bimvee-1.0.9.dev0/bimvee/importRosbag/importRosbag/messageTypes/geometry_msgs_Transform.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-# -*- coding: utf-8 -*-
-
-"""
-Copyright (C) 2019 Event-driven Perception for Robotics
-Authors: Sim Bamford
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Intended as part of importRosbag.
-
-The importTopic function receives a list of messages and returns
-a dict with one field for each data field in the message, where the field
-will contain an appropriate iterable to contain the interpretted contents of each message.
-In some cases, static info is repeated in each message; in which case a field may not contain an iterable. 
-
-This function imports the ros message type defined at:
-http://docs.ros.org/melodic/api/geometry_msgs/html/msg/Transform.html    
-"""
-
-#%%
-
-from tqdm import tqdm
-import numpy as np
-
-# Local imports
-
-from .common import unpackRosTimestamp, unpackRosFloat64Array
-
-def importTopic(msgs, **kwargs):
-    numEvents = 0
-    sizeOfArray = 1024
-    tsAll = np.zeros((sizeOfArray), dtype=np.float64)
-    poseAll = np.zeros((sizeOfArray, 7), dtype=np.float64)
-    for idx, msg in enumerate(tqdm(msgs, position=0, leave=True)):
-        if sizeOfArray <= idx:
-            tsAll = np.append(tsAll, np.zeros((sizeOfArray), dtype=np.float64))
-            poseAll = np.concatenate((poseAll, np.zeros((sizeOfArray, 7), dtype=np.float64)))
-            sizeOfArray *= 2
-        # Note - ignoring kwargs['useRosMsgTimestamps'] as there is no choice
-        tsAll[idx], _ = unpackRosTimestamp(msg['time'], 0)
-        poseAll[idx, :], _ = unpackRosFloat64Array(msg['data'], 7, 0)
-    numEvents = idx + 1
-    # Crop arrays to number of events
-    tsAll = tsAll[:numEvents]
-    
-    ''' Needed?
-    from timestamps import zeroTimestampsForAChannel, rezeroTimestampsForImportedDicts, unwrapTimestamps
-    tsAll = unwrapTimestamps(tsAll) # here we could pass in wrapTime=2**62, but actually it handles this internally
-    '''
-    poseAll = poseAll[:numEvents]
-    point = poseAll[:, 0:3]
-    rotation = poseAll[:, [6, 3, 4, 5]] # Switch quaternion form from xyzw to wxyz
-    outDict = {
-        'ts': tsAll,
-        'point': point,
-        'rotation': rotation}
-    return outDict
+# -*- coding: utf-8 -*-
+
+"""
+Copyright (C) 2019 Event-driven Perception for Robotics
+Authors: Sim Bamford
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Intended as part of importRosbag.
+
+The importTopic function receives a list of messages and returns
+a dict with one field for each data field in the message, where the field
+will contain an appropriate iterable to contain the interpretted contents of each message.
+In some cases, static info is repeated in each message; in which case a field may not contain an iterable. 
+
+This function imports the ros message type defined at:
+http://docs.ros.org/melodic/api/geometry_msgs/html/msg/Transform.html    
+"""
+
+#%%
+
+from tqdm import tqdm
+import numpy as np
+
+# Local imports
+
+from .common import unpackRosTimestamp, unpackRosFloat64Array
+
+def importTopic(msgs, **kwargs):
+    numEvents = 0
+    sizeOfArray = 1024
+    tsAll = np.zeros((sizeOfArray), dtype=np.float64)
+    poseAll = np.zeros((sizeOfArray, 7), dtype=np.float64)
+    for idx, msg in enumerate(tqdm(msgs, position=0, leave=True)):
+        if sizeOfArray <= idx:
+            tsAll = np.append(tsAll, np.zeros((sizeOfArray), dtype=np.float64))
+            poseAll = np.concatenate((poseAll, np.zeros((sizeOfArray, 7), dtype=np.float64)))
+            sizeOfArray *= 2
+        # Note - ignoring kwargs['useRosMsgTimestamps'] as there is no choice
+        tsAll[idx], _ = unpackRosTimestamp(msg['time'], 0)
+        poseAll[idx, :], _ = unpackRosFloat64Array(msg['data'], 7, 0)
+    numEvents = idx + 1
+    # Crop arrays to number of events
+    tsAll = tsAll[:numEvents]
+    
+    ''' Needed?
+    from timestamps import zeroTimestampsForAChannel, rezeroTimestampsForImportedDicts, unwrapTimestamps
+    tsAll = unwrapTimestamps(tsAll) # here we could pass in wrapTime=2**62, but actually it handles this internally
+    '''
+    poseAll = poseAll[:numEvents]
+    point = poseAll[:, 0:3]
+    rotation = poseAll[:, [6, 3, 4, 5]] # Switch quaternion form from xyzw to wxyz
+    outDict = {
+        'ts': tsAll,
+        'point': point,
+        'rotation': rotation}
+    return outDict
```

### Comparing `bimvee-1.0.9/bimvee/importRosbag/importRosbag/messageTypes/geometry_msgs_TransformStamped.py` & `bimvee-1.0.9.dev0/bimvee/importRosbag/importRosbag/messageTypes/geometry_msgs_TransformStamped.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-# -*- coding: utf-8 -*-
-
-"""
-Copyright (C) 2019 Event-driven Perception for Robotics
-Authors: Sim Bamford
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Intended as part of importRosbag.
-
-The importTopic function receives a list of messages and returns
-a dict with one field for each data field in the message, where the field
-will contain an appropriate iterable to contain the interpretted contents of each message.
-In some cases, static info is repeated in each message; in which case a field may not contain an iterable. 
-
-This function imports the ros message type defined at:    
-http://docs.ros.org/api/geometry_msgs/html/msg/TransformStamped.html
-
-The result is a ts plus a 7-column np array of np.float64,
-where the cols are x, y, z, q-w, q-x, q-y, q-z, (i.e. quaternion orientation)
-
-NOTE: QUATERNION ORDER GETS MODIFIED from xyzw to wxyz
-
-NOTE - this code is identical to geometry_msgs_PoseStamped
-"""
-
-#%%
-
-from tqdm import tqdm
-import numpy as np
-
-from .common import unpackRosString, unpackRosTimestamp, unpackRosFloat64Array
-
-def importTopic(msgs, **kwargs):
-    #if 'Stamped' not in kwargs.get('messageType', 'Stamped'):
-    #    return interpretMsgsAsPose6qAlt(msgs, **kwargs)
-    sizeOfArray = 1024
-    tsAll = np.zeros((sizeOfArray), dtype=np.float64)
-    poseAll = np.zeros((sizeOfArray, 7), dtype=np.float64)
-    for idx, msg in enumerate(tqdm(msgs, position=0, leave=True)):
-        if sizeOfArray <= idx:
-            tsAll = np.append(tsAll, np.zeros((sizeOfArray), dtype=np.float64))
-            poseAll = np.concatenate((poseAll, np.zeros((sizeOfArray, 7), dtype=np.float64)))
-            sizeOfArray *= 2
-        # TODO: maybe implement kwargs['useRosMsgTimestamps']
-        data = msg['data']
-        #seq = unpack('=L', data[0:4])[0]
-        tsAll[idx], ptr = unpackRosTimestamp(data, 4)
-        frame_id, ptr = unpackRosString(data, ptr)
-        poseAll[idx, :], _ = unpackRosFloat64Array(data, 7, ptr)
-    # Crop arrays to number of events
-    numEvents = idx + 1
-    tsAll = tsAll[:numEvents]
-    poseAll = poseAll[:numEvents]
-    point = poseAll[:, 0:3]
-    rotation = poseAll[:, [6, 3, 4, 5]] # Switch quaternion form from xyzw to wxyz
-    outDict = {
-        'ts': tsAll,
-        'point': point,
-        'rotation': rotation}
-    return outDict
+# -*- coding: utf-8 -*-
+
+"""
+Copyright (C) 2019 Event-driven Perception for Robotics
+Authors: Sim Bamford
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Intended as part of importRosbag.
+
+The importTopic function receives a list of messages and returns
+a dict with one field for each data field in the message, where the field
+will contain an appropriate iterable to contain the interpretted contents of each message.
+In some cases, static info is repeated in each message; in which case a field may not contain an iterable. 
+
+This function imports the ros message type defined at:    
+http://docs.ros.org/api/geometry_msgs/html/msg/TransformStamped.html
+
+The result is a ts plus a 7-column np array of np.float64,
+where the cols are x, y, z, q-w, q-x, q-y, q-z, (i.e. quaternion orientation)
+
+NOTE: QUATERNION ORDER GETS MODIFIED from xyzw to wxyz
+
+NOTE - this code is identical to geometry_msgs_PoseStamped
+"""
+
+#%%
+
+from tqdm import tqdm
+import numpy as np
+
+from .common import unpackRosString, unpackRosTimestamp, unpackRosFloat64Array
+
+def importTopic(msgs, **kwargs):
+    #if 'Stamped' not in kwargs.get('messageType', 'Stamped'):
+    #    return interpretMsgsAsPose6qAlt(msgs, **kwargs)
+    sizeOfArray = 1024
+    tsAll = np.zeros((sizeOfArray), dtype=np.float64)
+    poseAll = np.zeros((sizeOfArray, 7), dtype=np.float64)
+    for idx, msg in enumerate(tqdm(msgs, position=0, leave=True)):
+        if sizeOfArray <= idx:
+            tsAll = np.append(tsAll, np.zeros((sizeOfArray), dtype=np.float64))
+            poseAll = np.concatenate((poseAll, np.zeros((sizeOfArray, 7), dtype=np.float64)))
+            sizeOfArray *= 2
+        # TODO: maybe implement kwargs['useRosMsgTimestamps']
+        data = msg['data']
+        #seq = unpack('=L', data[0:4])[0]
+        tsAll[idx], ptr = unpackRosTimestamp(data, 4)
+        frame_id, ptr = unpackRosString(data, ptr)
+        poseAll[idx, :], _ = unpackRosFloat64Array(data, 7, ptr)
+    # Crop arrays to number of events
+    numEvents = idx + 1
+    tsAll = tsAll[:numEvents]
+    poseAll = poseAll[:numEvents]
+    point = poseAll[:, 0:3]
+    rotation = poseAll[:, [6, 3, 4, 5]] # Switch quaternion form from xyzw to wxyz
+    outDict = {
+        'ts': tsAll,
+        'point': point,
+        'rotation': rotation}
+    return outDict
```

### Comparing `bimvee-1.0.9/bimvee/importRosbag/importRosbag/messageTypes/geometry_msgs_TwistStamped.py` & `bimvee-1.0.9.dev0/bimvee/importRosbag/importRosbag/messageTypes/geometry_msgs_TwistStamped.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-# -*- coding: utf-8 -*-
-
-"""
-Copyright (C) 2019 Event-driven Perception for Robotics
-Authors: Sim Bamford
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Intended as part of importRosbag.
-
-The interpretMessages function receives a list of messages and returns
-a dict with one field for each data field in the message, where the field
-will contain an appropriate iterable to contain the interpretted contents of each message.
-
-This function imports the ros message type defined at:
-http://docs.ros.org/melodic/api/geometry_msgs/html/msg/TwistStamped.html
-"""
-
-#%%
-
-from tqdm import tqdm
-import numpy as np
-
-from .common import unpackRosString, unpackRosTimestamp, unpackRosFloat64Array
-
-def importTopic(msgs, **kwargs):
-    sizeOfArray = 1024
-    ts = np.zeros((sizeOfArray), dtype=np.float64)
-    linV = np.zeros((sizeOfArray, 3), dtype=np.float64)
-    angV = np.zeros((sizeOfArray, 3), dtype=np.float64)
-    for idx, msg in enumerate(tqdm(msgs, position=0, leave=True)):
-        if sizeOfArray <= idx:
-            ts = np.append(ts, np.zeros((sizeOfArray), dtype=np.float64))
-            linV = np.concatenate((linV, np.zeros((sizeOfArray, 3), dtype=np.float64)))
-            angV = np.concatenate((angV, np.zeros((sizeOfArray, 3), dtype=np.float64)))
-            sizeOfArray *= 2
-        data = msg['data']
-        #seq = unpack('=L', data[0:4])[0]
-        ts[idx], ptr = unpackRosTimestamp(data, 4)
-        frame_id, ptr = unpackRosString(data, ptr)
-        linV[idx, :], ptr = unpackRosFloat64Array(data, 3, ptr)
-        angV[idx, :], _ = unpackRosFloat64Array(data, 3, ptr)
-    # Crop arrays to number of events
-    numEvents = idx + 1
-    ts = ts[:numEvents]
-    linV = linV[:numEvents]
-    angV = angV[:numEvents]
-    outDict = {
-        'ts': ts,
-        'linV': linV,
-        'angV': angV}
-    return outDict
-
+# -*- coding: utf-8 -*-
+
+"""
+Copyright (C) 2019 Event-driven Perception for Robotics
+Authors: Sim Bamford
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Intended as part of importRosbag.
+
+The interpretMessages function receives a list of messages and returns
+a dict with one field for each data field in the message, where the field
+will contain an appropriate iterable to contain the interpretted contents of each message.
+
+This function imports the ros message type defined at:
+http://docs.ros.org/melodic/api/geometry_msgs/html/msg/TwistStamped.html
+"""
+
+#%%
+
+from tqdm import tqdm
+import numpy as np
+
+from .common import unpackRosString, unpackRosTimestamp, unpackRosFloat64Array
+
+def importTopic(msgs, **kwargs):
+    sizeOfArray = 1024
+    ts = np.zeros((sizeOfArray), dtype=np.float64)
+    linV = np.zeros((sizeOfArray, 3), dtype=np.float64)
+    angV = np.zeros((sizeOfArray, 3), dtype=np.float64)
+    for idx, msg in enumerate(tqdm(msgs, position=0, leave=True)):
+        if sizeOfArray <= idx:
+            ts = np.append(ts, np.zeros((sizeOfArray), dtype=np.float64))
+            linV = np.concatenate((linV, np.zeros((sizeOfArray, 3), dtype=np.float64)))
+            angV = np.concatenate((angV, np.zeros((sizeOfArray, 3), dtype=np.float64)))
+            sizeOfArray *= 2
+        data = msg['data']
+        #seq = unpack('=L', data[0:4])[0]
+        ts[idx], ptr = unpackRosTimestamp(data, 4)
+        frame_id, ptr = unpackRosString(data, ptr)
+        linV[idx, :], ptr = unpackRosFloat64Array(data, 3, ptr)
+        angV[idx, :], _ = unpackRosFloat64Array(data, 3, ptr)
+    # Crop arrays to number of events
+    numEvents = idx + 1
+    ts = ts[:numEvents]
+    linV = linV[:numEvents]
+    angV = angV[:numEvents]
+    outDict = {
+        'ts': ts,
+        'linV': linV,
+        'angV': angV}
+    return outDict
+
```

### Comparing `bimvee-1.0.9/bimvee/importRosbag/importRosbag/messageTypes/sensor_msgs_CameraInfo.py` & `bimvee-1.0.9.dev0/bimvee/importRosbag/importRosbag/messageTypes/sensor_msgs_CameraInfo.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-# -*- coding: utf-8 -*-
-
-"""
-Copyright (C) 2019 Event-driven Perception for Robotics
-Authors: Sim Bamford
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Intended as part of importRosbag.
-
-The importTopic function receives a list of messages and returns
-a dict with one field for each data field in the message, where the field
-will contain an appropriate iterable to contain the interpretted contents of each message.
-In some cases, static info is repeated in each message; in which case a field may not contain an iterable. 
-
-This function imports the ros message type defined at:
-
-http://docs.ros.org/api/sensor_msgs/html/msg/CameraInfo.html
-We assume that there will only be one camera_info msg per channel,
-so the resulting dict is populated by the following fields:
-    std_msgs/Header header
-    uint32 height
-    uint32 width
-    string distortion_model
-    <following as numpy matrices of the appropriate dimensions>
-    float64[] D (distortion params)
-    float64[9] K (Intrinsic camera matrix)
-    float64[9] R (rectification matrix - only for stereo setup)
-    float64[12] P (projection matrix)
-    <ignoring the following for now:>
-    uint32 binning_x
-    uint32 binning_y
-    sensor_msgs/RegionOfInterest roi
-
-"""
-
-#%%
-
-from .common import unpackRosString, unpackRosUint32, unpackRosFloat64Array
-
-def importTopic(msgs, **kwargs):
-
-    outDict = {}
-    data = msgs[0]['data'] # There is one calibration msg per frame. 
-    # Just use the first one
-    #seq = unpack('=L', data[0:4])[0]
-    #timeS, timeNs = unpack('=LL', data[4:12])
-    frame_id, ptr = unpackRosString(data, 12)
-    outDict['height'], ptr = unpackRosUint32(data, ptr)
-    outDict['width'], ptr = unpackRosUint32(data, ptr)
-    outDict['distortionModel'], ptr = unpackRosString(data, ptr)
-    numElementsInD, ptr = unpackRosUint32(data, ptr)
-    outDict['D'], ptr = unpackRosFloat64Array(data, numElementsInD, ptr)
-    outDict['K'], ptr = unpackRosFloat64Array(data, 9, ptr)
-    outDict['K'] = outDict['K'].reshape(3, 3)
-    outDict['R'], ptr = unpackRosFloat64Array(data, 9, ptr)
-    outDict['R'] = outDict['R'].reshape(3, 3)
-    outDict['P'], ptr = unpackRosFloat64Array(data, 12, ptr)
-    outDict['P'] = outDict['P'].reshape(3, 4)
-    # Ignore binning and ROI
-    return outDict
+# -*- coding: utf-8 -*-
+
+"""
+Copyright (C) 2019 Event-driven Perception for Robotics
+Authors: Sim Bamford
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Intended as part of importRosbag.
+
+The importTopic function receives a list of messages and returns
+a dict with one field for each data field in the message, where the field
+will contain an appropriate iterable to contain the interpretted contents of each message.
+In some cases, static info is repeated in each message; in which case a field may not contain an iterable. 
+
+This function imports the ros message type defined at:
+
+http://docs.ros.org/api/sensor_msgs/html/msg/CameraInfo.html
+We assume that there will only be one camera_info msg per channel,
+so the resulting dict is populated by the following fields:
+    std_msgs/Header header
+    uint32 height
+    uint32 width
+    string distortion_model
+    <following as numpy matrices of the appropriate dimensions>
+    float64[] D (distortion params)
+    float64[9] K (Intrinsic camera matrix)
+    float64[9] R (rectification matrix - only for stereo setup)
+    float64[12] P (projection matrix)
+    <ignoring the following for now:>
+    uint32 binning_x
+    uint32 binning_y
+    sensor_msgs/RegionOfInterest roi
+
+"""
+
+#%%
+
+from .common import unpackRosString, unpackRosUint32, unpackRosFloat64Array
+
+def importTopic(msgs, **kwargs):
+
+    outDict = {}
+    data = msgs[0]['data'] # There is one calibration msg per frame. 
+    # Just use the first one
+    #seq = unpack('=L', data[0:4])[0]
+    #timeS, timeNs = unpack('=LL', data[4:12])
+    frame_id, ptr = unpackRosString(data, 12)
+    outDict['height'], ptr = unpackRosUint32(data, ptr)
+    outDict['width'], ptr = unpackRosUint32(data, ptr)
+    outDict['distortionModel'], ptr = unpackRosString(data, ptr)
+    numElementsInD, ptr = unpackRosUint32(data, ptr)
+    outDict['D'], ptr = unpackRosFloat64Array(data, numElementsInD, ptr)
+    outDict['K'], ptr = unpackRosFloat64Array(data, 9, ptr)
+    outDict['K'] = outDict['K'].reshape(3, 3)
+    outDict['R'], ptr = unpackRosFloat64Array(data, 9, ptr)
+    outDict['R'] = outDict['R'].reshape(3, 3)
+    outDict['P'], ptr = unpackRosFloat64Array(data, 12, ptr)
+    outDict['P'] = outDict['P'].reshape(3, 4)
+    # Ignore binning and ROI
+    return outDict
```

### Comparing `bimvee-1.0.9/bimvee/importRosbag/importRosbag/messageTypes/sensor_msgs_Imu.py` & `bimvee-1.0.9.dev0/bimvee/importRosbag/importRosbag/messageTypes/sensor_msgs_Imu.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-# -*- coding: utf-8 -*-
-
-"""
-Copyright (C) 2019 Event-driven Perception for Robotics
-Authors: Sim Bamford
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Intended as part of importRosbag.
-
-The importTopic function receives a list of messages and returns
-a dict with one field for each data field in the message, where the field
-will contain an appropriate iterable to contain the interpretted contents of each message.
-In some cases, static info is repeated in each message; in which case a field may not contain an iterable. 
-
-This function imports the ros message type defined at:
-http://docs.ros.org/api/sensor_msgs/html/msg/Imu.html
-"""
-
-#%%
-
-from tqdm import tqdm
-import numpy as np
-
-from .common import unpackRosString, unpackRosTimestamp, unpackRosFloat64Array
-
-def importTopic(msgs, **kwargs):
-    '''
-    ros message is defined here:
-        http://docs.ros.org/api/geometry_msgs/html/msg/PoseStamped.html
-    the result is are np arrays of float64 for:
-        rotQ (4 cols, quaternion)
-        angV (3 cols)
-        acc (3 cols)
-        mag (3 cols)
-        temp (1 cols) - but I'll probably ignore this to start with
-    '''
-    sizeOfArray = 1024
-    tsAll = np.zeros((sizeOfArray), dtype=np.float64)
-    rotQAll = np.zeros((sizeOfArray, 4), dtype=np.float64)
-    angVAll = np.zeros((sizeOfArray, 3), dtype=np.float64)
-    accAll = np.zeros((sizeOfArray, 3), dtype=np.float64)
-    magAll = np.zeros((sizeOfArray, 3), dtype=np.float64)
-    #tempAll = np.zeros((sizeOfArray, 1), dtype=np.float64)
-    for idx, msg in enumerate(tqdm(msgs, position=0, leave=True)):
-        if sizeOfArray <= idx:
-            tsAll = np.append(tsAll, np.zeros((sizeOfArray), dtype=np.float64))
-            rotQAll = np.concatenate((rotQAll, np.zeros((sizeOfArray, 4), dtype=np.float64)))
-            angVAll = np.concatenate((angVAll, np.zeros((sizeOfArray, 3), dtype=np.float64)))
-            accAll = np.concatenate((accAll, np.zeros((sizeOfArray, 3), dtype=np.float64)))
-            magAll = np.concatenate((magAll, np.zeros((sizeOfArray, 3), dtype=np.float64)))
-            sizeOfArray *= 2
-        # TODO: maybe implement kwargs['useRosMsgTimestamps']
-        data = msg['data']
-        #seq = unpack('=L', data[0:4])[0]
-        tsAll[idx], ptr = unpackRosTimestamp(data, 4)
-        frame_id, ptr = unpackRosString(data, ptr)
-        rotQAll[idx, :], ptr = unpackRosFloat64Array(data, 4, ptr)
-        ptr += 72 # Skip the covariance matrix
-        angVAll[idx, :], ptr = unpackRosFloat64Array(data, 3, ptr)
-        ptr += 72 # Skip the covariance matrix
-        accAll[idx, :], ptr = unpackRosFloat64Array(data, 3, ptr)
-        #ptr += 24
-        #ptr += 72 # Skip the covariance matrix
-    numEvents = idx + 1
-    # Crop arrays to number of events
-    tsAll = tsAll[:numEvents]
-    rotQAll = rotQAll[:numEvents]
-    angVAll = angVAll[:numEvents]
-    accAll = accAll[:numEvents]
-    magAll = magAll[:numEvents]
-    outDict = {
-        'ts': tsAll,
-        'rotQ': rotQAll,
-        'angV': angVAll,
-        'acc': accAll,
-        'mag': magAll
-        }
-    return outDict
+# -*- coding: utf-8 -*-
+
+"""
+Copyright (C) 2019 Event-driven Perception for Robotics
+Authors: Sim Bamford
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Intended as part of importRosbag.
+
+The importTopic function receives a list of messages and returns
+a dict with one field for each data field in the message, where the field
+will contain an appropriate iterable to contain the interpretted contents of each message.
+In some cases, static info is repeated in each message; in which case a field may not contain an iterable. 
+
+This function imports the ros message type defined at:
+http://docs.ros.org/api/sensor_msgs/html/msg/Imu.html
+"""
+
+#%%
+
+from tqdm import tqdm
+import numpy as np
+
+from .common import unpackRosString, unpackRosTimestamp, unpackRosFloat64Array
+
+def importTopic(msgs, **kwargs):
+    '''
+    ros message is defined here:
+        http://docs.ros.org/api/geometry_msgs/html/msg/PoseStamped.html
+    the result is are np arrays of float64 for:
+        rotQ (4 cols, quaternion)
+        angV (3 cols)
+        acc (3 cols)
+        mag (3 cols)
+        temp (1 cols) - but I'll probably ignore this to start with
+    '''
+    sizeOfArray = 1024
+    tsAll = np.zeros((sizeOfArray), dtype=np.float64)
+    rotQAll = np.zeros((sizeOfArray, 4), dtype=np.float64)
+    angVAll = np.zeros((sizeOfArray, 3), dtype=np.float64)
+    accAll = np.zeros((sizeOfArray, 3), dtype=np.float64)
+    magAll = np.zeros((sizeOfArray, 3), dtype=np.float64)
+    #tempAll = np.zeros((sizeOfArray, 1), dtype=np.float64)
+    for idx, msg in enumerate(tqdm(msgs, position=0, leave=True)):
+        if sizeOfArray <= idx:
+            tsAll = np.append(tsAll, np.zeros((sizeOfArray), dtype=np.float64))
+            rotQAll = np.concatenate((rotQAll, np.zeros((sizeOfArray, 4), dtype=np.float64)))
+            angVAll = np.concatenate((angVAll, np.zeros((sizeOfArray, 3), dtype=np.float64)))
+            accAll = np.concatenate((accAll, np.zeros((sizeOfArray, 3), dtype=np.float64)))
+            magAll = np.concatenate((magAll, np.zeros((sizeOfArray, 3), dtype=np.float64)))
+            sizeOfArray *= 2
+        # TODO: maybe implement kwargs['useRosMsgTimestamps']
+        data = msg['data']
+        #seq = unpack('=L', data[0:4])[0]
+        tsAll[idx], ptr = unpackRosTimestamp(data, 4)
+        frame_id, ptr = unpackRosString(data, ptr)
+        rotQAll[idx, :], ptr = unpackRosFloat64Array(data, 4, ptr)
+        ptr += 72 # Skip the covariance matrix
+        angVAll[idx, :], ptr = unpackRosFloat64Array(data, 3, ptr)
+        ptr += 72 # Skip the covariance matrix
+        accAll[idx, :], ptr = unpackRosFloat64Array(data, 3, ptr)
+        #ptr += 24
+        #ptr += 72 # Skip the covariance matrix
+    numEvents = idx + 1
+    # Crop arrays to number of events
+    tsAll = tsAll[:numEvents]
+    rotQAll = rotQAll[:numEvents]
+    angVAll = angVAll[:numEvents]
+    accAll = accAll[:numEvents]
+    magAll = magAll[:numEvents]
+    outDict = {
+        'ts': tsAll,
+        'rotQ': rotQAll,
+        'angV': angVAll,
+        'acc': accAll,
+        'mag': magAll
+        }
+    return outDict
```

### Comparing `bimvee-1.0.9/bimvee/importRosbag/importRosbag/messageTypes/sensor_msgs_PointCloud2.py` & `bimvee-1.0.9.dev0/bimvee/importRosbag/importRosbag/messageTypes/sensor_msgs_PointCloud2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-# -*- coding: utf-8 -*-
-
-"""
-Copyright (C) 2019 Event-driven Perception for Robotics
-Authors: Sim Bamford
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Intended as part of importRosbag.
-
-The importTopic function receives a list of messages and returns
-a dict with one field for each data field in the message, where the field
-will contain an appropriate iterable to contain the interpretted contents of each message.
-In some cases, static info is repeated in each message; in which case a field may not contain an iterable. 
-
-This function imports the ros message type defined at:
-http://docs.ros.org/api/sensor_msgs/html/msg/PointCloud2.html
-
-For simplicity, we're currently directly unpacking the format that we are 
-encountering in the data, which is x,y,z,_,rgb,_,_,_ 
-each as 32-bit little-endian floats
-"""
-
-#%%
-
-
-from tqdm import tqdm
-import numpy as np
-
-from .common import unpackRosString, unpackRosUint8, unpackRosUint32, \
-                    unpackRosTimestamp
-
-def importTopic(msgs, **kwargs):
-    '''
-    ros message is defined here:
-        http://docs.ros.org/api/geometry_msgs/html/msg/PoseStamped.html
-    the result is are np arrays of float64 for:
-        rotQ (4 cols, quaternion)
-        angV (3 cols)
-        acc (3 cols)
-        mag (3 cols)
-        temp (1 cols) - but I'll probably ignore this to start with
-    '''
-    #tempAll = np.zeros((sizeOfArray, 1), dtype=np.float64)
-    #for msg in tqdm(msgs, position=0, leave=True):
-    tsByMessage = []
-    pointsByMessage = []
-    for msg in tqdm(msgs):
-        
-        data = msg['data']
-        ptr = 0
-        seq, ptr = unpackRosUint32(data, ptr)
-        ts, ptr = unpackRosTimestamp(data, ptr)
-        frame_id, ptr = unpackRosString(data, ptr)
-        height, ptr = unpackRosUint32(data, ptr)
-        width, ptr = unpackRosUint32(data, ptr) 
-
-        if width > 0 and height > 0:
-
-            arraySize, ptr = unpackRosUint32(data, ptr)
-            for element in range(arraySize):
-                # Move through the field definitions - we'll ignore these
-                # until we encounter a file that uses a different set
-                name, ptr = unpackRosString(data, ptr)
-                offset, ptr = unpackRosUint32(data, ptr)
-                datatype, ptr = unpackRosUint8(data, ptr)
-                count, ptr = unpackRosUint32(data, ptr)
-        
-            isBigendian, ptr = unpackRosUint8(data, ptr)
-            pointStep, ptr = unpackRosUint32(data, ptr)
-            rowStep, ptr = unpackRosUint32(data, ptr)
-
-            numPoints = width * height
-            points = np.empty((numPoints, 3), dtype=np.float32)
-            arraySize, ptr = unpackRosUint32(data, ptr)
-            # assert arraySize = width*height
-            for x in range(width):
-                for y in range(height):            
-                    points[x*height + y, :] = np.frombuffer(data[ptr:ptr+12], dtype=np.float32)
-                    ptr += 32 
-            pointsByMessage.append(points)
-            tsByMessage.append(np.ones((numPoints), dtype=np.float64) * ts)
-    if not pointsByMessage: # None of the messages contained any points
-        return None
-    points = np.concatenate(pointsByMessage)        
-    ts = np.concatenate(tsByMessage)        
-    
-    # Crop arrays to number of events
-    outDict = {
-        'ts': ts,
-        'point': points,
-        }
-    return outDict
+# -*- coding: utf-8 -*-
+
+"""
+Copyright (C) 2019 Event-driven Perception for Robotics
+Authors: Sim Bamford
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Intended as part of importRosbag.
+
+The importTopic function receives a list of messages and returns
+a dict with one field for each data field in the message, where the field
+will contain an appropriate iterable to contain the interpretted contents of each message.
+In some cases, static info is repeated in each message; in which case a field may not contain an iterable. 
+
+This function imports the ros message type defined at:
+http://docs.ros.org/api/sensor_msgs/html/msg/PointCloud2.html
+
+For simplicity, we're currently directly unpacking the format that we are 
+encountering in the data, which is x,y,z,_,rgb,_,_,_ 
+each as 32-bit little-endian floats
+"""
+
+#%%
+
+
+from tqdm import tqdm
+import numpy as np
+
+from .common import unpackRosString, unpackRosUint8, unpackRosUint32, \
+                    unpackRosTimestamp
+
+def importTopic(msgs, **kwargs):
+    '''
+    ros message is defined here:
+        http://docs.ros.org/api/geometry_msgs/html/msg/PoseStamped.html
+    the result is are np arrays of float64 for:
+        rotQ (4 cols, quaternion)
+        angV (3 cols)
+        acc (3 cols)
+        mag (3 cols)
+        temp (1 cols) - but I'll probably ignore this to start with
+    '''
+    #tempAll = np.zeros((sizeOfArray, 1), dtype=np.float64)
+    #for msg in tqdm(msgs, position=0, leave=True):
+    tsByMessage = []
+    pointsByMessage = []
+    for msg in tqdm(msgs):
+        
+        data = msg['data']
+        ptr = 0
+        seq, ptr = unpackRosUint32(data, ptr)
+        ts, ptr = unpackRosTimestamp(data, ptr)
+        frame_id, ptr = unpackRosString(data, ptr)
+        height, ptr = unpackRosUint32(data, ptr)
+        width, ptr = unpackRosUint32(data, ptr) 
+
+        if width > 0 and height > 0:
+
+            arraySize, ptr = unpackRosUint32(data, ptr)
+            for element in range(arraySize):
+                # Move through the field definitions - we'll ignore these
+                # until we encounter a file that uses a different set
+                name, ptr = unpackRosString(data, ptr)
+                offset, ptr = unpackRosUint32(data, ptr)
+                datatype, ptr = unpackRosUint8(data, ptr)
+                count, ptr = unpackRosUint32(data, ptr)
+        
+            isBigendian, ptr = unpackRosUint8(data, ptr)
+            pointStep, ptr = unpackRosUint32(data, ptr)
+            rowStep, ptr = unpackRosUint32(data, ptr)
+
+            numPoints = width * height
+            points = np.empty((numPoints, 3), dtype=np.float32)
+            arraySize, ptr = unpackRosUint32(data, ptr)
+            # assert arraySize = width*height
+            for x in range(width):
+                for y in range(height):            
+                    points[x*height + y, :] = np.frombuffer(data[ptr:ptr+12], dtype=np.float32)
+                    ptr += pointStep
+            pointsByMessage.append(points)
+            tsByMessage.append(np.ones((numPoints), dtype=np.float64) * ts)
+    if not pointsByMessage: # None of the messages contained any points
+        return None
+    points = np.concatenate(pointsByMessage)        
+    ts = np.concatenate(tsByMessage)        
+    
+    # Crop arrays to number of events
+    outDict = {
+        'ts': ts,
+        'point': points,
+        }
+    return outDict
```

### Comparing `bimvee-1.0.9/bimvee/importRosbag/importRosbag/messageTypes/tf_tfMessage.py` & `bimvee-1.0.9.dev0/bimvee/importRosbag/importRosbag/messageTypes/tf_tfMessage.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-# -*- coding: utf-8 -*-
-
-"""
-Copyright (C) 2019 Event-driven Perception for Robotics
-Authors: Sim Bamford
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Intended as part of importRosbag.
-
-The importTopic function receives a list of messages and returns
-a dict with one field for each data field in the message, where the field
-will contain an appropriate iterable to contain the interpretted contents of each message.
-In some cases, static info is repeated in each message; in which case a field may not contain an iterable. 
-
-This function imports the ros message type defined at:    
-http://docs.ros.org/api/tf/html/msg/tfMessage.html
-
-Each message contains an array of transform_stamped messages
-
-The result is a ts plus a 7-column np array of np.float64,
-where the cols are x, y, z, q-w, q-x, q-y, q-z, (i.e. quaternion orientation)
-
-NOTE: QUATERNION ORDER GETS MODIFIED from xyzw to wxyz
-
-NOTE - this code is similar to geometry_msgs_TransformStamped
-"""
-
-#%%
-
-from tqdm import tqdm
-import numpy as np
-
-from .common import unpackRosString, unpackRosTimestamp, \
-                    unpackRosFloat64Array, unpackRosUint32
-
-def importTopic(msgs, **kwargs):
-    #if 'Stamped' not in kwargs.get('messageType', 'Stamped'):
-    #    return interpretMsgsAsPose6qAlt(msgs, **kwargs)
-    sizeOfArray = 1024
-    tsAll = np.zeros((sizeOfArray), dtype=np.float64)
-    poseAll = np.zeros((sizeOfArray, 7), dtype=np.float64)
-    frameIdAll = []
-    childFrameIdAll = []
-    idx = 0
-    for msg in tqdm(msgs, position=0, leave=True):
-        data = msg['data']
-        numTfInMsg, ptr = unpackRosUint32(data, 0)
-        for tfIdx in range(numTfInMsg): 
-            while sizeOfArray <= idx + numTfInMsg:
-                tsAll = np.append(tsAll, np.zeros((sizeOfArray), dtype=np.float64))
-                poseAll = np.concatenate((poseAll, np.zeros((sizeOfArray, 7), dtype=np.float64)))
-                sizeOfArray *= 2
-            seq, ptr = unpackRosUint32(data, ptr)
-            tsAll[idx], ptr = unpackRosTimestamp(data, ptr)
-            frame_id, ptr = unpackRosString(data, ptr)
-            frameIdAll.append(frame_id)
-            child_frame_id, ptr = unpackRosString(data, ptr)
-            childFrameIdAll.append(child_frame_id)
-            poseAll[idx, :], ptr = unpackRosFloat64Array(data, 7, ptr)
-            idx += 1
-    # Crop arrays to number of events
-    numEvents = idx
-    tsAll = tsAll[:numEvents]
-    poseAll = poseAll[:numEvents]
-    point = poseAll[:, 0:3]
-    rotation = poseAll[:, [6, 3, 4, 5]] # Switch quaternion form from xyzw to wxyz
-    outDict = {
-        'ts': tsAll,
-        'point': point,
-        'rotation': rotation,
-        'frameId': np.array(frameIdAll, dtype='object'),
-        'childFrameId': np.array(childFrameIdAll, dtype='object')}
-    return outDict
+# -*- coding: utf-8 -*-
+
+"""
+Copyright (C) 2019 Event-driven Perception for Robotics
+Authors: Sim Bamford
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Intended as part of importRosbag.
+
+The importTopic function receives a list of messages and returns
+a dict with one field for each data field in the message, where the field
+will contain an appropriate iterable to contain the interpretted contents of each message.
+In some cases, static info is repeated in each message; in which case a field may not contain an iterable. 
+
+This function imports the ros message type defined at:    
+http://docs.ros.org/api/tf/html/msg/tfMessage.html
+
+Each message contains an array of transform_stamped messages
+
+The result is a ts plus a 7-column np array of np.float64,
+where the cols are x, y, z, q-w, q-x, q-y, q-z, (i.e. quaternion orientation)
+
+NOTE: QUATERNION ORDER GETS MODIFIED from xyzw to wxyz
+
+NOTE - this code is similar to geometry_msgs_TransformStamped
+"""
+
+#%%
+
+from tqdm import tqdm
+import numpy as np
+
+from .common import unpackRosString, unpackRosTimestamp, \
+                    unpackRosFloat64Array, unpackRosUint32
+
+def importTopic(msgs, **kwargs):
+    #if 'Stamped' not in kwargs.get('messageType', 'Stamped'):
+    #    return interpretMsgsAsPose6qAlt(msgs, **kwargs)
+    sizeOfArray = 1024
+    tsAll = np.zeros((sizeOfArray), dtype=np.float64)
+    poseAll = np.zeros((sizeOfArray, 7), dtype=np.float64)
+    frameIdAll = []
+    childFrameIdAll = []
+    idx = 0
+    for msg in tqdm(msgs, position=0, leave=True):
+        data = msg['data']
+        numTfInMsg, ptr = unpackRosUint32(data, 0)
+        for tfIdx in range(numTfInMsg): 
+            while sizeOfArray <= idx + numTfInMsg:
+                tsAll = np.append(tsAll, np.zeros((sizeOfArray), dtype=np.float64))
+                poseAll = np.concatenate((poseAll, np.zeros((sizeOfArray, 7), dtype=np.float64)))
+                sizeOfArray *= 2
+            seq, ptr = unpackRosUint32(data, ptr)
+            tsAll[idx], ptr = unpackRosTimestamp(data, ptr)
+            frame_id, ptr = unpackRosString(data, ptr)
+            frameIdAll.append(frame_id)
+            child_frame_id, ptr = unpackRosString(data, ptr)
+            childFrameIdAll.append(child_frame_id)
+            poseAll[idx, :], ptr = unpackRosFloat64Array(data, 7, ptr)
+            idx += 1
+    # Crop arrays to number of events
+    numEvents = idx
+    tsAll = tsAll[:numEvents]
+    poseAll = poseAll[:numEvents]
+    point = poseAll[:, 0:3]
+    rotation = poseAll[:, [6, 3, 4, 5]] # Switch quaternion form from xyzw to wxyz
+    outDict = {
+        'ts': tsAll,
+        'point': point,
+        'rotation': rotation,
+        'frameId': np.array(frameIdAll, dtype='object'),
+        'childFrameId': np.array(childFrameIdAll, dtype='object')}
+    return outDict
```

### Comparing `bimvee-1.0.9/bimvee/importRpgDvsRos.py` & `bimvee-1.0.9.dev0/bimvee/importRpgDvsRos.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,141 +1,142 @@
-# -*- coding: utf-8 -*-
-
-"""https://github.com/event-driven-robotics/importRosbag
-Copyright (C) 2019 Event-driven Perception for Robotics
-Authors: Sim Bamford
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
-importRpgDvsRos uses the importRosbag submodule
-(original located at https://github.com/event-driven-robotics/importRosbag)
-to import a rosbag, containing a selected set of ros msg types.
-In particular, this supports the dvs_msgs/EventArray messages defined at:
-http://rpg.ifi.uzh.ch/davis_data.html
-It also supports some standard ros types:
-    geometry_msgs/PoseStamped 
-    geometry_msgs/Transform
-    geometry_msgs/TransformStamped
-    geometry_msgs/TwistStamped
-    sensor_msgs/CameraInfo, (calibration)
-    sensor_msgs/Image
-    sensor_msgs/Imu 
-    sensor_msgs/PointCloud2
-    tf/tfMessage
-Furthermore there is support for:
-    esim_msgs/OpticFlow
-
-It returns nested dicts of the form:
-{
-    info
-    data
-        channelName
-            dvs
-                "pol": numpy array of bool
-                "x": numpy array of uint16
-                "y": numpy array of uint16
-                "ts": numpy array of float - seconds (basic format is int with unit increments of 80 ns) 
-            frame ...
-            imu ...
-            etc ...
-
-It optionally reorders the resulting data to support legacy templates (kwarg=template) 
-Here follow 2 example templates:
-    
-template = {
-    'left': {
-        'dvs': '/davis/left/events',
-    }, 'right': {
-        'dvs': '/davis/right/events',
-        }
-    }    
-    
-template = {
-    'ch0': {
-        'dvs': '/dvs/events',
-        'frame': '/dvs/image_raw',
-        'pose6q': '/optitrack/davis',
-        'cam': '/dvs/camera_info',
-        'imu': '/dvs/imu'
-        }
-    }    
-
-If a template is supplied, any connections which are not named in the template are not imported but simply listed.
-If an empty template is supplied, then the contained types are printed out.
-Use this to inspect a new .bag file before defining the import template.
-Without any template, the default behaviour is to put any imported data into 
-its own channel, named after the topic in the bag.
-"""
-
-#%%
-
-import string
-
-# Local imports
-from .timestamps import zeroTimestampsForAChannel, rezeroTimestampsForImportedDicts
-from .importRosbag.importRosbag.importRosbag import importRosbag
-    
-def bimveeTypeForRosbagType(rosbagType):
-    rosbagType = rosbagType.replace('/','_')
-    if rosbagType == 'dvs_msgs_EventArray': return 'dvs'
-    if rosbagType == 'esim_msgs_OpticFlow': return 'flowMap'
-    if rosbagType == 'geometry_msgs_PoseStamped': return 'pose6q'
-    if rosbagType == 'geometry_msgs_Transform': return 'pose6q'
-    if rosbagType == 'geometry_msgs_TransformStamped': return 'pose6q'
-    if rosbagType == 'geometry_msgs_TwistStamped': return 'twist'
-    if rosbagType == 'sensor_msgs_CameraInfo': return 'cam'
-    if rosbagType == 'sensor_msgs_Image': return 'frame'
-    if rosbagType == 'sensor_msgs_Imu': return 'imu'
-    if rosbagType == 'sensor_msgs_PointCloud2': return 'point3'
-    if rosbagType == 'tf_tfMessage': return 'pose6q'
-    return None
-
-def importRpgDvsRos(filePathOrName, **kwargs):    
-    template = kwargs.get('template')
-    if template == {}: # Just list contents of bag without importing
-        topics = importRosbag(filePathOrName=filePathOrName, listTopics=True, **kwargs)
-        return
-    topics = importRosbag(filePathOrName=filePathOrName, **kwargs)
-    outDict = {
-        'info': kwargs,
-        'data': {}
-            }
-    outDict['info']['filePathOrName'] = filePathOrName
-    if template is None:
-        for topicLabel in topics.keys():
-            rosbagType = topics[topicLabel].pop('rosbagType')
-            bimveeType = bimveeTypeForRosbagType(rosbagType)
-            if bimveeType is None:
-                print('Actually, ' + topicLabel + ' has not been imported, because the rosbag message type ' + rosbagType + ' has not been recognised.')
-            else:
-                outDict['data'][topicLabel] = {bimveeType: topics[topicLabel]}
-    else:
-        # If we get to here then there is a template to parse
-        # The template becomes the data branch of the importedDict
-        for channelKey in template.keys():
-            channelKeyStripped = str(channelKey).translate(str.maketrans('', '', string.punctuation))
-            outDict['data'][channelKeyStripped] = {}
-            for dataType in template[channelKey]:
-                topicLabel = template[channelKey][dataType]
-                topic = topics.pop(topicLabel)
-                rosbagType = topic.pop('rosbagType')
-                bimveeType = bimveeTypeForRosbagType(rosbagType)
-                if bimveeType != dataType:
-                    print('dataType "', dataType, '" not correctly defined for topic: "', topicLabel, '"')
-                else:
-                    outDict['data'][channelKeyStripped][dataType] = topic
-    # Post processing
-    if kwargs.get('zeroTime', kwargs.get('zeroTimestamps', True)):
-        # Optional: start the timestamps at zero for the first event
-        # This is done collectively for all the concurrent imports
-        for channelKey in outDict['data'].keys():
-            zeroTimestampsForAChannel(outDict['data'][channelKey])
-        # jointly rezero for all channels
-        rezeroTimestampsForImportedDicts(outDict)
-    return outDict
+# -*- coding: utf-8 -*-
+
+"""https://github.com/event-driven-robotics/importRosbag
+Copyright (C) 2019 Event-driven Perception for Robotics
+Authors: Sim Bamford
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
+importRpgDvsRos uses the importRosbag submodule
+(original located at https://github.com/event-driven-robotics/importRosbag)
+to import a rosbag, containing a selected set of ros msg types.
+In particular, this supports the dvs_msgs/EventArray messages defined at:
+http://rpg.ifi.uzh.ch/davis_data.html
+It also supports some standard ros types:
+    geometry_msgs/PoseStamped 
+    geometry_msgs/Transform
+    geometry_msgs/TransformStamped
+    geometry_msgs/TwistStamped
+    sensor_msgs/CameraInfo, (calibration)
+    sensor_msgs/Image
+    sensor_msgs/Imu 
+    sensor_msgs/PointCloud2
+    tf/tfMessage
+Furthermore there is support for:
+    esim_msgs/OpticFlow
+
+It returns nested dicts of the form:
+{
+    info
+    data
+        channelName
+            dvs
+                "pol": numpy array of bool
+                "x": numpy array of uint16
+                "y": numpy array of uint16
+                "ts": numpy array of float - seconds (basic format is int with unit increments of 80 ns) 
+            frame ...
+            imu ...
+            etc ...
+
+It optionally reorders the resulting data to support legacy templates (kwarg=template) 
+Here follow 2 example templates:
+    
+template = {
+    'left': {
+        'dvs': '/davis/left/events',
+    }, 'right': {
+        'dvs': '/davis/right/events',
+        }
+    }    
+    
+template = {
+    'ch0': {
+        'dvs': '/dvs/events',
+        'frame': '/dvs/image_raw',
+        'pose6q': '/optitrack/davis',
+        'cam': '/dvs/camera_info',
+        'imu': '/dvs/imu'
+        }
+    }    
+
+If a template is supplied, any connections which are not named in the template are not imported but simply listed.
+If an empty template is supplied, then the contained types are printed out.
+Use this to inspect a new .bag file before defining the import template.
+Without any template, the default behaviour is to put any imported data into 
+its own channel, named after the topic in the bag.
+"""
+
+#%%
+
+import string
+
+# Local imports
+from .timestamps import zeroTimestampsForAChannel, rezeroTimestampsForImportedDicts
+from .importRosbag.importRosbag.importRosbag import importRosbag
+    
+def bimveeTypeForRosbagType(rosbagType):
+    rosbagType = rosbagType.replace('/','_')
+    if rosbagType == 'dvs_msgs_EventArray': return 'dvs'
+    if rosbagType == 'esim_msgs_OpticFlow': return 'flowMap'
+    if rosbagType == 'geometry_msgs_PoseStamped': return 'pose6q'
+    if rosbagType == 'geometry_msgs_Transform': return 'pose6q'
+    if rosbagType == 'geometry_msgs_TransformStamped': return 'pose6q'
+    if rosbagType == 'geometry_msgs_TwistStamped': return 'twist'
+    if rosbagType == 'sensor_msgs_CameraInfo': return 'cam'
+    if rosbagType == 'sensor_msgs_Image': return 'frame'
+    if rosbagType == 'sensor_msgs_Imu': return 'imu'
+    if rosbagType == 'sensor_msgs_PointCloud2': return 'point3'
+    if rosbagType == 'tf_tfMessage': return 'pose6q'
+    if rosbagType == 'vicon_Subject': return 'pose6q'
+    return None
+
+def importRpgDvsRos(filePathOrName, **kwargs):    
+    template = kwargs.get('template')
+    if template == {}: # Just list contents of bag without importing
+        topics = importRosbag(filePathOrName=filePathOrName, listTopics=True, **kwargs)
+        return
+    topics = importRosbag(filePathOrName=filePathOrName, **kwargs)
+    outDict = {
+        'info': kwargs,
+        'data': {}
+            }
+    outDict['info']['filePathOrName'] = filePathOrName
+    if template is None:
+        for topicLabel in topics.keys():
+            rosbagType = topics[topicLabel].pop('rosbagType')
+            bimveeType = bimveeTypeForRosbagType(rosbagType)
+            if bimveeType is None:
+                print('Actually, ' + topicLabel + ' has not been imported, because the rosbag message type ' + rosbagType + ' has not been recognised.')
+            else:
+                outDict['data'][topicLabel] = {bimveeType: topics[topicLabel]}
+    else:
+        # If we get to here then there is a template to parse
+        # The template becomes the data branch of the importedDict
+        for channelKey in template.keys():
+            channelKeyStripped = str(channelKey).translate(str.maketrans('', '', string.punctuation))
+            outDict['data'][channelKeyStripped] = {}
+            for dataType in template[channelKey]:
+                topicLabel = template[channelKey][dataType]
+                topic = topics.pop(topicLabel)
+                rosbagType = topic.pop('rosbagType')
+                bimveeType = bimveeTypeForRosbagType(rosbagType)
+                if bimveeType != dataType:
+                    print('dataType "', dataType, '" not correctly defined for topic: "', topicLabel, '"')
+                else:
+                    outDict['data'][channelKeyStripped][dataType] = topic
+    # Post processing
+    if kwargs.get('zeroTime', kwargs.get('zeroTimestamps', True)):
+        # Optional: start the timestamps at zero for the first event
+        # This is done collectively for all the concurrent imports
+        for channelKey in outDict['data'].keys():
+            zeroTimestampsForAChannel(outDict['data'][channelKey])
+        # jointly rezero for all channels
+        rezeroTimestampsForImportedDicts(outDict)
+    return outDict
```

### Comparing `bimvee-1.0.9/bimvee/importSecDvs.py` & `bimvee-1.0.9.dev0/bimvee/importSecDvs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,184 +1,192 @@
-# -*- coding: utf-8 -*-
-
-"""
-Copyright (C) 2020 Event-driven Perception for Robotics
-Authors: Sim Bamford
-         Ander Arriandiaga Laresgoiti
-
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
-importSecDvs opens a .bin file, assumed to contain encoded data from SecDvs gen3.
-Returns a dict in this format:
-{'info': {},
- 'data': {
-         ch0: {
-               dvs: {
-                     'ts': np.array of np.float64 in seconds 
-                     'x': np.array of np.uint16 in pixels
-                     'y': np.array of np.uint16 in pixels
-                     'pol': np.array of np.bool -- 1 = ON event 
-                    }}}}
-"""
-
-import numpy as np
-from tqdm import tqdm 
-
-# Local imports
-from .timestamps import unwrapTimestamps, zeroTimestampsForADataType
-
-def importSecDvs(**kwargs):
-    filePathOrName = kwargs['filePathOrName']
-    print('Attempting to import ' + filePathOrName + ' as secdvs')
-    with open(filePathOrName, 'rb') as file:
-        data = np.fromfile(file, dtype='>u4')
-
-    print('Clipping any rows without column info...')
-    # Hunt for the first col iteratively and cut data before this
-    for idx, word in enumerate(data):
-        if word & 0x4000000:
-            break
-    data = data[idx:]
-
-    print('Building indices for word types  ...')
-    isTs = (data & 0x08000000).astype(np.bool) # Reference timestamp, i.e. tsMsb
-    isCol = (data & 0x4000000).astype(np.bool) # X and tsLsb
-    isRow = (data & 0x80000000).astype(np.bool) # y and pol
-
-    print('Handling col data ...')
-    # create an index which points data back to col
-    numCol = np.count_nonzero(isCol)
-    colIdsRange = np.arange(numCol)
-    colIdsSparse = np.where(isCol)[0]
-    colIdsNext = np.append(colIdsSparse[1:], len(data))
-    colIdx = np.zeros_like(data)
-    for rangeIdx, firstIdx, nextIdx in zip(colIdsRange, colIdsSparse, colIdsNext):
-        colIdx[firstIdx:nextIdx] = rangeIdx
-    # now we can isolate col
-    col = data[isCol]
-    # convert col data
-    xByCol = (col & 0x000003FF).astype(np.uint16) # column Address
-    tsSmallByCol = (col & 0x1FF800) >> 11
-	# create col data vectors which match data
-    x = xByCol[colIdx]
-    tsSmall = tsSmallByCol[colIdx]
-    
-    print('Handling timestamp data ...')
-
-    # from data extract the "start col" flag
-    isStartCol = (data & 0x200000).astype(np.bool) & isCol
-    # now, for each startCol, we want to search backwards through data for a ts    
-    # To do this, we find the "data" idx of start col, we create a set of tsIds
-    # and then we search tsIds for each dataIdx    
-    tsIdsSparse = np.where(isTs)[0]
-    # Actually find the tsMsb at this point, to avoid more indexing
-    tsMsbSparse = (data[isTs] & 0x003FFFFF) << 10
-    tsMsbSparse = np.insert(tsMsbSparse, 0, tsMsbSparse[0] - (1 << 10))
-    # create an index which points data back to startCols
-    startColIdsSparse = np.where(isStartCol)[0]
-    # Search tsIds for each dataIdx
-    tsForStartCol = np.zeros_like(startColIdsSparse)
-    for idx, startColIdx in enumerate(startColIdsSparse):
-        tsForStartCol[idx] = tsMsbSparse[np.searchsorted(tsIdsSparse, startColIdx)]
-
-    # Now we have the ts(Large) for each startCol event. Now create a tsLarge
-    # array which matches data; do this in just the same way as above for
-    # tsSmall given col and colIdx
-    # create an index which points data back to col
-    numStartCol = np.count_nonzero(isStartCol)
-    startColIdsRange = np.arange(numStartCol)
-    startColIdsSparse = np.where(isStartCol)[0]
-    startColIdsNext = np.append(startColIdsSparse[1:], len(data))
-    startColIdx = np.zeros_like(data)
-    for rangeIdx, firstIdx, nextIdx in zip(startColIdsRange, startColIdsSparse, startColIdsNext):
-        startColIdx[firstIdx:nextIdx] = rangeIdx
-    tsLarge = tsForStartCol[startColIdx]
-
-    # Now we have tsLarge and tsSmall aligned by data, 
-    # we can sum these to give the full ts
-    ts = tsLarge + tsSmall
-
-    print('Handling row data ...')
-
-    # Now we have x and ts for each row in data; 
-    # now select these just for group/row data
-    x = x[isRow]
-    ts = ts[isRow]
-    data = data[isRow]
-
-    # A major timewrap is possible, so handle unwrapping before the following 
-    # processing, which will mix up the timestamps
-    ts = unwrapTimestamps(ts)  / 1000000 # Convert to seconds in the same step
-    
-    # Break out addr and pol for each of the two groups
-    pol1 = ((data & 0x00010000) >> 16).astype(np.bool)
-    yLarge1 = ((data & 0x00FC0000) >> 15).astype(np.uint16) # grp1Address
-    pol2 = ((data & 0x00020000) >> 17).astype(np.bool)
-    grp2Offset = (data & 0x7C000000) >> 23 
-    yLarge2 = (grp2Offset + yLarge1).astype(np.uint16)
-
-    # for each of the single bit indices, select events for each of the two groups
-    grp1Events = data & 0xFF
-    grp2Events = data & 0xFF00
-    tsToConcatenate = []
-    xToConcatenate = []
-    yToConcatenate = []
-    polToConcatenate = []
-    for idx in tqdm(range(8)):
-        #group 1
-        grp1Bool = (grp1Events & (2 ** idx)).astype(np.bool)
-        tsToConcatenate.append(ts[grp1Bool])
-        xToConcatenate.append(x[grp1Bool])
-        yToConcatenate.append(yLarge1[grp1Bool] + idx)
-        polToConcatenate.append(pol1[grp1Bool])
-        # group 2        
-        grp2Bool = (grp2Events & (2 ** (idx + 8))).astype(np.bool)
-        tsToConcatenate.append(ts[grp2Bool])
-        xToConcatenate.append(x[grp2Bool])
-        yToConcatenate.append(yLarge2[grp2Bool] + idx)
-        polToConcatenate.append(pol2[grp2Bool])
-
-    print('Post-processing steps ...')
-
-    # Concatenate the resulting arrays
-    ts = np.concatenate(tsToConcatenate)
-    x = np.concatenate(xToConcatenate)
-    y = np.concatenate(yToConcatenate)
-    pol = np.concatenate(polToConcatenate)
-    
-    # The above selection strategy mixed up the timestamps, so sort the events by ts
-    
-    ids = np.argsort(ts)
-    
-    ts = ts[ids]
-    x = x[ids]
-    y = y[ids]
-    pol = pol[ids]
-    
-    dvsDict = {'ts': ts,
-               'x': x,
-               'y': y,
-               'pol': pol,
-               }
-
-    if kwargs.get('zeroTime', kwargs.get('zeroTimestamps', True)): 
-        zeroTimestampsForADataType(dvsDict)
-    outDict = {
-    'info': {'filePathOrName':filePathOrName,
-        'fileFormat': 'secdvs'},
-    'data': {
-        'ch0': {
-            'dvs': dvsDict
-            }
-        }
-    }
-    print('Done.')
-            
-    return outDict
+# -*- coding: utf-8 -*-
+
+"""
+Copyright (C) 2020 Event-driven Perception for Robotics
+Authors: Sim Bamford
+         Ander Arriandiaga Laresgoiti
+
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
+importSecDvs opens a .bin file, assumed to contain encoded data from SecDvs gen3.
+Returns a dict in this format:
+{'info': {},
+ 'data': {
+         ch0: {
+               dvs: {
+                     'ts': np.array of np.float64 in seconds 
+                     'x': np.array of np.uint16 in pixels
+                     'y': np.array of np.uint16 in pixels
+                     'pol': np.array of np.bool -- 1 = ON event 
+                    }}}}
+"""
+
+import numpy as np
+from tqdm import tqdm 
+
+# Local imports
+from .timestamps import unwrapTimestamps, zeroTimestampsForADataType
+
+def importSecDvs(**kwargs):
+    filePathOrName = kwargs['filePathOrName']
+    print('Attempting to import ' + filePathOrName + ' as secdvs')
+    with open(filePathOrName, 'rb') as file:
+        data = np.fromfile(file, dtype='>u4')
+
+    print('Clipping any rows without column info...')
+    # Hunt for the first col iteratively and cut data before this
+    for idx, word in enumerate(data):
+        if word & 0x4000000:
+            break
+    data = data[idx:]
+
+    print('Building indices for word types  ...')
+    isTs = (data & 0x08000000).astype(np.bool) # Reference timestamp, i.e. tsMsb
+    isCol = (data & 0x4000000).astype(np.bool) # X and tsLsb
+    isRow = (data & 0x80000000).astype(np.bool) # y and pol
+
+    print('Handling col data ...')
+    # create an index which points data back to col
+    numCol = np.count_nonzero(isCol)
+    colIdsRange = np.arange(numCol)
+    colIdsSparse = np.where(isCol)[0]
+    colIdsNext = np.append(colIdsSparse[1:], len(data))
+    colIdx = np.zeros_like(data)
+    for rangeIdx, firstIdx, nextIdx in zip(colIdsRange, colIdsSparse, colIdsNext):
+        colIdx[firstIdx:nextIdx] = rangeIdx
+    # now we can isolate col
+    col = data[isCol]
+    # convert col data
+    xByCol = (col & 0x000003FF).astype(np.uint16) # column Address
+    tsSmallByCol = (col & 0x1FF800) >> 11
+	# create col data vectors which match data
+    x = xByCol[colIdx]
+    tsSmall = tsSmallByCol[colIdx]
+    
+    print('Handling timestamp data ...')
+
+    # from data extract the "start col" flag
+    isStartCol = (data & 0x200000).astype(np.bool) & isCol
+    # now, for each startCol, we want to search backwards through data for a ts    
+    # To do this, we find the "data" idx of start col, we create a set of tsIds
+    # and then we search tsIds for each dataIdx    
+    tsIdsSparse = np.where(isTs)[0]
+    # Actually find the tsMsb at this point, to avoid more indexing
+    tsMsbSparse = (data[isTs] & 0x003FFFFF) << 10
+    tsMsbSparse = np.insert(tsMsbSparse, 0, tsMsbSparse[0] - (1 << 10))
+    # create an index which points data back to startCols
+    startColIdsSparse = np.where(isStartCol)[0]
+    # Search tsIds for each dataIdx
+    tsForStartCol = np.zeros_like(startColIdsSparse)
+    for idx, startColIdx in enumerate(startColIdsSparse):
+        tsForStartCol[idx] = tsMsbSparse[np.searchsorted(tsIdsSparse, startColIdx)]
+
+    # Now we have the ts(Large) for each startCol event. Now create a tsLarge
+    # array which matches data; do this in just the same way as above for
+    # tsSmall given col and colIdx
+    # create an index which points data back to col
+    numStartCol = np.count_nonzero(isStartCol)
+    startColIdsRange = np.arange(numStartCol)
+    startColIdsSparse = np.where(isStartCol)[0]
+    startColIdsNext = np.append(startColIdsSparse[1:], len(data))
+    startColIdx = np.zeros_like(data)
+    for rangeIdx, firstIdx, nextIdx in zip(startColIdsRange, startColIdsSparse, startColIdsNext):
+        startColIdx[firstIdx:nextIdx] = rangeIdx
+    tsLarge = tsForStartCol[startColIdx]
+
+    # Now we have tsLarge and tsSmall aligned by data, 
+    # we can sum these to give the full ts
+    ts = tsLarge + tsSmall
+
+    print('Handling row data ...')
+
+    # Now we have x and ts for each row in data; 
+    # now select these just for group/row data
+    x = x[isRow]
+    ts = ts[isRow]
+    data = data[isRow]
+
+    # A major timewrap is possible, so handle unwrapping before the following 
+    # processing, which will mix up the timestamps
+    # Noticing that for whatever reason, there can be discontinuities in the 
+    # minor timestamps, there is a first call to unwrap timestamps which 
+    # uses a wrapTime of 1024 us. This would introduce about 1 ms of delay
+    # in the case of an actual major timewrap
+    ts = unwrapTimestamps(ts, wrapTime=1024)  
+    ts = unwrapTimestamps(ts)  / 1000000 # Convert to seconds in the same step
+    
+    # Break out addr and pol for each of the two groups
+    pol1 = ((data & 0x00010000) >> 16).astype(np.bool)
+    yLarge1 = ((data & 0x00FC0000) >> 15).astype(np.uint16) # grp1Address
+    pol2 = ((data & 0x00020000) >> 17).astype(np.bool)
+    grp2Offset = (data & 0x7C000000) >> 23 
+    yLarge2 = (grp2Offset + yLarge1).astype(np.uint16)
+
+    # for each of the single bit indices, select events for each of the two groups
+    grp1Events = data & 0xFF
+    grp2Events = data & 0xFF00
+    tsToConcatenate = []
+    xToConcatenate = []
+    yToConcatenate = []
+    polToConcatenate = []
+    for idx in tqdm(range(8)):
+        #group 1
+        grp1Bool = (grp1Events & (2 ** idx)).astype(np.bool)
+        tsToConcatenate.append(ts[grp1Bool])
+        xToConcatenate.append(x[grp1Bool])
+        yToConcatenate.append(yLarge1[grp1Bool] + idx)
+        polToConcatenate.append(pol1[grp1Bool])
+        # group 2        
+        grp2Bool = (grp2Events & (2 ** (idx + 8))).astype(np.bool)
+        tsToConcatenate.append(ts[grp2Bool])
+        xToConcatenate.append(x[grp2Bool])
+        yToConcatenate.append(yLarge2[grp2Bool] + idx)
+        polToConcatenate.append(pol2[grp2Bool])
+
+    print('Post-processing steps ...')
+
+    # Concatenate the resulting arrays
+    ts = np.concatenate(tsToConcatenate)
+    x = np.concatenate(xToConcatenate)
+    y = np.concatenate(yToConcatenate)
+    pol = np.concatenate(polToConcatenate)
+    
+    # The above selection strategy mixed up the timestamps, so sort the events by ts
+    
+    ids = np.argsort(ts)
+    
+    ts = ts[ids]
+    x = x[ids]
+    y = y[ids]
+    pol = pol[ids]
+    
+    # Invert polarity, in line with library-wide definition
+    pol = ~pol
+    
+    dvsDict = {'ts': ts,
+               'x': x,
+               'y': y,
+               'pol': pol,
+               }
+
+    if kwargs.get('zeroTime', kwargs.get('zeroTimestamps', True)): 
+        zeroTimestampsForADataType(dvsDict)
+    outDict = {
+    'info': {'filePathOrName':filePathOrName,
+        'fileFormat': 'secdvs'},
+    'data': {
+        'ch0': {
+            'dvs': dvsDict
+            }
+        }
+    }
+    print('Done.')
+            
+    return outDict
```

### Comparing `bimvee-1.0.9/bimvee/info.py` & `bimvee-1.0.9.dev0/bimvee/info.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,109 +1,112 @@
-# -*- coding: utf-8 -*-
-"""
-Copyright (C) 2019 Event-driven Perception for Robotics
-Authors: Sim Bamford
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
-Contains general functions for text summaries of the contents of dicts which result 
-from imports using importAe function
-"""
-
-from math import log10, floor
-import numpy as np
-import pprint
-pp = pprint.PrettyPrinter(indent=12)
-
-# Round to 3 s.f.
-def sf3(x):
-    if x and isinstance(x, (int, float, complex)) and not isinstance(x, bool):
-        return round(x, -int(floor(log10(abs(x)))) + 2)
-    else:
-        return x
-
-def fieldMinMax(dataTypeDict, fieldName):
-    if fieldName in dataTypeDict:
-        field = dataTypeDict[fieldName]
-        if type(field) == np.ndarray:
-            if field.shape[0] > 1:
-                # Handle 2D arrays, e.g. an array containing x, y, z in columns
-                if len(field.shape) > 1:
-                    for dim1Idx in range(field.shape[1]):
-                        print('            ', 
-                              sf3(np.min(field[:, dim1Idx])), 
-                              ' >= ', fieldName, ' - col ', dim1Idx,  
-                              ' >= ', sf3(np.max(field[:, dim1Idx])))
-                else:
-                    print('            ', 
-                          sf3(np.min(field)), 
-                          ' >= ', fieldName,
-                          ' >= ', sf3(np.max(field)))
-
-def info(containers, **kwargs):
-    if not isinstance(containers, list):
-        containers = [containers]
-    for container in containers:
-        pp.pprint(container['info'])
-        for channelName in container['data']:
-            print('    Channel: ' + channelName)
-            for dataType in container['data'][channelName]:
-                print('        DataType: ' + dataType)
-                dataTypeDict = container['data'][channelName][dataType]
-                if 'ts' in dataTypeDict:
-                    print('            Num events: ', len(dataTypeDict['ts']))
-                    fieldMinMax(dataTypeDict, 'ts')
-                    if 'tsOffset' in dataTypeDict:
-                        print('            Ts offset: ', dataTypeDict['tsOffset'])
-                    for fieldName in dataTypeDict.keys():
-                        if fieldName not in ['ts', 'tsOffset']:
-                            fieldMinMax(dataTypeDict, fieldName)
-                else:
-                    pp.pprint(dataTypeDict)
-                print()
-            print()
-def infoTs(containers, **kwargs):
-    if not isinstance(containers, list):
-        containers = [containers]
-    for container in containers:
-        print(container['info'])
-        for channelName in container['data']:
-            print('    Channel: ' + channelName)
-            for dataType in container['data'][channelName]:
-                print('        DataType: ' + dataType)
-                dataTypeDict = container['data'][channelName][dataType]
-                if 'ts' in dataTypeDict:
-                    fieldMinMax(dataTypeDict, 'ts')
-                if 'tsOffset' in dataTypeDict:
-                    print('            Ts offset: ', dataTypeDict['tsOffset'])
-
-#%% Legacy function names
-
-def dict_keys_print(d, indent):
-    print(' ' * (4 * indent - 2) + '{ ', end='')
-    first = True
-    for key, value in d.items():
-        if first:
-            print(str(key), end='')
-            first = False
-        else:
-            print(' ' * 4 * indent + str(key), end='')
-        if isinstance(value, dict):
-            print(':')
-            dict_keys_print(value, indent + 1)
-        else:
-            print(',')
-            continue
-    print(' ' * (4 * indent - 2) + '}')
-
-def infoForImportedDicts(container, **kwargs):
-    info(container, **kwargs)
-
-def infoTsForImportedDicts(container, **kwargs):
+# -*- coding: utf-8 -*-
+"""
+Copyright (C) 2019 Event-driven Perception for Robotics
+Authors: Sim Bamford
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
+Contains general functions for text summaries of the contents of dicts which result 
+from imports using importAe function
+"""
+
+from math import log10, floor
+import numpy as np
+import pprint
+pp = pprint.PrettyPrinter(indent=12)
+
+# Round to 3 s.f.
+def sf3(x):
+    if x and isinstance(x, (int, float, complex)) and not isinstance(x, bool):
+        return round(x, -int(floor(log10(abs(x)))) + 2)
+    else:
+        return x
+
+def fieldMinMax(dataTypeDict, fieldName):
+    if fieldName in dataTypeDict:
+        field = dataTypeDict[fieldName]
+        if type(field) == np.ndarray:
+            if field.shape[0] > 1:
+                # Handle 2D arrays, e.g. an array containing x, y, z in columns
+                try:
+                    if len(field.shape) > 1:
+                        for dim1Idx in range(field.shape[1]):
+                            print('            ', 
+                                  sf3(np.min(field[:, dim1Idx])), 
+                                  ' >= ', fieldName, ' - col ', dim1Idx,  
+                                  ' >= ', sf3(np.max(field[:, dim1Idx])))
+                    else:
+                        print('            ', 
+                              sf3(np.min(field)), 
+                              ' >= ', fieldName,
+                              ' >= ', sf3(np.max(field)))
+                except ValueError:
+                    print('            ', fieldName, ' contains data error!')  
+
+def info(containers, **kwargs):
+    if not isinstance(containers, list):
+        containers = [containers]
+    for container in containers:
+        pp.pprint(container['info'])
+        for channelName in container['data']:
+            print('    Channel: ' + channelName)
+            for dataType in container['data'][channelName]:
+                print('        DataType: ' + dataType)
+                dataTypeDict = container['data'][channelName][dataType]
+                if 'ts' in dataTypeDict:
+                    print('            Num events: ', len(dataTypeDict['ts']))
+                    fieldMinMax(dataTypeDict, 'ts')
+                    if 'tsOffset' in dataTypeDict:
+                        print('            Ts offset: ', dataTypeDict['tsOffset'])
+                    for fieldName in dataTypeDict.keys():
+                        if fieldName not in ['ts', 'tsOffset']:
+                            fieldMinMax(dataTypeDict, fieldName)
+                else:
+                    pp.pprint(dataTypeDict)
+                print()
+            print()
+def infoTs(containers, **kwargs):
+    if not isinstance(containers, list):
+        containers = [containers]
+    for container in containers:
+        print(container['info'])
+        for channelName in container['data']:
+            print('    Channel: ' + channelName)
+            for dataType in container['data'][channelName]:
+                print('        DataType: ' + dataType)
+                dataTypeDict = container['data'][channelName][dataType]
+                if 'ts' in dataTypeDict:
+                    fieldMinMax(dataTypeDict, 'ts')
+                if 'tsOffset' in dataTypeDict:
+                    print('            Ts offset: ', dataTypeDict['tsOffset'])
+
+#%% Legacy function names
+
+def dict_keys_print(d, indent):
+    print(' ' * (4 * indent - 2) + '{ ', end='')
+    first = True
+    for key, value in d.items():
+        if first:
+            print(str(key), end='')
+            first = False
+        else:
+            print(' ' * 4 * indent + str(key), end='')
+        if isinstance(value, dict):
+            print(':')
+            dict_keys_print(value, indent + 1)
+        else:
+            print(',')
+            continue
+    print(' ' * (4 * indent - 2) + '}')
+
+def infoForImportedDicts(container, **kwargs):
+    info(container, **kwargs)
+
+def infoTsForImportedDicts(container, **kwargs):
     infoTs(container, **kwargs)
```

### Comparing `bimvee-1.0.9/bimvee/plot.py` & `bimvee-1.0.9.dev0/bimvee/plot.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,59 @@
-# -*- coding: utf-8 -*-
-"""
-Copyright (C) 2019 Event-driven Perception for Robotics
-Authors: Sim Bamford
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
-Takes a dict as imported by importAe, and for each channel, 
-tries to run the appropriate general visualisation function
-"""
-
-# local imports
-from .plotDvsContrast import plotDvsContrast
-from .plotEventRate import plotEventRate
-from .plotFrame import plotFrame
-from .plotPose import plotPose
-from .plotImu import plotImu
-from .plotFlow import plotFlow
-
-def plot(inDict, **kwargs):
-    if isinstance(inDict, list):
-        for inDictInst in inDict:
-            plot(inDictInst, **kwargs)
-        return
-    if isinstance(inDict, dict):
-        if 'info' in inDict: # Special handling for a file-level container
-            kwargs['title'] = inDict['info'].get('filePathOrName', '')
-            plot(inDict['data'], **kwargs)
-        else:
-            title = kwargs.get('title', '')
-            for keyName in inDict.keys():
-                if isinstance(inDict[keyName], dict):
-                    if keyName == 'dvs':
-                        plotDvsContrast(inDict[keyName], **kwargs)
-                        plotEventRate(inDict[keyName], **kwargs)
-                    elif keyName == 'frame':
-                        plotFrame(inDict[keyName], **kwargs)
-                    elif keyName == 'imu':
-                        plotImu(inDict[keyName], **kwargs)
-                    elif keyName == 'pose6q':
-                        plotPose(inDict[keyName], **kwargs)
-                    elif keyName == 'point3' in channel:
-                        plotPose(inDict[keyName], **kwargs)
-                    elif keyName == 'flow' in channel:
-                        plotFlow(inDict[keyName], **kwargs)
-                    else:
-                        kwargs['title'] = (title + '-' + keyName).lstrip('-')
-                        plot(inDict[keyName], **kwargs)
+# -*- coding: utf-8 -*-
+"""
+Copyright (C) 2019 Event-driven Perception for Robotics
+Authors: Sim Bamford
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
+Takes a dict as imported by importAe, and for each channel, 
+tries to run the appropriate general visualisation function
+"""
+
+# local imports
+from .plotDvsContrast import plotDvsContrast
+from .plotEventRate import plotEventRate
+from .plotFrame import plotFrame
+from .plotPose import plotPose
+from .plotImu import plotImu
+from .plotFlow import plotFlow
+from .container import Container
+
+def plot(inDict, **kwargs):
+    if isinstance(inDict, Container):
+        inDict = inDict.container
+    
+    if isinstance(inDict, list):
+        for inDictInst in inDict:
+            plot(inDictInst, **kwargs)
+        return
+    if isinstance(inDict, dict):
+        if 'info' in inDict: # Special handling for a file-level container
+            kwargs['title'] = inDict['info'].get('filePathOrName', '')
+            plot(inDict['data'], **kwargs)
+        else:
+            title = kwargs.get('title', '')
+            for keyName in inDict.keys():
+                if isinstance(inDict[keyName], dict):
+                    if keyName == 'dvs':
+                        plotDvsContrast(inDict[keyName], **kwargs)
+                        plotEventRate(inDict[keyName], **kwargs)
+                    elif keyName == 'frame':
+                        plotFrame(inDict[keyName], **kwargs)
+                    elif keyName == 'imu':
+                        plotImu(inDict[keyName], **kwargs)
+                    elif keyName == 'pose6q':
+                        plotPose(inDict[keyName], **kwargs)
+                    elif keyName == 'point3' in channel:
+                        plotPose(inDict[keyName], **kwargs)
+                    elif keyName == 'flow' in channel:
+                        plotFlow(inDict[keyName], **kwargs)
+                    else:
+                        kwargs['title'] = (title + '-' + keyName).lstrip('-')
+                        plot(inDict[keyName], **kwargs)
```

### Comparing `bimvee-1.0.9/bimvee/plotCorrelogram.py` & `bimvee-1.0.9.dev0/bimvee/plotCorrelogram.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,339 +1,339 @@
-# -*- coding: utf-8 -*-
-"""
-Copyright (C) 2019 Event-driven Perception for Robotics
-Author: Sim Bamford
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
-plotCorrelogram receives "inDict", which is a container for (2D) polarity events, 
-(Or a higher level container), containing fields with numpy arrays:    
-    ts
-    x
-    y
-    pol
-Autocorrelation
-A correlogram is created for the chosen range of pixels.
-Choose the pixels by setting the kwargs:
-    xMin
-    xMax
-    yMin
-    yMax
-By default, all pixels are included. 
-By default, all pixels are autocorrelated individually, and then the results are 
-combined, so the end result is a mean over all pixels.
-TODO: Could do an autocorrelation for all spikes for the range together.
-minTime and maxTime are used to constrain time. 
-By default, polarities are combined; separate them with splitByPol=true
-numBins is interpretted as the number of time bins in each of positive 
-and negative directions, not including a central bin. 
-"""
-
-#%% Plot tsPix (single pixel timestamps)
-
-import matplotlib.pyplot as plt
-import numpy as np
-from tqdm import trange
-
-# local imports
-from .split import cropSpace, cropTime, splitByPolarity
-    
-# TODO: include a linear spacing option
-def defineBoundariesAndDensities(**kwargs):
-    numBins = kwargs.get('numBins', 50)
-    minOffset = kwargs.get('minOffset', 0.00001) # 10 us
-    maxOffset = kwargs.get('maxOffset', 1.0) # 100 ms
-    logSpacing = kwargs.get('spacing', 'linear') == 'log'
-    mirrored = kwargs.get('mirrored', True)
-    if logSpacing:
-        boundaries = np.geomspace(minOffset, maxOffset, numBins+1)
-        if mirrored:
-            boundaries = np.concatenate((-np.flip(boundaries), boundaries))
-        elif not mirrored:
-            boundaries = np.concatenate((np.zeros((1)), boundaries))        
-    elif (not logSpacing) and mirrored: # Linear; ignore minOffset
-        boundaries = np.linspace(-maxOffset, maxOffset, numBins*2)
-    elif (not logSpacing) and (not mirrored):
-        boundaries = np.linspace(0, maxOffset, (numBins))
-    # now there are boundaries either starting from zero ot mirrored around zero 
-    # for each bin, including a central bin, and the extreme boundaries 
-    # are the edge of the time region of interest.
-    widths = (boundaries[1:] - boundaries[:-1])
-    densities = 1 / widths
-    centres = (boundaries[1:] + boundaries[:-1]) / 2
-    return boundaries, densities, centres, widths
-
-def interSpikeInterval(ts, boundaries, densities, **kwargs):
-    hist = np.zeros((len(densities)), dtype=np.float64)
-    diff = ts[1:] - ts[:-1]
-    for idx, (boundary1, boundary2) in enumerate(zip(boundaries[:-1], boundaries[1:])):
-        hist[idx] = np.sum(np.logical_and(diff >= boundary1, diff <= boundary2))
-    hist = hist * densities
-    sumHist = np.sum(hist) # Avoid dividing by zero in case the hist is empty
-    if sumHist:
-        hist = hist / sumHist
-    return hist
-
-# Plot the timings of the spikes in events2 w.r.t. the spikes in events1
-def plotInterSpikeIntervalSingle(events, **kwargs):    
-    if (len(events['ts']) == 0):
-        return
-    # use other library functions to do spatiotemporal cropping
-    # If this is called from plotInterSpikeInterval then this has already been done, 
-    # But do it here as well so that this function can be independent.
-    events = cropSpace(events, **kwargs)
-    events = cropTime(events, zeroTime=False, **kwargs)
-    kwargs['mirrored'] = False
-    boundaries, densities, centres, widths = defineBoundariesAndDensities(**kwargs)
-    # Spatial cropping has happened; now iterate through defacto spatial range
-    minX = np.min(events['x'])
-    maxX = np.max(events['x'])
-    minY = np.min(events['y'])
-    maxY = np.max(events['y'])
-    hist = np.zeros((len(densities)), dtype=np.float64)
-    for currX in trange(minX, maxX+1, leave=True, position=0):
-        currXLogical = events['x']==currX
-        tsForCurrX = events['ts'][currXLogical]
-        yForCurrX = events['y'][currXLogical]
-        for currY in range(minY, maxY+1):
-            tsXY = tsForCurrX[yForCurrX==currY]
-            if np.any(tsXY): 
-                hist = hist + interSpikeInterval(tsXY, boundaries, densities, **kwargs)
-    # Normalise
-    weightedSum = np.sum(hist / densities)
-    if weightedSum > 0:
-        hist = hist / np.sum(weightedSum)
-    axes = kwargs.get('axes')
-    if axes is None:
-        fig, axes = plt.subplots()
-        kwargs['axes'] = axes
-
-    axes.bar(centres, hist, widths, antialiased=False)
-    #axes.set_ylim(minX + minY*numX - 1, maxX + maxY*numX + 1)
-    #plt.xticks(theRange, labels)
-    title = kwargs.get('title', '')
-    if kwargs.get('minX', False) or  kwargs.get('maxX', False):
-        title = title + ' ' + str(minX) + '<=X<=' + str(maxX)
-    if kwargs.get('minY', False) or  kwargs.get('maxY', False):
-        title = title + ' ' + str(minY) + '<=Y<=' + str(maxY)
-    axes.set_title(title)
-
-    callback = kwargs.get('callback')
-    if callback is not None:
-        callback(**kwargs) 
-        
-def plotInterSpikeInterval(inDict, **kwargs):
-    # Boilerplate for descending container hierarchy
-    if isinstance(inDict, list):
-        for inDictInst in inDict:
-            plotInterSpikeInterval(inDictInst, **kwargs)
-        return
-    if 'info' in inDict: # Top level container
-        fileName = inDict['info'].get('filePathOrName', '')
-        print('plotInterSpikeInterval was called for file ' + fileName)
-        if not inDict['data']:
-            print('The import contains no data.')
-            return
-        for channelName in inDict['data']:
-            channelData = inDict['data'][channelName]
-            if 'dvs' in channelData and len(channelData['dvs']['ts']) > 0:
-                kwargs['title'] = ' '.join([fileName, str(channelName)])
-                plotInterSpikeInterval(channelData['dvs'], **kwargs)
-            else:
-                print('Channel ' + channelName + ' skipped because it contains no polarity data')
-        return
-    print('plotInterSpikeInterval working: ' + kwargs.get('title', 'unnamed'))
-    # use other library functions to do spatiotemporal cropping
-    inDict = cropSpace(inDict, **kwargs)
-    inDict = cropTime(inDict, zeroTime=False, **kwargs)
-    if kwargs.get('splitByPol', False):
-        splitDict = splitByPolarity(inDict)        
-        fig, axes = plt.subplots(1, 3)
-
-        kwargs['axes'] = axes[0]
-        kwargs['title'] = 'on + off'
-        print(kwargs['title'])
-        plotInterSpikeIntervalSingle(inDict, **kwargs)
-
-        kwargs['axes'] = axes[1]
-        kwargs['title'] = 'off'
-        print(kwargs['title'])
-        plotInterSpikeIntervalSingle(splitDict['0'], **kwargs)
-
-        kwargs['axes'] = axes[2]
-        kwargs['title'] = 'on'
-        print(kwargs['title'])
-        plotInterSpikeIntervalSingle(splitDict['1'], **kwargs)
-
-    else:            
-        axes = kwargs.get('axes')
-        if axes is None:
-            fig, axes = plt.subplots()
-            kwargs['axes'] = axes
-        kwargs['title'] = 'auto'
-        plotInterSpikeIntervalSingle(inDict, **kwargs)
-    
-# Alias using common abbreviation
-def plotIsi(inDict, **kwargs):
-    plotInterSpikeInterval(inDict, **kwargs)
-
-def crossCorrelation(ts1, ts2, boundaries, densities, **kwargs):
-    hist = np.zeros((len(densities)), dtype=np.float64)
-    # TODO: think about a nice array-based way to do the following:
-    for ts in ts1:
-        firstIdx = np.searchsorted(ts2, ts+boundaries[0])
-        lastIdx = np.searchsorted(ts2, ts+boundaries[-1])
-        selectedTs2 = ts2[firstIdx: lastIdx] - ts
-        histIds = np.searchsorted(boundaries, selectedTs2) - 1
-        for histIdx in histIds:
-            try:
-                hist[histIdx] = hist[histIdx] + 1
-            except IndexError:
-                pass # Out of bounds - we don't want it
-    # If this was intended as an autocorrelation then we need to remove the 
-    # self-correlations
-    if kwargs.get('auto', False):
-        centreIdx = int(len(boundaries) / 2) - 1 
-        hist[centreIdx] = hist[centreIdx] - len(ts1)
-    hist = hist * densities
-    sumHist = np.sum(hist) # Avoid dividing by zero in case the hist is empty
-    if sumHist:
-        hist = hist / sumHist
-    return hist
-
-# Plot the timings of the spikes in events2 w.r.t. the spikes in events1
-def plotCrossCorrelation(events1, events2, **kwargs):    
-    if (len(events1['ts']) == 0) or (len(events2['ts']) == 0):
-        return
-    # use other library functions to do spatiotemporal cropping
-    # If this is called from plotautocorrelation then this has already been done, 
-    # But do it here as well so that this function can be independent.
-    events1 = cropSpace(events1, **kwargs)
-    events1 = cropTime(events1, zeroTime=False, **kwargs)
-    events2 = cropSpace(events2, **kwargs)
-    events2 = cropTime(events2, zeroTime=False, **kwargs)
-    boundaries, densities, centres, widths = defineBoundariesAndDensities(**kwargs)
-    # Spatial cropping has happened; now iterate through defacto spatial range
-    minX = min(np.min(events1['x']), np.min(events2['x']))
-    maxX = max(np.max(events1['x']), np.max(events2['x']))
-    minY = min(np.min(events1['y']), np.min(events2['y']))
-    maxY = max(np.max(events1['y']), np.max(events2['y']))
-    hist = np.zeros((len(densities)), dtype=np.float64)
-    # TODO: This loop could be much more efficient, following the pattern in plotInterSpikeInterval, above
-    for currX in trange(minX, maxX+1, leave=True, position=0): 
-        for currY in range(minY, maxY+1):
-            ts1 = events1['ts'][np.logical_and(events1['x']==currX, events1['y']==currY)]
-            ts2 = events2['ts'][np.logical_and(events2['x']==currX, events2['y']==currY)]
-            if np.any(ts1) and np.any(ts2): 
-                hist = hist + crossCorrelation(ts1, ts2, boundaries, densities, **kwargs)
-    # Normalise
-    weightedSum = np.sum(hist / densities)
-    if weightedSum > 0:
-        hist = hist / np.sum(weightedSum)
-    axes = kwargs.get('axes')
-    if axes is None:
-        fig, axes = plt.subplots()
-        kwargs['axes'] = axes
-
-    axes.bar(centres, hist, widths, antialiased=False)
-    #axes.set_ylim(minX + minY*numX - 1, maxX + maxY*numX + 1)
-    #plt.xticks(theRange, labels)
-    title = kwargs.get('title', '')
-    if kwargs.get('minX', False) or  kwargs.get('maxX', False):
-        title = title + ' ' + str(minX) + '<=X<=' + str(maxX)
-    if kwargs.get('minY', False) or  kwargs.get('maxY', False):
-        title = title + ' ' + str(minY) + '<=Y<=' + str(maxY)
-    axes.set_title(title)
-
-    callback = kwargs.get('callback')
-    if callback is not None:
-        callback(**kwargs)    
-
-def plotAutoCorrelation(inDict, **kwargs):
-    # Boilerplate for descending container hierarchy
-    if isinstance(inDict, list):
-        for inDictInst in inDict:
-            plotCorrelogram(inDictInst, **kwargs)
-        return
-    if 'info' in inDict: # Top level container
-        fileName = inDict['info'].get('filePathOrName', '')
-        print('plotAutocorrelation was called for file ' + fileName)
-        if not inDict['data']:
-            print('The import contains no data.')
-            return
-        for channelName in inDict['data']:
-            channelData = inDict['data'][channelName]
-            if 'dvs' in channelData and len(channelData['dvs']['ts']) > 0:
-                kwargs['title'] = ' '.join([fileName, str(channelName)])
-                plotCorrelogram(channelData['dvs'], **kwargs)
-            else:
-                print('Channel ' + channelName + ' skipped because it contains no polarity data')
-        return
-    print('plotAutocorrelation working: ' + kwargs.get('title', 'unnamed'))
-    # use other library functions to do spatiotemporal cropping
-    inDict = cropSpace(inDict, **kwargs)
-    inDict = cropTime(inDict, zeroTime=False, **kwargs)
-    if kwargs.get('splitByPol', False):
-        splitDict = splitByPolarity(inDict)        
-        fig, axes = plt.subplots(2, 2)
-
-        kwargs['axes'] = axes[0, 0]
-        kwargs['title'] = 'on + off auto'
-        print(kwargs['title'])
-        kwargs['auto'] = True
-        plotCrossCorrelation(inDict, inDict, **kwargs)
-
-        kwargs['axes'] = axes[0, 1]
-        kwargs['title'] = 'off auto'
-        print(kwargs['title'])
-        kwargs['auto'] = True
-        plotCrossCorrelation(splitDict['0'], splitDict['0'], **kwargs)
-
-        kwargs['axes'] = axes[1, 0]
-        kwargs['title'] = 'on auto'
-        print(kwargs['title'])
-        kwargs['auto'] = True
-        plotCrossCorrelation(splitDict['1'], splitDict['1'], **kwargs)
-
-        kwargs['axes'] = axes[1, 1]
-        kwargs['title'] = 'on w.r.t. off cross'
-        print(kwargs['title'])
-        kwargs['auto'] = False
-        plotCrossCorrelation(splitDict['0'], splitDict['1'], **kwargs)
-
-    elif kwargs.get('splitByPolAlt', False):
-        splitDict = splitByPolarity(inDict)        
-        fig, axes = plt.subplots(3, 1)
-        kwargs['axes'] = axes[0]
-        kwargs['title'] = 'on + off auto'
-        print(kwargs['title'])
-        kwargs['auto'] = True
-        plotCrossCorrelation(inDict, inDict, **kwargs)
-        kwargs['axes'] = axes[1]
-        kwargs['title'] = 'on w.r.t. off cross'
-        print(kwargs['title'])
-        kwargs['auto'] = False
-        plotCrossCorrelation(splitDict['0'], splitDict['1'], **kwargs)
-        kwargs['axes'] = axes[2]
-        kwargs['title'] = 'off w.r.t. on cross'
-        print(kwargs['title'])
-        kwargs['auto'] = False
-        plotCrossCorrelation(splitDict['1'], splitDict['0'], **kwargs)
-    else:            
-        axes = kwargs.get('axes')
-        if axes is None:
-            fig, axes = plt.subplots()
-            kwargs['axes'] = axes
-        kwargs['title'] = 'auto'
-        kwargs['auto'] = True
-        plotCrossCorrelation(inDict, inDict, **kwargs)
-
-# For a single trace, this is synonymous with autocorrelation
-def plotCorrelogram(inDict, **kwargs):
+# -*- coding: utf-8 -*-
+"""
+Copyright (C) 2019 Event-driven Perception for Robotics
+Author: Sim Bamford
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
+plotCorrelogram receives "inDict", which is a container for (2D) polarity events, 
+(Or a higher level container), containing fields with numpy arrays:    
+    ts
+    x
+    y
+    pol
+Autocorrelation
+A correlogram is created for the chosen range of pixels.
+Choose the pixels by setting the kwargs:
+    xMin
+    xMax
+    yMin
+    yMax
+By default, all pixels are included. 
+By default, all pixels are autocorrelated individually, and then the results are 
+combined, so the end result is a mean over all pixels.
+TODO: Could do an autocorrelation for all spikes for the range together.
+minTime and maxTime are used to constrain time. 
+By default, polarities are combined; separate them with splitByPol=true
+numBins is interpretted as the number of time bins in each of positive 
+and negative directions, not including a central bin. 
+"""
+
+#%% Plot tsPix (single pixel timestamps)
+
+import matplotlib.pyplot as plt
+import numpy as np
+from tqdm import trange
+
+# local imports
+from .split import cropSpace, cropTime, splitByPolarity
+    
+# TODO: include a linear spacing option
+def defineBoundariesAndDensities(**kwargs):
+    numBins = kwargs.get('numBins', 50)
+    minOffset = kwargs.get('minOffset', 0.00001) # 10 us
+    maxOffset = kwargs.get('maxOffset', 1.0) # 100 ms
+    logSpacing = kwargs.get('spacing', 'linear') == 'log'
+    mirrored = kwargs.get('mirrored', True)
+    if logSpacing:
+        boundaries = np.geomspace(minOffset, maxOffset, numBins+1)
+        if mirrored:
+            boundaries = np.concatenate((-np.flip(boundaries), boundaries))
+        elif not mirrored:
+            boundaries = np.concatenate((np.zeros((1)), boundaries))        
+    elif (not logSpacing) and mirrored: # Linear; ignore minOffset
+        boundaries = np.linspace(-maxOffset, maxOffset, numBins*2)
+    elif (not logSpacing) and (not mirrored):
+        boundaries = np.linspace(0, maxOffset, (numBins))
+    # now there are boundaries either starting from zero ot mirrored around zero 
+    # for each bin, including a central bin, and the extreme boundaries 
+    # are the edge of the time region of interest.
+    widths = (boundaries[1:] - boundaries[:-1])
+    densities = 1 / widths
+    centres = (boundaries[1:] + boundaries[:-1]) / 2
+    return boundaries, densities, centres, widths
+
+def interSpikeInterval(ts, boundaries, densities, **kwargs):
+    hist = np.zeros((len(densities)), dtype=np.float64)
+    diff = ts[1:] - ts[:-1]
+    for idx, (boundary1, boundary2) in enumerate(zip(boundaries[:-1], boundaries[1:])):
+        hist[idx] = np.sum(np.logical_and(diff >= boundary1, diff <= boundary2))
+    hist = hist * densities
+    sumHist = np.sum(hist) # Avoid dividing by zero in case the hist is empty
+    if sumHist:
+        hist = hist / sumHist
+    return hist
+
+# Plot the timings of the spikes in events2 w.r.t. the spikes in events1
+def plotInterSpikeIntervalSingle(events, **kwargs):    
+    if (len(events['ts']) == 0):
+        return
+    # use other library functions to do spatiotemporal cropping
+    # If this is called from plotInterSpikeInterval then this has already been done, 
+    # But do it here as well so that this function can be independent.
+    events = cropSpace(events, **kwargs)
+    events = cropTime(events, zeroTime=False, **kwargs)
+    kwargs['mirrored'] = False
+    boundaries, densities, centres, widths = defineBoundariesAndDensities(**kwargs)
+    # Spatial cropping has happened; now iterate through defacto spatial range
+    minX = np.min(events['x'])
+    maxX = np.max(events['x'])
+    minY = np.min(events['y'])
+    maxY = np.max(events['y'])
+    hist = np.zeros((len(densities)), dtype=np.float64)
+    for currX in trange(minX, maxX+1, leave=True, position=0):
+        currXLogical = events['x']==currX
+        tsForCurrX = events['ts'][currXLogical]
+        yForCurrX = events['y'][currXLogical]
+        for currY in range(minY, maxY+1):
+            tsXY = tsForCurrX[yForCurrX==currY]
+            if np.any(tsXY): 
+                hist = hist + interSpikeInterval(tsXY, boundaries, densities, **kwargs)
+    # Normalise
+    weightedSum = np.sum(hist / densities)
+    if weightedSum > 0:
+        hist = hist / np.sum(weightedSum)
+    axes = kwargs.get('axes')
+    if axes is None:
+        fig, axes = plt.subplots()
+        kwargs['axes'] = axes
+
+    axes.bar(centres, hist, widths, antialiased=False)
+    #axes.set_ylim(minX + minY*numX - 1, maxX + maxY*numX + 1)
+    #plt.xticks(theRange, labels)
+    title = kwargs.get('title', '')
+    if kwargs.get('minX', False) or  kwargs.get('maxX', False):
+        title = title + ' ' + str(minX) + '<=X<=' + str(maxX)
+    if kwargs.get('minY', False) or  kwargs.get('maxY', False):
+        title = title + ' ' + str(minY) + '<=Y<=' + str(maxY)
+    axes.set_title(title)
+
+    callback = kwargs.get('callback')
+    if callback is not None:
+        callback(**kwargs) 
+        
+def plotInterSpikeInterval(inDict, **kwargs):
+    # Boilerplate for descending container hierarchy
+    if isinstance(inDict, list):
+        for inDictInst in inDict:
+            plotInterSpikeInterval(inDictInst, **kwargs)
+        return
+    if 'info' in inDict: # Top level container
+        fileName = inDict['info'].get('filePathOrName', '')
+        print('plotInterSpikeInterval was called for file ' + fileName)
+        if not inDict['data']:
+            print('The import contains no data.')
+            return
+        for channelName in inDict['data']:
+            channelData = inDict['data'][channelName]
+            if 'dvs' in channelData and len(channelData['dvs']['ts']) > 0:
+                kwargs['title'] = ' '.join([fileName, str(channelName)])
+                plotInterSpikeInterval(channelData['dvs'], **kwargs)
+            else:
+                print('Channel ' + channelName + ' skipped because it contains no polarity data')
+        return
+    print('plotInterSpikeInterval working: ' + kwargs.get('title', 'unnamed'))
+    # use other library functions to do spatiotemporal cropping
+    inDict = cropSpace(inDict, **kwargs)
+    inDict = cropTime(inDict, zeroTime=False, **kwargs)
+    if kwargs.get('splitByPol', False):
+        splitDict = splitByPolarity(inDict)        
+        fig, axes = plt.subplots(1, 3)
+
+        kwargs['axes'] = axes[0]
+        kwargs['title'] = 'on + off'
+        print(kwargs['title'])
+        plotInterSpikeIntervalSingle(inDict, **kwargs)
+
+        kwargs['axes'] = axes[1]
+        kwargs['title'] = 'off'
+        print(kwargs['title'])
+        plotInterSpikeIntervalSingle(splitDict['0'], **kwargs)
+
+        kwargs['axes'] = axes[2]
+        kwargs['title'] = 'on'
+        print(kwargs['title'])
+        plotInterSpikeIntervalSingle(splitDict['1'], **kwargs)
+
+    else:            
+        axes = kwargs.get('axes')
+        if axes is None:
+            fig, axes = plt.subplots()
+            kwargs['axes'] = axes
+        kwargs['title'] = 'auto'
+        plotInterSpikeIntervalSingle(inDict, **kwargs)
+    
+# Alias using common abbreviation
+def plotIsi(inDict, **kwargs):
+    plotInterSpikeInterval(inDict, **kwargs)
+
+def crossCorrelation(ts1, ts2, boundaries, densities, **kwargs):
+    hist = np.zeros((len(densities)), dtype=np.float64)
+    # TODO: think about a nice array-based way to do the following:
+    for ts in ts1:
+        firstIdx = np.searchsorted(ts2, ts+boundaries[0])
+        lastIdx = np.searchsorted(ts2, ts+boundaries[-1])
+        selectedTs2 = ts2[firstIdx: lastIdx] - ts
+        histIds = np.searchsorted(boundaries, selectedTs2) - 1
+        for histIdx in histIds:
+            try:
+                hist[histIdx] = hist[histIdx] + 1
+            except IndexError:
+                pass # Out of bounds - we don't want it
+    # If this was intended as an autocorrelation then we need to remove the 
+    # self-correlations
+    if kwargs.get('auto', False):
+        centreIdx = int(len(boundaries) / 2) - 1 
+        hist[centreIdx] = hist[centreIdx] - len(ts1)
+    hist = hist * densities
+    sumHist = np.sum(hist) # Avoid dividing by zero in case the hist is empty
+    if sumHist:
+        hist = hist / sumHist
+    return hist
+
+# Plot the timings of the spikes in events2 w.r.t. the spikes in events1
+def plotCrossCorrelation(events1, events2, **kwargs):    
+    if (len(events1['ts']) == 0) or (len(events2['ts']) == 0):
+        return
+    # use other library functions to do spatiotemporal cropping
+    # If this is called from plotautocorrelation then this has already been done, 
+    # But do it here as well so that this function can be independent.
+    events1 = cropSpace(events1, **kwargs)
+    events1 = cropTime(events1, zeroTime=False, **kwargs)
+    events2 = cropSpace(events2, **kwargs)
+    events2 = cropTime(events2, zeroTime=False, **kwargs)
+    boundaries, densities, centres, widths = defineBoundariesAndDensities(**kwargs)
+    # Spatial cropping has happened; now iterate through defacto spatial range
+    minX = min(np.min(events1['x']), np.min(events2['x']))
+    maxX = max(np.max(events1['x']), np.max(events2['x']))
+    minY = min(np.min(events1['y']), np.min(events2['y']))
+    maxY = max(np.max(events1['y']), np.max(events2['y']))
+    hist = np.zeros((len(densities)), dtype=np.float64)
+    # TODO: This loop could be much more efficient, following the pattern in plotInterSpikeInterval, above
+    for currX in trange(minX, maxX+1, leave=True, position=0): 
+        for currY in range(minY, maxY+1):
+            ts1 = events1['ts'][np.logical_and(events1['x']==currX, events1['y']==currY)]
+            ts2 = events2['ts'][np.logical_and(events2['x']==currX, events2['y']==currY)]
+            if np.any(ts1) and np.any(ts2): 
+                hist = hist + crossCorrelation(ts1, ts2, boundaries, densities, **kwargs)
+    # Normalise
+    weightedSum = np.sum(hist / densities)
+    if weightedSum > 0:
+        hist = hist / np.sum(weightedSum)
+    axes = kwargs.get('axes')
+    if axes is None:
+        fig, axes = plt.subplots()
+        kwargs['axes'] = axes
+
+    axes.bar(centres, hist, widths, antialiased=False)
+    #axes.set_ylim(minX + minY*numX - 1, maxX + maxY*numX + 1)
+    #plt.xticks(theRange, labels)
+    title = kwargs.get('title', '')
+    if kwargs.get('minX', False) or  kwargs.get('maxX', False):
+        title = title + ' ' + str(minX) + '<=X<=' + str(maxX)
+    if kwargs.get('minY', False) or  kwargs.get('maxY', False):
+        title = title + ' ' + str(minY) + '<=Y<=' + str(maxY)
+    axes.set_title(title)
+
+    callback = kwargs.get('callback')
+    if callback is not None:
+        callback(**kwargs)    
+
+def plotAutoCorrelation(inDict, **kwargs):
+    # Boilerplate for descending container hierarchy
+    if isinstance(inDict, list):
+        for inDictInst in inDict:
+            plotCorrelogram(inDictInst, **kwargs)
+        return
+    if 'info' in inDict: # Top level container
+        fileName = inDict['info'].get('filePathOrName', '')
+        print('plotAutocorrelation was called for file ' + fileName)
+        if not inDict['data']:
+            print('The import contains no data.')
+            return
+        for channelName in inDict['data']:
+            channelData = inDict['data'][channelName]
+            if 'dvs' in channelData and len(channelData['dvs']['ts']) > 0:
+                kwargs['title'] = ' '.join([fileName, str(channelName)])
+                plotCorrelogram(channelData['dvs'], **kwargs)
+            else:
+                print('Channel ' + channelName + ' skipped because it contains no polarity data')
+        return
+    print('plotAutocorrelation working: ' + kwargs.get('title', 'unnamed'))
+    # use other library functions to do spatiotemporal cropping
+    inDict = cropSpace(inDict, **kwargs)
+    inDict = cropTime(inDict, zeroTime=False, **kwargs)
+    if kwargs.get('splitByPol', False):
+        splitDict = splitByPolarity(inDict)        
+        fig, axes = plt.subplots(2, 2)
+
+        kwargs['axes'] = axes[0, 0]
+        kwargs['title'] = 'on + off auto'
+        print(kwargs['title'])
+        kwargs['auto'] = True
+        plotCrossCorrelation(inDict, inDict, **kwargs)
+
+        kwargs['axes'] = axes[0, 1]
+        kwargs['title'] = 'off auto'
+        print(kwargs['title'])
+        kwargs['auto'] = True
+        plotCrossCorrelation(splitDict['0'], splitDict['0'], **kwargs)
+
+        kwargs['axes'] = axes[1, 0]
+        kwargs['title'] = 'on auto'
+        print(kwargs['title'])
+        kwargs['auto'] = True
+        plotCrossCorrelation(splitDict['1'], splitDict['1'], **kwargs)
+
+        kwargs['axes'] = axes[1, 1]
+        kwargs['title'] = 'on w.r.t. off cross'
+        print(kwargs['title'])
+        kwargs['auto'] = False
+        plotCrossCorrelation(splitDict['0'], splitDict['1'], **kwargs)
+
+    elif kwargs.get('splitByPolAlt', False):
+        splitDict = splitByPolarity(inDict)        
+        fig, axes = plt.subplots(3, 1)
+        kwargs['axes'] = axes[0]
+        kwargs['title'] = 'on + off auto'
+        print(kwargs['title'])
+        kwargs['auto'] = True
+        plotCrossCorrelation(inDict, inDict, **kwargs)
+        kwargs['axes'] = axes[1]
+        kwargs['title'] = 'on w.r.t. off cross'
+        print(kwargs['title'])
+        kwargs['auto'] = False
+        plotCrossCorrelation(splitDict['0'], splitDict['1'], **kwargs)
+        kwargs['axes'] = axes[2]
+        kwargs['title'] = 'off w.r.t. on cross'
+        print(kwargs['title'])
+        kwargs['auto'] = False
+        plotCrossCorrelation(splitDict['1'], splitDict['0'], **kwargs)
+    else:            
+        axes = kwargs.get('axes')
+        if axes is None:
+            fig, axes = plt.subplots()
+            kwargs['axes'] = axes
+        kwargs['title'] = 'auto'
+        kwargs['auto'] = True
+        plotCrossCorrelation(inDict, inDict, **kwargs)
+
+# For a single trace, this is synonymous with autocorrelation
+def plotCorrelogram(inDict, **kwargs):
     plotAutoCorrelation(inDict, **kwargs)
```

### Comparing `bimvee-1.0.9/bimvee/plotDvsContrast.py` & `bimvee-1.0.9.dev0/bimvee/plotDvsContrast.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,292 +1,343 @@
-# -*- coding: utf-8 -*-
-'''
-Copyright (C) 2019 Event-driven Perception for Robotics
-Authors: Sim Bamford
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
-plotDvsContrast takes 'inDict' - a dict containing an imported ae file, 
-as created by importAe, and creates a series of green/red plots of
-polarity data.
-It creates a completely separate plot for each channel which contains 'pol' data
-Creates an image from events with contrast, by accumulating events up and down 
-to a maximum level at which full color is used. 
-The number of subplots is given by the numPlots parameter.
-'distributeBy' can either be 'time' or 'events', to decide how the points 
-around which data is rendered are chosen.
-The events are then recruited by the time points, spreading out until
-either they are about to overlap with a neighbouring point, or until 
-a certain ratio of a full array is reached. 
-
-Parameters which can be used:
- - numPlots
- - distributeBy
- - minTime, startTime
- - maxTime, endTime, stopTime
- - proportionOfPixels
- - contrast
- - flipVertical
- - flipHorizontal
- - transpose
-'''
-
-import numpy as np
-import matplotlib.pyplot as plt
-from math import log10, floor
-
-
-def roundToSf(x, sig=3):
-    try:
-        return round(x, sig - int(floor(log10(abs(x)))) - 1)
-    except ValueError:  # log of zero
-        return 0
-
-
-'''
-nomenclature:
-    idx = index
-    ids = indices
-'''
-
-
-def idsEventsInTimeRange(events, **kwargs):
-    startTime = kwargs.get('startTime', kwargs.get('minTime', kwargs.get('beginTime', events['ts'][0])))
-    endTime = kwargs.get('stopTime', kwargs.get('maxTime', kwargs.get('endTime', events['ts'][-1])))
-    # The following returns logical indices
-    # return (events['ts'] >= startTime) & (events['ts'] < endTime)
-    # Alternatively, search for the start and end indices, then return a range
-    # This might be faster, given that the ts array is already sorted
-    startIdx = np.searchsorted(events['ts'], startTime)
-    endIdx = np.searchsorted(events['ts'], endTime)
-    return range(startIdx, endIdx)
-
-
-def getEventsInTimeRange(events, **kwargs):
-    ids = kwargs.get('ids', idsEventsInTimeRange(events, **kwargs))
-    return {
-        'y': events['y'][ids],
-        'x': events['x'][ids],
-        'pol': events['pol'][ids]
-    }
-
-
-def getEventImage(events, **kwargs):
-    # dims might be in the events dict, but allow override from kwargs
-    try:
-        dimX = kwargs.get('dimX', events.get('dimX', np.max(events['x']) + 1))
-        dimY = kwargs.get('dimY', events.get('dimY', np.max(events['y']) + 1))
-    except ValueError:  # no defined dims and events arrays are empty
-        dimX = 1
-        dimY = 1
-    if kwargs.get('polarised', (kwargs.get('polarized'), True)):
-        eventImagePos = np.histogram2d(events['y'][events['pol']], 
-                                     events['x'][events['pol']], 
-                                     bins=[dimY, dimX],
-                                     range=[[0, dimY-1], [0, dimX-1]]
-                                     )[0]
-        eventImageNeg = np.histogram2d(events['y'][~events['pol']], 
-                                     events['x'][~events['pol']],
-                                     bins=[dimY, dimX],
-                                     range=[[0, dimY-1], [0, dimX-1]]
-                                     )[0]
-        if kwargs.get('pol_to_show') is None or kwargs.get('pol_to_show') == 'Both':
-            eventImage = eventImagePos - eventImageNeg
-        elif kwargs.get('pol_to_show') == 'Pos':
-            eventImage = eventImagePos
-        elif kwargs.get('pol_to_show') == 'Neg':
-            eventImage = - eventImageNeg
-    else:
-        eventImage = np.histogram2d(events['y'],
-                                    events['x'],
-                                    bins=[dimY, dimX],
-                                    range=[[0, dimY - 1], [0, dimX - 1]]
-                                    )[0]
-    # Clip the values according to the contrast
-    contrast = kwargs.get('contrast', 3)
-    eventImage = np.clip(eventImage, -contrast, contrast)
-    return eventImage
-
-
-def getEventImageForTimeRange(events, **kwargs):
-    events = getEventsInTimeRange(events, **kwargs)
-    return getEventImage(events, **kwargs)
-
-
-# This function accepts a dict of events and returns an event-image
-# formed by collecting count number of events in the past/future from time ts
-# direction =
-# -1 : look back in the past;
-# 1: look to the future
-def getEventImageByCount(events, **kwargs):
-    direction = kwargs.get('direction', -1)  # default direction is past
-    ts = kwargs.get('ts', 0)
-    count = kwargs.get('count', 0)
-    seedEventId = np.searchsorted(events['ts'], ts, side='right')
-    startOrEndEventId = min(max(seedEventId + direction * count, 0), len(events['ts']) - 1) # limit ID within range
-    startOrEndTime = events['ts'][startOrEndEventId]
-    firstEventId = min(seedEventId, startOrEndEventId)
-    lastEventId = max(seedEventId, startOrEndEventId)
-    selectedEvents = {
-        'y': events['y'][firstEventId:lastEventId],
-        'x': events['x'][firstEventId:lastEventId],
-        'pol': events['pol'][firstEventId:lastEventId]
-    }
-    return getEventImage(selectedEvents, **kwargs), startOrEndTime
-
-
-def plotDvsContrastSingle(inDict, **kwargs):
-    frameFromEvents = getEventImage(inDict, **kwargs)
-    if kwargs.get('transpose', False):
-        frameFromEvents = np.transpose(frameFromEvents)
-    if kwargs.get('flipVertical', False):
-        frameFromEvents = np.flip(frameFromEvents, axis=0)
-    if kwargs.get('flipHorizontal', False):
-        frameFromEvents = np.flip(frameFromEvents, axis=1)
-    contrast = kwargs.get('contrast', 3)
-    axes = kwargs.get('axes')
-    if axes is None:
-        fig, axes = plt.subplots()
-    if kwargs.get('polarised', (kwargs.get('polarized'), False)):
-        cmap = kwargs.get('cmap', kwargs.get('colormap', 'seismic_r'))
-        image = axes.imshow(frameFromEvents, cmap=cmap,
-                            vmin=-contrast, vmax=contrast)
-    else:
-        cmap = kwargs.get('cmap', kwargs.get('colormap', 'gray'))
-        image = axes.imshow(frameFromEvents, cmap=cmap,
-                            vmin=0, vmax=contrast)
-    axes.set_aspect('equal', adjustable='box')
-    title = kwargs.get('title')
-    if title is not None:
-        axes.set_title(title)
-
-    callback = kwargs.get('callback')
-    if callback is not None:
-        kwargs['axes'] = axes
-        callback(frameFromEvents=frameFromEvents, **kwargs)
-    return image
-
-
-def plotDvsContrast(inDicts, **kwargs):
-    if isinstance(inDicts, list):
-        for inDict in inDicts:
-            plotDvsContrast(inDict, **kwargs)
-        return
-    else:
-        inDict = inDicts
-    if not isinstance(inDict, dict):
-        return
-    if 'ts' not in inDict:
-        title = kwargs.pop('title', '')
-        if 'info' in inDict and isinstance(inDict, dict):
-            fileName = inDict['info'].get('filePathOrName')
-            if fileName is not None:
-                print('plotDvsContrast was called for file ' + fileName)
-                title = (title + ' ' + fileName).lstrip()
-        for key in inDict.keys():
-            kwargs['title'] = (title + ' ' + key).lstrip()
-            plotDvsContrast(inDict[key], **kwargs)
-        return
-    # From this point onwards, it's a data-type container
-    if 'pol' not in inDict:
-        return
-    # From this point onwards, it's a dvs container        
-
-    # The proportion of an array-full of events which is shown on a plot
-    proportionOfPixels = kwargs.get('proportionOfPixels', 0.1)
-    # useAllData overrides the above - the windows used for the images together include all the data 
-    useAllData = kwargs.get('useAllData', False)
-
-    numPlots = kwargs.get('numPlots', 6)
-
-    # Choice of distributing by 'time' or by 'numEvents'
-    distributeBy = kwargs.get('distributeBy', 'time').lower()
-
-    # % Distribute plots in a raster with a 3:4 ratio
-    numPlotsX = int(round(np.sqrt(numPlots / 3 * 4)))
-    numPlotsY = int(np.ceil(numPlots / numPlotsX))
-
-    # TODO: if the actual sensor size is known, use this instead of the following defaults
-    minX = kwargs.get('minX', inDict['x'].min())
-    maxX = kwargs.get('maxX', inDict['x'].max())
-    minY = kwargs.get('minY', inDict['y'].min())
-    maxY = kwargs.get('maxY', inDict['y'].max())
-    kwargs['minX'] = minX
-    kwargs['maxX'] = maxX
-    kwargs['minY'] = minY
-    kwargs['maxY'] = maxY
-
-    numPixelsInArray = (maxY + 1 - minY) * (maxX + 1 - minX)
-    numEventsToSelectEachWay = int(round(numPixelsInArray * proportionOfPixels / 2.0))
-
-    # The following section results in a set of tuples of first and last event idx
-    # one for each plot. It does this considering the choices of distributeBy, useAllData, and proportionOfPixels
-
-    # unpack ts for brevity
-    ts = inDict['ts']
-
-    minTime = kwargs.get('minTime', kwargs.get('startTime', kwargs.get('beginTime', ts.min())))
-    maxTime = kwargs.get('maxTime', kwargs.get('stopTime', kwargs.get('endTime', ts.max())))
-    minEventIdx = np.searchsorted(ts, minTime)
-    maxEventIdx = np.searchsorted(ts, maxTime)
-    numEvents = maxEventIdx - minEventIdx
-    if distributeBy == 'time':
-        totalTime = maxTime - minTime
-        timeStep = totalTime / numPlots
-        if useAllData:
-            timeBoundaries = np.arange(minTime, maxTime + timeStep / 2, timeStep)
-            firstEventIds = [
-                np.where(ts >= timeBoundary)[0][0]
-                for timeBoundary in timeBoundaries]
-            lastEventIds = [firstEventIdx - 1 for firstEventIdx in firstEventIds]
-            lastEventIds = lastEventIds[1:]
-            firstEventIds = firstEventIds[:-1]
-        else:
-            timeCentres = np.arange(minTime + timeStep * 0.5, maxTime, timeStep)
-            centreEventIds = np.searchsorted(ts, timeCentres)
-            firstEventIds = [idx - numEventsToSelectEachWay for idx in centreEventIds]
-            lastEventIds = [idx + numEventsToSelectEachWay for idx in centreEventIds]
-    else:  # distribute by event number
-        eventsPerStep = int(numEvents / numPlots)
-        if useAllData:
-            firstEventIds = range(minEventIdx, maxEventIdx, eventsPerStep)
-            lastEventIds = [firstEventIdx - 1 for firstEventIdx in firstEventIds]
-            lastEventIds = lastEventIds[1:]
-            firstEventIds = firstEventIds[:-1]
-        else:
-            centreEventIds = range(int(eventsPerStep / 2), numEvents, eventsPerStep)
-            firstEventIds = [idx - numEventsToSelectEachWay for idx in centreEventIds]
-            lastEventIds = [idx + numEventsToSelectEachWay for idx in centreEventIds]
-    firstEventIds = np.clip(firstEventIds, minEventIdx, maxEventIdx - 1)
-    lastEventIds = np.clip(lastEventIds, minEventIdx, maxEventIdx - 1)
-    firstTimes = ts[firstEventIds]
-    lastTimes = ts[lastEventIds]
-    timeCentres = (firstTimes + lastTimes) / 2
-    titles = [
-        str(roundToSf(firstTime)) + ' - ' + str(roundToSf(lastTime)) + ' s'
-        for firstTime, lastTime in zip(firstTimes, lastTimes)]
-
-    fig, allAxes = plt.subplots(numPlotsY, numPlotsX)
-    if numPlots == 1:
-        allAxes = [allAxes]
-    else:
-        allAxes = allAxes.flatten()
-    fig.suptitle(kwargs.get('title', ''))
-
-    for axes, firstEventIdx, lastEventIdx, title in zip(allAxes, firstEventIds, lastEventIds, titles):
-        dvsDataDict = {
-            'x': inDict['x'][firstEventIdx:lastEventIdx],
-            'y': inDict['y'][firstEventIdx:lastEventIdx],
-            'pol': inDict['pol'][firstEventIdx:lastEventIdx],
-            'ts': inDict['ts'][firstEventIdx:lastEventIdx]
-        }
-        kwargs['title'] = title
-        image = plotDvsContrastSingle(inDict=dvsDataDict, axes=axes, **kwargs)
-    fig.colorbar(image)
-    return timeCentres
+# -*- coding: utf-8 -*-
+'''
+Copyright (C) 2019 Event-driven Perception for Robotics
+Authors: Sim Bamford
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
+plotDvsContrast takes 'inDict' - a dict containing an imported ae file, 
+as created by importAe, and creates a series of green/red plots of
+polarity data.
+It creates a completely separate plot for each channel which contains 'pol' data
+Creates an image from events with contrast, by accumulating events up and down 
+to a maximum level at which full color is used. 
+The number of subplots is given by the numPlots parameter.
+'distributeBy' can either be 'time' or 'events', to decide how the points 
+around which data is rendered are chosen.
+The events are then recruited by the time points, spreading out until
+either they are about to overlap with a neighbouring point, or until 
+a certain ratio of a full array is reached. 
+
+Parameters which can be used:
+ - numPlots
+ - distributeBy
+ - minTime, startTime
+ - maxTime, endTime, stopTime
+ - proportionOfPixels
+ - contrast
+ - flipVertical
+ - flipHorizontal
+ - transpose
+'''
+
+import numpy as np
+import matplotlib.pyplot as plt
+from math import log10, floor
+
+from .split import selectByRange
+
+
+def roundToSf(x, sig=3):
+    try:
+        return round(x, sig - int(floor(log10(abs(x)))) - 1)
+    except ValueError:  # log of zero
+        return 0
+
+
+'''
+nomenclature:
+    idx = index
+    ids = indices
+'''
+
+
+def idsEventsInTimeRange(events, **kwargs):
+    startTime = kwargs.get('startTime', kwargs.get('minTime', kwargs.get('beginTime', events['ts'][0])))
+    endTime = kwargs.get('stopTime', kwargs.get('maxTime', kwargs.get('endTime', events['ts'][-1])))
+    # The following returns logical indices
+    # return (events['ts'] >= startTime) & (events['ts'] < endTime)
+    # Alternatively, search for the start and end indices, then return a range
+    # This might be faster, given that the ts array is already sorted
+    startIdx = np.searchsorted(events['ts'], startTime)
+    endIdx = np.searchsorted(events['ts'], endTime)
+    return range(startIdx, endIdx)
+
+
+def getEventsInTimeRange(events, **kwargs):
+    ids = kwargs.get('ids', idsEventsInTimeRange(events, **kwargs))
+    return {
+        'y': events['y'][ids],
+        'x': events['x'][ids],
+        'pol': events['pol'][ids],
+        'ts': events['ts'][ids]
+    }
+
+
+def getEventImage(events, **kwargs):
+    # dims might be in the events dict, but allow override from kwargs
+    try:
+        dimX = kwargs.get('dimX', events.get('dimX', np.max(events['x']) + 1))
+        dimY = kwargs.get('dimY', events.get('dimY', np.max(events['y']) + 1))
+    except ValueError:  # no defined dims and events arrays are empty
+        dimX = 1
+        dimY = 1
+    try:
+        if kwargs.get('image_type') == 'count':
+            eventImagePos = np.histogram2d(events['y'][events['pol']],
+                                         events['x'][events['pol']],
+                                         bins=[dimY, dimX],
+                                         range=[[-0.5, dimY-0.5], [-0.5, dimX-0.5]]
+                                         )[0]
+            eventImageNeg = np.histogram2d(events['y'][~events['pol']],
+                                         events['x'][~events['pol']],
+                                         bins=[dimY, dimX],
+                                         range=[[-0.5, dimY-0.5], [-0.5, dimX-0.5]]
+                                         )[0]
+            if kwargs.get('pol_to_show') is None or kwargs.get('pol_to_show') == 'Both':
+                eventImage = eventImagePos - eventImageNeg
+            elif kwargs.get('pol_to_show') == 'Pos':
+                eventImage = eventImagePos
+            elif kwargs.get('pol_to_show') == 'Neg':
+                eventImage = - eventImageNeg
+        elif kwargs.get('image_type') == 'not_polarized':
+            eventImage = np.histogram2d(events['y'],
+                                        events['x'],
+                                        bins=[dimY, dimX],
+                                        range=[[-0.5, dimY-0.5], [-0.5, dimX-0.5]]
+                                        )[0]
+        elif kwargs.get('image_type') == 'time_image':
+            eventImage = np.zeros((dimY, dimX))
+            eventImage[events['y'], events['x']] = (events['ts'] - events['ts'][0])
+            eventImage = eventImage / eventImage.max()
+        elif kwargs.get('image_type') == 'binary':
+            eventImage = np.zeros((dimY, dimX))
+            if kwargs.get('pol_to_show') is None or kwargs.get('pol_to_show') == 'Both':
+                eventImage[events['y'], events['x']] = (events['pol'].astype(int) * 2 - 1)
+            elif kwargs.get('pol_to_show') == 'Pos':
+                eventImage[events['y'][events['pol']], events['x'][events['pol']]] = 1
+            elif kwargs.get('pol_to_show') == 'Neg':
+                eventImage[events['y'][~events['pol']], events['x'][~events['pol']]] = -1
+        elif kwargs.get('image_type') == 'coloured':
+            pos_colour = [255, 0, 0]
+            neg_colour = [0, 0, 255]
+            eventImage = np.full((dimY, dimX, 3), 255, dtype=np.uint8)
+            if kwargs.get('pol_to_show') is None or kwargs.get('pol_to_show') == 'Both':
+                eventImage[events['y'], events['x']] = [pos_colour if p else neg_colour for p in events['pol']]
+            elif kwargs.get('pol_to_show') == 'Pos':
+                eventImage[events['y'][events['pol']], events['x'][events['pol']]] = pos_colour
+            elif kwargs.get('pol_to_show') == 'Neg':
+                eventImage[events['y'][~events['pol']], events['x'][~events['pol']]] = neg_colour
+    except ValueError:
+        pass
+    except IndexError:
+        pass
+    # Clip the values according to the contrast
+    if not kwargs.get('image_type') == 'coloured':
+        contrast = kwargs.get('contrast', 3)
+        eventImage = np.clip(eventImage, -contrast, contrast)
+    return eventImage
+
+
+def getEventImageForTimeRange(events, **kwargs):
+    events = getEventsInTimeRange(events, **kwargs)
+    return getEventImage(events, **kwargs)
+
+
+'''
+This function accepts a dict of events and returns a new event dict
+formed by collecting count number of events in the past/future from time ts
+direction:
+  -1: look back in the past;
+  0: look equally to past and future;
+  1: look to the future
+'''
+def getEventsByCount(events, **kwargs):
+    direction = kwargs.get('direction', -1)  # default direction is past
+    ts = kwargs.get('ts', 0)
+    count = kwargs.get('count', 0)
+    seedEventId = np.searchsorted(events['ts'], ts, side='right')
+    if direction == 0:
+        halfCount = int(count/2)
+        firstEventId = max(seedEventId - halfCount, 0)
+        lastEventId = min(seedEventId + halfCount, len(events['ts']) - 1)
+        # startOrEndTime reports end time in this case
+        startOrEndTime = events['ts'][lastEventId]
+    else:
+        startOrEndEventId = min(max(seedEventId + direction * count, 0), 
+                                len(events['ts']) - 1) # limit ID within range
+        startOrEndTime = events['ts'][startOrEndEventId]
+        firstEventId = min(seedEventId, startOrEndEventId)
+        lastEventId = max(seedEventId, startOrEndEventId)
+    selectedEvents = selectByRange(events, firstEventId, lastEventId + 1)
+    return selectedEvents, startOrEndTime
+
+
+'''
+This function accepts a dict of events and returns an event-image
+formed by collecting count number of events in the past/future from time ts
+direction:
+  -1: look back in the past;
+  0: look equally to past and future;
+  1: look to the future
+'''
+def getEventImageByCount(events, **kwargs):
+    selectedEvents, startOrEndTime = getEventsByCount(events, **kwargs)
+    return getEventImage(selectedEvents, **kwargs), startOrEndTime
+
+
+def plotDvsContrastSingle(inDict, **kwargs):
+    frameFromEvents = getEventImage(inDict, **kwargs)
+    if kwargs.get('transpose', False):
+        frameFromEvents = np.transpose(frameFromEvents)
+    if kwargs.get('flipVertical', False):
+        frameFromEvents = np.flip(frameFromEvents, axis=0)
+    if kwargs.get('flipHorizontal', False):
+        frameFromEvents = np.flip(frameFromEvents, axis=1)
+    contrast = kwargs.get('contrast', 3)
+    axes = kwargs.get('axes')
+    if axes is None:
+        fig, axes = plt.subplots()
+    if kwargs.get('polarised', (kwargs.get('polarized'), False)):
+        cmap = kwargs.get('cmap', kwargs.get('colormap', 'seismic_r'))
+        image = axes.imshow(frameFromEvents, cmap=cmap,
+                            vmin=-contrast, vmax=contrast)
+    else:
+        cmap = kwargs.get('cmap', kwargs.get('colormap', 'gray'))
+        image = axes.imshow(frameFromEvents, cmap=cmap,
+                            vmin=0, vmax=contrast)
+    axes.set_aspect('equal', adjustable='box')
+    title = kwargs.get('title')
+    if title is not None:
+        axes.set_title(title)
+
+    callback = kwargs.get('callback')
+    if callback is not None:
+        kwargs['axes'] = axes
+        callback(frameFromEvents=frameFromEvents, **kwargs)
+    return image
+
+
+def plotDvsContrast(inDicts, **kwargs):
+    if isinstance(inDicts, list):
+        for inDict in inDicts:
+            plotDvsContrast(inDict, **kwargs)
+        return
+    else:
+        inDict = inDicts
+    if not isinstance(inDict, dict):
+        return
+    if 'ts' not in inDict:
+        title = kwargs.pop('title', '')
+        if 'info' in inDict and isinstance(inDict, dict):
+            fileName = inDict['info'].get('filePathOrName')
+            if fileName is not None:
+                print('plotDvsContrast was called for file ' + fileName)
+                title = (title + ' ' + fileName).lstrip()
+        for key in inDict.keys():
+            kwargs['title'] = (title + ' ' + key).lstrip()
+            plotDvsContrast(inDict[key], **kwargs)
+        return
+    # From this point onwards, it's a data-type container
+    if 'pol' not in inDict:
+        return
+    # From this point onwards, it's a dvs container        
+
+    # The proportion of an array-full of events which is shown on a plot
+    proportionOfPixels = kwargs.get('proportionOfPixels', 0.1)
+    # useAllData overrides the above - the windows used for the images together include all the data 
+    useAllData = kwargs.get('useAllData', False)
+
+    numPlots = kwargs.get('numPlots', 6)
+
+    # Choice of distributing by 'time' or by 'numEvents'
+    distributeBy = kwargs.get('distributeBy', 'time').lower()
+
+    # % Distribute plots in a raster with a 3:4 ratio
+    numPlotsX = int(round(np.sqrt(numPlots / 3 * 4)))
+    numPlotsY = int(np.ceil(numPlots / numPlotsX))
+
+    # TODO: if the actual sensor size is known, use this instead of the following defaults
+    minX = kwargs.get('minX', inDict['x'].min())
+    maxX = kwargs.get('maxX', inDict['x'].max())
+    minY = kwargs.get('minY', inDict['y'].min())
+    maxY = kwargs.get('maxY', inDict['y'].max())
+    kwargs['minX'] = minX
+    kwargs['maxX'] = maxX
+    kwargs['minY'] = minY
+    kwargs['maxY'] = maxY
+
+    numPixelsInArray = (maxY + 1 - minY) * (maxX + 1 - minX)
+    numEventsToSelectEachWay = int(round(numPixelsInArray * proportionOfPixels / 2.0))
+
+    # The following section results in a set of tuples of first and last event idx
+    # one for each plot. It does this considering the choices of distributeBy, useAllData, and proportionOfPixels
+
+    # unpack ts for brevity
+    ts = inDict['ts']
+
+    minTime = kwargs.get('minTime', kwargs.get('startTime', kwargs.get('beginTime', ts.min())))
+    maxTime = kwargs.get('maxTime', kwargs.get('stopTime', kwargs.get('endTime', ts.max())))
+    minEventIdx = np.searchsorted(ts, minTime)
+    maxEventIdx = np.searchsorted(ts, maxTime)
+    numEvents = maxEventIdx - minEventIdx
+    if distributeBy == 'time':
+        totalTime = maxTime - minTime
+        timeStep = totalTime / numPlots
+        if useAllData:
+            timeBoundaries = np.arange(minTime, maxTime + timeStep / 2, timeStep)
+            firstEventIds = [
+                np.where(ts >= timeBoundary)[0][0]
+                for timeBoundary in timeBoundaries]
+            lastEventIds = [firstEventIdx - 1 for firstEventIdx in firstEventIds]
+            lastEventIds = lastEventIds[1:]
+            firstEventIds = firstEventIds[:-1]
+        else:
+            timeCentres = np.arange(minTime + timeStep * 0.5, maxTime, timeStep)
+            centreEventIds = np.searchsorted(ts, timeCentres)
+            firstEventIds = [idx - numEventsToSelectEachWay for idx in centreEventIds]
+            lastEventIds = [idx + numEventsToSelectEachWay for idx in centreEventIds]
+    else:  # distribute by event number
+        eventsPerStep = int(numEvents / numPlots)
+        if useAllData:
+            firstEventIds = range(minEventIdx, maxEventIdx, eventsPerStep)
+            lastEventIds = [firstEventIdx - 1 for firstEventIdx in firstEventIds]
+            lastEventIds = lastEventIds[1:]
+            firstEventIds = firstEventIds[:-1]
+        else:
+            centreEventIds = range(int(eventsPerStep / 2), numEvents, eventsPerStep)
+            firstEventIds = [idx - numEventsToSelectEachWay for idx in centreEventIds]
+            lastEventIds = [idx + numEventsToSelectEachWay for idx in centreEventIds]
+    firstEventIds = np.clip(firstEventIds, minEventIdx, maxEventIdx - 1)
+    lastEventIds = np.clip(lastEventIds, minEventIdx, maxEventIdx - 1)
+    firstTimes = ts[firstEventIds]
+    lastTimes = ts[lastEventIds]
+    timeCentres = (firstTimes + lastTimes) / 2
+    titles = [
+        str(roundToSf(firstTime)) + ' - ' + str(roundToSf(lastTime)) + ' s'
+        for firstTime, lastTime in zip(firstTimes, lastTimes)]
+
+    fig, allAxes = plt.subplots(numPlotsY, numPlotsX)
+    if numPlots == 1:
+        allAxes = [allAxes]
+    else:
+        allAxes = allAxes.flatten()
+    fig.suptitle(kwargs.get('title', ''))
+
+    for axes, firstEventIdx, lastEventIdx, title in zip(allAxes, firstEventIds, lastEventIds, titles):
+        dvsDataDict = {
+            'x': inDict['x'][firstEventIdx:lastEventIdx],
+            'y': inDict['y'][firstEventIdx:lastEventIdx],
+            'pol': inDict['pol'][firstEventIdx:lastEventIdx],
+            'ts': inDict['ts'][firstEventIdx:lastEventIdx]
+        }
+        kwargs['title'] = title
+        image = plotDvsContrastSingle(inDict=dvsDataDict, axes=axes, **kwargs)
+    fig.colorbar(image)
+    return timeCentres
```

### Comparing `bimvee-1.0.9/bimvee/plotDvsLastTs.py` & `bimvee-1.0.9.dev0/bimvee/plotDvsLastTs.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,176 +1,176 @@
-# -*- coding: utf-8 -*-
-'''
-Copyright (C) 2019 Event-driven Perception for Robotics
-Authors: Sim Bamford
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
-plotDvsLastTs takes a dict containing address-event data. 
-Minimally, there must be x, y, and ts fields. 
-For a given "time" (or a list of times, in which case subplots), 
-creates a plot in which pixels are ordered according to their
-last time stamp, and the order is represented by colour from red (recent)
-to blue (oldest) through the spectrum.
-
-Parameters which can be used:
- - time
- - minX
- - minY
- - maxX
- - maxY
- - flipVertical, flipHorizontal, transpose (applied in this order)
- - title
- - axis (to plot on; if not passed in, a new figure is created)
- - cmap
-'''
-
-import numpy as np
-import matplotlib.pyplot as plt
-from math import log10, floor
-import matplotlib.colors as colors
-
-# Optional import of rankdata method from scipy
-try: 
-    from scipy.stats import rankdata
-except ModuleNotFoundError:
-    # Stripped down version of implementation from scipy
-    def rankdata(a, method='average'):
-        arr = np.ravel(np.asarray(a))
-        algo = 'mergesort' if method == 'ordinal' else 'quicksort'
-        sorter = np.argsort(arr, kind=algo)
-        inv = np.empty(sorter.size, dtype=np.intp)
-        inv[sorter] = np.arange(sorter.size, dtype=np.intp)
-        if method == 'ordinal':
-            return inv + 1
-        arr = arr[sorter]
-        obs = np.r_[True, arr[1:] != arr[:-1]]
-        dense = obs.cumsum()[inv]
-        # cumulative counts of each unique value
-        count = np.r_[np.nonzero(obs)[0], len(obs)]
-        # average method
-        return .5 * (count[dense] + count[dense - 1] + 1)
-
-def roundToSf(x, sig=3): # https://stackoverflow.com/questions/3410976/how-to-round-a-number-to-significant-figures-in-python
-    try:
-        return round(x, sig-int(floor(log10(abs(x))))-1)
-    except ValueError: # log of zero
-        return 0
-
-def plotDvsLastTsSingle(inDict, **kwargs):
-    
-    time = kwargs.get('time', kwargs.get('maxTime', kwargs.get('lastTime', 
-           kwargs.get('ts', kwargs.get('maxTs', kwargs.get('lastTs', 
-           np.max(inDict['ts'])))))))
-    minTime = kwargs.get('minTime', kwargs.get('firstTime', 
-              kwargs.get('minTs', kwargs.get('firstTs', 
-              np.min(inDict['ts'])))))
-        
-    # TODO: if the actual sensor size is known, use this instead of the following 
-    minY = kwargs.get('minY',inDict['y'].min())
-    maxY = kwargs.get('maxY',inDict['y'].max())
-    minX = kwargs.get('minX',inDict['x'].min())
-    maxX = kwargs.get('maxX',inDict['x'].max())
-    sizeX = maxX - minX + 1
-    sizeY = maxY - minY + 1
-    tsArray = np.ones((sizeY, sizeX), dtype=np.float64) * -1
-
-    # populate the array by running time forward to time
-    chosenLogical = inDict['ts'] <= time
-    chosenLogical &= inDict['ts'] >= minTime
-    chosenLogical &= inDict['x'] >= minX
-    chosenLogical &= inDict['x'] <= maxX
-    chosenLogical &= inDict['y'] >= minY
-    chosenLogical &= inDict['y'] <= maxY
-    xChosen = inDict['x'][chosenLogical] - minX
-    yChosen = inDict['y'][chosenLogical] - minY
-    tsChosen = inDict['ts'][chosenLogical]
-    for x, y, ts in zip(xChosen, yChosen, tsChosen):
-        tsArray[y, x] = ts         
-    
-    ordinal = kwargs.get('ordinal', False)
-    if ordinal:
-        tsArrayFlattened = tsArray.flatten()
-        tsOrdinal = rankdata(tsArrayFlattened, method='dense') - 1 # min rank is 1
-        if np.any(tsArrayFlattened == -1):
-            tsOrdinal -= 1 # If there are unset timestamps, they will have rank 0 - push these to -1
-        tsArray = tsOrdinal.reshape(tsArray.shape)
-    else:
-        pass # TODO: cardinal
-    axes = kwargs.get('axes')
-    if axes is None:
-        fig, axes = plt.subplots()
-        kwargs['axes'] = axes
-
-    transpose = kwargs.get('transpose', False)
-    if transpose:
-        tsArray = np.transpose(tsArray)
-    cmap = plt.get_cmap(kwargs.get('cmap', 'jet'))
-    cmap.set_under(color='white')
-    image = axes.imshow(tsArray, cmap=cmap, norm=colors.Normalize(vmin=0, vmax=np.max(tsArray)))
-    axes.set_aspect('equal', adjustable='box')
-    axes.grid(b=False)
-    if kwargs.get('flipVertical', False):
-        axes.invert_yaxis()
-    if kwargs.get('flipHorizontal', False):
-        axes.invert_xaxis()
-    title = kwargs.get('title')
-    if title is not None:
-        axes.set_title(title)
-    axes.set_title(str(roundToSf(minTime)) + ' - ' + str(roundToSf(time)) + ' s')
-    
-    callback = kwargs.get('callback')
-    if callback is not None:
-        callback(tsArray=tsArray, **kwargs)
-    
-    return image
-
-def plotDvsLastTs(inDict, **kwargs):
-    # Boilerplate for descending higher level containers
-    if isinstance(inDict, list):
-        for inDictInst in inDict:
-            plotDvsLastTs(inDictInst, **kwargs)
-        return
-    if 'info' in inDict: # Top level container
-        fileName = inDict['info'].get('filePathOrName', '')
-        print('plotDvsContrast was called for file ' + fileName)
-        if not inDict['data']:
-            print('The import contains no data.')
-            return
-        for channelName in inDict['data']:
-            channelData = inDict['data'][channelName]
-            if 'dvs' in channelData and len(channelData['dvs']['ts']) > 0:
-                kwargs['title'] = ' '.join([fileName, str(channelName)])
-                plotDvsLastTs(channelData['dvs'], **kwargs)
-            else:
-                print('Channel ' + channelName + ' skipped because it contains no polarity data')
-        return
-    times = kwargs.get('time', kwargs.get('maxTime', kwargs.get('lastTime', 
-           kwargs.get('ts', kwargs.get('maxTs', kwargs.get('lastTs', 
-           np.max(inDict['ts'])))))))
-    minTimes = kwargs.get('minTime', kwargs.get('firstTime', 
-              kwargs.get('minTs', kwargs.get('firstTs', 
-              np.min(inDict['ts'])))))
-    if np.isscalar(times):
-        times = [times]
-        minTimes = [minTimes]
-    numPlots = len(times)
-    numPlotsX = int(round(np.sqrt(numPlots / 3 * 4)))
-    numPlotsY = int(np.ceil(numPlots / numPlotsX))
-    fig, allAxes = plt.subplots(numPlotsY, numPlotsX)
-    if numPlots == 1:
-        allAxes = [allAxes]
-    else:
-        allAxes = allAxes.flatten()
-    fig.suptitle(kwargs.get('title', ''))
-    for time, minTime, axes in zip(times, minTimes, allAxes):
-        kwargs['time'] = time
-        kwargs['minTime'] = minTime
-        kwargs['axes'] = axes
-        plotDvsLastTsSingle(inDict, **kwargs)
+# -*- coding: utf-8 -*-
+'''
+Copyright (C) 2019 Event-driven Perception for Robotics
+Authors: Sim Bamford
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
+plotDvsLastTs takes a dict containing address-event data. 
+Minimally, there must be x, y, and ts fields. 
+For a given "time" (or a list of times, in which case subplots), 
+creates a plot in which pixels are ordered according to their
+last time stamp, and the order is represented by colour from red (recent)
+to blue (oldest) through the spectrum.
+
+Parameters which can be used:
+ - time
+ - minX
+ - minY
+ - maxX
+ - maxY
+ - flipVertical, flipHorizontal, transpose (applied in this order)
+ - title
+ - axis (to plot on; if not passed in, a new figure is created)
+ - cmap
+'''
+
+import numpy as np
+import matplotlib.pyplot as plt
+from math import log10, floor
+import matplotlib.colors as colors
+
+# Optional import of rankdata method from scipy
+try: 
+    from scipy.stats import rankdata
+except ModuleNotFoundError:
+    # Stripped down version of implementation from scipy
+    def rankdata(a, method='average'):
+        arr = np.ravel(np.asarray(a))
+        algo = 'mergesort' if method == 'ordinal' else 'quicksort'
+        sorter = np.argsort(arr, kind=algo)
+        inv = np.empty(sorter.size, dtype=np.intp)
+        inv[sorter] = np.arange(sorter.size, dtype=np.intp)
+        if method == 'ordinal':
+            return inv + 1
+        arr = arr[sorter]
+        obs = np.r_[True, arr[1:] != arr[:-1]]
+        dense = obs.cumsum()[inv]
+        # cumulative counts of each unique value
+        count = np.r_[np.nonzero(obs)[0], len(obs)]
+        # average method
+        return .5 * (count[dense] + count[dense - 1] + 1)
+
+def roundToSf(x, sig=3): # https://stackoverflow.com/questions/3410976/how-to-round-a-number-to-significant-figures-in-python
+    try:
+        return round(x, sig-int(floor(log10(abs(x))))-1)
+    except ValueError: # log of zero
+        return 0
+
+def plotDvsLastTsSingle(inDict, **kwargs):
+    
+    time = kwargs.get('time', kwargs.get('maxTime', kwargs.get('lastTime', 
+           kwargs.get('ts', kwargs.get('maxTs', kwargs.get('lastTs', 
+           np.max(inDict['ts'])))))))
+    minTime = kwargs.get('minTime', kwargs.get('firstTime', 
+              kwargs.get('minTs', kwargs.get('firstTs', 
+              np.min(inDict['ts'])))))
+        
+    # TODO: if the actual sensor size is known, use this instead of the following 
+    minY = kwargs.get('minY',inDict['y'].min())
+    maxY = kwargs.get('maxY',inDict['y'].max())
+    minX = kwargs.get('minX',inDict['x'].min())
+    maxX = kwargs.get('maxX',inDict['x'].max())
+    sizeX = maxX - minX + 1
+    sizeY = maxY - minY + 1
+    tsArray = np.ones((sizeY, sizeX), dtype=np.float64) * -1
+
+    # populate the array by running time forward to time
+    chosenLogical = inDict['ts'] <= time
+    chosenLogical &= inDict['ts'] >= minTime
+    chosenLogical &= inDict['x'] >= minX
+    chosenLogical &= inDict['x'] <= maxX
+    chosenLogical &= inDict['y'] >= minY
+    chosenLogical &= inDict['y'] <= maxY
+    xChosen = inDict['x'][chosenLogical] - minX
+    yChosen = inDict['y'][chosenLogical] - minY
+    tsChosen = inDict['ts'][chosenLogical]
+    for x, y, ts in zip(xChosen, yChosen, tsChosen):
+        tsArray[y, x] = ts         
+    
+    ordinal = kwargs.get('ordinal', False)
+    if ordinal:
+        tsArrayFlattened = tsArray.flatten()
+        tsOrdinal = rankdata(tsArrayFlattened, method='dense') - 1 # min rank is 1
+        if np.any(tsArrayFlattened == -1):
+            tsOrdinal -= 1 # If there are unset timestamps, they will have rank 0 - push these to -1
+        tsArray = tsOrdinal.reshape(tsArray.shape)
+    else:
+        pass # TODO: cardinal
+    axes = kwargs.get('axes')
+    if axes is None:
+        fig, axes = plt.subplots()
+        kwargs['axes'] = axes
+
+    transpose = kwargs.get('transpose', False)
+    if transpose:
+        tsArray = np.transpose(tsArray)
+    cmap = plt.get_cmap(kwargs.get('cmap', 'jet'))
+    cmap.set_under(color='white')
+    image = axes.imshow(tsArray, cmap=cmap, norm=colors.Normalize(vmin=0, vmax=np.max(tsArray)))
+    axes.set_aspect('equal', adjustable='box')
+    axes.grid(b=False)
+    if kwargs.get('flipVertical', False):
+        axes.invert_yaxis()
+    if kwargs.get('flipHorizontal', False):
+        axes.invert_xaxis()
+    title = kwargs.get('title')
+    if title is not None:
+        axes.set_title(title)
+    axes.set_title(str(roundToSf(minTime)) + ' - ' + str(roundToSf(time)) + ' s')
+    
+    callback = kwargs.get('callback')
+    if callback is not None:
+        callback(tsArray=tsArray, **kwargs)
+    
+    return image
+
+def plotDvsLastTs(inDict, **kwargs):
+    # Boilerplate for descending higher level containers
+    if isinstance(inDict, list):
+        for inDictInst in inDict:
+            plotDvsLastTs(inDictInst, **kwargs)
+        return
+    if 'info' in inDict: # Top level container
+        fileName = inDict['info'].get('filePathOrName', '')
+        print('plotDvsContrast was called for file ' + fileName)
+        if not inDict['data']:
+            print('The import contains no data.')
+            return
+        for channelName in inDict['data']:
+            channelData = inDict['data'][channelName]
+            if 'dvs' in channelData and len(channelData['dvs']['ts']) > 0:
+                kwargs['title'] = ' '.join([fileName, str(channelName)])
+                plotDvsLastTs(channelData['dvs'], **kwargs)
+            else:
+                print('Channel ' + channelName + ' skipped because it contains no polarity data')
+        return
+    times = kwargs.get('time', kwargs.get('maxTime', kwargs.get('lastTime', 
+           kwargs.get('ts', kwargs.get('maxTs', kwargs.get('lastTs', 
+           np.max(inDict['ts'])))))))
+    minTimes = kwargs.get('minTime', kwargs.get('firstTime', 
+              kwargs.get('minTs', kwargs.get('firstTs', 
+              np.min(inDict['ts'])))))
+    if np.isscalar(times):
+        times = [times]
+        minTimes = [minTimes]
+    numPlots = len(times)
+    numPlotsX = int(round(np.sqrt(numPlots / 3 * 4)))
+    numPlotsY = int(np.ceil(numPlots / numPlotsX))
+    fig, allAxes = plt.subplots(numPlotsY, numPlotsX)
+    if numPlots == 1:
+        allAxes = [allAxes]
+    else:
+        allAxes = allAxes.flatten()
+    fig.suptitle(kwargs.get('title', ''))
+    for time, minTime, axes in zip(times, minTimes, allAxes):
+        kwargs['time'] = time
+        kwargs['minTime'] = minTime
+        kwargs['axes'] = axes
+        plotDvsLastTsSingle(inDict, **kwargs)
```

### Comparing `bimvee-1.0.9/bimvee/plotEventRate.py` & `bimvee-1.0.9.dev0/bimvee/plotEventRate.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-# -*- coding: utf-8 -*-
-'''
-Copyright (C) 2019 Event-driven Perception for Robotics
-Authors: Sim Bamford
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
-plotEventRate takes 'inDict' - a dict containing an imported ae file, 
-as created by importAe, and creates a series of plots of event rates.
-It creates one plot for each dataType dct contianing a 'ts' field.
-
-Parameters which can be used:
- - min/maxTime
- - min/maxX/Y
- - flipVertical/Horizontal
- - transpose
-'''
-
-import numpy as np
-import matplotlib.pyplot as plt
-from math import log10, floor
-
-def roundToSf(x, sig=3):
-    try:
-        return round(x, sig-int(floor(log10(abs(x))))-1)
-    except ValueError: # log of zero
-        return 0
-
-''' 
-Descend a container hierarchically, looking for 'ts' fields to work on
-'''
-
-def plotEventRate(inDicts, **kwargs):
-    if isinstance(inDicts, list):
-        for inDict in inDicts:
-            plotEventRate(inDict, **kwargs)
-        return
-    else:
-        inDict = inDicts
-    if not isinstance(inDict, dict):
-        return
-    if 'ts' not in inDict:
-        title = kwargs.pop('title', '')
-        if 'info' in inDict and isinstance(inDict, dict):
-            fileName = inDict['info'].get('filePathOrName')
-            if fileName is not None:
-                print('plotEventRate was called for file ' + fileName)
-                title = (title + ' ' + fileName).lstrip()
-        for key in inDict.keys():
-            kwargs['title'] = (title + ' ' + key).lstrip()
-            plotEventRate(inDict[key], **kwargs)
-    else: # It's a data-type container
-        # Break out data array for cleaner code
-        ts = inDict['ts']
-        if ts.shape[0] == 0: 
-            return
-        if ts.shape[0] == 1:
-            title = kwargs.get('title', 'this container')
-            print('Only one event in ' + title)
-            return
-        startTime = kwargs.get('startTime', kwargs.get('minTime', kwargs.get('firstTime', np.min(ts))))
-        endTime = kwargs.get('endTime', kwargs.get('maxTime', kwargs.get('lastTime', np.max(ts))))
-        freqs = kwargs.get('freqs')
-        if freqs is None:
-            periods = kwargs.get('periods', [0.001, 0.01, 0.1, 1])
-        else:
-            periods = [1/f for f in freqs]        
-        axes = kwargs.get('axes') 
-        if axes is None:
-            fig, axes = plt.subplots()
-            kwargs['axes'] = axes
-        legend = kwargs.get('legend', [])
-        for period in periods:
-            endTimes = [t + period for t in np.arange(startTime, endTime, period)]
-            midTimes = [t - period / 2 for t in endTimes]
-            endIds = [np.searchsorted(ts, t) for t in endTimes]
-            counts = [end-start for start, end in zip(endIds[:-1], endIds[1:])]
-            counts.insert(0, endIds[0])
-            rates = [count/period for count in counts]
-            if kwargs.get('perPixel', False):
-                minX = inDict.get('minX', kwargs.get('minX', min(inDict['x']))) 
-                maxX = inDict.get('maxX', kwargs.get('maxX', max(inDict['x']))) 
-                minY = inDict.get('minY', kwargs.get('minY', min(inDict['y']))) 
-                maxY = inDict.get('maxY', kwargs.get('maxY', max(inDict['y']))) 
-                numPixels = (maxX - minX + 1) * (maxY - minY + 1)
-                rates = rates / numPixels
-            endTimes = np.arange(startTime, endTime, period)
-            axes.plot(midTimes, rates)
-            plt.xlabel('Time (s)')
-            plt.ylabel('Rate (events/s)')
-            legend.append('period: ' + str(period) + ' s')
-        axes.legend(legend)
-        kwargs['legend'] = legend
-        if kwargs.get('title') is not None:
-            axes.set_title(kwargs.get('title'))            
-        callback = kwargs.get('callback')
-        if callback is not None:
-            kwargs = callback(**kwargs)            
-
-
-                
+# -*- coding: utf-8 -*-
+'''
+Copyright (C) 2019 Event-driven Perception for Robotics
+Authors: Sim Bamford
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
+plotEventRate takes 'inDict' - a dict containing an imported ae file, 
+as created by importAe, and creates a series of plots of event rates.
+It creates one plot for each dataType dct contianing a 'ts' field.
+
+Parameters which can be used:
+ - min/maxTime
+ - min/maxX/Y
+ - flipVertical/Horizontal
+ - transpose
+'''
+
+import numpy as np
+import matplotlib.pyplot as plt
+from math import log10, floor
+
+def roundToSf(x, sig=3):
+    try:
+        return round(x, sig-int(floor(log10(abs(x))))-1)
+    except ValueError: # log of zero
+        return 0
+
+''' 
+Descend a container hierarchically, looking for 'ts' fields to work on
+'''
+
+def plotEventRate(inDicts, **kwargs):
+    if isinstance(inDicts, list):
+        for inDict in inDicts:
+            plotEventRate(inDict, **kwargs)
+        return
+    else:
+        inDict = inDicts
+    if not isinstance(inDict, dict):
+        return
+    if 'ts' not in inDict:
+        title = kwargs.pop('title', '')
+        if 'info' in inDict and isinstance(inDict, dict):
+            fileName = inDict['info'].get('filePathOrName')
+            if fileName is not None:
+                print('plotEventRate was called for file ' + fileName)
+                title = (title + ' ' + fileName).lstrip()
+        for key in inDict.keys():
+            kwargs['title'] = (title + ' ' + key).lstrip()
+            plotEventRate(inDict[key], **kwargs)
+    else: # It's a data-type container
+        # Break out data array for cleaner code
+        ts = inDict['ts']
+        if ts.shape[0] == 0: 
+            return
+        if ts.shape[0] == 1:
+            title = kwargs.get('title', 'this container')
+            print('Only one event in ' + title)
+            return
+        startTime = kwargs.get('startTime', kwargs.get('minTime', kwargs.get('firstTime', np.min(ts))))
+        endTime = kwargs.get('endTime', kwargs.get('maxTime', kwargs.get('lastTime', np.max(ts))))
+        freqs = kwargs.get('freqs')
+        if freqs is None:
+            periods = kwargs.get('periods', [0.001, 0.01, 0.1, 1])
+        else:
+            periods = [1/f for f in freqs]        
+        axes = kwargs.get('axes') 
+        if axes is None:
+            fig, axes = plt.subplots()
+            kwargs['axes'] = axes
+        legend = kwargs.get('legend', [])
+        for period in periods:
+            endTimes = [t + period for t in np.arange(startTime, endTime, period)]
+            midTimes = [t - period / 2 for t in endTimes]
+            endIds = [np.searchsorted(ts, t) for t in endTimes]
+            counts = [end-start for start, end in zip(endIds[:-1], endIds[1:])]
+            counts.insert(0, endIds[0])
+            rates = [count/period for count in counts]
+            if kwargs.get('perPixel', False):
+                minX = inDict.get('minX', kwargs.get('minX', min(inDict['x']))) 
+                maxX = inDict.get('maxX', kwargs.get('maxX', max(inDict['x']))) 
+                minY = inDict.get('minY', kwargs.get('minY', min(inDict['y']))) 
+                maxY = inDict.get('maxY', kwargs.get('maxY', max(inDict['y']))) 
+                numPixels = (maxX - minX + 1) * (maxY - minY + 1)
+                rates = rates / numPixels
+            endTimes = np.arange(startTime, endTime, period)
+            axes.plot(midTimes, rates)
+            plt.xlabel('Time (s)')
+            plt.ylabel('Rate (events/s)')
+            legend.append('period: ' + str(period) + ' s')
+        axes.legend(legend)
+        kwargs['legend'] = legend
+        if kwargs.get('title') is not None:
+            axes.set_title(kwargs.get('title'))            
+        callback = kwargs.get('callback')
+        if callback is not None:
+            kwargs = callback(**kwargs)            
+
+
+
```

### Comparing `bimvee-1.0.9/bimvee/plotFlow.py` & `bimvee-1.0.9.dev0/bimvee/plotFlow.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Copyright (C) 2020 Event-driven Perception for Robotics
-Authors: Sim Bamford
-         Aiko Dinale
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
-plotImu takes 'inDict' - a dictionary containing imported IMU data 
-(or a higher level container, in which attempts to descend and call itself) 
-as created by importAe, and plots against time the various dimensions of the 
-IMU samples contained. 
-"""
-import os
-import matplotlib.pyplot as plt
-import seaborn as sns
-
-sns.set(palette="colorblind")
-
-# Color Palette for Color Blindness
-zesty_palette     = ['#F5793A', '#A95AA1', '#85C0F9', '#0F2080']
-retro_palette     = ['#601A4A', '#EE442F', '#63ACBE', '#F9F4EC']
-corporate_palette = ['#8DB8AD', '#EBE7E0', '#C6D4E1', '#44749D']
-
-#-----------------------------------------------------------------------------------------------------
-def plotFlow(flowDict, fig_path=None, fig_name=None, fig_subtitle=None):
-    """
-    Plot the FLOW events in flowDict against the time. If specified, save the
-    generated figure as fig_name.png at the location defined by fig_path.
-
-    Arguments:
-        flowDict {dict} -- dictionary of FLOW events as formatted by bimvee from event-driven library
-
-    Keyword Arguments:
-        fig_path {string} -- save path for the generated figure (default: {None})
-        fig_name {string} -- name of the generated figure (default: {None})
-        fig_subtitle {string} -- figure sub-title (default: {None})
-    """
-    fig = plt.figure(figsize=(16.0, 10.0))
-    if isinstance(fig_subtitle, str):
-        fig.suptitle("FLOW Events\n" + fig_subtitle, fontsize=20, fontweight='bold')
-    else:
-        fig.suptitle("FLOW Events", fontsize=20, fontweight='bold')
-
-
-    ax11 = plt.subplot(2, 1, 1)
-    plt.plot(flowDict['ts'], flowDict['vx'], color=retro_palette[0], marker='.', linewidth=0.0)
-    plt.xlabel('Time [s]', fontsize=10, fontweight='bold')
-    plt.ylabel('Vx [px/s]', fontsize=10, fontweight='bold')
-    plt.grid(True)
-
-    plt.subplot(2, 1, 2, sharex=ax11)
-    plt.plot(flowDict['ts'], flowDict['vy'], color=retro_palette[1], marker='.', linewidth=0.0)
-    plt.xlabel('Time [s]', fontsize=10, fontweight='bold')
-    plt.ylabel('Vy [px/s]', fontsize=10, fontweight='bold')
-    plt.grid(True)
-
-    fig.tight_layout()
-    if isinstance(fig_subtitle, str):
-        fig.subplots_adjust(top=0.9)
-    else:
-        fig.subplots_adjust(top=0.95)
-
-    fig.align_ylabels()
-
-    if isinstance(fig_path, str) and isinstance(fig_name, str):
-        plt.savefig(os.path.join(fig_path, fig_name + ".png"), dpi=300, bbox_inches='tight')
-        print("Saving " + fig_name + ".png")
-        plt.close()
-    else:
-        plt.show()
-
-#-----------------------------------------------------------------------------------------------------
-def plotFlowDistribution(flowDict, fig_path=None, fig_name=None, fig_subtitle=None):
-    """
-    Plot the distribution of the FLOW events in flowDict and save the generated
-    figure as fig_name.png at the location defined by fig_path.
-
-    Arguments:
-        flowDict {dict} -- dictionary of FLOW events as formatted by bimvee from event-driven library
-
-    Keyword Arguments:
-        fig_path {string} -- save path for the generated figure (default: {None})
-        fig_name {string} -- name of the generated figure (default: {None})
-        fig_subtitle {string} -- figure sub-title (default: {None})
-    """
-    fig = plt.figure(figsize=(14.0, 10.0))
-    if isinstance(fig_subtitle, str):
-        fig.suptitle("FLOW Events Distribution\n" + fig_subtitle, fontsize=20, fontweight='bold')
-    else:
-        fig.suptitle("FLOW Events Distribution", fontsize=20, fontweight='bold')
-    
-    plt.subplot(2,1,1)
-    sns.distplot(flowDict['vx'], bins=100, color = retro_palette[0])
-    plt.xlabel('Vx [px/s]', fontsize=10, fontweight='bold')
-
-    plt.subplot(2,1,2)
-    sns.distplot(flowDict['vy'], bins=100, color = retro_palette[1])
-    plt.xlabel('Vy [px/s]', fontsize=10, fontweight='bold')
-
-    fig.tight_layout()
-    if isinstance(fig_subtitle, str):
-        fig.subplots_adjust(top=0.9)
-    else:
-        fig.subplots_adjust(top=0.95)
-
-    if isinstance(fig_path, str) and isinstance(fig_name, str):
-        plt.savefig(os.path.join(fig_path, fig_name + '.png'), dpi=300, bbox_inches='tight')
-        print("Saving " + fig_name + ".png")
-        plt.close()
-    else:
-        plt.show()
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Copyright (C) 2020 Event-driven Perception for Robotics
+Authors: Sim Bamford
+         Aiko Dinale
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
+plotImu takes 'inDict' - a dictionary containing imported IMU data 
+(or a higher level container, in which attempts to descend and call itself) 
+as created by importAe, and plots against time the various dimensions of the 
+IMU samples contained. 
+"""
+import os
+import matplotlib.pyplot as plt
+import seaborn as sns
+
+sns.set(palette="colorblind")
+
+# Color Palette for Color Blindness
+zesty_palette     = ['#F5793A', '#A95AA1', '#85C0F9', '#0F2080']
+retro_palette     = ['#601A4A', '#EE442F', '#63ACBE', '#F9F4EC']
+corporate_palette = ['#8DB8AD', '#EBE7E0', '#C6D4E1', '#44749D']
+
+#-----------------------------------------------------------------------------------------------------
+def plotFlow(flowDict, fig_path=None, fig_name=None, fig_subtitle=None):
+    """
+    Plot the FLOW events in flowDict against the time. If specified, save the
+    generated figure as fig_name.png at the location defined by fig_path.
+
+    Arguments:
+        flowDict {dict} -- dictionary of FLOW events as formatted by bimvee from event-driven library
+
+    Keyword Arguments:
+        fig_path {string} -- save path for the generated figure (default: {None})
+        fig_name {string} -- name of the generated figure (default: {None})
+        fig_subtitle {string} -- figure sub-title (default: {None})
+    """
+    fig = plt.figure(figsize=(16.0, 10.0))
+    if isinstance(fig_subtitle, str):
+        fig.suptitle("FLOW Events\n" + fig_subtitle, fontsize=20, fontweight='bold')
+    else:
+        fig.suptitle("FLOW Events", fontsize=20, fontweight='bold')
+
+
+    ax11 = plt.subplot(2, 1, 1)
+    plt.plot(flowDict['ts'], flowDict['vx'], color=retro_palette[0], marker='.', linewidth=0.0)
+    plt.xlabel('Time [s]', fontsize=10, fontweight='bold')
+    plt.ylabel('Vx [px/s]', fontsize=10, fontweight='bold')
+    plt.grid(True)
+
+    plt.subplot(2, 1, 2, sharex=ax11)
+    plt.plot(flowDict['ts'], flowDict['vy'], color=retro_palette[1], marker='.', linewidth=0.0)
+    plt.xlabel('Time [s]', fontsize=10, fontweight='bold')
+    plt.ylabel('Vy [px/s]', fontsize=10, fontweight='bold')
+    plt.grid(True)
+
+    fig.tight_layout()
+    if isinstance(fig_subtitle, str):
+        fig.subplots_adjust(top=0.9)
+    else:
+        fig.subplots_adjust(top=0.95)
+
+    fig.align_ylabels()
+
+    if isinstance(fig_path, str) and isinstance(fig_name, str):
+        plt.savefig(os.path.join(fig_path, fig_name + ".png"), dpi=300, bbox_inches='tight')
+        print("Saving " + fig_name + ".png")
+        plt.close()
+    else:
+        plt.show()
+
+#-----------------------------------------------------------------------------------------------------
+def plotFlowDistribution(flowDict, fig_path=None, fig_name=None, fig_subtitle=None):
+    """
+    Plot the distribution of the FLOW events in flowDict and save the generated
+    figure as fig_name.png at the location defined by fig_path.
+
+    Arguments:
+        flowDict {dict} -- dictionary of FLOW events as formatted by bimvee from event-driven library
+
+    Keyword Arguments:
+        fig_path {string} -- save path for the generated figure (default: {None})
+        fig_name {string} -- name of the generated figure (default: {None})
+        fig_subtitle {string} -- figure sub-title (default: {None})
+    """
+    fig = plt.figure(figsize=(14.0, 10.0))
+    if isinstance(fig_subtitle, str):
+        fig.suptitle("FLOW Events Distribution\n" + fig_subtitle, fontsize=20, fontweight='bold')
+    else:
+        fig.suptitle("FLOW Events Distribution", fontsize=20, fontweight='bold')
+    
+    plt.subplot(2,1,1)
+    sns.distplot(flowDict['vx'], bins=100, color = retro_palette[0])
+    plt.xlabel('Vx [px/s]', fontsize=10, fontweight='bold')
+
+    plt.subplot(2,1,2)
+    sns.distplot(flowDict['vy'], bins=100, color = retro_palette[1])
+    plt.xlabel('Vy [px/s]', fontsize=10, fontweight='bold')
+
+    fig.tight_layout()
+    if isinstance(fig_subtitle, str):
+        fig.subplots_adjust(top=0.9)
+    else:
+        fig.subplots_adjust(top=0.95)
+
+    if isinstance(fig_path, str) and isinstance(fig_name, str):
+        plt.savefig(os.path.join(fig_path, fig_name + '.png'), dpi=300, bbox_inches='tight')
+        print("Saving " + fig_name + ".png")
+        plt.close()
+    else:
+        plt.show()
```

### Comparing `bimvee-1.0.9/bimvee/plotFrame.py` & `bimvee-1.0.9.dev0/bimvee/plotFrame.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-# -*- coding: utf-8 -*-
-
-'''
-Copyright (C) 2019 Event-driven Perception for Robotics
-Authors: Sim Bamford
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
-plotFrame takes 'inDict' - a dictionary containing imported frame data 
-(or a higher level container, in which attempts to descend and call itself) 
-as created by importAe, and creates a series of images from selected
-frames.
-The number of subplots is given by the numPlots parameter.
-'distributeBy' can either be 'time' or 'events', to decide how the points 
-around which data is rendered are chosen. 
-The frame events are then chosen as those nearest to the time points.
-If the 'distributeBy' is 'time' then if the further parameters 'minTime' 
-and 'maxTime' are used then the time window used is only between
-those limits.
-Params include:
-numPlots, distributeBy, minTime, maxTime, flipVertical, flipHorizontal, transpose
-'''
-
-import numpy as np
-import matplotlib.pyplot as plt
-from math import log10, floor
-
-def roundToSf(x, sig=3):
-    try:
-        return round(x, sig-int(floor(log10(abs(x))))-1)
-    except ValueError: # log of zero
-        return 0
-
-def plotFrame(inDicts, **kwargs):
-    if isinstance(inDicts, list):
-        for inDict in inDicts:
-            plotFrame(inDict, **kwargs)
-        return
-    else:
-        inDict = inDicts
-    if not isinstance(inDict, dict):
-        return
-    if 'ts' not in inDict:
-        title = kwargs.pop('title', '')
-        if 'info' in inDict and isinstance(inDict, dict):
-            fileName = inDict['info'].get('filePathOrName')
-            if fileName is not None:
-                print('plotFrame was called for file ' + fileName)
-                title = (title + ' ' + fileName).lstrip()
-        for key in inDict.keys():
-            kwargs['title'] = (title + ' ' + key).lstrip()
-            plotFrame(inDict[key], **kwargs)
-        return
-    # From this point onwards, it's a data-type container
-    if 'frames' not in inDict:
-        return
-    # From this point onwards, it's a frame data-type container
-    distributeBy = kwargs.get('distributeBy', 'time').lower()
-    numPlots = kwargs.get('numPlots', 6)
-    
-    ts = inDict['ts']
-    frames = inDict['frames']
-    numFrames = len(ts)
-    if numFrames < numPlots:
-        numPlots = numFrames
-
-    if numFrames == numPlots:
-        distributeBy = 'events'
-    
-    # Distribute plots in a raster with a 3:4 ratio
-    numPlotsX = int(np.round(np.sqrt(numPlots / 3 * 4)))
-    numPlotsY = int(np.ceil(numPlots / numPlotsX))
-    
-    minTime = kwargs.get('startTime', kwargs.get('minTime', kwargs.get('beginTime', ts[0])))
-    maxTime = kwargs.get('stopTime', kwargs.get('maxTime', kwargs.get('endTime', ts[-1])))
-
-    if distributeBy == 'time':
-        totalTime = maxTime - minTime
-        timeStep = totalTime / numPlots
-        timePoints = np.arange(minTime + timeStep * 0.5, maxTime, timeStep)
-    else: # distribute by event number
-        framesPerStep = numFrames / numPlots
-        timePoints = ts(int(np.ceil(np.arange(framesPerStep * 0.5, numFrames, framesPerStep))))
-
-    fig, axes = plt.subplots(numPlotsY, numPlotsX)
-    fig.suptitle(kwargs.get('title', ''))
-    
-    axes = axes.flatten().tolist()
-    for ax, timePoint in zip(axes, timePoints):
-
-        # Find eventIndex nearest to timePoint
-        frameIdx = np.searchsorted(ts, timePoint)
-        frame = frames[frameIdx]
-        if kwargs.get('transpose', False):
-            frame = np.transpose(frame)
-        if kwargs.get('flipVertical', False):
-            frame = np.flip(frame, axis=0)
-        if kwargs.get('flipHorizontal', False):
-            frame = np.flip(frame, axis=1)
-        ax.imshow(frame, cmap='gray')
-        ax.grid(b=False)
-        ax.set_title('Time: ' + str(roundToSf(timePoint)) + ' s; frame number: ' + str(frameIdx))
-
-#%%
-'''
-    Optional extra - not including it by default because I don't want this 
-    extra dependency, but this is a quick way to see frame data as a video
-'''
-
-'''       
-from imageio import mimwrite
-def framesToGif(framesDict, **kwargs):
-    ts = framesDict['ts']
-    frames = framesDict['frames']
-    outputFilePathAndName = kwargs.get('outputFilePathAndName', 'framesAsMovie.mp4')
-    frameRate = len(ts) / (ts[-1] - ts[0])
-    framesExpanded = [np.expand_dims(f, 0) for f in frames]
-    framesAllArray = np.concatenate(framesExpanded, 0)
-    mimwrite(outputFilePathAndName, framesAllArray , fps = int(frameRate))
-'''
-
+# -*- coding: utf-8 -*-
+
+'''
+Copyright (C) 2019 Event-driven Perception for Robotics
+Authors: Sim Bamford
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
+plotFrame takes 'inDict' - a dictionary containing imported frame data 
+(or a higher level container, in which attempts to descend and call itself) 
+as created by importAe, and creates a series of images from selected
+frames.
+The number of subplots is given by the numPlots parameter.
+'distributeBy' can either be 'time' or 'events', to decide how the points 
+around which data is rendered are chosen. 
+The frame events are then chosen as those nearest to the time points.
+If the 'distributeBy' is 'time' then if the further parameters 'minTime' 
+and 'maxTime' are used then the time window used is only between
+those limits.
+Params include:
+numPlots, distributeBy, minTime, maxTime, flipVertical, flipHorizontal, transpose
+'''
+
+import numpy as np
+import matplotlib.pyplot as plt
+from math import log10, floor
+
+def roundToSf(x, sig=3):
+    try:
+        return round(x, sig-int(floor(log10(abs(x))))-1)
+    except ValueError: # log of zero
+        return 0
+
+def plotFrame(inDicts, **kwargs):
+    if isinstance(inDicts, list):
+        for inDict in inDicts:
+            plotFrame(inDict, **kwargs)
+        return
+    else:
+        inDict = inDicts
+    if not isinstance(inDict, dict):
+        return
+    if 'ts' not in inDict:
+        title = kwargs.pop('title', '')
+        if 'info' in inDict and isinstance(inDict, dict):
+            fileName = inDict['info'].get('filePathOrName')
+            if fileName is not None:
+                print('plotFrame was called for file ' + fileName)
+                title = (title + ' ' + fileName).lstrip()
+        for key in inDict.keys():
+            kwargs['title'] = (title + ' ' + key).lstrip()
+            plotFrame(inDict[key], **kwargs)
+        return
+    # From this point onwards, it's a data-type container
+    if 'frames' not in inDict:
+        return
+    # From this point onwards, it's a frame data-type container
+    distributeBy = kwargs.get('distributeBy', 'time').lower()
+    numPlots = kwargs.get('numPlots', 6)
+    
+    ts = inDict['ts']
+    frames = inDict['frames']
+    numFrames = len(ts)
+    if numFrames < numPlots:
+        numPlots = numFrames
+
+    if numFrames == numPlots:
+        distributeBy = 'events'
+    
+    # Distribute plots in a raster with a 3:4 ratio
+    numPlotsX = int(np.round(np.sqrt(numPlots / 3 * 4)))
+    numPlotsY = int(np.ceil(numPlots / numPlotsX))
+    
+    minTime = kwargs.get('startTime', kwargs.get('minTime', kwargs.get('beginTime', ts[0])))
+    maxTime = kwargs.get('stopTime', kwargs.get('maxTime', kwargs.get('endTime', ts[-1])))
+
+    if distributeBy == 'time':
+        totalTime = maxTime - minTime
+        timeStep = totalTime / numPlots
+        timePoints = np.arange(minTime + timeStep * 0.5, maxTime, timeStep)
+    else: # distribute by event number
+        framesPerStep = numFrames / numPlots
+        timePoints = ts(int(np.ceil(np.arange(framesPerStep * 0.5, numFrames, framesPerStep))))
+
+    fig, axes = plt.subplots(numPlotsY, numPlotsX)
+    fig.suptitle(kwargs.get('title', ''))
+    
+    axes = axes.flatten().tolist()
+    for ax, timePoint in zip(axes, timePoints):
+
+        # Find eventIndex nearest to timePoint
+        frameIdx = np.searchsorted(ts, timePoint)
+        frame = frames[frameIdx]
+        if kwargs.get('transpose', False):
+            frame = np.transpose(frame)
+        if kwargs.get('flipVertical', False):
+            frame = np.flip(frame, axis=0)
+        if kwargs.get('flipHorizontal', False):
+            frame = np.flip(frame, axis=1)
+        ax.imshow(frame, cmap='gray')
+        ax.grid(b=False)
+        ax.set_title('Time: ' + str(roundToSf(timePoint)) + ' s; frame number: ' + str(frameIdx))
+
+#%%
+'''
+    Optional extra - not including it by default because I don't want this 
+    extra dependency, but this is a quick way to see frame data as a video
+'''
+
+'''       
+from imageio import mimwrite
+def framesToGif(framesDict, **kwargs):
+    ts = framesDict['ts']
+    frames = framesDict['frames']
+    outputFilePathAndName = kwargs.get('outputFilePathAndName', 'framesAsMovie.mp4')
+    frameRate = len(ts) / (ts[-1] - ts[0])
+    framesExpanded = [np.expand_dims(f, 0) for f in frames]
+    framesAllArray = np.concatenate(framesExpanded, 0)
+    mimwrite(outputFilePathAndName, framesAllArray , fps = int(frameRate))
+'''
+
```

### Comparing `bimvee-1.0.9/bimvee/plotImu.py` & `bimvee-1.0.9.dev0/bimvee/plotImu.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,158 +1,160 @@
-# -*- coding: utf-8 -*-
-"""
-Copyright (C) 2019 Event-driven Perception for Robotics
-Authors: Sim Bamford
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
-plotImu takes 'inDict' - a dictionary containing imported IMU data 
-(or a higher level container, in which attempts to descend and call itself) 
-as created by importAe, and plots against time the various dimensions of the 
-IMU samples contained. 
-"""
-import os, sys
-import matplotlib.pyplot as plt
-import seaborn as sns
-
-sns.set(palette="colorblind")
-
-# Color Palette for Color Blindness
-zesty_palette     = ['#F5793A', '#A95AA1', '#85C0F9', '#0F2080']
-retro_palette     = ['#601A4A', '#EE442F', '#63ACBE', '#F9F4EC']
-corporate_palette = ['#8DB8AD', '#EBE7E0', '#C6D4E1', '#44749D']
-
-#-----------------------------------------------------------------------------------------------------
-def plotImu(inDict, **kwargs):
-    if isinstance(inDict, list):
-        for inDictInst in inDict:
-            plotImu(inDictInst, **kwargs)
-        return
-    if 'info' in inDict:
-        fileName = inDict['info'].get('filePathOrName', '')
-        print('plotImu was called for file ' + fileName)
-        if not inDict['data']:
-            print('The import contains no data.')
-            return
-        for channelName in inDict['data']:
-            channelData = inDict['data'][channelName]
-            if 'imu' in channelData and len(channelData['imu']['ts']) > 0:
-                kwargs['title'] = ' '.join([fileName, str(channelName)])
-                plotImu(channelData['imu'], **kwargs)
-            else:
-                print('Channel ' + channelName + ' skipped because it contains no polarity data')
-        return
-    if 'temp' in inDict: 
-        numSubplots = 4
-    else:
-        numSubplots = 3
-    fig, allAxes = plt.subplots(numSubplots, 1)
-    fig.suptitle(kwargs.get('title', ''))
-    axesAcc = allAxes[0]
-    axesAcc.plot(inDict['ts'], inDict['acc'][:, 0], 'r')
-    axesAcc.plot(inDict['ts'], inDict['acc'][:, 1], 'g')
-    axesAcc.plot(inDict['ts'], inDict['acc'][:, 2], 'b')
-    axesAcc.set_title('Acceleration (m/s)')
-    axesAcc.legend(['x', 'y', 'z'])
-
-    axesAngV = allAxes[1]
-    axesAngV.plot(inDict['ts'], inDict['angV'][:, 0], 'r')
-    axesAngV.plot(inDict['ts'], inDict['angV'][:, 1], 'g')
-    axesAngV.plot(inDict['ts'], inDict['angV'][:, 2], 'b')
-    axesAngV.set_title('Angular velocity (rad/s)')
-    axesAngV.legend(['x', 'y', 'z'])
-
-    axesMag = allAxes[2]
-    axesMag.plot(inDict['ts'], inDict['mag'])
-    axesMag.set_title('Mag (uT)')
-    axesMag.legend(['x', 'y', 'z'])
-
-    if 'temp' in inDict: 
-        axesTemp = allAxes[3]
-        axesTemp.plot(inDict['ts'], inDict['temp'])
-        axesTemp.set_title('Temp (K)')
-
-
-#-----------------------------------------------------------------------------------------------------
-def plotImuDistribution(imuDict, unitIMU='FPGA', fig_path=None, fig_name=None, fig_subtitle=None):
-    """
-    Plot the distribution of the IMU data in imuDict. If specified, save the
-    generated figure as fig_name.png at the location defined by fig_path.
-
-    Arguments:
-        imuDict {dict} -- dictionary of IMU data (as formatted by bimvee)
-
-    Keyword Arguments:
-        unitIMU {str} -- either 'FPGA' or 'SI' (default: {'FPGA'})
-        fig_path {string} -- save path for the generated figure (default: {None})
-        fig_name {string} -- name of the generated figure (default: {None})
-        fig_subtitle {string} -- figure sub-title (default: {None})
-    """
-    fig = plt.figure(figsize=(14.0, 10.0))
-    if isinstance(fig_subtitle, str):
-        fig.suptitle("IMU Samples Distribution\n" + fig_subtitle, fontsize=20, fontweight='bold')
-    else:
-        fig.suptitle("IMU Samples Distribution", fontsize=20, fontweight='bold')
-
-    plt.subplot(3,2,1)
-    sns.distplot([v for v, s in zip(imuDict['value'], imuDict['sensor']) if s == 0], bins=100, color=zesty_palette[0])
-    plt.title("Accelerometer", fontsize=16, fontweight='bold')
-    if unitIMU == 'FPGA':
-        plt.xlabel('accX [fpga]', fontsize=10, fontweight='bold')
-    elif unitIMU == 'SI':
-        plt.xlabel('accX [m/s]', fontsize=10, fontweight='bold')
-
-    plt.subplot(3,2,2)
-    sns.distplot([v for v, s in zip(imuDict['value'], imuDict['sensor']) if s == 3], bins=100, color=zesty_palette[0])
-    plt.title("Gyroscope", fontsize=16, fontweight='bold')
-    if unitIMU == 'FPGA':
-        plt.xlabel('gyroX [fpga]', fontsize=10, fontweight='bold')
-    elif unitIMU == 'SI':
-        plt.xlabel('gyroX [rad/s]', fontsize=10, fontweight='bold')
-
-    plt.subplot(3,2,3)
-    sns.distplot([v for v, s in zip(imuDict['value'], imuDict['sensor']) if s == 1], bins=100, color=zesty_palette[1])
-    if unitIMU == 'FPGA':
-        plt.xlabel('accY [fpga]', fontsize=10, fontweight='bold')
-    elif unitIMU == 'SI':
-        plt.xlabel('accY [m/s]', fontsize=10, fontweight='bold')
-
-    plt.subplot(3,2,4)
-    sns.distplot([v for v, s in zip(imuDict['value'], imuDict['sensor']) if s == 4], bins=100, color=zesty_palette[1])
-    if unitIMU == 'FPGA':
-        plt.xlabel('gyroY [fpga]', fontsize=10, fontweight='bold')
-    elif unitIMU == 'SI':
-        plt.xlabel('gyroY [rad/s]', fontsize=10, fontweight='bold')
-
-    plt.subplot(3,2,5)
-    sns.distplot([v for v, s in zip(imuDict['value'], imuDict['sensor']) if s == 2], bins=100, color=zesty_palette[3])
-    if unitIMU == 'FPGA':
-        plt.xlabel('accZ [fpga]', fontsize=10, fontweight='bold')
-    elif unitIMU == 'SI':
-        plt.xlabel('accZ [m/s]', fontsize=10, fontweight='bold')
-
-    plt.subplot(3,2,6)
-    sns.distplot([v for v, s in zip(imuDict['value'], imuDict['sensor']) if s == 5], bins=100, color=zesty_palette[3])
-    if unitIMU == 'FPGA':
-        plt.xlabel('gyroZ [fpga]', fontsize=10, fontweight='bold')
-    elif unitIMU == 'SI':
-        plt.xlabel('gyroZ [rad/s]', fontsize=10, fontweight='bold')
-
-    fig.tight_layout()
-    if isinstance(fig_subtitle, str):
-        fig.subplots_adjust(top=0.85)
-    else:
-        fig.subplots_adjust(top=0.9)
-
-    if isinstance(fig_path, str) and isinstance(fig_name, str): 
-        plt.savefig(os.path.join(fig_path, fig_name + '.png'), dpi=300, bbox_inches='tight')
-        print("Saving " + fig_name + ".png")
-        plt.close()
-    else:
-        plt.show()
+# -*- coding: utf-8 -*-
+"""
+Copyright (C) 2019 Event-driven Perception for Robotics
+Authors: Sim Bamford
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
+plotImu takes 'inDict' - a dictionary containing imported IMU data 
+(or a higher level container, in which attempts to descend and call itself) 
+as created by importAe, and plots against time the various dimensions of the 
+IMU samples contained. 
+"""
+import os, sys
+import matplotlib.pyplot as plt
+import seaborn as sns
+
+sns.set(palette="colorblind")
+
+# Color Palette for Color Blindness
+zesty_palette     = ['#F5793A', '#A95AA1', '#85C0F9', '#0F2080']
+retro_palette     = ['#601A4A', '#EE442F', '#63ACBE', '#F9F4EC']
+corporate_palette = ['#8DB8AD', '#EBE7E0', '#C6D4E1', '#44749D']
+
+#-----------------------------------------------------------------------------------------------------
+def plotImu(inDict, **kwargs):
+    if isinstance(inDict, list):
+        for inDictInst in inDict:
+            plotImu(inDictInst, **kwargs)
+        return
+    if 'info' in inDict:
+        fileName = inDict['info'].get('filePathOrName', '')
+        print('plotImu was called for file ' + fileName)
+        if not inDict['data']:
+            print('The import contains no data.')
+            return
+        for channelName in inDict['data']:
+            channelData = inDict['data'][channelName]
+            if 'imu' in channelData and len(channelData['imu']['ts']) > 0:
+                kwargs['title'] = ' '.join([fileName, str(channelName)])
+                plotImu(channelData['imu'], **kwargs)
+            else:
+                print('Channel ' + channelName + ' skipped because it contains no polarity data')
+        return
+    if 'temp' in inDict: 
+        numSubplots = 4
+    else:
+        numSubplots = 3
+    fig, allAxes = plt.subplots(numSubplots, 1)
+    fig.suptitle(kwargs.get('title', ''))
+    axesAcc = allAxes[0]
+    axesAcc.plot(inDict['ts'], inDict['acc'][:, 0], 'r')
+    axesAcc.plot(inDict['ts'], inDict['acc'][:, 1], 'g')
+    axesAcc.plot(inDict['ts'], inDict['acc'][:, 2], 'b')
+    axesAcc.set_title('Acceleration (m/s)')
+    axesAcc.legend(['x', 'y', 'z'])
+
+    axesAngV = allAxes[1]
+    axesAngV.plot(inDict['ts'], inDict['angV'][:, 0], 'r')
+    axesAngV.plot(inDict['ts'], inDict['angV'][:, 1], 'g')
+    axesAngV.plot(inDict['ts'], inDict['angV'][:, 2], 'b')
+    axesAngV.set_title('Angular velocity (rad/s)')
+    axesAngV.legend(['x', 'y', 'z'])
+
+    axesMag = allAxes[2]
+    axesMag.plot(inDict['ts'], inDict['mag'][:, 0], 'r')
+    axesMag.plot(inDict['ts'], inDict['mag'][:, 1], 'g')
+    axesMag.plot(inDict['ts'], inDict['mag'][:, 2], 'b')
+    axesMag.set_title('Mag (uT)')
+    axesMag.legend(['x', 'y', 'z'])
+
+    if 'temp' in inDict: 
+        axesTemp = allAxes[3]
+        axesTemp.plot(inDict['ts'], inDict['temp'])
+        axesTemp.set_title('Temp (K)')
+
+
+#-----------------------------------------------------------------------------------------------------
+def plotImuDistribution(imuDict, unitIMU='FPGA', fig_path=None, fig_name=None, fig_subtitle=None):
+    """
+    Plot the distribution of the IMU data in imuDict. If specified, save the
+    generated figure as fig_name.png at the location defined by fig_path.
+
+    Arguments:
+        imuDict {dict} -- dictionary of IMU data (as formatted by bimvee)
+
+    Keyword Arguments:
+        unitIMU {str} -- either 'FPGA' or 'SI' (default: {'FPGA'})
+        fig_path {string} -- save path for the generated figure (default: {None})
+        fig_name {string} -- name of the generated figure (default: {None})
+        fig_subtitle {string} -- figure sub-title (default: {None})
+    """
+    fig = plt.figure(figsize=(14.0, 10.0))
+    if isinstance(fig_subtitle, str):
+        fig.suptitle("IMU Samples Distribution\n" + fig_subtitle, fontsize=20, fontweight='bold')
+    else:
+        fig.suptitle("IMU Samples Distribution", fontsize=20, fontweight='bold')
+
+    plt.subplot(3,2,1)
+    sns.distplot([v for v, s in zip(imuDict['value'], imuDict['sensor']) if s == 0], bins=100, color=zesty_palette[0])
+    plt.title("Accelerometer", fontsize=16, fontweight='bold')
+    if unitIMU == 'FPGA':
+        plt.xlabel('accX [fpga]', fontsize=10, fontweight='bold')
+    elif unitIMU == 'SI':
+        plt.xlabel('accX [m/s]', fontsize=10, fontweight='bold')
+
+    plt.subplot(3,2,2)
+    sns.distplot([v for v, s in zip(imuDict['value'], imuDict['sensor']) if s == 3], bins=100, color=zesty_palette[0])
+    plt.title("Gyroscope", fontsize=16, fontweight='bold')
+    if unitIMU == 'FPGA':
+        plt.xlabel('gyroX [fpga]', fontsize=10, fontweight='bold')
+    elif unitIMU == 'SI':
+        plt.xlabel('gyroX [rad/s]', fontsize=10, fontweight='bold')
+
+    plt.subplot(3,2,3)
+    sns.distplot([v for v, s in zip(imuDict['value'], imuDict['sensor']) if s == 1], bins=100, color=zesty_palette[1])
+    if unitIMU == 'FPGA':
+        plt.xlabel('accY [fpga]', fontsize=10, fontweight='bold')
+    elif unitIMU == 'SI':
+        plt.xlabel('accY [m/s]', fontsize=10, fontweight='bold')
+
+    plt.subplot(3,2,4)
+    sns.distplot([v for v, s in zip(imuDict['value'], imuDict['sensor']) if s == 4], bins=100, color=zesty_palette[1])
+    if unitIMU == 'FPGA':
+        plt.xlabel('gyroY [fpga]', fontsize=10, fontweight='bold')
+    elif unitIMU == 'SI':
+        plt.xlabel('gyroY [rad/s]', fontsize=10, fontweight='bold')
+
+    plt.subplot(3,2,5)
+    sns.distplot([v for v, s in zip(imuDict['value'], imuDict['sensor']) if s == 2], bins=100, color=zesty_palette[3])
+    if unitIMU == 'FPGA':
+        plt.xlabel('accZ [fpga]', fontsize=10, fontweight='bold')
+    elif unitIMU == 'SI':
+        plt.xlabel('accZ [m/s]', fontsize=10, fontweight='bold')
+
+    plt.subplot(3,2,6)
+    sns.distplot([v for v, s in zip(imuDict['value'], imuDict['sensor']) if s == 5], bins=100, color=zesty_palette[3])
+    if unitIMU == 'FPGA':
+        plt.xlabel('gyroZ [fpga]', fontsize=10, fontweight='bold')
+    elif unitIMU == 'SI':
+        plt.xlabel('gyroZ [rad/s]', fontsize=10, fontweight='bold')
+
+    fig.tight_layout()
+    if isinstance(fig_subtitle, str):
+        fig.subplots_adjust(top=0.85)
+    else:
+        fig.subplots_adjust(top=0.9)
+
+    if isinstance(fig_path, str) and isinstance(fig_name, str): 
+        plt.savefig(os.path.join(fig_path, fig_name + '.png'), dpi=300, bbox_inches='tight')
+        print("Saving " + fig_name + ".png")
+        plt.close()
+    else:
+        plt.show()
```

### Comparing `bimvee-1.0.9/bimvee/timestamps.py` & `bimvee-1.0.9.dev0/bimvee/timestamps.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,337 +1,465 @@
-# -*- coding: utf-8 -*-
-"""
-Copyright (C) 2019 Event-driven Perception for Robotics
-Author: Sim Bamford
-This program is free software: you can redistribute it and/or modify it under 
-the terms of the GNU General Public License as published by the Free Software 
-Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY 
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
-PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with 
-this program. If not, see <https://www.gnu.org/licenses/>.
-
-Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
-Various functions for working with timestamps
-
-zeroTimestamps(imports)
-
-imports can either be an importDict as produced by importAe, or it can be a list of them. 
-For each import, for each channel and for each datatype, the first timestamp is found. 
-We assume that these timestamps are already synchronised.
-We take the lowest, and use that to zero all the timestamps. 
-
-unwrapTimestamps()
-taking a numpy array (expected to by dtype=np.float64), return the array where
-any timestamp wrap events have been treated by advancing all the timestamps 
-after every wrap event.
-The 'wrapTime' argument is the time at which wrapping is expected to occur.
-If this is not given, then the maximum timestamp before each wrap event is used.
-    
-"""
-
-#%%
-
-import numpy as np
-
-def zeroTimestampsForADataType(dataTypeDict, tsOffset=None):
-    # Probably the common format is 'ts' for all dtypes, 
-    # but handle any exceptions here, example: if dtypeName == 'frame':
-    tsOffsetInitial = dataTypeDict.get('tsOffset', 0)
-    if tsOffset is None:
-        tsOffset = - np.min(dataTypeDict['ts'])
-    dataTypeDict['ts'] = dataTypeDict['ts'] + tsOffset
-    dataTypeDict['tsOffset'] = tsOffset + tsOffsetInitial
-
-def getFirstTimestampForAChannel(channelDict):
-    firstTimestamp = np.float64(np.inf)    
-    for dtypeName in channelDict:
-        # Probably the common format is 'ts' for all dtypes, 
-        # but handle any exceptions here, example: if dtypeName == 'frame':
-        try:
-            firstTimestamp = min(firstTimestamp, 
-                             channelDict[dtypeName]['ts'][0]) 
-        except KeyError:
-            # This dataType doesn't have a ts; no problem. 
-            pass
-    return firstTimestamp
-
-def zeroTimestampsForAChannel(channelDict, tsOffset=None):
-    if tsOffset is None:
-        tsOffset = -getFirstTimestampForAChannel(channelDict)
-    for dtypeName in channelDict:
-        # Probably the common format is 'ts' for all dtypes, 
-        # but handle any exceptions here, example: if dtypeName == 'frame':
-        try:
-            channelDict[dtypeName]['ts'] = channelDict[dtypeName]['ts'] + tsOffset
-            channelDict[dtypeName]['tsOffset'] = tsOffset
-        except KeyError:
-            # This dataType doesn't have a ts; no problem. 
-            pass
-
-''' 
-This function receives a single importedDict from importing one file. 
-It is focused on the problem of aligning data between multiple datatypes,
-Within the dataType dicts there are timestamps which may or may not come from a device, like Stefi.
-Let's call these data-level timestamps.
-At the level of the info branch of the dict we may have system clock time 
-at which a recording started.
-Let's call these info-level timestamps.
-This function only considers data-level timestamps.
-It assumes that timestamps have already been aligned individually within datatypes.
-Therefore each dataType dict which contains 'ts' should also contain 'tsOffset',
-which says how much time was added to the 'ts' field.
-This function aligns these so that the first event across the file is at ts = 0.
-The tsOffset needed to achieve this is then added to the info branch of the dict
-as tsOffsetFromData.
-'''    
-def rezeroTimestampsForAnImportedDict(importedDict):
-    # Find largest (i.e. least negative) offset
-    tsOffset = np.float64(-np.inf)
-    for channelName in importedDict['data']:
-        for dataType in importedDict['data'][channelName]:
-            tsOffset = max(tsOffset, importedDict['data'][channelName][dataType].get('tsOffset', -np.inf))
-    # Now we have the least negative tsOffset, iterate through all, reapplying it
-    for channelName in importedDict['data']:
-        for dataType in importedDict['data'][channelName]:
-            try:
-                tsOffsetCurrent = importedDict['data'][channelName][dataType].get('tsOffset', 0.0)
-                importedDict['data'][channelName][dataType]['ts'] = \
-                    importedDict['data'][channelName][dataType]['ts'] + tsOffset - tsOffsetCurrent
-                importedDict['data'][channelName][dataType]['tsOffset'] = tsOffset
-            except KeyError:
-                # This dataType doesn't have a ts; no problem. 
-                pass
-    importedDict['info']['tsOffsetFromData'] = tsOffset
-
-''' 
-This function receives a list of importedDicts - each one from importing one file. 
-It is focused on the problem of aligning data between multiple datatypes,
-Within the dataType dicts there are timestamps which might come from a device -
-let's call these data-level timestamps.
-At the level of info branch of the dict we have system clock time at which 
-a recording started - Let's call these info-level timestamps.
-It first calls the above function rezeroTimestampsForAnImportedDict for each file, 
-so that timestamps are aligned individually within the dict for each file. 
-The timestamp which was used to achieve this will be in ['info']['tsOffsetFromData'].
-There may additionally be ['info']['tsOffsetFromInfo'] - the info level timestamps.
-If info/level timestamops are available for all files, these are used to rezero
-all the data across multiple files.
-If any are absent, then they are ignored, and alignment across multiple files
-is based on data-level timestamps.
-'''      
-def rezeroTimestampsForImportedDicts(importedDicts):
-    if not isinstance(importedDicts, list):
-        importedDicts = [importedDicts]
-    # Find largest (i.e. least negative) offset
-    tsOffsetFromData = np.float64(-np.inf)
-    # Confusingly, info-level timestamps run in the other direction! TODO: could fix this
-    tsOffsetFromInfo = np.float64(np.inf)
-    allHaveInfoTsOffset = True
-    for importedDict in importedDicts:
-        rezeroTimestampsForAnImportedDict(importedDict)
-        tsOffsetFromData = max(tsOffsetFromData, importedDict['info']['tsOffsetFromData'])
-        if importedDict['info'].get('tsOffsetFromInfo', 0) != 0: # 0 is a placeholder used by the exporter - if it's zero, we assume it is not a real value that we care about.
-            tsOffsetFromInfo = min(tsOffsetFromInfo, importedDict['info']['tsOffsetFromInfo'])
-        else:
-            allHaveInfoTsOffset = False
-    if len(importedDicts) == 1:
-        return
-    # Now we have the extreme tsOffsets, iterate through all, reapplying 
-    for importedDict in importedDicts:
-        if allHaveInfoTsOffset and len(importedDicts) > 1:
-            if tsOffsetFromInfo == importedDict['info']['tsOffsetFromInfo']:
-                # The reason for this if clause is to catch a floating point 
-                # precision error due to mixing very big and very small timestamps. 
-                tsOffset = tsOffsetFromData                
-            else:
-                tsOffset = importedDict['info']['tsOffsetFromData'] - tsOffsetFromInfo + importedDict['info']['tsOffsetFromInfo']
-            
-        else:
-            tsOffset = tsOffsetFromData
-        for channelName in importedDict['data']:
-            for dataType in importedDict['data'][channelName]:
-                try:
-                    tsOffsetCurrent = importedDict['data'][channelName][dataType].get('tsOffset', 0.0)
-                    importedDict['data'][channelName][dataType]['ts'] = \
-                        importedDict['data'][channelName][dataType]['ts'] + tsOffset - tsOffsetCurrent
-                    importedDict['data'][channelName][dataType]['tsOffset'] = tsOffset
-                except KeyError:
-                    # This dataType doesn't have a ts; no problem. 
-                    pass
-
-'''
-using container as a general term for datatype dicts, channels, fileDicts or any hierarchical list of them...
-recurse through the structure, modifying timestamps and tsOffsets by a fixed amount
-'''
-def offsetTimestampsForAContainer(container, offset):
-    if isinstance(container, list):
-        for elem in container:
-            offsetTimestampsForAContainer(elem, offset)
-        return
-    if isinstance(container, dict):
-        if 'ts' in container:
-            # It's a datatype dict
-            container['ts'] = container['ts'] + offset
-            container['tsOffset'] = container['tsOffset'] + offset
-        else:
-            for field in container.values():
-                offsetTimestampsForAContainer(field, offset)
-    else:
-        # We have descended too far
-        return
-
-'''
-Takes ts where as int or float and returns it as float64, unwrapping where necessary.
-If you pass in wrapTime that takes precedence - make sure you pass in the right type though.
-If not, but you pass in tsBits (the number of timestamp bits), 
-then the wrapTime is 2**wrapTime.
-Otherwise, tsBits is guess by looking at the highest actual ts. 
-'''
-
-def unwrapTimestamps(ts, **kwargs):
-    wrapTime = kwargs.get('wrapTime', 2**int(kwargs.get('tsBits', np.ceil(np.log2(np.max(ts)))))) # This would fail in the edge case of e.g. max ts=64, but it's highly unlikely
-    # In the case that tsBits has been explicitly passed in, assume the input
-    # array is uint and remove any extra bits before continuing. 
-    tsBits = kwargs.get('tsBits')
-    if tsBits is not None and tsBits < 32:
-        ts = ts & (np.uint32(0x1 << tsBits) - 1)
-    ts = ts.astype(np.float64) 
-    diff = ts[1:] - ts[:-1] 
-    wrapPoints = np.where(diff < 0)[0]
-    for wrapPoint in wrapPoints:
-        ts[wrapPoint+1:] = ts[wrapPoint+1:] + wrapTime
-    return ts
-
-def cropSelectedFields(dataTypeDict, fieldList, selectedBool):
-    for fieldName in fieldList:
-        dataTypeDict[fieldName] = dataTypeDict[fieldName][selectedBool]
-
-'''
-Accepts a container at any level of the container hierarchy and finds the highest timestamp contained
-'''
-def getLastTimestamp(inDict):
-    lastTs = 0
-    if isinstance(inDict, list):
-        for inDictElement in inDict:
-            lastTs = max(lastTs, getLastTimestamp(inDictElement))
-    elif isinstance(inDict, dict):
-        if 'ts' in inDict:
-            return inDict['ts'][-1]
-        else: # It's a dictionary - go through it's elements
-            for keyName in inDict.keys():
-                lastTs = max(lastTs, getLastTimestamp(inDict[keyName]))
-    return lastTs
-
-'''
-cropDataByTimeRange was here - replaced by cropTime in split.py
-'''
-
-'''
-Sort a dict containing ts according to ts, applying the new sort order to all
-the fields where axis 0 
-'''
-def sortDataTypeDictByTime(inDict):
-    ts = inDict['ts']
-    ids = np.argsort(ts) 
-    numEvents = ts.shape[0]
-    outDict = {}
-    for fieldName in inDict.keys():
-        try:
-            assert len(inDict[fieldName]) == numEvents
-            outDict[fieldName] = inDict[fieldName][ids]
-        except (AssertionError, TypeError):
-            outDict[fieldName] = inDict[fieldName]
-    return outDict
-            
-#%% LEGACY CODE - timestamps for different data types present in aedat
-# There are exceptions around the timestamps for frame data to consider 
-'''
-def FindFirstAndLastTimeStamps(aedat):
-    
-    This is a sub-function of importAedat. 
-    For each field in aedat['data'], it finds the first and last timestamp. 
-    The min and max of these respectively are put into aedat.info
-    
-    
-    # Clip arrays to correct size and add them to the output structure.
-    # Also find first and last timeStamps
-    
-    if not 'data' in aedat:
-        print('No data found from which to extract time stamps')
-        return aedat
-    
-    firstTimeStamp = np.inf
-    lastTimeStamp = 0
-    
-    if 'special' in aedat['data']:
-    	if aedat['data']['special']['timeStamp'][0] < firstTimeStamp:
-    		firstTimeStamp = aedat['data']['special.timeStamp'][0]
-    	if aedat['data']['special']['timeStamp'][-1] > lastTimeStamp:
-    		lastTimeStamp = aedat['data']['special']['timeStamp'][-1]
-    
-    if 'polarity' in aedat['data']:
-    	if aedat['data']['polarity']['timeStamp'][0] < firstTimeStamp:
-    		firstTimeStamp = aedat['data']['polarity']['timeStamp'][0]
-    	if aedat['data']['polarity']['timeStamp'][-1] > lastTimeStamp:
-    		lastTimeStamp = aedat['data']['polarity']['timeStamp'][-1]
-    
-    if 'frame' in aedat['data']:    
-        if 'timeStampExposureStart' in aedat['data']['frame']:
-            if aedat['data']['frame']['timeStampExposureStart'][0] < firstTimeStamp:
-                firstTimeStamp = aedat['data']['frame']['timeStampExposureStart'][0]
-            if aedat['data']['frame']['timeStampExposureEnd'][-1] > lastTimeStamp:
-                lastTimeStamp = aedat['data']['frame']['timeStampExposureEnd'][-1]
-        else:
-            if aedat['data']['frame']['timeStampStart'][0] < firstTimeStamp:
-                firstTimeStamp = aedat['data']['frame']['timeStampStart'][0]
-            if aedat['data']['frame']['timeStampEnd'][-1] > lastTimeStamp:
-                lastTimeStamp = aedat['data']['frame']['timeStampEnd'][-1]
-    
-    if 'imu6' in aedat['data']:
-    	if aedat['data']['imu6']['timeStamp'][0] < firstTimeStamp:
-    		firstTimeStamp = aedat['data']['imu6']['timeStamp'][0]
-    	if aedat['data']['imu6']['timeStamp'][-1] > lastTimeStamp:
-    		lastTimeStamp = aedat['data']['imu6']['timeStamp'][-1]
-    
-    if 'sample' in aedat['data']:
-    	if aedat['data']['sample']['timeStamp'][0] < firstTimeStamp:
-    		firstTimeStamp = aedat['data']['sample']['timeStamp'][0]
-    	if aedat['data']['sample']['timeStamp'][-1] > lastTimeStamp:
-    		lastTimeStamp = aedat['data']['sample']['timeStamp'][-1]
-    
-    if 'ear' in aedat['data']:
-    	if aedat['data']['ear']['timeStamp'][0] < firstTimeStamp:
-    		firstTimeStamp = aedat['data']['ear']['timeStamp'][0]
-    	if aedat['data']['ear']['timeStamp'][-1] > lastTimeStamp:
-    		lastTimeStamp = aedat['data']['ear']['timeStamp'][-1]
-    
-    if 'point1D' in aedat['data']:
-    	if aedat['data']['point1D']['timeStamp'][0] < firstTimeStamp:
-    		firstTimeStamp = aedat['data']['point1D']['timeStamp'][0]
-    	if aedat['data']['point1D']['timeStamp'][-1] > lastTimeStamp:
-    		lastTimeStamp = aedat['data']['point1D']['timeStamp'][-1]
-    
-    if 'point2D' in aedat['data']:
-    	if aedat['data']['point2D']['timeStamp'][0] < firstTimeStamp:
-    		firstTimeStamp = aedat['data']['point2D']['timeStamp'][0]
-    	if aedat['data']['point2D']['timeStamp'][-1] > lastTimeStamp:
-    		lastTimeStamp = aedat['data']['point2D']['timeStamp'][-1]
-
-    if 'point3D' in aedat['data']:
-    	if aedat['data']['point3D']['timeStamp'][0] < firstTimeStamp:
-    		firstTimeStamp = aedat['data']['point3D']['timeStamp'][0]
-    	if aedat['data']['point3D']['timeStamp'][-1] > lastTimeStamp:
-    		lastTimeStamp = aedat['data']['point3D']['timeStamp'][-1]
-
-    if 'point4D' in aedat['data']:
-    	if aedat['data']['point4D']['timeStamp'][0] < firstTimeStamp:
-    		firstTimeStamp = aedat['data']['point4D']['timeStamp'][0]
-    	if aedat['data']['point4D']['timeStamp'][-1] > lastTimeStamp:
-    		lastTimeStamp = aedat['data']['point4D']['timeStamp'][-1]
-    
-    aedat['info']['firstTimeStamp'] = firstTimeStamp
-    aedat['info']['lastTimeStamp'] = lastTimeStamp
-
-    return aedat
+# -*- coding: utf-8 -*-
+"""
+Copyright (C) 2019 Event-driven Perception for Robotics
+Author: Sim Bamford
+This program is free software: you can redistribute it and/or modify it under 
+the terms of the GNU General Public License as published by the Free Software 
+Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY 
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
+PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with 
+this program. If not, see <https://www.gnu.org/licenses/>.
+
+Intended as part of bimvee (Batch Import, Manipulation, Visualisation and Export of Events etc)
+Various functions for working with timestamps
+
+zeroTimestamps(imports)
+
+imports can either be an importDict as produced by importAe, or it can be a list of them. 
+For each import, for each channel and for each datatype, the first timestamp is found. 
+We assume that these timestamps are already synchronised.
+We take the lowest, and use that to zero all the timestamps. 
+
+unwrapTimestamps()
+taking a numpy array (expected to by dtype=np.float64), return the array where
+any timestamp wrap events have been treated by advancing all the timestamps 
+after every wrap event.
+The 'wrapTime' argument is the time at which wrapping is expected to occur.
+If this is not given, then the maximum timestamp before each wrap event is used.
+    
+"""
+
+#%%
+
+import numpy as np
+import math
+
+def zeroTimestampsForADataType(dataTypeDict, tsOffset=None):
+    # Probably the common format is 'ts' for all dtypes, 
+    # but handle any exceptions here, example: if dtypeName == 'frame':
+    tsOffsetInitial = dataTypeDict.get('tsOffset', 0)
+    if tsOffset is None:
+        tsOffset = - np.min(dataTypeDict['ts'])
+    dataTypeDict['ts'] = dataTypeDict['ts'] + tsOffset
+    dataTypeDict['tsOffset'] = tsOffset + tsOffsetInitial
+
+def getFirstTimestampForAChannel(channelDict):
+    firstTimestamp = np.float64(np.inf)    
+    for dtypeName in channelDict:
+        # Probably the common format is 'ts' for all dtypes, 
+        # but handle any exceptions here, example: if dtypeName == 'frame':
+        try:
+            firstTimestamp = min(firstTimestamp, 
+                             channelDict[dtypeName]['ts'][0]) 
+        except KeyError:
+            # This dataType doesn't have a ts; no problem. 
+            pass
+    return firstTimestamp
+
+def zeroTimestampsForAChannelInSitu(channelDict, tsOffset=None):
+    if tsOffset is None:
+        tsOffset = -getFirstTimestampForAChannel(channelDict)
+    for dtypeName in channelDict:
+        try:
+            channelDict[dtypeName]['ts'] = channelDict[dtypeName]['ts'] + tsOffset
+            channelDict[dtypeName]['tsOffset'] = tsOffset
+        except KeyError:
+            # This dataType doesn't have a ts; no problem. 
+            pass
+
+
+'''
+Old behaviour was in situ - the same dicts were altered;
+This is retained as default behaviour for now for backwards compatibility
+TODO: deprecate old behaviour
+'''
+def zeroTimestampsForAChannel(channelDict, tsOffset=None, inSitu=True):
+    if inSitu:
+        zeroTimestampsForAChannelInSitu(channelDict, tsOffset)
+        return 
+    if tsOffset is None:
+        tsOffset = -getFirstTimestampForAChannel(channelDict)
+    newChannelDict = {}
+    for dataTypeName in channelDict.keys():
+        newDataTypeDict = channelDict[dataTypeName].copy()
+        try:
+            newDataTypeDict['ts'] = newDataTypeDict['ts'] + tsOffset
+            newDataTypeDict['tsOffset'] = tsOffset
+        except KeyError:
+            # This dataType doesn't have a ts; no problem. 
+            pass
+        newChannelDict[dataTypeName] = newDataTypeDict
+    return newChannelDict
+
+
+'''
+This function is similar to rezeroTimestampsForAnImportedDict below,
+but doesn't assume the info/data level of the dict structure.
+Also it doesn't modify dicts in situ but rather creates new ones.
+'''
+def rezeroTimestampsForMultipleChannels(inDict):
+    # Find largest (i.e. least negative) offset
+    tsOffset = np.float64(-np.inf)
+    for channelName in inDict:
+        for dataType in inDict[channelName]:
+            tsOffset = max(
+                tsOffset,
+                inDict[channelName][dataType].get('tsOffset', -np.inf))
+    # Now we have the least negative tsOffset, iterate through all, reapplying it
+    outDict = {}
+    for channelName in inDict:
+        outDict[channelName] = {}
+        for dataType in inDict[channelName]:
+            outDict[channelName][dataType] = inDict[channelName][dataType].copy()
+            try:
+                tsOffsetCurrent = outDict[channelName][dataType].get('tsOffset', 0.0)
+                outDict[channelName][dataType]['ts'] = (
+                    outDict[channelName][dataType]['ts'] +
+                    tsOffset - tsOffsetCurrent)
+                outDict[channelName][dataType]['tsOffset'] = tsOffset
+            except KeyError:
+                # This dataType doesn't have a ts; no problem. 
+                pass
+    return outDict, tsOffset
+
+'''
+First zero timestamps for each channel individually, and then realign them all jointly
+'''
+def zeroTimestampsForMultipleChannels(inDict):
+    intermediateDict = {}
+    for channelName in inDict:
+        intermediateDict[channelName] = zeroTimestampsForAChannel(
+            inDict[channelName], inSitu=False)
+    return rezeroTimestampsForMultipleChannels(intermediateDict)
+
+    
+''' 
+This function receives a single importedDict from importing one file. 
+It is focused on the problem of aligning data between multiple datatypes,
+Within the dataType dicts there are timestamps which may or may not come from a device, like Stefi.
+Let's call these data-level timestamps.
+At the level of the info branch of the dict we may have system clock time 
+at which a recording started.
+Let's call these info-level timestamps.
+This function only considers data-level timestamps.
+It assumes that timestamps have already been aligned individually within datatypes.
+Therefore each dataType dict which contains 'ts' should also contain 'tsOffset',
+which says how much time was added to the 'ts' field.
+This function aligns these so that the first event across the file is at ts = 0.
+The tsOffset needed to achieve this is then added to the info branch of the dict
+as tsOffsetFromData.
+TODO: Rebuild by calling rezeroTimestampsForMultipleChannels, above; this would
+also remove in-situ modification behaviour.
+'''
+def rezeroTimestampsForAnImportedDict(importedDict):
+    # Find largest (i.e. least negative) offset
+    tsOffset = np.float64(-np.inf)
+    for channelName in importedDict['data']:
+        for dataType in importedDict['data'][channelName]:
+            tsOffset = max(tsOffset, importedDict['data'][channelName][dataType].get('tsOffset', -np.inf))
+    # Now we have the least negative tsOffset, iterate through all, reapplying it
+    for channelName in importedDict['data']:
+        for dataType in importedDict['data'][channelName]:
+            try:
+                tsOffsetCurrent = importedDict['data'][channelName][dataType].get('tsOffset', 0.0)
+                importedDict['data'][channelName][dataType]['ts'] = \
+                    importedDict['data'][channelName][dataType]['ts'] + tsOffset - tsOffsetCurrent
+                importedDict['data'][channelName][dataType]['tsOffset'] = tsOffset
+            except KeyError:
+                # This dataType doesn't have a ts; no problem. 
+                pass
+    importedDict['info']['tsOffsetFromData'] = tsOffset
+
+''' 
+This function receives a list of importedDicts - each one from importing one file. 
+It is focused on the problem of aligning data between multiple datatypes,
+Within the dataType dicts there are timestamps which might come from a device -
+let's call these data-level timestamps.
+At the level of info branch of the dict we have system clock time at which 
+a recording started - Let's call these info-level timestamps.
+It first calls the above function rezeroTimestampsForAnImportedDict for each file, 
+so that timestamps are aligned individually within the dict for each file. 
+The timestamp which was used to achieve this will be in ['info']['tsOffsetFromData'].
+There may additionally be ['info']['tsOffsetFromInfo'] - the info level timestamps.
+If info/level timestamops are available for all files, these are used to rezero
+all the data across multiple files.
+If any are absent, then they are ignored, and alignment across multiple files
+is based on data-level timestamps.
+'''      
+def rezeroTimestampsForImportedDicts(importedDicts):
+    if not isinstance(importedDicts, list):
+        importedDicts = [importedDicts]
+    # Find largest (i.e. least negative) offset
+    tsOffsetFromData = np.float64(-np.inf)
+    # Confusingly, info-level timestamps run in the other direction! TODO: could fix this
+    tsOffsetFromInfo = np.float64(np.inf)
+    allHaveInfoTsOffset = True
+    for importedDict in importedDicts:
+        rezeroTimestampsForAnImportedDict(importedDict)
+        tsOffsetFromData = max(tsOffsetFromData, importedDict['info']['tsOffsetFromData'])
+        if importedDict['info'].get('tsOffsetFromInfo', 0) != 0: # 0 is a placeholder used by the exporter - if it's zero, we assume it is not a real value that we care about.
+            tsOffsetFromInfo = min(tsOffsetFromInfo, importedDict['info']['tsOffsetFromInfo'])
+        else:
+            allHaveInfoTsOffset = False
+    if len(importedDicts) == 1:
+        return
+    # Now we have the extreme tsOffsets, iterate through all, reapplying 
+    for importedDict in importedDicts:
+        if allHaveInfoTsOffset and len(importedDicts) > 1:
+            if tsOffsetFromInfo == importedDict['info']['tsOffsetFromInfo']:
+                # The reason for this if clause is to catch a floating point 
+                # precision error due to mixing very big and very small timestamps. 
+                tsOffset = importedDict['info']['tsOffsetFromData']                
+            else:
+                tsOffset = importedDict['info']['tsOffsetFromData'] - tsOffsetFromInfo + importedDict['info']['tsOffsetFromInfo']
+            
+        else:
+            tsOffset = tsOffsetFromData
+        for channelName in importedDict['data']:
+            for dataType in importedDict['data'][channelName]:
+                try:
+                    tsOffsetCurrent = importedDict['data'][channelName][dataType].get('tsOffset', 0.0)
+                    importedDict['data'][channelName][dataType]['ts'] = \
+                        importedDict['data'][channelName][dataType]['ts'] + tsOffset - tsOffsetCurrent
+                    importedDict['data'][channelName][dataType]['tsOffset'] = tsOffset
+                except KeyError:
+                    # This dataType doesn't have a ts; no problem. 
+                    pass
+
+'''
+using container as a general term for datatype dicts, channels, fileDicts or any hierarchical list of them...
+recurse through the structure, modifying timestamps and tsOffsets by a fixed amount
+'''
+def offsetTimestampsForAContainer(container, offset):
+    if isinstance(container, list):
+        for elem in container:
+            offsetTimestampsForAContainer(elem, offset)
+        return
+    if isinstance(container, dict):
+        if 'ts' in container:
+            # It's a datatype dict
+            container['ts'] = container['ts'] + offset
+            container['tsOffset'] = container['tsOffset'] + offset
+        else:
+            for field in container.values():
+                offsetTimestampsForAContainer(field, offset)
+    else:
+        # We have descended too far
+        return
+
+'''
+Takes ts where as int or float and returns it as float64, unwrapping where necessary.
+If you pass in wrapTime that takes precedence - make sure you pass in the right type though.
+If not, but you pass in tsBits (the number of timestamp bits), 
+then the wrapTime is 2**wrapTime.
+Otherwise, tsBits is guessed by looking at the highest actual ts. 
+'''
+
+def unwrapTimestamps(ts, **kwargs):
+    wrapTime = kwargs.get('wrapTime', 2**int(kwargs.get('tsBits', np.ceil(np.log2(np.max(ts)))))) # This would fail in the edge case of e.g. max ts=64, but it's highly unlikely
+    # In the case that tsBits has been explicitly passed in, assume the input
+    # array is uint and remove any extra bits before continuing. 
+    tsBits = kwargs.get('tsBits')
+    if tsBits is not None and tsBits < 32:
+        ts = ts & (np.uint32(0x1 << tsBits) - 1)
+    ts = ts.astype(np.float64) 
+    diff = ts[1:] - ts[:-1] 
+    wrapPoints = np.where(diff < 0)[0]
+    for wrapPoint in wrapPoints:
+        ts[wrapPoint+1:] = ts[wrapPoint+1:] + wrapTime
+    return ts
+
+def cropSelectedFields(dataTypeDict, fieldList, selectedBool):
+    for fieldName in fieldList:
+        dataTypeDict[fieldName] = dataTypeDict[fieldName][selectedBool]
+
+'''
+Accepts a container at any level of the container hierarchy and finds the highest timestamp contained
+'''
+def getLastTimestamp(inDict):
+    lastTs = 0
+    if isinstance(inDict, list):
+        for inDictElement in inDict:
+            lastTs = max(lastTs, getLastTimestamp(inDictElement))
+    elif isinstance(inDict, dict):
+        if 'ts' in inDict:
+            return inDict['ts'][-1]
+        else: # It's a dictionary - go through it's elements
+            for keyName in inDict.keys():
+                lastTs = max(lastTs, getLastTimestamp(inDict[keyName]))
+    return lastTs
+
+'''
+cropDataByTimeRange was here - replaced by cropTime in split.py
+'''
+
+'''
+Sort a dict containing ts according to ts, applying the new sort order to all
+the fields where axis 0 
+'''
+def sortDataTypeDictByTime(inDict):
+    try:
+        ts = inDict['ts']
+    except KeyError:
+        return inDict
+    ids = np.argsort(ts) 
+    numEvents = ts.shape[0]
+    outDict = {}
+    for fieldName in inDict.keys():
+        try:
+            if isinstance(inDict[fieldName], list):
+                assert len(inDict[fieldName]) == numEvents
+                outDict[fieldName] = [inDict[fieldName][idx] for idx in ids]
+            elif isinstance(inDict[fieldName], np.ndarray):
+                assert len(inDict[fieldName]) == numEvents
+                outDict[fieldName] = inDict[fieldName][ids]
+            else:
+                outDict[fieldName] = inDict[fieldName]
+        except (AssertionError, TypeError):
+            outDict[fieldName] = inDict[fieldName]
+    return outDict
+    
+'''
+If two or more file-level containers are merged, in general it's not possible 
+to align their timestamps without some extra prior knowledge. Here we reset
+all tsOffset fields, to avoid them being used to readjust timestamps incorrectly. 
+We assume that there's no overlap of channel names. 
+We also assume 
+'''    
+def mergeContainers(listOfDicts):
+    outDict = {'info': {'filePathOrName': 'merged'},
+               'data': {}}
+    for inDict in listOfDicts:
+        outDict['data'].update(inDict['data'])
+    for channelName in outDict['data']:
+        for dataTypeName in outDict['data'][channelName]:
+            outDict['data'][channelName][dataTypeName]['tsOffset'] = 0
+    return outDict
+
+
+# A function intended to find the nearest timestamp
+# adapted from https://stackoverflow.com/questions/2566412/find-nearest-value-in-numpy-array
+def findNearest(array, value):
+    idx = np.searchsorted(array, value) # side="left" param is the default
+    if idx > 0 and (idx == len(array) or math.fabs(value - array[idx-1]) < math.fabs(value - array[idx])):
+        return idx-1
+    else:
+        return idx
+
+def findNearestTsIdx(inDict, tsIdeal):
+    return findNearest(inDict['ts'], tsIdeal)
+
+def getNearestEvent(inDict, tsIdeal):
+    idx = findNearest(inDict['ts'], tsIdeal)
+    return getEvent(inDict, idx)
+
+'''
+Possibly a temporary home for this utility function
+Given any dataType container dict, return a dict which just contains the data
+for the indexed event or sample
+'''
+def getEvent(inDict, idx):
+    outDict = inDict.copy()
+    numEvents = len(outDict['ts'])
+    for key in outDict.keys():
+        try:
+            if len(outDict[key]) == numEvents:
+                outDict[key] = outDict[key][idx]
+        except TypeError:
+            continue
+    return outDict
+
+
+
+#%% LEGACY CODE - timestamps for different data types present in aedat
+# There are exceptions around the timestamps for frame data to consider 
+'''
+def FindFirstAndLastTimeStamps(aedat):
+    
+    This is a sub-function of importAedat. 
+    For each field in aedat['data'], it finds the first and last timestamp. 
+    The min and max of these respectively are put into aedat.info
+    
+    
+    # Clip arrays to correct size and add them to the output structure.
+    # Also find first and last timeStamps
+    
+    if not 'data' in aedat:
+        print('No data found from which to extract time stamps')
+        return aedat
+    
+    firstTimeStamp = np.inf
+    lastTimeStamp = 0
+    
+    if 'special' in aedat['data']:
+    	if aedat['data']['special']['timeStamp'][0] < firstTimeStamp:
+    		firstTimeStamp = aedat['data']['special.timeStamp'][0]
+    	if aedat['data']['special']['timeStamp'][-1] > lastTimeStamp:
+    		lastTimeStamp = aedat['data']['special']['timeStamp'][-1]
+    
+    if 'polarity' in aedat['data']:
+    	if aedat['data']['polarity']['timeStamp'][0] < firstTimeStamp:
+    		firstTimeStamp = aedat['data']['polarity']['timeStamp'][0]
+    	if aedat['data']['polarity']['timeStamp'][-1] > lastTimeStamp:
+    		lastTimeStamp = aedat['data']['polarity']['timeStamp'][-1]
+    
+    if 'frame' in aedat['data']:    
+        if 'timeStampExposureStart' in aedat['data']['frame']:
+            if aedat['data']['frame']['timeStampExposureStart'][0] < firstTimeStamp:
+                firstTimeStamp = aedat['data']['frame']['timeStampExposureStart'][0]
+            if aedat['data']['frame']['timeStampExposureEnd'][-1] > lastTimeStamp:
+                lastTimeStamp = aedat['data']['frame']['timeStampExposureEnd'][-1]
+        else:
+            if aedat['data']['frame']['timeStampStart'][0] < firstTimeStamp:
+                firstTimeStamp = aedat['data']['frame']['timeStampStart'][0]
+            if aedat['data']['frame']['timeStampEnd'][-1] > lastTimeStamp:
+                lastTimeStamp = aedat['data']['frame']['timeStampEnd'][-1]
+    
+    if 'imu6' in aedat['data']:
+    	if aedat['data']['imu6']['timeStamp'][0] < firstTimeStamp:
+    		firstTimeStamp = aedat['data']['imu6']['timeStamp'][0]
+    	if aedat['data']['imu6']['timeStamp'][-1] > lastTimeStamp:
+    		lastTimeStamp = aedat['data']['imu6']['timeStamp'][-1]
+    
+    if 'sample' in aedat['data']:
+    	if aedat['data']['sample']['timeStamp'][0] < firstTimeStamp:
+    		firstTimeStamp = aedat['data']['sample']['timeStamp'][0]
+    	if aedat['data']['sample']['timeStamp'][-1] > lastTimeStamp:
+    		lastTimeStamp = aedat['data']['sample']['timeStamp'][-1]
+    
+    if 'ear' in aedat['data']:
+    	if aedat['data']['ear']['timeStamp'][0] < firstTimeStamp:
+    		firstTimeStamp = aedat['data']['ear']['timeStamp'][0]
+    	if aedat['data']['ear']['timeStamp'][-1] > lastTimeStamp:
+    		lastTimeStamp = aedat['data']['ear']['timeStamp'][-1]
+    
+    if 'point1D' in aedat['data']:
+    	if aedat['data']['point1D']['timeStamp'][0] < firstTimeStamp:
+    		firstTimeStamp = aedat['data']['point1D']['timeStamp'][0]
+    	if aedat['data']['point1D']['timeStamp'][-1] > lastTimeStamp:
+    		lastTimeStamp = aedat['data']['point1D']['timeStamp'][-1]
+    
+    if 'point2D' in aedat['data']:
+    	if aedat['data']['point2D']['timeStamp'][0] < firstTimeStamp:
+    		firstTimeStamp = aedat['data']['point2D']['timeStamp'][0]
+    	if aedat['data']['point2D']['timeStamp'][-1] > lastTimeStamp:
+    		lastTimeStamp = aedat['data']['point2D']['timeStamp'][-1]
+
+    if 'point3D' in aedat['data']:
+    	if aedat['data']['point3D']['timeStamp'][0] < firstTimeStamp:
+    		firstTimeStamp = aedat['data']['point3D']['timeStamp'][0]
+    	if aedat['data']['point3D']['timeStamp'][-1] > lastTimeStamp:
+    		lastTimeStamp = aedat['data']['point3D']['timeStamp'][-1]
+
+    if 'point4D' in aedat['data']:
+    	if aedat['data']['point4D']['timeStamp'][0] < firstTimeStamp:
+    		firstTimeStamp = aedat['data']['point4D']['timeStamp'][0]
+    	if aedat['data']['point4D']['timeStamp'][-1] > lastTimeStamp:
+    		lastTimeStamp = aedat['data']['point4D']['timeStamp'][-1]
+    
+    aedat['info']['firstTimeStamp'] = firstTimeStamp
+    aedat['info']['lastTimeStamp'] = lastTimeStamp
+
+    return aedat
 '''
```

### Comparing `bimvee-1.0.9/bimvee.egg-info/SOURCES.txt` & `bimvee-1.0.9.dev0/bimvee.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 LICENSE.txt
 README.md
 setup.cfg
 setup.py
 bimvee/__init__.py
 bimvee/container.py
+bimvee/events.py
 bimvee/exportHdf5.py
 bimvee/exportIitYarp.py
 bimvee/exportPoseRpgEsimCsv.py
+bimvee/exportRpgDvsRos.py
 bimvee/geometry.py
 bimvee/importAe.py
 bimvee/importAer2.py
+bimvee/importBoundingBoxes.py
 bimvee/importExportBatches.py
 bimvee/importFrames.py
 bimvee/importHdf5.py
 bimvee/importIitNumpy.py
 bimvee/importIitVicon.py
 bimvee/importIitYarp.py
+bimvee/importProph.py
 bimvee/importRpgDvsRos.py
 bimvee/importSecDvs.py
+bimvee/importSkeleton.py
+bimvee/importUdsAedat.py
 bimvee/info.py
 bimvee/plot.py
 bimvee/plotCorrelogram.py
 bimvee/plotDvsContrast.py
 bimvee/plotDvsLastTs.py
+bimvee/plotDvsSpaceTime.py
 bimvee/plotEventRate.py
 bimvee/plotFlow.py
 bimvee/plotFrame.py
 bimvee/plotImu.py
 bimvee/plotPose.py
 bimvee/plotSpikeogram.py
 bimvee/pose.py
@@ -34,21 +41,32 @@
 bimvee/timestamps.py
 bimvee/visualiser.py
 bimvee.egg-info/PKG-INFO
 bimvee.egg-info/SOURCES.txt
 bimvee.egg-info/dependency_links.txt
 bimvee.egg-info/requires.txt
 bimvee.egg-info/top_level.txt
+bimvee/importRosbag/setup.py
 bimvee/importRosbag/importRosbag/__init__.py
 bimvee/importRosbag/importRosbag/importRosbag.py
 bimvee/importRosbag/importRosbag/messageTypes/common.py
 bimvee/importRosbag/importRosbag/messageTypes/dvs_msgs_EventArray.py
 bimvee/importRosbag/importRosbag/messageTypes/esim_msgs_OpticFlow.py
 bimvee/importRosbag/importRosbag/messageTypes/geometry_msgs_PoseStamped.py
 bimvee/importRosbag/importRosbag/messageTypes/geometry_msgs_Transform.py
 bimvee/importRosbag/importRosbag/messageTypes/geometry_msgs_TransformStamped.py
 bimvee/importRosbag/importRosbag/messageTypes/geometry_msgs_TwistStamped.py
 bimvee/importRosbag/importRosbag/messageTypes/sensor_msgs_CameraInfo.py
 bimvee/importRosbag/importRosbag/messageTypes/sensor_msgs_Image.py
 bimvee/importRosbag/importRosbag/messageTypes/sensor_msgs_Imu.py
 bimvee/importRosbag/importRosbag/messageTypes/sensor_msgs_PointCloud2.py
-bimvee/importRosbag/importRosbag/messageTypes/tf_tfMessage.py
+bimvee/importRosbag/importRosbag/messageTypes/tf_tfMessage.py
+bimvee/visualisers/__init__.py
+bimvee/visualisers/visualiserBase.py
+bimvee/visualisers/visualiserBoundingBoxes.py
+bimvee/visualisers/visualiserDvs.py
+bimvee/visualisers/visualiserFrame.py
+bimvee/visualisers/visualiserImu.py
+bimvee/visualisers/visualiserOpticFlow.py
+bimvee/visualisers/visualiserPoint3.py
+bimvee/visualisers/visualiserPose6q.py
+bimvee/visualisers/visualiserSkeleton.py
```

### Comparing `bimvee-1.0.9/setup.py` & `bimvee-1.0.9.dev0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,43 @@
-# Always prefer setuptools over distutils
-from setuptools import setup, find_packages
-# To use a consistent encoding
-from os import path
-
-here = path.abspath(path.dirname(__file__))
-
-# Get the long description from the README file
-with open(path.join(here, 'README.md'), encoding='utf-8') as f:
-    long_description = f.read()
-    
-setup(
-  name = 'bimvee',
-  packages=['bimvee', 'bimvee.importRosbag.importRosbag', 'bimvee.importRosbag.importRosbag.messageTypes'],
-  version = '1.0.9',
-  license='gpl',
-  description = 'Batch Import, Manipulation, Visualisation and Export of Events etc',
-  long_description=long_description,
-  long_description_content_type='text/markdown',
-  author = 'Event-driven Perception for Robotics group at Istituto Italiano di Tecnologia: Simeon Bamford, Suman Ghosh, Aiko Dinale, Massimiliano Iaconi, Ander Arriandiaga, etc',
-  author_email = 'simbamford@gmail.com',
-  url = 'https://github.com/event-driven-robotics/bimvee',
-  download_url = 'https://github.com/event-driven-robotics/bimvee_pkg/archive/v1.0.tar.gz',
-  keywords = ['event', 'event camera', 'event-based', 'event-driven', 'spike', 'dvs', 'dynamic vision sensor', 'neuromorphic', 'aer', 'address-event representation' 'spiking neural network', 'davis', 'atis', 'celex' ],
-  install_requires=[
-          'numpy',
-          'tqdm',
-          'setuptools',
-          'matplotlib',
-          'seaborn',
-          'imageio',
-          'hickle'
-      ],
-  classifiers=[
-    'Development Status :: 3 - Alpha',
-    'Intended Audience :: Developers',
-    'Topic :: Software Development :: Build Tools',
-    'License :: OSI Approved :: GNU General Public License (GPL)',
-    'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.7',
-  ],
-)
+# Always prefer setuptools over distutils
+from setuptools import setup, find_packages
+# To use a consistent encoding
+from os import path
+
+here = path.abspath(path.dirname(__file__))
+
+# Get the long description from the README file
+with open(path.join(here, 'README.md'), encoding='utf-8') as f:
+    long_description = f.read()
+    
+setup(
+  name = 'bimvee',
+  packages=['bimvee', 'bimvee.importRosbag', 'bimvee.importRosbag.importRosbag', 'bimvee.importRosbag.importRosbag.messageTypes', 'bimvee.visualisers'],
+  version = '1.0.9dev',
+  license='gpl',
+  description = 'Batch Import, Manipulation, Visualisation and Export of Events etc',
+  long_description=long_description,
+  long_description_content_type='text/markdown',
+  author = 'Event-driven Perception for Robotics group at Istituto Italiano di Tecnologia: Simeon Bamford, Suman Ghosh, Aiko Dinale, Massimiliano Iacono, Ander Arriandiaga, etc',
+  author_email = 'simbamford@gmail.com',
+  url = 'https://github.com/event-driven-robotics/bimvee',
+  download_url = 'https://github.com/event-driven-robotics/bimvee_pkg/archive/v1.0.tar.gz',
+  keywords = ['event', 'event camera', 'event-based', 'event-driven', 'spike', 'dvs', 'dynamic vision sensor', 'neuromorphic', 'aer', 'address-event representation' 'spiking neural network', 'davis', 'atis', 'celex' ],
+  install_requires=[
+          'numpy',
+          'tqdm',
+          'setuptools',
+          'matplotlib',
+          'seaborn',
+          'imageio',
+          'hickle',
+          'opencv-python'
+      ],
+  classifiers=[
+    'Development Status :: 3 - Alpha',
+    'Intended Audience :: Developers',
+    'Topic :: Software Development :: Build Tools',
+    'License :: OSI Approved :: GNU General Public License (GPL)',
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3.7',
+  ],
+)
```

