# Comparing `tmp/neobuilder-5.0.0b1.tar.gz` & `tmp/neobuilder-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neobuilder-5.0.0b1.tar", last modified: Mon Apr 15 15:44:26 2024, max compression
+gzip compressed data, was "neobuilder-5.1.0.tar", last modified: Tue Apr 30 15:03:31 2024, max compression
```

## Comparing `neobuilder-5.0.0b1.tar` & `neobuilder-5.1.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:26.237934 neobuilder-5.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-04-15 15:44:26.237934 neobuilder-5.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:26.229934 neobuilder-5.0.0b1/neobuilder/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:26.229934 neobuilder-5.0.0b1/neobuilder/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/cli/neobuilder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:26.225934 neobuilder-5.0.0b1/neobuilder/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:26.229934 neobuilder-5.0.0b1/neobuilder/data/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/data/templates/dataclass.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/data/templates/dataclass_module.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/data/templates/grpc_receiver.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/data/templates/grpc_sender.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/data/templates/init.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/data/templates/interface.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:26.229934 neobuilder-5.0.0b1/neobuilder/data/templates/macros/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/data/templates/macros/indentclude.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:26.229934 neobuilder-5.0.0b1/neobuilder/data/templates/parts/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/data/templates/parts/_enum_map.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/data/templates/parts/_interface_method.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/data/templates/parts/_interface_service.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/data/templates/parts/_nested_messages.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/data/templates/root_init.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:26.233934 neobuilder-5.0.0b1/neobuilder/descwrap/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/descwrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/descwrap/_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/descwrap/_method.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:26.233934 neobuilder-5.0.0b1/neobuilder/generators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:26.233934 neobuilder-5.0.0b1/neobuilder/generators/servicebuilders/
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/generators/servicebuilders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/generators/servicebuilders/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/generators/servicebuilders/grpc_receiver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/generators/servicebuilders/grpc_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/generators/servicebuilders/grpc_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/generators/servicebuilders/implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/generators/servicebuilders/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:26.233934 neobuilder-5.0.0b1/neobuilder/generators/symbols/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/generators/symbols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/generators/symbols/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    16693 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/generators/symbols/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     7423 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/generators/symbols/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/generators/symbols/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:26.233934 neobuilder-5.0.0b1/neobuilder/neobuilder/
--rw-r--r--   0 runner    (1001) docker     (127)    15793 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/neobuilder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:26.233934 neobuilder-5.0.0b1/neobuilder/neobuilder/render/
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/neobuilder/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/neobuilder/render/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:26.237934 neobuilder-5.0.0b1/neobuilder/structs/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/structs/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/structs/protofile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/neobuilder/structs/pytype.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:26.237934 neobuilder-5.0.0b1/neobuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-04-15 15:44:26.000000 neobuilder-5.0.0b1/neobuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-15 15:44:26.000000 neobuilder-5.0.0b1/neobuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 15:44:26.000000 neobuilder-5.0.0b1/neobuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-15 15:44:26.000000 neobuilder-5.0.0b1/neobuilder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-15 15:44:26.000000 neobuilder-5.0.0b1/neobuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 15:44:26.000000 neobuilder-5.0.0b1/neobuilder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 15:44:26.237934 neobuilder-5.0.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:44:26.237934 neobuilder-5.0.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/tests/test_neobuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)    13492 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/tests/test_services.py
--rw-r--r--   0 runner    (1001) docker     (127)    60294 2024-04-15 15:44:16.000000 neobuilder-5.0.0b1/tests/test_zdataclassbuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:31.044690 neobuilder-5.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-30 15:03:21.000000 neobuilder-5.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-04-30 15:03:31.044690 neobuilder-5.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-30 15:03:21.000000 neobuilder-5.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:31.036690 neobuilder-5.1.0/neobuilder/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:31.040691 neobuilder-5.1.0/neobuilder/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/cli/neobuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:31.036690 neobuilder-5.1.0/neobuilder/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:31.040691 neobuilder-5.1.0/neobuilder/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/data/templates/dataclass.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/data/templates/dataclass_module.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/data/templates/grpc_receiver.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/data/templates/grpc_sender.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/data/templates/init.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/data/templates/interface.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:31.040691 neobuilder-5.1.0/neobuilder/data/templates/macros/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/data/templates/macros/indentclude.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:31.040691 neobuilder-5.1.0/neobuilder/data/templates/parts/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/data/templates/parts/_enum_map.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/data/templates/parts/_interface_method.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/data/templates/parts/_interface_service.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/data/templates/parts/_nested_messages.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/data/templates/root_init.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:31.040691 neobuilder-5.1.0/neobuilder/descwrap/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/descwrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/descwrap/_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/descwrap/_method.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:31.040691 neobuilder-5.1.0/neobuilder/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:31.044690 neobuilder-5.1.0/neobuilder/generators/servicebuilders/
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/generators/servicebuilders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/generators/servicebuilders/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/generators/servicebuilders/grpc_receiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/generators/servicebuilders/grpc_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/generators/servicebuilders/grpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/generators/servicebuilders/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/generators/servicebuilders/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:31.044690 neobuilder-5.1.0/neobuilder/generators/symbols/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/generators/symbols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/generators/symbols/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16693 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/generators/symbols/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/generators/symbols/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/generators/symbols/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:31.044690 neobuilder-5.1.0/neobuilder/neobuilder/
+-rw-r--r--   0 runner    (1001) docker     (127)    16038 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/neobuilder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:31.044690 neobuilder-5.1.0/neobuilder/neobuilder/render/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/neobuilder/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/neobuilder/render/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:31.044690 neobuilder-5.1.0/neobuilder/structs/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/structs/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/structs/protofile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-30 15:03:21.000000 neobuilder-5.1.0/neobuilder/structs/pytype.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:31.044690 neobuilder-5.1.0/neobuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-04-30 15:03:31.000000 neobuilder-5.1.0/neobuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-30 15:03:31.000000 neobuilder-5.1.0/neobuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:03:31.000000 neobuilder-5.1.0/neobuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-30 15:03:31.000000 neobuilder-5.1.0/neobuilder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-30 15:03:31.000000 neobuilder-5.1.0/neobuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-30 15:03:31.000000 neobuilder-5.1.0/neobuilder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-30 15:03:21.000000 neobuilder-5.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:03:31.044690 neobuilder-5.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-30 15:03:21.000000 neobuilder-5.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:31.044690 neobuilder-5.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-04-30 15:03:21.000000 neobuilder-5.1.0/tests/test_neobuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13492 2024-04-30 15:03:21.000000 neobuilder-5.1.0/tests/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60294 2024-04-30 15:03:21.000000 neobuilder-5.1.0/tests/test_zdataclassbuilder.py
```

### Comparing `neobuilder-5.0.0b1/LICENSE` & `neobuilder-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neobuilder-5.0.0b1/PKG-INFO` & `neobuilder-5.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neobuilder
-Version: 5.0.0b1
+Version: 5.1.0
 Summary: Builds Neobuf Packages from Protobuf files using Protoplasm! :D
 Author-email: Thordur Matthiasson <thordurm@ccpgames.com>
 License: MIT License
         
         Copyright (c) 2022-2024 CCP Games
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `neobuilder-5.0.0b1/README.md` & `neobuilder-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `neobuilder-5.0.0b1/neobuilder/cli/neobuilder.py` & `neobuilder-5.1.0/neobuilder/cli/neobuilder.py`

 * *Files identical despite different names*

### Comparing `neobuilder-5.0.0b1/neobuilder/data/templates/dataclass_module.jinja2` & `neobuilder-5.1.0/neobuilder/data/templates/dataclass_module.jinja2`

 * *Files identical despite different names*

### Comparing `neobuilder-5.0.0b1/neobuilder/descwrap/_field.py` & `neobuilder-5.1.0/neobuilder/descwrap/_field.py`

 * *Files identical despite different names*

### Comparing `neobuilder-5.0.0b1/neobuilder/descwrap/_method.py` & `neobuilder-5.1.0/neobuilder/descwrap/_method.py`

 * *Files identical despite different names*

### Comparing `neobuilder-5.0.0b1/neobuilder/generators/servicebuilders/__init__.py` & `neobuilder-5.1.0/neobuilder/generators/servicebuilders/__init__.py`

 * *Files identical despite different names*

### Comparing `neobuilder-5.0.0b1/neobuilder/generators/servicebuilders/base.py` & `neobuilder-5.1.0/neobuilder/generators/servicebuilders/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     def get_template_context(self) -> Dict:
         return {
             'module_full_name': self.module.get_module_full_name(),
             'iso_timestamp': datetime.datetime.now().isoformat(),
         }
 
     def render_top(self) -> str:
