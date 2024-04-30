# Comparing `tmp/mobile-env-rl-3.5.tar.gz` & `tmp/mobile_env_rl-3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobile-env-rl-3.5.tar", last modified: Mon Dec 18 11:13:35 2023, max compression
+gzip compressed data, was "mobile_env_rl-3.6.tar", last modified: Tue Apr 30 07:05:48 2024, max compression
```

## Comparing `mobile-env-rl-3.5.tar` & `mobile_env_rl-3.6.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-12-18 11:13:35.213533 mobile-env-rl-3.5/
--rw-r--r--   0 david     (1000) david     (1000)    11357 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/LICENSE
--rw-r--r--   0 david     (1000) david     (1000)    24115 2023-12-18 11:13:35.213533 mobile-env-rl-3.5/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)     9723 2023-12-18 10:59:57.000000 mobile-env-rl-3.5/README.md
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-12-18 11:13:35.126868 mobile-env-rl-3.5/android_env/
--rw-r--r--   0 david     (1000) david     (1000)      736 2023-09-21 07:17:48.000000 mobile-env-rl-3.5/android_env/__init__.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-12-18 11:13:35.126868 mobile-env-rl-3.5/android_env/components/
--rw-r--r--   0 david     (1000) david     (1000)      610 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/android_env/components/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)     1473 2023-03-10 15:36:10.000000 mobile-env-rl-3.5/android_env/components/action_type.py
--rw-r--r--   0 david     (1000) david     (1000)    29061 2023-11-01 06:36:26.000000 mobile-env-rl-3.5/android_env/components/adb_controller.py
--rw-r--r--   0 david     (1000) david     (1000)    16011 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/android_env/components/adb_controller_test.py
--rw-r--r--   0 david     (1000) david     (1000)     1462 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/android_env/components/adb_log_stream.py
--rw-r--r--   0 david     (1000) david     (1000)     1560 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/android_env/components/adb_log_stream_test.py
--rw-r--r--   0 david     (1000) david     (1000)    12159 2023-11-21 13:26:37.000000 mobile-env-rl-3.5/android_env/components/app_screen_checker.py
--rw-r--r--   0 david     (1000) david     (1000)     5955 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/android_env/components/app_screen_checker_test.py
--rw-r--r--   0 david     (1000) david     (1000)    25660 2023-12-12 10:37:19.000000 mobile-env-rl-3.5/android_env/components/coordinator.py
--rw-r--r--   0 david     (1000) david     (1000)     6308 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/android_env/components/coordinator_test.py
--rw-r--r--   0 david     (1000) david     (1000)     6292 2023-11-21 13:26:37.000000 mobile-env-rl-3.5/android_env/components/dumpsys_thread.py
--rw-r--r--   0 david     (1000) david     (1000)     3567 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/android_env/components/dumpsys_thread_test.py
--rw-r--r--   0 david     (1000) david     (1000)     3098 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/android_env/components/errors.py
--rw-r--r--   0 david     (1000) david     (1000)    38093 2023-11-30 15:03:42.000000 mobile-env-rl-3.5/android_env/components/event_listeners.py
--rw-r--r--   0 david     (1000) david     (1000)     1570 2023-09-21 07:17:48.000000 mobile-env-rl-3.5/android_env/components/log_stream.py
--rw-r--r--   0 david     (1000) david     (1000)     2485 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/android_env/components/log_stream_test.py
--rw-r--r--   0 david     (1000) david     (1000)     7591 2023-03-10 15:36:10.000000 mobile-env-rl-3.5/android_env/components/logcat_thread.py
--rw-r--r--   0 david     (1000) david     (1000)     4370 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/android_env/components/logcat_thread_test.py
--rw-r--r--   0 david     (1000) david     (1000)    15562 2023-11-21 13:26:37.000000 mobile-env-rl-3.5/android_env/components/screen_analyzer_thread.py
--rw-r--r--   0 david     (1000) david     (1000)    12602 2023-03-10 15:36:10.000000 mobile-env-rl-3.5/android_env/components/setup_step_interpreter.py
--rw-r--r--   0 david     (1000) david     (1000)    14297 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/android_env/components/setup_step_interpreter_test.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-12-18 11:13:35.126868 mobile-env-rl-3.5/android_env/components/simulators/
--rw-r--r--   0 david     (1000) david     (1000)     1009 2023-09-21 07:17:48.000000 mobile-env-rl-3.5/android_env/components/simulators/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)     8705 2023-12-12 10:37:19.000000 mobile-env-rl-3.5/android_env/components/simulators/base_simulator.py
--rw-r--r--   0 david     (1000) david     (1000)     5734 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/android_env/components/simulators/base_simulator_test.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-12-18 11:13:35.130201 mobile-env-rl-3.5/android_env/components/simulators/emulator/
--rw-r--r--   0 david     (1000) david     (1000)      610 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/android_env/components/simulators/emulator/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)     9766 2023-09-21 03:02:32.000000 mobile-env-rl-3.5/android_env/components/simulators/emulator/emulator_launcher.py
--rw-r--r--   0 david     (1000) david     (1000)     5734 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/android_env/components/simulators/emulator/emulator_launcher_test.py
--rw-r--r--   0 david     (1000) david     (1000)     8274 2023-12-12 10:37:19.000000 mobile-env-rl-3.5/android_env/components/simulators/emulator/emulator_simulator.py
--rw-r--r--   0 david     (1000) david     (1000)     9058 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/android_env/components/simulators/emulator/emulator_simulator_test.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-12-18 11:13:35.130201 mobile-env-rl-3.5/android_env/components/simulators/fake/
--rw-r--r--   0 david     (1000) david     (1000)      610 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/android_env/components/simulators/fake/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)     5030 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/android_env/components/simulators/fake/fake_simulator.py
--rw-r--r--   0 david     (1000) david     (1000)     2586 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/android_env/components/simulators/fake/fake_simulator_test.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-12-18 11:13:35.130201 mobile-env-rl-3.5/android_env/components/simulators/remote/
--rw-r--r--   0 david     (1000) david     (1000)      621 2023-09-21 07:17:48.000000 mobile-env-rl-3.5/android_env/components/simulators/remote/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)    10564 2023-12-12 10:37:19.000000 mobile-env-rl-3.5/android_env/components/simulators/remote/daemon.py
--rw-r--r--   0 david     (1000) david     (1000)     4230 2023-12-11 09:35:13.000000 mobile-env-rl-3.5/android_env/components/simulators/remote/remote_adb_controller.py
--rw-r--r--   0 david     (1000) david     (1000)     2407 2023-09-21 07:17:48.000000 mobile-env-rl-3.5/android_env/components/simulators/remote/remote_base.py
--rw-r--r--   0 david     (1000) david     (1000)     2498 2023-09-21 07:17:48.000000 mobile-env-rl-3.5/android_env/components/simulators/remote/remote_log_stream.py
--rw-r--r--   0 david     (1000) david     (1000)    10652 2023-12-12 11:28:18.000000 mobile-env-rl-3.5/android_env/components/simulators/remote/remote_simulator.py
--rw-r--r--   0 david     (1000) david     (1000)     6722 2023-06-30 11:54:24.000000 mobile-env-rl-3.5/android_env/components/specs.py
--rw-r--r--   0 david     (1000) david     (1000)     5002 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/android_env/components/specs_test.py
--rw-r--r--   0 david     (1000) david     (1000)    46873 2023-12-01 01:50:07.000000 mobile-env-rl-3.5/android_env/components/task_manager.py
--rw-r--r--   0 david     (1000) david     (1000)    12689 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/android_env/components/task_manager_test.py
--rw-r--r--   0 david     (1000) david     (1000)     3815 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/android_env/components/thread_function.py
--rw-r--r--   0 david     (1000) david     (1000)     2153 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/android_env/components/thread_function_test.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-12-18 11:13:35.130201 mobile-env-rl-3.5/android_env/components/tools/
--rw-r--r--   0 david     (1000) david     (1000)      628 2023-03-10 15:36:10.000000 mobile-env-rl-3.5/android_env/components/tools/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)     8066 2023-12-07 14:04:27.000000 mobile-env-rl-3.5/android_env/components/tools/easyocr_wrapper.py
--rw-r--r--   0 david     (1000) david     (1000)     3635 2023-03-10 15:36:10.000000 mobile-env-rl-3.5/android_env/components/tools/naive_functions.py
--rw-r--r--   0 david     (1000) david     (1000)     1046 2023-12-01 01:32:42.000000 mobile-env-rl-3.5/android_env/components/tools/sbert_holder.py
--rw-r--r--   0 david     (1000) david     (1000)     3579 2023-03-10 15:36:10.000000 mobile-env-rl-3.5/android_env/components/tools/types.py
--rw-r--r--   0 david     (1000) david     (1000)     1831 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/android_env/components/utils.py
--rw-r--r--   0 david     (1000) david     (1000)     2787 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/android_env/components/utils_test.py
--rw-r--r--   0 david     (1000) david     (1000)     5239 2023-11-21 13:26:37.000000 mobile-env-rl-3.5/android_env/components/vh_analyzer_thread.py
--rw-r--r--   0 david     (1000) david     (1000)     8455 2023-12-12 10:37:19.000000 mobile-env-rl-3.5/android_env/environment.py
--rw-r--r--   0 david     (1000) david     (1000)     6499 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/android_env/environment_test.py
--rw-r--r--   0 david     (1000) david     (1000)    16871 2023-12-12 11:27:44.000000 mobile-env-rl-3.5/android_env/loader.py
--rw-r--r--   0 david     (1000) david     (1000)     3591 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/android_env/loader_test.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-12-18 11:13:35.176867 mobile-env-rl-3.5/android_env/proto/
--rw-r--r--   0 david     (1000) david     (1000)      610 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/android_env/proto/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)     3792 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/android_env/proto/adb.proto
--rw-r--r--   0 david     (1000) david     (1000)     6581 2023-11-29 11:46:08.000000 mobile-env-rl-3.5/android_env/proto/adb_pb2.py
--rw-r--r--   0 david     (1000) david     (1000)      159 2023-11-29 11:46:08.000000 mobile-env-rl-3.5/android_env/proto/adb_pb2_grpc.py
--rw-r--r--   0 david     (1000) david     (1000)    41044 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/android_env/proto/emulator_controller.proto
--rw-r--r--   0 david     (1000) david     (1000)    23631 2023-11-29 11:46:08.000000 mobile-env-rl-3.5/android_env/proto/emulator_controller_pb2.py
--rw-r--r--   0 david     (1000) david     (1000)    67018 2023-11-29 11:46:08.000000 mobile-env-rl-3.5/android_env/proto/emulator_controller_pb2_grpc.py
--rw-r--r--   0 david     (1000) david     (1000)     1327 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/android_env/proto/raw_observation.proto
--rw-r--r--   0 david     (1000) david     (1000)     1471 2023-11-29 11:46:08.000000 mobile-env-rl-3.5/android_env/proto/raw_observation_pb2.py
--rw-r--r--   0 david     (1000) david     (1000)      159 2023-11-29 11:46:08.000000 mobile-env-rl-3.5/android_env/proto/raw_observation_pb2_grpc.py
--rw-r--r--   0 david     (1000) david     (1000)    11922 2023-11-29 10:47:25.000000 mobile-env-rl-3.5/android_env/proto/task.proto
--rw-r--r--   0 david     (1000) david     (1000)    10417 2023-11-29 11:46:08.000000 mobile-env-rl-3.5/android_env/proto/task_pb2.py
--rw-r--r--   0 david     (1000) david     (1000)      159 2023-11-29 11:46:08.000000 mobile-env-rl-3.5/android_env/proto/task_pb2_grpc.py
--rw-r--r--   0 david     (1000) david     (1000)     2143 2023-04-15 09:07:59.000000 mobile-env-rl-3.5/android_env/utils.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-12-18 11:13:35.180200 mobile-env-rl-3.5/android_env/wrappers/
--rw-r--r--   0 david     (1000) david     (1000)     2285 2023-12-06 11:24:33.000000 mobile-env-rl-3.5/android_env/wrappers/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)     3112 2023-08-22 08:25:54.000000 mobile-env-rl-3.5/android_env/wrappers/base_wrapper.py
--rw-r--r--   0 david     (1000) david     (1000)     9011 2023-03-10 15:36:10.000000 mobile-env-rl-3.5/android_env/wrappers/discrete_action_wrapper.py
--rw-r--r--   0 david     (1000) david     (1000)     4814 2023-03-10 15:36:10.000000 mobile-env-rl-3.5/android_env/wrappers/flat_interface_wrapper.py
--rw-r--r--   0 david     (1000) david     (1000)     3984 2023-03-10 15:36:10.000000 mobile-env-rl-3.5/android_env/wrappers/float_pixels_wrapper.py
--rw-r--r--   0 david     (1000) david     (1000)     3914 2023-03-10 15:36:10.000000 mobile-env-rl-3.5/android_env/wrappers/gym_wrapper.py
--rw-r--r--   0 david     (1000) david     (1000)     5178 2023-12-06 14:03:11.000000 mobile-env-rl-3.5/android_env/wrappers/image_rescale_wrapper.py
--rw-r--r--   0 david     (1000) david     (1000)     4312 2021-11-28 12:52:01.000000 mobile-env-rl-3.5/android_env/wrappers/last_action_wrapper.py
--rw-r--r--   0 david     (1000) david     (1000)     5821 2023-11-21 13:26:37.000000 mobile-env-rl-3.5/android_env/wrappers/recorder_wrapper.py
--rw-r--r--   0 david     (1000) david     (1000)    13653 2023-12-12 10:37:19.000000 mobile-env-rl-3.5/android_env/wrappers/tap_action_wrapper.py
--rw-r--r--   0 david     (1000) david     (1000)    16648 2023-12-12 10:37:19.000000 mobile-env-rl-3.5/android_env/wrappers/vh_io_wrapper.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-12-18 11:13:35.213533 mobile-env-rl-3.5/mobile_env_rl.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)    24115 2023-12-18 11:13:35.000000 mobile-env-rl-3.5/mobile_env_rl.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)     3817 2023-12-18 11:13:35.000000 mobile-env-rl-3.5/mobile_env_rl.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2023-12-18 11:13:35.000000 mobile-env-rl-3.5/mobile_env_rl.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)      294 2023-12-18 11:13:35.000000 mobile-env-rl-3.5/mobile_env_rl.egg-info/requires.txt
--rw-r--r--   0 david     (1000) david     (1000)       12 2023-12-18 11:13:35.000000 mobile-env-rl-3.5/mobile_env_rl.egg-info/top_level.txt
--rw-r--r--   0 david     (1000) david     (1000)     1123 2023-12-18 06:36:05.000000 mobile-env-rl-3.5/pyproject.toml
--rw-r--r--   0 david     (1000) david     (1000)       38 2023-12-18 11:13:35.213533 mobile-env-rl-3.5/setup.cfg
--rw-r--r--   0 david     (1000) david     (1000)     4708 2023-12-18 06:35:40.000000 mobile-env-rl-3.5/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-12-18 11:13:35.180200 mobile-env-rl-3.5/tests/
--rw-r--r--   0 david     (1000) david     (1000)     2984 2023-10-31 08:21:33.000000 mobile-env-rl-3.5/tests/test_css_selector.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-04-30 07:05:48.912834 mobile_env_rl-3.6/
+-rw-r--r--   0 david     (1000) david     (1000)    11357 2021-11-28 12:52:01.000000 mobile_env_rl-3.6/LICENSE
+-rw-r--r--   0 david     (1000) david     (1000)    24819 2024-04-30 07:05:48.912834 mobile_env_rl-3.6/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)    10427 2024-04-30 06:54:18.000000 mobile_env_rl-3.6/README.md
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-04-30 07:05:48.789505 mobile_env_rl-3.6/android_env/
+-rw-r--r--   0 david     (1000) david     (1000)      736 2023-12-18 11:31:48.000000 mobile_env_rl-3.6/android_env/__init__.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-04-30 07:05:48.792838 mobile_env_rl-3.6/android_env/components/
+-rw-r--r--   0 david     (1000) david     (1000)      610 2021-11-28 12:52:01.000000 mobile_env_rl-3.6/android_env/components/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)     1473 2023-03-10 15:36:10.000000 mobile_env_rl-3.6/android_env/components/action_type.py
+-rw-r--r--   0 david     (1000) david     (1000)    29061 2023-12-18 11:31:48.000000 mobile_env_rl-3.6/android_env/components/adb_controller.py
+-rw-r--r--   0 david     (1000) david     (1000)    16011 2021-11-28 12:52:01.000000 mobile_env_rl-3.6/android_env/components/adb_controller_test.py
+-rw-r--r--   0 david     (1000) david     (1000)     1462 2021-11-28 12:52:01.000000 mobile_env_rl-3.6/android_env/components/adb_log_stream.py
+-rw-r--r--   0 david     (1000) david     (1000)     1560 2021-11-28 12:52:01.000000 mobile_env_rl-3.6/android_env/components/adb_log_stream_test.py
+-rw-r--r--   0 david     (1000) david     (1000)    12159 2023-12-18 11:31:48.000000 mobile_env_rl-3.6/android_env/components/app_screen_checker.py
+-rw-r--r--   0 david     (1000) david     (1000)     5955 2021-11-28 12:52:01.000000 mobile_env_rl-3.6/android_env/components/app_screen_checker_test.py
+-rw-r--r--   0 david     (1000) david     (1000)    25660 2023-12-18 11:31:48.000000 mobile_env_rl-3.6/android_env/components/coordinator.py
+-rw-r--r--   0 david     (1000) david     (1000)     6308 2021-11-28 12:52:01.000000 mobile_env_rl-3.6/android_env/components/coordinator_test.py
+-rw-r--r--   0 david     (1000) david     (1000)     6292 2023-12-18 11:31:48.000000 mobile_env_rl-3.6/android_env/components/dumpsys_thread.py
+-rw-r--r--   0 david     (1000) david     (1000)     3567 2021-11-28 12:52:01.000000 mobile_env_rl-3.6/android_env/components/dumpsys_thread_test.py
+-rw-r--r--   0 david     (1000) david     (1000)     3098 2021-11-28 12:52:01.000000 mobile_env_rl-3.6/android_env/components/errors.py
+-rw-r--r--   0 david     (1000) david     (1000)    38093 2024-03-11 07:40:42.000000 mobile_env_rl-3.6/android_env/components/event_listeners.py
+-rw-r--r--   0 david     (1000) david     (1000)     1570 2023-12-18 11:31:48.000000 mobile_env_rl-3.6/android_env/components/log_stream.py
+-rw-r--r--   0 david     (1000) david     (1000)     2485 2021-11-28 12:52:01.000000 mobile_env_rl-3.6/android_env/components/log_stream_test.py
+-rw-r--r--   0 david     (1000) david     (1000)     7591 2023-03-10 15:36:10.000000 mobile_env_rl-3.6/android_env/components/logcat_thread.py
+-rw-r--r--   0 david     (1000) david     (1000)     4370 2021-11-28 12:52:01.000000 mobile_env_rl-3.6/android_env/components/logcat_thread_test.py
+-rw-r--r--   0 david     (1000) david     (1000)    15562 2023-12-18 11:31:48.000000 mobile_env_rl-3.6/android_env/components/screen_analyzer_thread.py
+-rw-r--r--   0 david     (1000) david     (1000)    12877 2024-04-01 09:14:35.000000 mobile_env_rl-3.6/android_env/components/setup_step_interpreter.py
+-rw-r--r--   0 david     (1000) david     (1000)    14297 2021-11-28 12:52:01.000000 mobile_env_rl-3.6/android_env/components/setup_step_interpreter_test.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-04-30 07:05:48.792838 mobile_env_rl-3.6/android_env/components/simulators/
+-rw-r--r--   0 david     (1000) david     (1000)     1009 2023-12-18 11:31:48.000000 mobile_env_rl-3.6/android_env/components/simulators/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)     8705 2023-12-18 11:31:48.000000 mobile_env_rl-3.6/android_env/components/simulators/base_simulator.py
+-rw-r--r--   0 david     (1000) david     (1000)     5734 2021-11-28 12:52:01.000000 mobile_env_rl-3.6/android_env/components/simulators/base_simulator_test.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-04-30 07:05:48.792838 mobile_env_rl-3.6/android_env/components/simulators/emulator/
+-rw-r--r--   0 david     (1000) david     (1000)      610 2021-11-28 12:52:01.000000 mobile_env_rl-3.6/android_env/components/simulators/emulator/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)     9766 2023-09-21 03:02:32.000000 mobile_env_rl-3.6/android_env/components/simulators/emulator/emulator_launcher.py
+-rw-r--r--   0 david     (1000) david     (1000)     5734 2021-11-28 12:52:01.000000 mobile_env_rl-3.6/android_env/components/simulators/emulator/emulator_launcher_test.py
+-rw-r--r--   0 david     (1000) david     (1000)     8274 2023-12-18 11:31:48.000000 mobile_env_rl-3.6/android_env/components/simulators/emulator/emulator_simulator.py
+-rw-r--r--   0 david     (1000) david     (1000)     9058 2021-11-28 12:52:01.000000 mobile_env_rl-3.6/android_env/components/simulators/emulator/emulator_simulator_test.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-04-30 07:05:48.792838 mobile_env_rl-3.6/android_env/components/simulators/fake/
+-rw-r--r--   0 david     (1000) david     (1000)      610 2021-11-28 12:52:01.000000 mobile_env_rl-3.6/android_env/components/simulators/fake/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)     5030 2021-11-28 12:52:01.000000 mobile_env_rl-3.6/android_env/components/simulators/fake/fake_simulator.py
+-rw-r--r--   0 david     (1000) david     (1000)     2586 2021-11-28 12:52:01.000000 mobile_env_rl-3.6/android_env/components/simulators/fake/fake_simulator_test.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-04-30 07:05:48.792838 mobile_env_rl-3.6/android_env/components/simulators/remote/
+-rw-r--r--   0 david     (1000) david     (1000)      621 2023-12-18 11:31:48.000000 mobile_env_rl-3.6/android_env/components/simulators/remote/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)    10564 2023-12-18 11:31:48.000000 mobile_env_rl-3.6/android_env/components/simulators/remote/daemon.py
+-rw-r--r--   0 david     (1000) david     (1000)     4230 2023-12-18 11:31:48.000000 mobile_env_rl-3.6/android_env/components/simulators/remote/remote_adb_controller.py
+-rw-r--r--   0 david     (1000) david     (1000)     2407 2023-12-18 11:31:48.000000 mobile_env_rl-3.6/android_env/components/simulators/remote/remote_base.py
+-rw-r--r--   0 david     (1000) david     (1000)     2498 2023-12-18 11:31:48.000000 mobile_env_rl-3.6/android_env/components/simulators/remote/remote_log_stream.py
+-rw-r--r--   0 david     (1000) david     (1000)    10652 2023-12-18 11:31:48.000000 mobile_env_rl-3.6/android_env/components/simulators/remote/remote_simulator.py
+-rw-r--r--   0 david     (1000) david     (1000)     6722 2023-12-18 11:31:48.000000 mobile_env_rl-3.6/android_env/components/specs.py
+-rw-r--r--   0 david     (1000) david     (1000)     5002 2021-11-28 12:52:01.000000 mobile_env_rl-3.6/android_env/components/specs_test.py
+-rw-r--r--   0 david     (1000) david     (1000)    46873 2023-12-18 11:31:48.000000 mobile_env_rl-3.6/android_env/components/task_manager.py
+-rw-r--r--   0 david     (1000) david     (1000)    12689 2021-11-28 12:52:01.000000 mobile_env_rl-3.6/android_env/components/task_manager_test.py
+-rw-r--r--   0 david     (1000) david     (1000)     3815 2021-11-28 12:52:01.000000 mobile_env_rl-3.6/android_env/components/thread_function.py
+-rw-r--r--   0 david     (1000) david     (1000)     2153 2021-11-28 12:52:01.000000 mobile_env_rl-3.6/android_env/components/thread_function_test.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-04-30 07:05:48.792838 mobile_env_rl-3.6/android_env/components/tools/
+-rw-r--r--   0 david     (1000) david     (1000)      628 2023-03-10 15:36:10.000000 mobile_env_rl-3.6/android_env/components/tools/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)     8066 2023-12-18 11:31:48.000000 mobile_env_rl-3.6/android_env/components/tools/easyocr_wrapper.py
+-rw-r--r--   0 david     (1000) david     (1000)     3635 2023-03-10 15:36:10.000000 mobile_env_rl-3.6/android_env/components/tools/naive_functions.py
+-rw-r--r--   0 david     (1000) david     (1000)     1046 2023-12-18 11:31:48.000000 mobile_env_rl-3.6/android_env/components/tools/sbert_holder.py
+-rw-r--r--   0 david     (1000) david     (1000)     3579 2023-03-10 15:36:10.000000 mobile_env_rl-3.6/android_env/components/tools/types.py
+-rw-r--r--   0 david     (1000) david     (1000)     1831 2021-11-28 12:52:01.000000 mobile_env_rl-3.6/android_env/components/utils.py
+-rw-r--r--   0 david     (1000) david     (1000)     2787 2021-11-28 12:52:01.000000 mobile_env_rl-3.6/android_env/components/utils_test.py
+-rw-r--r--   0 david     (1000) david     (1000)     5239 2023-12-18 11:31:48.000000 mobile_env_rl-3.6/android_env/components/vh_analyzer_thread.py
+-rw-r--r--   0 david     (1000) david     (1000)     8531 2024-04-01 09:14:35.000000 mobile_env_rl-3.6/android_env/environment.py
+-rw-r--r--   0 david     (1000) david     (1000)     6499 2021-11-28 12:52:01.000000 mobile_env_rl-3.6/android_env/environment_test.py
+-rw-r--r--   0 david     (1000) david     (1000)    17035 2024-03-11 07:40:42.000000 mobile_env_rl-3.6/android_env/loader.py
+-rw-r--r--   0 david     (1000) david     (1000)     3591 2021-11-28 12:52:01.000000 mobile_env_rl-3.6/android_env/loader_test.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-04-30 07:05:48.866169 mobile_env_rl-3.6/android_env/proto/
+-rw-r--r--   0 david     (1000) david     (1000)      610 2021-11-28 12:52:01.000000 mobile_env_rl-3.6/android_env/proto/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)     4608 2024-04-01 09:14:35.000000 mobile_env_rl-3.6/android_env/proto/adb.proto
+-rw-r--r--   0 david     (1000) david     (1000)     6962 2024-03-22 12:00:38.000000 mobile_env_rl-3.6/android_env/proto/adb_pb2.py
+-rw-r--r--   0 david     (1000) david     (1000)      159 2024-03-22 12:00:38.000000 mobile_env_rl-3.6/android_env/proto/adb_pb2_grpc.py
+-rw-r--r--   0 david     (1000) david     (1000)    41044 2021-11-28 12:52:01.000000 mobile_env_rl-3.6/android_env/proto/emulator_controller.proto
+-rw-r--r--   0 david     (1000) david     (1000)    23761 2024-03-22 12:00:38.000000 mobile_env_rl-3.6/android_env/proto/emulator_controller_pb2.py
+-rw-r--r--   0 david     (1000) david     (1000)    67018 2024-03-22 12:00:38.000000 mobile_env_rl-3.6/android_env/proto/emulator_controller_pb2_grpc.py
+-rw-r--r--   0 david     (1000) david     (1000)     1327 2021-11-28 12:52:01.000000 mobile_env_rl-3.6/android_env/proto/raw_observation.proto
+-rw-r--r--   0 david     (1000) david     (1000)     1505 2024-03-22 12:00:38.000000 mobile_env_rl-3.6/android_env/proto/raw_observation_pb2.py
+-rw-r--r--   0 david     (1000) david     (1000)      159 2024-03-22 12:00:38.000000 mobile_env_rl-3.6/android_env/proto/raw_observation_pb2_grpc.py
+-rw-r--r--   0 david     (1000) david     (1000)    11922 2023-12-18 11:31:48.000000 mobile_env_rl-3.6/android_env/proto/task.proto
+-rw-r--r--   0 david     (1000) david     (1000)    10451 2024-03-22 12:00:38.000000 mobile_env_rl-3.6/android_env/proto/task_pb2.py
+-rw-r--r--   0 david     (1000) david     (1000)      159 2024-03-22 12:00:38.000000 mobile_env_rl-3.6/android_env/proto/task_pb2_grpc.py
+-rw-r--r--   0 david     (1000) david     (1000)     2670 2024-03-11 07:40:42.000000 mobile_env_rl-3.6/android_env/utils.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-04-30 07:05:48.869502 mobile_env_rl-3.6/android_env/wrappers/
+-rw-r--r--   0 david     (1000) david     (1000)     2285 2023-12-18 11:31:48.000000 mobile_env_rl-3.6/android_env/wrappers/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)     3112 2023-12-18 11:31:48.000000 mobile_env_rl-3.6/android_env/wrappers/base_wrapper.py
+-rw-r--r--   0 david     (1000) david     (1000)     9011 2023-03-10 15:36:10.000000 mobile_env_rl-3.6/android_env/wrappers/discrete_action_wrapper.py
+-rw-r--r--   0 david     (1000) david     (1000)     4814 2023-03-10 15:36:10.000000 mobile_env_rl-3.6/android_env/wrappers/flat_interface_wrapper.py
+-rw-r--r--   0 david     (1000) david     (1000)     3984 2023-03-10 15:36:10.000000 mobile_env_rl-3.6/android_env/wrappers/float_pixels_wrapper.py
+-rw-r--r--   0 david     (1000) david     (1000)     3914 2023-03-10 15:36:10.000000 mobile_env_rl-3.6/android_env/wrappers/gym_wrapper.py
+-rw-r--r--   0 david     (1000) david     (1000)     5178 2023-12-18 11:31:48.000000 mobile_env_rl-3.6/android_env/wrappers/image_rescale_wrapper.py
+-rw-r--r--   0 david     (1000) david     (1000)     4312 2021-11-28 12:52:01.000000 mobile_env_rl-3.6/android_env/wrappers/last_action_wrapper.py
+-rw-r--r--   0 david     (1000) david     (1000)     5821 2023-12-18 11:31:48.000000 mobile_env_rl-3.6/android_env/wrappers/recorder_wrapper.py
+-rw-r--r--   0 david     (1000) david     (1000)    13653 2023-12-18 11:31:48.000000 mobile_env_rl-3.6/android_env/wrappers/tap_action_wrapper.py
+-rw-r--r--   0 david     (1000) david     (1000)    16766 2024-04-01 09:14:35.000000 mobile_env_rl-3.6/android_env/wrappers/vh_io_wrapper.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-04-30 07:05:48.909500 mobile_env_rl-3.6/mobile_env_rl.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)    24819 2024-04-30 07:05:48.000000 mobile_env_rl-3.6/mobile_env_rl.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)     3817 2024-04-30 07:05:48.000000 mobile_env_rl-3.6/mobile_env_rl.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2024-04-30 07:05:48.000000 mobile_env_rl-3.6/mobile_env_rl.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) david     (1000)      294 2024-04-30 07:05:48.000000 mobile_env_rl-3.6/mobile_env_rl.egg-info/requires.txt
+-rw-r--r--   0 david     (1000) david     (1000)       12 2024-04-30 07:05:48.000000 mobile_env_rl-3.6/mobile_env_rl.egg-info/top_level.txt
+-rw-r--r--   0 david     (1000) david     (1000)     1123 2024-04-30 06:54:18.000000 mobile_env_rl-3.6/pyproject.toml
+-rw-r--r--   0 david     (1000) david     (1000)       38 2024-04-30 07:05:48.912834 mobile_env_rl-3.6/setup.cfg
+-rw-r--r--   0 david     (1000) david     (1000)     4708 2024-04-30 06:54:18.000000 mobile_env_rl-3.6/setup.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-04-30 07:05:48.869502 mobile_env_rl-3.6/tests/
+-rw-r--r--   0 david     (1000) david     (1000)     2984 2023-10-31 08:21:33.000000 mobile_env_rl-3.6/tests/test_css_selector.py
```

### Comparing `mobile-env-rl-3.5/LICENSE` & `mobile_env_rl-3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/PKG-INFO` & `mobile_env_rl-3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobile-env-rl
-Version: 3.5
+Version: 3.6
 Summary: A Universal Platform for Training and Evaluation of Mobile Interaction
 Home-page: https://github.com/X-LANCE/Mobile-Env
 Author: Danyang Zhang @X-Lance
 Author-email: "Danyang Zhang @X-Lance" <zdy004007@126.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
