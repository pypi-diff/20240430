# Comparing `tmp/brayns-3.7.1.tar.gz` & `tmp/brayns-3.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brayns-3.7.1.tar", last modified: Thu Apr  4 14:12:20 2024, max compression
+gzip compressed data, was "brayns-3.7.2.tar", last modified: Tue Apr 30 12:58:06 2024, max compression
```

## Comparing `brayns-3.7.1.tar` & `brayns-3.7.2.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:12:20.856512 brayns-3.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-04 14:12:18.000000 brayns-3.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-04 14:12:20.856512 brayns-3.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-04 14:12:18.000000 brayns-3.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:12:20.844512 brayns-3.7.1/brayns/
--rw-r--r--   0 runner    (1001) docker     (127)     8993 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:12:20.848512 brayns-3.7.1/brayns/core/
--rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/core/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/core/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/core/camera_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/core/color_ramp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/core/coloring.py
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/core/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/core/framebuffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/core/gbuffer_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7158 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/core/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/core/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/core/light.py
--rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/core/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    14941 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/core/material.py
--rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/core/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/core/near_clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/core/opacity_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/core/pick.py
--rw-r--r--   0 runner    (1001) docker     (127)     8780 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/core/projection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/core/renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/core/simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/core/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/core/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/core/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:12:20.848512 brayns-3.7.1/brayns/movie/
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/movie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/movie/movie.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/movie/movie_frames.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:12:20.848512 brayns-3.7.1/brayns/network/
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/network/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/network/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/network/future.py
--rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/network/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:12:20.848512 brayns-3.7.1/brayns/network/jsonrpc/
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/network/jsonrpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/network/jsonrpc/json_rpc_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/network/jsonrpc/json_rpc_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/network/jsonrpc/json_rpc_future.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/network/jsonrpc/json_rpc_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/network/jsonrpc/json_rpc_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/network/jsonrpc/json_rpc_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/network/jsonrpc/json_rpc_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/network/jsonrpc/json_rpc_reply.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/network/jsonrpc/json_rpc_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/network/jsonrpc/json_rpc_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/network/jsonrpc/json_rpc_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/network/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/network/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:12:20.852512 brayns-3.7.1/brayns/network/websocket/
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/network/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/network/websocket/async_web_socket.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/network/websocket/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/network/websocket/event_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/network/websocket/web_socket.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/network/websocket/web_socket_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/network/websocket/web_socket_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/network/websocket/web_socket_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:12:20.852512 brayns-3.7.1/brayns/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/plugins/atlas.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/plugins/bbp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/plugins/cell_placement.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/plugins/circuit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/plugins/cylindric_camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/plugins/dti.py
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/plugins/morphology.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/plugins/nrrd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/plugins/protein.py
--rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/plugins/sonata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/plugins/xyz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:12:20.852512 brayns-3.7.1/brayns/service/
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/service/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/service/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:12:20.856512 brayns-3.7.1/brayns/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/utils/bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/utils/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/utils/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/utils/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/utils/plane_equation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/utils/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/utils/rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/utils/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/utils/vector.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-04 14:12:18.000000 brayns-3.7.1/brayns/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:12:20.844512 brayns-3.7.1/brayns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-04 14:12:20.000000 brayns-3.7.1/brayns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-04 14:12:20.000000 brayns-3.7.1/brayns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:12:20.000000 brayns-3.7.1/brayns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 14:12:20.000000 brayns-3.7.1/brayns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 14:12:20.000000 brayns-3.7.1/brayns.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-04 14:12:18.000000 brayns-3.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-04 14:12:20.856512 brayns-3.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-04 14:12:18.000000 brayns-3.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:58:06.845795 brayns-3.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-30 12:58:04.000000 brayns-3.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-30 12:58:06.845795 brayns-3.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-30 12:58:04.000000 brayns-3.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:58:06.833795 brayns-3.7.2/brayns/
+-rw-r--r--   0 runner    (1001) docker     (127)     8993 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:58:06.837795 brayns-3.7.2/brayns/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/core/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/core/camera_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/core/color_ramp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/core/coloring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/core/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/core/framebuffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/core/gbuffer_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7158 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/core/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/core/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/core/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/core/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14941 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/core/material.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/core/near_clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/core/opacity_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/core/pick.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8780 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/core/projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/core/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/core/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/core/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/core/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/core/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:58:06.837795 brayns-3.7.2/brayns/movie/
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/movie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/movie/movie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/movie/movie_frames.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:58:06.837795 brayns-3.7.2/brayns/network/
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/network/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/network/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/network/future.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/network/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:58:06.837795 brayns-3.7.2/brayns/network/jsonrpc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/network/jsonrpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/network/jsonrpc/json_rpc_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/network/jsonrpc/json_rpc_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/network/jsonrpc/json_rpc_future.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/network/jsonrpc/json_rpc_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/network/jsonrpc/json_rpc_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/network/jsonrpc/json_rpc_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/network/jsonrpc/json_rpc_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/network/jsonrpc/json_rpc_reply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/network/jsonrpc/json_rpc_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/network/jsonrpc/json_rpc_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/network/jsonrpc/json_rpc_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/network/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/network/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:58:06.841795 brayns-3.7.2/brayns/network/websocket/
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/network/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/network/websocket/async_web_socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/network/websocket/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/network/websocket/event_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/network/websocket/web_socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/network/websocket/web_socket_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/network/websocket/web_socket_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/network/websocket/web_socket_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:58:06.841795 brayns-3.7.2/brayns/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/plugins/atlas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/plugins/bbp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/plugins/cell_placement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/plugins/circuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/plugins/cylindric_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/plugins/dti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/plugins/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/plugins/nrrd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/plugins/protein.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/plugins/sonata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/plugins/xyz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:58:06.841795 brayns-3.7.2/brayns/service/
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/service/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/service/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:58:06.845795 brayns-3.7.2/brayns/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/utils/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/utils/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/utils/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/utils/plane_equation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/utils/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/utils/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/utils/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/utils/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-30 12:58:04.000000 brayns-3.7.2/brayns/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:58:06.833795 brayns-3.7.2/brayns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-30 12:58:06.000000 brayns-3.7.2/brayns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-30 12:58:06.000000 brayns-3.7.2/brayns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 12:58:06.000000 brayns-3.7.2/brayns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-30 12:58:06.000000 brayns-3.7.2/brayns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-30 12:58:06.000000 brayns-3.7.2/brayns.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-30 12:58:04.000000 brayns-3.7.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-30 12:58:06.845795 brayns-3.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-30 12:58:04.000000 brayns-3.7.2/setup.py
```

### Comparing `brayns-3.7.1/PKG-INFO` & `brayns-3.7.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brayns
-Version: 3.7.1
+Version: 3.7.2
 Summary: Brayns Python API
 Home-page: https://github.com/BlueBrain/Brayns
 Author: Blue Brain Project
 Author-email: bbp-open-source@googlegroups.com
 License: LGPLv3
 Download-URL: https://github.com/BlueBrain/Brayns
 Project-URL: Tracker, https://bbpteam.epfl.ch/project/issues/projects/BRAYNS/issues