-        # TODO(thordurm@ccpgames.com) 2022-06-24: Remove!
+        # TODO(thordurm@ccpgames.com) 2022-06-24: Remove... why?
         return ('# Auto-Generated file - DO NOT EDIT!\n'
                 f'# Source module: {self.module.get_module_full_name()}\n'
                 f'# Generated at: {datetime.datetime.now().isoformat()}\n')
 
     def render_service_list(self) -> List[str]:
         return [svc.render(self.builder_name) for svc in self.module.service_map.values()]
 
@@ -45,14 +45,15 @@
         self.service = service
         self.indent_level = indent_level
         self.indent_str = self.service.indent
         self.base_indent = self.indent_str * indent_level
 
     def get_template_context(self) -> Dict:
         return {
+            'is_grpc': self.service.module.is_grpc_file(),
             'service': self.service,
             'service_name': self.service.service_descriptor.name,
             '_indent_level': self.indent_level,
             '_indent_str': self.indent_str,
             '_base_indent': self.base_indent,
             'method_list': [self.get_method_context(m) for m in self.service.method_map.values()],
             'indent_spaces': self.indent_level * 4,
```

### Comparing `neobuilder-5.0.0b1/neobuilder/generators/servicebuilders/grpc_receiver.py` & `neobuilder-5.1.0/neobuilder/generators/servicebuilders/grpc_receiver.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
         return f'{self.module.get_file_full_name()[:-7]}_grpc_receiver.py'
 
     def render_imports(self) -> str:
         import_set = {
             f'from {self.module.get_package()} import {self.module.get_module_name()} as pb2',
             f'from {self.module.get_package()} import {self.module.get_module_name()}_grpc as pb2_grpc',
             f'from {self.module.get_package()} import {self.module.get_module_name()[:-3]}dc as dc',
-            f'from {self.module.get_package()} import {self.module.get_module_name()[:-3]}api as api',
         }
 
         for s in self.module.service_map.values():
             for m in s.method_map.values():
                 if m.input:
                     if m.input.self_import:
                         if self.module.descriptor != m.input.self_import.descriptor.file:
@@ -38,14 +37,15 @@
         if import_set:
             return '\n'.join(sorted(import_set))
         return ''
 
     def get_template_context(self) -> Dict:
         d = super().get_template_context()
         d.update({
+            'api_import': f'from {self.module.get_package()} import {self.module.get_module_name()[:-3]}api as api',
             'services': self.render_services(),
             'imports': self.render_imports(),
             'all_list': [f'{svc.service_descriptor.name}GrpcServicer' for svc in self.module.service_map.values()],
         })
         return d
 
     def render(self) -> str:
@@ -56,15 +56,15 @@
     builder_name = __name__.split('.')[-1]  # Grab module name
 
     def render(self) -> str:
         __ = self.indent_str
         i = self.base_indent
         return (
             f'{i}class {self.service.service_descriptor.name}GrpcServicer(plasm.BaseGrpcServicer, pb2_grpc.{self.service.service_descriptor.name}Servicer):\n'
-            f'{i}{__}def __init__(self, implementation: api.{self.service.service_descriptor.name}Interface):\n'
+            f"{i}{__}def __init__(self, implementation: 'api.{self.service.service_descriptor.name}Interface'):\n"
             f'{i}{__}{__}super().__init__(implementation)\n'
             '\n'
             f'{i}{__}def add_to_server(self, server):\n'
             f'{i}{__}{__}pb2_grpc.add_{self.service.service_descriptor.name}Servicer_to_server(self, server)\n'
             '\n'
             f'{self.render_methods()}'
             '\n'
```

### Comparing `neobuilder-5.0.0b1/neobuilder/generators/servicebuilders/grpc_sender.py` & `neobuilder-5.1.0/neobuilder/generators/servicebuilders/grpc_sender.py`

 * *Files identical despite different names*

### Comparing `neobuilder-5.0.0b1/neobuilder/generators/servicebuilders/grpc_server.py` & `neobuilder-5.1.0/neobuilder/generators/servicebuilders/grpc_server.py`

 * *Files identical despite different names*

### Comparing `neobuilder-5.0.0b1/neobuilder/generators/servicebuilders/implementation.py` & `neobuilder-5.1.0/neobuilder/generators/servicebuilders/implementation.py`

 * *Files identical despite different names*

### Comparing `neobuilder-5.0.0b1/neobuilder/generators/servicebuilders/interface.py` & `neobuilder-5.1.0/neobuilder/generators/servicebuilders/interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,18 @@
         return f'{self.module.get_file_full_name()[:-7]}_api.py'
 
     def get_import_lines(self) -> List[str]:
         import_set = {
             f'from {self.module.get_package()} import {self.module.get_module_name()[:-3]}dc as dc'
         }
         for s in self.module.service_map.values():
+
+            if self.module.is_grpc_file():
+                import_set.add(f'from {self.module.get_package()}.{self.module.get_module_name()[:-3]}grpc_receiver import {s.service_descriptor.name}GrpcServicer')
+
             for m in s.method_map.values():
                 # From 3.2
                 if m.input.self_import.get_package() != 'google.protobuf':
                     import_set.add(m.input.self_import.get_render_import(self.module.descriptor))
 
                 if m.output.self_import.get_package() != 'google.protobuf':
                     import_set.add(m.output.self_import.get_render_import(self.module.descriptor))
```

### Comparing `neobuilder-5.0.0b1/neobuilder/generators/symbols/common.py` & `neobuilder-5.1.0/neobuilder/generators/symbols/common.py`

 * *Files identical despite different names*

### Comparing `neobuilder-5.0.0b1/neobuilder/generators/symbols/dataclass.py` & `neobuilder-5.1.0/neobuilder/generators/symbols/dataclass.py`

 * *Files identical despite different names*

### Comparing `neobuilder-5.0.0b1/neobuilder/generators/symbols/modules.py` & `neobuilder-5.1.0/neobuilder/generators/symbols/modules.py`

 * *Files 5% similar despite different names*

```diff
@@ -159,14 +159,15 @@
             'proto_import': self.render_proto_import(),
             'enum_list': [en.render_py() for en in self.enum_map.values()],
             'message_list': [pc.render_py() for pc in self.message_map.values()],
             'all_list': self.get_all_list(),
         })
 
     def write_dataclass_file(self):