@@ -245,14 +245,22 @@
 Requires-Dist: pytest-xdist; extra == "testing"
 
 <!-- vimc: call SyntaxRange#Include('```sh', '```', 'sh', 'NonText'): -->
 <!-- vimc: call SyntaxRange#Include('```bibtex', '```', 'bib', 'NonText'): -->
 
 ## NEWS!!
 
+* (2024-04-30 v3.6)
+  * Updated function to load a remote simulator to enable providing the remote
+    resources with a different path with the path of the local task definition
+    file.
+  * Updated task template toolkit, added new slot modifiers and sytaxes for
+    task config file.
+  * Fixed known bugs.
+
 * (2023-12-18 v3.5)
   * Owing to the long time delay of VH check and screenshot check, we updated
     the mechanism of managing the check time. By this way, the requirement of
     sufficient check for the episode events and the resulted long delay can be
     balanced.
   * Added multiple rating methods to `ResponseEvent`: regex matching, fuzzy
     matching, and vector encoding matching.
@@ -263,14 +271,16 @@
     and enabled resizing the image before and after transferring to shrink the
     transferred data.
   * Merged annotation tool to the main branch. The original annotation-tool
     branch is deprecated.
   * Added support to `ResponseEvent` to annotation tool.
   * Supplemented several commandline options to annotation-tool.
 