```

### Comparing `brayns-3.7.1/README.md` & `brayns-3.7.2/README.md`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/__init__.py` & `brayns-3.7.2/brayns/__init__.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/core/__init__.py` & `brayns-3.7.2/brayns/core/__init__.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/core/application.py` & `brayns-3.7.2/brayns/core/application.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/core/camera.py` & `brayns-3.7.2/brayns/core/camera.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/core/camera_controller.py` & `brayns-3.7.2/brayns/core/camera_controller.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/core/color_ramp.py` & `brayns-3.7.2/brayns/core/color_ramp.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/core/coloring.py` & `brayns-3.7.2/brayns/core/coloring.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/core/entrypoint.py` & `brayns-3.7.2/brayns/core/entrypoint.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/core/framebuffer.py` & `brayns-3.7.2/brayns/core/framebuffer.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/core/gbuffer_exporter.py` & `brayns-3.7.2/brayns/core/gbuffer_exporter.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/core/geometry.py` & `brayns-3.7.2/brayns/core/geometry.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/core/image.py` & `brayns-3.7.2/brayns/core/image.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/core/light.py` & `brayns-3.7.2/brayns/core/light.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/core/loader.py` & `brayns-3.7.2/brayns/core/loader.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/core/material.py` & `brayns-3.7.2/brayns/core/material.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/core/model.py` & `brayns-3.7.2/brayns/core/model.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/core/near_clip.py` & `brayns-3.7.2/brayns/core/near_clip.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/core/opacity_curve.py` & `brayns-3.7.2/brayns/core/opacity_curve.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/core/pick.py` & `brayns-3.7.2/brayns/core/pick.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/core/projection.py` & `brayns-3.7.2/brayns/core/projection.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/core/renderer.py` & `brayns-3.7.2/brayns/core/renderer.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/core/simulation.py` & `brayns-3.7.2/brayns/core/simulation.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/core/snapshot.py` & `brayns-3.7.2/brayns/core/snapshot.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/core/version.py` & `brayns-3.7.2/brayns/core/version.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/core/view.py` & `brayns-3.7.2/brayns/core/view.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/movie/__init__.py` & `brayns-3.7.2/brayns/movie/__init__.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/movie/movie.py` & `brayns-3.7.2/brayns/movie/movie.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/movie/movie_frames.py` & `brayns-3.7.2/brayns/movie/movie_frames.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/network/__init__.py` & `brayns-3.7.2/brayns/network/__init__.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/network/client.py` & `brayns-3.7.2/brayns/network/client.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/network/connector.py` & `brayns-3.7.2/brayns/network/connector.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/network/future.py` & `brayns-3.7.2/brayns/network/future.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/network/instance.py` & `brayns-3.7.2/brayns/network/instance.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/network/jsonrpc/__init__.py` & `brayns-3.7.2/brayns/network/jsonrpc/__init__.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/network/jsonrpc/json_rpc_dispatcher.py` & `brayns-3.7.2/brayns/network/jsonrpc/json_rpc_dispatcher.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/network/jsonrpc/json_rpc_error.py` & `brayns-3.7.2/brayns/network/jsonrpc/json_rpc_error.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/network/jsonrpc/json_rpc_future.py` & `brayns-3.7.2/brayns/network/jsonrpc/json_rpc_future.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/network/jsonrpc/json_rpc_handler.py` & `brayns-3.7.2/brayns/network/jsonrpc/json_rpc_handler.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/network/jsonrpc/json_rpc_listener.py` & `brayns-3.7.2/brayns/network/jsonrpc/json_rpc_listener.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/network/jsonrpc/json_rpc_manager.py` & `brayns-3.7.2/brayns/network/jsonrpc/json_rpc_manager.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/network/jsonrpc/json_rpc_progress.py` & `brayns-3.7.2/brayns/network/jsonrpc/json_rpc_progress.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/network/jsonrpc/json_rpc_reply.py` & `brayns-3.7.2/brayns/network/jsonrpc/json_rpc_reply.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/network/jsonrpc/json_rpc_request.py` & `brayns-3.7.2/brayns/network/jsonrpc/json_rpc_request.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/network/jsonrpc/json_rpc_task.py` & `brayns-3.7.2/brayns/network/jsonrpc/json_rpc_task.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/network/jsonrpc/json_rpc_tasks.py` & `brayns-3.7.2/brayns/network/jsonrpc/json_rpc_tasks.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/network/listener.py` & `brayns-3.7.2/brayns/network/listener.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/network/logger.py` & `brayns-3.7.2/brayns/network/logger.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/network/websocket/__init__.py` & `brayns-3.7.2/brayns/network/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/network/websocket/async_web_socket.py` & `brayns-3.7.2/brayns/network/websocket/async_web_socket.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/network/websocket/errors.py` & `brayns-3.7.2/brayns/network/websocket/errors.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/network/websocket/event_loop.py` & `brayns-3.7.2/brayns/network/websocket/event_loop.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/network/websocket/web_socket.py` & `brayns-3.7.2/brayns/network/websocket/web_socket.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/network/websocket/web_socket_client.py` & `brayns-3.7.2/brayns/network/websocket/web_socket_client.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/network/websocket/web_socket_connector.py` & `brayns-3.7.2/brayns/network/websocket/web_socket_connector.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/network/websocket/web_socket_listener.py` & `brayns-3.7.2/brayns/network/websocket/web_socket_listener.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/plugins/__init__.py` & `brayns-3.7.2/brayns/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/plugins/atlas.py` & `brayns-3.7.2/brayns/plugins/atlas.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/plugins/bbp.py` & `brayns-3.7.2/brayns/plugins/bbp.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/plugins/cell_placement.py` & `brayns-3.7.2/brayns/plugins/cell_placement.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/plugins/circuit.py` & `brayns-3.7.2/brayns/plugins/circuit.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/plugins/cylindric_camera.py` & `brayns-3.7.2/brayns/plugins/cylindric_camera.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/plugins/dti.py` & `brayns-3.7.2/brayns/plugins/dti.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/plugins/morphology.py` & `brayns-3.7.2/brayns/plugins/morphology.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/plugins/nrrd.py` & `brayns-3.7.2/brayns/plugins/nrrd.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/plugins/protein.py` & `brayns-3.7.2/brayns/plugins/protein.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/plugins/sonata.py` & `brayns-3.7.2/brayns/plugins/sonata.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/plugins/xyz.py` & `brayns-3.7.2/brayns/plugins/xyz.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/service/__init__.py` & `brayns-3.7.2/brayns/service/__init__.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/service/manager.py` & `brayns-3.7.2/brayns/service/manager.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/service/process.py` & `brayns-3.7.2/brayns/service/process.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/service/service.py` & `brayns-3.7.2/brayns/service/service.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/utils/__init__.py` & `brayns-3.7.2/brayns/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/utils/bounds.py` & `brayns-3.7.2/brayns/utils/bounds.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/utils/color.py` & `brayns-3.7.2/brayns/utils/color.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/utils/error.py` & `brayns-3.7.2/brayns/utils/error.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/utils/image.py` & `brayns-3.7.2/brayns/utils/image.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/utils/json_schema.py` & `brayns-3.7.2/brayns/utils/json_schema.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/utils/plane_equation.py` & `brayns-3.7.2/brayns/utils/plane_equation.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/utils/quaternion.py` & `brayns-3.7.2/brayns/utils/quaternion.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/utils/rotation.py` & `brayns-3.7.2/brayns/utils/rotation.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/utils/transform.py` & `brayns-3.7.2/brayns/utils/transform.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/utils/vector.py` & `brayns-3.7.2/brayns/utils/vector.py`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/brayns/version.py` & `brayns-3.7.2/brayns/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 # FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this library; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
-VERSION = "3.7.1"
+VERSION = "3.7.2"
 """Version tag of brayns Python package (major.minor.patch)."""