+        log.debug(f' - - write_dataclass_file() {self.get_render_file_name()}')
         self.write_file(self.get_render_file_name(), self.render_dataclass_file())
 
     #
     # GRPC SERVER FILE!
     #
 
     def write_grpc_server_file(self):
@@ -178,36 +179,39 @@
 
     #
     # API FILE!
     #
 
     def write_api_file(self):
         b = servicebuilders.get_module_builder('interface')(self)
+        log.debug(f' - - write_api_file() {b.get_render_filename()}')
         self.write_file(b.get_render_filename(), b.render())
 
     def render_api_file(self):
         return self.render('interface')
 
     #
     # GRPC FILE! - grpc_receiver
     #
 
     def write_grpc_file(self):
         b = servicebuilders.get_module_builder('grpc_receiver')(self)
+        log.debug(f' - - write_grpc_file() {b.get_render_filename()}')
         self.write_file(b.get_render_filename(), b.render())
 
     def render_grpc_file(self):
         return self.render('grpc_receiver')
 
     #
     # GRPC IMPL FILE!
     #
 
     def write_grpc_impl_file(self):
         b = servicebuilders.get_module_builder('grpc_sender')(self)
+        log.debug(f' - - write_grpc_impl_file() {b.get_render_filename()}')
         self.write_file(b.get_render_filename(), b.render())
 
     def render_grpc_impl_file(self):
         return self.render('grpc_sender')
 
     #
     # Implementation FILE!