+For more details, please see our [Change Log](Changelog) and Documents.
+
 * (2023-10-31 v3.0) Migrated VH node specification from the original VH path to
   Mobile-Env-customized CSS selector (me-selector) and added repeatability
   control to EventSlots. Repeatability control for EventSlots may be useful to
   prevent repetitive triggering of an `OR`-type virtual event combining
   multiple types of event sources.
 
 Please see our [Change Log](Changelog) and
@@ -381,19 +391,22 @@
 just required. Detailed instructions can be found in [Extending a New
 Environment (App) or a New Task Based on
 Mobile-Env](docs/task-definition-en.md).
 
 Several demo task definitions are provided under `demos`. Three of them are
 migrated from  AndroidEnv:
 
-* `classic_2048.m.textproto` - Classic 2048 game.
+* `classic_2048.m.textproto` - [Classic 2048
+  game](https://github.com/google-deepmind/android_env/blob/main/docs/example_tasks.md#classic-2048).
 * `accessibility_forwarder_clock_set_timer.m.textproto` - A simple task
-  requiring the agent to reset a running timer.
-* `systemui_egg_land_default.m.textproto` - Flappy Droid. An open-sourced
-  implementation of classic game, Flappy Bird.
+  requiring the agent to [reset a running
+  timer](https://github.com/google-deepmind/android_env/blob/main/docs/example_tasks.md#accessibility-forwarder).
+* `systemui_egg_land_default.m.textproto` - [Flappy
+  Droid](https://github.com/google-deepmind/android_env/blob/main/docs/example_tasks.md#flappydroid).
+  An open-sourced implementation of classic game, Flappy Bird.
 
 Another one, `openmoneybox.add_billings.textproto` is defined upon an
 open-sourced billing app,
 [OpenMoneyBox](https://f-droid.org/en/packages/com.igisw.openmoneybox/).
 Details are referred to in the task definition files.
 
 ### Miscellaneous Auxiliary Tools
@@ -452,18 +465,19 @@
 at <https://arxiv.org/abs/2305.08144>.
 
 If you find Mobile-Env useful in your research, you can cite the project using
 the following BibTeX:
 
 ```bibtex
 @article{DanyangZhang2023_MobileEnv,
-  title     = {{Mobile-Env}: An Evaluation Platform and Benchmark for Interactive Agents in LLM Era},
+  title     = {{Mobile-Env}: An Evaluation Platform and Benchmark for LLM-GUI Interaction},
   author    = {Danyang Zhang and
-               Lu Chen and
+               Hongshen Xu and
                Zihan Zhao and
+               Lu Chen and
                Ruisheng Cao and
                Kai Yu},
   journal   = {CoRR},
   volume    = {abs/2305.08144},
   year      = {2023},
   url       = {https://arxiv.org/abs/2305.08144},
   eprinttype = {arXiv},
```

### Comparing `mobile-env-rl-3.5/README.md` & `mobile_env_rl-3.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 <!-- vimc: call SyntaxRange#Include('```sh', '```', 'sh', 'NonText'): -->
 <!-- vimc: call SyntaxRange#Include('```bibtex', '```', 'bib', 'NonText'): -->
 
 ## NEWS!!
 
+* (2024-04-30 v3.6)
+  * Updated function to load a remote simulator to enable providing the remote
+    resources with a different path with the path of the local task definition
+    file.
+  * Updated task template toolkit, added new slot modifiers and sytaxes for
+    task config file.
+  * Fixed known bugs.
+
 * (2023-12-18 v3.5)
   * Owing to the long time delay of VH check and screenshot check, we updated
     the mechanism of managing the check time. By this way, the requirement of
     sufficient check for the episode events and the resulted long delay can be
     balanced.
   * Added multiple rating methods to `ResponseEvent`: regex matching, fuzzy
     matching, and vector encoding matching.
@@ -17,14 +25,16 @@
     and enabled resizing the image before and after transferring to shrink the
     transferred data.
   * Merged annotation tool to the main branch. The original annotation-tool
     branch is deprecated.
   * Added support to `ResponseEvent` to annotation tool.
   * Supplemented several commandline options to annotation-tool.
 
+For more details, please see our [Change Log](Changelog) and Documents.
+
 * (2023-10-31 v3.0) Migrated VH node specification from the original VH path to
   Mobile-Env-customized CSS selector (me-selector) and added repeatability
   control to EventSlots. Repeatability control for EventSlots may be useful to
   prevent repetitive triggering of an `OR`-type virtual event combining
   multiple types of event sources.
 
 Please see our [Change Log](Changelog) and
@@ -135,19 +145,22 @@
 just required. Detailed instructions can be found in [Extending a New
 Environment (App) or a New Task Based on
 Mobile-Env](docs/task-definition-en.md).
 
 Several demo task definitions are provided under `demos`. Three of them are
 migrated from  AndroidEnv:
 
-* `classic_2048.m.textproto` - Classic 2048 game.
+* `classic_2048.m.textproto` - [Classic 2048
+  game](https://github.com/google-deepmind/android_env/blob/main/docs/example_tasks.md#classic-2048).
 * `accessibility_forwarder_clock_set_timer.m.textproto` - A simple task
-  requiring the agent to reset a running timer.
-* `systemui_egg_land_default.m.textproto` - Flappy Droid. An open-sourced
-  implementation of classic game, Flappy Bird.
+  requiring the agent to [reset a running
+  timer](https://github.com/google-deepmind/android_env/blob/main/docs/example_tasks.md#accessibility-forwarder).
+* `systemui_egg_land_default.m.textproto` - [Flappy
+  Droid](https://github.com/google-deepmind/android_env/blob/main/docs/example_tasks.md#flappydroid).
+  An open-sourced implementation of classic game, Flappy Bird.
 
 Another one, `openmoneybox.add_billings.textproto` is defined upon an
 open-sourced billing app,
 [OpenMoneyBox](https://f-droid.org/en/packages/com.igisw.openmoneybox/).
 Details are referred to in the task definition files.
 
 ### Miscellaneous Auxiliary Tools
@@ -206,18 +219,19 @@
 at <https://arxiv.org/abs/2305.08144>.
 
 If you find Mobile-Env useful in your research, you can cite the project using
 the following BibTeX:
 
 ```bibtex
 @article{DanyangZhang2023_MobileEnv,
-  title     = {{Mobile-Env}: An Evaluation Platform and Benchmark for Interactive Agents in LLM Era},
+  title     = {{Mobile-Env}: An Evaluation Platform and Benchmark for LLM-GUI Interaction},
   author    = {Danyang Zhang and
-               Lu Chen and
+               Hongshen Xu and
                Zihan Zhao and
+               Lu Chen and
                Ruisheng Cao and
                Kai Yu},
   journal   = {CoRR},
   volume    = {abs/2305.08144},
   year      = {2023},
   url       = {https://arxiv.org/abs/2305.08144},
   eprinttype = {arXiv},
```

### Comparing `mobile-env-rl-3.5/android_env/__init__.py` & `mobile_env_rl-3.6/android_env/__init__.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/__init__.py` & `mobile_env_rl-3.6/android_env/components/__init__.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/action_type.py` & `mobile_env_rl-3.6/android_env/components/action_type.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/adb_controller.py` & `mobile_env_rl-3.6/android_env/components/adb_controller.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/adb_controller_test.py` & `mobile_env_rl-3.6/android_env/components/adb_controller_test.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/adb_log_stream.py` & `mobile_env_rl-3.6/android_env/components/adb_log_stream.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/adb_log_stream_test.py` & `mobile_env_rl-3.6/android_env/components/adb_log_stream_test.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/app_screen_checker.py` & `mobile_env_rl-3.6/android_env/components/app_screen_checker.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/app_screen_checker_test.py` & `mobile_env_rl-3.6/android_env/components/app_screen_checker_test.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/coordinator.py` & `mobile_env_rl-3.6/android_env/components/coordinator.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/coordinator_test.py` & `mobile_env_rl-3.6/android_env/components/coordinator_test.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/dumpsys_thread.py` & `mobile_env_rl-3.6/android_env/components/dumpsys_thread.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/dumpsys_thread_test.py` & `mobile_env_rl-3.6/android_env/components/dumpsys_thread_test.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/errors.py` & `mobile_env_rl-3.6/android_env/components/errors.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/event_listeners.py` & `mobile_env_rl-3.6/android_env/components/event_listeners.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,15 +225,15 @@
         self._flag_cache = self._flag
         self._value_cache = self._value
         self._flag = False
         self._value = []
         #  }}} method `snapshot` # 
     def is_set(self) -> bool:
         return self._flag_cache
-    def get(self) -> List[W]:
+    def get(self) -> List[V]:
         #  method `get` {{{ # 
         """
         return lsit the wrapped type
         """
 
         return self._value_cache if self.is_set() else []
         #  }}} method `get` #
```

### Comparing `mobile-env-rl-3.5/android_env/components/log_stream.py` & `mobile_env_rl-3.6/android_env/components/log_stream.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/log_stream_test.py` & `mobile_env_rl-3.6/android_env/components/log_stream_test.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/logcat_thread.py` & `mobile_env_rl-3.6/android_env/components/logcat_thread.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/logcat_thread_test.py` & `mobile_env_rl-3.6/android_env/components/logcat_thread_test.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/screen_analyzer_thread.py` & `mobile_env_rl-3.6/android_env/components/screen_analyzer_thread.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/setup_step_interpreter.py` & `mobile_env_rl-3.6/android_env/components/setup_step_interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # coding=utf-8
+# vim: set tabstop=2 shiftwidth=2:
 # Copyright 2023 SJTU X-Lance Lab
 # 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 # 
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -29,15 +30,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """A component that parses and processes SetupSteps."""
 
 import copy
 import random
-import re
+#import re
 import time
 from typing import Any, Dict, Optional, Sequence
 
 from absl import logging
 from android_env.components import adb_controller as adb_control
 from android_env.components import app_screen_checker
 from android_env.components import errors
@@ -253,14 +254,20 @@
     elif call_type == 'start_screen_pinning':
       self._adb_controller.start_screen_pinning(
           adb_cmd.start_screen_pinning.full_activity)
 
     elif call_type == 'disable_animations':
       self._adb_controller.disable_animations()
 
+    elif call_type == "shell_command":
+      self._adb_controller._execute_shell_command(adb_cmd.shell_command.command)
+
+    elif call_type == "adb_command":
+      self._adb_controller._execute_normal_command(adb_cmd.adb_command.command)
+
     else:
       raise NotImplementedError('No ADB call type [%s].' % call_type)
 
   def _wait_for_app_screen(
       self, wait_for_app_screen: task_pb2.WaitForAppScreen) -> None:
     """Waits for a given `app_screen` to be the current screen."""
```

### Comparing `mobile-env-rl-3.5/android_env/components/setup_step_interpreter_test.py` & `mobile_env_rl-3.6/android_env/components/setup_step_interpreter_test.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/simulators/__init__.py` & `mobile_env_rl-3.6/android_env/components/simulators/__init__.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/simulators/base_simulator.py` & `mobile_env_rl-3.6/android_env/components/simulators/base_simulator.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/simulators/base_simulator_test.py` & `mobile_env_rl-3.6/android_env/components/simulators/base_simulator_test.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/simulators/emulator/__init__.py` & `mobile_env_rl-3.6/android_env/components/simulators/emulator/__init__.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/simulators/emulator/emulator_launcher.py` & `mobile_env_rl-3.6/android_env/components/simulators/emulator/emulator_launcher.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/simulators/emulator/emulator_launcher_test.py` & `mobile_env_rl-3.6/android_env/components/simulators/emulator/emulator_launcher_test.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/simulators/emulator/emulator_simulator.py` & `mobile_env_rl-3.6/android_env/components/simulators/emulator/emulator_simulator.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/simulators/emulator/emulator_simulator_test.py` & `mobile_env_rl-3.6/android_env/components/simulators/emulator/emulator_simulator_test.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/simulators/fake/__init__.py` & `mobile_env_rl-3.6/android_env/components/simulators/fake/__init__.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/simulators/fake/fake_simulator.py` & `mobile_env_rl-3.6/android_env/components/simulators/fake/fake_simulator.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/simulators/fake/fake_simulator_test.py` & `mobile_env_rl-3.6/android_env/components/simulators/fake/fake_simulator_test.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/simulators/remote/__init__.py` & `mobile_env_rl-3.6/android_env/components/simulators/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/simulators/remote/daemon.py` & `mobile_env_rl-3.6/android_env/components/simulators/remote/daemon.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/simulators/remote/remote_adb_controller.py` & `mobile_env_rl-3.6/android_env/components/simulators/remote/remote_adb_controller.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/simulators/remote/remote_base.py` & `mobile_env_rl-3.6/android_env/components/simulators/remote/remote_base.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/simulators/remote/remote_log_stream.py` & `mobile_env_rl-3.6/android_env/components/simulators/remote/remote_log_stream.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/simulators/remote/remote_simulator.py` & `mobile_env_rl-3.6/android_env/components/simulators/remote/remote_simulator.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/specs.py` & `mobile_env_rl-3.6/android_env/components/specs.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/specs_test.py` & `mobile_env_rl-3.6/android_env/components/specs_test.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/task_manager.py` & `mobile_env_rl-3.6/android_env/components/task_manager.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/task_manager_test.py` & `mobile_env_rl-3.6/android_env/components/task_manager_test.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/thread_function.py` & `mobile_env_rl-3.6/android_env/components/thread_function.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/thread_function_test.py` & `mobile_env_rl-3.6/android_env/components/thread_function_test.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/tools/__init__.py` & `mobile_env_rl-3.6/android_env/components/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/tools/easyocr_wrapper.py` & `mobile_env_rl-3.6/android_env/components/tools/easyocr_wrapper.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/tools/naive_functions.py` & `mobile_env_rl-3.6/android_env/components/tools/naive_functions.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/tools/sbert_holder.py` & `mobile_env_rl-3.6/android_env/components/tools/sbert_holder.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/tools/types.py` & `mobile_env_rl-3.6/android_env/components/tools/types.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/utils.py` & `mobile_env_rl-3.6/android_env/components/utils.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/utils_test.py` & `mobile_env_rl-3.6/android_env/components/utils_test.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/components/vh_analyzer_thread.py` & `mobile_env_rl-3.6/android_env/components/vh_analyzer_thread.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/environment.py` & `mobile_env_rl-3.6/android_env/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Android environment implementation."""
 
-from typing import Any, Dict, List, Union
+from typing import Any, Union, Optional
+from typing import Dict, List
 from absl import logging
 from android_env.components import coordinator as coordinator_lib
 from android_env.components import task_manager as task_manager_lib
 from android_env.utils import fix_path
 from android_env.proto import task_pb2
 from google.protobuf import text_format
 import os.path
@@ -108,21 +109,21 @@
   @property
   def raw_observation(self):
     return self._latest_observation
 
   def android_logs(self) -> Dict[str, Any]:
     return self._coordinator.get_logs()
 
-  def add_task(self, task_path: str, **kwargs: Dict[str, Any]):
+  def add_task(self, task_path: str, remote_path: Optional[str] = None, **kwargs: Dict[str, Any]):
     #  method `add_task` {{{ # 
     task = task_pb2.Task()
     with open(task_path, 'r') as f:
       text_format.Parse(f.read(), task)
 
-    fix_path(task, os.path.dirname(task_path))
+    fix_path(task, os.path.dirname(task_path), remote_path)
     #for st in task.setup_steps:
       #if st.HasField("adb_call") and\
           #st.adb_call.HasField("install_apk"):
         #apk_path = st.adb_call.install_apk.filesystem.path
         #if not os.path.isabs(apk_path):
           #st.adb_call.install_apk.filesystem.path =\
               #os.path.normpath(
```

### Comparing `mobile-env-rl-3.5/android_env/environment_test.py` & `mobile_env_rl-3.6/android_env/environment_test.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/loader.py` & `mobile_env_rl-3.6/android_env/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,14 +252,15 @@
                , special_token_pattern: str = r"\[\w+\]"
                , unify_vocabulary: Optional[str] = None
                , text_model: TextModel = naive_functions
                , icon_model: IconModel = naive_functions
                , sbert_holder: Optional[SBERTHolder] = None
                , with_view_hierarchy: bool = False
                , coordinator_args: Optional[Dict[str, Any]] = None
+               , remote_path: Optional[str] = None
                ) -> environment.AndroidEnv:
   """Loads an AndroidEnv instance.
 
   Args:
     task_path (str): Path to the task textproto file or the directory of task
       textproto file set
 
@@ -312,14 +313,17 @@
 
     with_view_hierarchy (bool): if the view hierarchy should be included in the
       observation
 
     coordinator_args (Optional[Dict[str, Any]]): overrides several default
       arguments of Coordinator
 
+    remote_path (Optional[str]): set a different folder path for resources on
+      remote machine
+
   Returns:
     env: An AndroidEnv instance.
   """
 
   coordinator_args: Dict[str, Any] = coordinator_args or {}
 
   # Prepare task.
@@ -353,15 +357,15 @@
           st.adb_call.install_apk.filesystem.path =\
               "{:}-{:}{:}".format(main_name,
                 mitm_config.get("patch-suffix", "patched"),
                 extension)
 
   # transform the paths in task definitions
   for t in task_list:
-    fix_path(t, task_directory)
+    fix_path(t, task_directory, remote_path)
 
   # Create simulator.
   simulator = remote_simulator.RemoteSimulator( address=address
                                               , port=port
                                               , timeout=timeout
                                               , launch_timeout=launch_timeout
                                               , retry=retry
```

### Comparing `mobile-env-rl-3.5/android_env/loader_test.py` & `mobile_env_rl-3.6/android_env/loader_test.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/proto/__init__.py` & `mobile_env_rl-3.6/android_env/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/proto/adb_pb2.py` & `mobile_env_rl-3.6/android_env/proto/adb_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,66 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: android_env/proto/adb.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x61ndroid_env/proto/adb.proto\x12\x0b\x61ndroid_env\"\x85\x10\n\x07\x41\x64\x62\x43\x61ll\x12\x36\n\x0binstall_apk\x18\x01 \x01(\x0b\x32\x1f.android_env.AdbCall.InstallApkH\x00\x12<\n\x0estart_activity\x18\x02 \x01(\x0b\x32\".android_env.AdbCall.StartActivityH\x00\x12\x34\n\nforce_stop\x18\x03 \x01(\x0b\x32\x1e.android_env.AdbCall.ForceStopH\x00\x12\x36\n\x0b\x63lear_cache\x18\x04 \x01(\x0b\x32\x1f.android_env.AdbCall.ClearCacheH\x00\x12\x42\n\x11grant_permissions\x18\x05 \x01(\x0b\x32%.android_env.AdbCall.GrantPermissionsH\x00\x12\'\n\x03tap\x18\x06 \x01(\x0b\x32\x18.android_env.AdbCall.TapH\x00\x12\x38\n\x0cpress_button\x18\x07 \x01(\x0b\x32 .android_env.AdbCall.PressButtonH\x00\x12-\n\x06rotate\x18\x08 \x01(\x0b\x32\x1b.android_env.AdbCall.RotateH\x00\x12U\n\x1bstart_accessibility_service\x18\t \x01(\x0b\x32..android_env.AdbCall.StartAccessibilityServiceH\x00\x12G\n\x14start_screen_pinning\x18\n \x01(\x0b\x32\'.android_env.AdbCall.StartScreenPinningH\x00\x12I\n\x15start_random_activity\x18\x0b \x01(\x0b\x32(.android_env.AdbCall.StartRandomActivityH\x00\x12R\n\x1a\x66orce_stop_random_activity\x18\x0c \x01(\x0b\x32,.android_env.AdbCall.ForceStopRandomActivityH\x00\x12T\n\x1b\x63lear_cache_random_activity\x18\r \x01(\x0b\x32-.android_env.AdbCall.ClearCacheRandomActivityH\x00\x12\x44\n\x12\x64isable_animations\x18\x0e \x01(\x0b\x32&.android_env.AdbCall.DisableAnimationsH\x00\x12\x38\n\x0cstart_intent\x18\x0f \x01(\x0b\x32 .android_env.AdbCall.StartIntentH\x00\x12\x42\n\x11uninstall_package\x18\x10 \x01(\x0b\x32%.android_env.AdbCall.UninstallPackageH\x00\x1av\n\nInstallApk\x12@\n\nfilesystem\x18\x02 \x01(\x0b\x32*.android_env.AdbCall.InstallApk.FilesystemH\x00\x1a\x1a\n\nFilesystem\x12\x0c\n\x04path\x18\x01 \x01(\tB\n\n\x08location\x1aH\n\rStartActivity\x12\x15\n\rfull_activity\x18\x01 \x01(\t\x12\x12\n\nextra_args\x18\x02 \x03(\t\x12\x0c\n\x04\x66lag\x18\x03 \x01(\t\x1a\x45\n\x0bStartIntent\x12\x10\n\x08\x64\x61ta_uri\x18\x01 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x02 \x01(\t\x12\x14\n\x0cpackage_name\x18\x03 \x01(\t\x1aU\n\x13StartRandomActivity\x12\x15\n\ractivity_list\x18\x01 \x03(\t\x12\x12\n\nextra_args\x18\x02 \x03(\t\x12\x13\n\x0btimeout_sec\x18\x04 \x01(\x02\x1a(\n\x10UninstallPackage\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x1a!\n\tForceStop\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x1a\x19\n\x17\x46orceStopRandomActivity\x1a\x13\n\x11\x44isableAnimations\x1a\"\n\nClearCache\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x1a\x1a\n\x18\x43learCacheRandomActivity\x1a=\n\x10GrantPermissions\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x13\n\x0bpermissions\x18\x02 \x03(\t\x1a\x1b\n\x03Tap\x12\t\n\x01x\x18\x01 \x01(\x05\x12\t\n\x01y\x18\x02 \x01(\x05\x1a\x64\n\x0bPressButton\x12\x37\n\x06\x62utton\x18\x01 \x01(\x0e\x32\'.android_env.AdbCall.PressButton.Button\"\x1c\n\x06\x42utton\x12\x08\n\x04HOME\x10\x00\x12\x08\n\x04\x42\x41\x43K\x10\x01\x1a\x9c\x01\n\x06Rotate\x12<\n\x0borientation\x18\x01 \x01(\x0e\x32\'.android_env.AdbCall.Rotate.Orientation\"T\n\x0bOrientation\x12\x0e\n\nPORTRAIT_0\x10\x00\x12\x10\n\x0cLANDSCAPE_90\x10\x01\x12\x10\n\x0cPORTRAIT_180\x10\x02\x12\x11\n\rLANDSCAPE_270\x10\x03\x1a\x31\n\x19StartAccessibilityService\x12\x14\n\x0c\x66ull_service\x18\x01 \x01(\t\x1a+\n\x12StartScreenPinning\x12\x15\n\rfull_activity\x18\x01 \x01(\tB\t\n\x07\x63ommandb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x61ndroid_env/proto/adb.proto\x12\x0b\x61ndroid_env\"\x8d\x11\n\x07\x41\x64\x62\x43\x61ll\x12\x36\n\x0binstall_apk\x18\x01 \x01(\x0b\x32\x1f.android_env.AdbCall.InstallApkH\x00\x12<\n\x0estart_activity\x18\x02 \x01(\x0b\x32\".android_env.AdbCall.StartActivityH\x00\x12\x34\n\nforce_stop\x18\x03 \x01(\x0b\x32\x1e.android_env.AdbCall.ForceStopH\x00\x12\x36\n\x0b\x63lear_cache\x18\x04 \x01(\x0b\x32\x1f.android_env.AdbCall.ClearCacheH\x00\x12\x42\n\x11grant_permissions\x18\x05 \x01(\x0b\x32%.android_env.AdbCall.GrantPermissionsH\x00\x12\'\n\x03tap\x18\x06 \x01(\x0b\x32\x18.android_env.AdbCall.TapH\x00\x12\x38\n\x0cpress_button\x18\x07 \x01(\x0b\x32 .android_env.AdbCall.PressButtonH\x00\x12-\n\x06rotate\x18\x08 \x01(\x0b\x32\x1b.android_env.AdbCall.RotateH\x00\x12U\n\x1bstart_accessibility_service\x18\t \x01(\x0b\x32..android_env.AdbCall.StartAccessibilityServiceH\x00\x12G\n\x14start_screen_pinning\x18\n \x01(\x0b\x32\'.android_env.AdbCall.StartScreenPinningH\x00\x12I\n\x15start_random_activity\x18\x0b \x01(\x0b\x32(.android_env.AdbCall.StartRandomActivityH\x00\x12R\n\x1a\x66orce_stop_random_activity\x18\x0c \x01(\x0b\x32,.android_env.AdbCall.ForceStopRandomActivityH\x00\x12T\n\x1b\x63lear_cache_random_activity\x18\r \x01(\x0b\x32-.android_env.AdbCall.ClearCacheRandomActivityH\x00\x12\x44\n\x12\x64isable_animations\x18\x0e \x01(\x0b\x32&.android_env.AdbCall.DisableAnimationsH\x00\x12\x38\n\x0cstart_intent\x18\x0f \x01(\x0b\x32 .android_env.AdbCall.StartIntentH\x00\x12\x42\n\x11uninstall_package\x18\x10 \x01(\x0b\x32%.android_env.AdbCall.UninstallPackageH\x00\x12\x35\n\rshell_command\x18\x11 \x01(\x0b\x32\x1c.android_env.AdbCall.CommandH\x00\x12\x33\n\x0b\x61\x64\x62_command\x18\x12 \x01(\x0b\x32\x1c.android_env.AdbCall.CommandH\x00\x1av\n\nInstallApk\x12@\n\nfilesystem\x18\x02 \x01(\x0b\x32*.android_env.AdbCall.InstallApk.FilesystemH\x00\x1a\x1a\n\nFilesystem\x12\x0c\n\x04path\x18\x01 \x01(\tB\n\n\x08location\x1aH\n\rStartActivity\x12\x15\n\rfull_activity\x18\x01 \x01(\t\x12\x12\n\nextra_args\x18\x02 \x03(\t\x12\x0c\n\x04\x66lag\x18\x03 \x01(\t\x1a\x45\n\x0bStartIntent\x12\x10\n\x08\x64\x61ta_uri\x18\x01 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x02 \x01(\t\x12\x14\n\x0cpackage_name\x18\x03 \x01(\t\x1aU\n\x13StartRandomActivity\x12\x15\n\ractivity_list\x18\x01 \x03(\t\x12\x12\n\nextra_args\x18\x02 \x03(\t\x12\x13\n\x0btimeout_sec\x18\x04 \x01(\x02\x1a(\n\x10UninstallPackage\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x1a!\n\tForceStop\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x1a\x19\n\x17\x46orceStopRandomActivity\x1a\x13\n\x11\x44isableAnimations\x1a\"\n\nClearCache\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x1a\x1a\n\x18\x43learCacheRandomActivity\x1a=\n\x10GrantPermissions\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x13\n\x0bpermissions\x18\x02 \x03(\t\x1a\x1b\n\x03Tap\x12\t\n\x01x\x18\x01 \x01(\x05\x12\t\n\x01y\x18\x02 \x01(\x05\x1a\x64\n\x0bPressButton\x12\x37\n\x06\x62utton\x18\x01 \x01(\x0e\x32\'.android_env.AdbCall.PressButton.Button\"\x1c\n\x06\x42utton\x12\x08\n\x04HOME\x10\x00\x12\x08\n\x04\x42\x41\x43K\x10\x01\x1a\x9c\x01\n\x06Rotate\x12<\n\x0borientation\x18\x01 \x01(\x0e\x32\'.android_env.AdbCall.Rotate.Orientation\"T\n\x0bOrientation\x12\x0e\n\nPORTRAIT_0\x10\x00\x12\x10\n\x0cLANDSCAPE_90\x10\x01\x12\x10\n\x0cPORTRAIT_180\x10\x02\x12\x11\n\rLANDSCAPE_270\x10\x03\x1a\x31\n\x19StartAccessibilityService\x12\x14\n\x0c\x66ull_service\x18\x01 \x01(\t\x1a+\n\x12StartScreenPinning\x12\x15\n\rfull_activity\x18\x01 \x01(\t\x1a\x1a\n\x07\x43ommand\x12\x0f\n\x07\x63ommand\x18\x01 \x03(\tB\t\n\x07\x63ommandb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'android_env.proto.adb_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   _globals['_ADBCALL']._serialized_start=45
-  _globals['_ADBCALL']._serialized_end=2098
-  _globals['_ADBCALL_INSTALLAPK']._serialized_start=1099
-  _globals['_ADBCALL_INSTALLAPK']._serialized_end=1217
-  _globals['_ADBCALL_INSTALLAPK_FILESYSTEM']._serialized_start=1179
-  _globals['_ADBCALL_INSTALLAPK_FILESYSTEM']._serialized_end=1205
-  _globals['_ADBCALL_STARTACTIVITY']._serialized_start=1219
-  _globals['_ADBCALL_STARTACTIVITY']._serialized_end=1291
-  _globals['_ADBCALL_STARTINTENT']._serialized_start=1293
-  _globals['_ADBCALL_STARTINTENT']._serialized_end=1362
-  _globals['_ADBCALL_STARTRANDOMACTIVITY']._serialized_start=1364
-  _globals['_ADBCALL_STARTRANDOMACTIVITY']._serialized_end=1449
-  _globals['_ADBCALL_UNINSTALLPACKAGE']._serialized_start=1451
-  _globals['_ADBCALL_UNINSTALLPACKAGE']._serialized_end=1491
-  _globals['_ADBCALL_FORCESTOP']._serialized_start=1493
-  _globals['_ADBCALL_FORCESTOP']._serialized_end=1526
-  _globals['_ADBCALL_FORCESTOPRANDOMACTIVITY']._serialized_start=1528
-  _globals['_ADBCALL_FORCESTOPRANDOMACTIVITY']._serialized_end=1553
-  _globals['_ADBCALL_DISABLEANIMATIONS']._serialized_start=1555
-  _globals['_ADBCALL_DISABLEANIMATIONS']._serialized_end=1574
-  _globals['_ADBCALL_CLEARCACHE']._serialized_start=1576
-  _globals['_ADBCALL_CLEARCACHE']._serialized_end=1610
-  _globals['_ADBCALL_CLEARCACHERANDOMACTIVITY']._serialized_start=1612
-  _globals['_ADBCALL_CLEARCACHERANDOMACTIVITY']._serialized_end=1638
-  _globals['_ADBCALL_GRANTPERMISSIONS']._serialized_start=1640
-  _globals['_ADBCALL_GRANTPERMISSIONS']._serialized_end=1701
-  _globals['_ADBCALL_TAP']._serialized_start=1703
-  _globals['_ADBCALL_TAP']._serialized_end=1730
-  _globals['_ADBCALL_PRESSBUTTON']._serialized_start=1732
-  _globals['_ADBCALL_PRESSBUTTON']._serialized_end=1832
-  _globals['_ADBCALL_PRESSBUTTON_BUTTON']._serialized_start=1804
-  _globals['_ADBCALL_PRESSBUTTON_BUTTON']._serialized_end=1832
-  _globals['_ADBCALL_ROTATE']._serialized_start=1835
-  _globals['_ADBCALL_ROTATE']._serialized_end=1991
-  _globals['_ADBCALL_ROTATE_ORIENTATION']._serialized_start=1907
-  _globals['_ADBCALL_ROTATE_ORIENTATION']._serialized_end=1991
-  _globals['_ADBCALL_STARTACCESSIBILITYSERVICE']._serialized_start=1993
-  _globals['_ADBCALL_STARTACCESSIBILITYSERVICE']._serialized_end=2042
-  _globals['_ADBCALL_STARTSCREENPINNING']._serialized_start=2044
-  _globals['_ADBCALL_STARTSCREENPINNING']._serialized_end=2087
+  _globals['_ADBCALL']._serialized_end=2234
+  _globals['_ADBCALL_INSTALLAPK']._serialized_start=1207
+  _globals['_ADBCALL_INSTALLAPK']._serialized_end=1325
+  _globals['_ADBCALL_INSTALLAPK_FILESYSTEM']._serialized_start=1287
+  _globals['_ADBCALL_INSTALLAPK_FILESYSTEM']._serialized_end=1313
+  _globals['_ADBCALL_STARTACTIVITY']._serialized_start=1327
+  _globals['_ADBCALL_STARTACTIVITY']._serialized_end=1399
+  _globals['_ADBCALL_STARTINTENT']._serialized_start=1401
+  _globals['_ADBCALL_STARTINTENT']._serialized_end=1470
+  _globals['_ADBCALL_STARTRANDOMACTIVITY']._serialized_start=1472
+  _globals['_ADBCALL_STARTRANDOMACTIVITY']._serialized_end=1557
+  _globals['_ADBCALL_UNINSTALLPACKAGE']._serialized_start=1559
+  _globals['_ADBCALL_UNINSTALLPACKAGE']._serialized_end=1599
+  _globals['_ADBCALL_FORCESTOP']._serialized_start=1601
+  _globals['_ADBCALL_FORCESTOP']._serialized_end=1634
+  _globals['_ADBCALL_FORCESTOPRANDOMACTIVITY']._serialized_start=1636
+  _globals['_ADBCALL_FORCESTOPRANDOMACTIVITY']._serialized_end=1661
+  _globals['_ADBCALL_DISABLEANIMATIONS']._serialized_start=1663
+  _globals['_ADBCALL_DISABLEANIMATIONS']._serialized_end=1682
+  _globals['_ADBCALL_CLEARCACHE']._serialized_start=1684
+  _globals['_ADBCALL_CLEARCACHE']._serialized_end=1718
+  _globals['_ADBCALL_CLEARCACHERANDOMACTIVITY']._serialized_start=1720
+  _globals['_ADBCALL_CLEARCACHERANDOMACTIVITY']._serialized_end=1746
+  _globals['_ADBCALL_GRANTPERMISSIONS']._serialized_start=1748
+  _globals['_ADBCALL_GRANTPERMISSIONS']._serialized_end=1809
+  _globals['_ADBCALL_TAP']._serialized_start=1811
+  _globals['_ADBCALL_TAP']._serialized_end=1838
+  _globals['_ADBCALL_PRESSBUTTON']._serialized_start=1840
+  _globals['_ADBCALL_PRESSBUTTON']._serialized_end=1940
+  _globals['_ADBCALL_PRESSBUTTON_BUTTON']._serialized_start=1912
+  _globals['_ADBCALL_PRESSBUTTON_BUTTON']._serialized_end=1940
+  _globals['_ADBCALL_ROTATE']._serialized_start=1943
+  _globals['_ADBCALL_ROTATE']._serialized_end=2099
+  _globals['_ADBCALL_ROTATE_ORIENTATION']._serialized_start=2015
+  _globals['_ADBCALL_ROTATE_ORIENTATION']._serialized_end=2099
+  _globals['_ADBCALL_STARTACCESSIBILITYSERVICE']._serialized_start=2101
+  _globals['_ADBCALL_STARTACCESSIBILITYSERVICE']._serialized_end=2150
+  _globals['_ADBCALL_STARTSCREENPINNING']._serialized_start=2152
+  _globals['_ADBCALL_STARTSCREENPINNING']._serialized_end=2195
+  _globals['_ADBCALL_COMMAND']._serialized_start=2197
+  _globals['_ADBCALL_COMMAND']._serialized_end=2223
 # @@protoc_insertion_point(module_scope)
```

### Comparing `mobile-env-rl-3.5/android_env/proto/emulator_controller.proto` & `mobile_env_rl-3.6/android_env/proto/emulator_controller.proto`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/proto/emulator_controller_pb2.py` & `mobile_env_rl-3.6/android_env/proto/emulator_controller_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: android_env/proto/emulator_controller.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -16,22 +17,22 @@
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+android_env/proto/emulator_controller.proto\x12\x19\x61ndroid.emulation.control\x1a\x1bgoogle/protobuf/empty.proto\"\xd7\x01\n\nVmRunState\x12=\n\x05state\x18\x01 \x01(\x0e\x32..android.emulation.control.VmRunState.RunState\"\x89\x01\n\x08RunState\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07RUNNING\x10\x01\x12\x0e\n\nRESTORE_VM\x10\x02\x12\n\n\x06PAUSED\x10\x03\x12\x0b\n\x07SAVE_VM\x10\x04\x12\x0c\n\x08SHUTDOWN\x10\x05\x12\r\n\tTERMINATE\x10\x07\x12\t\n\x05RESET\x10\t\x12\x12\n\x0eINTERNAL_ERROR\x10\n\"\"\n\x0eParameterValue\x12\x10\n\x04\x64\x61ta\x18\x01 \x03(\x02\x42\x02\x10\x01\"\xc3\x04\n\x12PhysicalModelValue\x12J\n\x06target\x18\x01 \x01(\x0e\x32:.android.emulation.control.PhysicalModelValue.PhysicalType\x12\x43\n\x06status\x18\x02 \x01(\x0e\x32\x33.android.emulation.control.PhysicalModelValue.State\x12\x38\n\x05value\x18\x03 \x01(\x0b\x32).android.emulation.control.ParameterValue\"U\n\x05State\x12\x06\n\x02OK\x10\x00\x12\x17\n\nNO_SERVICE\x10\xfd\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x15\n\x08\x44ISABLED\x10\xfe\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x14\n\x07UNKNOWN\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x8a\x02\n\x0cPhysicalType\x12\x0c\n\x08POSITION\x10\x00\x12\x0c\n\x08ROTATION\x10\x01\x12\x12\n\x0eMAGNETIC_FIELD\x10\x02\x12\x0f\n\x0bTEMPERATURE\x10\x03\x12\r\n\tPROXIMITY\x10\x04\x12\t\n\x05LIGHT\x10\x05\x12\x0c\n\x08PRESSURE\x10\x06\x12\x0c\n\x08HUMIDITY\x10\x07\x12\x0c\n\x08VELOCITY\x10\x08\x12\x12\n\x0e\x41MBIENT_MOTION\x10\t\x12\x10\n\x0cHINGE_ANGLE0\x10\n\x12\x10\n\x0cHINGE_ANGLE1\x10\x0b\x12\x10\n\x0cHINGE_ANGLE2\x10\x0c\x12\r\n\tROLLABLE0\x10\r\x12\r\n\tROLLABLE1\x10\x0e\x12\r\n\tROLLABLE2\x10\x0f\"\xf8\x03\n\x0bSensorValue\x12\x41\n\x06target\x18\x01 \x01(\x0e\x32\x31.android.emulation.control.SensorValue.SensorType\x12<\n\x06status\x18\x02 \x01(\x0e\x32,.android.emulation.control.SensorValue.State\x12\x38\n\x05value\x18\x03 \x01(\x0b\x32).android.emulation.control.ParameterValue\"U\n\x05State\x12\x06\n\x02OK\x10\x00\x12\x17\n\nNO_SERVICE\x10\xfd\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x15\n\x08\x44ISABLED\x10\xfe\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x14\n\x07UNKNOWN\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xd6\x01\n\nSensorType\x12\x10\n\x0c\x41\x43\x43\x45LERATION\x10\x00\x12\r\n\tGYROSCOPE\x10\x01\x12\x12\n\x0eMAGNETIC_FIELD\x10\x02\x12\x0f\n\x0bORIENTATION\x10\x03\x12\x0f\n\x0bTEMPERATURE\x10\x04\x12\r\n\tPROXIMITY\x10\x05\x12\t\n\x05LIGHT\x10\x06\x12\x0c\n\x08PRESSURE\x10\x07\x12\x0c\n\x08HUMIDITY\x10\x08\x12\x1f\n\x1bMAGNETIC_FIELD_UNCALIBRATED\x10\t\x12\x1a\n\x16GYROSCOPE_UNCALIBRATED\x10\n\"\xd2\x01\n\nLogMessage\x12\x10\n\x08\x63ontents\x18\x01 \x01(\t\x12\r\n\x05start\x18\x02 \x01(\x03\x12\x0c\n\x04next\x18\x03 \x01(\x03\x12;\n\x04sort\x18\x04 \x01(\x0e\x32-.android.emulation.control.LogMessage.LogType\x12\x37\n\x07\x65ntries\x18\x05 \x03(\x0b\x32&.android.emulation.control.LogcatEntry\"\x1f\n\x07LogType\x12\x08\n\x04Text\x10\x00\x12\n\n\x06Parsed\x10\x01\"\x86\x02\n\x0bLogcatEntry\x12\x11\n\ttimestamp\x18\x01 \x01(\x04\x12\x0b\n\x03pid\x18\x02 \x01(\r\x12\x0b\n\x03tid\x18\x03 \x01(\r\x12>\n\x05level\x18\x04 \x01(\x0e\x32/.android.emulation.control.LogcatEntry.LogLevel\x12\x0b\n\x03tag\x18\x05 \x01(\t\x12\x0b\n\x03msg\x18\x06 \x01(\t\"p\n\x08LogLevel\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x01\x12\x0b\n\x07VERBOSE\x10\x02\x12\t\n\x05\x44\x45\x42UG\x10\x03\x12\x08\n\x04INFO\x10\x04\x12\x08\n\x04WARN\x10\x05\x12\x07\n\x03\x45RR\x10\x06\x12\t\n\x05\x46\x41TAL\x10\x07\x12\n\n\x06SILENT\x10\x08\"\xf0\x01\n\x0fVmConfiguration\x12S\n\x0ehypervisorType\x18\x01 \x01(\x0e\x32;.android.emulation.control.VmConfiguration.VmHypervisorType\x12\x18\n\x10numberOfCpuCores\x18\x02 \x01(\x05\x12\x14\n\x0cramSizeBytes\x18\x03 \x01(\x03\"X\n\x10VmHypervisorType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04NONE\x10\x01\x12\x07\n\x03KVM\x10\x02\x12\x08\n\x04HAXM\x10\x03\x12\x07\n\x03HVF\x10\x04\x12\x08\n\x04WHPX\x10\x05\x12\x07\n\x03GVM\x10\x06\"\x18\n\x08\x43lipData\x12\x0c\n\x04text\x18\x01 \x01(\t\"\xfa\x01\n\x05Touch\x12\t\n\x01x\x18\x01 \x01(\x05\x12\t\n\x01y\x18\x02 \x01(\x05\x12\x12\n\nidentifier\x18\x03 \x01(\x05\x12\x10\n\x08pressure\x18\x04 \x01(\x05\x12\x13\n\x0btouch_major\x18\x05 \x01(\x05\x12\x13\n\x0btouch_minor\x18\x06 \x01(\x05\x12\x44\n\nexpiration\x18\x07 \x01(\x0e\x32\x30.android.emulation.control.Touch.EventExpiration\"E\n\x0f\x45ventExpiration\x12 \n\x1c\x45VENT_EXPIRATION_UNSPECIFIED\x10\x00\x12\x10\n\x0cNEVER_EXPIRE\x10\x01\"P\n\nTouchEvent\x12\x31\n\x07touches\x18\x01 \x03(\x0b\x32 .android.emulation.control.Touch\x12\x0f\n\x07\x64isplay\x18\x02 \x01(\x05\"D\n\nMouseEvent\x12\t\n\x01x\x18\x01 \x01(\x05\x12\t\n\x01y\x18\x02 \x01(\x05\x12\x0f\n\x07\x62uttons\x18\x03 \x01(\x05\x12\x0f\n\x07\x64isplay\x18\x04 \x01(\x05\"\xc1\x02\n\rKeyboardEvent\x12\x46\n\x08\x63odeType\x18\x01 \x01(\x0e\x32\x34.android.emulation.control.KeyboardEvent.KeyCodeType\x12H\n\teventType\x18\x02 \x01(\x0e\x32\x35.android.emulation.control.KeyboardEvent.KeyEventType\x12\x0f\n\x07keyCode\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\x0c\n\x04text\x18\x05 \x01(\t\"<\n\x0bKeyCodeType\x12\x07\n\x03Usb\x10\x00\x12\t\n\x05\x45vdev\x10\x01\x12\x07\n\x03XKB\x10\x02\x12\x07\n\x03Win\x10\x03\x12\x07\n\x03Mac\x10\x04\"4\n\x0cKeyEventType\x12\x0b\n\x07keydown\x10\x00\x12\t\n\x05keyup\x10\x01\x12\x0c\n\x08keypress\x10\x02\"2\n\x0b\x46ingerprint\x12\x12\n\nisTouching\x18\x01 \x01(\x08\x12\x0f\n\x07touchId\x18\x02 \x01(\x05\"\x8c\x01\n\x08GpsState\x12\x15\n\rpassiveUpdate\x18\x01 \x01(\x08\x12\x10\n\x08latitude\x18\x02 \x01(\x01\x12\x11\n\tlongitude\x18\x03 \x01(\x01\x12\r\n\x05speed\x18\x04 \x01(\x01\x12\x0f\n\x07\x62\x65\x61ring\x18\x05 \x01(\x01\x12\x10\n\x08\x61ltitude\x18\x06 \x01(\x01\x12\x12\n\nsatellites\x18\x07 \x01(\x05\"\x87\x04\n\x0c\x42\x61tteryState\x12\x12\n\nhasBattery\x18\x01 \x01(\x08\x12\x11\n\tisPresent\x18\x02 \x01(\x08\x12G\n\x07\x63harger\x18\x03 \x01(\x0e\x32\x36.android.emulation.control.BatteryState.BatteryCharger\x12\x13\n\x0b\x63hargeLevel\x18\x04 \x01(\x05\x12\x45\n\x06health\x18\x05 \x01(\x0e\x32\x35.android.emulation.control.BatteryState.BatteryHealth\x12\x45\n\x06status\x18\x06 \x01(\x0e\x32\x35.android.emulation.control.BatteryState.BatteryStatus\"W\n\rBatteryStatus\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08\x43HARGING\x10\x01\x12\x0f\n\x0b\x44ISCHARGING\x10\x02\x12\x10\n\x0cNOT_CHARGING\x10\x03\x12\x08\n\x04\x46ULL\x10\x04\"9\n\x0e\x42\x61tteryCharger\x12\x08\n\x04NONE\x10\x00\x12\x06\n\x02\x41\x43\x10\x01\x12\x07\n\x03USB\x10\x02\x12\x0c\n\x08WIRELESS\x10\x03\"P\n\rBatteryHealth\x12\x08\n\x04GOOD\x10\x00\x12\n\n\x06\x46\x41ILED\x10\x01\x12\x08\n\x04\x44\x45\x41\x44\x10\x02\x12\x0f\n\x0bOVERVOLTAGE\x10\x03\x12\x0e\n\nOVERHEATED\x10\x04\"\xae\x01\n\x0eImageTransport\x12K\n\x07\x63hannel\x18\x01 \x01(\x0e\x32:.android.emulation.control.ImageTransport.TransportChannel\x12\x0e\n\x06handle\x18\x02 \x01(\t\"?\n\x10TransportChannel\x12!\n\x1dTRANSPORT_CHANNEL_UNSPECIFIED\x10\x00\x12\x08\n\x04MMAP\x10\x01\"P\n\rFoldedDisplay\x12\r\n\x05width\x18\x01 \x01(\r\x12\x0e\n\x06height\x18\x02 \x01(\r\x12\x0f\n\x07xOffset\x18\x03 \x01(\r\x12\x0f\n\x07yOffset\x18\x04 \x01(\r\"\xe5\x02\n\x0bImageFormat\x12@\n\x06\x66ormat\x18\x01 \x01(\x0e\x32\x30.android.emulation.control.ImageFormat.ImgFormat\x12\x35\n\x08rotation\x18\x02 \x01(\x0b\x32#.android.emulation.control.Rotation\x12\r\n\x05width\x18\x03 \x01(\r\x12\x0e\n\x06height\x18\x04 \x01(\r\x12\x0f\n\x07\x64isplay\x18\x05 \x01(\r\x12<\n\ttransport\x18\x06 \x01(\x0b\x32).android.emulation.control.ImageTransport\x12?\n\rfoldedDisplay\x18\x07 \x01(\x0b\x32(.android.emulation.control.FoldedDisplay\".\n\tImgFormat\x12\x07\n\x03PNG\x10\x00\x12\x0c\n\x08RGBA8888\x10\x01\x12\n\n\x06RGB888\x10\x02\"\x97\x01\n\x05Image\x12\x36\n\x06\x66ormat\x18\x01 \x01(\x0b\x32&.android.emulation.control.ImageFormat\x12\x11\n\x05width\x18\x02 \x01(\rB\x02\x18\x01\x12\x12\n\x06height\x18\x03 \x01(\rB\x02\x18\x01\x12\r\n\x05image\x18\x04 \x01(\x0c\x12\x0b\n\x03seq\x18\x05 \x01(\r\x12\x13\n\x0btimestampUs\x18\x06 \x01(\x04\"\xd5\x01\n\x08Rotation\x12\x42\n\x08rotation\x18\x01 \x01(\x0e\x32\x30.android.emulation.control.Rotation.SkinRotation\x12\r\n\x05xAxis\x18\x02 \x01(\x01\x12\r\n\x05yAxis\x18\x03 \x01(\x01\x12\r\n\x05zAxis\x18\x04 \x01(\x01\"X\n\x0cSkinRotation\x12\x0c\n\x08PORTRAIT\x10\x00\x12\r\n\tLANDSCAPE\x10\x01\x12\x14\n\x10REVERSE_PORTRAIT\x10\x02\x12\x15\n\x11REVERSE_LANDSCAPE\x10\x03\"\xf4\x01\n\tPhoneCall\x12\x41\n\toperation\x18\x01 \x01(\x0e\x32..android.emulation.control.PhoneCall.Operation\x12\x0e\n\x06number\x18\x02 \x01(\t\"\x93\x01\n\tOperation\x12\x0c\n\x08InitCall\x10\x00\x12\x0e\n\nAcceptCall\x10\x01\x12\x16\n\x12RejectCallExplicit\x10\x02\x12\x12\n\x0eRejectCallBusy\x10\x03\x12\x12\n\x0e\x44isconnectCall\x10\x04\x12\x13\n\x0fPlaceCallOnHold\x10\x05\x12\x13\n\x0fTakeCallOffHold\x10\x06\"\xbc\x01\n\rPhoneResponse\x12\x43\n\x08response\x18\x01 \x01(\x0e\x32\x31.android.emulation.control.PhoneResponse.Response\"f\n\x08Response\x12\x06\n\x02OK\x10\x00\x12\x10\n\x0c\x42\x61\x64Operation\x10\x01\x12\r\n\tBadNumber\x10\x02\x12\x11\n\rInvalidAction\x10\x03\x12\x10\n\x0c\x41\x63tionFailed\x10\x04\x12\x0c\n\x08RadioOff\x10\x05\"#\n\x05\x45ntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"<\n\tEntryList\x12/\n\x05\x65ntry\x18\x01 \x03(\x0b\x32 .android.emulation.control.Entry\"\xbd\x01\n\x0e\x45mulatorStatus\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x0e\n\x06uptime\x18\x02 \x01(\x04\x12\x0e\n\x06\x62ooted\x18\x03 \x01(\x08\x12<\n\x08vmConfig\x18\x04 \x01(\x0b\x32*.android.emulation.control.VmConfiguration\x12<\n\x0ehardwareConfig\x18\x05 \x01(\x0b\x32$.android.emulation.control.EntryList\"\xfe\x01\n\x0b\x41udioFormat\x12\x14\n\x0csamplingRate\x18\x01 \x01(\x04\x12\x41\n\x08\x63hannels\x18\x02 \x01(\x0e\x32/.android.emulation.control.AudioFormat.Channels\x12\x43\n\x06\x66ormat\x18\x03 \x01(\x0e\x32\x33.android.emulation.control.AudioFormat.SampleFormat\"/\n\x0cSampleFormat\x12\x0e\n\nAUD_FMT_U8\x10\x00\x12\x0f\n\x0b\x41UD_FMT_S16\x10\x01\" \n\x08\x43hannels\x12\x08\n\x04Mono\x10\x00\x12\n\n\x06Stereo\x10\x01\"g\n\x0b\x41udioPacket\x12\x36\n\x06\x66ormat\x18\x01 \x01(\x0b\x32&.android.emulation.control.AudioFormat\x12\x11\n\ttimestamp\x18\x02 \x01(\x04\x12\r\n\x05\x61udio\x18\x03 \x01(\x0c\".\n\nSmsMessage\x12\x12\n\nsrcAddress\x18\x01 \x01(\t\x12\x0c\n\x04text\x18\x02 \x01(\t\"\xcb\x02\n\x14\x44isplayConfiguration\x12\r\n\x05width\x18\x01 \x01(\r\x12\x0e\n\x06height\x18\x02 \x01(\r\x12\x0b\n\x03\x64pi\x18\x03 \x01(\r\x12\r\n\x05\x66lags\x18\x04 \x01(\r\x12\x0f\n\x07\x64isplay\x18\x05 \x01(\r\"\xe6\x01\n\x0c\x44isplayFlags\x12\x1c\n\x18\x44ISPLAYFLAGS_UNSPECIFIED\x10\x00\x12\x1f\n\x1bVIRTUAL_DISPLAY_FLAG_PUBLIC\x10\x01\x12%\n!VIRTUAL_DISPLAY_FLAG_PRESENTATION\x10\x02\x12\x1f\n\x1bVIRTUAL_DISPLAY_FLAG_SECURE\x10\x04\x12)\n%VIRTUAL_DISPLAY_FLAG_OWN_CONTENT_ONLY\x10\x08\x12$\n VIRTUAL_DISPLAY_FLAG_AUTO_MIRROR\x10\x10\"Z\n\x15\x44isplayConfigurations\x12\x41\n\x08\x64isplays\x18\x01 \x03(\x0b\x32/.android.emulation.control.DisplayConfiguration\"\xc8\x01\n\x0cNotification\x12@\n\x05\x65vent\x18\x01 \x01(\x0e\x32\x31.android.emulation.control.Notification.EventType\"v\n\tEventType\x12!\n\x1dVIRTUAL_SCENE_CAMERA_INACTIVE\x10\x00\x12\x1f\n\x1bVIRTUAL_SCENE_CAMERA_ACTIVE\x10\x01\x12%\n!DISPLAY_CONFIGURATIONS_CHANGED_UI\x10\x02\"1\n\x0eRotationRadian\x12\t\n\x01x\x18\x01 \x01(\x02\x12\t\n\x01y\x18\x02 \x01(\x02\x12\t\n\x01z\x18\x03 \x01(\x02\"+\n\x08Velocity\x12\t\n\x01x\x18\x01 \x01(\x02\x12\t\n\x01y\x18\x02 \x01(\x02\x12\t\n\x01z\x18\x03 \x01(\x02\"\xe8\x01\n\x07Posture\x12>\n\x05value\x18\x03 \x01(\x0e\x32/.android.emulation.control.Posture.PostureValue\"\x9c\x01\n\x0cPostureValue\x12\x13\n\x0fPOSTURE_UNKNOWN\x10\x00\x12\x12\n\x0ePOSTURE_CLOSED\x10\x01\x12\x17\n\x13POSTURE_HALF_OPENED\x10\x02\x12\x12\n\x0ePOSTURE_OPENED\x10\x03\x12\x13\n\x0fPOSTURE_FLIPPED\x10\x04\x12\x10\n\x0cPOSTURE_TENT\x10\x05\x12\x0f\n\x0bPOSTURE_MAX\x10\x06\x32\x8a\x18\n\x12\x45mulatorController\x12\x62\n\x0cstreamSensor\x12&.android.emulation.control.SensorValue\x1a&.android.emulation.control.SensorValue\"\x00\x30\x01\x12]\n\tgetSensor\x12&.android.emulation.control.SensorValue\x1a&.android.emulation.control.SensorValue\"\x00\x12M\n\tsetSensor\x12&.android.emulation.control.SensorValue\x1a\x16.google.protobuf.Empty\"\x00\x12[\n\x10setPhysicalModel\x12-.android.emulation.control.PhysicalModelValue\x1a\x16.google.protobuf.Empty\"\x00\x12r\n\x10getPhysicalModel\x12-.android.emulation.control.PhysicalModelValue\x1a-.android.emulation.control.PhysicalModelValue\"\x00\x12w\n\x13streamPhysicalModel\x12-.android.emulation.control.PhysicalModelValue\x1a-.android.emulation.control.PhysicalModelValue\"\x00\x30\x01\x12M\n\x0csetClipboard\x12#.android.emulation.control.ClipData\x1a\x16.google.protobuf.Empty\"\x00\x12M\n\x0cgetClipboard\x12\x16.google.protobuf.Empty\x1a#.android.emulation.control.ClipData\"\x00\x12R\n\x0fstreamClipboard\x12\x16.google.protobuf.Empty\x1a#.android.emulation.control.ClipData\"\x00\x30\x01\x12O\n\nsetBattery\x12\'.android.emulation.control.BatteryState\x1a\x16.google.protobuf.Empty\"\x00\x12O\n\ngetBattery\x12\x16.google.protobuf.Empty\x1a\'.android.emulation.control.BatteryState\"\x00\x12G\n\x06setGps\x12#.android.emulation.control.GpsState\x1a\x16.google.protobuf.Empty\"\x00\x12G\n\x06getGps\x12\x16.google.protobuf.Empty\x1a#.android.emulation.control.GpsState\"\x00\x12S\n\x0fsendFingerprint\x12&.android.emulation.control.Fingerprint\x1a\x16.google.protobuf.Empty\"\x00\x12M\n\x07sendKey\x12(.android.emulation.control.KeyboardEvent\x1a\x16.google.protobuf.Empty\"\x00\x12L\n\tsendTouch\x12%.android.emulation.control.TouchEvent\x1a\x16.google.protobuf.Empty\"\x00\x12L\n\tsendMouse\x12%.android.emulation.control.MouseEvent\x1a\x16.google.protobuf.Empty\"\x00\x12]\n\tsendPhone\x12$.android.emulation.control.PhoneCall\x1a(.android.emulation.control.PhoneResponse\"\x00\x12\\\n\x07sendSms\x12%.android.emulation.control.SmsMessage\x1a(.android.emulation.control.PhoneResponse\"\x00\x12P\n\tgetStatus\x12\x16.google.protobuf.Empty\x1a).android.emulation.control.EmulatorStatus\"\x00\x12[\n\rgetScreenshot\x12&.android.emulation.control.ImageFormat\x1a .android.emulation.control.Image\"\x00\x12`\n\x10streamScreenshot\x12&.android.emulation.control.ImageFormat\x1a .android.emulation.control.Image\"\x00\x30\x01\x12\x61\n\x0bstreamAudio\x12&.android.emulation.control.AudioFormat\x1a&.android.emulation.control.AudioPacket\"\x00\x30\x01\x12Q\n\x0binjectAudio\x12&.android.emulation.control.AudioPacket\x1a\x16.google.protobuf.Empty\"\x00(\x01\x12[\n\tgetLogcat\x12%.android.emulation.control.LogMessage\x1a%.android.emulation.control.LogMessage\"\x00\x12`\n\x0cstreamLogcat\x12%.android.emulation.control.LogMessage\x1a%.android.emulation.control.LogMessage\"\x00\x30\x01\x12M\n\nsetVmState\x12%.android.emulation.control.VmRunState\x1a\x16.google.protobuf.Empty\"\x00\x12M\n\ngetVmState\x12\x16.google.protobuf.Empty\x1a%.android.emulation.control.VmRunState\"\x00\x12\x80\x01\n\x18setDisplayConfigurations\x12\x30.android.emulation.control.DisplayConfigurations\x1a\x30.android.emulation.control.DisplayConfigurations\"\x00\x12\x66\n\x18getDisplayConfigurations\x12\x16.google.protobuf.Empty\x1a\x30.android.emulation.control.DisplayConfigurations\"\x00\x12Y\n\x12streamNotification\x12\x16.google.protobuf.Empty\x1a\'.android.emulation.control.Notification\"\x00\x30\x01\x12_\n\x18rotateVirtualSceneCamera\x12).android.emulation.control.RotationRadian\x1a\x16.google.protobuf.Empty\"\x00\x12^\n\x1dsetVirtualSceneCameraVelocity\x12#.android.emulation.control.Velocity\x1a\x16.google.protobuf.Empty\"\x00\x12J\n\nsetPosture\x12\".android.emulation.control.Posture\x1a\x16.google.protobuf.Empty\"\x00\x42&\n\x1c\x63om.android.emulator.controlP\x01\xa2\x02\x03\x41\x45\x43\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'android_env.proto.emulator_controller_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\034com.android.emulator.controlP\001\242\002\003AEC'
-  _PARAMETERVALUE.fields_by_name['data']._options = None
-  _PARAMETERVALUE.fields_by_name['data']._serialized_options = b'\020\001'
-  _IMAGE.fields_by_name['width']._options = None
-  _IMAGE.fields_by_name['width']._serialized_options = b'\030\001'
-  _IMAGE.fields_by_name['height']._options = None
-  _IMAGE.fields_by_name['height']._serialized_options = b'\030\001'
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\034com.android.emulator.controlP\001\242\002\003AEC'
+  _globals['_PARAMETERVALUE'].fields_by_name['data']._options = None
+  _globals['_PARAMETERVALUE'].fields_by_name['data']._serialized_options = b'\020\001'
+  _globals['_IMAGE'].fields_by_name['width']._options = None
+  _globals['_IMAGE'].fields_by_name['width']._serialized_options = b'\030\001'
+  _globals['_IMAGE'].fields_by_name['height']._options = None
+  _globals['_IMAGE'].fields_by_name['height']._serialized_options = b'\030\001'
   _globals['_VMRUNSTATE']._serialized_start=104
   _globals['_VMRUNSTATE']._serialized_end=319
   _globals['_VMRUNSTATE_RUNSTATE']._serialized_start=182
   _globals['_VMRUNSTATE_RUNSTATE']._serialized_end=319
   _globals['_PARAMETERVALUE']._serialized_start=321
   _globals['_PARAMETERVALUE']._serialized_end=355
   _globals['_PHYSICALMODELVALUE']._serialized_start=358
```

### Comparing `mobile-env-rl-3.5/android_env/proto/emulator_controller_pb2_grpc.py` & `mobile_env_rl-3.6/android_env/proto/emulator_controller_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/proto/raw_observation.proto` & `mobile_env_rl-3.6/android_env/proto/raw_observation.proto`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/proto/raw_observation_pb2.py` & `mobile_env_rl-3.6/android_env/proto/raw_observation_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: android_env/proto/raw_observation.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `mobile-env-rl-3.5/android_env/proto/task.proto` & `mobile_env_rl-3.6/android_env/proto/task.proto`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/proto/task_pb2.py` & `mobile_env_rl-3.6/android_env/proto/task_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: android_env/proto/task.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `mobile-env-rl-3.5/android_env/utils.py` & `mobile_env_rl-3.6/android_env/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,41 +16,52 @@
 Created by Danyang Zhang @X-Lance.
 """
 
 from android_env.proto import task_pb2
 import os.path
 from typing import Optional
 
-def fix_path(task: task_pb2.Task, task_directory: str) -> task_pb2.Task:
+def fix_path(task: task_pb2.Task, task_directory: str, remote_path: Optional[str] = None) -> task_pb2.Task:
     """
     Fixes the path setting in `task` and return it back.
 
     Args:
         task (task_pb2.Task): task config object
         task_directory (str): the path which is expected to be the base path,
           usually is the directory of the task config file
+        remote_path (Optional[str]): a different path for resources on the
+          remote machine
 
     Return:
         task_pb2.Task: task config object with the fixed path
     """
 
-    for st in task.setup_steps:
-        _fix(st, task_directory)
-    for st in task.reset_steps:
-        _fix(st, task_directory)
+    if remote_path is None:
+        for st in task.setup_steps:
+            _fix(st, task_directory)
+        for st in task.reset_steps:
+            _fix(st, task_directory)
+    else:
+        for st in task.setup_steps:
+            _fix(st, remote_path)
+        for st in task.reset_steps:
+            _fix(st, remote_path)
     for evt_s in task.event_sources:
         if evt_s.HasField("icon_match"):
             attribute_name: Optional[str] = evt_s.WhichOneof("event")
             if attribute_name=="icon_match" or attribute_name=="icon_detect_match":
                 path: str = getattr(evt_s, attribute_name).path
                 if not os.path.isabs(path):
                     getattr(evt_s, attribute_name).path =\
                             os.path.normpath(os.path.join(task_directory, path))
     return task
 
-def _fix(setup: task_pb2.SetupStep, task_directory: str):
+def _fix(setup: task_pb2.SetupStep, task_directory: str, and_abs: bool = False):
     if setup.HasField("adb_call")\
             and setup.adb_call.HasField("install_apk"):
         apk_path = setup.adb_call.install_apk.filesystem.path
         if not os.path.isabs(apk_path):
             setup.adb_call.install_apk.filesystem.path =\
                     os.path.normpath(os.path.join(task_directory, apk_path))
+        elif and_abs:
+            setup.adb_call.install_apk.filesystem.path =\
+                    os.path.normpath(os.path.join(task_directory, os.path.basename(apk_path)))
```

### Comparing `mobile-env-rl-3.5/android_env/wrappers/__init__.py` & `mobile_env_rl-3.6/android_env/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/wrappers/base_wrapper.py` & `mobile_env_rl-3.6/android_env/wrappers/base_wrapper.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/wrappers/discrete_action_wrapper.py` & `mobile_env_rl-3.6/android_env/wrappers/discrete_action_wrapper.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/wrappers/flat_interface_wrapper.py` & `mobile_env_rl-3.6/android_env/wrappers/flat_interface_wrapper.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/wrappers/float_pixels_wrapper.py` & `mobile_env_rl-3.6/android_env/wrappers/float_pixels_wrapper.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/wrappers/gym_wrapper.py` & `mobile_env_rl-3.6/android_env/wrappers/gym_wrapper.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/wrappers/image_rescale_wrapper.py` & `mobile_env_rl-3.6/android_env/wrappers/image_rescale_wrapper.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/wrappers/last_action_wrapper.py` & `mobile_env_rl-3.6/android_env/wrappers/last_action_wrapper.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/wrappers/recorder_wrapper.py` & `mobile_env_rl-3.6/android_env/wrappers/recorder_wrapper.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/wrappers/tap_action_wrapper.py` & `mobile_env_rl-3.6/android_env/wrappers/tap_action_wrapper.py`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/android_env/wrappers/vh_io_wrapper.py` & `mobile_env_rl-3.6/android_env/wrappers/vh_io_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,15 @@
         UP = 1
         RIGHT = 2
         DOWN = 3
     #  }}} Enum Types for VH Actions # 
 
     bounds_pattern: Pattern[str] = re.compile(r"\[(\d+),(\d+)\]\[(\d+),(\d+)\]")
 
+    # TODO: enable to set a custom filter_elements
     def __init__( self
                 , env: AndroidEnv
                 , tokenizer: PreTrainedTokenizer
                 , nb_click_frames: int = 3
                 , nb_scroll_frmaes: int = 10
                 , wait_sec: float = 0.
                 , action_batch: bool = False
@@ -271,15 +272,16 @@
                                 }
                               )
             return actions
         #  }}} method _process_action # 
 
     def _process_timestep(self, timestep: dm_env.TimeStep) -> dm_env.TimeStep:
         #  method _process_timestep {{{ # 
-        self._bbox_list: List[List[int]] = filter_elements(timestep.observation["view_hierarchy"])[1]
+        if timestep.observation["view_hierarchy"] is not None:
+            self._bbox_list: List[List[int]] = filter_elements(timestep.observation["view_hierarchy"])[1]
         return timestep
         #  }}} method _process_timestep # 
 
     def step(self, action: Dict[str, np.ndarray]) -> dm_env.TimeStep:
         #  method step {{{ # 
         """
         Args:
```

### Comparing `mobile-env-rl-3.5/mobile_env_rl.egg-info/PKG-INFO` & `mobile_env_rl-3.6/mobile_env_rl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobile-env-rl
-Version: 3.5
+Version: 3.6
 Summary: A Universal Platform for Training and Evaluation of Mobile Interaction
 Home-page: https://github.com/X-LANCE/Mobile-Env
 Author: Danyang Zhang @X-Lance
 Author-email: "Danyang Zhang @X-Lance" <zdy004007@126.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
@@ -245,14 +245,22 @@
 Requires-Dist: pytest-xdist; extra == "testing"
 
 <!-- vimc: call SyntaxRange#Include('```sh', '```', 'sh', 'NonText'): -->
 <!-- vimc: call SyntaxRange#Include('```bibtex', '```', 'bib', 'NonText'): -->
 
 ## NEWS!!
 
+* (2024-04-30 v3.6)
+  * Updated function to load a remote simulator to enable providing the remote
+    resources with a different path with the path of the local task definition
+    file.
+  * Updated task template toolkit, added new slot modifiers and sytaxes for
+    task config file.
+  * Fixed known bugs.
+
 * (2023-12-18 v3.5)
   * Owing to the long time delay of VH check and screenshot check, we updated
     the mechanism of managing the check time. By this way, the requirement of
     sufficient check for the episode events and the resulted long delay can be
     balanced.
   * Added multiple rating methods to `ResponseEvent`: regex matching, fuzzy
     matching, and vector encoding matching.
@@ -263,14 +271,16 @@
     and enabled resizing the image before and after transferring to shrink the
     transferred data.
   * Merged annotation tool to the main branch. The original annotation-tool
     branch is deprecated.
   * Added support to `ResponseEvent` to annotation tool.
   * Supplemented several commandline options to annotation-tool.
 
+For more details, please see our [Change Log](Changelog) and Documents.
+
 * (2023-10-31 v3.0) Migrated VH node specification from the original VH path to
   Mobile-Env-customized CSS selector (me-selector) and added repeatability
   control to EventSlots. Repeatability control for EventSlots may be useful to
   prevent repetitive triggering of an `OR`-type virtual event combining
   multiple types of event sources.
 
 Please see our [Change Log](Changelog) and
@@ -381,19 +391,22 @@
 just required. Detailed instructions can be found in [Extending a New
 Environment (App) or a New Task Based on
 Mobile-Env](docs/task-definition-en.md).
 
 Several demo task definitions are provided under `demos`. Three of them are
 migrated from  AndroidEnv:
 
-* `classic_2048.m.textproto` - Classic 2048 game.
+* `classic_2048.m.textproto` - [Classic 2048
+  game](https://github.com/google-deepmind/android_env/blob/main/docs/example_tasks.md#classic-2048).
 * `accessibility_forwarder_clock_set_timer.m.textproto` - A simple task
-  requiring the agent to reset a running timer.
-* `systemui_egg_land_default.m.textproto` - Flappy Droid. An open-sourced
-  implementation of classic game, Flappy Bird.
+  requiring the agent to [reset a running
+  timer](https://github.com/google-deepmind/android_env/blob/main/docs/example_tasks.md#accessibility-forwarder).
+* `systemui_egg_land_default.m.textproto` - [Flappy
+  Droid](https://github.com/google-deepmind/android_env/blob/main/docs/example_tasks.md#flappydroid).
+  An open-sourced implementation of classic game, Flappy Bird.
 
 Another one, `openmoneybox.add_billings.textproto` is defined upon an
 open-sourced billing app,
 [OpenMoneyBox](https://f-droid.org/en/packages/com.igisw.openmoneybox/).
 Details are referred to in the task definition files.
 
 ### Miscellaneous Auxiliary Tools
@@ -452,18 +465,19 @@
 at <https://arxiv.org/abs/2305.08144>.
 
 If you find Mobile-Env useful in your research, you can cite the project using
 the following BibTeX:
 
 ```bibtex
 @article{DanyangZhang2023_MobileEnv,
-  title     = {{Mobile-Env}: An Evaluation Platform and Benchmark for Interactive Agents in LLM Era},
+  title     = {{Mobile-Env}: An Evaluation Platform and Benchmark for LLM-GUI Interaction},
   author    = {Danyang Zhang and
-               Lu Chen and
+               Hongshen Xu and
                Zihan Zhao and
+               Lu Chen and
                Ruisheng Cao and
                Kai Yu},
   journal   = {CoRR},
   volume    = {abs/2305.08144},
   year      = {2023},
   url       = {https://arxiv.org/abs/2305.08144},
   eprinttype = {arXiv},
```

### Comparing `mobile-env-rl-3.5/mobile_env_rl.egg-info/SOURCES.txt` & `mobile_env_rl-3.6/mobile_env_rl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mobile-env-rl-3.5/pyproject.toml` & `mobile_env_rl-3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mobile-env-rl"
-version = "3.5"
+version = "3.6"
 authors = [{name = "Danyang Zhang @X-Lance", email = "zdy004007@126.com"}]
 license = {file = "LICENSE"}
 description = "A Universal Platform for Training and Evaluation of Mobile Interaction"
 keywords = ["InfoUI interaction"]
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `mobile-env-rl-3.5/setup.py` & `mobile_env_rl-3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
   def run(self):
     self.run_command('generate_protos')
     build_py.run(self)
 
 setup(
     name='mobile-env-rl',
-    version='3.5',
+    version='3.6',
     description='Mobile-Env: A Universal Platform for Training and Evaluation of Mobile Interaction',
     long_description=description,
     author='Danyang Zhang @X-Lance',
     license='Apache License, Version 2.0',
     keywords='InfoUI interaction',
     url='https://github.com/X-LANCE/Mobile-Env',
     packages=find_packages(exclude=['examples']),
```

### Comparing `mobile-env-rl-3.5/tests/test_css_selector.py` & `mobile_env_rl-3.6/tests/test_css_selector.py`

 * *Files identical despite different names*