```

### Comparing `brayns-3.7.1/brayns.egg-info/PKG-INFO` & `brayns-3.7.2/brayns.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brayns
-Version: 3.7.1
+Version: 3.7.2
 Summary: Brayns Python API
 Home-page: https://github.com/BlueBrain/Brayns
 Author: Blue Brain Project
 Author-email: bbp-open-source@googlegroups.com
 License: LGPLv3
 Download-URL: https://github.com/BlueBrain/Brayns
 Project-URL: Tracker, https://bbpteam.epfl.ch/project/issues/projects/BRAYNS/issues
```

### Comparing `brayns-3.7.1/brayns.egg-info/SOURCES.txt` & `brayns-3.7.2/brayns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/requirements.txt` & `brayns-3.7.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `brayns-3.7.1/setup.cfg` & `brayns-3.7.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = brayns
-version = 3.7.1
+version = 3.7.2
 url = https://github.com/BlueBrain/Brayns
 download_url = https://github.com/BlueBrain/Brayns
 project_urls = 
 	Tracker = https://bbpteam.epfl.ch/project/issues/projects/BRAYNS/issues
 	Source = https://github.com/BlueBrain/Brayns
 author = Blue Brain Project
 author_email = bbp-open-source@googlegroups.com
```

### Comparing `brayns-3.7.1/setup.py` & `brayns-3.7.2/setup.py`

 * *Files identical despite different names*