```

### Comparing `neobuilder-5.0.0b1/neobuilder/generators/symbols/service.py` & `neobuilder-5.1.0/neobuilder/generators/symbols/service.py`

 * *Files identical despite different names*

### Comparing `neobuilder-5.0.0b1/neobuilder/neobuilder/__init__.py` & `neobuilder-5.1.0/neobuilder/neobuilder/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,19 @@
         self._next_version = None
         self.commit_message = 'No commit message'
         self.verbose = verbose
         logging.basicConfig(level=(logging.DEBUG if self.verbose else logging.INFO),
                             format='%(levelname)8s - %(message)s')
         log.info(f'Initializing Neobuilder {self.neobuilder_version()}')
 
+        log.debug(f'{self.package=}')
+        log.debug(f'{self.protopath=}')
+        log.debug(f'{self.build_root=}')
+        log.debug(f'{self.proto_include=}')
+
     @staticmethod
     def _get_basic_proto_path() -> str:
         if _PY_3_9_PLUS:
             from importlib import resources
             return str(resources.files('grpc_tools').joinpath('_proto'))
         else:
             import pkg_resources  # noqa
@@ -333,14 +338,15 @@
         m = strimp.get_module(protofile.pb2_module(), logger=log, reraise=True)
         if not m:
             log.error(f'protofile={protofile}')
             raise ImportError('ERROR! Module not found! %s' % protofile.pb2_module())
         else:
             try:
                 p = modules.ProtoModule(m)
+                log.debug(f' - Writing ProtoModule: {p.get_module_full_name()}')
                 p.write_rendered_file()
             except Exception as ex:
                 log.exception(f'ERROR! Bad stuff happened! %r' % ex)
                 raise
 
     def add_inits(self):
         log.debug('Adding __init__ files to generated modules...')
```

### Comparing `neobuilder-5.0.0b1/neobuilder/neobuilder/render/__init__.py` & `neobuilder-5.1.0/neobuilder/neobuilder/render/__init__.py`

 * *Files identical despite different names*

### Comparing `neobuilder-5.0.0b1/neobuilder/neobuilder/render/renderer.py` & `neobuilder-5.1.0/neobuilder/neobuilder/render/renderer.py`

 * *Files identical despite different names*

### Comparing `neobuilder-5.0.0b1/neobuilder/structs/protofile.py` & `neobuilder-5.1.0/neobuilder/structs/protofile.py`

 * *Files identical despite different names*

### Comparing `neobuilder-5.0.0b1/neobuilder/structs/pytype.py` & `neobuilder-5.1.0/neobuilder/structs/pytype.py`

 * *Files identical despite different names*

### Comparing `neobuilder-5.0.0b1/neobuilder.egg-info/PKG-INFO` & `neobuilder-5.1.0/neobuilder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neobuilder
-Version: 5.0.0b1
+Version: 5.1.0
 Summary: Builds Neobuf Packages from Protobuf files using Protoplasm! :D
 Author-email: Thordur Matthiasson <thordurm@ccpgames.com>
 License: MIT License
         
         Copyright (c) 2022-2024 CCP Games
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `neobuilder-5.0.0b1/neobuilder.egg-info/SOURCES.txt` & `neobuilder-5.1.0/neobuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neobuilder-5.0.0b1/pyproject.toml` & `neobuilder-5.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `neobuilder-5.0.0b1/tests/test_services.py` & `neobuilder-5.1.0/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `neobuilder-5.0.0b1/tests/test_zdataclassbuilder.py` & `neobuilder-5.1.0/tests/test_zdataclassbuilder.py`

 * *Files identical despite different names*

